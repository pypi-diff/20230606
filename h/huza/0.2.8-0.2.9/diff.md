# Comparing `tmp/huza-0.2.8.tar.gz` & `tmp/huza-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huza-0.2.8.tar", last modified: Thu Apr  6 07:14:33 2023, max compression
+gzip compressed data, was "huza-0.2.9.tar", last modified: Wed May 10 02:15:56 2023, max compression
```

## Comparing `huza-0.2.8.tar` & `huza-0.2.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.687781 huza-0.2.8/
--rw-r--r--   0 root         (0) root         (0)     1062 2022-11-21 06:24:02.000000 huza-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-06 07:14:33.687781 huza-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2022-11-21 06:24:02.000000 huza-0.2.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.678781 huza-0.2.8/huza/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.680781 huza-0.2.8/huza/base/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      751 2022-01-04 03:29:52.000000 huza-0.2.8/huza/base/action.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-05 12:11:37.000000 huza-0.2.8/huza/base/dockview.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-11-21 06:24:02.000000 huza-0.2.8/huza/base/mainwindow.py
--rw-r--r--   0 root         (0) root         (0)     6674 2023-04-04 07:57:27.000000 huza-0.2.8/huza/base/mainwindow_run.py
--rw-r--r--   0 root         (0) root         (0)      653 2022-05-17 09:25:15.000000 huza-0.2.8/huza/base/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.680781 huza-0.2.8/huza/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      701 2022-01-04 03:29:52.000000 huza-0.2.8/huza/cli/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.681781 huza-0.2.8/huza/icons/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/icons/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33436 2022-01-04 03:29:52.000000 huza-0.2.8/huza/icons/iconbase.py
--rw-r--r--   0 root         (0) root         (0)     1281 2022-01-04 03:29:52.000000 huza-0.2.8/huza/icons/iconcore.py
--rw-r--r--   0 root         (0) root         (0)  1532400 2022-01-04 03:29:52.000000 huza-0.2.8/huza/icons/img.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.683781 huza-0.2.8/huza/mainwindow/
--rw-r--r--   0 root         (0) root         (0)       33 2022-01-04 03:29:52.000000 huza-0.2.8/huza/mainwindow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-04-04 07:57:27.000000 huza-0.2.8/huza/mainwindow/main.py
--rw-r--r--   0 root         (0) root         (0)      538 2022-01-04 03:29:52.000000 huza-0.2.8/huza/mainwindow/main_actions.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-04-04 07:57:27.000000 huza-0.2.8/huza/mainwindow/main_docks.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-06 07:13:51.000000 huza-0.2.8/huza/mainwindow/main_ribbon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.684781 huza-0.2.8/huza/ribbon/
--rw-r--r--   0 root         (0) root         (0)     1599 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/RibbonButton.py
--rw-r--r--   0 root         (0) root         (0)     2370 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/RibbonPane.py
--rw-r--r--   0 root         (0) root         (0)      719 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/RibbonTab.py
--rw-r--r--   0 root         (0) root         (0)      937 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/RibbonWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.686781 huza-0.2.8/huza/ribbon/qss/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/qss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6330 2022-07-25 02:53:50.000000 huza-0.2.8/huza/ribbon/qss/default_qss.py
--rw-r--r--   0 root         (0) root         (0)       55 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/qss/mainqss.py
--rw-r--r--   0 root         (0) root         (0)       97 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/qss/ribbonpaneqss.py
--rw-r--r--   0 root         (0) root         (0)      900 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/qss/ribbonqss.py
--rw-r--r--   0 root         (0) root         (0)      706 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/qss/ribbonsmallbuttonqss.py
--rw-r--r--   0 root         (0) root         (0)      745 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/qss/ribbosbutton.py
--rw-r--r--   0 root         (0) root         (0)      158 2022-01-04 03:29:52.000000 huza-0.2.8/huza/ribbon/scale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.686781 huza-0.2.8/huza/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1026 2022-06-16 03:42:50.000000 huza-0.2.8/huza/scripts/img2base64.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.686781 huza-0.2.8/huza/splash/
--rw-r--r--   0 root         (0) root         (0)      189 2022-01-04 03:29:52.000000 huza-0.2.8/huza/splash/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2269 2022-01-04 03:29:52.000000 huza-0.2.8/huza/splash/splash.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.687781 huza-0.2.8/huza/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.8/huza/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-04-03 08:25:57.000000 huza-0.2.8/huza/util/buildui.py
--rw-r--r--   0 root         (0) root         (0)     1070 2022-01-04 03:29:52.000000 huza-0.2.8/huza/util/constant.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-04 07:57:27.000000 huza-0.2.8/huza/util/mainui.py
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-06 07:13:51.000000 huza-0.2.8/huza/util/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 07:14:33.679781 huza-0.2.8/huza.egg-info/
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-06 07:14:33.000000 huza-0.2.8/huza.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1229 2023-04-06 07:14:33.000000 huza-0.2.8/huza.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 07:14:33.000000 huza-0.2.8/huza.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-06 07:14:33.000000 huza-0.2.8/huza.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-06 07:14:33.000000 huza-0.2.8/huza.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-06 07:14:33.000000 huza-0.2.8/huza.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-04 03:36:49.000000 huza-0.2.8/huza.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     5644 2022-01-04 03:29:52.000000 huza-0.2.8/nsis.nsi
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 07:14:33.687781 huza-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2001 2022-11-21 06:24:02.000000 huza-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.429268 huza-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1062 2022-11-21 06:24:02.000000 huza-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-10 02:15:56.429268 huza-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2022-11-21 06:24:02.000000 huza-0.2.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.420268 huza-0.2.9/huza/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.422268 huza-0.2.9/huza/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      751 2022-01-04 03:29:52.000000 huza-0.2.9/huza/base/action.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-05 12:11:37.000000 huza-0.2.9/huza/base/dockview.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2022-11-21 06:24:02.000000 huza-0.2.9/huza/base/mainwindow.py
+-rw-r--r--   0 root         (0) root         (0)     6674 2023-04-04 07:57:27.000000 huza-0.2.9/huza/base/mainwindow_run.py
+-rw-r--r--   0 root         (0) root         (0)      653 2022-05-17 09:25:15.000000 huza-0.2.9/huza/base/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.422268 huza-0.2.9/huza/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      701 2022-01-04 03:29:52.000000 huza-0.2.9/huza/cli/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.423268 huza-0.2.9/huza/icons/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33436 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/iconbase.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/iconcore.py
+-rw-r--r--   0 root         (0) root         (0)  1532400 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/img.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.425268 huza-0.2.9/huza/mainwindow/
+-rw-r--r--   0 root         (0) root         (0)       33 2022-01-04 03:29:52.000000 huza-0.2.9/huza/mainwindow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-04 07:57:27.000000 huza-0.2.9/huza/mainwindow/main.py
+-rw-r--r--   0 root         (0) root         (0)      538 2022-01-04 03:29:52.000000 huza-0.2.9/huza/mainwindow/main_actions.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-04-04 07:57:27.000000 huza-0.2.9/huza/mainwindow/main_docks.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-06 07:13:51.000000 huza-0.2.9/huza/mainwindow/main_ribbon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.426268 huza-0.2.9/huza/ribbon/
+-rw-r--r--   0 root         (0) root         (0)     1599 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonButton.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonPane.py
+-rw-r--r--   0 root         (0) root         (0)      719 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonTab.py
+-rw-r--r--   0 root         (0) root         (0)      937 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.428268 huza-0.2.9/huza/ribbon/qss/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6330 2022-07-25 02:53:50.000000 huza-0.2.9/huza/ribbon/qss/default_qss.py
+-rw-r--r--   0 root         (0) root         (0)       55 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/mainqss.py
+-rw-r--r--   0 root         (0) root         (0)       97 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbonpaneqss.py
+-rw-r--r--   0 root         (0) root         (0)      900 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbonqss.py
+-rw-r--r--   0 root         (0) root         (0)      706 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbonsmallbuttonqss.py
+-rw-r--r--   0 root         (0) root         (0)      745 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbosbutton.py
+-rw-r--r--   0 root         (0) root         (0)      158 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/scale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.428268 huza-0.2.9/huza/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2022-06-16 03:42:50.000000 huza-0.2.9/huza/scripts/img2base64.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.428268 huza-0.2.9/huza/splash/
+-rw-r--r--   0 root         (0) root         (0)      189 2022-01-04 03:29:52.000000 huza-0.2.9/huza/splash/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2022-01-04 03:29:52.000000 huza-0.2.9/huza/splash/splash.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.429268 huza-0.2.9/huza/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-04-03 08:25:57.000000 huza-0.2.9/huza/util/buildui.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-01-04 03:29:52.000000 huza-0.2.9/huza/util/constant.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-05-10 02:12:48.000000 huza-0.2.9/huza/util/mainui.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-10 02:12:48.000000 huza-0.2.9/huza/util/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.421268 huza-0.2.9/huza.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-04 03:36:49.000000 huza-0.2.9/huza.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     5644 2022-01-04 03:29:52.000000 huza-0.2.9/nsis.nsi
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 02:15:56.429268 huza-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-05-10 02:12:48.000000 huza-0.2.9/setup.py
```

### Comparing `huza-0.2.8/LICENSE` & `huza-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/PKG-INFO` & `huza-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: huza
-Version: 0.2.8
+Version: 0.2.9
 Summary: Self-use pyqt framework
 Home-page: https://github.com/huyidao625/Huza
 Author: hufei
 Author-email: hufei625@qq.com
 License: MIT License
+Project-URL: Wiki, https://www.hudh.cn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 Huza
 ======
 
 自用的PyQT框架
```

### Comparing `huza-0.2.8/huza/base/action.py` & `huza-0.2.9/huza/base/action.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/base/dockview.py` & `huza-0.2.9/huza/base/dockview.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/base/mainwindow.py` & `huza-0.2.9/huza/base/mainwindow.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/base/mainwindow_run.py` & `huza-0.2.9/huza/base/mainwindow_run.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/base/widget.py` & `huza-0.2.9/huza/base/widget.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/cli/shell.py` & `huza-0.2.9/huza/cli/shell.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/icons/iconbase.py` & `huza-0.2.9/huza/icons/iconbase.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/icons/iconcore.py` & `huza-0.2.9/huza/icons/iconcore.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/icons/img.py` & `huza-0.2.9/huza/icons/img.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/mainwindow/main.py` & `huza-0.2.9/huza/mainwindow/main.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/mainwindow/main_actions.py` & `huza-0.2.9/huza/mainwindow/main_actions.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/mainwindow/main_docks.py` & `huza-0.2.9/huza/mainwindow/main_docks.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/mainwindow/main_ribbon.py` & `huza-0.2.9/huza/mainwindow/main_ribbon.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/RibbonButton.py` & `huza-0.2.9/huza/ribbon/RibbonButton.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/RibbonPane.py` & `huza-0.2.9/huza/ribbon/RibbonPane.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/RibbonTab.py` & `huza-0.2.9/huza/ribbon/RibbonTab.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/RibbonWidget.py` & `huza-0.2.9/huza/ribbon/RibbonWidget.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/qss/default_qss.py` & `huza-0.2.9/huza/ribbon/qss/default_qss.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/qss/ribbonqss.py` & `huza-0.2.9/huza/ribbon/qss/ribbonqss.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/qss/ribbonsmallbuttonqss.py` & `huza-0.2.9/huza/ribbon/qss/ribbonsmallbuttonqss.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/ribbon/qss/ribbosbutton.py` & `huza-0.2.9/huza/ribbon/qss/ribbosbutton.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/scripts/img2base64.py` & `huza-0.2.9/huza/scripts/img2base64.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/splash/splash.py` & `huza-0.2.9/huza/splash/splash.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/util/buildui.py` & `huza-0.2.9/huza/util/buildui.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/util/constant.py` & `huza-0.2.9/huza/util/constant.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/huza/util/mainui.py` & `huza-0.2.9/huza/util/mainui.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     if dock_name in mainui.docks:
         return mainui.docks.get(dock_name)
     return None
 
 
 def get_dock_current_ui(mainui, dock_name: str):
     if dock_name in mainui.docks:
-        return mainui.docks.get(dock_name).widget().ui()
+        widget = mainui.docks.get(dock_name).widget()
+        if widget is None:
+            return None
+        return widget.ui()
     return None
 
 
 def get_dock_ui(mainui, dock_name: str, uiname: str):
     if dock_name in mainui.dockviews:
         dockviews = mainui.dockviews.get(dock_name)
         if uiname in dockviews:
```

### Comparing `huza-0.2.8/huza.egg-info/PKG-INFO` & `huza-0.2.9/huza.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: huza
-Version: 0.2.8
+Version: 0.2.9
 Summary: Self-use pyqt framework
 Home-page: https://github.com/huyidao625/Huza
 Author: hufei
 Author-email: hufei625@qq.com
 License: MIT License
+Project-URL: Wiki, https://www.hudh.cn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 Huza
 ======
 
 自用的PyQT框架
```

### Comparing `huza-0.2.8/huza.egg-info/SOURCES.txt` & `huza-0.2.9/huza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/nsis.nsi` & `huza-0.2.9/nsis.nsi`

 * *Files identical despite different names*

### Comparing `huza-0.2.8/setup.py` & `huza-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,10 +66,16 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Topic :: System :: Networking',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
-    ]
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
+    ],
+    project_urls={
+        'Wiki': 'https://www.hudh.cn'
+    }
+
 )
```

