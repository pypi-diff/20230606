# Comparing `tmp/a2-0.3.5.tar.gz` & `tmp/a2-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2-0.3.5.tar", max compression
+gzip compressed data, was "a2-0.3.6.tar", max compression
```

## Comparing `a2-0.3.5.tar` & `a2-0.3.6.tar`

### file list

```diff
@@ -1,1961 +1,56 @@
--rw-r--r--   0        0        0     3941 2023-06-06 15:55:03.871988 a2-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.5/src/a2/__init__.py
--rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.5/src/a2/cli/__init__.py
--rw-r--r--   0        0        0      200 2023-01-13 09:53:11.940626 a2-0.3.5/src/a2/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      297 2023-01-13 09:40:55.677429 a2-0.3.5/src/a2/cli/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.5/src/a2/cli/cli_plotting/__init__.py
--rw-r--r--   0        0        0      203 2023-01-13 09:53:11.952627 a2-0.3.5/src/a2/cli/cli_plotting/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      359 2023-01-13 09:53:14.892690 a2-0.3.5/src/a2/cli/cli_plotting/__pycache__/plot.cpython-310.pyc
--rw-r--r--   0        0        0     2101 2023-02-16 10:12:23.148895 a2-0.3.5/src/a2/cli/cli_plotting/__pycache__/single_plots.cpython-310.pyc
--rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.5/src/a2/cli/cli_plotting/plot.py
--rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.5/src/a2/cli/cli_plotting/single_plots.py
--rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.5/src/a2/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.5/src/a2/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.5/src/a2/data/emoji/__init__.py
--rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.5/src/a2/data/emoji/emoji_df.csv
--rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0023_fe0f_20e3.png
--rw-r--r--   0        0        0     1221 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/002a_fe0f_20e3.png
--rw-r--r--   0        0        0     1065 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0030_fe0f_20e3.png
--rw-r--r--   0        0        0      989 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0031_fe0f_20e3.png
--rw-r--r--   0        0        0     1043 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0032_fe0f_20e3.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0033_fe0f_20e3.png
--rw-r--r--   0        0        0     1077 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0034_fe0f_20e3.png
--rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0035_fe0f_20e3.png
--rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0036_fe0f_20e3.png
--rw-r--r--   0        0        0      985 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0037_fe0f_20e3.png
--rw-r--r--   0        0        0     1120 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0038_fe0f_20e3.png
--rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/0039_fe0f_20e3.png
--rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/00a9.png
--rw-r--r--   0        0        0     1091 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/00ae.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f004.png
--rw-r--r--   0        0        0     1141 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f0cf.png
--rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f170.png
--rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f171.png
--rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f17e.png
--rw-r--r--   0        0        0     1075 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f17f.png
--rw-r--r--   0        0        0     1342 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f18e.png
--rw-r--r--   0        0        0     1352 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f191.png
--rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f192.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f193.png
--rw-r--r--   0        0        0     1150 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f194.png
--rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f195.png
--rw-r--r--   0        0        0     1194 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f196.png
--rw-r--r--   0        0        0     1264 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f197.png
--rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f198.png
--rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f199.png
--rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f19a.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1e8.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1e9.png
--rw-r--r--   0        0        0     1245 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1ea.png
--rw-r--r--   0        0        0     1346 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1eb.png
--rw-r--r--   0        0        0     1555 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1ec.png
--rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1ee.png
--rw-r--r--   0        0        0     1206 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f1.png
--rw-r--r--   0        0        0     1444 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f2.png
--rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f4.png
--rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f6.png
--rw-r--r--   0        0        0     1193 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f7.png
--rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f8.png
--rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1f9.png
--rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1fa.png
--rw-r--r--   0        0        0     1379 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1fc.png
--rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1fd.png
--rw-r--r--   0        0        0     1592 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e6_1f1ff.png
--rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1e6.png
--rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1e7.png
--rw-r--r--   0        0        0      935 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1e9.png
--rw-r--r--   0        0        0      998 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1ea.png
--rw-r--r--   0        0        0     1253 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1eb.png
--rw-r--r--   0        0        0     1348 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1ec.png
--rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1ed.png
--rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1ee.png
--rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1ef.png
--rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f1.png
--rw-r--r--   0        0        0     2553 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f2.png
--rw-r--r--   0        0        0     2134 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f3.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f4.png
--rw-r--r--   0        0        0     1467 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f6.png
--rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f7.png
--rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f8.png
--rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1f9.png
--rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1fb.png
--rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1fc.png
--rw-r--r--   0        0        0     1417 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1fe.png
--rw-r--r--   0        0        0     2195 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e7_1f1ff.png
--rw-r--r--   0        0        0     1263 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1e6.png
--rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1e8.png
--rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1e9.png
--rw-r--r--   0        0        0     1831 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1eb.png
--rw-r--r--   0        0        0     1460 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1ec.png
--rw-r--r--   0        0        0      879 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1ed.png
--rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1ee.png
--rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f0.png
--rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f1.png
--rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f2.png
--rw-r--r--   0        0        0     1055 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f3.png
--rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f4.png
--rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f5.png
--rw-r--r--   0        0        0     1521 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1f7.png
--rw-r--r--   0        0        0     1609 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1fa.png
--rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1fb.png
--rw-r--r--   0        0        0     1215 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1fc.png
--rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1fd.png
--rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1fe.png
--rw-r--r--   0        0        0     1236 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e8_1f1ff.png
--rw-r--r--   0        0        0     1280 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1ea.png
--rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1ec.png
--rw-r--r--   0        0        0     1331 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1ef.png
--rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1f0.png
--rw-r--r--   0        0        0     2283 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1f2.png
--rw-r--r--   0        0        0     1737 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1f4.png
--rw-r--r--   0        0        0     1324 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1e9_1f1ff.png
--rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1e6.png
--rw-r--r--   0        0        0     1976 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1e8.png
--rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1ea.png
--rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1ec.png
--rw-r--r--   0        0        0     1270 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1ed.png
--rw-r--r--   0        0        0     1719 2022-11-18 15:36:28.436585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1f7.png
--rw-r--r--   0        0        0     1513 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1f8.png
--rw-r--r--   0        0        0     1477 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1f9.png
--rw-r--r--   0        0        0      969 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ea_1f1fa.png
--rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1eb_1f1ee.png
--rw-r--r--   0        0        0     2421 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1eb_1f1ef.png
--rw-r--r--   0        0        0     2067 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1eb_1f1f0.png
--rw-r--r--   0        0        0     1005 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1eb_1f1f2.png
--rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1eb_1f1f4.png
--rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1eb_1f1f7.png
--rw-r--r--   0        0        0     1362 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1e6.png
--rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1e7.png
--rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1e9.png
--rw-r--r--   0        0        0     1583 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1ea.png
--rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1eb.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1ec.png
--rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1ed.png
--rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1ee.png
--rw-r--r--   0        0        0     1202 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f1.png
--rw-r--r--   0        0        0     1570 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f2.png
--rw-r--r--   0        0        0     1023 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f3.png
--rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f5.png
--rw-r--r--   0        0        0     1641 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f6.png
--rw-r--r--   0        0        0     1677 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f7.png
--rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f8.png
--rw-r--r--   0        0        0     1224 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1f9.png
--rw-r--r--   0        0        0     1354 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1fa.png
--rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1fc.png
--rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ec_1f1fe.png
--rw-r--r--   0        0        0     1138 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ed_1f1f0.png
--rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ed_1f1f2.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ed_1f1f3.png
--rw-r--r--   0        0        0     1843 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ed_1f1f7.png
--rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ed_1f1f9.png
--rw-r--r--   0        0        0     1317 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ed_1f1fa.png
--rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1e8.png
--rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1e9.png
--rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1ea.png
--rw-r--r--   0        0        0     1453 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f1.png
--rw-r--r--   0        0        0     1135 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f2.png
--rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f3.png
--rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f4.png
--rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f6.png
--rw-r--r--   0        0        0     1566 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f7.png
--rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f8.png
--rw-r--r--   0        0        0      995 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ee_1f1f9.png
--rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ef_1f1ea.png
--rw-r--r--   0        0        0     1536 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ef_1f1f2.png
--rw-r--r--   0        0        0     1361 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ef_1f1f4.png
--rw-r--r--   0        0        0     1019 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ef_1f1f5.png
--rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1ea.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1ec.png
--rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1ed.png
--rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1ee.png
--rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1f2.png
--rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1f3.png
--rw-r--r--   0        0        0     1552 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1f5.png
--rw-r--r--   0        0        0     1531 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1f7.png
--rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1fc.png
--rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1fe.png
--rw-r--r--   0        0        0     1473 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f0_1f1ff.png
--rw-r--r--   0        0        0     1229 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1e6.png
--rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1e7.png
--rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1e8.png
--rw-r--r--   0        0        0     1314 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1ee.png
--rw-r--r--   0        0        0     1483 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1f0.png
--rw-r--r--   0        0        0     1995 2022-11-18 15:36:28.440585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1f7.png
--rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1f8.png
--rw-r--r--   0        0        0     1333 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1f9.png
--rw-r--r--   0        0        0     1363 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1fa.png
--rw-r--r--   0        0        0     1056 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1fb.png
--rw-r--r--   0        0        0     1336 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f1_1f1fe.png
--rw-r--r--   0        0        0     1158 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1e6.png
--rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1e8.png
--rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1e9.png
--rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1ea.png
--rw-r--r--   0        0        0     1073 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1eb.png
--rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1ec.png
--rw-r--r--   0        0        0     1577 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1ed.png
--rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f0.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f1.png
--rw-r--r--   0        0        0     1574 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f2.png
--rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f3.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f4.png
--rw-r--r--   0        0        0     1791 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f5.png
--rw-r--r--   0        0        0     1505 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f6.png
--rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f7.png
--rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f8.png
--rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1f9.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1fa.png
--rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1fb.png
--rw-r--r--   0        0        0     1364 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1fc.png
--rw-r--r--   0        0        0     1311 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1fd.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1fe.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f2_1f1ff.png
--rw-r--r--   0        0        0     1835 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1e6.png
--rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1e8.png
--rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1ea.png
--rw-r--r--   0        0        0     1149 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1eb.png
--rw-r--r--   0        0        0      881 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1ec.png
--rw-r--r--   0        0        0     1377 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1ee.png
--rw-r--r--   0        0        0     1234 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1f1.png
--rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1f4.png
--rw-r--r--   0        0        0      999 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1f5.png
--rw-r--r--   0        0        0     1148 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1f7.png
--rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1fa.png
--rw-r--r--   0        0        0     1683 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f3_1f1ff.png
--rw-r--r--   0        0        0     1419 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f4_1f1f2.png
--rw-r--r--   0        0        0     1550 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1e6.png
--rw-r--r--   0        0        0      977 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1ea.png
--rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1eb.png
--rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1ec.png
--rw-r--r--   0        0        0     1695 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1ed.png
--rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f0.png
--rw-r--r--   0        0        0     1040 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f1.png
--rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f2.png
--rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f3.png
--rw-r--r--   0        0        0     1622 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f7.png
--rw-r--r--   0        0        0     1211 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f8.png
--rw-r--r--   0        0        0     1590 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1f9.png
--rw-r--r--   0        0        0     1022 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1fc.png
--rw-r--r--   0        0        0     1607 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f5_1f1fe.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f6_1f1e6.png
--rw-r--r--   0        0        0     1792 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f7_1f1ea.png
--rw-r--r--   0        0        0      954 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f7_1f1f4.png
--rw-r--r--   0        0        0     1872 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f7_1f1f8.png
--rw-r--r--   0        0        0     1298 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f7_1f1fa.png
--rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f7_1f1fc.png
--rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1e6.png
--rw-r--r--   0        0        0     1729 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1e7.png
--rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1e8.png
--rw-r--r--   0        0        0     1203 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1e9.png
--rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1ea.png
--rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1ec.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1ed.png
--rw-r--r--   0        0        0     1613 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1ee.png
--rw-r--r--   0        0        0     1658 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1ef.png
--rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f0.png
--rw-r--r--   0        0        0     1411 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f1.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.444585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f2.png
--rw-r--r--   0        0        0     1228 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f3.png
--rw-r--r--   0        0        0      884 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f4.png
--rw-r--r--   0        0        0     1557 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f7.png
--rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f8.png
--rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1f9.png
--rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1fb.png
--rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1fd.png
--rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1fe.png
--rw-r--r--   0        0        0     2344 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f8_1f1ff.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1e6.png
--rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1e8.png
--rw-r--r--   0        0        0      968 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1e9.png
--rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1eb.png
--rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1ec.png
--rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1ed.png
--rw-r--r--   0        0        0     1440 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1ef.png
--rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f0.png
--rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f1.png
--rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f2.png
--rw-r--r--   0        0        0     1118 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f3.png
--rw-r--r--   0        0        0     1163 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f4.png
--rw-r--r--   0        0        0     1213 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f7.png
--rw-r--r--   0        0        0     1448 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1f9.png
--rw-r--r--   0        0        0     2227 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1fb.png
--rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1fc.png
--rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1f9_1f1ff.png
--rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1e6.png
--rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1ec.png
--rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1f2.png
--rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1f3.png
--rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1f8.png
--rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1fe.png
--rw-r--r--   0        0        0     1743 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fa_1f1ff.png
--rw-r--r--   0        0        0     1197 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1e6.png
--rw-r--r--   0        0        0     1337 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1e8.png
--rw-r--r--   0        0        0     1580 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1ea.png
--rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1ec.png
--rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1ee.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1f3.png
--rw-r--r--   0        0        0     1594 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fb_1f1fa.png
--rw-r--r--   0        0        0     1319 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fc_1f1eb.png
--rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fc_1f1f8.png
--rw-r--r--   0        0        0     1128 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fd_1f1f0.png
--rw-r--r--   0        0        0     1184 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fe_1f1ea.png
--rw-r--r--   0        0        0     1649 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1fe_1f1f9.png
--rw-r--r--   0        0        0     2075 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ff_1f1e6.png
--rw-r--r--   0        0        0     1071 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ff_1f1f2.png
--rw-r--r--   0        0        0     2394 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f1ff_1f1fc.png
--rw-r--r--   0        0        0     1081 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f201.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f202.png
--rw-r--r--   0        0        0     1478 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f21a.png
--rw-r--r--   0        0        0     1514 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f22f.png
--rw-r--r--   0        0        0     1682 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f232.png
--rw-r--r--   0        0        0     1372 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f233.png
--rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f234.png
--rw-r--r--   0        0        0     1667 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f235.png
--rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f236.png
--rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f237.png
--rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f238.png
--rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f239.png
--rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f23a.png
--rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f250.png
--rw-r--r--   0        0        0     1181 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f251.png
--rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f300.png
--rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f301.png
--rw-r--r--   0        0        0     1753 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f302.png
--rw-r--r--   0        0        0     2162 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f303.png
--rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f304.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f305.png
--rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f306.png
--rw-r--r--   0        0        0     2397 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f307.png
--rw-r--r--   0        0        0     3358 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f308.png
--rw-r--r--   0        0        0     1972 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f309.png
--rw-r--r--   0        0        0     2761 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f30a.png
--rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f30b.png
--rw-r--r--   0        0        0     1639 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f30c.png
--rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f30d.png
--rw-r--r--   0        0        0     3347 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f30e.png
--rw-r--r--   0        0        0     3956 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f30f.png
--rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f310.png
--rw-r--r--   0        0        0     1274 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f311.png
--rw-r--r--   0        0        0     2102 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f312.png
--rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f313.png
--rw-r--r--   0        0        0     2310 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f314.png
--rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f315.png
--rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f316.png
--rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f317.png
--rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f318.png
--rw-r--r--   0        0        0     1394 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f319.png
--rw-r--r--   0        0        0     1551 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f31a.png
--rw-r--r--   0        0        0     1589 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f31b.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f31c.png
--rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f31d.png
--rw-r--r--   0        0        0     3537 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f31e.png
--rw-r--r--   0        0        0     1898 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f31f.png
--rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f320.png
--rw-r--r--   0        0        0     1925 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f321.png
--rw-r--r--   0        0        0     1971 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f324.png
--rw-r--r--   0        0        0     1326 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f325.png
--rw-r--r--   0        0        0     2070 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f326.png
--rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f327.png
--rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f328.png
--rw-r--r--   0        0        0     1323 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f329.png
--rw-r--r--   0        0        0     2338 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f32a.png
--rw-r--r--   0        0        0     1345 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f32b.png
--rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f32c.png
--rw-r--r--   0        0        0     2143 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f32d.png
--rw-r--r--   0        0        0     3164 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f32e.png
--rw-r--r--   0        0        0     2846 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f32f.png
--rw-r--r--   0        0        0     2278 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f330.png
--rw-r--r--   0        0        0     1332 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f331.png
--rw-r--r--   0        0        0     2597 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f332.png
--rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f333.png
--rw-r--r--   0        0        0     3072 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f334.png
--rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f335.png
--rw-r--r--   0        0        0     1845 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f336.png
--rw-r--r--   0        0        0     3135 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f337.png
--rw-r--r--   0        0        0     3604 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f338.png
--rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f339.png
--rw-r--r--   0        0        0     3826 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f33a.png
--rw-r--r--   0        0        0     2868 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f33b.png
--rw-r--r--   0        0        0     2956 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f33c.png
--rw-r--r--   0        0        0     3578 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f33d.png
--rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f33e.png
--rw-r--r--   0        0        0     2049 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f33f.png
--rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f340.png
--rw-r--r--   0        0        0     2961 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f341.png
--rw-r--r--   0        0        0     2139 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f342.png
--rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f343.png
--rw-r--r--   0        0        0     2132 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f344.png
--rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f345.png
--rw-r--r--   0        0        0     1652 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f346.png
--rw-r--r--   0        0        0     3397 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f347.png
--rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f348.png
--rw-r--r--   0        0        0     1901 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f349.png
--rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f34a.png
--rw-r--r--   0        0        0     2346 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f34b.png
--rw-r--r--   0        0        0     2330 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f34c.png
--rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f34d.png
--rw-r--r--   0        0        0     2045 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f34e.png
--rw-r--r--   0        0        0     1960 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f34f.png
--rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f350.png
--rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f351.png
--rw-r--r--   0        0        0     2440 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f352.png
--rw-r--r--   0        0        0     3080 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f353.png
--rw-r--r--   0        0        0     3804 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f354.png
--rw-r--r--   0        0        0     2094 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f355.png
--rw-r--r--   0        0        0     2512 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f356.png
--rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f357.png
--rw-r--r--   0        0        0     2273 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f358.png
--rw-r--r--   0        0        0     2050 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f359.png
--rw-r--r--   0        0        0     1857 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f35a.png
--rw-r--r--   0        0        0     2172 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f35b.png
--rw-r--r--   0        0        0     3130 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f35c.png
--rw-r--r--   0        0        0     2982 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f35d.png
--rw-r--r--   0        0        0     1849 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f35e.png
--rw-r--r--   0        0        0     2730 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f35f.png
--rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f360.png
--rw-r--r--   0        0        0     2058 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f361.png
--rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f362.png
--rw-r--r--   0        0        0     2825 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f363.png
--rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f364.png
--rw-r--r--   0        0        0     1761 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f365.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f366.png
--rw-r--r--   0        0        0     2335 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f367.png
--rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f368.png
--rw-r--r--   0        0        0     4358 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f369.png
--rw-r--r--   0        0        0     2375 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f36a.png
--rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f36b.png
--rw-r--r--   0        0        0     2528 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f36c.png
--rw-r--r--   0        0        0     2993 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f36d.png
--rw-r--r--   0        0        0     1876 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f36e.png
--rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f36f.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f370.png
--rw-r--r--   0        0        0     4187 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f371.png
--rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f372.png
--rw-r--r--   0        0        0     2053 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f373.png
--rw-r--r--   0        0        0     1571 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f374.png
--rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f375.png
--rw-r--r--   0        0        0     1653 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f376.png
--rw-r--r--   0        0        0     1820 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f377.png
--rw-r--r--   0        0        0     2130 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f378.png
--rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f379.png
--rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f37a.png
--rw-r--r--   0        0        0     3070 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f37b.png
--rw-r--r--   0        0        0     1840 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f37c.png
--rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f37d.png
--rw-r--r--   0        0        0     2490 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f37e.png
--rw-r--r--   0        0        0     3063 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f37f.png
--rw-r--r--   0        0        0     2216 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f380.png
--rw-r--r--   0        0        0     2290 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f381.png
--rw-r--r--   0        0        0     2452 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f382.png
--rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f383.png
--rw-r--r--   0        0        0     3064 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f384.png
--rw-r--r--   0        0        0     3193 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f385.png
--rw-r--r--   0        0        0     2478 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f386.png
--rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f387.png
--rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f388.png
--rw-r--r--   0        0        0     3725 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f389.png
--rw-r--r--   0        0        0     3748 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f38a.png
--rw-r--r--   0        0        0     2909 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f38b.png
--rw-r--r--   0        0        0     2120 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f38c.png
--rw-r--r--   0        0        0     2268 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f38d.png
--rw-r--r--   0        0        0     3885 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f38e.png
--rw-r--r--   0        0        0    13409 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f38f.png
--rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f390.png
--rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f391.png
--rw-r--r--   0        0        0     2593 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f392.png
--rw-r--r--   0        0        0     1595 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f393.png
--rw-r--r--   0        0        0     1673 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f396.png
--rw-r--r--   0        0        0     1273 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f397.png
--rw-r--r--   0        0        0     2738 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f399.png
--rw-r--r--   0        0        0     1254 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f39a.png
--rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f39b.png
--rw-r--r--   0        0        0     2621 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f39e.png
--rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f39f.png
--rw-r--r--   0        0        0     3774 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a0.png
--rw-r--r--   0        0        0     3756 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a1.png
--rw-r--r--   0        0        0     2888 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a2.png
--rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a3.png
--rw-r--r--   0        0        0     1510 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a4.png
--rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a5.png
--rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a6.png
--rw-r--r--   0        0        0     2400 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a7.png
--rw-r--r--   0        0        0     3744 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a8.png
--rw-r--r--   0        0        0     1380 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3a9.png
--rw-r--r--   0        0        0     3014 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3aa.png
--rw-r--r--   0        0        0     1519 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ab.png
--rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ac.png
--rw-r--r--   0        0        0     3610 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ad.png
--rw-r--r--   0        0        0     2008 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ae.png
--rw-r--r--   0        0        0     2799 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3af.png
--rw-r--r--   0        0        0     2850 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b0.png
--rw-r--r--   0        0        0     1685 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b1.png
--rw-r--r--   0        0        0     1690 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b2.png
--rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b3.png
--rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b4.png
--rw-r--r--   0        0        0      989 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b5.png
--rw-r--r--   0        0        0     1731 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b6.png
--rw-r--r--   0        0        0     2673 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b7.png
--rw-r--r--   0        0        0     2595 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b8.png
--rw-r--r--   0        0        0     1147 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3b9.png
--rw-r--r--   0        0        0     3202 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ba.png
--rw-r--r--   0        0        0     3440 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3bb.png
--rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3bc.png
--rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3bd.png
--rw-r--r--   0        0        0     2114 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3be.png
--rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3bf.png
--rw-r--r--   0        0        0     3092 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c0.png
--rw-r--r--   0        0        0     1384 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c1.png
--rw-r--r--   0        0        0     3205 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c2.png
--rw-r--r--   0        0        0     2226 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c3.png
--rw-r--r--   0        0        0     2518 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c3_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2449 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c3_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3228 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c4.png
--rw-r--r--   0        0        0     3265 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c4_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c4_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2901 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c5.png
--rw-r--r--   0        0        0     2765 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c6.png
--rw-r--r--   0        0        0     2834 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c7.png
--rw-r--r--   0        0        0     2681 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c8.png
--rw-r--r--   0        0        0     2430 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3c9.png
--rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ca.png
--rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ca_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2879 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ca_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3446 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cb.png
--rw-r--r--   0        0        0     3400 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3505 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cb_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cc.png
--rw-r--r--   0        0        0     2502 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cc_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cd.png
--rw-r--r--   0        0        0     2826 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ce.png
--rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3cf.png
--rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d0.png
--rw-r--r--   0        0        0     1866 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d1.png
--rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d2.png
--rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d3.png
--rw-r--r--   0        0        0     3018 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d4.png
--rw-r--r--   0        0        0     2698 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d5.png
--rw-r--r--   0        0        0     3183 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d6.png
--rw-r--r--   0        0        0     3121 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d7.png
--rw-r--r--   0        0        0     3021 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d8.png
--rw-r--r--   0        0        0     1628 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3d9.png
--rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3da.png
--rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3db.png
--rw-r--r--   0        0        0     3123 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3dc.png
--rw-r--r--   0        0        0     3133 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3dd.png
--rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3de.png
--rw-r--r--   0        0        0     4049 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3df.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e0.png
--rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e1.png
--rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e2.png
--rw-r--r--   0        0        0     2318 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e3.png
--rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e4.png
--rw-r--r--   0        0        0     1880 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e5.png
--rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e6.png
--rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e7.png
--rw-r--r--   0        0        0     2990 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e8.png
--rw-r--r--   0        0        0     3226 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3e9.png
--rw-r--r--   0        0        0     2202 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ea.png
--rw-r--r--   0        0        0     2239 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3eb.png
--rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ec.png
--rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ed.png
--rw-r--r--   0        0        0     1482 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ee.png
--rw-r--r--   0        0        0     2396 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3ef.png
--rw-r--r--   0        0        0     3103 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f0.png
--rw-r--r--   0        0        0      848 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f3.png
--rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_1f308.png
--rw-r--r--   0        0        0     1389 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f3_fe0f_200d_26a7_fe0f.png
--rw-r--r--   0        0        0      761 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f4.png
--rw-r--r--   0        0        0     1096 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f4_200d_2620_fe0f.png
--rw-r--r--   0        0        0     1283 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0065_e006e_e0067_e007f.png
--rw-r--r--   0        0        0     1451 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0073_e0063_e0074_e007f.png
--rw-r--r--   0        0        0     2115 2022-11-18 15:36:28.448585 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f4_e0067_e0062_e0077_e006c_e0073_e007f.png
--rw-r--r--   0        0        0     4095 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f5.png
--rw-r--r--   0        0        0      495 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f7.png
--rw-r--r--   0        0        0     3310 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f8.png
--rw-r--r--   0        0        0     2605 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3f9.png
--rw-r--r--   0        0        0     2936 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f3fa.png
--rw-r--r--   0        0        0     1698 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f400.png
--rw-r--r--   0        0        0     2505 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f401.png
--rw-r--r--   0        0        0     1710 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f402.png
--rw-r--r--   0        0        0     1549 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f403.png
--rw-r--r--   0        0        0     2271 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f404.png
--rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f405.png
--rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f406.png
--rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f407.png
--rw-r--r--   0        0        0     2893 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f408.png
--rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f408_200d_2b1b.png
--rw-r--r--   0        0        0     4191 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f409.png
--rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f40a.png
--rw-r--r--   0        0        0     2014 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f40b.png
--rw-r--r--   0        0        0     3036 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f40c.png
--rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f40d.png
--rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f40e.png
--rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f40f.png
--rw-r--r--   0        0        0     1862 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f410.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f411.png
--rw-r--r--   0        0        0     2556 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f412.png
--rw-r--r--   0        0        0     2453 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f413.png
--rw-r--r--   0        0        0     2304 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f414.png
--rw-r--r--   0        0        0     2328 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f415.png
--rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f415_200d_1f9ba.png
--rw-r--r--   0        0        0     1591 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f416.png
--rw-r--r--   0        0        0     1773 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f417.png
--rw-r--r--   0        0        0     1699 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f418.png
--rw-r--r--   0        0        0     2151 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f419.png
--rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f41a.png
--rw-r--r--   0        0        0     3478 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f41b.png
--rw-r--r--   0        0        0     2245 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f41c.png
--rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f41d.png
--rw-r--r--   0        0        0     3427 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f41e.png
--rw-r--r--   0        0        0     1868 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f41f.png
--rw-r--r--   0        0        0     3171 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f420.png
--rw-r--r--   0        0        0     3511 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f421.png
--rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f422.png
--rw-r--r--   0        0        0     2750 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f423.png
--rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f424.png
--rw-r--r--   0        0        0     2506 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f425.png
--rw-r--r--   0        0        0     1535 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f426.png
--rw-r--r--   0        0        0     1612 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f427.png
--rw-r--r--   0        0        0     1805 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f428.png
--rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f429.png
--rw-r--r--   0        0        0     1655 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f42a.png
--rw-r--r--   0        0        0     2229 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f42b.png
--rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f42c.png
--rw-r--r--   0        0        0     2063 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f42d.png
--rw-r--r--   0        0        0     2011 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f42e.png
--rw-r--r--   0        0        0     3152 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f42f.png
--rw-r--r--   0        0        0     1994 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f430.png
--rw-r--r--   0        0        0     2193 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f431.png
--rw-r--r--   0        0        0     4538 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f432.png
--rw-r--r--   0        0        0     2468 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f433.png
--rw-r--r--   0        0        0     2249 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f434.png
--rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f435.png
--rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f436.png
--rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f437.png
--rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f438.png
--rw-r--r--   0        0        0     2911 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f439.png
--rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43a.png
--rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43b.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43b_200d_2744_fe0f.png
--rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43c.png
--rw-r--r--   0        0        0     1528 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43d.png
--rw-r--r--   0        0        0      771 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43e.png
--rw-r--r--   0        0        0     3248 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f43f.png
--rw-r--r--   0        0        0     1237 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f440.png
--rw-r--r--   0        0        0     2158 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f441.png
--rw-r--r--   0        0        0     1409 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f441_fe0f_200d_1f5e8_fe0f.png
--rw-r--r--   0        0        0     1291 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f442.png
--rw-r--r--   0        0        0     1094 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f443.png
--rw-r--r--   0        0        0     1491 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f444.png
--rw-r--r--   0        0        0     1666 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f445.png
--rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f446.png
--rw-r--r--   0        0        0     1039 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f447.png
--rw-r--r--   0        0        0      972 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f448.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f449.png
--rw-r--r--   0        0        0     1180 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f44a.png
--rw-r--r--   0        0        0     1977 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f44b.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f44c.png
--rw-r--r--   0        0        0     1454 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f44d.png
--rw-r--r--   0        0        0     1423 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f44e.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f44f.png
--rw-r--r--   0        0        0     1459 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f450.png
--rw-r--r--   0        0        0     3262 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f451.png
--rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f452.png
--rw-r--r--   0        0        0     1157 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f453.png
--rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f454.png
--rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f455.png
--rw-r--r--   0        0        0     2568 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f456.png
--rw-r--r--   0        0        0     1811 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f457.png
--rw-r--r--   0        0        0     3086 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f458.png
--rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f459.png
--rw-r--r--   0        0        0     1671 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f45a.png
--rw-r--r--   0        0        0     1638 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f45b.png
--rw-r--r--   0        0        0     2326 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f45c.png
--rw-r--r--   0        0        0     1758 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f45d.png
--rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f45e.png
--rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f45f.png
--rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f460.png
--rw-r--r--   0        0        0     1465 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f461.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f462.png
--rw-r--r--   0        0        0      806 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f463.png
--rw-r--r--   0        0        0      905 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f464.png
--rw-r--r--   0        0        0     1012 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f465.png
--rw-r--r--   0        0        0     2126 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f466.png
--rw-r--r--   0        0        0     2215 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f467.png
--rw-r--r--   0        0        0     2023 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468.png
--rw-r--r--   0        0        0     4097 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f33e.png
--rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f373.png
--rw-r--r--   0        0        0     2948 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f37c.png
--rw-r--r--   0        0        0     2403 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f393.png
--rw-r--r--   0        0        0     3325 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f3a4.png
--rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f3a8.png
--rw-r--r--   0        0        0     2669 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f3eb.png
--rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f3ed.png
--rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f466.png
--rw-r--r--   0        0        0     2694 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     2644 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f467.png
--rw-r--r--   0        0        0     3625 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     3062 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     3524 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466.png
--rw-r--r--   0        0        0     4079 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     3727 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467.png
--rw-r--r--   0        0        0     4567 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     4614 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f468_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     3437 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466.png
--rw-r--r--   0        0        0     4310 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     3696 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467.png
--rw-r--r--   0        0        0     4734 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     4600 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f469_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f4bb.png
--rw-r--r--   0        0        0     2409 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f4bc.png
--rw-r--r--   0        0        0     3178 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f527.png
--rw-r--r--   0        0        0     3350 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f52c.png
--rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f680.png
--rw-r--r--   0        0        0     3740 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f692.png
--rw-r--r--   0        0        0     2564 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9af.png
--rw-r--r--   0        0        0     2081 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9b0.png
--rw-r--r--   0        0        0     2301 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9b1.png
--rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9b2.png
--rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9b3.png
--rw-r--r--   0        0        0     3029 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9bc.png
--rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_1f9bd.png
--rw-r--r--   0        0        0     2561 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_2695_fe0f.png
--rw-r--r--   0        0        0     2680 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_2696_fe0f.png
--rw-r--r--   0        0        0     2660 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_2708_fe0f.png
--rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f468.png
--rw-r--r--   0        0        0     2437 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f468_200d_2764_fe0f_200d_1f48b_200d_1f468.png
--rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469.png
--rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f33e.png
--rw-r--r--   0        0        0     3312 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f373.png
--rw-r--r--   0        0        0     2951 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f37c.png
--rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f393.png
--rw-r--r--   0        0        0     3648 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f3a4.png
--rw-r--r--   0        0        0     3778 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f3a8.png
--rw-r--r--   0        0        0     2988 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f3eb.png
--rw-r--r--   0        0        0     3394 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f3ed.png
--rw-r--r--   0        0        0     2519 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f466.png
--rw-r--r--   0        0        0     2793 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f467.png
--rw-r--r--   0        0        0     3700 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     3363 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466.png
--rw-r--r--   0        0        0     3984 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f466_200d_1f466.png
--rw-r--r--   0        0        0     3860 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467.png
--rw-r--r--   0        0        0     4626 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f466.png
--rw-r--r--   0        0        0     4582 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f469_200d_1f467_200d_1f467.png
--rw-r--r--   0        0        0     2002 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f4bb.png
--rw-r--r--   0        0        0     2411 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f4bc.png
--rw-r--r--   0        0        0     3131 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f527.png
--rw-r--r--   0        0        0     3659 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f52c.png
--rw-r--r--   0        0        0     3150 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f680.png
--rw-r--r--   0        0        0     3773 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f692.png
--rw-r--r--   0        0        0     2532 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9af.png
--rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9b0.png
--rw-r--r--   0        0        0     2744 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9b1.png
--rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9b2.png
--rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9b3.png
--rw-r--r--   0        0        0     3044 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9bc.png
--rw-r--r--   0        0        0     2575 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_1f9bd.png
--rw-r--r--   0        0        0     2722 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2695_fe0f.png
--rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2696_fe0f.png
--rw-r--r--   0        0        0     2931 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2708_fe0f.png
--rw-r--r--   0        0        0     3634 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f468.png
--rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f469.png
--rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f468.png
--rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f469_200d_2764_fe0f_200d_1f48b_200d_1f469.png
--rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46a.png
--rw-r--r--   0        0        0     3563 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46b.png
--rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46c.png
--rw-r--r--   0        0        0     3729 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46d.png
--rw-r--r--   0        0        0     3074 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46e.png
--rw-r--r--   0        0        0     3026 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46e_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3184 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46e_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46f.png
--rw-r--r--   0        0        0     3282 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f46f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2859 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f470.png
--rw-r--r--   0        0        0     2914 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f470_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2994 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f470_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2408 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f471.png
--rw-r--r--   0        0        0     2558 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f471_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f471_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2225 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f472.png
--rw-r--r--   0        0        0     2279 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f473.png
--rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f473_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f473_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2160 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f474.png
--rw-r--r--   0        0        0     2445 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f475.png
--rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f476.png
--rw-r--r--   0        0        0     3221 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f477.png
--rw-r--r--   0        0        0     3455 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f477_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3157 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f477_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2492 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f478.png
--rw-r--r--   0        0        0     3442 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f479.png
--rw-r--r--   0        0        0     2863 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f47a.png
--rw-r--r--   0        0        0     2131 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f47b.png
--rw-r--r--   0        0        0     2657 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f47c.png
--rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f47d.png
--rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f47e.png
--rw-r--r--   0        0        0     2312 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f47f.png
--rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f480.png
--rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f481.png
--rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f481_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2232 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f481_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f482.png
--rw-r--r--   0        0        0     2451 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f482_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2572 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f482_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3554 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f483.png
--rw-r--r--   0        0        0     1511 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f484.png
--rw-r--r--   0        0        0     2498 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f485.png
--rw-r--r--   0        0        0     2577 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f486.png
--rw-r--r--   0        0        0     2578 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f486_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f486_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2902 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f487.png
--rw-r--r--   0        0        0     3136 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f487_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2768 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f487_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2127 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f488.png
--rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f489.png
--rw-r--r--   0        0        0     2073 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f48a.png
--rw-r--r--   0        0        0     2182 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f48b.png
--rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f48c.png
--rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f48d.png
--rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f48e.png
--rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f48f.png
--rw-r--r--   0        0        0    13813 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f490.png
--rw-r--r--   0        0        0     3493 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f491.png
--rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f492.png
--rw-r--r--   0        0        0     1344 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f493.png
--rw-r--r--   0        0        0     1561 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f494.png
--rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f495.png
--rw-r--r--   0        0        0     2111 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f496.png
--rw-r--r--   0        0        0     1760 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f497.png
--rw-r--r--   0        0        0     1985 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f498.png
--rw-r--r--   0        0        0     1130 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f499.png
--rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f49a.png
--rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f49b.png
--rw-r--r--   0        0        0     1112 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f49c.png
--rw-r--r--   0        0        0     2849 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f49d.png
--rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f49e.png
--rw-r--r--   0        0        0     1082 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f49f.png
--rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a0.png
--rw-r--r--   0        0        0     1218 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a1.png
--rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a2.png
--rw-r--r--   0        0        0     2163 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a3.png
--rw-r--r--   0        0        0      663 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a4.png
--rw-r--r--   0        0        0     2101 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a5.png
--rw-r--r--   0        0        0     1905 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a6.png
--rw-r--r--   0        0        0     1268 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a7.png
--rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a8.png
--rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4a9.png
--rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4aa.png
--rw-r--r--   0        0        0     1890 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ab.png
--rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ac.png
--rw-r--r--   0        0        0     1370 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ad.png
--rw-r--r--   0        0        0     1790 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ae.png
--rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4af.png
--rw-r--r--   0        0        0     2079 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b0.png
--rw-r--r--   0        0        0      996 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b1.png
--rw-r--r--   0        0        0      731 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b2.png
--rw-r--r--   0        0        0     1261 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b3.png
--rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b4.png
--rw-r--r--   0        0        0     2022 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b5.png
--rw-r--r--   0        0        0     2210 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b6.png
--rw-r--r--   0        0        0     1974 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b7.png
--rw-r--r--   0        0        0     3067 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b8.png
--rw-r--r--   0        0        0     1480 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4b9.png
--rw-r--r--   0        0        0     2448 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ba.png
--rw-r--r--   0        0        0     1176 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4bb.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4bc.png
--rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4bd.png
--rw-r--r--   0        0        0      907 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4be.png
--rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4bf.png
--rw-r--r--   0        0        0     2307 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c0.png
--rw-r--r--   0        0        0     1335 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c1.png
--rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c2.png
--rw-r--r--   0        0        0     1241 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c3.png
--rw-r--r--   0        0        0     1257 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c4.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c5.png
--rw-r--r--   0        0        0     1568 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c6.png
--rw-r--r--   0        0        0     2054 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c7.png
--rw-r--r--   0        0        0     1861 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c8.png
--rw-r--r--   0        0        0     1762 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4c9.png
--rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ca.png
--rw-r--r--   0        0        0     1189 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4cb.png
--rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4cc.png
--rw-r--r--   0        0        0     1466 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4cd.png
--rw-r--r--   0        0        0     2382 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ce.png
--rw-r--r--   0        0        0      803 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4cf.png
--rw-r--r--   0        0        0      935 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d0.png
--rw-r--r--   0        0        0     1723 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d1.png
--rw-r--r--   0        0        0     2351 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d2.png
--rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d3.png
--rw-r--r--   0        0        0     1766 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d4.png
--rw-r--r--   0        0        0     1593 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d5.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d6.png
--rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d7.png
--rw-r--r--   0        0        0     1661 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d8.png
--rw-r--r--   0        0        0     1807 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4d9.png
--rw-r--r--   0        0        0     2567 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4da.png
--rw-r--r--   0        0        0     1381 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4db.png
--rw-r--r--   0        0        0     2294 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4dc.png
--rw-r--r--   0        0        0     2169 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4dd.png
--rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4de.png
--rw-r--r--   0        0        0     1650 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4df.png
--rw-r--r--   0        0        0     1045 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e0.png
--rw-r--r--   0        0        0     2446 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e1.png
--rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e2.png
--rw-r--r--   0        0        0     2230 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e3.png
--rw-r--r--   0        0        0     1412 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e4.png
--rw-r--r--   0        0        0     1396 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e5.png
--rw-r--r--   0        0        0     1493 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e6.png
--rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e7.png
--rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e8.png
--rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4e9.png
--rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ea.png
--rw-r--r--   0        0        0     2096 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4eb.png
--rw-r--r--   0        0        0     2146 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ec.png
--rw-r--r--   0        0        0     1703 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ed.png
--rw-r--r--   0        0        0     1507 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ee.png
--rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ef.png
--rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f0.png
--rw-r--r--   0        0        0     1517 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f1.png
--rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f2.png
--rw-r--r--   0        0        0     1436 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f3.png
--rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f4.png
--rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f5.png
--rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f6.png
--rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f7.png
--rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f8.png
--rw-r--r--   0        0        0     1917 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4f9.png
--rw-r--r--   0        0        0     2416 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4fa.png
--rw-r--r--   0        0        0     1837 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4fb.png
--rw-r--r--   0        0        0     1155 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4fc.png
--rw-r--r--   0        0        0     2361 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4fd.png
--rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f4ff.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f500.png
--rw-r--r--   0        0        0     1196 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f501.png
--rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f502.png
--rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f503.png
--rw-r--r--   0        0        0     1313 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f504.png
--rw-r--r--   0        0        0     1209 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f505.png
--rw-r--r--   0        0        0     1611 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f506.png
--rw-r--r--   0        0        0     2099 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f507.png
--rw-r--r--   0        0        0     1884 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f508.png
--rw-r--r--   0        0        0     2513 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f509.png
--rw-r--r--   0        0        0     3375 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f50a.png
--rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f50b.png
--rw-r--r--   0        0        0     1447 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f50c.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f50d.png
--rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f50e.png
--rw-r--r--   0        0        0     2493 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f50f.png
--rw-r--r--   0        0        0     2190 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f510.png
--rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f511.png
--rw-r--r--   0        0        0     1356 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f512.png
--rw-r--r--   0        0        0     1472 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f513.png
--rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f514.png
--rw-r--r--   0        0        0     2107 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f515.png
--rw-r--r--   0        0        0     1450 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f516.png
--rw-r--r--   0        0        0     2545 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f517.png
--rw-r--r--   0        0        0     1393 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f518.png
--rw-r--r--   0        0        0     1003 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f519.png
--rw-r--r--   0        0        0      723 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f51a.png
--rw-r--r--   0        0        0      949 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f51b.png
--rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f51c.png
--rw-r--r--   0        0        0      731 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f51d.png
--rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f51e.png
--rw-r--r--   0        0        0     1156 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f51f.png
--rw-r--r--   0        0        0     1441 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f520.png
--rw-r--r--   0        0        0     1340 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f521.png
--rw-r--r--   0        0        0     1353 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f522.png
--rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f523.png
--rw-r--r--   0        0        0     1160 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f524.png
--rw-r--r--   0        0        0     2128 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f525.png
--rw-r--r--   0        0        0     1502 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f526.png
--rw-r--r--   0        0        0     1216 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f527.png
--rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f528.png
--rw-r--r--   0        0        0     1853 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f529.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f52a.png
--rw-r--r--   0        0        0     2371 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f52b.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f52c.png
--rw-r--r--   0        0        0     2039 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f52d.png
--rw-r--r--   0        0        0     3144 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f52e.png
--rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f52f.png
--rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f530.png
--rw-r--r--   0        0        0     2726 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f531.png
--rw-r--r--   0        0        0      733 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f532.png
--rw-r--r--   0        0        0      531 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f533.png
--rw-r--r--   0        0        0      961 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f534.png
--rw-r--r--   0        0        0      952 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f535.png
--rw-r--r--   0        0        0      780 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f536.png
--rw-r--r--   0        0        0      847 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f537.png
--rw-r--r--   0        0        0      668 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f538.png
--rw-r--r--   0        0        0      719 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f539.png
--rw-r--r--   0        0        0      566 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f53a.png
--rw-r--r--   0        0        0      654 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f53b.png
--rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f53c.png
--rw-r--r--   0        0        0      972 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f53d.png
--rw-r--r--   0        0        0     1553 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f549.png
--rw-r--r--   0        0        0     1919 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f54a.png
--rw-r--r--   0        0        0     1294 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f54b.png
--rw-r--r--   0        0        0     2786 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f54c.png
--rw-r--r--   0        0        0     2481 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f54d.png
--rw-r--r--   0        0        0     1663 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f54e.png
--rw-r--r--   0        0        0     1700 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f550.png
--rw-r--r--   0        0        0     1660 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f551.png
--rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f552.png
--rw-r--r--   0        0        0     1748 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f553.png
--rw-r--r--   0        0        0     1749 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f554.png
--rw-r--r--   0        0        0     1687 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f555.png
--rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f556.png
--rw-r--r--   0        0        0     1767 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f557.png
--rw-r--r--   0        0        0     1635 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f558.png
--rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f559.png
--rw-r--r--   0        0        0     1720 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f55a.png
--rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f55b.png
--rw-r--r--   0        0        0     1778 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f55c.png
--rw-r--r--   0        0        0     1707 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f55d.png
--rw-r--r--   0        0        0     1648 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f55e.png
--rw-r--r--   0        0        0     1689 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f55f.png
--rw-r--r--   0        0        0     1722 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f560.png
--rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f561.png
--rw-r--r--   0        0        0     1679 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f562.png
--rw-r--r--   0        0        0     1717 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f563.png
--rw-r--r--   0        0        0     1637 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f564.png
--rw-r--r--   0        0        0     1619 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f565.png
--rw-r--r--   0        0        0     1725 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f566.png
--rw-r--r--   0        0        0     1678 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f567.png
--rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f56f.png
--rw-r--r--   0        0        0     2228 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f570.png
--rw-r--r--   0        0        0      714 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f573.png
--rw-r--r--   0        0        0     1301 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f574.png
--rw-r--r--   0        0        0     3208 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f575.png
--rw-r--r--   0        0        0     3188 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3174 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f575_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0      841 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f576.png
--rw-r--r--   0        0        0     1848 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f577.png
--rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f578.png
--rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f579.png
--rw-r--r--   0        0        0     2299 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f57a.png
--rw-r--r--   0        0        0     3424 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f587.png
--rw-r--r--   0        0        0     1232 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f58a.png
--rw-r--r--   0        0        0     1662 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f58b.png
--rw-r--r--   0        0        0     1928 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f58c.png
--rw-r--r--   0        0        0     1260 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f58d.png
--rw-r--r--   0        0        0     1529 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f590.png
--rw-r--r--   0        0        0      871 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f595.png
--rw-r--r--   0        0        0     1489 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f596.png
--rw-r--r--   0        0        0     1165 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5a4.png
--rw-r--r--   0        0        0      973 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5a5.png
--rw-r--r--   0        0        0     1403 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5a8.png
--rw-r--r--   0        0        0      761 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5b1.png
--rw-r--r--   0        0        0     1783 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5b2.png
--rw-r--r--   0        0        0     2515 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5bc.png
--rw-r--r--   0        0        0      831 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5c2.png
--rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5c3.png
--rw-r--r--   0        0        0     1035 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5c4.png
--rw-r--r--   0        0        0     4755 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5d1.png
--rw-r--r--   0        0        0     1897 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5d2.png
--rw-r--r--   0        0        0     2281 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5d3.png
--rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5dc.png
--rw-r--r--   0        0        0     1484 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5dd.png
--rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5de.png
--rw-r--r--   0        0        0     1129 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5e1.png
--rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5e3.png
--rw-r--r--   0        0        0      839 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5e8.png
--rw-r--r--   0        0        0     1569 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5ef.png
--rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5f3.png
--rw-r--r--   0        0        0     4392 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5fa.png
--rw-r--r--   0        0        0     1425 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5fb.png
--rw-r--r--   0        0        0     2590 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5fc.png
--rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5fd.png
--rw-r--r--   0        0        0     1010 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5fe.png
--rw-r--r--   0        0        0     1759 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f5ff.png
--rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f600.png
--rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f601.png
--rw-r--r--   0        0        0     2808 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f602.png
--rw-r--r--   0        0        0     2198 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f603.png
--rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f604.png
--rw-r--r--   0        0        0     2690 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f605.png
--rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f606.png
--rw-r--r--   0        0        0     3349 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f607.png
--rw-r--r--   0        0        0     2347 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f608.png
--rw-r--r--   0        0        0     1949 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f609.png
--rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f60a.png
--rw-r--r--   0        0        0     2305 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f60b.png
--rw-r--r--   0        0        0     1922 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f60c.png
--rw-r--r--   0        0        0     2417 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f60d.png
--rw-r--r--   0        0        0     2129 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f60e.png
--rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f60f.png
--rw-r--r--   0        0        0     1777 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f610.png
--rw-r--r--   0        0        0     1645 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f611.png
--rw-r--r--   0        0        0     1865 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f612.png
--rw-r--r--   0        0        0     2480 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f613.png
--rw-r--r--   0        0        0     1794 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f614.png
--rw-r--r--   0        0        0     1847 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f615.png
--rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f616.png
--rw-r--r--   0        0        0     1878 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f617.png
--rw-r--r--   0        0        0     2543 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f618.png
--rw-r--r--   0        0        0     2010 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f619.png
--rw-r--r--   0        0        0     2040 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f61a.png
--rw-r--r--   0        0        0     2093 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f61b.png
--rw-r--r--   0        0        0     2563 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f61c.png
--rw-r--r--   0        0        0     2292 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f61d.png
--rw-r--r--   0        0        0     1764 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f61e.png
--rw-r--r--   0        0        0     1962 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f61f.png
--rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f620.png
--rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f621.png
--rw-r--r--   0        0        0     2477 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f622.png
--rw-r--r--   0        0        0     1947 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f623.png
--rw-r--r--   0        0        0     3109 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f624.png
--rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f625.png
--rw-r--r--   0        0        0     1691 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f626.png
--rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f627.png
--rw-r--r--   0        0        0     2236 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f628.png
--rw-r--r--   0        0        0     2300 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f629.png
--rw-r--r--   0        0        0     2659 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62a.png
--rw-r--r--   0        0        0     2376 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62b.png
--rw-r--r--   0        0        0     1959 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62c.png
--rw-r--r--   0        0        0     2464 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62d.png
--rw-r--r--   0        0        0     1681 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62e.png
--rw-r--r--   0        0        0     3413 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62e_200d_1f4a8.png
--rw-r--r--   0        0        0     1895 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f62f.png
--rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f630.png
--rw-r--r--   0        0        0     2986 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f631.png
--rw-r--r--   0        0        0     2122 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f632.png
--rw-r--r--   0        0        0     2367 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f633.png
--rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f634.png
--rw-r--r--   0        0        0     2059 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f635.png
--rw-r--r--   0        0        0     3751 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f635_200d_1f4ab.png
--rw-r--r--   0        0        0     1711 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f636.png
--rw-r--r--   0        0        0     4477 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f636_200d_1f32b_fe0f.png
--rw-r--r--   0        0        0     2431 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f637.png
--rw-r--r--   0        0        0     2358 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f638.png
--rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f639.png
--rw-r--r--   0        0        0     2628 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f63a.png
--rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f63b.png
--rw-r--r--   0        0        0     2509 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f63c.png
--rw-r--r--   0        0        0     2625 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f63d.png
--rw-r--r--   0        0        0     2423 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f63e.png
--rw-r--r--   0        0        0     2830 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f63f.png
--rw-r--r--   0        0        0     3113 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f640.png
--rw-r--r--   0        0        0     1784 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f641.png
--rw-r--r--   0        0        0     1841 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f642.png
--rw-r--r--   0        0        0     1804 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f643.png
--rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f644.png
--rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f645.png
--rw-r--r--   0        0        0     2860 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f645_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3058 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f645_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3132 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f646.png
--rw-r--r--   0        0        0     3051 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f646_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3260 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f646_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2497 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f647.png
--rw-r--r--   0        0        0     2862 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f647_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2829 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f647_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2542 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f648.png
--rw-r--r--   0        0        0     2640 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f649.png
--rw-r--r--   0        0        0     2350 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64a.png
--rw-r--r--   0        0        0     2576 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64b.png
--rw-r--r--   0        0        0     2762 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64b_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2406 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64b_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1918 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64c.png
--rw-r--r--   0        0        0     2133 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64d.png
--rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64d_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1984 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64d_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2123 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64e.png
--rw-r--r--   0        0        0     2383 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64e_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64e_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1910 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f64f.png
--rw-r--r--   0        0        0     3216 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f680.png
--rw-r--r--   0        0        0     3045 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f681.png
--rw-r--r--   0        0        0     3402 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f682.png
--rw-r--r--   0        0        0     2144 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f683.png
--rw-r--r--   0        0        0     2088 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f684.png
--rw-r--r--   0        0        0     2044 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f685.png
--rw-r--r--   0        0        0     2384 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f686.png
--rw-r--r--   0        0        0     2168 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f687.png
--rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f688.png
--rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f689.png
--rw-r--r--   0        0        0     1964 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f68a.png
--rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f68b.png
--rw-r--r--   0        0        0     2469 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f68c.png
--rw-r--r--   0        0        0     2164 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f68d.png
--rw-r--r--   0        0        0     3075 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f68e.png
--rw-r--r--   0        0        0     1852 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f68f.png
--rw-r--r--   0        0        0     2315 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f690.png
--rw-r--r--   0        0        0     2769 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f691.png
--rw-r--r--   0        0        0     2906 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f692.png
--rw-r--r--   0        0        0     2109 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f693.png
--rw-r--r--   0        0        0     2206 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f694.png
--rw-r--r--   0        0        0     3166 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f695.png
--rw-r--r--   0        0        0     2435 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f696.png
--rw-r--r--   0        0        0     2501 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f697.png
--rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f698.png
--rw-r--r--   0        0        0     2429 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f699.png
--rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f69a.png
--rw-r--r--   0        0        0     2309 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f69b.png
--rw-r--r--   0        0        0     2980 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f69c.png
--rw-r--r--   0        0        0     1988 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f69d.png
--rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f69e.png
--rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f69f.png
--rw-r--r--   0        0        0     2526 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a0.png
--rw-r--r--   0        0        0     1735 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a1.png
--rw-r--r--   0        0        0     2413 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a2.png
--rw-r--r--   0        0        0     1966 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a3.png
--rw-r--r--   0        0        0     2262 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a3_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2156 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a3_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2041 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a4.png
--rw-r--r--   0        0        0     1795 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a5.png
--rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a6.png
--rw-r--r--   0        0        0     2554 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a7.png
--rw-r--r--   0        0        0     2975 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a8.png
--rw-r--r--   0        0        0      917 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6a9.png
--rw-r--r--   0        0        0      951 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6aa.png
--rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ab.png
--rw-r--r--   0        0        0     1543 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ac.png
--rw-r--r--   0        0        0     1875 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ad.png
--rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ae.png
--rw-r--r--   0        0        0     1929 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6af.png
--rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b0.png
--rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b1.png
--rw-r--r--   0        0        0     2702 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b2.png
--rw-r--r--   0        0        0     2181 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b3.png
--rw-r--r--   0        0        0     3994 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b4.png
--rw-r--r--   0        0        0     3960 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b4_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3931 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b4_200d_2642_fe0f.png
--rw-r--r--   0        0        0     4126 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b5.png
--rw-r--r--   0        0        0     4684 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b5_200d_2640_fe0f.png
--rw-r--r--   0        0        0     4495 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b5_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1893 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b6.png
--rw-r--r--   0        0        0     2212 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b6_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b6_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2018 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b7.png
--rw-r--r--   0        0        0     1190 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b8.png
--rw-r--r--   0        0        0     1142 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6b9.png
--rw-r--r--   0        0        0     1170 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ba.png
--rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6bb.png
--rw-r--r--   0        0        0     1188 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6bc.png
--rw-r--r--   0        0        0     1173 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6bd.png
--rw-r--r--   0        0        0     1457 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6be.png
--rw-r--r--   0        0        0     2007 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6bf.png
--rw-r--r--   0        0        0     2399 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6c0.png
--rw-r--r--   0        0        0     2784 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6c1.png
--rw-r--r--   0        0        0     1350 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6c2.png
--rw-r--r--   0        0        0     1244 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6c3.png
--rw-r--r--   0        0        0     1089 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6c4.png
--rw-r--r--   0        0        0     1292 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6c5.png
--rw-r--r--   0        0        0     1881 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6cb.png
--rw-r--r--   0        0        0     1564 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6cc.png
--rw-r--r--   0        0        0     4037 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6cd.png
--rw-r--r--   0        0        0     2362 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ce.png
--rw-r--r--   0        0        0     1192 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6cf.png
--rw-r--r--   0        0        0     1220 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6d0.png
--rw-r--r--   0        0        0      875 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6d1.png
--rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6d2.png
--rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6d5.png
--rw-r--r--   0        0        0     1632 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6d6.png
--rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6d7.png
--rw-r--r--   0        0        0     8111 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6dd.png
--rw-r--r--   0        0        0     4305 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6de.png
--rw-r--r--   0        0        0     3886 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6df.png
--rw-r--r--   0        0        0     2317 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e0.png
--rw-r--r--   0        0        0     1601 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e1.png
--rw-r--r--   0        0        0     2017 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e2.png
--rw-r--r--   0        0        0     2352 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e3.png
--rw-r--r--   0        0        0     3595 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e4.png
--rw-r--r--   0        0        0     2267 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e5.png
--rw-r--r--   0        0        0     2443 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6e9.png
--rw-r--r--   0        0        0     1908 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6eb.png
--rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6ec.png
--rw-r--r--   0        0        0     3617 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f0.png
--rw-r--r--   0        0        0     2329 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f3.png
--rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f4.png
--rw-r--r--   0        0        0     3308 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f5.png
--rw-r--r--   0        0        0     1926 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f6.png
--rw-r--r--   0        0        0     2647 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f7.png
--rw-r--r--   0        0        0     1416 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f8.png
--rw-r--r--   0        0        0     1452 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6f9.png
--rw-r--r--   0        0        0     3549 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6fa.png
--rw-r--r--   0        0        0     1981 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6fb.png
--rw-r--r--   0        0        0     3566 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f6fc.png
--rw-r--r--   0        0        0      911 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e0.png
--rw-r--r--   0        0        0      949 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e1.png
--rw-r--r--   0        0        0      857 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e2.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e3.png
--rw-r--r--   0        0        0     1016 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e4.png
--rw-r--r--   0        0        0      630 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e5.png
--rw-r--r--   0        0        0      544 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e6.png
--rw-r--r--   0        0        0      486 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e7.png
--rw-r--r--   0        0        0      695 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e8.png
--rw-r--r--   0        0        0      568 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7e9.png
--rw-r--r--   0        0        0      537 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7ea.png
--rw-r--r--   0        0        0      534 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7eb.png
--rw-r--r--   0        0        0      335 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f7f0.png
--rw-r--r--   0        0        0     1468 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f90c.png
--rw-r--r--   0        0        0      959 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f90d.png
--rw-r--r--   0        0        0     1168 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f90e.png
--rw-r--r--   0        0        0     1031 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f90f.png
--rw-r--r--   0        0        0     2728 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f910.png
--rw-r--r--   0        0        0     2691 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f911.png
--rw-r--r--   0        0        0     2684 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f912.png
--rw-r--r--   0        0        0     2539 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f913.png
--rw-r--r--   0        0        0     2157 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f914.png
--rw-r--r--   0        0        0     2019 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f915.png
--rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f916.png
--rw-r--r--   0        0        0     2530 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f917.png
--rw-r--r--   0        0        0     1300 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f918.png
--rw-r--r--   0        0        0     1397 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f919.png
--rw-r--r--   0        0        0     1383 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f91a.png
--rw-r--r--   0        0        0     1239 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f91b.png
--rw-r--r--   0        0        0     1276 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f91c.png
--rw-r--r--   0        0        0     1399 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f91d.png
--rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f91e.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f91f.png
--rw-r--r--   0        0        0     2550 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f920.png
--rw-r--r--   0        0        0     3526 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f921.png
--rw-r--r--   0        0        0     1684 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f922.png
--rw-r--r--   0        0        0     2752 2022-11-18 15:36:28.336582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f923.png
--rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f924.png
--rw-r--r--   0        0        0     2241 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f925.png
--rw-r--r--   0        0        0     2211 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f926.png
--rw-r--r--   0        0        0     2487 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f926_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2222 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f926_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2604 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f927.png
--rw-r--r--   0        0        0     1957 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f928.png
--rw-r--r--   0        0        0     3007 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f929.png
--rw-r--r--   0        0        0     2941 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f92a.png
--rw-r--r--   0        0        0     2316 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f92b.png
--rw-r--r--   0        0        0     2135 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f92c.png
--rw-r--r--   0        0        0     2253 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f92d.png
--rw-r--r--   0        0        0     3481 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f92e.png
--rw-r--r--   0        0        0     3562 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f92f.png
--rw-r--r--   0        0        0     2250 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f930.png
--rw-r--r--   0        0        0     2852 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f931.png
--rw-r--r--   0        0        0     1656 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f932.png
--rw-r--r--   0        0        0     1585 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f933.png
--rw-r--r--   0        0        0     3154 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f934.png
--rw-r--r--   0        0        0     2265 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f935.png
--rw-r--r--   0        0        0     2536 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f935_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2112 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f935_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2791 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f936.png
--rw-r--r--   0        0        0     2649 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f937.png
--rw-r--r--   0        0        0     2917 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f937_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2398 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f937_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f938.png
--rw-r--r--   0        0        0     2235 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f938_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2155 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f938_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3423 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f939.png
--rw-r--r--   0        0        0     3506 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f939_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3465 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f939_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2695 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93a.png
--rw-r--r--   0        0        0     3981 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93c.png
--rw-r--r--   0        0        0     3878 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93c_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3927 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93c_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93d.png
--rw-r--r--   0        0        0     3287 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93d_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2618 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93d_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2954 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93e.png
--rw-r--r--   0        0        0     3042 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93e_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3126 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93e_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2827 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f93f.png
--rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f940.png
--rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f941.png
--rw-r--r--   0        0        0     2319 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f942.png
--rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f943.png
--rw-r--r--   0        0        0     1133 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f944.png
--rw-r--r--   0        0        0     2674 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f945.png
--rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f947.png
--rw-r--r--   0        0        0     1808 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f948.png
--rw-r--r--   0        0        0     2087 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f949.png
--rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f94a.png
--rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f94b.png
--rw-r--r--   0        0        0     2270 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f94c.png
--rw-r--r--   0        0        0     2214 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f94d.png
--rw-r--r--   0        0        0     2622 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f94e.png
--rw-r--r--   0        0        0     1705 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f94f.png
--rw-r--r--   0        0        0     2311 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f950.png
--rw-r--r--   0        0        0     2485 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f951.png
--rw-r--r--   0        0        0     2890 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f952.png
--rw-r--r--   0        0        0     2832 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f953.png
--rw-r--r--   0        0        0     1741 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f954.png
--rw-r--r--   0        0        0     2090 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f955.png
--rw-r--r--   0        0        0     1414 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f956.png
--rw-r--r--   0        0        0     4262 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f957.png
--rw-r--r--   0        0        0     3316 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f958.png
--rw-r--r--   0        0        0     2853 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f959.png
--rw-r--r--   0        0        0     1015 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f95a.png
--rw-r--r--   0        0        0     1727 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f95b.png
--rw-r--r--   0        0        0     3624 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f95c.png
--rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f95d.png
--rw-r--r--   0        0        0     2837 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f95e.png
--rw-r--r--   0        0        0     2009 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f95f.png
--rw-r--r--   0        0        0     1509 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f960.png
--rw-r--r--   0        0        0     1724 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f961.png
--rw-r--r--   0        0        0     1278 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f962.png
--rw-r--r--   0        0        0     1504 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f963.png
--rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f964.png
--rw-r--r--   0        0        0     2092 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f965.png
--rw-r--r--   0        0        0     2813 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f966.png
--rw-r--r--   0        0        0     2219 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f967.png
--rw-r--r--   0        0        0     2790 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f968.png
--rw-r--r--   0        0        0     2651 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f969.png
--rw-r--r--   0        0        0     2666 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f96a.png
--rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f96b.png
--rw-r--r--   0        0        0     3117 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f96c.png
--rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f96d.png
--rw-r--r--   0        0        0     2615 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f96e.png
--rw-r--r--   0        0        0     3023 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f96f.png
--rw-r--r--   0        0        0     2696 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f970.png
--rw-r--r--   0        0        0     2412 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f971.png
--rw-r--r--   0        0        0     2349 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f972.png
--rw-r--r--   0        0        0     3929 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f973.png
--rw-r--r--   0        0        0     2106 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f974.png
--rw-r--r--   0        0        0     2491 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f975.png
--rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f976.png
--rw-r--r--   0        0        0     2065 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f977.png
--rw-r--r--   0        0        0     2697 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f978.png
--rw-r--r--   0        0        0     3326 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f979.png
--rw-r--r--   0        0        0     2404 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f97a.png
--rw-r--r--   0        0        0     1975 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f97b.png
--rw-r--r--   0        0        0     1541 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f97c.png
--rw-r--r--   0        0        0     2260 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f97d.png
--rw-r--r--   0        0        0     2291 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f97e.png
--rw-r--r--   0        0        0      996 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f97f.png
--rw-r--r--   0        0        0     3907 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f980.png
--rw-r--r--   0        0        0     3404 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f981.png
--rw-r--r--   0        0        0     2013 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f982.png
--rw-r--r--   0        0        0     3489 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f983.png
--rw-r--r--   0        0        0     3552 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f984.png
--rw-r--r--   0        0        0     2600 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f985.png
--rw-r--r--   0        0        0     2282 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f986.png
--rw-r--r--   0        0        0     1855 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f987.png
--rw-r--r--   0        0        0     2029 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f988.png
--rw-r--r--   0        0        0     2574 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f989.png
--rw-r--r--   0        0        0     2522 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f98a.png
--rw-r--r--   0        0        0     2937 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f98b.png
--rw-r--r--   0        0        0     2432 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f98c.png
--rw-r--r--   0        0        0     1950 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f98d.png
--rw-r--r--   0        0        0     3110 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f98e.png
--rw-r--r--   0        0        0     1713 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f98f.png
--rw-r--r--   0        0        0     4212 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f990.png
--rw-r--r--   0        0        0     4058 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f991.png
--rw-r--r--   0        0        0     2540 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f992.png
--rw-r--r--   0        0        0     2060 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f993.png
--rw-r--r--   0        0        0     2587 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f994.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f995.png
--rw-r--r--   0        0        0     2149 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f996.png
--rw-r--r--   0        0        0     2046 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f997.png
--rw-r--r--   0        0        0     1932 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f998.png
--rw-r--r--   0        0        0     1793 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f999.png
--rw-r--r--   0        0        0     4253 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f99a.png
--rw-r--r--   0        0        0     1338 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f99b.png
--rw-r--r--   0        0        0     2652 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f99c.png
--rw-r--r--   0        0        0     1442 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f99d.png
--rw-r--r--   0        0        0     3170 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f99e.png
--rw-r--r--   0        0        0     3035 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f99f.png
--rw-r--r--   0        0        0     3160 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a0.png
--rw-r--r--   0        0        0     1386 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a1.png
--rw-r--r--   0        0        0     1745 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a2.png
--rw-r--r--   0        0        0     1946 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a3.png
--rw-r--r--   0        0        0     2772 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a4.png
--rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a5.png
--rw-r--r--   0        0        0     2185 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a6.png
--rw-r--r--   0        0        0     2603 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a7.png
--rw-r--r--   0        0        0     1870 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a8.png
--rw-r--r--   0        0        0     1782 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9a9.png
--rw-r--r--   0        0        0     1986 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9aa.png
--rw-r--r--   0        0        0     1721 2022-11-18 15:36:28.372583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ab.png
--rw-r--r--   0        0        0     1659 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ac.png
--rw-r--r--   0        0        0     1328 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ad.png
--rw-r--r--   0        0        0     3191 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ae.png
--rw-r--r--   0        0        0      801 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9af.png
--rw-r--r--   0        0        0     1127 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b0.png
--rw-r--r--   0        0        0     1559 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b1.png
--rw-r--r--   0        0        0      833 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b2.png
--rw-r--r--   0        0        0     1131 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b3.png
--rw-r--r--   0        0        0     1101 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b4.png
--rw-r--r--   0        0        0      921 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b5.png
--rw-r--r--   0        0        0     1240 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b6.png
--rw-r--r--   0        0        0     1290 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b7.png
--rw-r--r--   0        0        0     3429 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b8.png
--rw-r--r--   0        0        0     3693 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b8_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3512 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b8_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3996 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b9.png
--rw-r--r--   0        0        0     4529 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b9_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3957 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9b9_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2908 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ba.png
--rw-r--r--   0        0        0     1819 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9bb.png
--rw-r--r--   0        0        0     1750 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9bc.png
--rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9bd.png
--rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9be.png
--rw-r--r--   0        0        0     1429 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9bf.png
--rw-r--r--   0        0        0     1368 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c0.png
--rw-r--r--   0        0        0     3498 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c1.png
--rw-r--r--   0        0        0     1692 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c2.png
--rw-r--r--   0        0        0     1825 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c3.png
--rw-r--r--   0        0        0     1754 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c4.png
--rw-r--r--   0        0        0     2237 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c5.png
--rw-r--r--   0        0        0     2313 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c6.png
--rw-r--r--   0        0        0     1936 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c7.png
--rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c8.png
--rw-r--r--   0        0        0     1859 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9c9.png
--rw-r--r--   0        0        0     2521 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ca.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cb.png
--rw-r--r--   0        0        0     3993 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cc.png
--rw-r--r--   0        0        0     1802 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cd.png
--rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cd_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cd_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ce.png
--rw-r--r--   0        0        0     1672 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ce_200d_2640_fe0f.png
--rw-r--r--   0        0        0     1371 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ce_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2635 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cf.png
--rw-r--r--   0        0        0     2699 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cf_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9cf_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2484 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d0.png
--rw-r--r--   0        0        0     2148 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1.png
--rw-r--r--   0        0        0     4085 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f33e.png
--rw-r--r--   0        0        0     3096 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f373.png
--rw-r--r--   0        0        0     2947 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f37c.png
--rw-r--r--   0        0        0     3304 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f384.png
--rw-r--r--   0        0        0     2602 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f393.png
--rw-r--r--   0        0        0     3162 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a4.png
--rw-r--r--   0        0        0     3507 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3a8.png
--rw-r--r--   0        0        0     2985 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3eb.png
--rw-r--r--   0        0        0     3277 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f3ed.png
--rw-r--r--   0        0        0     1983 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bb.png
--rw-r--r--   0        0        0     2284 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f4bc.png
--rw-r--r--   0        0        0     3264 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f527.png
--rw-r--r--   0        0        0     3470 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f52c.png
--rw-r--r--   0        0        0     3285 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f680.png
--rw-r--r--   0        0        0     3739 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f692.png
--rw-r--r--   0        0        0     3138 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f91d_200d_1f9d1.png
--rw-r--r--   0        0        0     2547 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9af.png
--rw-r--r--   0        0        0     2030 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b0.png
--rw-r--r--   0        0        0     2393 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b1.png
--rw-r--r--   0        0        0     1800 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b2.png
--rw-r--r--   0        0        0     2200 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9b3.png
--rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bc.png
--rw-r--r--   0        0        0     2244 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_1f9bd.png
--rw-r--r--   0        0        0     2529 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_2695_fe0f.png
--rw-r--r--   0        0        0     2671 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_2696_fe0f.png
--rw-r--r--   0        0        0     2718 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d1_200d_2708_fe0f.png
--rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d2.png
--rw-r--r--   0        0        0     2801 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d3.png
--rw-r--r--   0        0        0     2178 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d4.png
--rw-r--r--   0        0        0     4333 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d4_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3689 2022-11-18 15:36:28.352583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d4_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2258 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d5.png
--rw-r--r--   0        0        0     3176 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d6.png
--rw-r--r--   0        0        0     3180 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d6_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d6_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3412 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d7.png
--rw-r--r--   0        0        0     3963 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d7_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3608 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d7_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2201 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d8.png
--rw-r--r--   0        0        0     2189 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d8_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2314 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d8_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3401 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d9.png
--rw-r--r--   0        0        0     3318 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d9_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3327 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9d9_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2627 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9da.png
--rw-r--r--   0        0        0     3146 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9da_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2586 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9da_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2949 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9db.png
--rw-r--r--   0        0        0     3078 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9db_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3077 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9db_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3533 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9dc.png
--rw-r--r--   0        0        0     3786 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9dc_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3488 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9dc_200d_2642_fe0f.png
--rw-r--r--   0        0        0     3089 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9dd.png
--rw-r--r--   0        0        0     3289 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9dd_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3449 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9dd_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2735 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9de.png
--rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9de_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2841 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9de_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2737 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9df.png
--rw-r--r--   0        0        0     2739 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9df_200d_2640_fe0f.png
--rw-r--r--   0        0        0     2760 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9df_200d_2642_fe0f.png
--rw-r--r--   0        0        0     2467 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e0.png
--rw-r--r--   0        0        0     1175 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e1.png
--rw-r--r--   0        0        0     1084 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e2.png
--rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e3.png
--rw-r--r--   0        0        0     1581 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e4.png
--rw-r--r--   0        0        0     1812 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e5.png
--rw-r--r--   0        0        0     1914 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e6.png
--rw-r--r--   0        0        0     1351 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e7.png
--rw-r--r--   0        0        0     2523 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e8.png
--rw-r--r--   0        0        0     1911 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9e9.png
--rw-r--r--   0        0        0     2524 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ea.png
--rw-r--r--   0        0        0     1718 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9eb.png
--rw-r--r--   0        0        0     3148 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ec.png
--rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ed.png
--rw-r--r--   0        0        0     3580 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ee.png
--rw-r--r--   0        0        0     3068 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ef.png
--rw-r--r--   0        0        0     1488 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f0.png
--rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f1.png
--rw-r--r--   0        0        0     1816 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f2.png
--rw-r--r--   0        0        0     2325 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f3.png
--rw-r--r--   0        0        0     1117 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f4.png
--rw-r--r--   0        0        0     2571 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f5.png
--rw-r--r--   0        0        0     2874 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f6.png
--rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f7.png
--rw-r--r--   0        0        0     2489 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f8.png
--rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9f9.png
--rw-r--r--   0        0        0     2773 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9fa.png
--rw-r--r--   0        0        0     1623 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9fb.png
--rw-r--r--   0        0        0     2401 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9fc.png
--rw-r--r--   0        0        0     2080 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9fd.png
--rw-r--r--   0        0        0     1461 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9fe.png
--rw-r--r--   0        0        0     2710 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1f9ff.png
--rw-r--r--   0        0        0     2121 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa70.png
--rw-r--r--   0        0        0     1499 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa71.png
--rw-r--r--   0        0        0     1002 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa72.png
--rw-r--r--   0        0        0     2386 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa73.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa74.png
--rw-r--r--   0        0        0     1146 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa78.png
--rw-r--r--   0        0        0     1312 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa79.png
--rw-r--r--   0        0        0     1968 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa7a.png
--rw-r--r--   0        0        0     4290 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa7b.png
--rw-r--r--   0        0        0     2091 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa7c.png
--rw-r--r--   0        0        0     2378 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa80.png
--rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa81.png
--rw-r--r--   0        0        0     3182 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa82.png
--rw-r--r--   0        0        0     1651 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa83.png
--rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa84.png
--rw-r--r--   0        0        0     9582 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa85.png
--rw-r--r--   0        0        0     3331 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa86.png
--rw-r--r--   0        0        0     2815 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa90.png
--rw-r--r--   0        0        0     1145 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa91.png
--rw-r--r--   0        0        0     1548 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa92.png
--rw-r--r--   0        0        0     1251 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa93.png
--rw-r--r--   0        0        0     2078 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa94.png
--rw-r--r--   0        0        0     1644 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa95.png
--rw-r--r--   0        0        0     1803 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa96.png
--rw-r--r--   0        0        0     2194 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa97.png
--rw-r--r--   0        0        0     1906 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa98.png
--rw-r--r--   0        0        0     2641 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa99.png
--rw-r--r--   0        0        0     1455 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa9a.png
--rw-r--r--   0        0        0     1387 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa9b.png
--rw-r--r--   0        0        0     2654 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa9c.png
--rw-r--r--   0        0        0     1534 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa9d.png
--rw-r--r--   0        0        0     1070 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa9e.png
--rw-r--r--   0        0        0      844 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fa9f.png
--rw-r--r--   0        0        0     1214 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa0.png
--rw-r--r--   0        0        0     1646 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa1.png
--rw-r--r--   0        0        0     3421 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa2.png
--rw-r--r--   0        0        0     2517 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa3.png
--rw-r--r--   0        0        0     2137 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa4.png
--rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa5.png
--rw-r--r--   0        0        0     1357 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa6.png
--rw-r--r--   0        0        0      739 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa7.png
--rw-r--r--   0        0        0     1398 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa8.png
--rw-r--r--   0        0        0     4069 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faa9.png
--rw-r--r--   0        0        0     3116 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faaa.png
--rw-r--r--   0        0        0     2959 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faab.png
--rw-r--r--   0        0        0     3385 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1faac.png
--rw-r--r--   0        0        0     3390 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab0.png
--rw-r--r--   0        0        0     2544 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab1.png
--rw-r--r--   0        0        0     2712 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab2.png
--rw-r--r--   0        0        0     2220 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab3.png
--rw-r--r--   0        0        0     2337 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab4.png
--rw-r--r--   0        0        0     1796 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab5.png
--rw-r--r--   0        0        0     1694 2022-11-18 15:36:28.376583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab6.png
--rw-r--r--   0        0        0     3028 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab7.png
--rw-r--r--   0        0        0     8701 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab8.png
--rw-r--r--   0        0        0     3220 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fab9.png
--rw-r--r--   0        0        0     3143 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1faba.png
--rw-r--r--   0        0        0     3145 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fac0.png
--rw-r--r--   0        0        0     2355 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fac1.png
--rw-r--r--   0        0        0     1207 2022-11-18 15:36:28.368583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fac2.png
--rw-r--r--   0        0        0     2880 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fac3.png
--rw-r--r--   0        0        0     2915 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fac4.png
--rw-r--r--   0        0        0     3239 2022-11-18 15:36:28.356583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fac5.png
--rw-r--r--   0        0        0     2208 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad0.png
--rw-r--r--   0        0        0     2166 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad1.png
--rw-r--r--   0        0        0     1780 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad2.png
--rw-r--r--   0        0        0     1470 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad3.png
--rw-r--r--   0        0        0     1942 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad4.png
--rw-r--r--   0        0        0     2275 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad5.png
--rw-r--r--   0        0        0     1506 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad6.png
--rw-r--r--   0        0        0     2456 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad7.png
--rw-r--r--   0        0        0     3231 2022-11-18 15:36:28.384583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad8.png
--rw-r--r--   0        0        0     2883 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/1fad9.png
--rw-r--r--   0        0        0     3754 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae0.png
--rw-r--r--   0        0        0     2667 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae1.png
--rw-r--r--   0        0        0     3645 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae2.png
--rw-r--r--   0        0        0     3805 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae3.png
--rw-r--r--   0        0        0     3362 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae4.png
--rw-r--r--   0        0        0     2324 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae5.png
--rw-r--r--   0        0        0     2612 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae6.png
--rw-r--r--   0        0        0     8233 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/1fae7.png
--rw-r--r--   0        0        0     3094 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf0.png
--rw-r--r--   0        0        0     3119 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf1.png
--rw-r--r--   0        0        0     3274 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf2.png
--rw-r--r--   0        0        0     2474 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf3.png
--rw-r--r--   0        0        0     2475 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf4.png
--rw-r--r--   0        0        0     4017 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf5.png
--rw-r--r--   0        0        0     2903 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/1faf6.png
--rw-r--r--   0        0        0      979 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/203c.png
--rw-r--r--   0        0        0     1134 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2049.png
--rw-r--r--   0        0        0      574 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/2122.png
--rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/2139.png
--rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2194.png
--rw-r--r--   0        0        0     1027 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2195.png
--rw-r--r--   0        0        0     1046 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2196.png
--rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2197.png
--rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2198.png
--rw-r--r--   0        0        0     1000 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2199.png
--rw-r--r--   0        0        0     1098 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/21a9.png
--rw-r--r--   0        0        0     1061 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/21aa.png
--rw-r--r--   0        0        0     1401 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/231a.png
--rw-r--r--   0        0        0     2614 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/231b.png
--rw-r--r--   0        0        0      983 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/2328.png
--rw-r--r--   0        0        0     1078 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23cf.png
--rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23e9.png
--rw-r--r--   0        0        0     1097 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23ea.png
--rw-r--r--   0        0        0     1069 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23eb.png
--rw-r--r--   0        0        0     1086 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23ec.png
--rw-r--r--   0        0        0     1085 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23ed.png
--rw-r--r--   0        0        0     1153 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23ee.png
--rw-r--r--   0        0        0     1009 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23ef.png
--rw-r--r--   0        0        0     3657 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/23f0.png
--rw-r--r--   0        0        0     2800 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/23f1.png
--rw-r--r--   0        0        0     2100 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/23f2.png
--rw-r--r--   0        0        0     2759 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/23f3.png
--rw-r--r--   0        0        0     1053 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23f8.png
--rw-r--r--   0        0        0      952 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23f9.png
--rw-r--r--   0        0        0     1014 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/23fa.png
--rw-r--r--   0        0        0     1295 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/24c2.png
--rw-r--r--   0        0        0      408 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/25aa.png
--rw-r--r--   0        0        0      194 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/25ab.png
--rw-r--r--   0        0        0     1011 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/25b6.png
--rw-r--r--   0        0        0     1028 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/25c0.png
--rw-r--r--   0        0        0      196 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/25fb.png
--rw-r--r--   0        0        0      291 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/25fc.png
--rw-r--r--   0        0        0      175 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/25fd.png
--rw-r--r--   0        0        0      283 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/25fe.png
--rw-r--r--   0        0        0     1597 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2600.png
--rw-r--r--   0        0        0      934 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2601.png
--rw-r--r--   0        0        0     1630 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2602.png
--rw-r--r--   0        0        0     3102 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2603.png
--rw-r--r--   0        0        0     2996 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2604.png
--rw-r--r--   0        0        0     2616 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/260e.png
--rw-r--r--   0        0        0     1309 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2611.png
--rw-r--r--   0        0        0     2749 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2614.png
--rw-r--r--   0        0        0     1869 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/2615.png
--rw-r--r--   0        0        0     2927 2022-11-18 15:36:28.380583 a2-0.3.5/src/a2/data/emoji/emoji_images/2618.png
--rw-r--r--   0        0        0     1186 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/261d.png
--rw-r--r--   0        0        0     1956 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/2620.png
--rw-r--r--   0        0        0     1258 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2622.png
--rw-r--r--   0        0        0     1740 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2623.png
--rw-r--r--   0        0        0     1113 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2626.png
--rw-r--r--   0        0        0     1243 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/262a.png
--rw-r--r--   0        0        0     1349 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/262e.png
--rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/262f.png
--rw-r--r--   0        0        0     1621 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2638.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/2639.png
--rw-r--r--   0        0        0     1931 2022-11-18 15:36:28.340582 a2-0.3.5/src/a2/data/emoji/emoji_images/263a.png
--rw-r--r--   0        0        0     1373 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2640.png
--rw-r--r--   0        0        0     1449 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2642.png
--rw-r--r--   0        0        0     1307 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2648.png
--rw-r--r--   0        0        0     1302 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2649.png
--rw-r--r--   0        0        0     1204 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/264a.png
--rw-r--r--   0        0        0     1498 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/264b.png
--rw-r--r--   0        0        0     1435 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/264c.png
--rw-r--r--   0        0        0     1437 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/264d.png
--rw-r--r--   0        0        0     1217 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/264e.png
--rw-r--r--   0        0        0     1252 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/264f.png
--rw-r--r--   0        0        0     1250 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2650.png
--rw-r--r--   0        0        0     1424 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2651.png
--rw-r--r--   0        0        0     1355 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2652.png
--rw-r--r--   0        0        0     1223 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2653.png
--rw-r--r--   0        0        0     1041 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/265f.png
--rw-r--r--   0        0        0      990 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/2660.png
--rw-r--r--   0        0        0     1105 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/2663.png
--rw-r--r--   0        0        0     1024 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/2665.png
--rw-r--r--   0        0        0      819 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/2666.png
--rw-r--r--   0        0        0     1476 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/2668.png
--rw-r--r--   0        0        0     1547 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/267b.png
--rw-r--r--   0        0        0      902 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/267e.png
--rw-r--r--   0        0        0     1487 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/267f.png
--rw-r--r--   0        0        0     1688 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/2692.png
--rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/2693.png
--rw-r--r--   0        0        0     1924 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/2694.png
--rw-r--r--   0        0        0     1600 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2695.png
--rw-r--r--   0        0        0     2360 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/2696.png
--rw-r--r--   0        0        0     2664 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/2697.png
--rw-r--r--   0        0        0     2767 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/2699.png
--rw-r--r--   0        0        0     1680 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/269b.png
--rw-r--r--   0        0        0     2332 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/269c.png
--rw-r--r--   0        0        0      862 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/26a0.png
--rw-r--r--   0        0        0      822 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/26a1.png
--rw-r--r--   0        0        0     1297 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/26a7.png
--rw-r--r--   0        0        0      833 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/26aa.png
--rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/26ab.png
--rw-r--r--   0        0        0     1809 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/26b0.png
--rw-r--r--   0        0        0     1967 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/26b1.png
--rw-r--r--   0        0        0     1834 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/26bd.png
--rw-r--r--   0        0        0     2594 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/26be.png
--rw-r--r--   0        0        0     2364 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/26c4.png
--rw-r--r--   0        0        0     1471 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/26c5.png
--rw-r--r--   0        0        0     2224 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/26c8.png
--rw-r--r--   0        0        0     1288 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/26ce.png
--rw-r--r--   0        0        0     1106 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/26cf.png
--rw-r--r--   0        0        0     2363 2022-11-18 15:36:28.408584 a2-0.3.5/src/a2/data/emoji/emoji_images/26d1.png
--rw-r--r--   0        0        0     3241 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/26d3.png
--rw-r--r--   0        0        0     1286 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/26d4.png
--rw-r--r--   0        0        0     1219 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/26e9.png
--rw-r--r--   0        0        0     2405 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/26ea.png
--rw-r--r--   0        0        0     2999 2022-11-18 15:36:28.388583 a2-0.3.5/src/a2/data/emoji/emoji_images/26f0.png
--rw-r--r--   0        0        0     1902 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/26f1.png
--rw-r--r--   0        0        0     3153 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/26f2.png
--rw-r--r--   0        0        0     1712 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/26f3.png
--rw-r--r--   0        0        0     2385 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/26f4.png
--rw-r--r--   0        0        0     2439 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/26f5.png
--rw-r--r--   0        0        0     3013 2022-11-18 15:36:28.360583 a2-0.3.5/src/a2/data/emoji/emoji_images/26f7.png
--rw-r--r--   0        0        0     1886 2022-11-18 15:36:28.404584 a2-0.3.5/src/a2/data/emoji/emoji_images/26f8.png
--rw-r--r--   0        0        0     3213 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/26f9.png
--rw-r--r--   0        0        0     3294 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2640_fe0f.png
--rw-r--r--   0        0        0     3168 2022-11-18 15:36:28.364583 a2-0.3.5/src/a2/data/emoji/emoji_images/26f9_fe0f_200d_2642_fe0f.png
--rw-r--r--   0        0        0     1854 2022-11-18 15:36:28.392583 a2-0.3.5/src/a2/data/emoji/emoji_images/26fa.png
--rw-r--r--   0        0        0     2366 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/26fd.png
--rw-r--r--   0        0        0     3030 2022-11-18 15:36:28.416584 a2-0.3.5/src/a2/data/emoji/emoji_images/2702.png
--rw-r--r--   0        0        0     1137 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2705.png
--rw-r--r--   0        0        0     2700 2022-11-18 15:36:28.396584 a2-0.3.5/src/a2/data/emoji/emoji_images/2708.png
--rw-r--r--   0        0        0      871 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/2709.png
--rw-r--r--   0        0        0     1669 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/270a.png
--rw-r--r--   0        0        0     1464 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/270b.png
--rw-r--r--   0        0        0     1407 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/270c.png
--rw-r--r--   0        0        0     1751 2022-11-18 15:36:28.348582 a2-0.3.5/src/a2/data/emoji/emoji_images/270d.png
--rw-r--r--   0        0        0     1587 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/270f.png
--rw-r--r--   0        0        0     1526 2022-11-18 15:36:28.412584 a2-0.3.5/src/a2/data/emoji/emoji_images/2712.png
--rw-r--r--   0        0        0      631 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2714.png
--rw-r--r--   0        0        0      518 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2716.png
--rw-r--r--   0        0        0      890 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/271d.png
--rw-r--r--   0        0        0     1315 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2721.png
--rw-r--r--   0        0        0     1385 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2728.png
--rw-r--r--   0        0        0     1187 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/2733.png
--rw-r--r--   0        0        0     1432 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/2734.png
--rw-r--r--   0        0        0     3717 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2744.png
--rw-r--r--   0        0        0     1179 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/2747.png
--rw-r--r--   0        0        0      782 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/274c.png
--rw-r--r--   0        0        0     1100 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/274e.png
--rw-r--r--   0        0        0      685 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2753.png
--rw-r--r--   0        0        0      624 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2754.png
--rw-r--r--   0        0        0      690 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2755.png
--rw-r--r--   0        0        0      568 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2757.png
--rw-r--r--   0        0        0     1038 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/2763.png
--rw-r--r--   0        0        0     1358 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/2764.png
--rw-r--r--   0        0        0     3565 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1f525.png
--rw-r--r--   0        0        0     3181 2022-11-18 15:36:28.344582 a2-0.3.5/src/a2/data/emoji/emoji_images/2764_fe0f_200d_1fa79.png
--rw-r--r--   0        0        0      251 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2795.png
--rw-r--r--   0        0        0      200 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2796.png
--rw-r--r--   0        0        0      249 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2797.png
--rw-r--r--   0        0        0     1047 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/27a1.png
--rw-r--r--   0        0        0      858 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/27b0.png
--rw-r--r--   0        0        0      686 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/27bf.png
--rw-r--r--   0        0        0     1083 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2934.png
--rw-r--r--   0        0        0     1076 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2935.png
--rw-r--r--   0        0        0     1044 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b05.png
--rw-r--r--   0        0        0     1034 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b06.png
--rw-r--r--   0        0        0     1054 2022-11-18 15:36:28.420584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b07.png
--rw-r--r--   0        0        0      700 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b1b.png
--rw-r--r--   0        0        0      203 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b1c.png
--rw-r--r--   0        0        0     1704 2022-11-18 15:36:28.400584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b50.png
--rw-r--r--   0        0        0     1025 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/2b55.png
--rw-r--r--   0        0        0      614 2022-11-18 15:36:28.424584 a2-0.3.5/src/a2/data/emoji/emoji_images/3030.png
--rw-r--r--   0        0        0      791 2022-11-18 15:36:28.428584 a2-0.3.5/src/a2/data/emoji/emoji_images/303d.png
--rw-r--r--   0        0        0     1614 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/3297.png
--rw-r--r--   0        0        0     1733 2022-11-18 15:36:28.432584 a2-0.3.5/src/a2/data/emoji/emoji_images/3299.png
--rw-r--r--   0        0        0  2152796 2022-07-06 14:12:42.663962 a2-0.3.5/src/a2/data/font/Symbola.ttf
--rw-r--r--   0        0        0  3727644 2022-07-06 14:12:42.683963 a2-0.3.5/src/a2/data/font/Symbola_hint.ttf
--rw-r--r--   0        0        0       44 2022-07-06 14:12:42.683963 a2-0.3.5/src/a2/data/font/sharefonts.net.txt
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.5/src/a2/data/vocabularies/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.5/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
--rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.5/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
--rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.5/src/a2/dataset/__init__.py
--rw-r--r--   0        0        0      366 2023-02-21 14:04:45.557653 a2-0.3.5/src/a2/dataset/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      645 2023-01-30 15:08:36.152054 a2-0.3.5/src/a2/dataset/__pycache__/emojis.cpython-310.pyc
--rw-r--r--   0        0        0     8810 2023-06-06 15:04:03.968979 a2-0.3.5/src/a2/dataset/__pycache__/load_dataset.cpython-310.pyc
--rw-r--r--   0        0        0      434 2022-08-02 15:37:53.112570 a2-0.3.5/src/a2/dataset/__pycache__/manipulate_datasets.cpython-310.pyc
--rw-r--r--   0        0        0    39422 2023-01-30 15:08:36.940073 a2-0.3.5/src/a2/dataset/__pycache__/radar.cpython-310.pyc
--rw-r--r--   0        0        0     8738 2023-01-30 15:08:36.944073 a2-0.3.5/src/a2/dataset/__pycache__/stations.cpython-310.pyc
--rw-r--r--   0        0        0     1040 2023-02-20 13:59:16.193086 a2-0.3.5/src/a2/dataset/__pycache__/tweets.cpython-310.pyc
--rw-r--r--   0        0        0     2155 2022-12-14 09:39:28.258310 a2-0.3.5/src/a2/dataset/__pycache__/units.cpython-310.pyc
--rw-r--r--   0        0        0    15533 2023-06-06 13:09:57.413845 a2-0.3.5/src/a2/dataset/__pycache__/utils_dataset.cpython-310.pyc
--rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.5/src/a2/dataset/emojis.py
--rw-r--r--   0        0        0     8160 2023-06-06 14:01:17.881575 a2-0.3.5/src/a2/dataset/load_dataset.py
--rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.5/src/a2/dataset/radar.py
--rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.5/src/a2/dataset/stations.py
--rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.5/src/a2/dataset/tweets.py
--rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.5/src/a2/dataset/units.py
--rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.3.5/src/a2/dataset/utils_dataset.py
--rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.5/src/a2/plotting/__init__.py
--rw-r--r--   0        0        0      366 2022-12-14 09:39:30.762420 a2-0.3.5/src/a2/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7136 2023-05-16 09:07:00.708334 a2-0.3.5/src/a2/plotting/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     1901 2023-02-14 15:41:10.653195 a2-0.3.5/src/a2/plotting/__pycache__/axes_utils.cpython-310.pyc
--rw-r--r--   0        0        0    22974 2023-05-16 11:22:14.741608 a2-0.3.5/src/a2/plotting/__pycache__/histograms.cpython-310.pyc
--rw-r--r--   0        0        0     3123 2022-12-14 09:39:32.242484 a2-0.3.5/src/a2/plotting/__pycache__/parallel_plotting.cpython-310.pyc
--rw-r--r--   0        0        0     2721 2022-12-14 09:39:32.242484 a2-0.3.5/src/a2/plotting/__pycache__/timeseries.cpython-310.pyc
--rw-r--r--   0        0        0    14561 2023-05-16 09:07:00.712334 a2-0.3.5/src/a2/plotting/__pycache__/utils_plotting.cpython-310.pyc
--rw-r--r--   0        0        0    29227 2023-02-20 13:59:16.709099 a2-0.3.5/src/a2/plotting/__pycache__/weather_maps.cpython-310.pyc
--rw-r--r--   0        0        0     8164 2023-05-12 12:06:36.401113 a2-0.3.5/src/a2/plotting/analysis.py
--rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.5/src/a2/plotting/axes_utils.py
--rw-r--r--   0        0        0    30638 2023-05-16 11:22:03.945363 a2-0.3.5/src/a2/plotting/histograms.py
--rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.5/src/a2/plotting/parallel_plotting.py
--rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.5/src/a2/plotting/timeseries.py
--rw-r--r--   0        0        0    16218 2023-05-12 12:06:36.401113 a2-0.3.5/src/a2/plotting/utils_plotting.py
--rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.5/src/a2/plotting/weather_maps.py
--rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.5/src/a2/preprocess/__init__.py
--rw-r--r--   0        0        0      228 2022-11-10 09:21:06.475180 a2-0.3.5/src/a2/preprocess/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3659 2022-12-06 08:50:28.056225 a2-0.3.5/src/a2/preprocess/__pycache__/embedding.cpython-310.pyc
--rw-r--r--   0        0        0    26114 2023-05-23 13:01:09.722463 a2-0.3.5/src/a2/preprocess/__pycache__/normalize_text.cpython-310.pyc
--rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.5/src/a2/preprocess/embedding.py
--rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.3.5/src/a2/preprocess/normalize_text.py
--rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.3.5/src/a2/training/__init__.py
--rw-r--r--   0        0        0      343 2023-05-16 09:06:59.916315 a2-0.3.5/src/a2/training/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4800 2023-05-16 09:07:02.808385 a2-0.3.5/src/a2/training/__pycache__/benchmarks.cpython-310.pyc
--rw-r--r--   0        0        0     2912 2023-06-06 15:20:27.594394 a2-0.3.5/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     3990 2023-06-06 15:46:01.463325 a2-0.3.5/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     4976 2023-06-06 15:47:37.209538 a2-0.3.5/src/a2/training/__pycache__/tracking.cpython-310.pyc
--rw-r--r--   0        0        0     2217 2023-05-16 09:07:02.804385 a2-0.3.5/src/a2/training/__pycache__/tracking_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-16 09:07:02.804385 a2-0.3.5/src/a2/training/__pycache__/training_deep500.cpython-310.pyc
--rw-r--r--   0        0        0     8646 2023-06-06 15:04:05.473018 a2-0.3.5/src/a2/training/__pycache__/training_hugging.cpython-310.pyc
--rw-r--r--   0        0        0     6756 2023-04-18 13:46:32.335340 a2-0.3.5/src/a2/training/__pycache__/training_performance.cpython-310.pyc
--rw-r--r--   0        0        0      306 2023-01-30 15:08:44.672258 a2-0.3.5/src/a2/training/__pycache__/utils_training.cpython-310.pyc
--rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.3.5/src/a2/training/benchmarks.py
--rw-r--r--   0        0        0     2863 2023-06-06 15:14:17.260894 a2-0.3.5/src/a2/training/dataset_hugging.py
--rw-r--r--   0        0        0     4213 2023-06-06 15:45:58.319253 a2-0.3.5/src/a2/training/evaluate_hugging.py
--rw-r--r--   0        0        0     4563 2023-06-06 15:48:04.766178 a2-0.3.5/src/a2/training/tracking.py
--rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.3.5/src/a2/training/tracking_hugging.py
--rw-r--r--   0        0        0     6390 2023-05-12 12:06:13.512505 a2-0.3.5/src/a2/training/training_deep500.py
--rw-r--r--   0        0        0    11299 2023-06-06 14:58:39.420340 a2-0.3.5/src/a2/training/training_hugging.py
--rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.3.5/src/a2/training/training_performance.py
--rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.5/src/a2/training/utils_training.py
--rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.5/src/a2/twitter/__init__.py
--rw-r--r--   0        0        0      249 2022-11-10 09:22:53.001431 a2-0.3.5/src/a2/twitter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4896 2023-02-20 13:59:24.705291 a2-0.3.5/src/a2/twitter/__pycache__/downloader.cpython-310.pyc
--rw-r--r--   0        0        0     9148 2023-05-23 13:01:12.894332 a2-0.3.5/src/a2/twitter/__pycache__/locations.cpython-310.pyc
--rw-r--r--   0        0        0     8339 2022-08-01 13:51:16.422462 a2-0.3.5/src/a2/twitter/__pycache__/manipulate_tweets.cpython-310.pyc
--rw-r--r--   0        0        0     5836 2023-02-20 13:59:24.705291 a2-0.3.5/src/a2/twitter/__pycache__/twitter_api.cpython-310.pyc
--rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.5/src/a2/twitter/downloader.py
--rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.3.5/src/a2/twitter/locations.py
--rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.5/src/a2/twitter/twitter_api.py
--rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.3.5/src/a2/utils/__init__.py
--rw-r--r--   0        0        0      376 2023-06-06 12:42:23.443076 a2-0.3.5/src/a2/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7195 2023-06-06 15:39:11.206038 a2-0.3.5/src/a2/utils/__pycache__/argparse.cpython-310.pyc
--rw-r--r--   0        0        0      787 2023-05-16 09:06:59.920315 a2-0.3.5/src/a2/utils/__pycache__/checks.cpython-310.pyc
--rw-r--r--   0        0        0      558 2023-02-20 15:49:06.840044 a2-0.3.5/src/a2/utils/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     9546 2023-06-06 15:04:04.548994 a2-0.3.5/src/a2/utils/__pycache__/file_handling.cpython-310.pyc
--rw-r--r--   0        0        0      445 2023-05-16 09:07:00.248323 a2-0.3.5/src/a2/utils/__pycache__/strings.cpython-310.pyc
--rw-r--r--   0        0        0     6104 2023-05-16 09:07:00.248323 a2-0.3.5/src/a2/utils/__pycache__/testing.cpython-310.pyc
--rw-r--r--   0        0        0      545 2022-12-14 09:39:28.222309 a2-0.3.5/src/a2/utils/__pycache__/times.cpython-310.pyc
--rw-r--r--   0        0        0     6704 2023-05-16 09:07:00.336325 a2-0.3.5/src/a2/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     8426 2023-06-06 15:52:32.536430 a2-0.3.5/src/a2/utils/argparse.py
--rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.3.5/src/a2/utils/checks.py
--rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.5/src/a2/utils/constants.py
--rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.3.5/src/a2/utils/file_handling.py
--rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.3.5/src/a2/utils/strings.py
--rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.3.5/src/a2/utils/testing.py
--rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.5/src/a2/utils/times.py
--rw-r--r--   0        0        0     6088 2023-05-12 12:06:36.405113 a2-0.3.5/src/a2/utils/utils.py
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 a2-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     3941 2023-06-06 16:29:51.630832 a2-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.6/src/a2/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.6/src/a2/cli/__init__.py
+-rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.6/src/a2/cli/cli_plotting/__init__.py
+-rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.6/src/a2/cli/cli_plotting/plot.py
+-rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.6/src/a2/cli/cli_plotting/single_plots.py
+-rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.6/src/a2/cli/main.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.6/src/a2/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.6/src/a2/data/emoji/__init__.py
+-rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.6/src/a2/data/emoji/emoji_df.csv
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.6/src/a2/data/vocabularies/__init__.py
+-rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.6/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
+-rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.6/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
+-rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.6/src/a2/dataset/__init__.py
+-rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.6/src/a2/dataset/emojis.py
+-rw-r--r--   0        0        0     8227 2023-06-06 16:23:55.890263 a2-0.3.6/src/a2/dataset/load_dataset.py
+-rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.6/src/a2/dataset/radar.py
+-rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.6/src/a2/dataset/stations.py
+-rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.6/src/a2/dataset/tweets.py
+-rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.6/src/a2/dataset/units.py
+-rw-r--r--   0        0        0    17623 2023-06-06 13:09:51.493718 a2-0.3.6/src/a2/dataset/utils_dataset.py
+-rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.6/src/a2/plotting/__init__.py
+-rw-r--r--   0        0        0     8164 2023-05-12 12:06:36.401113 a2-0.3.6/src/a2/plotting/analysis.py
+-rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.6/src/a2/plotting/axes_utils.py
+-rw-r--r--   0        0        0    30638 2023-05-16 11:22:03.945363 a2-0.3.6/src/a2/plotting/histograms.py
+-rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.6/src/a2/plotting/parallel_plotting.py
+-rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.6/src/a2/plotting/timeseries.py
+-rw-r--r--   0        0        0    16218 2023-05-12 12:06:36.401113 a2-0.3.6/src/a2/plotting/utils_plotting.py
+-rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.6/src/a2/plotting/weather_maps.py
+-rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.6/src/a2/preprocess/__init__.py
+-rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.6/src/a2/preprocess/embedding.py
+-rw-r--r--   0        0        0    30389 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/preprocess/normalize_text.py
+-rw-r--r--   0        0        0      172 2023-05-12 12:06:13.512505 a2-0.3.6/src/a2/training/__init__.py
+-rw-r--r--   0        0        0     3889 2023-05-12 12:12:57.271066 a2-0.3.6/src/a2/training/benchmarks.py
+-rw-r--r--   0        0        0     2863 2023-06-06 15:14:17.260894 a2-0.3.6/src/a2/training/dataset_hugging.py
+-rw-r--r--   0        0        0     4213 2023-06-06 15:45:58.319253 a2-0.3.6/src/a2/training/evaluate_hugging.py
+-rw-r--r--   0        0        0     4563 2023-06-06 15:48:04.766178 a2-0.3.6/src/a2/training/tracking.py
+-rw-r--r--   0        0        0     1780 2023-05-12 12:06:13.512505 a2-0.3.6/src/a2/training/tracking_hugging.py
+-rw-r--r--   0        0        0     6390 2023-05-12 12:06:13.512505 a2-0.3.6/src/a2/training/training_deep500.py
+-rw-r--r--   0        0        0    11299 2023-06-06 14:58:39.420340 a2-0.3.6/src/a2/training/training_hugging.py
+-rw-r--r--   0        0        0     6821 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/training/training_performance.py
+-rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.6/src/a2/training/utils_training.py
+-rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.6/src/a2/twitter/__init__.py
+-rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.6/src/a2/twitter/downloader.py
+-rw-r--r--   0        0        0    11489 2023-06-06 13:55:59.732319 a2-0.3.6/src/a2/twitter/locations.py
+-rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.6/src/a2/twitter/twitter_api.py
+-rw-r--r--   0        0        0      196 2023-06-06 12:24:26.982480 a2-0.3.6/src/a2/utils/__init__.py
+-rw-r--r--   0        0        0     8658 2023-06-06 16:22:16.123856 a2-0.3.6/src/a2/utils/argparse.py
+-rw-r--r--   0        0        0      518 2023-05-11 10:46:59.965258 a2-0.3.6/src/a2/utils/checks.py
+-rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.6/src/a2/utils/constants.py
+-rw-r--r--   0        0        0     9361 2023-06-06 14:01:17.485564 a2-0.3.6/src/a2/utils/file_handling.py
+-rw-r--r--   0        0        0       90 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/utils/strings.py
+-rw-r--r--   0        0        0     5327 2023-05-12 12:06:33.277030 a2-0.3.6/src/a2/utils/testing.py
+-rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.6/src/a2/utils/times.py
+-rw-r--r--   0        0        0     6088 2023-05-12 12:06:36.405113 a2-0.3.6/src/a2/utils/utils.py
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 a2-0.3.6/PKG-INFO
```

### Comparing `a2-0.3.5/pyproject.toml` & `a2-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "a2"
-version = "0.3.5"
+version = "0.3.6"
 description = "Package for predicting information about the weather from social media data as application 2 for maelstrom project"
 authors = ["Kristian Ehlert <kristian.ehlert@4-cast.de>"]
 packages = [{ include = "a2", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jupyterlab = "^3.4.3"
```

### Comparing `a2-0.3.5/src/a2/cli/cli_plotting/single_plots.py` & `a2-0.3.6/src/a2/cli/cli_plotting/single_plots.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/data/emoji/emoji_df.csv` & `a2-0.3.6/src/a2/data/emoji/emoji_df.csv`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt` & `a2-0.3.6/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/dataset/emojis.py` & `a2-0.3.6/src/a2/dataset/emojis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/dataset/load_dataset.py` & `a2-0.3.6/src/a2/dataset/load_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,17 @@
 ) -> xarray.Dataset:
     """
     loads dataset from disk and converts columns into convenient data formats
 
     Parameters:
     ----------
     filename: Filename of cn file
-    reset_index: Reset index coordinate
     raw: Just load file, no conversions
+    reset_index: Reset index coordinate
+    reset_index_raw: Reset index coordinate even when `raw="true"`
     drop_variables: List of variables to drop
     convert_bounding_box: Convert bounding box coordinates from string to dictionary
     open_dataset: Open the dataset instead of loading it in memory
 
     Returns
     -------
     dataset of tweets
```

### Comparing `a2-0.3.5/src/a2/dataset/radar.py` & `a2-0.3.6/src/a2/dataset/radar.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/dataset/stations.py` & `a2-0.3.6/src/a2/dataset/stations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/dataset/tweets.py` & `a2-0.3.6/src/a2/dataset/tweets.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/dataset/units.py` & `a2-0.3.6/src/a2/dataset/units.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/dataset/utils_dataset.py` & `a2-0.3.6/src/a2/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/analysis.py` & `a2-0.3.6/src/a2/plotting/analysis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/axes_utils.py` & `a2-0.3.6/src/a2/plotting/axes_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/histograms.py` & `a2-0.3.6/src/a2/plotting/histograms.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/parallel_plotting.py` & `a2-0.3.6/src/a2/plotting/parallel_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/timeseries.py` & `a2-0.3.6/src/a2/plotting/timeseries.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/utils_plotting.py` & `a2-0.3.6/src/a2/plotting/utils_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/plotting/weather_maps.py` & `a2-0.3.6/src/a2/plotting/weather_maps.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/preprocess/embedding.py` & `a2-0.3.6/src/a2/preprocess/embedding.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/preprocess/normalize_text.py` & `a2-0.3.6/src/a2/preprocess/normalize_text.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/training/__pycache__/dataset_hugging.cpython-310.pyc` & `a2-0.3.6/src/a2/training/dataset_hugging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,179 @@
-00000000: 6f0d 0d0a 0000 0000 494d 7f64 2f0b 0000  o.......IM.d/...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
-00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c04 5a04 6400 6401 6c05 5a06 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6401 6c07 5a07 6400 6401 6c08 5a08 4700  d.l.Z.d.d.l.Z.G.
-00000060: 6402 6403 8400 6403 8302 5a09 6401 5300  d.d...d...Z.d.S.
-00000070: 2904 e900 0000 004e 6300 0000 0000 0000  )......Nc.......
-00000080: 0000 0000 0000 0000 0013 0000 0040 0000  .............@..
-00000090: 0073 8200 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-000000a0: 5a03 6418 6403 6504 6404 6505 6604 6405  Z.d.d.e.d.e.f.d.
-000000b0: 6406 8405 5a06 6407 6507 6602 6408 6409  d...Z.d.e.f.d.d.
-000000c0: 8404 5a08 090a 090b 090c 090a 6419 640d  ..Z.........d.d.
-000000d0: 6509 6a0a 640e 650b 6a0c 640f 4200 6410  e.j.d.e.j.d.B.d.
-000000e0: 650b 6a0c 640f 4200 6411 6505 6412 6504  e.j.d.B.d.e.d.e.
-000000f0: 6413 6504 6414 6505 6415 650d 6a0e 650f  d.e.d.e.d.e.j.e.
-00000100: 6a0a 650f 6a10 6602 1900 6610 6416 6417  j.e.j.f...f.d.d.
-00000110: 8405 5a11 640f 5300 291a da12 4461 7461  ..Z.d.S.)...Data
-00000120: 7365 7448 7567 6769 6e67 4661 6365 6146  setHuggingFaceaF
-00000130: 0100 000a 2020 2020 5573 6564 2074 6f20  ....    Used to 
-00000140: 6372 6561 7465 2064 6174 6173 6574 2069  create dataset i
-00000150: 6e20 4875 6767 696e 6720 4661 6365 2066  n Hugging Face f
-00000160: 6f72 6d61 742e 0a0a 2020 2020 4174 7472  ormat...    Attr
-00000170: 6962 7574 6573 0a20 2020 202d 2d2d 2d2d  ibutes.    -----
-00000180: 2d2d 2d2d 2d0a 2020 2020 746f 6b65 6e69  -----.    tokeni
-00000190: 7a65 7220 3a20 4875 6767 696e 6720 4661  zer : Hugging Fa
-000001a0: 6365 2074 6f6b 656e 697a 6572 0a0a 2020  ce tokenizer..  
-000001b0: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
-000001c0: 2d0a 2020 2020 5573 6520 4875 6767 696e  -.    Use Huggin
-000001d0: 6720 4661 6365 206d 6f64 656c 2066 6f6c  g Face model fol
-000001e0: 6465 7273 2074 6f20 696e 6974 6961 6c69  ders to initiali
-000001f0: 7a65 2074 6f6b 656e 697a 6572 2061 6e64  ze tokenizer and
-00000200: 2062 7569 6c64 2061 0a20 2020 2048 7567   build a.    Hug
-00000210: 6769 6e67 2046 6163 6520 6461 7461 7365  ging Face datase
-00000220: 7420 6672 6f6d 2061 6e20 7861 7272 6179  t from an xarray
-00000230: 2064 6174 6173 6574 2e0a 2020 2020 4361   dataset..    Ca
-00000240: 6e20 6265 2072 6575 7365 6420 746f 2062  n be reused to b
-00000250: 696c 6420 7468 6520 7465 7374 2064 6174  ild the test dat
-00000260: 6173 6574 2066 6f72 2076 616c 6964 6174  aset for validat
-00000270: 696f 6e2e 0a20 2020 2046 da0c 6d6f 6465  ion..    F..mode
-00000280: 6c5f 666f 6c64 6572 da08 7573 655f 6661  l_folder..use_fa
-00000290: 7374 6303 0000 0000 0000 0000 0000 0003  stc.............
-000002a0: 0000 0004 0000 0043 0000 0073 1c00 0000  .......C...s....
-000002b0: 7c01 7c00 5f00 7401 6a02 6a03 7c01 6401  |.|._.t.j.j.|.d.
-000002c0: 6402 8d02 7c00 5f04 6400 5300 2903 4e46  d...|._.d.S.).NF
-000002d0: 2901 7204 0000 0029 0572 0300 0000 da0c  ).r....).r......
-000002e0: 7472 616e 7366 6f72 6d65 7273 da0d 4175  transformers..Au
-000002f0: 746f 546f 6b65 6e69 7a65 72da 0f66 726f  toTokenizer..fro
-00000300: 6d5f 7072 6574 7261 696e 6564 da09 746f  m_pretrained..to
-00000310: 6b65 6e69 7a65 7229 03da 0473 656c 6672  kenizer)...selfr
-00000320: 0300 0000 7204 0000 00a9 0072 0a00 0000  ....r......r....
-00000330: fa3d 2f68 6f6d 652f 6b72 6973 7469 616e  .=/home/kristian
-00000340: 2f50 726f 6a65 6374 732f 6132 2f73 7263  /Projects/a2/src
-00000350: 2f61 322f 7472 6169 6e69 6e67 2f64 6174  /a2/training/dat
-00000360: 6173 6574 5f68 7567 6769 6e67 2e70 79da  aset_hugging.py.
-00000370: 085f 5f69 6e69 745f 5f19 0000 0073 0a00  .__init__....s..
-00000380: 0000 0601 0601 0201 0201 0cfe 7a1b 4461  ............z.Da
-00000390: 7461 7365 7448 7567 6769 6e67 4661 6365  tasetHuggingFace
-000003a0: 2e5f 5f69 6e69 745f 5fda 0178 6302 0000  .__init__..xc...
-000003b0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000003c0: 0043 0000 0073 1200 0000 7c00 6a00 7c01  .C...s....|.j.|.
-000003d0: 6401 1900 6402 6403 8d02 5300 2904 4eda  d...d.d...S.).N.
-000003e0: 0669 6e70 7574 7354 2901 da07 7061 6464  .inputsT)...padd
-000003f0: 696e 6729 0172 0800 0000 2902 7209 0000  ing).r....).r...
-00000400: 0072 0d00 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00000410: 720b 0000 00da 095f 746f 6b5f 6675 6e63  r......_tok_func
-00000420: 2000 0000 7302 0000 0012 017a 1c44 6174   ...s......z.Dat
-00000430: 6173 6574 4875 6767 696e 6746 6163 652e  asetHuggingFace.
-00000440: 5f74 6f6b 5f66 756e 6354 da04 7465 7874  _tok_funcT..text
-00000450: da07 7261 696e 696e 67da 0264 73da 0d69  ..raining..ds..i
-00000460: 6e64 6963 6573 5f74 7261 696e 4eda 1069  ndices_trainN..i
-00000470: 6e64 6963 6573 5f76 616c 6964 6174 65da  ndices_validate.
-00000480: 0574 7261 696e da0a 6b65 795f 696e 7075  .train..key_inpu
-00000490: 7473 da09 6b65 795f 6c61 6265 6cda 0b72  ts..key_label..r
-000004a0: 6573 6574 5f69 6e64 6578 da06 7265 7475  eset_index..retu
-000004b0: 726e 6308 0000 0000 0000 0000 0000 000c  rnc.............
-000004c0: 0000 0006 0000 0043 0000 0073 e800 0000  .......C...s....
-000004d0: 7c04 7219 7400 7c02 6401 7500 7c03 6401  |.r.t.|.d.u.|.d.
-000004e0: 7500 6702 8301 6402 6b02 7219 7401 6403  u.g...d.k.r.t.d.
-000004f0: 7c02 9b02 6404 7c03 9b00 6405 9d05 8301  |...d.|...d.....
-00000500: 8201 7402 6a03 6a04 a005 7c01 7c05 7c06  ..t.j.j...|.|.|.
-00000510: 6702 a102 0100 7c07 722c 7402 6a03 6a06  g.....|.r,t.j.j.
-00000520: a007 7c01 a101 7d01 7c04 7338 7c03 6401  ..|...}.|.s8|.d.
-00000530: 7501 7238 7c01 6a08 7c03 6406 8d01 7d01  u.r8|.j.|.d...}.
-00000540: 7c01 7c05 7c06 6702 1900 a009 a100 7d08  |.|.|.g.......}.
-00000550: 7c05 6407 7c06 6408 6902 7d09 7c08 6a0a  |.d.|.d.i.}.|.j.
-00000560: 7c09 6409 8d01 7d08 740b 6a0c a00d 7c08  |.d...}.t.j...|.
-00000570: a101 7d0a 7c0a 6a0e 7c00 6a0f 640a 640b  ..}.|.j.|.j.d.d.
-00000580: 8d02 7d0b 7c04 7264 7c02 6401 7500 7266  ..}.|.rd|.d.u.rf
-00000590: 7c03 6401 7500 7266 7c0b 5300 740b a010  |.d.u.rf|.S.t...
-000005a0: 7c0b a011 7c02 a101 7c0b a011 7c03 a101  |...|...|...|...
-000005b0: 640c 9c02 a101 5300 290d 614a 0200 000a  d.....S.).aJ....
-000005c0: 2020 2020 2020 2020 4372 6561 7465 2048          Create H
-000005d0: 7567 6769 6e67 2046 6163 6520 6461 7461  ugging Face data
-000005e0: 7365 7420 2864 6174 6173 6574 732e 4461  set (datasets.Da
-000005f0: 7461 7365 7444 6963 7429 2066 726f 6d20  tasetDict) from 
-00000600: 7861 7272 6179 2064 6174 6173 6574 0a0a  xarray dataset..
-00000610: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00000620: 7273 3a0a 2020 2020 2020 2020 2d2d 2d2d  rs:.        ----
-00000630: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2064  ------.        d
-00000640: 733a 2078 6172 7261 7920 6461 7461 7365  s: xarray datase
-00000650: 740a 2020 2020 2020 2020 696e 6469 6365  t.        indice
-00000660: 735f 7472 6169 6e3a 2056 6172 6961 626c  s_train: Variabl
-00000670: 6520 2769 6e64 6578 2720 7661 6c75 6573  e 'index' values
-00000680: 2074 6861 7420 6172 6520 7573 6564 2066   that are used f
-00000690: 6f72 2074 7261 696e 696e 670a 2020 2020  or training.    
-000006a0: 2020 2020 696e 6469 6365 735f 7661 6c69      indices_vali
-000006b0: 6461 7465 3a20 5661 7269 6162 6c65 2027  date: Variable '
-000006c0: 696e 6465 7827 2076 616c 7565 7320 7468  index' values th
-000006d0: 6174 2061 7265 2075 7365 6420 666f 7220  at are used for 
-000006e0: 7661 6c69 6461 7469 6f6e 0a20 2020 2020  validation.     
-000006f0: 2020 2074 7261 696e 3a20 4966 2074 6865     train: If the
-00000700: 2064 6174 6173 6574 2069 7320 7573 6564   dataset is used
-00000710: 2066 6f72 2074 7261 696e 696e 670a 2020   for training.  
-00000720: 2020 2020 2020 6b65 795f 696e 7075 7473        key_inputs
-00000730: 3a20 4b65 7920 6f66 2076 6172 6961 626c  : Key of variabl
-00000740: 6520 7573 6564 2061 7320 696e 7075 7420  e used as input 
-00000750: 746f 206d 6f64 656c 0a20 2020 2020 2020  to model.       
-00000760: 206b 6579 5f6c 6162 656c 3a20 4b65 7920   key_label: Key 
-00000770: 6f66 2076 6172 6961 626c 6520 7573 6564  of variable used
-00000780: 2061 7320 6c61 6265 6c20 666f 7220 7472   as label for tr
-00000790: 6169 6e69 6e67 0a20 2020 2020 2020 2072  aining.        r
-000007a0: 6573 6574 5f69 6e64 6578 3a20 5265 7365  eset_index: Rese
-000007b0: 7420 696e 6465 7820 636f 6f72 6469 6e61  t index coordina
-000007c0: 7465 0a0a 2020 2020 2020 2020 5265 7475  te..        Retu
-000007d0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-000007e0: 2d2d 2d0a 2020 2020 2020 2020 6461 7461  ---.        data
-000007f0: 7365 7473 2e44 6174 6173 6574 4469 6374  sets.DatasetDict
-00000800: 0a20 2020 2020 2020 204e e901 0000 007a  .        N.....z
-00000810: 0e69 6e64 6963 6573 5f74 7261 696e 3d7a  .indices_train=z
-00000820: 0520 616e 6420 7a2b 2063 616e 2065 6974  . and z+ can eit
-00000830: 6865 7220 6265 2062 6f74 6820 4e6f 6e65  her be both None
-00000840: 206f 7220 6861 7665 2074 6f20 6265 2073   or have to be s
-00000850: 6574 2129 01da 0569 6e64 6578 720e 0000  et!)...indexr...
-00000860: 00da 056c 6162 656c 2901 da07 636f 6c75  ...label)...colu
-00000870: 6d6e 7354 2901 da07 6261 7463 6865 6429  mnsT)...batched)
-00000880: 0272 1600 0000 da04 7465 7374 2912 da03  .r......test)...
-00000890: 7375 6dda 0a56 616c 7565 4572 726f 72da  sum..ValueError.
-000008a0: 0261 32da 0764 6174 6173 6574 da0d 7574  .a2..dataset..ut
-000008b0: 696c 735f 6461 7461 7365 74da 1661 7373  ils_dataset..ass
-000008c0: 6572 745f 6b65 7973 5f69 6e5f 6461 7461  ert_keys_in_data
-000008d0: 7365 74da 0c6c 6f61 645f 6461 7461 7365  set..load_datase
-000008e0: 74da 1672 6573 6574 5f69 6e64 6578 5f63  t..reset_index_c
-000008f0: 6f6f 7264 696e 6174 65da 0373 656c da09  oordinate..sel..
-00000900: 746f 5f70 616e 6461 73da 0672 656e 616d  to_pandas..renam
-00000910: 65da 0864 6174 6173 6574 73da 0744 6174  e..datasets..Dat
-00000920: 6173 6574 da0b 6672 6f6d 5f70 616e 6461  aset..from_panda
-00000930: 73da 036d 6170 7210 0000 00da 0b44 6174  s..mapr......Dat
-00000940: 6173 6574 4469 6374 da06 7365 6c65 6374  asetDict..select
-00000950: 290c 7209 0000 0072 1300 0000 7214 0000  ).r....r....r...
-00000960: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000970: 7218 0000 0072 1900 0000 da02 6466 721e  r....r......dfr.
-00000980: 0000 00da 0b64 6174 6173 6574 735f 6473  .....datasets_ds
-00000990: da06 746f 6b5f 6473 720a 0000 0072 0a00  ..tok_dsr....r..
-000009a0: 0000 720b 0000 00da 0562 7569 6c64 2300  ..r......build#.
-000009b0: 0000 7326 0000 001c 1b16 0114 0104 010e  ..s&............
-000009c0: 010c 010c 0110 010c 010c 010c 0110 0114  ................
-000009d0: 0104 0104 0208 0208 0104 fe04 ff7a 1844  .............z.D
-000009e0: 6174 6173 6574 4875 6767 696e 6746 6163  atasetHuggingFac
-000009f0: 652e 6275 696c 6429 0146 2904 5472 1100  e.build).F).Tr..
-00000a00: 0000 7212 0000 0054 2912 da08 5f5f 6e61  ..r....T)...__na
-00000a10: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000a20: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000a30: 5f5f 646f 635f 5fda 0373 7472 da04 626f  __doc__..str..bo
-00000a40: 6f6c 720c 0000 00da 0464 6963 7472 1000  olr......dictr..
-00000a50: 0000 da06 7861 7272 6179 722d 0000 00da  ....xarrayr-....
-00000a60: 026e 70da 076e 6461 7272 6179 da01 74da  .np..ndarray..t.
-00000a70: 0555 6e69 6f6e 722c 0000 0072 3000 0000  .Unionr,...r0...
-00000a80: 7235 0000 0072 0a00 0000 720a 0000 0072  r5...r....r....r
-00000a90: 0a00 0000 720b 0000 0072 0200 0000 0a00  ....r....r......
-00000aa0: 0000 7332 0000 0008 0004 0114 0e0e 0702  ..s2............
-00000ab0: 0802 0102 0102 0104 f804 0202 fe08 0302  ................
-00000ac0: fd08 0402 fc02 0502 fb02 0602 fa02 0702  ................
-00000ad0: f902 0802 f810 090e f772 0200 0000 290a  .........r....).
-00000ae0: da06 7479 7069 6e67 7240 0000 00da 1761  ..typingr@.....a
-00000af0: 322e 6461 7461 7365 742e 6c6f 6164 5f64  2.dataset.load_d
-00000b00: 6174 6173 6574 7223 0000 0072 2c00 0000  atasetr#...r,...
-00000b10: da05 6e75 6d70 7972 3e00 0000 7205 0000  ..numpyr>...r...
-00000b20: 0072 3d00 0000 7202 0000 0072 0a00 0000  .r=...r....r....
-00000b30: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000b40: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
-00000b50: 0000 0800 0802 0801 0801 0801 0801 1203  ................
+00000000: 696d 706f 7274 2074 7970 696e 6720 6173  import typing as
+00000010: 2074 0a0a 696d 706f 7274 2061 322e 6461   t..import a2.da
+00000020: 7461 7365 742e 6c6f 6164 5f64 6174 6173  taset.load_datas
+00000030: 6574 0a69 6d70 6f72 7420 6461 7461 7365  et.import datase
+00000040: 7473 0a69 6d70 6f72 7420 6e75 6d70 7920  ts.import numpy 
+00000050: 6173 206e 700a 696d 706f 7274 2074 7261  as np.import tra
+00000060: 6e73 666f 726d 6572 730a 696d 706f 7274  nsformers.import
+00000070: 2078 6172 7261 790a 0a0a 636c 6173 7320   xarray...class 
+00000080: 4461 7461 7365 7448 7567 6769 6e67 4661  DatasetHuggingFa
+00000090: 6365 3a0a 2020 2020 2222 220a 2020 2020  ce:.    """.    
+000000a0: 5573 6564 2074 6f20 6372 6561 7465 2064  Used to create d
+000000b0: 6174 6173 6574 2069 6e20 4875 6767 696e  ataset in Huggin
+000000c0: 6720 4661 6365 2066 6f72 6d61 742e 0a0a  g Face format...
+000000d0: 2020 2020 4174 7472 6962 7574 6573 0a20      Attributes. 
+000000e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000000f0: 2020 746f 6b65 6e69 7a65 7220 3a20 4875    tokenizer : Hu
+00000100: 6767 696e 6720 4661 6365 2074 6f6b 656e  gging Face token
+00000110: 697a 6572 0a0a 2020 2020 4e6f 7465 730a  izer..    Notes.
+00000120: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5573      -----.    Us
+00000130: 6520 4875 6767 696e 6720 4661 6365 206d  e Hugging Face m
+00000140: 6f64 656c 2066 6f6c 6465 7273 2074 6f20  odel folders to 
+00000150: 696e 6974 6961 6c69 7a65 2074 6f6b 656e  initialize token
+00000160: 697a 6572 2061 6e64 2062 7569 6c64 2061  izer and build a
+00000170: 0a20 2020 2048 7567 6769 6e67 2046 6163  .    Hugging Fac
+00000180: 6520 6461 7461 7365 7420 6672 6f6d 2061  e dataset from a
+00000190: 6e20 7861 7272 6179 2064 6174 6173 6574  n xarray dataset
+000001a0: 2e0a 2020 2020 4361 6e20 6265 2072 6575  ..    Can be reu
+000001b0: 7365 6420 746f 2062 696c 6420 7468 6520  sed to bild the 
+000001c0: 7465 7374 2064 6174 6173 6574 2066 6f72  test dataset for
+000001d0: 2076 616c 6964 6174 696f 6e2e 0a20 2020   validation..   
+000001e0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+000001f0: 696e 6974 5f5f 2873 656c 662c 206d 6f64  init__(self, mod
+00000200: 656c 5f66 6f6c 6465 723a 2073 7472 2c20  el_folder: str, 
+00000210: 7573 655f 6661 7374 3a20 626f 6f6c 203d  use_fast: bool =
+00000220: 2046 616c 7365 293a 0a20 2020 2020 2020   False):.       
+00000230: 2073 656c 662e 6d6f 6465 6c5f 666f 6c64   self.model_fold
+00000240: 6572 203d 206d 6f64 656c 5f66 6f6c 6465  er = model_folde
+00000250: 720a 2020 2020 2020 2020 7365 6c66 2e74  r.        self.t
+00000260: 6f6b 656e 697a 6572 203d 2074 7261 6e73  okenizer = trans
+00000270: 666f 726d 6572 732e 4175 746f 546f 6b65  formers.AutoToke
+00000280: 6e69 7a65 722e 6672 6f6d 5f70 7265 7472  nizer.from_pretr
+00000290: 6169 6e65 6428 0a20 2020 2020 2020 2020  ained(.         
+000002a0: 2020 206d 6f64 656c 5f66 6f6c 6465 722c     model_folder,
+000002b0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+000002c0: 5f66 6173 743d 4661 6c73 652c 0a20 2020  _fast=False,.   
+000002d0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+000002e0: 5f74 6f6b 5f66 756e 6328 7365 6c66 2c20  _tok_func(self, 
+000002f0: 783a 2064 6963 7429 3a0a 2020 2020 2020  x: dict):.      
+00000300: 2020 7265 7475 726e 2073 656c 662e 746f    return self.to
+00000310: 6b65 6e69 7a65 7228 785b 2269 6e70 7574  kenizer(x["input
+00000320: 7322 5d2c 2070 6164 6469 6e67 3d54 7275  s"], padding=Tru
+00000330: 6529 0a0a 2020 2020 6465 6620 6275 696c  e)..    def buil
+00000340: 6428 0a20 2020 2020 2020 2073 656c 662c  d(.        self,
+00000350: 0a20 2020 2020 2020 2064 733a 2078 6172  .        ds: xar
+00000360: 7261 792e 4461 7461 7365 742c 0a20 2020  ray.Dataset,.   
+00000370: 2020 2020 2069 6e64 6963 6573 5f74 7261       indices_tra
+00000380: 696e 3a20 6e70 2e6e 6461 7272 6179 207c  in: np.ndarray |
+00000390: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
+000003a0: 6e64 6963 6573 5f76 616c 6964 6174 653a  ndices_validate:
+000003b0: 206e 702e 6e64 6172 7261 7920 7c20 4e6f   np.ndarray | No
+000003c0: 6e65 2c0a 2020 2020 2020 2020 7472 6169  ne,.        trai
+000003d0: 6e3a 2062 6f6f 6c20 3d20 5472 7565 2c0a  n: bool = True,.
+000003e0: 2020 2020 2020 2020 6b65 795f 696e 7075          key_inpu
+000003f0: 7473 3a20 7374 7220 3d20 2274 6578 7422  ts: str = "text"
+00000400: 2c0a 2020 2020 2020 2020 6b65 795f 6c61  ,.        key_la
+00000410: 6265 6c3a 2073 7472 203d 2022 7261 696e  bel: str = "rain
+00000420: 696e 6722 2c0a 2020 2020 2020 2020 7265  ing",.        re
+00000430: 7365 745f 696e 6465 783a 2062 6f6f 6c20  set_index: bool 
+00000440: 3d20 5472 7565 2c0a 2020 2020 2920 2d3e  = True,.    ) ->
+00000450: 2074 2e55 6e69 6f6e 5b64 6174 6173 6574   t.Union[dataset
+00000460: 732e 4461 7461 7365 742c 2064 6174 6173  s.Dataset, datas
+00000470: 6574 732e 4461 7461 7365 7444 6963 745d  ets.DatasetDict]
+00000480: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00000490: 2020 2020 2020 4372 6561 7465 2048 7567        Create Hug
+000004a0: 6769 6e67 2046 6163 6520 6461 7461 7365  ging Face datase
+000004b0: 7420 2864 6174 6173 6574 732e 4461 7461  t (datasets.Data
+000004c0: 7365 7444 6963 7429 2066 726f 6d20 7861  setDict) from xa
+000004d0: 7272 6179 2064 6174 6173 6574 0a0a 2020  rray dataset..  
+000004e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000004f0: 3a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  :.        ------
+00000500: 2d2d 2d2d 0a20 2020 2020 2020 2064 733a  ----.        ds:
+00000510: 2078 6172 7261 7920 6461 7461 7365 740a   xarray dataset.
+00000520: 2020 2020 2020 2020 696e 6469 6365 735f          indices_
+00000530: 7472 6169 6e3a 2056 6172 6961 626c 6520  train: Variable 
+00000540: 2769 6e64 6578 2720 7661 6c75 6573 2074  'index' values t
+00000550: 6861 7420 6172 6520 7573 6564 2066 6f72  hat are used for
+00000560: 2074 7261 696e 696e 670a 2020 2020 2020   training.      
+00000570: 2020 696e 6469 6365 735f 7661 6c69 6461    indices_valida
+00000580: 7465 3a20 5661 7269 6162 6c65 2027 696e  te: Variable 'in
+00000590: 6465 7827 2076 616c 7565 7320 7468 6174  dex' values that
+000005a0: 2061 7265 2075 7365 6420 666f 7220 7661   are used for va
+000005b0: 6c69 6461 7469 6f6e 0a20 2020 2020 2020  lidation.       
+000005c0: 2074 7261 696e 3a20 4966 2074 6865 2064   train: If the d
+000005d0: 6174 6173 6574 2069 7320 7573 6564 2066  ataset is used f
+000005e0: 6f72 2074 7261 696e 696e 670a 2020 2020  or training.    
+000005f0: 2020 2020 6b65 795f 696e 7075 7473 3a20      key_inputs: 
+00000600: 4b65 7920 6f66 2076 6172 6961 626c 6520  Key of variable 
+00000610: 7573 6564 2061 7320 696e 7075 7420 746f  used as input to
+00000620: 206d 6f64 656c 0a20 2020 2020 2020 206b   model.        k
+00000630: 6579 5f6c 6162 656c 3a20 4b65 7920 6f66  ey_label: Key of
+00000640: 2076 6172 6961 626c 6520 7573 6564 2061   variable used a
+00000650: 7320 6c61 6265 6c20 666f 7220 7472 6169  s label for trai
+00000660: 6e69 6e67 0a20 2020 2020 2020 2072 6573  ning.        res
+00000670: 6574 5f69 6e64 6578 3a20 5265 7365 7420  et_index: Reset 
+00000680: 696e 6465 7820 636f 6f72 6469 6e61 7465  index coordinate
+00000690: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000006a0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000006b0: 2d0a 2020 2020 2020 2020 6461 7461 7365  -.        datase
+000006c0: 7473 2e44 6174 6173 6574 4469 6374 0a20  ts.DatasetDict. 
+000006d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000006e0: 2020 2069 6620 7472 6169 6e20 616e 6420     if train and 
+000006f0: 2873 756d 285b 696e 6469 6365 735f 7472  (sum([indices_tr
+00000700: 6169 6e20 6973 204e 6f6e 652c 2069 6e64  ain is None, ind
+00000710: 6963 6573 5f76 616c 6964 6174 6520 6973  ices_validate is
+00000720: 204e 6f6e 655d 2920 3d3d 2031 293a 0a20   None]) == 1):. 
+00000730: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00000740: 2056 616c 7565 4572 726f 7228 6622 7b69   ValueError(f"{i
+00000750: 6e64 6963 6573 5f74 7261 696e 3d7d 2061  ndices_train=} a
+00000760: 6e64 207b 696e 6469 6365 735f 7661 6c69  nd {indices_vali
+00000770: 6461 7465 7d20 6361 6e20 6569 7468 6572  date} can either
+00000780: 2062 6520 626f 7468 204e 6f6e 6520 6f72   be both None or
+00000790: 2068 6176 6520 746f 2062 6520 7365 7421   have to be set!
+000007a0: 2229 0a20 2020 2020 2020 2061 322e 6461  ").        a2.da
+000007b0: 7461 7365 742e 7574 696c 735f 6461 7461  taset.utils_data
+000007c0: 7365 742e 6173 7365 7274 5f6b 6579 735f  set.assert_keys_
+000007d0: 696e 5f64 6174 6173 6574 2864 732c 205b  in_dataset(ds, [
+000007e0: 6b65 795f 696e 7075 7473 2c20 6b65 795f  key_inputs, key_
+000007f0: 6c61 6265 6c5d 290a 2020 2020 2020 2020  label]).        
+00000800: 6966 2072 6573 6574 5f69 6e64 6578 3a0a  if reset_index:.
+00000810: 2020 2020 2020 2020 2020 2020 6473 203d              ds =
+00000820: 2061 322e 6461 7461 7365 742e 6c6f 6164   a2.dataset.load
+00000830: 5f64 6174 6173 6574 2e72 6573 6574 5f69  _dataset.reset_i
+00000840: 6e64 6578 5f63 6f6f 7264 696e 6174 6528  ndex_coordinate(
+00000850: 6473 290a 2020 2020 2020 2020 6966 206e  ds).        if n
+00000860: 6f74 2074 7261 696e 2061 6e64 2069 6e64  ot train and ind
+00000870: 6963 6573 5f76 616c 6964 6174 6520 6973  ices_validate is
+00000880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00000890: 2020 2020 2020 2064 7320 3d20 6473 2e73         ds = ds.s
+000008a0: 656c 2869 6e64 6578 3d69 6e64 6963 6573  el(index=indices
+000008b0: 5f76 616c 6964 6174 6529 0a20 2020 2020  _validate).     
+000008c0: 2020 2064 6620 3d20 6473 5b5b 6b65 795f     df = ds[[key_
+000008d0: 696e 7075 7473 2c20 6b65 795f 6c61 6265  inputs, key_labe
+000008e0: 6c5d 5d2e 746f 5f70 616e 6461 7328 290a  l]].to_pandas().
+000008f0: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+00000900: 2074 2e4d 6170 7069 6e67 203d 207b 6b65   t.Mapping = {ke
+00000910: 795f 696e 7075 7473 3a20 2269 6e70 7574  y_inputs: "input
+00000920: 7322 2c20 6b65 795f 6c61 6265 6c3a 2022  s", key_label: "
+00000930: 6c61 6265 6c22 7d0a 2020 2020 2020 2020  label"}.        
+00000940: 6466 203d 2064 662e 7265 6e61 6d65 2863  df = df.rename(c
+00000950: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 2920  olumns=columns) 
+00000960: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+00000970: 2020 2020 2020 2020 6461 7461 7365 7473          datasets
+00000980: 5f64 7320 3d20 6461 7461 7365 7473 2e44  _ds = datasets.D
+00000990: 6174 6173 6574 2e66 726f 6d5f 7061 6e64  ataset.from_pand
+000009a0: 6173 2864 6629 0a20 2020 2020 2020 2074  as(df).        t
+000009b0: 6f6b 5f64 7320 3d20 6461 7461 7365 7473  ok_ds = datasets
+000009c0: 5f64 732e 6d61 7028 7365 6c66 2e5f 746f  _ds.map(self._to
+000009d0: 6b5f 6675 6e63 2c20 6261 7463 6865 643d  k_func, batched=
+000009e0: 5472 7565 290a 2020 2020 2020 2020 6966  True).        if
+000009f0: 206e 6f74 2074 7261 696e 206f 7220 2869   not train or (i
+00000a00: 6e64 6963 6573 5f74 7261 696e 2069 7320  ndices_train is 
+00000a10: 4e6f 6e65 2061 6e64 2069 6e64 6963 6573  None and indices
+00000a20: 5f76 616c 6964 6174 6520 6973 204e 6f6e  _validate is Non
+00000a30: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00000a40: 7265 7475 726e 2074 6f6b 5f64 730a 2020  return tok_ds.  
+00000a50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00000a60: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00000a70: 6174 6173 6574 732e 4461 7461 7365 7444  atasets.DatasetD
+00000a80: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+00000a90: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000aa0: 2020 2020 2020 2020 2020 2022 7472 6169             "trai
+00000ab0: 6e22 3a20 746f 6b5f 6473 2e73 656c 6563  n": tok_ds.selec
+00000ac0: 7428 696e 6469 6365 735f 7472 6169 6e29  t(indices_train)
+00000ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000ae0: 2020 2020 2020 2274 6573 7422 3a20 746f        "test": to
+00000af0: 6b5f 6473 2e73 656c 6563 7428 696e 6469  k_ds.select(indi
+00000b00: 6365 735f 7661 6c69 6461 7465 292c 0a20  ces_validate),. 
+00000b10: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00000b20: 0a20 2020 2020 2020 2020 2020 2029 0a    .            ).
```

### Comparing `a2-0.3.5/src/a2/training/__pycache__/evaluate_hugging.cpython-310.pyc` & `a2-0.3.6/src/a2/training/evaluate_hugging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,250 +1,264 @@
-00000000: 6f0d 0d0a 0000 0000 b654 7f64 7510 0000  o........T.du...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0014 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c03 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6401 6c06 5a05 6400 6401 6c07 5a05 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6401 6c08 5a08 6400 6401 6c09 5a0a 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6401 6c0b 5a0b 6400 6401 6c0c 5a0c 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6401 6c0d 5a0d 6402 650d 6a0e 6403 650a  d.l.Z.d.e.j.d.e.
-00000090: 6a0f 6401 4200 6404 650a 6a0f 6405 650a  j.d.B.d.e.j.d.e.
-000000a0: 6a0f 6406 650d 6a0e 660a 6407 6408 8404  j.d.e.j.f.d.d...
-000000b0: 5a10 6409 6502 6a11 6508 6a0e 6508 6a12  Z.d.e.j.e.j.e.j.
-000000c0: 6602 1900 640a 650c 6a13 6406 6502 6a14  f...d.e.j.d.e.j.
-000000d0: 650a 6a0f 650a 6a0f 6602 1900 6606 640b  e.j.e.j.f...f.d.
-000000e0: 640c 8404 5a15 090d 090e 0901 090f 6418  d...Z.........d.
-000000f0: 6402 650d 6a0e 6410 650a 6a0f 6411 6516  d.e.j.d.e.j.d.e.
-00000100: 6412 6516 6413 6516 6414 6502 6a17 650c  d.e.d.e.d.e.j.e.
-00000110: 6a18 1900 6415 6519 6406 6502 6a14 650a  j...d.e.d.e.j.e.
-00000120: 6a0f 650a 6a0f 650a 6a0f 6603 1900 6610  j.e.j.e.j.f...f.
-00000130: 6416 6417 8405 5a1a 6401 5300 2919 e900  d.d...Z.d.S.)...
-00000140: 0000 004e da02 6473 da0c 696e 6469 6365  ...N..ds..indice
-00000150: 735f 7465 7374 da0b 7072 6564 6963 7469  s_test..predicti
-00000160: 6f6e 73da 1870 7265 6469 6374 696f 6e5f  ons..prediction_
-00000170: 7072 6f62 6162 696c 6974 6965 73da 0672  probabilities..r
-00000180: 6574 7572 6e63 0400 0000 0000 0000 0000  eturnc..........
-00000190: 0000 0500 0000 0400 0000 4300 0000 7364  ..........C...sd
-000001a0: 0000 007c 0164 0175 0172 0b7c 006a 007c  ...|.d.u.r.|.j.|
-000001b0: 0164 028d 017d 046e 047c 00a0 01a1 007d  .d...}.n.|.....}
-000001c0: 0464 0367 017c 0266 027c 0464 043c 0064  .d.g.|.f.|.d.<.d
-000001d0: 0367 017c 0364 0164 0185 0264 0566 0219  .g.|.d.d...d.f..
-000001e0: 0066 027c 0464 063c 0064 0367 017c 0364  .f.|.d.<.d.g.|.d
-000001f0: 0164 0185 0264 0766 0219 0066 027c 0464  .d...d.f...f.|.d
-00000200: 083c 007c 0453 0029 0961 cd01 0000 0a20  .<.|.S.).a..... 
-00000210: 2020 2043 6f6e 7374 7275 6374 2074 6573     Construct tes
-00000220: 7420 6461 7461 7365 7420 7768 6572 6520  t dataset where 
-00000230: 7465 7374 2064 6174 6120 6973 2064 6566  test data is def
-00000240: 696e 6564 2062 7920 7468 6569 7220 696e  ined by their in
-00000250: 6469 6365 730a 2020 2020 616e 6420 636f  dices.    and co
-00000260: 7272 6573 706f 6e64 696e 6720 7072 6564  rresponding pred
-00000270: 6963 7469 6f6e 7320 616e 6420 7072 6564  ictions and pred
-00000280: 6963 7469 6f6e 5f70 726f 6261 6269 6c69  iction_probabili
-00000290: 7469 6573 0a0a 2020 2020 5061 7261 6d65  ties..    Parame
-000002a0: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
-000002b0: 2d2d 2d2d 0a20 2020 2064 733a 2078 6172  ----.    ds: xar
-000002c0: 7261 7920 6461 7461 7365 740a 2020 2020  ray dataset.    
-000002d0: 696e 6469 6365 735f 7465 7374 3a20 5661  indices_test: Va
-000002e0: 7269 6162 6c65 2027 696e 6465 7827 2076  riable 'index' v
-000002f0: 616c 7565 7320 7468 6174 2061 7265 2075  alues that are u
-00000300: 7365 6420 666f 7220 7465 7374 696e 670a  sed for testing.
-00000310: 2020 2020 7072 6564 6963 7469 6f6e 733a      predictions:
-00000320: 2050 7265 6469 6374 6564 206c 6162 656c   Predicted label
-00000330: 730a 2020 2020 7072 6564 6963 7469 6f6e  s.    prediction
-00000340: 5f70 726f 6261 6269 6c69 7469 6573 3a20  _probabilities: 
-00000350: 5072 6564 6963 7469 6f6e 2070 726f 6261  Prediction proba
-00000360: 6269 6c69 7479 2066 6f72 2062 6f74 6820  bility for both 
-00000370: 6c61 6265 6c73 2c0a 2020 2020 2020 2020  labels,.        
-00000380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000390: 2020 2020 2020 7368 6170 6520 3d20 5b6e        shape = [n
-000003a0: 5f74 6573 7473 2c20 325d 0a0a 2020 2020  _tests, 2]..    
-000003b0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-000003c0: 2d2d 2d0a 2020 2020 7861 7272 6179 2e44  ---.    xarray.D
-000003d0: 6174 6173 6574 0a20 2020 204e a901 da05  ataset.    N....
-000003e0: 696e 6465 7872 0800 0000 da0a 7072 6564  indexr......pred
-000003f0: 6963 7469 6f6e 7201 0000 00da 2270 7265  ictionr....."pre
-00000400: 6469 6374 696f 6e5f 7072 6f62 6162 696c  diction_probabil
-00000410: 6974 795f 6e6f 745f 7261 696e 696e 67e9  ity_not_raining.
-00000420: 0100 0000 da1e 7072 6564 6963 7469 6f6e  ......prediction
-00000430: 5f70 726f 6261 6269 6c69 7479 5f72 6169  _probability_rai
-00000440: 6e69 6e67 2902 da03 7365 6cda 0463 6f70  ning)...sel..cop
-00000450: 7929 0572 0200 0000 7203 0000 0072 0400  y).r....r....r..
-00000460: 0000 7205 0000 00da 0764 735f 7465 7374  ..r......ds_test
-00000470: a900 7210 0000 00fa 3e2f 686f 6d65 2f6b  ..r.....>/home/k
-00000480: 7269 7374 6961 6e2f 5072 6f6a 6563 7473  ristian/Projects
-00000490: 2f61 322f 7372 632f 6132 2f74 7261 696e  /a2/src/a2/train
-000004a0: 696e 672f 6576 616c 7561 7465 5f68 7567  ing/evaluate_hug
-000004b0: 6769 6e67 2e70 79da 0d62 7569 6c64 5f64  ging.py..build_d
-000004c0: 735f 7465 7374 0f00 0000 7316 0000 0008  s_test....s.....
-000004d0: 160e 0108 020e 0104 020e 0108 fe04 050e  ................
-000004e0: 0108 fe04 0472 1200 0000 da07 6461 7461  .....r......data
-000004f0: 7365 74da 0774 7261 696e 6572 6302 0000  set..trainerc...
-00000500: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00000510: 0043 0000 0073 3600 0000 7400 6a01 6a02  .C...s6...t.j.j.
-00000520: 6a03 7400 a004 7c01 a005 7c00 a101 6a06  j.t...|...|...j.
-00000530: a101 6401 6402 8d02 a007 a100 7d02 7c02  ..d.d.......}.|.
-00000540: a008 6403 a101 7d03 7c03 7c02 6602 5300  ..d...}.|.|.f.S.
-00000550: 2904 7aeb 0a20 2020 204d 616b 6520 7072  ).z..    Make pr
-00000560: 6564 6963 7469 6f6e 7320 6f6e 2048 7567  edictions on Hug
-00000570: 6769 6e67 2046 6163 6520 6461 7461 7365  ging Face datase
-00000580: 7420 6261 7365 640a 2020 2020 6f6e 2048  t based.    on H
-00000590: 7567 6769 6e67 2046 6163 6520 7472 6169  ugging Face trai
-000005a0: 6e65 7220 6f62 6a65 6374 0a0a 2020 2020  ner object..    
-000005b0: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
-000005d0: 6174 6173 6574 3a20 4875 6767 696e 6720  ataset: Hugging 
-000005e0: 4661 6365 2064 6174 6173 6574 0a20 2020  Face dataset.   
-000005f0: 2074 7261 696e 6572 3a20 4875 6767 696e   trainer: Huggin
-00000600: 6720 4661 6365 2074 7261 696e 6572 0a0a  g Face trainer..
-00000610: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00000620: 2d2d 2d2d 2d2d 2d0a 2020 2020 7861 7272  -------.    xarr
-00000630: 6179 2e44 6174 6173 6574 0a20 2020 2072  ay.Dataset.    r
-00000640: 0b00 0000 2901 da03 6469 6de9 ffff ffff  ....)...dim.....
-00000650: 2909 da05 746f 7263 68da 026e 6eda 0a66  )...torch..nn..f
-00000660: 756e 6374 696f 6e61 6cda 0773 6f66 746d  unctional..softm
-00000670: 6178 da06 5465 6e73 6f72 da07 7072 6564  ax..Tensor..pred
-00000680: 6963 7472 0400 0000 da05 6e75 6d70 79da  ictr......numpy.
-00000690: 0661 7267 6d61 7829 0472 1300 0000 7214  .argmax).r....r.
-000006a0: 0000 0072 0500 0000 7204 0000 0072 1000  ...r....r....r..
-000006b0: 0000 7210 0000 0072 1100 0000 da0f 7072  ..r....r......pr
-000006c0: 6564 6963 745f 6461 7461 7365 7435 0000  edict_dataset5..
-000006d0: 0073 0e00 0000 0811 1201 04ff 0402 02fe  .s..............
-000006e0: 0a03 0801 721f 0000 00da 0474 6578 74da  ....r......text.
-000006f0: 0772 6169 6e69 6e67 54da 1069 6e64 6963  .rainingT..indic
-00000700: 6573 5f76 616c 6964 6174 65da 0c66 6f6c  es_validate..fol
-00000710: 6465 725f 6d6f 6465 6cda 0a6b 6579 5f69  der_model..key_i
-00000720: 6e70 7574 73da 096b 6579 5f6c 6162 656c  nputs..key_label
-00000730: da10 666f 6c64 6572 5f74 6f6b 656e 697a  ..folder_tokeniz
-00000740: 6572 da04 6670 3136 6307 0000 0000 0000  er..fp16c.......
-00000750: 0000 0000 000e 0000 0008 0000 0043 0000  .............C..
-00000760: 0073 e200 0000 7400 6a01 6a02 a003 a100  .s....t.j.j.....
-00000770: 7310 6401 7d06 7404 a005 6402 7c06 9b02  s.d.}.t...d.|...
-00000780: 9d02 a101 0100 7c05 6403 7500 7216 7c02  ......|.d.u.r.|.
-00000790: 7d05 7400 6a01 6a06 a007 7c05 a101 7d07  }.t.j.j...|...}.
-000007a0: 7c07 6a08 7c00 7409 a00a 6700 a101 7c01  |.j.|.t...g...|.
-000007b0: 6401 7c03 7c04 6404 8d06 7d08 7400 6a01  d.|.|.d...}.t.j.
-000007c0: 6a0b a00c 7c02 a101 7d09 7c09 6a0d 7c08  j...|...}.|.j.|.
-000007d0: 7c07 6a0e 6405 6401 7c06 6406 6407 8d06  |.j.d.d.|.d.d...
-000007e0: 7d0a 740f a010 6408 a101 0100 7411 a012  }.t...d.....t...
-000007f0: a100 8f0f 0100 7413 7c08 7c0a 8302 5c02  ......t.|.|...\.
-00000800: 7d0b 7d0c 5700 6403 0400 0400 8303 0100  }.}.W.d.........
-00000810: 6e08 3100 7359 7701 0100 0100 0100 5900  n.1.sYw.......Y.
-00000820: 0100 740f a010 6409 a101 0100 7c00 6a14  ..t...d.....|.j.
-00000830: 7c01 640a 8d01 7c04 1900 6a15 7d0d 7c0d  |.d...|...j.}.|.
-00000840: 7c0b 7c0c 6603 5300 290b 6127 0300 000a  |.|.f.S.).a'....
-00000850: 2020 2020 4d61 6b65 2070 7265 6469 6374      Make predict
-00000860: 696f 6e73 206f 6e20 6c6f 6164 6564 2074  ions on loaded t
-00000870: 7261 696e 6564 2048 7567 6769 6e67 2046  rained Hugging F
-00000880: 6163 6520 6d6f 6465 6c0a 0a20 2020 2057  ace model..    W
-00000890: 4152 4e49 4e47 3a20 5472 7920 7573 696e  ARNING: Try usin
-000008a0: 6720 6f72 6967 696e 616c 2066 6f6c 6465  g original folde
-000008b0: 7220 666f 7220 6066 6f6c 6465 725f 746f  r for `folder_to
-000008c0: 6b65 6e69 7a65 7260 0a20 2020 2020 2020  kenizer`.       
-000008d0: 2020 2020 2020 6966 2072 756e 2069 6e74        if run int
-000008e0: 6f20 6973 7375 6573 2077 6865 6e20 696e  o issues when in
-000008f0: 6974 6961 6c69 7a69 6e67 2074 6f6b 656e  itializing token
-00000900: 697a 6572 210a 2020 2020 5061 7261 6d65  izer!.    Parame
-00000910: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
-00000920: 2d2d 2d2d 0a20 2020 2064 733a 2058 6172  ----.    ds: Xar
-00000930: 7261 7920 6461 7461 7365 740a 2020 2020  ray dataset.    
-00000940: 696e 6469 6365 735f 7661 6c69 6461 7465  indices_validate
-00000950: 3a20 5661 7269 6162 6c65 2027 696e 6465  : Variable 'inde
-00000960: 7827 2076 616c 7565 7320 7468 6174 2061  x' values that a
-00000970: 7265 2075 7365 6420 666f 7220 7661 6c69  re used for vali
-00000980: 6461 7469 6f6e 0a20 2020 2066 6f6c 6465  dation.    folde
-00000990: 725f 6d6f 6465 6c3a 2046 6f6c 6465 7220  r_model: Folder 
-000009a0: 6f66 2070 7265 7472 6169 6e65 6420 6d6f  of pretrained mo
-000009b0: 6465 6c0a 2020 2020 6b65 795f 696e 7075  del.    key_inpu
-000009c0: 7473 3a20 4b65 7920 6f66 2076 6172 6961  ts: Key of varia
-000009d0: 626c 6520 7573 6564 2061 7320 696e 7075  ble used as inpu
-000009e0: 7420 746f 206d 6f64 656c 0a20 2020 206b  t to model.    k
-000009f0: 6579 5f6c 6162 656c 3a20 4b65 7920 6f66  ey_label: Key of
-00000a00: 2076 6172 6961 626c 6520 7573 6564 2061   variable used a
-00000a10: 7320 6c61 6265 6c20 666f 7220 7472 6169  s label for trai
-00000a20: 6e69 6e67 0a20 2020 2066 6f6c 6465 725f  ning.    folder_
-00000a30: 746f 6b65 6e69 7a65 723a 2046 6f6c 6465  tokenizer: Folde
-00000a40: 7220 6f66 206f 7269 6769 6e61 6c20 6d6f  r of original mo
-00000a50: 6465 6c20 646f 776e 6c6f 6164 6564 2066  del downloaded f
-00000a60: 726f 6d20 4875 7567 696e 6720 4661 6365  rom Huuging Face
-00000a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a80: 2020 2020 2020 2028 6d61 7920 7275 6e20         (may run 
-00000a90: 696e 746f 2069 7373 7565 7320 6966 2075  into issues if u
-00000aa0: 7365 2066 6f6c 6465 725f 746f 6b65 6e69  se folder_tokeni
-00000ab0: 7a65 723d 666f 6c64 6572 5f6d 6f64 656c  zer=folder_model
-00000ac0: 290a 2020 2020 6670 3136 3a20 5768 6574  ).    fp16: Whet
-00000ad0: 6865 7220 746f 2075 7365 2066 7031 3620  her to use fp16 
-00000ae0: 3136 2d62 6974 2028 6d69 7865 6429 2070  16-bit (mixed) p
-00000af0: 7265 6369 7369 6f6e 2074 7261 696e 696e  recision trainin
-00000b00: 670a 2020 2020 2020 2020 2020 696e 7374  g.          inst
-00000b10: 6561 6420 6f66 2033 322d 6269 7420 7472  ead of 32-bit tr
-00000b20: 6169 6e69 6e67 2e0a 0a20 2020 2052 6574  aining...    Ret
-00000b30: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00000b40: 0a20 2020 2074 7275 7468 2c20 7072 6564  .    truth, pred
-00000b50: 6963 7469 6f6e 732c 2070 7265 6469 6374  ictions, predict
-00000b60: 696f 6e5f 7072 6f62 6162 696c 6974 6965  ion_probabilitie
-00000b70: 730a 2020 2020 467a 4331 362d 6269 7420  s.    FzC16-bit 
-00000b80: 6576 616c 7561 7469 6f6e 206f 6e6c 7920  evaluation only 
-00000b90: 6176 6169 6c61 626c 6520 6f6e 2073 7973  available on sys
-00000ba0: 7465 6d73 2077 6974 6820 4750 552e 2053  tems with GPU. S
-00000bb0: 6574 7469 6e67 2066 7031 363d 4e29 03da  etting fp16=N)..
-00000bc0: 0574 7261 696e 7224 0000 0072 2500 0000  .trainr$...r%...
-00000bd0: 7a02 2e2f 5429 05da 0974 6f6b 656e 697a  z../T)...tokeniz
-00000be0: 6572 da0d 666f 6c64 6572 5f6f 7574 7075  er..folder_outpu
-00000bf0: 74da 0c68 7970 6572 5f74 756e 696e 6772  t..hyper_tuningr
-00000c00: 2700 0000 da08 6576 616c 7561 7465 da0a  '.....evaluate..
-00000c10: 7072 6564 6963 7469 6e67 7a0f 646f 6e65  predictingz.done
-00000c20: 2070 7265 6469 6374 696e 6772 0700 0000   predictingr....
-00000c30: 2916 da02 6132 da08 7472 6169 6e69 6e67  )...a2..training
-00000c40: da0e 7574 696c 735f 7472 6169 6e69 6e67  ..utils_training
-00000c50: da0d 6770 755f 6176 6169 6c61 626c 65da  ..gpu_available.
-00000c60: 0877 6172 6e69 6e67 73da 0477 6172 6eda  .warnings..warn.
-00000c70: 0f64 6174 6173 6574 5f68 7567 6769 6e67  .dataset_hugging
-00000c80: da12 4461 7461 7365 7448 7567 6769 6e67  ..DatasetHugging
-00000c90: 4661 6365 da05 6275 696c 64da 026e 70da  Face..build..np.
-00000ca0: 076e 6461 7272 6179 da10 7472 6169 6e69  .ndarray..traini
-00000cb0: 6e67 5f68 7567 6769 6e67 da17 4875 6767  ng_hugging..Hugg
-00000cc0: 696e 6746 6163 6554 7261 696e 6572 436c  ingFaceTrainerCl
-00000cd0: 6173 73da 0b67 6574 5f74 7261 696e 6572  ass..get_trainer
-00000ce0: 7229 0000 00da 076c 6f67 6769 6e67 da04  r).....logging..
-00000cf0: 696e 666f 7217 0000 00da 076e 6f5f 6772  infor......no_gr
-00000d00: 6164 721f 0000 0072 0d00 0000 da06 7661  adr....r......va
-00000d10: 6c75 6573 290e 7202 0000 0072 2200 0000  lues).r....r"...
-00000d20: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
-00000d30: 2600 0000 7227 0000 00da 0e64 6174 6173  &...r'.....datas
-00000d40: 6574 5f6f 626a 6563 7472 1300 0000 da15  et_objectr......
-00000d50: 7472 6169 6e65 725f 6f62 6a65 6374 5f6c  trainer_object_l
-00000d60: 6f61 6465 6472 1400 0000 7204 0000 0072  oadedr....r....r
-00000d70: 0500 0000 da05 7472 7574 6872 1000 0000  ......truthr....
-00000d80: 7210 0000 0072 1100 0000 da1d 6d61 6b65  r....r......make
-00000d90: 5f70 7265 6469 6374 696f 6e73 5f6c 6f61  _predictions_loa
-00000da0: 6465 645f 6d6f 6465 6c4d 0000 0073 3c00  ded_modelM...s<.
-00000db0: 0000 0c1e 0401 1001 0801 0401 0e01 0401  ................
-00000dc0: 0201 0801 0201 0201 0201 0201 06fa 0e08  ................
-00000dd0: 0401 0201 0401 0201 0201 0201 0201 06fa  ................
-00000de0: 0a08 0a01 1001 1cff 0a02 1201 0a01 7243  ..............rC
-00000df0: 0000 0029 0472 2000 0000 7221 0000 004e  ...).r ...r!...N
-00000e00: 5429 1b72 3c00 0000 da06 7479 7069 6e67  T).r<.....typing
-00000e10: da01 7472 3200 0000 da1b 6132 2e74 7261  ..tr2.....a2.tra
-00000e20: 696e 696e 672e 6461 7461 7365 745f 6875  ining.dataset_hu
-00000e30: 6767 696e 6772 2e00 0000 da1c 6132 2e74  ggingr......a2.t
-00000e40: 7261 696e 696e 672e 7472 6169 6e69 6e67  raining.training
-00000e50: 5f68 7567 6769 6e67 da1a 6132 2e74 7261  _hugging..a2.tra
-00000e60: 696e 696e 672e 7574 696c 735f 7472 6169  ining.utils_trai
-00000e70: 6e69 6e67 da08 6461 7461 7365 7473 721d  ning..datasetsr.
-00000e80: 0000 0072 3700 0000 7217 0000 00da 0c74  ...r7...r......t
-00000e90: 7261 6e73 666f 726d 6572 73da 0678 6172  ransformers..xar
-00000ea0: 7261 79da 0744 6174 6173 6574 7238 0000  ray..Datasetr8..
-00000eb0: 0072 1200 0000 da05 556e 696f 6eda 0b44  .r......Union..D
-00000ec0: 6174 6173 6574 4469 6374 da07 5472 6169  atasetDict..Trai
-00000ed0: 6e65 72da 0554 7570 6c65 721f 0000 00da  ner..Tupler.....
-00000ee0: 0373 7472 da08 4f70 7469 6f6e 616c da10  .str..Optional..
-00000ef0: 4465 6265 7274 6154 6f6b 656e 697a 6572  DebertaTokenizer
-00000f00: da04 626f 6f6c 7243 0000 0072 1000 0000  ..boolrC...r....
-00000f10: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000f20: 083c 6d6f 6475 6c65 3e01 0000 0073 6400  .<module>....sd.
-00000f30: 0000 0800 0801 0801 0802 0801 0801 0801  ................
-00000f40: 0801 0801 0801 0801 0203 0401 02ff 0802  ................
-00000f50: 02fe 0403 02fd 0404 02fc 0405 0afb 0226  ...............&
-00000f60: 1001 02ff 0402 02fe 1003 0afd 021c 0201  ................
-00000f70: 0201 0201 04f9 0401 02ff 0402 02fe 0203  ................
-00000f80: 02fd 0204 02fc 0205 02fb 0a06 02fa 0207  ................
-00000f90: 02f9 1408 0ef8                           ......
+00000000: 696d 706f 7274 206c 6f67 6769 6e67 0a69  import logging.i
+00000010: 6d70 6f72 7420 7479 7069 6e67 2061 7320  mport typing as 
+00000020: 740a 696d 706f 7274 2077 6172 6e69 6e67  t.import warning
+00000030: 730a 0a69 6d70 6f72 7420 6132 2e74 7261  s..import a2.tra
+00000040: 696e 696e 672e 6461 7461 7365 745f 6875  ining.dataset_hu
+00000050: 6767 696e 670a 696d 706f 7274 2061 322e  gging.import a2.
+00000060: 7472 6169 6e69 6e67 2e74 7261 696e 696e  training.trainin
+00000070: 675f 6875 6767 696e 670a 696d 706f 7274  g_hugging.import
+00000080: 2061 322e 7472 6169 6e69 6e67 2e75 7469   a2.training.uti
+00000090: 6c73 5f74 7261 696e 696e 670a 696d 706f  ls_training.impo
+000000a0: 7274 2064 6174 6173 6574 730a 696d 706f  rt datasets.impo
+000000b0: 7274 206e 756d 7079 2061 7320 6e70 0a69  rt numpy as np.i
+000000c0: 6d70 6f72 7420 746f 7263 680a 696d 706f  mport torch.impo
+000000d0: 7274 2074 7261 6e73 666f 726d 6572 730a  rt transformers.
+000000e0: 696d 706f 7274 2078 6172 7261 790a 0a0a  import xarray...
+000000f0: 6465 6620 6275 696c 645f 6473 5f74 6573  def build_ds_tes
+00000100: 7428 0a20 2020 2064 733a 2078 6172 7261  t(.    ds: xarra
+00000110: 792e 4461 7461 7365 742c 0a20 2020 2069  y.Dataset,.    i
+00000120: 6e64 6963 6573 5f74 6573 743a 206e 702e  ndices_test: np.
+00000130: 6e64 6172 7261 7920 7c20 4e6f 6e65 2c0a  ndarray | None,.
+00000140: 2020 2020 7072 6564 6963 7469 6f6e 733a      predictions:
+00000150: 206e 702e 6e64 6172 7261 792c 0a20 2020   np.ndarray,.   
+00000160: 2070 7265 6469 6374 696f 6e5f 7072 6f62   prediction_prob
+00000170: 6162 696c 6974 6965 733a 206e 702e 6e64  abilities: np.nd
+00000180: 6172 7261 792c 0a29 202d 3e20 7861 7272  array,.) -> xarr
+00000190: 6179 2e44 6174 6173 6574 3a0a 2020 2020  ay.Dataset:.    
+000001a0: 2222 220a 2020 2020 436f 6e73 7472 7563  """.    Construc
+000001b0: 7420 7465 7374 2064 6174 6173 6574 2077  t test dataset w
+000001c0: 6865 7265 2074 6573 7420 6461 7461 2069  here test data i
+000001d0: 7320 6465 6669 6e65 6420 6279 2074 6865  s defined by the
+000001e0: 6972 2069 6e64 6963 6573 0a20 2020 2061  ir indices.    a
+000001f0: 6e64 2063 6f72 7265 7370 6f6e 6469 6e67  nd corresponding
+00000200: 2070 7265 6469 6374 696f 6e73 2061 6e64   predictions and
+00000210: 2070 7265 6469 6374 696f 6e5f 7072 6f62   prediction_prob
+00000220: 6162 696c 6974 6965 730a 0a20 2020 2050  abilities..    P
+00000230: 6172 616d 6574 6572 733a 0a20 2020 202d  arameters:.    -
+00000240: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6473  ---------.    ds
+00000250: 3a20 7861 7272 6179 2064 6174 6173 6574  : xarray dataset
+00000260: 0a20 2020 2069 6e64 6963 6573 5f74 6573  .    indices_tes
+00000270: 743a 2056 6172 6961 626c 6520 2769 6e64  t: Variable 'ind
+00000280: 6578 2720 7661 6c75 6573 2074 6861 7420  ex' values that 
+00000290: 6172 6520 7573 6564 2066 6f72 2074 6573  are used for tes
+000002a0: 7469 6e67 0a20 2020 2070 7265 6469 6374  ting.    predict
+000002b0: 696f 6e73 3a20 5072 6564 6963 7465 6420  ions: Predicted 
+000002c0: 6c61 6265 6c73 0a20 2020 2070 7265 6469  labels.    predi
+000002d0: 6374 696f 6e5f 7072 6f62 6162 696c 6974  ction_probabilit
+000002e0: 6965 733a 2050 7265 6469 6374 696f 6e20  ies: Prediction 
+000002f0: 7072 6f62 6162 696c 6974 7920 666f 7220  probability for 
+00000300: 626f 7468 206c 6162 656c 732c 0a20 2020  both labels,.   
+00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000320: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00000330: 203d 205b 6e5f 7465 7374 732c 2032 5d0a   = [n_tests, 2].
+00000340: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00000350: 202d 2d2d 2d2d 2d2d 0a20 2020 2078 6172   -------.    xar
+00000360: 7261 792e 4461 7461 7365 740a 2020 2020  ray.Dataset.    
+00000370: 2222 220a 2020 2020 6966 2069 6e64 6963  """.    if indic
+00000380: 6573 5f74 6573 7420 6973 206e 6f74 204e  es_test is not N
+00000390: 6f6e 653a 0a20 2020 2020 2020 2064 735f  one:.        ds_
+000003a0: 7465 7374 203d 2064 732e 7365 6c28 696e  test = ds.sel(in
+000003b0: 6465 783d 696e 6469 6365 735f 7465 7374  dex=indices_test
+000003c0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+000003d0: 2020 2020 6473 5f74 6573 7420 3d20 6473      ds_test = ds
+000003e0: 2e63 6f70 7928 290a 2020 2020 6473 5f74  .copy().    ds_t
+000003f0: 6573 745b 2270 7265 6469 6374 696f 6e22  est["prediction"
+00000400: 5d20 3d20 285b 2269 6e64 6578 225d 2c20  ] = (["index"], 
+00000410: 7072 6564 6963 7469 6f6e 7329 0a20 2020  predictions).   
+00000420: 2064 735f 7465 7374 5b22 7072 6564 6963   ds_test["predic
+00000430: 7469 6f6e 5f70 726f 6261 6269 6c69 7479  tion_probability
+00000440: 5f6e 6f74 5f72 6169 6e69 6e67 225d 203d  _not_raining"] =
+00000450: 2028 0a20 2020 2020 2020 205b 2269 6e64   (.        ["ind
+00000460: 6578 225d 2c0a 2020 2020 2020 2020 7072  ex"],.        pr
+00000470: 6564 6963 7469 6f6e 5f70 726f 6261 6269  ediction_probabi
+00000480: 6c69 7469 6573 5b3a 2c20 305d 2c0a 2020  lities[:, 0],.  
+00000490: 2020 290a 2020 2020 6473 5f74 6573 745b    ).    ds_test[
+000004a0: 2270 7265 6469 6374 696f 6e5f 7072 6f62  "prediction_prob
+000004b0: 6162 696c 6974 795f 7261 696e 696e 6722  ability_raining"
+000004c0: 5d20 3d20 280a 2020 2020 2020 2020 5b22  ] = (.        ["
+000004d0: 696e 6465 7822 5d2c 0a20 2020 2020 2020  index"],.       
+000004e0: 2070 7265 6469 6374 696f 6e5f 7072 6f62   prediction_prob
+000004f0: 6162 696c 6974 6965 735b 3a2c 2031 5d2c  abilities[:, 1],
+00000500: 0a20 2020 2029 0a20 2020 2072 6574 7572  .    ).    retur
+00000510: 6e20 6473 5f74 6573 740a 0a0a 6465 6620  n ds_test...def 
+00000520: 7072 6564 6963 745f 6461 7461 7365 7428  predict_dataset(
+00000530: 0a20 2020 2064 6174 6173 6574 3a20 742e  .    dataset: t.
+00000540: 556e 696f 6e5b 6461 7461 7365 7473 2e44  Union[datasets.D
+00000550: 6174 6173 6574 2c20 6461 7461 7365 7473  ataset, datasets
+00000560: 2e44 6174 6173 6574 4469 6374 5d2c 0a20  .DatasetDict],. 
+00000570: 2020 2074 7261 696e 6572 3a20 7472 616e     trainer: tran
+00000580: 7366 6f72 6d65 7273 2e54 7261 696e 6572  sformers.Trainer
+00000590: 2c0a 2920 2d3e 2074 2e54 7570 6c65 5b6e  ,.) -> t.Tuple[n
+000005a0: 702e 6e64 6172 7261 792c 206e 702e 6e64  p.ndarray, np.nd
+000005b0: 6172 7261 795d 3a0a 2020 2020 2222 220a  array]:.    """.
+000005c0: 2020 2020 4d61 6b65 2070 7265 6469 6374      Make predict
+000005d0: 696f 6e73 206f 6e20 4875 6767 696e 6720  ions on Hugging 
+000005e0: 4661 6365 2064 6174 6173 6574 2062 6173  Face dataset bas
+000005f0: 6564 0a20 2020 206f 6e20 4875 6767 696e  ed.    on Huggin
+00000600: 6720 4661 6365 2074 7261 696e 6572 206f  g Face trainer o
+00000610: 626a 6563 740a 0a20 2020 2050 6172 616d  bject..    Param
+00000620: 6574 6572 733a 0a20 2020 202d 2d2d 2d2d  eters:.    -----
+00000630: 2d2d 2d2d 2d0a 2020 2020 6461 7461 7365  -----.    datase
+00000640: 743a 2048 7567 6769 6e67 2046 6163 6520  t: Hugging Face 
+00000650: 6461 7461 7365 740a 2020 2020 7472 6169  dataset.    trai
+00000660: 6e65 723a 2048 7567 6769 6e67 2046 6163  ner: Hugging Fac
+00000670: 6520 7472 6169 6e65 720a 0a20 2020 2052  e trainer..    R
+00000680: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00000690: 2d2d 0a20 2020 2078 6172 7261 792e 4461  --.    xarray.Da
+000006a0: 7461 7365 740a 2020 2020 2222 220a 2020  taset.    """.  
+000006b0: 2020 7072 6564 6963 7469 6f6e 5f70 726f    prediction_pro
+000006c0: 6261 6269 6c69 7469 6573 203d 2074 6f72  babilities = tor
+000006d0: 6368 2e6e 6e2e 6675 6e63 7469 6f6e 616c  ch.nn.functional
+000006e0: 2e73 6f66 746d 6178 280a 2020 2020 2020  .softmax(.      
+000006f0: 2020 746f 7263 682e 5465 6e73 6f72 2874    torch.Tensor(t
+00000700: 7261 696e 6572 2e70 7265 6469 6374 2864  rainer.predict(d
+00000710: 6174 6173 6574 292e 7072 6564 6963 7469  ataset).predicti
+00000720: 6f6e 7329 2c20 6469 6d3d 310a 2020 2020  ons), dim=1.    
+00000730: 292e 6e75 6d70 7928 290a 2020 2020 7072  ).numpy().    pr
+00000740: 6564 6963 7469 6f6e 7320 3d20 7072 6564  edictions = pred
+00000750: 6963 7469 6f6e 5f70 726f 6261 6269 6c69  iction_probabili
+00000760: 7469 6573 2e61 7267 6d61 7828 2d31 290a  ties.argmax(-1).
+00000770: 2020 2020 7265 7475 726e 2070 7265 6469      return predi
+00000780: 6374 696f 6e73 2c20 7072 6564 6963 7469  ctions, predicti
+00000790: 6f6e 5f70 726f 6261 6269 6c69 7469 6573  on_probabilities
+000007a0: 0a0a 0a64 6566 206d 616b 655f 7072 6564  ...def make_pred
+000007b0: 6963 7469 6f6e 735f 6c6f 6164 6564 5f6d  ictions_loaded_m
+000007c0: 6f64 656c 280a 2020 2020 6473 3a20 7861  odel(.    ds: xa
+000007d0: 7272 6179 2e44 6174 6173 6574 2c0a 2020  rray.Dataset,.  
+000007e0: 2020 696e 6469 6365 735f 7661 6c69 6461    indices_valida
+000007f0: 7465 3a20 6e70 2e6e 6461 7272 6179 2c0a  te: np.ndarray,.
+00000800: 2020 2020 666f 6c64 6572 5f6d 6f64 656c      folder_model
+00000810: 3a20 7374 722c 0a20 2020 206b 6579 5f69  : str,.    key_i
+00000820: 6e70 7574 733a 2073 7472 203d 2022 7465  nputs: str = "te
+00000830: 7874 222c 0a20 2020 206b 6579 5f6c 6162  xt",.    key_lab
+00000840: 656c 3a20 7374 7220 3d20 2272 6169 6e69  el: str = "raini
+00000850: 6e67 222c 0a20 2020 2066 6f6c 6465 725f  ng",.    folder_
+00000860: 746f 6b65 6e69 7a65 723a 2074 2e4f 7074  tokenizer: t.Opt
+00000870: 696f 6e61 6c5b 7472 616e 7366 6f72 6d65  ional[transforme
+00000880: 7273 2e44 6562 6572 7461 546f 6b65 6e69  rs.DebertaTokeni
+00000890: 7a65 725d 203d 204e 6f6e 652c 0a20 2020  zer] = None,.   
+000008a0: 2066 7031 363a 2062 6f6f 6c20 3d20 5472   fp16: bool = Tr
+000008b0: 7565 2c0a 2920 2d3e 2074 2e54 7570 6c65  ue,.) -> t.Tuple
+000008c0: 5b6e 702e 6e64 6172 7261 792c 206e 702e  [np.ndarray, np.
+000008d0: 6e64 6172 7261 792c 206e 702e 6e64 6172  ndarray, np.ndar
+000008e0: 7261 795d 3a0a 2020 2020 2222 220a 2020  ray]:.    """.  
+000008f0: 2020 4d61 6b65 2070 7265 6469 6374 696f    Make predictio
+00000900: 6e73 206f 6e20 6c6f 6164 6564 2074 7261  ns on loaded tra
+00000910: 696e 6564 2048 7567 6769 6e67 2046 6163  ined Hugging Fac
+00000920: 6520 6d6f 6465 6c0a 0a20 2020 2057 4152  e model..    WAR
+00000930: 4e49 4e47 3a20 5472 7920 7573 696e 6720  NING: Try using 
+00000940: 6f72 6967 696e 616c 2066 6f6c 6465 7220  original folder 
+00000950: 666f 7220 6066 6f6c 6465 725f 746f 6b65  for `folder_toke
+00000960: 6e69 7a65 7260 0a20 2020 2020 2020 2020  nizer`.         
+00000970: 2020 2020 6966 2072 756e 2069 6e74 6f20      if run into 
+00000980: 6973 7375 6573 2077 6865 6e20 696e 6974  issues when init
+00000990: 6961 6c69 7a69 6e67 2074 6f6b 656e 697a  ializing tokeniz
+000009a0: 6572 210a 2020 2020 5061 7261 6d65 7465  er!.    Paramete
+000009b0: 7273 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  rs:.    --------
+000009c0: 2d2d 0a20 2020 2064 733a 2058 6172 7261  --.    ds: Xarra
+000009d0: 7920 6461 7461 7365 740a 2020 2020 696e  y dataset.    in
+000009e0: 6469 6365 735f 7661 6c69 6461 7465 3a20  dices_validate: 
+000009f0: 5661 7269 6162 6c65 2027 696e 6465 7827  Variable 'index'
+00000a00: 2076 616c 7565 7320 7468 6174 2061 7265   values that are
+00000a10: 2075 7365 6420 666f 7220 7661 6c69 6461   used for valida
+00000a20: 7469 6f6e 0a20 2020 2066 6f6c 6465 725f  tion.    folder_
+00000a30: 6d6f 6465 6c3a 2046 6f6c 6465 7220 6f66  model: Folder of
+00000a40: 2070 7265 7472 6169 6e65 6420 6d6f 6465   pretrained mode
+00000a50: 6c0a 2020 2020 6b65 795f 696e 7075 7473  l.    key_inputs
+00000a60: 3a20 4b65 7920 6f66 2076 6172 6961 626c  : Key of variabl
+00000a70: 6520 7573 6564 2061 7320 696e 7075 7420  e used as input 
+00000a80: 746f 206d 6f64 656c 0a20 2020 206b 6579  to model.    key
+00000a90: 5f6c 6162 656c 3a20 4b65 7920 6f66 2076  _label: Key of v
+00000aa0: 6172 6961 626c 6520 7573 6564 2061 7320  ariable used as 
+00000ab0: 6c61 6265 6c20 666f 7220 7472 6169 6e69  label for traini
+00000ac0: 6e67 0a20 2020 2066 6f6c 6465 725f 746f  ng.    folder_to
+00000ad0: 6b65 6e69 7a65 723a 2046 6f6c 6465 7220  kenizer: Folder 
+00000ae0: 6f66 206f 7269 6769 6e61 6c20 6d6f 6465  of original mode
+00000af0: 6c20 646f 776e 6c6f 6164 6564 2066 726f  l downloaded fro
+00000b00: 6d20 4875 7567 696e 6720 4661 6365 0a20  m Huuging Face. 
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 2020 2020 2028 6d61 7920 7275 6e20 696e       (may run in
+00000b30: 746f 2069 7373 7565 7320 6966 2075 7365  to issues if use
+00000b40: 2066 6f6c 6465 725f 746f 6b65 6e69 7a65   folder_tokenize
+00000b50: 723d 666f 6c64 6572 5f6d 6f64 656c 290a  r=folder_model).
+00000b60: 2020 2020 6670 3136 3a20 5768 6574 6865      fp16: Whethe
+00000b70: 7220 746f 2075 7365 2066 7031 3620 3136  r to use fp16 16
+00000b80: 2d62 6974 2028 6d69 7865 6429 2070 7265  -bit (mixed) pre
+00000b90: 6369 7369 6f6e 2074 7261 696e 696e 670a  cision training.
+00000ba0: 2020 2020 2020 2020 2020 696e 7374 6561            instea
+00000bb0: 6420 6f66 2033 322d 6269 7420 7472 6169  d of 32-bit trai
+00000bc0: 6e69 6e67 2e0a 0a20 2020 2052 6574 7572  ning...    Retur
+00000bd0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00000be0: 2020 2074 7275 7468 2c20 7072 6564 6963     truth, predic
+00000bf0: 7469 6f6e 732c 2070 7265 6469 6374 696f  tions, predictio
+00000c00: 6e5f 7072 6f62 6162 696c 6974 6965 730a  n_probabilities.
+00000c10: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
+00000c20: 6f74 2061 322e 7472 6169 6e69 6e67 2e75  ot a2.training.u
+00000c30: 7469 6c73 5f74 7261 696e 696e 672e 6770  tils_training.gp
+00000c40: 755f 6176 6169 6c61 626c 6528 293a 0a20  u_available():. 
+00000c50: 2020 2020 2020 2066 7031 3620 3d20 4661         fp16 = Fa
+00000c60: 6c73 650a 2020 2020 2020 2020 7761 726e  lse.        warn
+00000c70: 696e 6773 2e77 6172 6e28 6622 3136 2d62  ings.warn(f"16-b
+00000c80: 6974 2065 7661 6c75 6174 696f 6e20 6f6e  it evaluation on
+00000c90: 6c79 2061 7661 696c 6162 6c65 206f 6e20  ly available on 
+00000ca0: 7379 7374 656d 7320 7769 7468 2047 5055  systems with GPU
+00000cb0: 2e20 5365 7474 696e 6720 7b66 7031 363d  . Setting {fp16=
+00000cc0: 7d22 290a 2020 2020 6966 2066 6f6c 6465  }").    if folde
+00000cd0: 725f 746f 6b65 6e69 7a65 7220 6973 204e  r_tokenizer is N
+00000ce0: 6f6e 653a 0a20 2020 2020 2020 2066 6f6c  one:.        fol
+00000cf0: 6465 725f 746f 6b65 6e69 7a65 7220 3d20  der_tokenizer = 
+00000d00: 666f 6c64 6572 5f6d 6f64 656c 0a20 2020  folder_model.   
+00000d10: 2064 6174 6173 6574 5f6f 626a 6563 7420   dataset_object 
+00000d20: 3d20 6132 2e74 7261 696e 696e 672e 6461  = a2.training.da
+00000d30: 7461 7365 745f 6875 6767 696e 672e 4461  taset_hugging.Da
+00000d40: 7461 7365 7448 7567 6769 6e67 4661 6365  tasetHuggingFace
+00000d50: 2866 6f6c 6465 725f 746f 6b65 6e69 7a65  (folder_tokenize
+00000d60: 7229 0a20 2020 2064 6174 6173 6574 203d  r).    dataset =
+00000d70: 2064 6174 6173 6574 5f6f 626a 6563 742e   dataset_object.
+00000d80: 6275 696c 6428 0a20 2020 2020 2020 2064  build(.        d
+00000d90: 732c 0a20 2020 2020 2020 206e 702e 6e64  s,.        np.nd
+00000da0: 6172 7261 7928 5b5d 292c 0a20 2020 2020  array([]),.     
+00000db0: 2020 2069 6e64 6963 6573 5f76 616c 6964     indices_valid
+00000dc0: 6174 652c 0a20 2020 2020 2020 2074 7261  ate,.        tra
+00000dd0: 696e 3d46 616c 7365 2c0a 2020 2020 2020  in=False,.      
+00000de0: 2020 6b65 795f 696e 7075 7473 3d6b 6579    key_inputs=key
+00000df0: 5f69 6e70 7574 732c 0a20 2020 2020 2020  _inputs,.       
+00000e00: 206b 6579 5f6c 6162 656c 3d6b 6579 5f6c   key_label=key_l
+00000e10: 6162 656c 2c0a 2020 2020 290a 2020 2020  abel,.    ).    
+00000e20: 7472 6169 6e65 725f 6f62 6a65 6374 5f6c  trainer_object_l
+00000e30: 6f61 6465 6420 3d20 6132 2e74 7261 696e  oaded = a2.train
+00000e40: 696e 672e 7472 6169 6e69 6e67 5f68 7567  ing.training_hug
+00000e50: 6769 6e67 2e48 7567 6769 6e67 4661 6365  ging.HuggingFace
+00000e60: 5472 6169 6e65 7243 6c61 7373 2866 6f6c  TrainerClass(fol
+00000e70: 6465 725f 6d6f 6465 6c29 0a20 2020 2074  der_model).    t
+00000e80: 7261 696e 6572 203d 2074 7261 696e 6572  rainer = trainer
+00000e90: 5f6f 626a 6563 745f 6c6f 6164 6564 2e67  _object_loaded.g
+00000ea0: 6574 5f74 7261 696e 6572 280a 2020 2020  et_trainer(.    
+00000eb0: 2020 2020 6461 7461 7365 742c 0a20 2020      dataset,.   
+00000ec0: 2020 2020 2074 6f6b 656e 697a 6572 3d64       tokenizer=d
+00000ed0: 6174 6173 6574 5f6f 626a 6563 742e 746f  ataset_object.to
+00000ee0: 6b65 6e69 7a65 722c 0a20 2020 2020 2020  kenizer,.       
+00000ef0: 2066 6f6c 6465 725f 6f75 7470 7574 3d22   folder_output="
+00000f00: 2e2f 222c 0a20 2020 2020 2020 2068 7970  ./",.        hyp
+00000f10: 6572 5f74 756e 696e 673d 4661 6c73 652c  er_tuning=False,
+00000f20: 0a20 2020 2020 2020 2066 7031 363d 6670  .        fp16=fp
+00000f30: 3136 2c0a 2020 2020 2020 2020 6576 616c  16,.        eval
+00000f40: 7561 7465 3d54 7275 652c 0a20 2020 2029  uate=True,.    )
+00000f50: 0a20 2020 206c 6f67 6769 6e67 2e69 6e66  .    logging.inf
+00000f60: 6f28 2270 7265 6469 6374 696e 6722 290a  o("predicting").
+00000f70: 2020 2020 7769 7468 2074 6f72 6368 2e6e      with torch.n
+00000f80: 6f5f 6772 6164 2829 3a0a 2020 2020 2020  o_grad():.      
+00000f90: 2020 7072 6564 6963 7469 6f6e 732c 2070    predictions, p
+00000fa0: 7265 6469 6374 696f 6e5f 7072 6f62 6162  rediction_probab
+00000fb0: 696c 6974 6965 7320 3d20 7072 6564 6963  ilities = predic
+00000fc0: 745f 6461 7461 7365 7428 6461 7461 7365  t_dataset(datase
+00000fd0: 742c 2074 7261 696e 6572 290a 2020 2020  t, trainer).    
+00000fe0: 6c6f 6767 696e 672e 696e 666f 2822 646f  logging.info("do
+00000ff0: 6e65 2070 7265 6469 6374 696e 6722 290a  ne predicting").
+00001000: 2020 2020 7472 7574 6820 3d20 6473 2e73      truth = ds.s
+00001010: 656c 2869 6e64 6578 3d69 6e64 6963 6573  el(index=indices
+00001020: 5f76 616c 6964 6174 6529 5b6b 6579 5f6c  _validate)[key_l
+00001030: 6162 656c 5d2e 7661 6c75 6573 0a20 2020  abel].values.   
+00001040: 2072 6574 7572 6e20 7472 7574 682c 2070   return truth, p
+00001050: 7265 6469 6374 696f 6e73 2c20 7072 6564  redictions, pred
+00001060: 6963 7469 6f6e 5f70 726f 6261 6269 6c69  iction_probabili
+00001070: 7469 6573 0a                             ties.
```

### Comparing `a2-0.3.5/src/a2/training/benchmarks.py` & `a2-0.3.6/src/a2/training/benchmarks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/training/tracking.py` & `a2-0.3.6/src/a2/training/tracking.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/training/tracking_hugging.py` & `a2-0.3.6/src/a2/training/tracking_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/training/training_deep500.py` & `a2-0.3.6/src/a2/training/training_deep500.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/training/training_hugging.py` & `a2-0.3.6/src/a2/training/training_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/training/training_performance.py` & `a2-0.3.6/src/a2/training/training_performance.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/twitter/downloader.py` & `a2-0.3.6/src/a2/twitter/downloader.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/twitter/locations.py` & `a2-0.3.6/src/a2/twitter/locations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/twitter/twitter_api.py` & `a2-0.3.6/src/a2/twitter/twitter_api.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/utils/argparse.py` & `a2-0.3.6/src/a2/utils/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,21 @@
     parser.add_argument(
         "--data_filename_irrelevant",
         type=str,
         default="2017_2020_tweets_rain_sun_vocab_emojis_locations_bba_Tp_era5_no_bots_normalized_filtered.nc",
         help="Filename of training data.",
     )
     parser.add_argument(
+        "--n_tweets_irrelevant",
+        type=tuple[int, str],
+        default="all",
+        help='Number of irrelevant tweets used to create dataset, use all irrelevant tweets by default ("all").',
+    )
+
+    parser.add_argument(
         "--key_relevance",
         type=str,
         default="relevant",
         help="Filename of training data.",
     )
```

### Comparing `a2-0.3.5/src/a2/utils/checks.py` & `a2-0.3.6/src/a2/utils/checks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/utils/file_handling.py` & `a2-0.3.6/src/a2/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/utils/testing.py` & `a2-0.3.6/src/a2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/src/a2/utils/utils.py` & `a2-0.3.6/src/a2/utils/utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.5/PKG-INFO` & `a2-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2
-Version: 0.3.5
+Version: 0.3.6
 Summary: Package for predicting information about the weather from social media data as application 2 for maelstrom project
 Author: Kristian Ehlert
 Author-email: kristian.ehlert@4-cast.de
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

