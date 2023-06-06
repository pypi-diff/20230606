# Comparing `tmp/cloudlanguagetools-5.5.tar.gz` & `tmp/cloudlanguagetools-5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-5.5.tar", last modified: Thu May 18 23:23:07 2023, max compression
+gzip compressed data, was "cloudlanguagetools-5.6.tar", last modified: Tue Jun  6 08:37:44 2023, max compression
```

## Comparing `cloudlanguagetools-5.5.tar` & `cloudlanguagetools-5.6.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-05-18 23:23:07.523512 cloudlanguagetools-5.5/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-05-18 23:23:07.522512 cloudlanguagetools-5.5/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-03-31 05:42:35.000000 cloudlanguagetools-5.5/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-05-18 23:23:07.521512 cloudlanguagetools-5.5/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23230 2023-05-17 23:12:08.000000 cloudlanguagetools-5.5/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-18 23:22:51.000000 cloudlanguagetools-5.5/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2104 2023-04-04 02:45:57.000000 cloudlanguagetools-5.5/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-03-31 05:42:35.000000 cloudlanguagetools-5.5/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8418 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6035 2023-04-04 02:45:57.000000 cloudlanguagetools-5.5/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    12687 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-04-13 04:54:02.000000 cloudlanguagetools-5.5/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1705 2023-04-13 04:54:02.000000 cloudlanguagetools-5.5/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17689 2023-04-04 02:45:57.000000 cloudlanguagetools-5.5/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1115 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-04-04 02:45:57.000000 cloudlanguagetools-5.5/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-03-28 05:23:58.000000 cloudlanguagetools-5.5/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-05-18 23:23:07.522512 cloudlanguagetools-5.5/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-05-18 23:23:06.000000 cloudlanguagetools-5.5/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1367 2023-05-18 23:23:07.000000 cloudlanguagetools-5.5/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-05-18 23:23:06.000000 cloudlanguagetools-5.5/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-05-18 23:23:07.000000 cloudlanguagetools-5.5/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-05-18 23:23:07.000000 cloudlanguagetools-5.5/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-05-18 23:23:07.523512 cloudlanguagetools-5.5/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-05-18 23:23:03.000000 cloudlanguagetools-5.5/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-06 08:37:44.653119 cloudlanguagetools-5.6/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-06-06 08:37:44.652119 cloudlanguagetools-5.6/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-06 08:37:44.652119 cloudlanguagetools-5.6/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23230 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2133 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6830 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8418 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6123 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    12687 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1705 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17858 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1115 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-06 08:37:44.652119 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1400 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-06-06 08:37:44.653119 cloudlanguagetools-5.6/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-06-06 08:37:41.000000 cloudlanguagetools-5.6/setup.py
```

### Comparing `cloudlanguagetools-5.5/LICENSE` & `cloudlanguagetools-5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/PKG-INFO` & `cloudlanguagetools-5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.5
+Version: 5.6
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/amazon.py` & `cloudlanguagetools-5.6/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-5.6/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/azure.py` & `cloudlanguagetools-5.6/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-5.6/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/constants.py` & `cloudlanguagetools-5.6/cloudlanguagetools/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     VocalWare = enum.auto()
     Voicen = enum.auto()
     FptAi = enum.auto()
     PyThaiNLP = enum.auto()
     Spacy = enum.auto()
     Wenlin = enum.auto()
     LibreTranslate = enum.auto()
+    ElevenLabs = enum.auto()
     TestServiceA = enum.auto()
     TestServiceB = enum.auto()
 
 class Gender(enum.Enum):
     Male = enum.auto()
     Female = enum.auto()
     Any = enum.auto()
```

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/deepl.py` & `cloudlanguagetools-5.6/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-5.6/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-5.6/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/encryption.py` & `cloudlanguagetools-5.6/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/epitran.py` & `cloudlanguagetools-5.6/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/forvo.py` & `cloudlanguagetools-5.6/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/fptai.py` & `cloudlanguagetools-5.6/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/google.py` & `cloudlanguagetools-5.6/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/languages.py` & `cloudlanguagetools-5.6/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-5.6/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-5.6/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/naver.py` & `cloudlanguagetools-5.6/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/openai.py` & `cloudlanguagetools-5.6/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-5.6/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-5.6/cloudlanguagetools/servicemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import cloudlanguagetools.naver
 import cloudlanguagetools.amazon
 import cloudlanguagetools.forvo
 import cloudlanguagetools.cereproc
 import cloudlanguagetools.vocalware
 import cloudlanguagetools.fptai
 import cloudlanguagetools.voicen
+import cloudlanguagetools.elevenlabs
 import cloudlanguagetools.encryption
 
 LOAD_NLP_MODELS = os.environ.get('CLOUDLANGUAGETOOLS_CORE_LOAD_NLP', 'yes') == 'yes'
 LOAD_TEST_SERVICES_ONLY = os.environ.get('CLOUDLANGUAGETOOLS_CORE_TEST_SERVICES', 'no') == 'yes'
 
 if LOAD_TEST_SERVICES_ONLY:
     import cloudlanguagetools.test_services
@@ -49,14 +50,15 @@
             self.services[cloudlanguagetools.constants.Service.Naver.name] = cloudlanguagetools.naver.NaverService()
             self.services[cloudlanguagetools.constants.Service.Amazon.name] = cloudlanguagetools.amazon.AmazonService()
             self.services[cloudlanguagetools.constants.Service.Forvo.name] = cloudlanguagetools.forvo.ForvoService()
             self.services[cloudlanguagetools.constants.Service.CereProc.name] = cloudlanguagetools.cereproc.CereProcService()
             self.services[cloudlanguagetools.constants.Service.VocalWare.name] = cloudlanguagetools.vocalware.VocalWareService()
             self.services[cloudlanguagetools.constants.Service.FptAi.name] = cloudlanguagetools.fptai.FptAiService()
             self.services[cloudlanguagetools.constants.Service.Voicen.name] = cloudlanguagetools.voicen.VoicenService()
+            self.services[cloudlanguagetools.constants.Service.ElevenLabs.name] = cloudlanguagetools.elevenlabs.ElevenLabsService()
 
             if LOAD_NLP_MODELS:
                 self.services[cloudlanguagetools.constants.Service.EasyPronunciation.name] = cloudlanguagetools.easypronunciation.EasyPronunciationService()
                 self.services[cloudlanguagetools.constants.Service.Epitran.name] = cloudlanguagetools.epitran.EpitranService()
                 self.services[cloudlanguagetools.constants.Service.DeepL.name] = cloudlanguagetools.deepl.DeepLService()
                 self.services[cloudlanguagetools.constants.Service.PyThaiNLP.name] = cloudlanguagetools.pythainlp.PyThaiNLPService()
                 self.services[cloudlanguagetools.constants.Service.Spacy.name] = cloudlanguagetools.spacy.SpacyService()
```

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/spacy.py` & `cloudlanguagetools-5.6/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/test_services.py` & `cloudlanguagetools-5.6/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-5.6/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-5.6/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-5.6/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-5.6/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-5.6/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/voicen.py` & `cloudlanguagetools-5.6/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/watson.py` & `cloudlanguagetools-5.6/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-5.6/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-5.6/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.5
+Version: 5.6
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.5/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-5.6/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 cloudlanguagetools/argostranslate.py
 cloudlanguagetools/azure.py
 cloudlanguagetools/cereproc.py
 cloudlanguagetools/constants.py
 cloudlanguagetools/deepl.py
 cloudlanguagetools/dictionarylookup.py
 cloudlanguagetools/easypronunciation.py
+cloudlanguagetools/elevenlabs.py
 cloudlanguagetools/encryption.py
 cloudlanguagetools/epitran.py
 cloudlanguagetools/errors.py
 cloudlanguagetools/forvo.py
 cloudlanguagetools/fptai.py
 cloudlanguagetools/google.py
 cloudlanguagetools/keys.py
```

### Comparing `cloudlanguagetools-5.5/setup.py` & `cloudlanguagetools-5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='5.5',
+      version='5.6',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
```

