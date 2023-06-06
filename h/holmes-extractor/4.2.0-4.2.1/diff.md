# Comparing `tmp/holmes-extractor-4.2.0.tar.gz` & `tmp/holmes-extractor-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holmes-extractor-4.2.0.tar", last modified: Tue Jan 31 12:54:57 2023, max compression
+gzip compressed data, was "holmes-extractor-4.2.1.tar", last modified: Tue Jun  6 11:06:20 2023, max compression
```

## Comparing `holmes-extractor-4.2.0.tar` & `holmes-extractor-4.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/
--rw-rw-r--   0 richard   (1001) richard   (1001)     1125 2023-01-31 11:56:19.000000 holmes-extractor-4.2.0/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)       88 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/MANIFEST.in
--rw-rw-r--   0 richard   (1001) richard   (1001)     7683 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)   120787 2023-01-31 12:02:06.000000 holmes-extractor-4.2.0/README.md
--rw-rw-r--   0 richard   (1001) richard   (1001)     6111 2023-01-31 12:01:26.000000 holmes-extractor-4.2.0/SHORTREADME.md
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/
--rw-rw-r--   0 richard   (1001) richard   (1001)      147 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)       21 2023-01-31 11:55:19.000000 holmes-extractor-4.2.0/holmes_extractor/about.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    44286 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/classification.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      139 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/config.cfg
--rw-rw-r--   0 richard   (1001) richard   (1001)    13370 2023-01-31 12:07:17.000000 holmes-extractor-4.2.0/holmes_extractor/consoles.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     1256 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/errors.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/lang/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/__init__.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/lang/de/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/de/__init__.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/lang/de/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/de/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     7997 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/de/data/derivation.csv
--rw-rw-r--   0 richard   (1001) richard   (1001)    82412 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/de/language_specific_rules.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/lang/en/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/en/__init__.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/lang/en/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/en/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     8166 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/en/data/derivation.csv
--rw-rw-r--   0 richard   (1001) richard   (1001)    58023 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/lang/en/language_specific_rules.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    58740 2023-01-31 09:30:35.000000 holmes-extractor-4.2.0/holmes_extractor/manager.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    14883 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/ontology.py
--rw-rw-r--   0 richard   (1001) richard   (1001)   134690 2023-01-31 09:31:03.000000 holmes-extractor-4.2.0/holmes_extractor/parsing.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    46397 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/structural_matching.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    72970 2023-01-31 09:46:48.000000 holmes-extractor-4.2.0/holmes_extractor/topic_matching.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor/word_matching/
--rw-rw-r--   0 richard   (1001) richard   (1001)     7927 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/derivation.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     5958 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/direct.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     5505 2023-01-30 19:52:27.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/embedding.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     4829 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/entity.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     6996 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/entity_embedding.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     7091 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/general.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     8397 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/ontology.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     6330 2023-01-31 09:31:13.000000 holmes-extractor-4.2.0/holmes_extractor/word_matching/question.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/holmes_extractor.egg-info/
--rw-rw-r--   0 richard   (1001) richard   (1001)     7683 2023-01-31 12:54:57.000000 holmes-extractor-4.2.0/holmes_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)     1338 2023-01-31 12:54:57.000000 holmes-extractor-4.2.0/holmes_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        1 2023-01-31 12:54:57.000000 holmes-extractor-4.2.0/holmes_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       44 2023-01-31 12:54:57.000000 holmes-extractor-4.2.0/holmes_extractor.egg-info/requires.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       17 2023-01-31 12:54:57.000000 holmes-extractor-4.2.0/holmes_extractor.egg-info/top_level.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)      100 2023-01-30 19:15:26.000000 holmes-extractor-4.2.0/pyproject.toml
--rw-rw-r--   0 richard   (1001) richard   (1001)     1568 2023-01-31 12:54:57.393725 holmes-extractor-4.2.0/setup.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.102202 holmes-extractor-4.2.1/
+-rw-r--r--   0 richard    (501) staff       (20)     1125 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)       88 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/MANIFEST.in
+-rw-r--r--   0 richard    (501) staff       (20)     7734 2023-06-06 11:06:20.102254 holmes-extractor-4.2.1/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)   120935 2023-06-06 08:54:01.000000 holmes-extractor-4.2.1/README.md
+-rw-r--r--   0 richard    (501) staff       (20)     6111 2023-06-06 08:54:08.000000 holmes-extractor-4.2.1/SHORTREADME.md
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.099139 holmes-extractor-4.2.1/holmes_extractor/
+-rw-r--r--   0 richard    (501) staff       (20)      147 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)       21 2023-06-06 08:54:15.000000 holmes-extractor-4.2.1/holmes_extractor/about.py
+-rw-r--r--   0 richard    (501) staff       (20)    44286 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/classification.py
+-rw-r--r--   0 richard    (501) staff       (20)      139 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/config.cfg
+-rw-r--r--   0 richard    (501) staff       (20)    13370 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/consoles.py
+-rw-r--r--   0 richard    (501) staff       (20)     1256 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/errors.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.099866 holmes-extractor-4.2.1/holmes_extractor/lang/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/__init__.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.100031 holmes-extractor-4.2.1/holmes_extractor/lang/de/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/de/__init__.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.100327 holmes-extractor-4.2.1/holmes_extractor/lang/de/data/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/de/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)     7997 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/de/data/derivation.csv
+-rw-r--r--   0 richard    (501) staff       (20)    82412 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/de/language_specific_rules.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.100530 holmes-extractor-4.2.1/holmes_extractor/lang/en/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/en/__init__.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.100803 holmes-extractor-4.2.1/holmes_extractor/lang/en/data/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/en/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)     8166 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/en/data/derivation.csv
+-rw-r--r--   0 richard    (501) staff       (20)    58023 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/lang/en/language_specific_rules.py
+-rw-r--r--   0 richard    (501) staff       (20)    58740 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/manager.py
+-rw-r--r--   0 richard    (501) staff       (20)    14883 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/ontology.py
+-rw-r--r--   0 richard    (501) staff       (20)   134690 2023-06-06 09:35:15.000000 holmes-extractor-4.2.1/holmes_extractor/parsing.py
+-rw-r--r--   0 richard    (501) staff       (20)    46397 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/structural_matching.py
+-rw-r--r--   0 richard    (501) staff       (20)    72970 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/topic_matching.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.102068 holmes-extractor-4.2.1/holmes_extractor/word_matching/
+-rw-r--r--   0 richard    (501) staff       (20)     7927 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/derivation.py
+-rw-r--r--   0 richard    (501) staff       (20)     5958 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/direct.py
+-rw-r--r--   0 richard    (501) staff       (20)     5505 2023-06-06 10:02:59.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/embedding.py
+-rw-r--r--   0 richard    (501) staff       (20)     4829 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/entity.py
+-rw-r--r--   0 richard    (501) staff       (20)     6996 2023-06-06 10:03:03.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/entity_embedding.py
+-rw-r--r--   0 richard    (501) staff       (20)     7091 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/general.py
+-rw-r--r--   0 richard    (501) staff       (20)     8397 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/ontology.py
+-rw-r--r--   0 richard    (501) staff       (20)     6330 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/holmes_extractor/word_matching/question.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 11:06:20.099760 holmes-extractor-4.2.1/holmes_extractor.egg-info/
+-rw-r--r--   0 richard    (501) staff       (20)     7734 2023-06-06 11:06:20.000000 holmes-extractor-4.2.1/holmes_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)     1338 2023-06-06 11:06:20.000000 holmes-extractor-4.2.1/holmes_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 richard    (501) staff       (20)        1 2023-06-06 11:06:20.000000 holmes-extractor-4.2.1/holmes_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 richard    (501) staff       (20)       44 2023-06-06 11:06:20.000000 holmes-extractor-4.2.1/holmes_extractor.egg-info/requires.txt
+-rw-r--r--   0 richard    (501) staff       (20)       17 2023-06-06 11:06:20.000000 holmes-extractor-4.2.1/holmes_extractor.egg-info/top_level.txt
+-rw-r--r--   0 richard    (501) staff       (20)      100 2023-06-06 08:49:43.000000 holmes-extractor-4.2.1/pyproject.toml
+-rw-r--r--   0 richard    (501) staff       (20)     1608 2023-06-06 11:06:20.102488 holmes-extractor-4.2.1/setup.cfg
```

### Comparing `holmes-extractor-4.2.0/LICENSE` & `holmes-extractor-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/PKG-INFO` & `holmes-extractor-4.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holmes-extractor
-Version: 4.2.0
+Version: 4.2.1
 Summary: Information extraction from English and German texts based on predicate logic
 Home-page: https://github.com/richardpaulhudson/holmes-extractor
 Author: Richard Paul Hudson
 Author-email: hudsonrichardpaul@gmail.com
 License: MIT
 Keywords: nlp,information-extraction,spacy,spacy-extension,python,machine-learning,ontology,semantics
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,22 +21,23 @@
 Classifier: Natural Language :: German
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: <3.11,>=3.6
+Requires-Python: <3.12,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-**Holmes** is a Python 3 library (v3.6—v3.10) running on top of
+**Holmes** is a Python 3 library (v3.6—v3.11) running on top of
 [spaCy](https://spacy.io/) (v3.1—v3.5) that supports a number of use cases
 involving information extraction from English and German texts. In all use cases, the information
 extraction is based on analysing the semantic relationships expressed by the component parts of
 each sentence:
 
 - In the [chatbot](#getting-started) use case, the system is configured using one or more **search phrases**.
 Holmes then looks for structures whose meanings correspond to those of these search phrases within
```

### Comparing `holmes-extractor-4.2.0/README.md` & `holmes-extractor-4.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,22 +96,23 @@
         -   [8.4.5 Version 3.0.0](#version-300)
         -   [8.4.6 Version 4.0.0](#version-400)
         -   [8.4.7 Version 4.0.1](#version-401)
         -   [8.4.8 Version 4.0.2](#version-402)
         -   [8.4.9 Version 4.0.3](#version-403)
         -   [8.4.10 Version 4.1.0](#version-410)
         -   [8.4.11 Version 4.2.0](#version-420)
+        -   [8.4.12 Version 4.2.1](#version-421)
 
 <a id="introduction"></a>
 ### 1. Introduction
 
 <a id="the-basic-idea"></a>
 #### 1.1 The basic idea
 
-**Holmes** is a Python 3 library (v3.6—v3.10) running on top of
+**Holmes** is a Python 3 library (v3.6—v3.11) running on top of
 [spaCy](https://spacy.io/) (v3.1—v3.5) that supports a number of use cases
 involving information extraction from English and German texts. In all use cases, the information
 extraction is based on analysing the semantic relationships expressed by the component parts of
 each sentence:
 
 - In the [chatbot](#getting-started) use case, the system is configured using one or more **search phrases**.
 Holmes then looks for structures whose meanings correspond to those of these search phrases within
@@ -2122,7 +2123,12 @@
 - Support was added for [bespoke named-entity labels](#using-bespoke-named-entity-recognition).
 - [Documentation](#non-standard-interaction-with-spacy-models) was added about non-standard interaction with spaCy models.
 
 <a id="version-420"></a>
 ##### 8.4.11 Version 4.2.0
 
 - Support was added for spaCy version 3.5.
+
+<a id="version-421"></a>
+##### 8.4.12 Version 4.2.1
+
+- Support was added for Python version 3.11.
```

### Comparing `holmes-extractor-4.2.0/SHORTREADME.md` & `holmes-extractor-4.2.1/SHORTREADME.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**Holmes** is a Python 3 library (v3.6—v3.10) running on top of
+**Holmes** is a Python 3 library (v3.6—v3.11) running on top of
 [spaCy](https://spacy.io/) (v3.1—v3.5) that supports a number of use cases
 involving information extraction from English and German texts. In all use cases, the information
 extraction is based on analysing the semantic relationships expressed by the component parts of
 each sentence:
 
 - In the [chatbot](#getting-started) use case, the system is configured using one or more **search phrases**.
 Holmes then looks for structures whose meanings correspond to those of these search phrases within
```

### Comparing `holmes-extractor-4.2.0/holmes_extractor/classification.py` & `holmes-extractor-4.2.1/holmes_extractor/classification.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/consoles.py` & `holmes-extractor-4.2.1/holmes_extractor/consoles.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/errors.py` & `holmes-extractor-4.2.1/holmes_extractor/errors.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/lang/de/data/derivation.csv` & `holmes-extractor-4.2.1/holmes_extractor/lang/de/data/derivation.csv`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/lang/de/language_specific_rules.py` & `holmes-extractor-4.2.1/holmes_extractor/lang/de/language_specific_rules.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/lang/en/data/derivation.csv` & `holmes-extractor-4.2.1/holmes_extractor/lang/en/data/derivation.csv`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/lang/en/language_specific_rules.py` & `holmes-extractor-4.2.1/holmes_extractor/lang/en/language_specific_rules.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/manager.py` & `holmes-extractor-4.2.1/holmes_extractor/manager.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/ontology.py` & `holmes-extractor-4.2.1/holmes_extractor/ontology.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/parsing.py` & `holmes-extractor-4.2.1/holmes_extractor/parsing.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/structural_matching.py` & `holmes-extractor-4.2.1/holmes_extractor/structural_matching.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/topic_matching.py` & `holmes-extractor-4.2.1/holmes_extractor/topic_matching.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/derivation.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/derivation.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/direct.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/direct.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/embedding.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/embedding.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/entity.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/entity.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/entity_embedding.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/entity_embedding.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/general.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/general.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/ontology.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/ontology.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor/word_matching/question.py` & `holmes-extractor-4.2.1/holmes_extractor/word_matching/question.py`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/holmes_extractor.egg-info/PKG-INFO` & `holmes-extractor-4.2.1/holmes_extractor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holmes-extractor
-Version: 4.2.0
+Version: 4.2.1
 Summary: Information extraction from English and German texts based on predicate logic
 Home-page: https://github.com/richardpaulhudson/holmes-extractor
 Author: Richard Paul Hudson
 Author-email: hudsonrichardpaul@gmail.com
 License: MIT
 Keywords: nlp,information-extraction,spacy,spacy-extension,python,machine-learning,ontology,semantics
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,22 +21,23 @@
 Classifier: Natural Language :: German
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: <3.11,>=3.6
+Requires-Python: <3.12,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-**Holmes** is a Python 3 library (v3.6—v3.10) running on top of
+**Holmes** is a Python 3 library (v3.6—v3.11) running on top of
 [spaCy](https://spacy.io/) (v3.1—v3.5) that supports a number of use cases
 involving information extraction from English and German texts. In all use cases, the information
 extraction is based on analysing the semantic relationships expressed by the component parts of
 each sentence:
 
 - In the [chatbot](#getting-started) use case, the system is configured using one or more **search phrases**.
 Holmes then looks for structures whose meanings correspond to those of these search phrases within
```

### Comparing `holmes-extractor-4.2.0/holmes_extractor.egg-info/SOURCES.txt` & `holmes-extractor-4.2.1/holmes_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `holmes-extractor-4.2.0/setup.cfg` & `holmes-extractor-4.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holmes-extractor
-version = 4.2.0
+version = 4.2.1
 description = Information extraction from English and German texts based on predicate logic
 long_description = file: SHORTREADME.md
 long_description_content_type = text/markdown
 url = https://github.com/richardpaulhudson/holmes-extractor
 author = Richard Paul Hudson
 author_email = hudsonrichardpaul@gmail.com
 license = MIT
@@ -24,24 +24,25 @@
 	Natural Language :: German
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Scientific/Engineering :: Information Analysis
 	Topic :: Text Processing :: Linguistic
 
 [options]
 include_package_data = True
-python_requires = >=3.6,<3.11
+python_requires = >=3.6,<3.12
 install_requires = 
 	spacy>=3.1.0,<3.6.0
-	coreferee>=1.4.0
+	coreferee>=1.4.1
 	rdflib
 
 [options.package_data]
 * = *.cfg, *.csv
 
 [egg_info]
 tag_build =
```

