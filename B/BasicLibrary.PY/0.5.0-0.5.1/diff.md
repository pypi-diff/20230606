# Comparing `tmp/BasicLibrary.PY-0.5.0.tar.gz` & `tmp/BasicLibrary.PY-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BasicLibrary.PY-0.5.0.tar", last modified: Tue Jun  6 09:49:18 2023, max compression
+gzip compressed data, was "BasicLibrary.PY-0.5.1.tar", last modified: Tue Jun  6 10:10:25 2023, max compression
```

## Comparing `BasicLibrary.PY-0.5.0.tar` & `BasicLibrary.PY-0.5.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.230203 BasicLibrary.PY-0.5.0/
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:17.791201 BasicLibrary.PY-0.5.0/BasicLibrary/
--rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/__init__.py
--rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.0/BasicLibrary/__projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:17.843203 BasicLibrary.PY-0.5.0/BasicLibrary/biz/
--rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.0/BasicLibrary/biz/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.0/BasicLibrary/biz/stockHelper.py
--rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.0/BasicLibrary/biz/tencentHelper.py
--rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.0/BasicLibrary/configHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:17.956203 BasicLibrary.PY-0.5.0/BasicLibrary/data/
--rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/__init__.py
--rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/collectionHelper.py
--rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/dateTimeHelper.py
--rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/dictHelper.py
--rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/htmlHelper.py
--rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/listHelper.py
--rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/numberHelper.py
--rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/objectHelper.py
--rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/pandasHelper.py
--rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/randomHelper.py
--rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/reflectHelper.py
--rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/regexHelper.py
--rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/setHelper.py
--rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/data/stringHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.002203 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.029205 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/ddl.py
--rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/helper.py
--rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/mate.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.058205 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/ddl.py
--rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/mate.py
--rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/pool.py
--rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/__init__.py
--rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseClient.py
--rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseDDL.py
--rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseEnum.py
--rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseHelper.py
--rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseMate.py
--rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseUnitTest.py
--rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.0/BasicLibrary/enums.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.075205 BasicLibrary.PY-0.5.0/BasicLibrary/environment/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.0/BasicLibrary/environment/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.0/BasicLibrary/environment/consoleHelper.py
--rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/environment/envHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.106204 BasicLibrary.PY-0.5.0/BasicLibrary/io/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.0/BasicLibrary/io/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/io/dirHelper.py
--rw-rw-rw-   0        0        0     5194 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/io/fileHelper.py
--rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.0/BasicLibrary/io/ioHelper.py
--rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.0/BasicLibrary/io/pathHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.139202 BasicLibrary.PY-0.5.0/BasicLibrary/model/
--rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.0/BasicLibrary/model/__init__.py
--rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/model/container.py
--rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.0/BasicLibrary/model/dataCompare.py
--rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.0/BasicLibrary/model/kvPair.py
--rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.0/BasicLibrary/model/stopWatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.176202 BasicLibrary.PY-0.5.0/BasicLibrary/office/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.0/BasicLibrary/office/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.0/BasicLibrary/office/excelBookMate.py
--rw-rw-rw-   0        0        0     2418 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.0/BasicLibrary/office/excelHelper.py
--rw-rw-rw-   0        0        0     3047 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.0/BasicLibrary/office/excelMisc.py
--rw-rw-rw-   0        0        0    10519 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.0/BasicLibrary/office/excelSheetMate.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.190207 BasicLibrary.PY-0.5.0/BasicLibrary/pattern/
--rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.0/BasicLibrary/pattern/__init__.py
--rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.0/BasicLibrary/pattern/singleton.py
--rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.0/BasicLibrary/projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.202202 BasicLibrary.PY-0.5.0/BasicLibrary/syntax/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.0/BasicLibrary/syntax/__init__.py
--rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.0/BasicLibrary/syntax/switch.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:18.221207 BasicLibrary.PY-0.5.0/BasicLibrary/web/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.0/BasicLibrary/web/__init__.py
--rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.0/BasicLibrary/web/beautifulSoupHelper.py
--rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.0/BasicLibrary/web/requestHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:49:17.820205 BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/
--rw-rw-rw-   0        0        0     2466 2023-06-06 09:49:16.000000 BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-06-06 09:49:17.000000 BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:49:16.000000 BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 09:49:17.000000 BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2466 2023-06-06 09:49:18.228200 BasicLibrary.PY-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1781 2022-04-20 11:32:46.000000 BasicLibrary.PY-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 09:49:18.231202 BasicLibrary.PY-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     4281 2023-06-06 09:43:32.000000 BasicLibrary.PY-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.830735 BasicLibrary.PY-0.5.1/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:24.937441 BasicLibrary.PY-0.5.1/BasicLibrary/
+-rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/__init__.py
+-rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.1/BasicLibrary/__projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.009437 BasicLibrary.PY-0.5.1/BasicLibrary/biz/
+-rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.1/BasicLibrary/biz/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/biz/stockHelper.py
+-rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.1/BasicLibrary/biz/tencentHelper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/configHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.243019 BasicLibrary.PY-0.5.1/BasicLibrary/data/
+-rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/__init__.py
+-rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/collectionHelper.py
+-rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/dateTimeHelper.py
+-rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/dictHelper.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/htmlHelper.py
+-rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/listHelper.py
+-rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/numberHelper.py
+-rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/objectHelper.py
+-rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/pandasHelper.py
+-rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/randomHelper.py
+-rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/reflectHelper.py
+-rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/regexHelper.py
+-rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/setHelper.py
+-rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/data/stringHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.338546 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.398497 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/ddl.py
+-rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/helper.py
+-rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/mate.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.455553 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/ddl.py
+-rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/mate.py
+-rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/pool.py
+-rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/__init__.py
+-rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseClient.py
+-rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseDDL.py
+-rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseEnum.py
+-rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseHelper.py
+-rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseMate.py
+-rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseUnitTest.py
+-rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.1/BasicLibrary/enums.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.488736 BasicLibrary.PY-0.5.1/BasicLibrary/environment/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.1/BasicLibrary/environment/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/environment/consoleHelper.py
+-rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/environment/envHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.566734 BasicLibrary.PY-0.5.1/BasicLibrary/io/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/dirHelper.py
+-rw-rw-rw-   0        0        0     5194 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/fileHelper.py
+-rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/ioHelper.py
+-rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/io/pathHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.655736 BasicLibrary.PY-0.5.1/BasicLibrary/model/
+-rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/__init__.py
+-rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/container.py
+-rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/dataCompare.py
+-rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/kvPair.py
+-rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.1/BasicLibrary/model/stopWatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.750734 BasicLibrary.PY-0.5.1/BasicLibrary/office/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelBookMate.py
+-rw-rw-rw-   0        0        0     2418 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelHelper.py
+-rw-rw-rw-   0        0        0     3047 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelMisc.py
+-rw-rw-rw-   0        0        0    10519 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.1/BasicLibrary/office/excelSheetMate.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.774737 BasicLibrary.PY-0.5.1/BasicLibrary/pattern/
+-rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.1/BasicLibrary/pattern/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.1/BasicLibrary/pattern/singleton.py
+-rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.1/BasicLibrary/projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.785744 BasicLibrary.PY-0.5.1/BasicLibrary/syntax/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.1/BasicLibrary/syntax/__init__.py
+-rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.1/BasicLibrary/syntax/switch.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:25.818741 BasicLibrary.PY-0.5.1/BasicLibrary/web/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.1/BasicLibrary/web/__init__.py
+-rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.1/BasicLibrary/web/beautifulSoupHelper.py
+-rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.1/BasicLibrary/web/requestHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:10:24.960435 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/
+-rw-rw-rw-   0        0        0     2896 2023-06-06 10:10:23.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-06-06 10:10:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:10:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 10:10:24.000000 BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2896 2023-06-06 10:10:25.827737 BasicLibrary.PY-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:10:25.831739 BasicLibrary.PY-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     4281 2023-06-06 10:10:09.000000 BasicLibrary.PY-0.5.1/setup.py
```

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/__init__.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/__projectHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/__projectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/biz/stockHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/biz/stockHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/configHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/configHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/collectionHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/collectionHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/dateTimeHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/dateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/dictHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/dictHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/listHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/listHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/numberHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/numberHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/objectHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/objectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/pandasHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/pandasHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/randomHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/randomHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/reflectHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/reflectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/regexHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/regexHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/data/stringHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/data/stringHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/ddl.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/helper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/helper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MongoDB/mate.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MongoDB/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/ddl.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/mate.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/MySql/pool.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/MySql/pool.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseClient.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseClient.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseDDL.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseDDL.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseMate.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/dataBase/databaseUnitTest.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/dataBase/databaseUnitTest.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/environment/consoleHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/environment/consoleHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/environment/envHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/environment/envHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/io/dirHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/io/dirHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/io/fileHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/io/fileHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/io/ioHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/io/ioHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/io/pathHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/io/pathHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/model/container.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/model/container.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/model/dataCompare.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/model/dataCompare.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/model/kvPair.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/model/kvPair.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/office/excelBookMate.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelBookMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/office/excelHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/office/excelMisc.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelMisc.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/office/excelSheetMate.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/office/excelSheetMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/syntax/switch.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/syntax/switch.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/web/beautifulSoupHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/web/beautifulSoupHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary/web/requestHelper.py` & `BasicLibrary.PY-0.5.1/BasicLibrary/web/requestHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/PKG-INFO` & `BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.0
+Version: 0.5.1
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 
 整理常用的代码块，形成企业级的类库工具，供更多项目使用。
 
 ## 【零】目录格式
 
 1. 最外层是整个项目的根目录(本项目中为 BasicLibrary.PY)，这个目录作为 git 的根目录。
 2. 根目录下分布"部署文件""说明文件"等周边辅助文件(比如 setup.py、README.md等)
-3. 根目录下用 Python 包的形式架构项目的业务逻辑代码(本项目下为 hilandBasicLibrary)
+3. 根目录下用 Python 包的形式架构项目的业务逻辑代码(本项目下为 BasicLibrary)
    (一般每个项目只架构一个根 Python 包,然后再决定是在根包下再架构子包，还是在根包下直接写 ***.py 代码)
 
 ## 【一】发布步骤：
 
 0. 打开本项目的"终端"窗口(或者通过 windows 的资源管理器定位到本项目 setup.py 所在的目录)
 1. 打开修改 setup.py 文件 `VERSION = '0.4.3'`为新的值
 2. 运行命令 `python setup.py sdist`
@@ -46,14 +46,27 @@
 将本项目需求的第三方软件包统一组织在 requirements.txt 文件内。
 
 1. 组织第三方软件包进入文件的命令是：`pip freeze > requirements.txt`
 2. 重新安装所需的各第三方包的命令为：`pip install -r requirements.txt`
 
 ## 【三】部署
 
-1. 以下两个文件复制到项目根目录下
-    1. `__projectConfig.ini` 改名为 `_projectConfig.ini`
-    2. `__projectHelper.py` 改名为 `_projectHelper.py`
 
-2. 如果有敏感信息(比如账号口令等)不适合写在 ini 文件内的，可以将 `.env.default` 文件拷贝到文件 `_projectConfig.ini` 所在的项目根目录,然后改名为 `.env`,然后在 .env 文件内配置这些信息. (
-   ini 文件是嵌入到 vcs 系统的，但 .env 是不嵌入 vcs 系统的)
+### 1. 库安装（更新）说明
+更新公司类库 BasicLibrary.PY 的命令：
+
+```
+pip install BasicLibrary.PY -U
+# (因为本地的pip通常都为了加速，进行过换源处理了，换源之后缓存更新会比较慢。
+# 所以为了使用最新的库功能，可以使用原始的PIPY源，代码如下：)
+pip install BasicLibrary.PY -U -i https://pypi.org/simple
+```
+### 2. 库使用说明
+
+   1. 以下两个文件复制到项目根目录下
+       1. `__projectConfig.ini` 改名为 `_projectConfig.ini`
+       2. `__projectHelper.py` 改名为 `_projectHelper.py`
+
+   2. 如果有敏感信息(比如账号口令等)不适合写在 ini 文件内的，可以将 `.env.default` 文件拷贝到文件 `_projectConfig.ini` 所在的项目根目录,然后改名为 `.env`,然后在 .env 文件内配置这些信息. (
+      ini 文件是嵌入到 vcs 系统的，但 .env 是不嵌入 vcs 系统的)
+
```

### Comparing `BasicLibrary.PY-0.5.0/BasicLibrary.PY.egg-info/SOURCES.txt` & `BasicLibrary.PY-0.5.1/BasicLibrary.PY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.0/PKG-INFO` & `BasicLibrary.PY-0.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.0
+Version: 0.5.1
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 
 整理常用的代码块，形成企业级的类库工具，供更多项目使用。
 
 ## 【零】目录格式
 
 1. 最外层是整个项目的根目录(本项目中为 BasicLibrary.PY)，这个目录作为 git 的根目录。
 2. 根目录下分布"部署文件""说明文件"等周边辅助文件(比如 setup.py、README.md等)
-3. 根目录下用 Python 包的形式架构项目的业务逻辑代码(本项目下为 hilandBasicLibrary)
+3. 根目录下用 Python 包的形式架构项目的业务逻辑代码(本项目下为 BasicLibrary)
    (一般每个项目只架构一个根 Python 包,然后再决定是在根包下再架构子包，还是在根包下直接写 ***.py 代码)
 
 ## 【一】发布步骤：
 
 0. 打开本项目的"终端"窗口(或者通过 windows 的资源管理器定位到本项目 setup.py 所在的目录)
 1. 打开修改 setup.py 文件 `VERSION = '0.4.3'`为新的值
 2. 运行命令 `python setup.py sdist`
@@ -46,14 +46,27 @@
 将本项目需求的第三方软件包统一组织在 requirements.txt 文件内。
 
 1. 组织第三方软件包进入文件的命令是：`pip freeze > requirements.txt`
 2. 重新安装所需的各第三方包的命令为：`pip install -r requirements.txt`
 
 ## 【三】部署
 
-1. 以下两个文件复制到项目根目录下
-    1. `__projectConfig.ini` 改名为 `_projectConfig.ini`
-    2. `__projectHelper.py` 改名为 `_projectHelper.py`
 
-2. 如果有敏感信息(比如账号口令等)不适合写在 ini 文件内的，可以将 `.env.default` 文件拷贝到文件 `_projectConfig.ini` 所在的项目根目录,然后改名为 `.env`,然后在 .env 文件内配置这些信息. (
-   ini 文件是嵌入到 vcs 系统的，但 .env 是不嵌入 vcs 系统的)
+### 1. 库安装（更新）说明
+更新公司类库 BasicLibrary.PY 的命令：
+
+```
+pip install BasicLibrary.PY -U
+# (因为本地的pip通常都为了加速，进行过换源处理了，换源之后缓存更新会比较慢。
+# 所以为了使用最新的库功能，可以使用原始的PIPY源，代码如下：)
+pip install BasicLibrary.PY -U -i https://pypi.org/simple
+```
+### 2. 库使用说明
+
+   1. 以下两个文件复制到项目根目录下
+       1. `__projectConfig.ini` 改名为 `_projectConfig.ini`
+       2. `__projectHelper.py` 改名为 `_projectHelper.py`
+
+   2. 如果有敏感信息(比如账号口令等)不适合写在 ini 文件内的，可以将 `.env.default` 文件拷贝到文件 `_projectConfig.ini` 所在的项目根目录,然后改名为 `.env`,然后在 .env 文件内配置这些信息. (
+      ini 文件是嵌入到 vcs 系统的，但 .env 是不嵌入 vcs 系统的)
+
```

### Comparing `BasicLibrary.PY-0.5.0/README.md` & `BasicLibrary.PY-0.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 整理常用的代码块，形成企业级的类库工具，供更多项目使用。
 
 ## 【零】目录格式
 
 1. 最外层是整个项目的根目录(本项目中为 BasicLibrary.PY)，这个目录作为 git 的根目录。
 2. 根目录下分布"部署文件""说明文件"等周边辅助文件(比如 setup.py、README.md等)
-3. 根目录下用 Python 包的形式架构项目的业务逻辑代码(本项目下为 hilandBasicLibrary)
+3. 根目录下用 Python 包的形式架构项目的业务逻辑代码(本项目下为 BasicLibrary)
    (一般每个项目只架构一个根 Python 包,然后再决定是在根包下再架构子包，还是在根包下直接写 ***.py 代码)
 
 ## 【一】发布步骤：
 
 0. 打开本项目的"终端"窗口(或者通过 windows 的资源管理器定位到本项目 setup.py 所在的目录)
 1. 打开修改 setup.py 文件 `VERSION = '0.4.3'`为新的值
 2. 运行命令 `python setup.py sdist`
@@ -27,13 +27,25 @@
 将本项目需求的第三方软件包统一组织在 requirements.txt 文件内。
 
 1. 组织第三方软件包进入文件的命令是：`pip freeze > requirements.txt`
 2. 重新安装所需的各第三方包的命令为：`pip install -r requirements.txt`
 
 ## 【三】部署
 
-1. 以下两个文件复制到项目根目录下
-    1. `__projectConfig.ini` 改名为 `_projectConfig.ini`
-    2. `__projectHelper.py` 改名为 `_projectHelper.py`
 
-2. 如果有敏感信息(比如账号口令等)不适合写在 ini 文件内的，可以将 `.env.default` 文件拷贝到文件 `_projectConfig.ini` 所在的项目根目录,然后改名为 `.env`,然后在 .env 文件内配置这些信息. (
-   ini 文件是嵌入到 vcs 系统的，但 .env 是不嵌入 vcs 系统的)
+### 1. 库安装（更新）说明
+更新公司类库 BasicLibrary.PY 的命令：
+
+```
+pip install BasicLibrary.PY -U
+# (因为本地的pip通常都为了加速，进行过换源处理了，换源之后缓存更新会比较慢。
+# 所以为了使用最新的库功能，可以使用原始的PIPY源，代码如下：)
+pip install BasicLibrary.PY -U -i https://pypi.org/simple
+```
+### 2. 库使用说明
+
+   1. 以下两个文件复制到项目根目录下
+       1. `__projectConfig.ini` 改名为 `_projectConfig.ini`
+       2. `__projectHelper.py` 改名为 `_projectHelper.py`
+
+   2. 如果有敏感信息(比如账号口令等)不适合写在 ini 文件内的，可以将 `.env.default` 文件拷贝到文件 `_projectConfig.ini` 所在的项目根目录,然后改名为 `.env`,然后在 .env 文件内配置这些信息. (
+      ini 文件是嵌入到 vcs 系统的，但 .env 是不嵌入 vcs 系统的)
```

### Comparing `BasicLibrary.PY-0.5.0/setup.py` & `BasicLibrary.PY-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 NAME = 'BasicLibrary.PY'
 DESCRIPTION = '企业级的 PYTHON 库'
 URL = 'https://github.com/notinmood/BasicLibrary.PY'
 EMAIL = '9727005@qq.com'
 AUTHOR = 'xiedali'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.00'
+VERSION = '0.5.01'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

