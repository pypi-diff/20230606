# Comparing `tmp/pyqt-openai-0.1.51.tar.gz` & `tmp/pyqt-openai-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.1.51.tar", last modified: Sat May 20 09:19:25 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.61.tar", last modified: Tue Jun  6 13:44:24 2023, max compression
```

## Comparing `pyqt-openai-0.1.51.tar` & `pyqt-openai-0.1.61.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.581889 pyqt-openai-0.1.51/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.51/LICENSE
--rw-rw-rw-   0        0        0     6541 2023-05-20 09:19:25.580892 pyqt-openai-0.1.51/PKG-INFO
--rw-rw-rw-   0        0        0     6119 2023-05-20 08:13:30.000000 pyqt-openai-0.1.51/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.398221 pyqt-openai-0.1.51/pyqt_openai/
--rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     6737 2023-05-13 01:46:18.000000 pyqt-openai-0.1.51/pyqt_openai/a.py
--rw-rw-rw-   0        0        0     2316 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/aboutDialog.py
--rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/apiData.py
--rw-rw-rw-   0        0        0    13069 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/chatWidget.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.51/pyqt_openai/circleProfileImage.py
--rw-rw-rw-   0        0        0     5078 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/convListWidget.py
--rw-rw-rw-   0        0        0     7574 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/customizeDialog.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.488981 pyqt-openai-0.1.51/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.51/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.51/pyqt_openai/ico/add.svg
--rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.51/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.51/pyqt_openai/ico/customize.svg
--rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.51/pyqt_openai/ico/delete.svg
--rw-rw-rw-   0        0        0     1542 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/ico/discord.svg
--rw-rw-rw-   0        0        0     1552 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/ico/github.svg
--rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.51/pyqt_openai/ico/help.svg
--rw-rw-rw-   0        0        0      712 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/ico/history.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.51/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/ico/prompt.svg
--rw-rw-rw-   0        0        0      654 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/ico/save.svg
--rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.51/pyqt_openai/ico/search.svg
--rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.51/pyqt_openai/ico/setting.svg
--rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.51/pyqt_openai/ico/sidebar.svg
--rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.51/pyqt_openai/ico/stackontop.svg
--rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.51/pyqt_openai/ico/user.svg
--rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.51/pyqt_openai/ico/vertical_three_dots.svg
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.531863 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/__init__.py
--rw-rw-rw-   0        0        0     1558 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/currentImageView.py
--rw-rw-rw-   0        0        0     1735 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/explorerWidget.py
--rw-rw-rw-   0        0        0     3171 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageDallEPage.py
--rw-rw-rw-   0        0        0     4745 2023-05-20 09:19:05.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py
--rw-rw-rw-   0        0        0     5090 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageListWidget.py
--rw-rw-rw-   0        0        0    18549 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageSqlite.py
--rw-rw-rw-   0        0        0    10698 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py
--rw-rw-rw-   0        0        0     3867 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/leftSideBar.py
--rw-rw-rw-   0        0        0     1077 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/rightSideBar.py
--rw-rw-rw-   0        0        0     4044 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/thumbnailView.py
--rw-rw-rw-   0        0        0     2229 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/viewWidget.py
--rw-rw-rw-   0        0        0     1444 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/inputDialog.py
--rw-rw-rw-   0        0        0     3764 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/leftSideBar.py
--rw-rw-rw-   0        0        0    10956 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     1787 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/modelTable.py
--rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.51/pyqt_openai/notifier.py
--rw-rw-rw-   0        0        0    11060 2023-05-20 09:19:05.000000 pyqt-openai-0.1.51/pyqt_openai/openAiChatBotWidget.py
--rw-rw-rw-   0        0        0     3048 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/openAiThread.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.540840 pyqt-openai-0.1.51/pyqt_openai/prompt/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/prompt/__init__.py
--rw-rw-rw-   0        0        0     1780 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/prompt/promptGeneratorWidget.py
--rw-rw-rw-   0        0        0     9231 2023-05-20 09:19:05.000000 pyqt-openai-0.1.51/pyqt_openai/prompt/propPage.py
--rw-rw-rw-   0        0        0     4384 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/prompt/templatePage.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.552809 pyqt-openai-0.1.51/pyqt_openai/right_sidebar/
--rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/right_sidebar/__init__.py
--rw-rw-rw-   0        0        0     2060 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
--rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.51/pyqt_openai/right_sidebar/chatPage.py
--rw-rw-rw-   0        0        0    10982 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/right_sidebar/completionPage.py
--rw-rw-rw-   0        0        0     1623 2023-05-07 22:16:16.000000 pyqt-openai-0.1.51/pyqt_openai/right_sidebar/imagePage.py
--rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.51/pyqt_openai/searchBar.py
--rw-rw-rw-   0        0        0    30652 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/sqlite.py
--rw-rw-rw-   0        0        0     5918 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.51/pyqt_openai/svgLabel.py
--rw-rw-rw-   0        0        0     5935 2023-05-07 05:04:02.000000 pyqt-openai-0.1.51/pyqt_openai/svgToolButton.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.565931 pyqt-openai-0.1.51/pyqt_openai/test/
--rw-rw-rw-   0        0        0        0 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/test/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-05-05 02:56:55.000000 pyqt-openai-0.1.51/pyqt_openai/test/htmlformat.py
--rw-rw-rw-   0        0        0     4414 2023-05-13 01:46:18.000000 pyqt-openai-0.1.51/pyqt_openai/test/prompt_autocomplete.py
--rw-rw-rw-   0        0        0      908 2023-05-13 01:46:18.000000 pyqt-openai-0.1.51/pyqt_openai/test/rightSideBarTab.py
--rw-rw-rw-   0        0        0      761 2023-05-20 05:39:27.000000 pyqt-openai-0.1.51/pyqt_openai/test/sqlalchemy_example.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.568928 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/
--rw-rw-rw-   0        0        0        0 2023-05-05 07:22:12.000000 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.578934 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/in_model/
--rw-rw-rw-   0        0        0        0 2023-05-07 08:08:35.000000 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/in_model/__init__.py
--rw-rw-rw-   0        0        0      722 2023-05-05 12:31:35.000000 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/in_model/delete_model.py
--rw-rw-rw-   0        0        0     2559 2023-05-05 07:22:36.000000 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/in_model/make_model.py
--rw-rw-rw-   0        0        0      816 2023-05-11 12:24:04.000000 pyqt-openai-0.1.51/pyqt_openai/test/stable_diffusion/in_model/using_model.py
-drwxrwxrwx   0        0        0        0 2023-05-20 09:19:25.446093 pyqt-openai-0.1.51/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     6541 2023-05-20 09:19:25.000000 pyqt-openai-0.1.51/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2592 2023-05-20 09:19:25.000000 pyqt-openai-0.1.51/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 09:19:25.000000 pyqt-openai-0.1.51/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-20 09:19:25.000000 pyqt-openai-0.1.51/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 09:19:25.000000 pyqt-openai-0.1.51/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 09:19:25.581889 pyqt-openai-0.1.51/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-05-20 09:19:05.000000 pyqt-openai-0.1.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.640789 pyqt-openai-0.1.61/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.61/LICENSE
+-rw-rw-rw-   0        0        0     9704 2023-06-06 13:44:24.638794 pyqt-openai-0.1.61/PKG-INFO
+-rw-rw-rw-   0        0        0     9222 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.268123 pyqt-openai-0.1.61/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6737 2023-06-04 01:26:54.000000 pyqt-openai-0.1.61/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2756 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/aboutDialog.py
+-rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/apiData.py
+-rw-rw-rw-   0        0        0    16579 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/chatWidget.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.61/pyqt_openai/circleProfileImage.py
+-rw-rw-rw-   0        0        0     3337 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/commandCompleter.py
+-rw-rw-rw-   0        0        0     5078 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/convListWidget.py
+-rw-rw-rw-   0        0        0     7574 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/customizeDialog.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.459606 pyqt-openai-0.1.61/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.61/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.61/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.61/pyqt_openai/ico/customize.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0     1542 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/discord.svg
+-rw-rw-rw-   0        0        0     1552 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/github.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0      712 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/history.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.61/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0      654 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/save.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.61/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.61/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.61/pyqt_openai/ico/user.svg
+-rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.61/pyqt_openai/ico/vertical_three_dots.svg
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.526531 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/__init__.py
+-rw-rw-rw-   0        0        0     1558 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/currentImageView.py
+-rw-rw-rw-   0        0        0     1735 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/explorerWidget.py
+-rw-rw-rw-   0        0        0     3581 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageDallEPage.py
+-rw-rw-rw-   0        0        0     4558 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py
+-rw-rw-rw-   0        0        0     5090 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageListWidget.py
+-rw-rw-rw-   0        0        0    18549 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageSqlite.py
+-rw-rw-rw-   0        0        0    11118 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py
+-rw-rw-rw-   0        0        0     3867 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/leftSideBar.py
+-rw-rw-rw-   0        0        0     1077 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/rightSideBar.py
+-rw-rw-rw-   0        0        0     4044 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/thumbnailView.py
+-rw-rw-rw-   0        0        0     2229 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/viewWidget.py
+-rw-rw-rw-   0        0        0     1444 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3764 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    11458 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1787 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3293 2023-06-06 02:12:45.000000 pyqt-openai-0.1.61/pyqt_openai/notifier.py
+-rw-rw-rw-   0        0        0    11028 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/openAiChatBotWidget.py
+-rw-rw-rw-   0        0        0     3048 2023-06-03 03:53:41.000000 pyqt-openai-0.1.61/pyqt_openai/openAiThread.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.542478 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/__init__.py
+-rw-rw-rw-   0        0        0     2423 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     1768 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py
+-rw-rw-rw-   0        0        0     9467 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPage.py
+-rw-rw-rw-   0        0        0     1755 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPromptUnitInputDialog.py
+-rw-rw-rw-   0        0        0     9492 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/templatePage.py
+-rw-rw-rw-   0        0        0     1778 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/templatePromptUnitInputDialog.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.547452 pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/__init__.py
+-rw-rw-rw-   0        0        0      988 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/commandSuggestionWidget.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.591924 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2060 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    10982 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-07 22:16:16.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0   112813 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5934 2023-06-06 02:12:45.000000 pyqt-openai-0.1.61/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      738 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/svgLabel.py
+-rw-rw-rw-   0        0        0     5951 2023-06-06 02:12:45.000000 pyqt-openai-0.1.61/pyqt_openai/svgToolButton.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.635806 pyqt-openai-0.1.61/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-05-21 02:10:54.000000 pyqt-openai-0.1.61/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-05-21 02:10:54.000000 pyqt-openai-0.1.61/pyqt_openai/test/htmlformat.py
+-rw-rw-rw-   0        0        0      761 2023-05-21 02:10:54.000000 pyqt-openai-0.1.61/pyqt_openai/test/sqlalchemy_example.py
+-rw-rw-rw-   0        0        0     4884 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/toast.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.306025 pyqt-openai-0.1.61/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0     9704 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2629 2023-06-06 13:44:24.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 13:44:24.641788 pyqt-openai-0.1.61/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-06-06 13:44:08.000000 pyqt-openai-0.1.61/setup.py
```

### Comparing `pyqt-openai-0.1.51/LICENSE` & `pyqt-openai-0.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/PKG-INFO` & `pyqt-openai-0.1.61/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.51
+Version: 0.1.61
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,64 +55,124 @@
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable, autosaved in database)
+* support prompt generator (manageable, autosaved in database) 
 * support slash commands
 * support beginning and ending part of the prompt
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 * image generation (DALL-E, Stable Diffusion with DreamStudio API)
 * you can copy and download the image if you want. just hover the mouse cursor over the image.
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
-* pyperclip - to copy prompt template from prompt generator
+* aiohttp - for openai dependency 
+* pyperclip - to copy prompt text from prompt generator
 * stability_sdk - for Stable Diffusion
 
 ## Preview & Usage
 ### Overview
-#### Note: Some of these previews are not the latest.
+#### Windows
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
 <b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
 
 You can change screen between text chatbot and image generating tool screen.
+
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061)
 
+#### Linux (Ubuntu)
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba)
+
+If you use MacOS, please give me the pyqt-openai screen image from it.
+
 ### Conversation
+#### Preview 1
+I recorded this preview long time ago so GUI is different from the current version, but way of operating it is pretty much the same.
+
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
+#### Preview 2 (using prompt feature)
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead
 
 ### Prompt Generator
-https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-1e8c-4ba2-b5fe-4391df6250ff
+#### How to Generate
+This application has two types of prompts. One is <b>"Properties"</b> and the other one is <b>"Template"</b>. Properties are sets of attributes that are useful for forming the premises of a question. Templates are sentences that correspond to a single command. You can input a command to generate a sentence. This can be used as a question in itself.
+
+Both types can be managed as groups. After cloning or installing, if you run the program immediately, you will be able to see the default group and the items included in the group, just like the screen.
+
+For properties, there is a group named "Default" that provides a set of attributes referenced <a href="https://gptforwork.com/tools/prompt-generator">here</a>.
 
-You can use the additional prompt feature by "prompt menu" right next to input field.
+For templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example prompt for Alex Brogan) groups provided. Any custom template items created prior to version 0.1.6 will be moved to the Miscellaneous group.
+
+![prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/ce40139a-c03f-42ef-abd8-4a610d762394)
+
+With using these prompts you can pretty much get any response you want.
+
+You can use the additional prompt feature by "prompt menu" right next to "prompt input" field.
 
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
 
+Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
+
+#### Prompt Generator Preview
+Generating the prompt (Properties)
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-3c42c9c23602
+
+I recorded using the Windows recording feature. As a result, the "Add Dialog" that prompts for entering a group name does not appear in the preview. When you add a group, you will see the Add Dialog as expected.
+
+Then, how to generate template type prompt? Click any item in the group, it will be shown in the preview.
+
+You can copy that generated text with clicking "copy" button and include it to your prompt input.
+
+If you add a property group or template group with items, you can use it as a command by typing its name to the prompt input.
+
+<b>Use prompt as a command</b>
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553
+
+In this preview, i pressed the keyboard shortcut of each actions(show beginning, show ending, support prompt command) to use it rather than clicking them with mouse.
+
+I made the command suggestion GUI resemble the Discord command autocomplete popup, with which a lot of people have become accustomed.
+
 ### Image Generation
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
 
 ## How to Install
-1. open command propmt of your OS.
-2. git clone ~
-3. from the root directory, type "cd pyqt_openai"
-4. pip install -r requirements.txt
+1. git clone ~
+2. cd pyqt-openai
+3. pip install -r requirements.txt
+4. cd pyqt_openai
 5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
 6. python main.py
 
-If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error. 
+If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error.
+
+### Note
+If you use Linux and see this error:
+```
+qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it was found
+
+this application failed to start because no qt platform plugin could be initialized, reinstalling the application may fix this problem
+```
+
+run this command:
+```
+sudo apt-get install libxcb-xinerama0
+```
 
 ## Troubleshooting
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
 download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.51 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.61 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
@@ -29,48 +29,87 @@
 * support prompt generator (manageable, autosaved in database) * support slash
 commands * support beginning and ending part of the prompt * you can run this
 in background application * notification will pop up when response is generated
 * you can make window stack on top or control its transparency * image
 generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
 download the image if you want. just hover the mouse cursor over the image. ##
 Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * pyperclip - to copy
-prompt template from prompt generator * stability_sdk - for Stable Diffusion ##
-Preview & Usage ### Overview #### Note: Some of these previews are not the
-latest. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * aiohttp - for openai
+dependency * pyperclip - to copy prompt text from prompt generator *
+stability_sdk - for Stable Diffusion ## Preview & Usage ### Overview ####
+Windows ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
 51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
 inside the red box. see [How to install](#how-to-install) You can change screen
 between text chatbot and image generating tool screen. ![image](https://
 github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
-07655cab2061) ### Conversation https://user-images.githubusercontent.com/
-55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-
-1e8c-4ba2-b5fe-4391df6250ff You can use the additional prompt feature by
-"prompt menu" right next to input field. ![image](https://github.com/yjg30737/
-pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663) ### Image
-Generation ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install 1. open command propmt
-of your OS. 2. git clone ~ 3. from the root directory, type "cd pyqt_openai" 4.
-pip install -r requirements.txt 5. You should put your api key in the line
-edit. You can get it in official_site of openai. Sign up and log in before you
-get it. Be sure, this is a very important API key that belongs to you only, so
-you should remember it and keep it secure. 6. python main.py If installation
-doesn't work, you can contact me with bring up new issue in issue tab or check
-the troubleshooting below even it is only about very specific error. ##
-Troubleshooting If you see this error while installing the openai package ```
-subprocess-exited-with-error ``` download the package itself from pypi. Unzip
-it, access the package directory, type ``` python setup.py install ``` That
-will install the openai. Note: I don't know this can happen in newer version of
-openai as well, so tell me if you know about something ## Contact You can join
-pyqt-openai's Discord_Server to have a conversation about it or AI-related
-stuff ð ## Note I recommend to install sqlite management software. It's not
-necessary to run this app (obviously), but it's good practice to manage
-database about conversation history with AI and to know how this works. ## TODO
-list * DB for images (to further experiement of both DALL-E and Stable
-Diffusion or other image generation engine) * show the explanation of every
-model and terms related to AI (e.g. temperature, topp..) * save conversation
-history with other format (xlsx, csv, etc.) * tokenizer * highlight the source
-(optional, eventually) * support multiple language * use SQLAlchemy (maybe not)
-* show reason when the chat input is disabled for some reasons * add the basic
-example sources of making deep learning model with PyTorch (eventually) ## See
-Also * Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access
-from it * join_chatgpt_plugins_waitlist
+07655cab2061) #### Linux (Ubuntu) ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS,
+please give me the pyqt-openai screen image from it. ### Conversation ####
+Preview 1 I recorded this preview long time ago so GUI is different from the
+current version, but way of operating it is pretty much the same. https://user-
+images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-
+f60d8b2d6ced.mp4 #### Preview 2 (using prompt feature) https://github.com/
+yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ###
+Prompt Generator #### How to Generate This application has two types of
+prompts. One is "Properties" and the other one is "Template". Properties are
+sets of attributes that are useful for forming the premises of a question.
+Templates are sentences that correspond to a single command. You can input a
+command to generate a sentence. This can be used as a question in itself. Both
+types can be managed as groups. After cloning or installing, if you run the
+program immediately, you will be able to see the default group and the items
+included in the group, just like the screen. For properties, there is a group
+named "Default" that provides a set of attributes referenced here. For
+templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example
+prompt for Alex Brogan) groups provided. Any custom template items created
+prior to version 0.1.6 will be moved to the Miscellaneous group. !
+[prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+ce40139a-c03f-42ef-abd8-4a610d762394) With using these prompts you can pretty
+much get any response you want. You can use the additional prompt feature by
+"prompt menu" right next to "prompt input" field. ![image](https://github.com/
+yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
+Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
+#### Prompt Generator Preview Generating the prompt (Properties) https://
+github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-
+3c42c9c23602 I recorded using the Windows recording feature. As a result, the
+"Add Dialog" that prompts for entering a group name does not appear in the
+preview. When you add a group, you will see the Add Dialog as expected. Then,
+how to generate template type prompt? Click any item in the group, it will be
+shown in the preview. You can copy that generated text with clicking "copy"
+button and include it to your prompt input. If you add a property group or
+template group with items, you can use it as a command by typing its name to
+the prompt input. Use prompt as a command https://github.com/yjg30737/pyqt-
+openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553 In this preview, i
+pressed the keyboard shortcut of each actions(show beginning, show ending,
+support prompt command) to use it rather than clicking them with mouse. I made
+the command suggestion GUI resemble the Discord command autocomplete popup,
+with which a lot of people have become accustomed. ### Image Generation !
+[image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-
+4900-bfea-89da6f072c9d) ## How to Install 1. git clone ~ 2. cd pyqt-openai 3.
+pip install -r requirements.txt 4. cd pyqt_openai 5. You should put your api
+key in the line edit. You can get it in official_site of openai. Sign up and
+log in before you get it. Be sure, this is a very important API key that
+belongs to you only, so you should remember it and keep it secure. 6. python
+main.py If installation doesn't work, you can contact me with bring up new
+issue in issue tab or check the troubleshooting below even it is only about
+very specific error. ### Note If you use Linux and see this error: ```
+qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it
+was found this application failed to start because no qt platform plugin could
+be initialized, reinstalling the application may fix this problem ``` run this
+command: ``` sudo apt-get install libxcb-xinerama0 ``` ## Troubleshooting If
+you see this error while installing the openai package ``` subprocess-exited-
+with-error ``` download the package itself from pypi. Unzip it, access the
+package directory, type ``` python setup.py install ``` That will install the
+openai. Note: I don't know this can happen in newer version of openai as well,
+so tell me if you know about something ## Contact You can join pyqt-openai's
+Discord_Server to have a conversation about it or AI-related stuff ð ## Note
+I recommend to install sqlite management software. It's not necessary to run
+this app (obviously), but it's good practice to manage database about
+conversation history with AI and to know how this works. ## TODO list * DB for
+images (to further experiement of both DALL-E and Stable Diffusion or other
+image generation engine) * show the explanation of every model and terms
+related to AI (e.g. temperature, topp..) * save conversation history with other
+format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
+eventually) * support multiple language * use SQLAlchemy (maybe not) * show
+reason when the chat input is disabled for some reasons * add the basic example
+sources of making deep learning model with PyTorch (eventually) ## See Also *
+Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
+it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.51/README.md` & `pyqt-openai-0.1.61/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -43,64 +43,124 @@
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable, autosaved in database)
+* support prompt generator (manageable, autosaved in database) 
 * support slash commands
 * support beginning and ending part of the prompt
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 * image generation (DALL-E, Stable Diffusion with DreamStudio API)
 * you can copy and download the image if you want. just hover the mouse cursor over the image.
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
-* pyperclip - to copy prompt template from prompt generator
+* aiohttp - for openai dependency 
+* pyperclip - to copy prompt text from prompt generator
 * stability_sdk - for Stable Diffusion
 
 ## Preview & Usage
 ### Overview
-#### Note: Some of these previews are not the latest.
+#### Windows
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
 <b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
 
 You can change screen between text chatbot and image generating tool screen.
+
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061)
 
+#### Linux (Ubuntu)
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba)
+
+If you use MacOS, please give me the pyqt-openai screen image from it.
+
 ### Conversation
+#### Preview 1
+I recorded this preview long time ago so GUI is different from the current version, but way of operating it is pretty much the same.
+
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
+#### Preview 2 (using prompt feature)
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead
 
 ### Prompt Generator
-https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-1e8c-4ba2-b5fe-4391df6250ff
+#### How to Generate
+This application has two types of prompts. One is <b>"Properties"</b> and the other one is <b>"Template"</b>. Properties are sets of attributes that are useful for forming the premises of a question. Templates are sentences that correspond to a single command. You can input a command to generate a sentence. This can be used as a question in itself.
+
+Both types can be managed as groups. After cloning or installing, if you run the program immediately, you will be able to see the default group and the items included in the group, just like the screen.
+
+For properties, there is a group named "Default" that provides a set of attributes referenced <a href="https://gptforwork.com/tools/prompt-generator">here</a>.
 
-You can use the additional prompt feature by "prompt menu" right next to input field.
+For templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example prompt for Alex Brogan) groups provided. Any custom template items created prior to version 0.1.6 will be moved to the Miscellaneous group.
+
+![prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/ce40139a-c03f-42ef-abd8-4a610d762394)
+
+With using these prompts you can pretty much get any response you want.
+
+You can use the additional prompt feature by "prompt menu" right next to "prompt input" field.
 
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
 
+Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
+
+#### Prompt Generator Preview
+Generating the prompt (Properties)
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-3c42c9c23602
+
+I recorded using the Windows recording feature. As a result, the "Add Dialog" that prompts for entering a group name does not appear in the preview. When you add a group, you will see the Add Dialog as expected.
+
+Then, how to generate template type prompt? Click any item in the group, it will be shown in the preview.
+
+You can copy that generated text with clicking "copy" button and include it to your prompt input.
+
+If you add a property group or template group with items, you can use it as a command by typing its name to the prompt input.
+
+<b>Use prompt as a command</b>
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553
+
+In this preview, i pressed the keyboard shortcut of each actions(show beginning, show ending, support prompt command) to use it rather than clicking them with mouse.
+
+I made the command suggestion GUI resemble the Discord command autocomplete popup, with which a lot of people have become accustomed.
+
 ### Image Generation
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
 
 ## How to Install
-1. open command propmt of your OS.
-2. git clone ~
-3. from the root directory, type "cd pyqt_openai"
-4. pip install -r requirements.txt
+1. git clone ~
+2. cd pyqt-openai
+3. pip install -r requirements.txt
+4. cd pyqt_openai
 5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
 6. python main.py
 
-If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error. 
+If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error.
+
+### Note
+If you use Linux and see this error:
+```
+qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it was found
+
+this application failed to start because no qt platform plugin could be initialized, reinstalling the application may fix this problem
+```
+
+run this command:
+```
+sudo apt-get install libxcb-xinerama0
+```
 
 ## Troubleshooting
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
 download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>.
```

#### html2text {}

```diff
@@ -26,48 +26,87 @@
 * support prompt generator (manageable, autosaved in database) * support slash
 commands * support beginning and ending part of the prompt * you can run this
 in background application * notification will pop up when response is generated
 * you can make window stack on top or control its transparency * image
 generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
 download the image if you want. just hover the mouse cursor over the image. ##
 Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * pyperclip - to copy
-prompt template from prompt generator * stability_sdk - for Stable Diffusion ##
-Preview & Usage ### Overview #### Note: Some of these previews are not the
-latest. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * aiohttp - for openai
+dependency * pyperclip - to copy prompt text from prompt generator *
+stability_sdk - for Stable Diffusion ## Preview & Usage ### Overview ####
+Windows ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
 51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
 inside the red box. see [How to install](#how-to-install) You can change screen
 between text chatbot and image generating tool screen. ![image](https://
 github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
-07655cab2061) ### Conversation https://user-images.githubusercontent.com/
-55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-
-1e8c-4ba2-b5fe-4391df6250ff You can use the additional prompt feature by
-"prompt menu" right next to input field. ![image](https://github.com/yjg30737/
-pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663) ### Image
-Generation ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install 1. open command propmt
-of your OS. 2. git clone ~ 3. from the root directory, type "cd pyqt_openai" 4.
-pip install -r requirements.txt 5. You should put your api key in the line
-edit. You can get it in official_site of openai. Sign up and log in before you
-get it. Be sure, this is a very important API key that belongs to you only, so
-you should remember it and keep it secure. 6. python main.py If installation
-doesn't work, you can contact me with bring up new issue in issue tab or check
-the troubleshooting below even it is only about very specific error. ##
-Troubleshooting If you see this error while installing the openai package ```
-subprocess-exited-with-error ``` download the package itself from pypi. Unzip
-it, access the package directory, type ``` python setup.py install ``` That
-will install the openai. Note: I don't know this can happen in newer version of
-openai as well, so tell me if you know about something ## Contact You can join
-pyqt-openai's Discord_Server to have a conversation about it or AI-related
-stuff ð ## Note I recommend to install sqlite management software. It's not
-necessary to run this app (obviously), but it's good practice to manage
-database about conversation history with AI and to know how this works. ## TODO
-list * DB for images (to further experiement of both DALL-E and Stable
-Diffusion or other image generation engine) * show the explanation of every
-model and terms related to AI (e.g. temperature, topp..) * save conversation
-history with other format (xlsx, csv, etc.) * tokenizer * highlight the source
-(optional, eventually) * support multiple language * use SQLAlchemy (maybe not)
-* show reason when the chat input is disabled for some reasons * add the basic
-example sources of making deep learning model with PyTorch (eventually) ## See
-Also * Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access
-from it * join_chatgpt_plugins_waitlist
+07655cab2061) #### Linux (Ubuntu) ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS,
+please give me the pyqt-openai screen image from it. ### Conversation ####
+Preview 1 I recorded this preview long time ago so GUI is different from the
+current version, but way of operating it is pretty much the same. https://user-
+images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-
+f60d8b2d6ced.mp4 #### Preview 2 (using prompt feature) https://github.com/
+yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ###
+Prompt Generator #### How to Generate This application has two types of
+prompts. One is "Properties" and the other one is "Template". Properties are
+sets of attributes that are useful for forming the premises of a question.
+Templates are sentences that correspond to a single command. You can input a
+command to generate a sentence. This can be used as a question in itself. Both
+types can be managed as groups. After cloning or installing, if you run the
+program immediately, you will be able to see the default group and the items
+included in the group, just like the screen. For properties, there is a group
+named "Default" that provides a set of attributes referenced here. For
+templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example
+prompt for Alex Brogan) groups provided. Any custom template items created
+prior to version 0.1.6 will be moved to the Miscellaneous group. !
+[prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+ce40139a-c03f-42ef-abd8-4a610d762394) With using these prompts you can pretty
+much get any response you want. You can use the additional prompt feature by
+"prompt menu" right next to "prompt input" field. ![image](https://github.com/
+yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
+Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
+#### Prompt Generator Preview Generating the prompt (Properties) https://
+github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-
+3c42c9c23602 I recorded using the Windows recording feature. As a result, the
+"Add Dialog" that prompts for entering a group name does not appear in the
+preview. When you add a group, you will see the Add Dialog as expected. Then,
+how to generate template type prompt? Click any item in the group, it will be
+shown in the preview. You can copy that generated text with clicking "copy"
+button and include it to your prompt input. If you add a property group or
+template group with items, you can use it as a command by typing its name to
+the prompt input. Use prompt as a command https://github.com/yjg30737/pyqt-
+openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553 In this preview, i
+pressed the keyboard shortcut of each actions(show beginning, show ending,
+support prompt command) to use it rather than clicking them with mouse. I made
+the command suggestion GUI resemble the Discord command autocomplete popup,
+with which a lot of people have become accustomed. ### Image Generation !
+[image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-
+4900-bfea-89da6f072c9d) ## How to Install 1. git clone ~ 2. cd pyqt-openai 3.
+pip install -r requirements.txt 4. cd pyqt_openai 5. You should put your api
+key in the line edit. You can get it in official_site of openai. Sign up and
+log in before you get it. Be sure, this is a very important API key that
+belongs to you only, so you should remember it and keep it secure. 6. python
+main.py If installation doesn't work, you can contact me with bring up new
+issue in issue tab or check the troubleshooting below even it is only about
+very specific error. ### Note If you use Linux and see this error: ```
+qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it
+was found this application failed to start because no qt platform plugin could
+be initialized, reinstalling the application may fix this problem ``` run this
+command: ``` sudo apt-get install libxcb-xinerama0 ``` ## Troubleshooting If
+you see this error while installing the openai package ``` subprocess-exited-
+with-error ``` download the package itself from pypi. Unzip it, access the
+package directory, type ``` python setup.py install ``` That will install the
+openai. Note: I don't know this can happen in newer version of openai as well,
+so tell me if you know about something ## Contact You can join pyqt-openai's
+Discord_Server to have a conversation about it or AI-related stuff ð ## Note
+I recommend to install sqlite management software. It's not necessary to run
+this app (obviously), but it's good practice to manage database about
+conversation history with AI and to know how this works. ## TODO list * DB for
+images (to further experiement of both DALL-E and Stable Diffusion or other
+image generation engine) * show the explanation of every model and terms
+related to AI (e.g. temperature, topp..) * save conversation history with other
+format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
+eventually) * support multiple language * use SQLAlchemy (maybe not) * show
+reason when the chat input is disabled for some reasons * add the basic example
+sources of making deep learning model with PyTorch (eventually) ## See Also *
+Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
+it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/a.py` & `pyqt-openai-0.1.61/pyqt_openai/a.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/aboutDialog.py` & `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,58 @@
-from qtpy.QtCore import Qt, QUrl
-from qtpy.QtGui import QPixmap, QDesktopServices
-from qtpy.QtWidgets import QDialog, QPushButton, QHBoxLayout, QWidget, QVBoxLayout, QLabel
+import re
 
-from pyqt_openai.svgLabel import SvgLabel
+from qtpy.QtCore import Qt
+from qtpy.QtWidgets import QDialog, QVBoxLayout, QLineEdit, QFrame, QPushButton, QHBoxLayout, QWidget
 
+from pyqt_openai.sqlite import SqliteDatabase
 
-class ClickableLabel(SvgLabel):
-    def __init__(self):
-        super().__init__()
-        self.__url = '127.0.0.1'
 
-    def setUrl(self, url):
-        self.__url = url
-
-    def mouseReleaseEvent(self, QMouseEvent):
-        if QMouseEvent.button() == Qt.LeftButton:
-            QDesktopServices.openUrl(QUrl(self.__url))
-
-
-class AboutDialog(QDialog):
-    def __init__(self):
-        super().__init__()
+class PromptGroupInputDialog(QDialog):
+    def __init__(self, db: SqliteDatabase, parent=None):
+        super().__init__(parent)
+        self.__initVal(db)
         self.__initUi()
 
+    def __initVal(self, db):
+        self.__db = db
+
     def __initUi(self):
-        self.setWindowTitle('About')
+        self.setWindowTitle('New Prompt')
         self.setWindowFlags(Qt.Window | Qt.WindowCloseButtonHint)
 
-        self.__okBtn = QPushButton('OK')
-        self.__okBtn.clicked.connect(self.accept)
+        self.__newName = QLineEdit()
+        self.__newName.textChanged.connect(self.__setAccept)
 
-        p = QPixmap('pyqtopenai.png')
-        logoLbl = QLabel()
-        logoLbl.setPixmap(p)
-
-        expWidget = QLabel()
-        expWidget.setText('''
-        <h1>pyqt-openai</h1>
-        <p>Powered by qtpy</p>
-        ''')
-        expWidget.setAlignment(Qt.AlignTop)
-
-        self.__githubLbl = ClickableLabel()
-        self.__githubLbl.setSvgFile('ico/github.svg')
-        self.__githubLbl.setUrl('https://github.com/yjg30737/pyqt-openai')
-
-        self.__discordLbl = ClickableLabel()
-        self.__discordLbl.setSvgFile('ico/discord.svg')
-        self.__discordLbl.setUrl('https://discord.gg/cHekprskVE')
-        self.__discordLbl.setFixedSize(22, 19)
+        sep = QFrame()
+        sep.setFrameShape(QFrame.HLine)
+        sep.setFrameShadow(QFrame.Sunken)
 
-        lay = QHBoxLayout()
-        lay.addWidget(logoLbl)
-        lay.addWidget(expWidget)
-        lay.addWidget(self.__githubLbl)
-        lay.addWidget(self.__discordLbl)
-
-        topWidget = QWidget()
-        topWidget.setLayout(lay)
+        self.__okBtn = QPushButton('OK')
+        self.__okBtn.clicked.connect(self.accept)
 
         cancelBtn = QPushButton('Cancel')
         cancelBtn.clicked.connect(self.close)
 
         lay = QHBoxLayout()
         lay.addWidget(self.__okBtn)
         lay.addWidget(cancelBtn)
         lay.setAlignment(Qt.AlignRight)
         lay.setContentsMargins(0, 0, 0, 0)
 
         okCancelWidget = QWidget()
         okCancelWidget.setLayout(lay)
 
         lay = QVBoxLayout()
-        lay.addWidget(topWidget)
+        lay.addWidget(self.__newName)
+        lay.addWidget(sep)
         lay.addWidget(okCancelWidget)
 
         self.setLayout(lay)
 
+    def getPromptGroupName(self):
+        return self.__newName.text()
+
+    def __setAccept(self, text):
+        m = re.search('^[a-zA-Z_0-9]+$', text)
+        names = [obj[1] for obj in self.__db.selectPropPromptGroup()+self.__db.selectTemplatePromptGroup()]
+        f = (True if m else False) and text not in names
+        self.__okBtn.setEnabled(f)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/apiData.py` & `pyqt-openai-0.1.61/pyqt_openai/apiData.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/chatWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/chatWidget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from qtpy.QtCore import Qt, Signal
 from qtpy.QtGui import QFont, QTextCursor
 from qtpy.QtWidgets import QScrollArea, QCompleter, QVBoxLayout, QToolButton, QMenu, QAction, QWidget, QLabel, \
     QHBoxLayout, QTextEdit, QStackedWidget
 
+from pyqt_openai.commandCompleter import CommandCompleter
+from pyqt_openai.propmt_command_completer.commandSuggestionWidget import CommandSuggestionWidget
 from pyqt_openai.sqlite import SqliteDatabase
 from pyqt_openai.svgToolButton import SvgToolButton
 
 
 class ChatBrowser(QScrollArea):
     convUnitUpdated = Signal(int, int, str)
 
@@ -140,139 +142,120 @@
         self.widget().setCurrentIndex(1)
         for i in range(len(conv_data)):
             self.__setLabel(conv_data[i], False, not bool(i % 2))
 
 
 class TextEditPrompt(QTextEdit):
     returnPressed = Signal()
+    sendSuggestionWidget = Signal(str)
 
-    def __init__(self, db: SqliteDatabase):
+    def __init__(self):
         super().__init__()
-        self.__initVal(db)
+        self.__initVal()
         self.__initUi()
 
-    def __initVal(self, db):
-        self.__command_f = False
-        self.__completer = None
-        self.__db = db
+    def __initVal(self):
+        self.__commandSuggestionEnabled = False
 
     def __initUi(self):
-        self.__initPromptCommandAutocomplete()
         self.setStyleSheet('QTextEdit { border: 1px solid #AAA; } ')
 
-    def setPromptCommandAutocompletedEnabled(self, f):
-        self.__command_f = f
-
-    def __initPromptCommandAutocomplete(self):
-        p_grp = []
-        for group in self.__db.selectPropPromptGroup():
-            p_grp_attr = [attr for attr in self.__db.selectPropPromptAttribute(group[0])]
-            p_grp_value = ''
-            for attr_obj in p_grp_attr:
-                name = attr_obj[2]
-                value = attr_obj[3]
-                if value and value.strip():
-                    p_grp_value += f'{name}: {value}\n'
-            p_grp.append({'name': group[1], 'value': p_grp_value})
-
-        t_grp = [{'name': obj[1], 'value': obj[2]} for obj in self.__db.selectTemplatePrompt()]
-
-        self.__total_grp = p_grp+t_grp
-
-        # only name
-        grp_nm_arr = [obj['name'] for obj in self.__total_grp]
-
-        completer = QCompleter(grp_nm_arr)
-        completer.activated.connect(self.__activated)
-        self.setCompleter(completer)
-
-    def __activated(self, word):
-        for item in self.__total_grp:
-            if item['name'] == word:
-                v = item['value']
-                break
-        else:
-            # Handle the case when 'b' is not found
-            v = ''
-        self.textCursor().deletePreviousChar()
-        self.insertPlainText(v)
-
-    def setCompleter(self, completer):
-        if self.__completer:
-            self.__completer.activated.disconnect()
-
-        self.__completer = completer
-        self.__completer.setWidget(self)
-        self.__completer.setCompletionMode(QCompleter.PopupCompletion)
+    def setCommandSuggestionEnabled(self, f):
+        self.__commandSuggestionEnabled = f
 
     def keyPressEvent(self, e):
-        if self.__command_f:
-            if self.__completer and self.__completer.popup().isVisible():
-                if e.key() in (Qt.Key_Enter, Qt.Key_Return, Qt.Key_Escape, Qt.Key_Tab, Qt.Key_Backtab):
-                    e.ignore()
-                    return
-
-            if e.key() == Qt.Key_Slash:  # Activate completer when "/" is pressed
-                self.__initPromptCommandAutocomplete()
-                cr = self.cursorRect()
-                cr.setWidth(self.__completer.popup().sizeHintForColumn(
-                    0) + self.__completer.popup().verticalScrollBar().sizeHint().width())
-                self.__completer.complete(cr)
-            else:
-                self.__completer.popup().hide()
+        if self.__commandSuggestionEnabled:
+            if e.key() == Qt.Key_Up:
+                self.sendSuggestionWidget.emit('up')
+            elif e.key() == Qt.Key_Down:
+                self.sendSuggestionWidget.emit('down')
 
         if e.key() == Qt.Key_Return or e.key() == Qt.Key_Enter:
             if e.modifiers() == Qt.ShiftModifier:
                 return super().keyPressEvent(e)
             else:
-                self.returnPressed.emit()
+                if self.__commandSuggestionEnabled:
+                    self.sendSuggestionWidget.emit('enter')
+                else:
+                    self.returnPressed.emit()
         else:
             return super().keyPressEvent(e)
 
 
 class TextEditPropmtGroup(QWidget):
     textChanged = Signal()
+    onUpdateSuggestion = Signal()
+    onSendKeySignalToSuggestion = Signal(str)
 
     def __init__(self, db: SqliteDatabase):
         super().__init__()
         self.__initVal(db)
         self.__initUi()
 
     def __initVal(self, db):
         self.__db = db
 
     def __initUi(self):
-        self.__beginningTextEdit = TextEditPrompt(self.__db)
-        self.__beginningTextEdit.textChanged.connect(self.textChanged)
+        self.__beginningTextEdit = TextEditPrompt()
         self.__beginningTextEdit.setPlaceholderText('Beginning')
 
-        self.__textEdit = TextEditPrompt(self.__db)
-        self.__textEdit.textChanged.connect(self.textChanged)
+        self.__textEdit = TextEditPrompt()
         self.__textEdit.setPlaceholderText('Write some text...')
 
-        self.__endingTextEdit = TextEditPrompt(self.__db)
-        self.__endingTextEdit.textChanged.connect(self.textChanged)
+        # old code
+        # self.__textEdit.textChanged.connect(self.textChanged)
+        # self.__textEdit.sendSuggestionWidget.connect(self.__initPromptCommandAutocomplete)
+        # self.__textEdit.setPlaceholderText('Write some text...')
+
+        self.__endingTextEdit = TextEditPrompt()
         self.__endingTextEdit.setPlaceholderText('Ending')
 
+        # all false by default
         self.__beginningTextEdit.setVisible(False)
         self.__endingTextEdit.setVisible(False)
 
         self.__textGroup = [self.__beginningTextEdit, self.__textEdit, self.__endingTextEdit]
+        for w in self.__textGroup:
+            w.textChanged.connect(self.onUpdateSuggestion)
+            w.textChanged.connect(self.textChanged)
+            w.sendSuggestionWidget.connect(self.onSendKeySignalToSuggestion)
 
         lay = QVBoxLayout()
         for w in self.__textGroup:
             lay.addWidget(w)
         lay.setContentsMargins(0, 0, 0, 0)
         lay.setSpacing(0)
 
         self.setLayout(lay)
 
+    def executeCommand(self, item, grp):
+        command_key = item.text()
+        command = ''
+        for i in range(len(grp)):
+            if grp[i].get('name', '') == command_key:
+                command = grp[i].get('value', '')
+
+        w = self.getCurrentTextEdit()
+        if w:
+            cursor = w.textCursor()
+            cursor.deletePreviousChar()
+            cursor.select(QTextCursor.WordUnderCursor)
+            w.setTextCursor(cursor)
+            w.insertPlainText(command)
+
+            self.adjustHeight()
+
+    def getCurrentTextEdit(self):
+        for w in self.__textGroup:
+            if w.hasFocus():
+                return w
+
     def setCommandEnabled(self, f: bool):
         for w in self.__textGroup:
-            w.setPromptCommandAutocompletedEnabled(f)
+            w.setCommandSuggestionEnabled(f)
 
     def adjustHeight(self) -> int:
         """
         adjust overall height of text edit group based on their contents and return adjusted height
         :return:
         """
         groupHeight = 0
@@ -307,18 +290,43 @@
         super().__init__()
         self.__initVal(db)
         self.__initUi()
 
     def __initVal(self, db):
         self.__db = db
 
+        # prompt group
+        self.__p_grp = []
+
+        # False by default
+        self.__commandEnabled = False
+
     def __initUi(self):
+        # Create the command suggestion list
+        self.__suggestionWidget = CommandSuggestionWidget()
+        self.__suggestion_list = self.__suggestionWidget.getCommandList()
+
         self.__textEditGroup = TextEditPropmtGroup(self.__db)
         self.__textEditGroup.textChanged.connect(self.updateHeight)
 
+        # set command suggestion
+        self.__textEditGroup.onUpdateSuggestion.connect(self.__updateSuggestions)
+        self.__textEditGroup.onSendKeySignalToSuggestion.connect(self.__sendKeysignalToSuggestion)
+        
+        self.__suggestion_list.itemClicked.connect(self.executeCommand)
+
+        lay = QVBoxLayout()
+        lay.addWidget(self.__suggestionWidget)
+        lay.addWidget(self.__textEditGroup)
+        lay.setContentsMargins(0, 0, 0, 0)
+        lay.setSpacing(0)
+
+        leftWidget = QWidget()
+        leftWidget.setLayout(lay)
+
         settingsBtn = SvgToolButton()
         settingsBtn.setIcon('ico/vertical_three_dots.svg')
         settingsBtn.setToolTip('Prompt Settings')
 
         # Create the menu
         menu = QMenu(self)
 
@@ -352,34 +360,107 @@
         lay.setContentsMargins(1, 1, 1, 1)
         lay.setAlignment(Qt.AlignBottom)
 
         rightWidget = QWidget()
         rightWidget.setLayout(lay)
 
         lay = QHBoxLayout()
-        lay.addWidget(self.__textEditGroup)
+        lay.addWidget(leftWidget)
         lay.addWidget(rightWidget)
         lay.setContentsMargins(0, 0, 0, 0)
         lay.setSpacing(0)
         self.setLayout(lay)
+
+        self.__suggestionWidget.setVisible(False)
+
         self.updateHeight()
 
+    def __getEveryPromptCommands(self):
+        # get prop group
+        p_grp = []
+        for group in self.__db.selectPropPromptGroup():
+            p_grp_attr = [attr for attr in self.__db.selectPropPromptAttribute(group[0])]
+            p_grp_value = ''
+            for attr_obj in p_grp_attr:
+                name = attr_obj[2]
+                value = attr_obj[3]
+                if value and value.strip():
+                    p_grp_value += f'{name}: {value}\n'
+            p_grp.append({'name': group[1], 'value': p_grp_value})
+
+        # get template group
+        t_grp = []
+        for group in self.__db.selectTemplatePromptGroup():
+            t_grp_attr = [attr for attr in self.__db.selectTemplatePromptUnit(group[0])]
+            t_grp_value = ''
+            for attr_obj in t_grp_attr:
+                name = attr_obj[2]
+                value = attr_obj[3]
+                t_grp.append({'name': f'{attr_obj[2]}({group[1]})', 'value': value})
+
+        self.__p_grp = p_grp+t_grp
+
+        # TODO will include value as well
+        return [command['name'] for command in self.__p_grp]
+
+    def __updateSuggestions(self):
+        w = self.__textEditGroup.getCurrentTextEdit()
+        if w and self.__commandEnabled:
+            input_text_chunk = w.toPlainText().split()
+            input_text_chunk_exists = len(input_text_chunk) > 0
+            self.__suggestionWidget.setVisible(input_text_chunk_exists)
+            if input_text_chunk_exists:
+                input_text_chunk = input_text_chunk[-1]
+                starts_with_f = input_text_chunk.startswith('/')
+                self.__suggestionWidget.setVisible(starts_with_f)
+                w.setCommandSuggestionEnabled(starts_with_f)
+                if starts_with_f:
+                    command_word = input_text_chunk[1:]
+
+                    # Example: Add some dummy command suggestions
+                    commands = self.__getEveryPromptCommands()
+                    filtered_commands = commands
+                    if command_word:
+                        filtered_commands = [command for command in commands if command_word.lower() in command.lower()]
+                    filtered_commands_exists_f = len(filtered_commands) > 0
+                    self.__suggestionWidget.setVisible(filtered_commands_exists_f)
+                    if filtered_commands_exists_f:
+                        # Clear previous suggestions
+                        self.__suggestion_list.clear()
+
+                        # Add the filtered suggestions to the list
+                        self.__suggestion_list.addItems(filtered_commands)
+                        self.__suggestion_list.setCurrentRow(0)
+
+    def __sendKeysignalToSuggestion(self, key):
+        if key == 'up':
+            self.__suggestion_list.setCurrentRow(max(0, self.__suggestion_list.currentRow() - 1))
+        elif key == 'down':
+            self.__suggestion_list.setCurrentRow(
+                min(self.__suggestion_list.currentRow() + 1, self.__suggestion_list.count() - 1))
+        elif key == 'enter':
+            self.executeCommand(self.__suggestion_list.currentItem())
+
+    def executeCommand(self, item):
+        self.__textEditGroup.executeCommand(item, self.__p_grp)
+
     def updateHeight(self):
         overallHeight = self.__textEditGroup.adjustHeight()
-        self.setMaximumHeight(overallHeight)
+        self.setMaximumHeight(overallHeight + self.__suggestionWidget.maximumHeight())
 
     def getTextEdit(self):
         return self.__textEditGroup.getGroup()[1]
 
     def getContent(self):
         return self.__textEditGroup.getContent()
 
     def __showBeginning(self, f):
         self.__textEditGroup.getGroup()[0].setVisible(f)
 
     def __showEnding(self, f):
         self.__textEditGroup.getGroup()[-1].setVisible(f)
 
     def __supportPromptCommand(self, f):
+        self.__commandEnabled = f
         self.__textEditGroup.setCommandEnabled(f)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/circleProfileImage.py` & `pyqt-openai-0.1.61/pyqt_openai/circleProfileImage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/convListWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/convListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/customizeDialog.py` & `pyqt-openai-0.1.61/pyqt_openai/customizeDialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,32 +136,36 @@
             self.__pathFindBtn.clicked.connect(self.__customFind)
 
     def __customFind(self):
         self.findClicked.emit()
 
     def __find(self):
         if self.isForDirectory():
-            dirname = QFileDialog.getExistingDirectory(None, 'Open Directory', '', QFileDialog.ShowDirsOnly)
-            if dirname:
-                self.__pathLineEdit.setText(dirname)
-                self.added.emit(dirname)
+            filename = QFileDialog.getExistingDirectory(self, 'Open Directory', '', QFileDialog.ShowDirsOnly)
+            if filename:
+                pass
+            else:
+                return
         else:
             str_exp_files_to_open = self.__ext_of_files if self.__ext_of_files else 'All Files (*.*)'
             filename = QFileDialog.getOpenFileName(self, 'Find', '', str_exp_files_to_open)
             if filename[0]:
                 filename = filename[0]
-                self.__pathLineEdit.setText(filename)
-                self.added.emit(filename)
+            else:
+                return
+        self.__pathLineEdit.setText(filename)
+        self.added.emit(filename)
 
     def setAsDirectory(self, f: bool):
         self.__directory = f
 
     def isForDirectory(self) -> bool:
         return self.__directory
 
+
 class CustomizeDialog(QDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__initVal()
         self.__initUi()
 
     def __initVal(self):
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/customize.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/customize.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/discord.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/discord.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/github.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/github.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/help.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/help.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/history.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/history.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/save.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/save.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/search.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/search.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/setting.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/stackontop.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/stackontop.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/ico/user.svg` & `pyqt-openai-0.1.61/pyqt_openai/ico/user.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/currentImageView.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/currentImageView.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/explorerWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/explorerWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageDallEPage.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageDallEPage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import openai
 
 from qtpy.QtWidgets import QWidget, QPushButton, QComboBox, QPlainTextEdit, QSpinBox, QFormLayout, QTextEdit, QLabel
 from qtpy.QtCore import Signal, QThread
 
 from pyqt_openai.notifier import NotifierWidget
+from pyqt_openai.toast import Toast
 
 
 class DallEThread(QThread):
     replyGenerated = Signal(str)
+    errorGenerated = Signal(str)
 
     def __init__(self, openai_arg, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__openai_arg = openai_arg
 
     def run(self):
-        response = openai.Image.create(
-            **self.__openai_arg
-        )
-
-        for image_data in response['data']:
-            image_url = image_data['url']
-            self.replyGenerated.emit(image_url)
+        try:
+            response = openai.Image.create(
+                **self.__openai_arg
+            )
+
+            for image_data in response['data']:
+                image_url = image_data['url']
+                self.replyGenerated.emit(image_url)
+        except Exception as e:
+            self.errorGenerated.emit(str(e))
 
 
 class ImageDallEPage(QWidget):
     submitDallE = Signal(str)
     notifierWidgetActivated = Signal()
     # class name: ImageDatabase
     # file name: imageDb
@@ -77,14 +82,20 @@
             "n": self.__nSpinBox.value(),
             "size": self.__sizeCmbBox.currentText()
         }
         self.__t = DallEThread(openai_arg)
         self.__submitBtn.setEnabled(False)
         self.__t.start()
         self.__t.replyGenerated.connect(self.__afterGenerated)
+        self.__t.errorGenerated.connect(self.__failToGenerate)
+
+    def __failToGenerate(self, e):
+        toast = Toast(text=e, duration=3, parent=self)
+        toast.show()
+        self.__submitBtn.setEnabled(True)
 
     def __afterGenerated(self, image_url):
         self.submitDallE.emit(image_url)
         if not self.isVisible():
             self.__notifierWidget = NotifierWidget(informative_text='Response 👌', detailed_text='Click this!')
             self.__notifierWidget.show()
             self.__notifierWidget.doubleClicked.connect(self.notifierWidgetActivated)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,15 @@
     def showAiToolBar(self, f):
         self.__menuWidget.setVisible(f)
 
     def setAIEnabled(self, f):
         self.__rightSideBarWidget.setEnabled(f)
 
     def __addImageGroup(self):
-        self.__db.insertConv('New Chat')
-        cur_id = self.__db.getCursor().lastrowid
+        cur_id = self.__db.insertConv('New Chat')
         self.__browser.resetChatWidget(cur_id)
         self.__leftSideBarWidget.addImageGroup(cur_id)
         self.__lineEdit.setFocus()
         print('addImageGroup')
 
     def __deleteImageGroup(self):
         print('deleteImageGroup')
@@ -118,15 +117,8 @@
         if isinstance(arg, str):
             self.__viewWidget.showDallEResult(arg)
             # TODO
             # self.__leftSideBarWidget.addImageGroup('DALL-E', 'New Image Group', 0)
         # SD
         elif isinstance(arg, bytes):
             self.__viewWidget.showSdResult(arg)
-            # self.__leftSideBarWidget.addImageGroup('Stable Diffusion', 'New Image Group', 0)
-
-
-if __name__ == "__main__":
-    app = QApplication(sys.argv)
-    w = ImageGeneratingToolWidget()
-    w.show()
-    sys.exit(app.exec_())
+            # self.__leftSideBarWidget.addImageGroup('Stable Diffusion', 'New Image Group', 0)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageListWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageSqlite.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageSqlite.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,41 @@
 from qtpy.QtCore import Signal, QThread, QSettings
 from qtpy.QtWidgets import QWidget, QLineEdit, QVBoxLayout, QHBoxLayout, QGroupBox, QPushButton, QFormLayout, QSpinBox, QComboBox, \
     QLabel, QPlainTextEdit
 from stability_sdk import client
 
 from pyqt_openai.notifier import NotifierWidget
 from pyqt_openai.svgLabel import SvgLabel
+from pyqt_openai.toast import Toast
 
 # Our Host URL should not be prepended with "https" nor should it have a trailing slash.
 os.environ['STABILITY_HOST'] = 'grpc.stability.ai:443'
 
 
 class StableDiffusionThread(QThread):
     replyGenerated = Signal(bytes)
+    errorGenerated = Signal(str)
 
     def __init__(self, answers, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__answers = answers
 
     def run(self):
-        for resp in self.__answers:
-            for artifact in resp.artifacts:
-                if artifact.finish_reason == generation.FILTER:
-                    warnings.warn(
-                        "Your request activated the API's safety filters and could not be processed."
-                        "Please modify the prompt and try again.")
-                if artifact.type == generation.ARTIFACT_IMAGE:
-                    self.replyGenerated.emit(artifact.binary)
+        try:
+            for resp in self.__answers:
+                for artifact in resp.artifacts:
+                    if artifact.finish_reason == generation.FILTER:
+                        warnings.warn(
+                            "Your request activated the API's safety filters and could not be processed."
+                            "Please modify the prompt and try again.")
+                    if artifact.type == generation.ARTIFACT_IMAGE:
+                        self.replyGenerated.emit(artifact.binary)
+        except Exception as e:
+            self.errorGenerated.emit(str(e))
+
 
 
 class ImageStableDiffusionPage(QWidget):
     submitSd = Signal(bytes)
     notifierWidgetActivated = Signal()
 
     def __init__(self):
@@ -221,14 +227,20 @@
             # (Available Samplers: ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2, k_dpm_2_ancestral, k_dpmpp_2s_ancestral, k_lms, k_dpmpp_2m, k_dpmpp_sde)
         )
 
         self.__t = StableDiffusionThread(answers)
         self.__submitBtn.setEnabled(False)
         self.__t.start()
         self.__t.replyGenerated.connect(self.__afterGenerated)
+        self.__t.errorGenerated.connect(self.__failToGenerate)
+
+    def __failToGenerate(self, e):
+        toast = Toast(text=e, duration=3, parent=self)
+        toast.show()
+        self.__submitBtn.setEnabled(True)
 
     def __afterGenerated(self, image_bin):
         self.submitSd.emit(image_bin)
         if not self.isVisible():
             self.__notifierWidget = NotifierWidget(informative_text='Response 👌', detailed_text='Click this!')
             self.__notifierWidget.show()
             self.__notifierWidget.doubleClicked.connect(self.notifierWidgetActivated)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/leftSideBar.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/leftSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/rightSideBar.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/rightSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/thumbnailView.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/thumbnailView.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/image_gen_widget/viewWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/viewWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/inputDialog.py` & `pyqt-openai-0.1.61/pyqt_openai/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/leftSideBar.py` & `pyqt-openai-0.1.61/pyqt_openai/leftSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/main.py` & `pyqt-openai-0.1.61/pyqt_openai/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,35 @@
-import os
+import os, sys
 import openai, requests
 
+# Get the absolute path of the current script file
+script_path = os.path.abspath(__file__)
+
+# Get the root directory by going up one level from the script directory
+project_root = os.path.dirname(os.path.dirname(script_path))
+
+sys.path.insert(0, project_root)
+sys.path.insert(0, os.getcwd())  # Add the current directory as well
+
 from qtpy.QtGui import QGuiApplication, QFont, QIcon, QColor
 from qtpy.QtWidgets import QMainWindow, QToolBar, QHBoxLayout, QDialog, QLineEdit, QPushButton, QWidgetAction, QSpinBox, QLabel, QWidget, QApplication, \
     QComboBox, QSizePolicy, QStackedWidget, QAction, QMenu, QSystemTrayIcon, \
     QMessageBox, QCheckBox
 from qtpy.QtCore import Qt, QCoreApplication, QSettings
 
 from pyqt_openai.aboutDialog import AboutDialog
 from pyqt_openai.customizeDialog import CustomizeDialog
 from pyqt_openai.svgButton import SvgButton
 from pyqt_openai.image_gen_widget.imageGeneratingToolWidget import ImageGeneratingToolWidget
 from pyqt_openai.openAiChatBotWidget import OpenAIChatBotWidget
 
+# for testing pyside6
+# if you use pyside6 already, you don't have to remove the #
+# os.environ['QT_API'] = 'pyside6'
+
 QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
 QCoreApplication.setAttribute(Qt.AA_UseHighDpiPixmaps)  # HighDPI support
 # qt version should be above 5.14
 # todo check the qt version with qtpy
 if os.environ['QT_API'] == 'pyqt5' or os.environ['QT_API'] != 'pyside6':
     QGuiApplication.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
 
@@ -171,24 +184,24 @@
         tray_icon.activated.connect(self.__activated)
 
         tray_icon.setContextMenu(menu)
 
         tray_icon.show()
 
     def __activated(self, reason):
-        if reason == 3:
+        if reason == QSystemTrayIcon.DoubleClick:
             self.show()
 
     def __setToolBar(self):
         aiTypeToolBar = QToolBar()
         aiTypeToolBar.setMovable(False)
         aiTypeToolBar.addAction(self.__chooseAiAction)
 
         windowToolBar = QToolBar()
-        lay = QHBoxLayout()
+        lay = windowToolBar.layout()
         windowToolBar.addAction(self.__stackAction)
         windowToolBar.addAction(self.__customizeAction)
         windowToolBar.addAction(self.__transparentAction)
         windowToolBar.addAction(self.__showAiToolBarAction)
         windowToolBar.addAction(self.__apiAction)
         windowToolBar.setLayout(lay)
         windowToolBar.setMovable(False)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/modelTable.py` & `pyqt-openai-0.1.61/pyqt_openai/modelTable.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/notifier.py` & `pyqt-openai-0.1.61/pyqt_openai/notifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from qtpy import QtGui
+from qtpy.QtCore import Qt, QPoint, Signal, QTimer, QPropertyAnimation
 from qtpy.QtGui import QFont, QIcon
-from qtpy.QtWidgets import QWidget, QLabel, QHBoxLayout, QVBoxLayout, QDesktopWidget, QSizePolicy, qApp, QPushButton, \
+from qtpy.QtWidgets import QWidget, QLabel, QHBoxLayout, QVBoxLayout, QSizePolicy, QPushButton, \
     QApplication
-from qtpy.QtCore import Qt, QPoint, Signal, QTimer, QPropertyAnimation
 
 
 class NotifierWidget(QWidget):
     doubleClicked = Signal()
 
     def __init__(self, informative_text='', detailed_text=''):
         super().__init__()
@@ -41,15 +42,15 @@
         lay = QVBoxLayout()
         lay.addWidget(customMenuBar)
         lay.addWidget(self.__informativeTextLabel)
         lay.addWidget(self.__detailedTextLabel)
         lay.addWidget(self.__btnWidget)
         lay.setContentsMargins(0, 0, 0, 0)
 
-        ag = QDesktopWidget().availableGeometry()
+        ag = QtGui.QGuiApplication.primaryScreen().availableGeometry()
 
         geo = self.geometry()
         geo.moveBottomRight(QPoint(ag.width(), ag.height()))
         self.setGeometry(geo)
 
         lay.setContentsMargins(8, 8, 8, 8)
         self.setLayout(lay)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/openAiChatBotWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/openAiChatBotWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     QListWidgetItem, QFileDialog
 
 from pyqt_openai.apiData import ModelData
 from pyqt_openai.chatWidget import Prompt, ChatBrowser
 from pyqt_openai.leftSideBar import LeftSideBar
 from pyqt_openai.notifier import NotifierWidget
 from pyqt_openai.openAiThread import OpenAIThread
-from pyqt_openai.prompt.promptGeneratorWidget import PromptGeneratorWidget
+from pyqt_openai.prompt_gen_widget.promptGeneratorWidget import PromptGeneratorWidget
 from pyqt_openai.right_sidebar.aiPlaygroundWidget import AIPlaygroundWidget
 from pyqt_openai.sqlite import SqliteDatabase
 from pyqt_openai.svgButton import SvgButton
 
 
 class OpenAIChatBotWidget(QWidget):
     notifierWidgetActivated = Signal()
@@ -263,16 +263,15 @@
             conv = self.__db.selectConvUnit(id)
             self.__browser.replaceConv(id, conv)
         else:
             self.__browser.resetChatWidget(0)
 
 
     def __addConv(self):
-        self.__db.insertConv('New Chat')
-        cur_id = self.__db.getCursor().lastrowid
+        cur_id = self.__db.insertConv('New Chat')
         self.__browser.resetChatWidget(cur_id)
         self.__leftSideBarWidget.addToList(cur_id)
         self.__lineEdit.setFocus()
 
     def __updateConv(self, id, title=None):
         if title:
             self.__db.updateConv(id, title)
@@ -285,11 +284,10 @@
 
     def __export(self, ids):
         filename = QFileDialog.getSaveFileName(self, 'Save', os.path.expanduser('~'), 'SQLite DB file (*.db)')
         if filename[0]:
             filename = filename[0]
             self.__db.export(ids, filename)
 
-
     def __updateConvUnit(self, id, user_f, conv_unit=None):
         if conv_unit:
             self.__db.insertConvUnit(id, user_f, conv_unit)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/openAiThread.py` & `pyqt-openai-0.1.61/pyqt_openai/openAiThread.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/prompt/promptGeneratorWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pyperclip
-from qtpy.QtWidgets import QTextBrowser, QWidget, QLabel, QVBoxLayout, QPushButton, QTabWidget, QScrollArea
 
-from pyqt_openai.prompt.propPage import PropPage
-from pyqt_openai.prompt.templatePage import TemplatePage
+from qtpy.QtWidgets import QTextBrowser, QSplitter, QWidget, QLabel, QVBoxLayout, QPushButton, QTabWidget, QScrollArea
+from qtpy.QtCore import Qt
+
+from pyqt_openai.prompt_gen_widget.propPage import PropPage
+from pyqt_openai.prompt_gen_widget.templatePage import TemplatePage
 from pyqt_openai.sqlite import SqliteDatabase
 
 
 class PromptGeneratorWidget(QScrollArea):
     def __init__(self, db: SqliteDatabase):
         super().__init__()
         self.__initVal(db)
@@ -35,22 +37,42 @@
 
         copyBtn = QPushButton('Copy')
         copyBtn.clicked.connect(self.__copy)
 
         lay = QVBoxLayout()
         lay.addWidget(propmtLbl)
         lay.addWidget(promptTabWidget)
+
+        topWidget = QWidget()
+        topWidget.setLayout(lay)
+
+        lay = QVBoxLayout()
         lay.addWidget(previewLbl)
         lay.addWidget(self.__prompt)
         lay.addWidget(copyBtn)
 
-        mainWidget = QWidget()
-        mainWidget.setLayout(lay)
+        bottomWidget = QWidget()
+        bottomWidget.setLayout(lay)
+
+        mainSplitter = QSplitter()
+        mainSplitter.addWidget(topWidget)
+        mainSplitter.addWidget(bottomWidget)
+        mainSplitter.setOrientation(Qt.Vertical)
+        mainSplitter.setChildrenCollapsible(False)
+        mainSplitter.setHandleWidth(2)
+        mainSplitter.setStyleSheet(
+            '''
+            QSplitter::handle:vertical
+            {
+                background: #CCC;
+                height: 1px;
+            }
+            ''')
 
-        self.setWidget(mainWidget)
+        self.setWidget(mainSplitter)
         self.setWidgetResizable(True)
 
         self.setStyleSheet('QScrollArea { border: 0 }')
 
     def __textChanged(self, prompt_text):
         self.__prompt.clear()
         self.__prompt.setText(prompt_text)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/prompt/propPage.py` & `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from qtpy.QtCore import Signal, Qt, QEvent
 from qtpy.QtWidgets import QTableWidget, QLineEdit, QSizePolicy, QSpacerItem, QStackedWidget, QLabel, \
     QAbstractItemView, QTableWidgetItem, QHeaderView, QHBoxLayout, \
     QVBoxLayout, QWidget, QDialog, QListWidget, QListWidgetItem, QSplitter
 
 from pyqt_openai.inputDialog import InputDialog
+from pyqt_openai.prompt_gen_widget.promptGroupInputDialog import PromptGroupInputDialog
+from pyqt_openai.prompt_gen_widget.propPromptUnitInputDialog import PropPromptUnitInputDialog
 from pyqt_openai.sqlite import SqliteDatabase
 from pyqt_openai.svgButton import SvgButton
 
 
 class PropGroupList(QWidget):
     added = Signal(int)
     deleted = Signal(int)
@@ -70,18 +72,18 @@
         item.setData(Qt.UserRole, id)
         item.setText(name)
         self.__propList.addItem(item)
         self.__propList.setCurrentItem(item)
         self.added.emit(id)
 
     def __addGroup(self):
-        dialog = InputDialog('Add', '', self)
+        dialog = PromptGroupInputDialog(self.__db, self)
         reply = dialog.exec()
         if reply == QDialog.Accepted:
-            name = dialog.getText()
+            name = dialog.getPromptGroupName()
             id = self.__db.insertPropPromptGroup(name)
             self.__addGroupItem(id, name)
 
     def __deleteGroup(self):
         i = self.__propList.currentRow()
         item = self.__propList.takeItem(i)
         id = item.data(Qt.UserRole)
@@ -180,20 +182,20 @@
         name = self.__table.item(item.row(), 0)
         id = name.data(Qt.UserRole)
         name = name.text()
         value = self.__table.item(item.row(), 1).text()
         self.__db.updatePropPromptAttribute(self.__id, id, name, value)
 
     def __add(self):
-        dialog = InputDialog('Name', '', self)
+        dialog = PropPromptUnitInputDialog(self.__db, self.__id, self)
         reply = dialog.exec()
         if reply == QDialog.Accepted:
             self.__table.itemChanged.disconnect(self.__saveChangedPropPrompt)
 
-            name = dialog.getText()
+            name = dialog.getPromptName()
             self.__table.setRowCount(self.__table.rowCount()+1)
 
             item1 = QTableWidgetItem(name)
             item1.setTextAlignment(Qt.AlignCenter)
             self.__table.setItem(self.__table.rowCount()-1, 0, item1)
 
             item2 = QTableWidgetItem('')
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/right_sidebar/aiPlaygroundWidget.py` & `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/aiPlaygroundWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/right_sidebar/chatPage.py` & `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/chatPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/right_sidebar/completionPage.py` & `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/completionPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/right_sidebar/imagePage.py` & `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/imagePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/searchBar.py` & `pyqt-openai-0.1.61/pyqt_openai/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/svgButton.py` & `pyqt-openai-0.1.61/pyqt_openai/svgButton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os.path, posixpath
 
 from qtpy.QtGui import QColor, QPalette, qGray
-from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QPushButton
+from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, QApplication, QPushButton
 
 
 class SvgButton(QPushButton):
     def __init__(self, base_widget: QWidget = None, parent=None):
         super().__init__(parent)
         self.__baseWidget = base_widget
         self.__initVal()
         self.__styleInit()
 
     def __initVal(self):
         # to set size accordance with scale
-        sc = qApp.screens()[0]
+        sc = QApplication.screens()[0]
         sc.logicalDotsPerInchChanged.connect(self.__scaleChanged)
         self.__size = sc.logicalDotsPerInch() // 4
         self.__padding = self.__border_radius = self.__size // 10
         self.__background_color = 'transparent'
         self.__icon = ''
         self.__animation = ''
         self.installEventFilter(self)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/svgLabel.py` & `pyqt-openai-0.1.61/pyqt_openai/svgLabel.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 class SvgLabel(QLabel):
     def __init__(self):
         super().__init__()
         self.__renderer = ''
 
     def paintEvent(self, e):
         painter = QPainter(self)
-        painter.restore()
         if self.__renderer:
             self.__renderer.render(painter)
         return super().paintEvent(e)
 
     def setSvgFile(self, filename: str):
         filename = os.path.join(os.path.dirname(__file__), filename)
         self.__renderer = QSvgRenderer(filename)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/svgToolButton.py` & `pyqt-openai-0.1.61/pyqt_openai/svgToolButton.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os.path, posixpath
 
 from qtpy.QtGui import QColor, QPalette, qGray
-from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, qApp, QToolButton
+from qtpy.QtWidgets import QGraphicsColorizeEffect, QWidget, QApplication, QToolButton
 
 
 class SvgToolButton(QToolButton):
     def __init__(self, base_widget: QWidget = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__baseWidget = base_widget
         self.__initVal()
         self.__styleInit()
 
     def __initVal(self):
         # to set size accordance with scale
-        sc = qApp.screens()[0]
+        sc = QApplication.screens()[0]
         sc.logicalDotsPerInchChanged.connect(self.__scaleChanged)
         self.__size = sc.logicalDotsPerInch() // 4
         self.__padding = self.__border_radius = self.__size // 10
         self.__background_color = 'transparent'
         self.__icon = ''
         self.__animation = ''
         self.installEventFilter(self)
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai/test/htmlformat.py` & `pyqt-openai-0.1.61/pyqt_openai/test/htmlformat.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai/test/sqlalchemy_example.py` & `pyqt-openai-0.1.61/pyqt_openai/test/sqlalchemy_example.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.51/pyqt_openai.egg-info/PKG-INFO` & `pyqt-openai-0.1.61/pyqt_openai.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.51
+Version: 0.1.61
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,64 +55,124 @@
   * AI remembers past conversation
 * conversation management
   * add & delete conversations
   * save conversations
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable, autosaved in database)
+* support prompt generator (manageable, autosaved in database) 
 * support slash commands
 * support beginning and ending part of the prompt
 * you can run this in background application
   * notification will pop up when response is generated
 * you can make window stack on top or control its transparency
 * image generation (DALL-E, Stable Diffusion with DreamStudio API)
 * you can copy and download the image if you want. just hover the mouse cursor over the image.
 
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
-* pyperclip - to copy prompt template from prompt generator
+* aiohttp - for openai dependency 
+* pyperclip - to copy prompt text from prompt generator
 * stability_sdk - for Stable Diffusion
 
 ## Preview & Usage
 ### Overview
-#### Note: Some of these previews are not the latest.
+#### Windows
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
 <b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
 
 You can change screen between text chatbot and image generating tool screen.
+
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061)
 
+#### Linux (Ubuntu)
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba)
+
+If you use MacOS, please give me the pyqt-openai screen image from it.
+
 ### Conversation
+#### Preview 1
+I recorded this preview long time ago so GUI is different from the current version, but way of operating it is pretty much the same.
+
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
+#### Preview 2 (using prompt feature)
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead
 
 ### Prompt Generator
-https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-1e8c-4ba2-b5fe-4391df6250ff
+#### How to Generate
+This application has two types of prompts. One is <b>"Properties"</b> and the other one is <b>"Template"</b>. Properties are sets of attributes that are useful for forming the premises of a question. Templates are sentences that correspond to a single command. You can input a command to generate a sentence. This can be used as a question in itself.
+
+Both types can be managed as groups. After cloning or installing, if you run the program immediately, you will be able to see the default group and the items included in the group, just like the screen.
+
+For properties, there is a group named "Default" that provides a set of attributes referenced <a href="https://gptforwork.com/tools/prompt-generator">here</a>.
 
-You can use the additional prompt feature by "prompt menu" right next to input field.
+For templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example prompt for Alex Brogan) groups provided. Any custom template items created prior to version 0.1.6 will be moved to the Miscellaneous group.
+
+![prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/ce40139a-c03f-42ef-abd8-4a610d762394)
+
+With using these prompts you can pretty much get any response you want.
+
+You can use the additional prompt feature by "prompt menu" right next to "prompt input" field.
 
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
 
+Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
+
+#### Prompt Generator Preview
+Generating the prompt (Properties)
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-3c42c9c23602
+
+I recorded using the Windows recording feature. As a result, the "Add Dialog" that prompts for entering a group name does not appear in the preview. When you add a group, you will see the Add Dialog as expected.
+
+Then, how to generate template type prompt? Click any item in the group, it will be shown in the preview.
+
+You can copy that generated text with clicking "copy" button and include it to your prompt input.
+
+If you add a property group or template group with items, you can use it as a command by typing its name to the prompt input.
+
+<b>Use prompt as a command</b>
+
+https://github.com/yjg30737/pyqt-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553
+
+In this preview, i pressed the keyboard shortcut of each actions(show beginning, show ending, support prompt command) to use it rather than clicking them with mouse.
+
+I made the command suggestion GUI resemble the Discord command autocomplete popup, with which a lot of people have become accustomed.
+
 ### Image Generation
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
 
 ## How to Install
-1. open command propmt of your OS.
-2. git clone ~
-3. from the root directory, type "cd pyqt_openai"
-4. pip install -r requirements.txt
+1. git clone ~
+2. cd pyqt-openai
+3. pip install -r requirements.txt
+4. cd pyqt_openai
 5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
 6. python main.py
 
-If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error. 
+If installation doesn't work, you can contact me with bring up new issue in issue tab or check the troubleshooting below even it is only about very specific error.
+
+### Note
+If you use Linux and see this error:
+```
+qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it was found
+
+this application failed to start because no qt platform plugin could be initialized, reinstalling the application may fix this problem
+```
+
+run this command:
+```
+sudo apt-get install libxcb-xinerama0
+```
 
 ## Troubleshooting
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
 download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.51 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.61 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
@@ -29,48 +29,87 @@
 * support prompt generator (manageable, autosaved in database) * support slash
 commands * support beginning and ending part of the prompt * you can run this
 in background application * notification will pop up when response is generated
 * you can make window stack on top or control its transparency * image
 generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
 download the image if you want. just hover the mouse cursor over the image. ##
 Requirements * qtpy - the package allowing you to write code that works with
-both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * pyperclip - to copy
-prompt template from prompt generator * stability_sdk - for Stable Diffusion ##
-Preview & Usage ### Overview #### Note: Some of these previews are not the
-latest. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * aiohttp - for openai
+dependency * pyperclip - to copy prompt text from prompt generator *
+stability_sdk - for Stable Diffusion ## Preview & Usage ### Overview ####
+Windows ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
 51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
 inside the red box. see [How to install](#how-to-install) You can change screen
 between text chatbot and image generating tool screen. ![image](https://
 github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
-07655cab2061) ### Conversation https://user-images.githubusercontent.com/
-55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4 ### Prompt
-Generator https://github.com/yjg30737/pyqt-openai/assets/55078043/2f351442-
-1e8c-4ba2-b5fe-4391df6250ff You can use the additional prompt feature by
-"prompt menu" right next to input field. ![image](https://github.com/yjg30737/
-pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663) ### Image
-Generation ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install 1. open command propmt
-of your OS. 2. git clone ~ 3. from the root directory, type "cd pyqt_openai" 4.
-pip install -r requirements.txt 5. You should put your api key in the line
-edit. You can get it in official_site of openai. Sign up and log in before you
-get it. Be sure, this is a very important API key that belongs to you only, so
-you should remember it and keep it secure. 6. python main.py If installation
-doesn't work, you can contact me with bring up new issue in issue tab or check
-the troubleshooting below even it is only about very specific error. ##
-Troubleshooting If you see this error while installing the openai package ```
-subprocess-exited-with-error ``` download the package itself from pypi. Unzip
-it, access the package directory, type ``` python setup.py install ``` That
-will install the openai. Note: I don't know this can happen in newer version of
-openai as well, so tell me if you know about something ## Contact You can join
-pyqt-openai's Discord_Server to have a conversation about it or AI-related
-stuff ð ## Note I recommend to install sqlite management software. It's not
-necessary to run this app (obviously), but it's good practice to manage
-database about conversation history with AI and to know how this works. ## TODO
-list * DB for images (to further experiement of both DALL-E and Stable
-Diffusion or other image generation engine) * show the explanation of every
-model and terms related to AI (e.g. temperature, topp..) * save conversation
-history with other format (xlsx, csv, etc.) * tokenizer * highlight the source
-(optional, eventually) * support multiple language * use SQLAlchemy (maybe not)
-* show reason when the chat input is disabled for some reasons * add the basic
-example sources of making deep learning model with PyTorch (eventually) ## See
-Also * Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access
-from it * join_chatgpt_plugins_waitlist
+07655cab2061) #### Linux (Ubuntu) ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS,
+please give me the pyqt-openai screen image from it. ### Conversation ####
+Preview 1 I recorded this preview long time ago so GUI is different from the
+current version, but way of operating it is pretty much the same. https://user-
+images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-
+f60d8b2d6ced.mp4 #### Preview 2 (using prompt feature) https://github.com/
+yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ###
+Prompt Generator #### How to Generate This application has two types of
+prompts. One is "Properties" and the other one is "Template". Properties are
+sets of attributes that are useful for forming the premises of a question.
+Templates are sentences that correspond to a single command. You can input a
+command to generate a sentence. This can be used as a question in itself. Both
+types can be managed as groups. After cloning or installing, if you run the
+program immediately, you will be able to see the default group and the items
+included in the group, just like the screen. For properties, there is a group
+named "Default" that provides a set of attributes referenced here. For
+templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example
+prompt for Alex Brogan) groups provided. Any custom template items created
+prior to version 0.1.6 will be moved to the Miscellaneous group. !
+[prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+ce40139a-c03f-42ef-abd8-4a610d762394) With using these prompts you can pretty
+much get any response you want. You can use the additional prompt feature by
+"prompt menu" right next to "prompt input" field. ![image](https://github.com/
+yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
+Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
+#### Prompt Generator Preview Generating the prompt (Properties) https://
+github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-
+3c42c9c23602 I recorded using the Windows recording feature. As a result, the
+"Add Dialog" that prompts for entering a group name does not appear in the
+preview. When you add a group, you will see the Add Dialog as expected. Then,
+how to generate template type prompt? Click any item in the group, it will be
+shown in the preview. You can copy that generated text with clicking "copy"
+button and include it to your prompt input. If you add a property group or
+template group with items, you can use it as a command by typing its name to
+the prompt input. Use prompt as a command https://github.com/yjg30737/pyqt-
+openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553 In this preview, i
+pressed the keyboard shortcut of each actions(show beginning, show ending,
+support prompt command) to use it rather than clicking them with mouse. I made
+the command suggestion GUI resemble the Discord command autocomplete popup,
+with which a lot of people have become accustomed. ### Image Generation !
+[image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-
+4900-bfea-89da6f072c9d) ## How to Install 1. git clone ~ 2. cd pyqt-openai 3.
+pip install -r requirements.txt 4. cd pyqt_openai 5. You should put your api
+key in the line edit. You can get it in official_site of openai. Sign up and
+log in before you get it. Be sure, this is a very important API key that
+belongs to you only, so you should remember it and keep it secure. 6. python
+main.py If installation doesn't work, you can contact me with bring up new
+issue in issue tab or check the troubleshooting below even it is only about
+very specific error. ### Note If you use Linux and see this error: ```
+qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it
+was found this application failed to start because no qt platform plugin could
+be initialized, reinstalling the application may fix this problem ``` run this
+command: ``` sudo apt-get install libxcb-xinerama0 ``` ## Troubleshooting If
+you see this error while installing the openai package ``` subprocess-exited-
+with-error ``` download the package itself from pypi. Unzip it, access the
+package directory, type ``` python setup.py install ``` That will install the
+openai. Note: I don't know this can happen in newer version of openai as well,
+so tell me if you know about something ## Contact You can join pyqt-openai's
+Discord_Server to have a conversation about it or AI-related stuff ð ## Note
+I recommend to install sqlite management software. It's not necessary to run
+this app (obviously), but it's good practice to manage database about
+conversation history with AI and to know how this works. ## TODO list * DB for
+images (to further experiement of both DALL-E and Stable Diffusion or other
+image generation engine) * show the explanation of every model and terms
+related to AI (e.g. temperature, topp..) * save conversation history with other
+format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
+eventually) * support multiple language * use SQLAlchemy (maybe not) * show
+reason when the chat input is disabled for some reasons * add the basic example
+sources of making deep learning model with PyTorch (eventually) ## See Also *
+Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
+it * join_chatgpt_plugins_waitlist
```

### Comparing `pyqt-openai-0.1.51/pyqt_openai.egg-info/SOURCES.txt` & `pyqt-openai-0.1.61/pyqt_openai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 setup.py
 pyqt_openai/__init__.py
 pyqt_openai/a.py
 pyqt_openai/aboutDialog.py
 pyqt_openai/apiData.py
 pyqt_openai/chatWidget.py
 pyqt_openai/circleProfileImage.py
+pyqt_openai/commandCompleter.py
 pyqt_openai/convListWidget.py
 pyqt_openai/customizeDialog.py
 pyqt_openai/inputDialog.py
 pyqt_openai/leftSideBar.py
 pyqt_openai/main.py
 pyqt_openai/modelTable.py
 pyqt_openai/notifier.py
 pyqt_openai/openAiChatBotWidget.py
 pyqt_openai/openAiThread.py
 pyqt_openai/searchBar.py
 pyqt_openai/sqlite.py
 pyqt_openai/svgButton.py
 pyqt_openai/svgLabel.py
 pyqt_openai/svgToolButton.py
+pyqt_openai/toast.py
 pyqt_openai.egg-info/PKG-INFO
 pyqt_openai.egg-info/SOURCES.txt
 pyqt_openai.egg-info/dependency_links.txt
 pyqt_openai.egg-info/requires.txt
 pyqt_openai.egg-info/top_level.txt
 pyqt_openai/ico/__init__.py
 pyqt_openai/ico/add.svg
@@ -52,26 +54,24 @@
 pyqt_openai/image_gen_widget/imageListWidget.py
 pyqt_openai/image_gen_widget/imageSqlite.py
 pyqt_openai/image_gen_widget/imageStableDiffusionPage.py
 pyqt_openai/image_gen_widget/leftSideBar.py
 pyqt_openai/image_gen_widget/rightSideBar.py
 pyqt_openai/image_gen_widget/thumbnailView.py
 pyqt_openai/image_gen_widget/viewWidget.py
-pyqt_openai/prompt/__init__.py
-pyqt_openai/prompt/promptGeneratorWidget.py
-pyqt_openai/prompt/propPage.py
-pyqt_openai/prompt/templatePage.py
+pyqt_openai/prompt_gen_widget/__init__.py
+pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py
+pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py
+pyqt_openai/prompt_gen_widget/propPage.py
+pyqt_openai/prompt_gen_widget/propPromptUnitInputDialog.py
+pyqt_openai/prompt_gen_widget/templatePage.py
+pyqt_openai/prompt_gen_widget/templatePromptUnitInputDialog.py
+pyqt_openai/propmt_command_completer/__init__.py
+pyqt_openai/propmt_command_completer/commandSuggestionWidget.py
 pyqt_openai/right_sidebar/__init__.py
 pyqt_openai/right_sidebar/aiPlaygroundWidget.py
 pyqt_openai/right_sidebar/chatPage.py
 pyqt_openai/right_sidebar/completionPage.py
 pyqt_openai/right_sidebar/imagePage.py
 pyqt_openai/test/__init__.py
 pyqt_openai/test/htmlformat.py
-pyqt_openai/test/prompt_autocomplete.py
-pyqt_openai/test/rightSideBarTab.py
-pyqt_openai/test/sqlalchemy_example.py
-pyqt_openai/test/stable_diffusion/__init__.py
-pyqt_openai/test/stable_diffusion/in_model/__init__.py
-pyqt_openai/test/stable_diffusion/in_model/delete_model.py
-pyqt_openai/test/stable_diffusion/in_model/make_model.py
-pyqt_openai/test/stable_diffusion/in_model/using_model.py
+pyqt_openai/test/sqlalchemy_example.py
```

### Comparing `pyqt-openai-0.1.51/setup.py` & `pyqt-openai-0.1.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.1.51',
+    version='0.1.61',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
     package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'discord.svg', 'github.svg', 'help.svg', 'customize.svg', 'history.svg',
                                       'user.svg', 'sidebar.svg', 'prompt.svg', 'save.svg', 'stackontop.svg',
                                       'add.svg', 'delete.svg', 'setting.svg', 'search.svg',
```

