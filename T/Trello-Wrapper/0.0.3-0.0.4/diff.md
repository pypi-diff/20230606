# Comparing `tmp/Trello-Wrapper-0.0.3.tar.gz` & `tmp/Trello-Wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Trello-Wrapper-0.0.3.tar", last modified: Mon Jun  5 09:08:22 2023, max compression
+gzip compressed data, was "Trello-Wrapper-0.0.4.tar", last modified: Tue Jun  6 05:39:50 2023, max compression
```

## Comparing `Trello-Wrapper-0.0.3.tar` & `Trello-Wrapper-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1036 2023-06-05 06:52:02.000000 Trello-Wrapper-0.0.3/LICENSE
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1768 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/PKG-INFO
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1117 2023-06-05 07:54:07.000000 Trello-Wrapper-0.0.3/README.md
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.990804 Trello-Wrapper-0.0.3/Trello_Wrapper/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      765 2023-06-05 06:58:44.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/__init__.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/Trello_Wrapper/actions/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      235 2023-06-02 12:45:31.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/actions/__init__.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1562 2023-06-02 09:45:15.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_delete.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    10677 2023-06-02 09:45:57.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_get.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1551 2023-06-02 09:52:23.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_post.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     4001 2023-06-02 09:52:23.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_put.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/Trello_Wrapper/boards/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      234 2023-06-02 12:44:01.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/boards/__init__.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1684 2023-06-02 07:19:34.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_delete.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    20027 2023-06-02 09:38:34.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_get.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     8932 2023-06-02 08:05:47.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_post.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    15385 2023-06-02 08:01:57.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_put.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/Trello_Wrapper/cards/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      251 2023-06-02 13:17:19.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/cards/__init__.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     4632 2023-06-02 13:07:30.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_delete.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    18611 2023-06-02 13:01:25.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_get.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     9753 2023-06-02 13:04:45.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_post.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     6169 2023-06-02 13:06:53.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_put.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      240 2023-06-02 13:34:50.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/__init__.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1390 2023-06-02 13:34:02.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_delete.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     7037 2023-06-02 13:34:02.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_get.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     3073 2023-06-02 13:32:16.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_post.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     2230 2023-06-02 13:26:26.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_put.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/Trello_Wrapper/labels/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      236 2023-06-02 13:37:21.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/labels/__init__.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      671 2023-06-02 13:38:30.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_delete.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1047 2023-06-02 13:37:21.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_get.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1018 2023-06-02 13:42:06.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_post.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1676 2023-06-02 13:39:03.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_put.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/Trello_Wrapper/lists/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      234 2023-06-05 05:43:46.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/lists/__init__.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      138 2023-06-05 05:44:23.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_delete.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     3406 2023-06-05 05:54:10.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_get.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     2609 2023-06-05 05:48:57.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_post.py
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     3477 2023-06-05 05:52:43.000000 Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_put.py
-drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-05 09:08:22.990804 Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1768 2023-06-05 09:08:22.000000 Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1205 2023-06-05 09:08:22.000000 Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)        1 2023-06-05 09:08:22.000000 Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)        9 2023-06-05 09:08:22.000000 Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/requires.txt
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)       15 2023-06-05 09:08:22.000000 Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/top_level.txt
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)       38 2023-06-05 09:08:22.994803 Trello-Wrapper-0.0.3/setup.cfg
--rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      670 2023-06-05 09:08:15.000000 Trello-Wrapper-0.0.3/setup.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.781065 Trello-Wrapper-0.0.4/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1036 2023-06-05 06:52:02.000000 Trello-Wrapper-0.0.4/LICENSE
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1768 2023-06-06 05:39:50.781065 Trello-Wrapper-0.0.4/PKG-INFO
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1117 2023-06-05 07:54:07.000000 Trello-Wrapper-0.0.4/README.md
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.777065 Trello-Wrapper-0.0.4/Trello_Wrapper/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1091 2023-06-06 05:25:17.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/__init__.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.777065 Trello-Wrapper-0.0.4/Trello_Wrapper/actions/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      235 2023-06-02 12:45:31.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/actions/__init__.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1562 2023-06-02 09:45:15.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_delete.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    10677 2023-06-02 09:45:57.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_get.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1551 2023-06-02 09:52:23.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_post.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     4001 2023-06-02 09:52:23.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_put.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.777065 Trello-Wrapper-0.0.4/Trello_Wrapper/boards/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      234 2023-06-02 12:44:01.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/boards/__init__.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1684 2023-06-02 07:19:34.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_delete.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    20027 2023-06-02 09:38:34.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_get.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     8932 2023-06-02 08:05:47.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_post.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    15385 2023-06-02 08:01:57.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_put.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.777065 Trello-Wrapper-0.0.4/Trello_Wrapper/cards/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      251 2023-06-02 13:17:19.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/cards/__init__.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     4632 2023-06-02 13:07:30.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_delete.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)    18611 2023-06-02 13:01:25.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_get.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     9753 2023-06-02 13:04:45.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_post.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     6169 2023-06-02 13:06:53.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_put.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.781065 Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      240 2023-06-02 13:34:50.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/__init__.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1390 2023-06-02 13:34:02.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_delete.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     7037 2023-06-02 13:34:02.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_get.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     3073 2023-06-02 13:32:16.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_post.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     2230 2023-06-02 13:26:26.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_put.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.781065 Trello-Wrapper-0.0.4/Trello_Wrapper/labels/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      236 2023-06-02 13:37:21.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/labels/__init__.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      671 2023-06-02 13:38:30.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_delete.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1047 2023-06-02 13:37:21.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_get.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1018 2023-06-02 13:42:06.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_post.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1676 2023-06-02 13:39:03.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_put.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.781065 Trello-Wrapper-0.0.4/Trello_Wrapper/lists/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      234 2023-06-05 05:43:46.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/lists/__init__.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      138 2023-06-05 05:44:23.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_delete.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     3406 2023-06-05 05:54:10.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_get.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     2609 2023-06-05 05:48:57.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_post.py
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     3477 2023-06-05 05:52:43.000000 Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_put.py
+drwxrwxr-x   0 tsilavo   (1000) tsilavo   (1000)        0 2023-06-06 05:39:50.777065 Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1768 2023-06-06 05:39:50.000000 Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)     1205 2023-06-06 05:39:50.000000 Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)        1 2023-06-06 05:39:50.000000 Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)        9 2023-06-06 05:39:50.000000 Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/requires.txt
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)       15 2023-06-06 05:39:50.000000 Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)       38 2023-06-06 05:39:50.781065 Trello-Wrapper-0.0.4/setup.cfg
+-rw-rw-r--   0 tsilavo   (1000) tsilavo   (1000)      670 2023-06-06 05:27:27.000000 Trello-Wrapper-0.0.4/setup.py
```

### Comparing `Trello-Wrapper-0.0.3/LICENSE` & `Trello-Wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/PKG-INFO` & `Trello-Wrapper-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Trello-Wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Wrapper around the Trello API
 Home-page: https://github.com/Rtsil/Trello-Wrapper
 Author: Rtsil
 Author-email: rtsilavotahina@gmail.com
 Keywords: trello,wrapper,api
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Trello-Wrapper-0.0.3/README.md` & `Trello-Wrapper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/__init__.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 from Trello_Wrapper.boards import Boards
 from Trello_Wrapper.actions import Actions
 from Trello_Wrapper.cards import Cards
+from Trello_Wrapper.labels import Labels
+from Trello_Wrapper.checklists import Checklists
+from Trello_Wrapper.lists import Lists
+
 
 
 class Trello():
     def __init__(self, token=None, api_key=None):
         if token is None:
             token = os.getenv('TRELLO_TOKEN')
         if api_key is None:
@@ -13,16 +17,24 @@
 
         if token is None or api_key is None:
             raise ValueError("Missing base token or API key")
 
         self.token = token
         self.api_key = api_key
 
-    # Rest of the class methods...
     def Boards(self):
         return Boards(self.api_key, self.token)
 
     def Actions(self):
         return Actions(self.api_key, self.token)
 
     def Cards(self):
-        return Cards(self.api_key, self.token)
+        return Cards(self.api_key, self.token)
+    
+    def Labels(self):
+        return Labels(self.api_key, self.token)
+    
+    def Lists(self):
+        return Lists(self.api_key, self.token)
+    
+    def Checklists(self):
+        return Checklists(self.api_key, self.token)
```

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_delete.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_delete.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_get.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_get.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_post.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_post.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/actions/_put.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/actions/_put.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_delete.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_delete.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_get.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_get.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_post.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_post.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/boards/_put.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/boards/_put.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_delete.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_delete.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_get.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_get.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_post.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_post.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/cards/_put.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/cards/_put.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_delete.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_delete.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_get.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_get.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_post.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_post.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/checklists/_put.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/checklists/_put.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_delete.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_delete.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_get.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_get.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_post.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_post.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/labels/_put.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/labels/_put.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_get.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_get.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_post.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_post.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper/lists/_put.py` & `Trello-Wrapper-0.0.4/Trello_Wrapper/lists/_put.py`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/PKG-INFO` & `Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Trello-Wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Wrapper around the Trello API
 Home-page: https://github.com/Rtsil/Trello-Wrapper
 Author: Rtsil
 Author-email: rtsilavotahina@gmail.com
 Keywords: trello,wrapper,api
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Trello-Wrapper-0.0.3/Trello_Wrapper.egg-info/SOURCES.txt` & `Trello-Wrapper-0.0.4/Trello_Wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Trello-Wrapper-0.0.3/setup.py` & `Trello-Wrapper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 with open("README2.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='Trello-Wrapper',
-    version='0.0.3',
+    version='0.0.4',
     author='Rtsil',
     author_email='rtsilavotahina@gmail.com',
     description='A Python Wrapper around the Trello API',
     long_description=long_description,
     url='https://github.com/Rtsil/Trello-Wrapper',
     packages=find_packages(),
     classifiers=[
```

