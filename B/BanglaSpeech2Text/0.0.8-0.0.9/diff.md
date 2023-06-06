# Comparing `tmp/BanglaSpeech2Text-0.0.8.tar.gz` & `tmp/BanglaSpeech2Text-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanglaSpeech2Text-0.0.8.tar", last modified: Fri Jan 13 11:56:06 2023, max compression
+gzip compressed data, was "BanglaSpeech2Text-0.0.9.tar", last modified: Fri Jan 13 12:18:02 2023, max compression
```

## Comparing `BanglaSpeech2Text-0.0.8.tar` & `BanglaSpeech2Text-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 11:56:06.688015 BanglaSpeech2Text-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-01-13 11:56:06.673090 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/
--rw-rw-rw-   0        0        0     5865 2023-01-13 11:56:04.000000 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-01-13 11:56:06.000000 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 11:56:04.000000 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-12 15:49:57.000000 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      399 2023-01-13 11:56:04.000000 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-01-13 11:56:04.000000 BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-01-12 06:03:07.000000 BanglaSpeech2Text-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       24 2023-01-12 14:46:32.000000 BanglaSpeech2Text-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5865 2023-01-13 11:56:06.687010 BanglaSpeech2Text-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4176 2023-01-13 10:47:24.000000 BanglaSpeech2Text-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 11:56:06.675093 BanglaSpeech2Text-0.0.8/banglaspeech2text/
--rw-rw-rw-   0        0        0       76 2023-01-12 15:00:04.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/__init__.py
--rw-rw-rw-   0        0        0     3994 2023-01-13 11:37:18.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/speech2text.py
-drwxrwxrwx   0        0        0        0 2023-01-13 11:56:06.684651 BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/
--rw-rw-rw-   0        0        0      535 2023-01-13 11:37:00.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/__init__.py
--rw-rw-rw-   0        0        0    12299 2023-01-13 10:34:47.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/download_models.py
--rw-rw-rw-   0        0        0      447 2023-01-13 11:55:53.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/download_path.py
--rw-rw-rw-   0        0        0     2359 2023-01-13 11:55:27.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/extras.py
--rw-rw-rw-   0        0        0     1553 2023-01-13 09:21:18.000000 BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/install_packages.py
--rw-rw-rw-   0        0        0       42 2023-01-13 11:56:06.688015 BanglaSpeech2Text-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2235 2023-01-13 11:54:14.000000 BanglaSpeech2Text-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.155764 BanglaSpeech2Text-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.136213 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/
+-rw-rw-rw-   0        0        0     5865 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-01-13 12:18:01.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-12 15:49:57.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      367 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-01-12 06:03:07.000000 BanglaSpeech2Text-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-01-12 14:46:32.000000 BanglaSpeech2Text-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5865 2023-01-13 12:18:02.154765 BanglaSpeech2Text-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4176 2023-01-13 10:47:24.000000 BanglaSpeech2Text-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.145763 BanglaSpeech2Text-0.0.9/banglaspeech2text/
+-rw-rw-rw-   0        0        0       76 2023-01-12 15:00:04.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/__init__.py
+-rw-rw-rw-   0        0        0     3994 2023-01-13 11:37:18.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/speech2text.py
+drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.152765 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/
+-rw-rw-rw-   0        0        0      535 2023-01-13 11:37:00.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/__init__.py
+-rw-rw-rw-   0        0        0    12299 2023-01-13 10:34:47.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/download_models.py
+-rw-rw-rw-   0        0        0      447 2023-01-13 11:55:53.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/download_path.py
+-rw-rw-rw-   0        0        0     2359 2023-01-13 11:55:27.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/extras.py
+-rw-rw-rw-   0        0        0     1553 2023-01-13 09:21:18.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/install_packages.py
+-rw-rw-rw-   0        0        0       42 2023-01-13 12:18:02.155764 BanglaSpeech2Text-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2235 2023-01-13 12:17:15.000000 BanglaSpeech2Text-0.0.9/setup.py
```

### Comparing `BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/PKG-INFO` & `BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BanglaSpeech2Text
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open-source offline speech-to-text package for Bangla language. Fine-tuned on the latest whisper speech to text model for optimal performance.
 Home-page: https://github.com/shhossain/BanglaSpeech2Text
 Author: Sifat (shhossain)
 Author-email: <hossain@gmail.com>
 Project-URL: Documentation, https://github.com/shhossain/BanglaSpeech2Text
 Project-URL: Source, https://github.com/shhossain/BanglaSpeech2Text
 Project-URL: Bug Tracker, https://github.com/shhossain/BanglaSpeech2Text/issues
```

### Comparing `BanglaSpeech2Text-0.0.8/BanglaSpeech2Text.egg-info/SOURCES.txt` & `BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/LICENSE` & `BanglaSpeech2Text-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/PKG-INFO` & `BanglaSpeech2Text-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BanglaSpeech2Text
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open-source offline speech-to-text package for Bangla language. Fine-tuned on the latest whisper speech to text model for optimal performance.
 Home-page: https://github.com/shhossain/BanglaSpeech2Text
 Author: Sifat (shhossain)
 Author-email: <hossain@gmail.com>
 Project-URL: Documentation, https://github.com/shhossain/BanglaSpeech2Text
 Project-URL: Source, https://github.com/shhossain/BanglaSpeech2Text
 Project-URL: Bug Tracker, https://github.com/shhossain/BanglaSpeech2Text/issues
```

### Comparing `BanglaSpeech2Text-0.0.8/README.md` & `BanglaSpeech2Text-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/banglaspeech2text/speech2text.py` & `BanglaSpeech2Text-0.0.9/banglaspeech2text/speech2text.py`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/__init__.py` & `BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/download_models.py` & `BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/download_models.py`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/extras.py` & `BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/extras.py`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/banglaspeech2text/utils/install_packages.py` & `BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/install_packages.py`

 * *Files identical despite different names*

### Comparing `BanglaSpeech2Text-0.0.8/setup.py` & `BanglaSpeech2Text-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.0.8'
+version = '0.0.9'
 description = 'An open-source offline speech-to-text package for Bangla language. Fine-tuned on the latest whisper speech to text model for optimal performance.'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 name = 'BanglaSpeech2Text'
 author = 'Sifat (shhossain)'
```

