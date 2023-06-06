# Comparing `tmp/qna-builder-0.1.1.tar.gz` & `tmp/qna-builder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qna-builder-0.1.1.tar", last modified: Tue Jun  6 17:57:40 2023, max compression
+gzip compressed data, was "qna-builder-0.1.2.tar", last modified: Tue Jun  6 18:27:44 2023, max compression
```

## Comparing `qna-builder-0.1.1.tar` & `qna-builder-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:40.819372 qna-builder-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-06 17:57:40.819372 qna-builder-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-06 17:57:26.000000 qna-builder-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:40.819372 qna-builder-0.1.1/qna_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-06 17:57:40.000000 qna-builder-0.1.1/qna_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 17:57:40.000000 qna-builder-0.1.1/qna_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:40.000000 qna-builder-0.1.1/qna_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 17:57:40.000000 qna-builder-0.1.1/qna_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 17:57:40.000000 qna-builder-0.1.1/qna_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:40.819372 qna-builder-0.1.1/qnabuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 17:57:26.000000 qna-builder-0.1.1/qnabuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 17:57:26.000000 qna-builder-0.1.1/qnabuilder/_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-06 17:57:26.000000 qna-builder-0.1.1/qnabuilder/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-06 17:57:26.000000 qna-builder-0.1.1/qnabuilder/qna_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:57:40.819372 qna-builder-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-06 17:57:26.000000 qna-builder-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:27:44.698556 qna-builder-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-06 18:27:44.698556 qna-builder-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-06 18:27:33.000000 qna-builder-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:27:44.698556 qna-builder-0.1.2/qna_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 18:27:44.000000 qna-builder-0.1.2/qna_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:27:44.698556 qna-builder-0.1.2/qnabuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-06 18:27:33.000000 qna-builder-0.1.2/qnabuilder/qna_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 18:27:44.698556 qna-builder-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-06 18:27:33.000000 qna-builder-0.1.2/setup.py
```

### Comparing `qna-builder-0.1.1/PKG-INFO` & `qna-builder-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qna-builder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Similarity-based conversational dialog engine for Python.
 Home-page: https://github.com/msamsami/qna-builder
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,qna,qnabuilder,chat,chatbot,conversation,dialog
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
@@ -13,23 +13,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: kb_editor
 
-# QnA Bot
+# QnA Builder
 
-![](https://img.shields.io/badge/version-v0.1.1-green)
+![](https://img.shields.io/badge/version-v0.1.2-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/qna-bot/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/qna-builder)](https://pypi.org/project/qna-builder/)
 
 <p>
-<img src="logo.jpg" alt="QnA Bot logo" width="200"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/logo.jpg" alt="QnA Builder logo" width="200"/>
 <br>
 </p>
 
 ## Introduction
 
 **QnA Builder** is a simple, no code way to build chatbots in Python. It provides a similarity-based conversational dialog
 engine, **QnA Bot**, which makes it easy to generate automated responses to input questions according to a set of known
```

### Comparing `qna-builder-0.1.1/README.md` & `qna-builder-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# QnA Bot
+# QnA Builder
 
-![](https://img.shields.io/badge/version-v0.1.1-green)
+![](https://img.shields.io/badge/version-v0.1.2-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/qna-bot/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/qna-builder)](https://pypi.org/project/qna-builder/)
 
 <p>
-<img src="logo.jpg" alt="QnA Bot logo" width="200"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/logo.jpg" alt="QnA Builder logo" width="200"/>
 <br>
 </p>
 
 ## Introduction
 
 **QnA Builder** is a simple, no code way to build chatbots in Python. It provides a similarity-based conversational dialog
 engine, **QnA Bot**, which makes it easy to generate automated responses to input questions according to a set of known
```

### Comparing `qna-builder-0.1.1/qna_builder.egg-info/PKG-INFO` & `qna-builder-0.1.2/qna_builder.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qna-builder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Similarity-based conversational dialog engine for Python.
 Home-page: https://github.com/msamsami/qna-builder
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,qna,qnabuilder,chat,chatbot,conversation,dialog
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
@@ -13,23 +13,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: kb_editor
 
-# QnA Bot
+# QnA Builder
 
-![](https://img.shields.io/badge/version-v0.1.1-green)
+![](https://img.shields.io/badge/version-v0.1.2-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/qna-bot/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/qna-builder)](https://pypi.org/project/qna-builder/)
 
 <p>
-<img src="logo.jpg" alt="QnA Bot logo" width="200"/>
+<img src="https://raw.githubusercontent.com/msamsami/qna-builder/main/logo.jpg" alt="QnA Builder logo" width="200"/>
 <br>
 </p>
 
 ## Introduction
 
 **QnA Builder** is a simple, no code way to build chatbots in Python. It provides a similarity-based conversational dialog
 engine, **QnA Bot**, which makes it easy to generate automated responses to input questions according to a set of known
```

### Comparing `qna-builder-0.1.1/qnabuilder/__init__.py` & `qna-builder-0.1.2/qnabuilder/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 qna-bot is a similarity-based conversational dialog engine for Python that helps you quickly and easily create
 smart chatbots using a knowledge base of pre-defined questions and answers.
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = "Mehdi Samsami"
 
 __all__ = [
     "QnABot",
     "EmbeddingModel",
     "SimilarityMetric",
     "QnAKnowledgeBase",
```

### Comparing `qna-builder-0.1.1/qnabuilder/_utils.py` & `qna-builder-0.1.2/qnabuilder/_utils.py`

 * *Files identical despite different names*

### Comparing `qna-builder-0.1.1/qnabuilder/qna_bot.py` & `qna-builder-0.1.2/qnabuilder/qna_bot.py`

 * *Files identical despite different names*

### Comparing `qna-builder-0.1.1/setup.py` & `qna-builder-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 from os import path
 from setuptools import setup
 
 
 setup(
     name='qna-builder',
-    version='0.1.1',
+    version='0.1.2',
     description='Similarity-based conversational dialog engine for Python.',
     keywords=['python', 'qna', 'qnabuilder', 'chat', 'chatbot', 'conversation', 'dialog'],
     author='Mehdi Samsami',
     author_email='mehdisamsami@live.com',
     url='https://github.com/msamsami/qna-builder',
     long_description=codecs.open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

