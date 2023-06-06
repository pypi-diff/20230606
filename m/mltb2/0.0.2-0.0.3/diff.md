# Comparing `tmp/mltb2-0.0.2.tar.gz` & `tmp/mltb2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.0.2.tar", last modified: Sat Jun  3 05:17:09 2023, max compression
+gzip compressed data, was "mltb2-0.0.3.tar", last modified: Tue Jun  6 09:57:04 2023, max compression
```

## Comparing `mltb2-0.0.2.tar` & `mltb2-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-03 05:16:55.000000 mltb2-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 05:16:55.000000 mltb2-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 05:17:09.056301 mltb2-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-03 05:16:55.000000 mltb2-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-03 05:16:55.000000 mltb2-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-03 05:17:09.056301 mltb2-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-03 05:16:55.000000 mltb2-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 09:56:55.000000 mltb2-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 09:56:55.000000 mltb2-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 09:57:04.926392 mltb2-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-06 09:56:55.000000 mltb2-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-06 09:56:55.000000 mltb2-0.0.3/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 09:57:04.000000 mltb2-0.0.3/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-06 09:56:55.000000 mltb2-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-06 09:57:04.926392 mltb2-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-06 09:56:55.000000 mltb2-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:57:04.926392 mltb2-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 09:56:55.000000 mltb2-0.0.3/tests/test_transformers.py
```

### Comparing `mltb2-0.0.2/LICENSE` & `mltb2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.2/PKG-INFO` & `mltb2-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
@@ -31,49 +31,49 @@
 Provides-Extra: checking
 Provides-Extra: optional
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
 
-# Machine Learning Toolbox 2 - MLTB2 - [Sphinx DOC](https://telekom.github.io/mltb2/)
+# Machine Learning Toolbox 2 - MLTB2
 
 [![MIT License](https://img.shields.io/github/license/telekom/mltb2)](https://github.com/telekom/mltb2/blob/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/mltb2)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/mltb2.svg)](https://pypi.python.org/pypi/mltb2)
 <br/>
 [![pytest](https://github.com/telekom/mltb2/actions/workflows/pytest.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/pytest.yml)
 [![Static Code Checks](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml)
 [![Build & Deploy Doc](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml)
 [![GitHub issues](https://img.shields.io/github/issues-raw/telekom/mltb2)](https://github.com/telekom/mltb2/issues)
 
 📦 A box of machine learning tools. 📦
 
-## Main Components
+## Components and Documentation
 
-[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/code-doc/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
+[Documentation Page](https://telekom.github.io/mltb2/)
+
+[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
 Split texts into sentences. For German and English language.
 This is done with the [SoMaJo](https://github.com/tsproisl/SoMaJo) tool.
 
-[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/code-doc/somajo.html#mltb2.somajo.JaccardSimilarity)\
+[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.JaccardSimilarity)\
 Calculate the [jaccard similarity](https://en.wikipedia.org/wiki/Jaccard_index).
 
-[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/code-doc/transformers.html#mltb2.transformers.TransformersTokenCounter)\
+[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/api-reference/transformers.html#mltb2.transformers.TransformersTokenCounter)\
 Count tokens made by a [Transformers](https://github.com/huggingface/transformers) tokenizer.
 
-[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/code-doc/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
+[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/api-reference/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
 Split the text into sections with a specified maximum token length.
 Does not divide words, but always whole sentences.
 
-[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/code-doc/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
+[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/api-reference/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
 An [Optuna pruner](https://optuna.readthedocs.io/en/stable/reference/pruners.html)
 to use statistical significance (a t-test which serves as a heuristic) to stop
 unpromising trials early, avoiding unnecessary repeated training during cross validation.
-Furthermore, there is a
-[detailed description and an example of use](https://telekom.github.io/mltb2/doc/SignificanceRepeatedTrainingPruner.html).
 
 ## Installation
 
 MLTB2 is available at [the Python Package Index (PyPI)](https://pypi.org/project/mltb2/).
 It can be installed with pip:
 
 ```bash
```

### Comparing `mltb2-0.0.2/README.md` & `mltb2-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Machine Learning Toolbox 2 - MLTB2 - [Sphinx DOC](https://telekom.github.io/mltb2/)
+# Machine Learning Toolbox 2 - MLTB2
 
 [![MIT License](https://img.shields.io/github/license/telekom/mltb2)](https://github.com/telekom/mltb2/blob/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/mltb2)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/mltb2.svg)](https://pypi.python.org/pypi/mltb2)
 <br/>
 [![pytest](https://github.com/telekom/mltb2/actions/workflows/pytest.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/pytest.yml)
 [![Static Code Checks](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml)
 [![Build & Deploy Doc](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml)
 [![GitHub issues](https://img.shields.io/github/issues-raw/telekom/mltb2)](https://github.com/telekom/mltb2/issues)
 
 📦 A box of machine learning tools. 📦
 
-## Main Components
+## Components and Documentation
 
-[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/code-doc/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
+[Documentation Page](https://telekom.github.io/mltb2/)
+
+[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
 Split texts into sentences. For German and English language.
 This is done with the [SoMaJo](https://github.com/tsproisl/SoMaJo) tool.
 
-[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/code-doc/somajo.html#mltb2.somajo.JaccardSimilarity)\
+[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.JaccardSimilarity)\
 Calculate the [jaccard similarity](https://en.wikipedia.org/wiki/Jaccard_index).
 
-[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/code-doc/transformers.html#mltb2.transformers.TransformersTokenCounter)\
+[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/api-reference/transformers.html#mltb2.transformers.TransformersTokenCounter)\
 Count tokens made by a [Transformers](https://github.com/huggingface/transformers) tokenizer.
 
-[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/code-doc/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
+[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/api-reference/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
 Split the text into sections with a specified maximum token length.
 Does not divide words, but always whole sentences.
 
-[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/code-doc/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
+[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/api-reference/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
 An [Optuna pruner](https://optuna.readthedocs.io/en/stable/reference/pruners.html)
 to use statistical significance (a t-test which serves as a heuristic) to stop
 unpromising trials early, avoiding unnecessary repeated training during cross validation.
-Furthermore, there is a
-[detailed description and an example of use](https://telekom.github.io/mltb2/doc/SignificanceRepeatedTrainingPruner.html).
 
 ## Installation
 
 MLTB2 is available at [the Python Package Index (PyPI)](https://pypi.org/project/mltb2/).
 It can be installed with pip:
 
 ```bash
```

### Comparing `mltb2-0.0.2/mltb2/somajo.py` & `mltb2-0.0.3/mltb2/somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.2/mltb2/somajo_transformers.py` & `mltb2-0.0.3/mltb2/somajo_transformers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2023 Philip May
+# Copyright (c) 2023 Philip May, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """SoMaJo and Transformers tools."""
 
 
 from dataclasses import dataclass
@@ -21,20 +22,24 @@
     Does not divide words, but always whole sentences.
 
     Args:
         max_token: Maximum number of tokens per text section.
         somajo_sentence_splitter: The sentence splitter to be used.
         transformers_token_counter: The token counter to be used.
         show_progress_bar: Show a progressbar during processing.
+        ignore_overly_long_sentences: If this is ``False`` an ``ValueError`` exception is
+            raised if a sentence is longer than ``max_token``.
+            If it is true, then the sentence is simply ignored.
     """
 
     max_token: int
     somajo_sentence_splitter: SoMaJoSentenceSplitter
     transformers_token_counter: TransformersTokenCounter
     show_progress_bar: bool = True
+    ignore_overly_long_sentences: bool = False
 
     def __call__(self, text: str) -> List[str]:
         """Split the text into sections.
 
         Args:
             text: The text to be split.
         Returns:
@@ -48,15 +53,18 @@
         result_splits: List[str] = []
         current_sentences: List[str] = []
         current_count: int = 0
         for sentence, count in zip(
             tqdm(sentences, disable=not self.show_progress_bar), counts  # type: ignore
         ):
             if count > self.max_token:
-                raise ValueError("No sentence may be longer than 'max_token'.")
+                if self.ignore_overly_long_sentences:
+                    continue
+                else:
+                    raise ValueError("No sentence may be longer than 'max_token'.")
             if current_count + count <= self.max_token:
                 current_count += count
                 current_sentences.append(sentence)
             else:
                 result_split = " ".join(current_sentences)
                 result_splits.append(result_split)
                 current_sentences = []
```

### Comparing `mltb2-0.0.2/mltb2/transformers.py` & `mltb2-0.0.3/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.2/mltb2.egg-info/PKG-INFO` & `mltb2-0.0.3/mltb2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
@@ -31,49 +31,49 @@
 Provides-Extra: checking
 Provides-Extra: optional
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
 
-# Machine Learning Toolbox 2 - MLTB2 - [Sphinx DOC](https://telekom.github.io/mltb2/)
+# Machine Learning Toolbox 2 - MLTB2
 
 [![MIT License](https://img.shields.io/github/license/telekom/mltb2)](https://github.com/telekom/mltb2/blob/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/mltb2)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/mltb2.svg)](https://pypi.python.org/pypi/mltb2)
 <br/>
 [![pytest](https://github.com/telekom/mltb2/actions/workflows/pytest.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/pytest.yml)
 [![Static Code Checks](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/static_checks.yml)
 [![Build & Deploy Doc](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml/badge.svg)](https://github.com/telekom/mltb2/actions/workflows/build_deploy_doc.yml)
 [![GitHub issues](https://img.shields.io/github/issues-raw/telekom/mltb2)](https://github.com/telekom/mltb2/issues)
 
 📦 A box of machine learning tools. 📦
 
-## Main Components
+## Components and Documentation
 
-[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/code-doc/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
+[Documentation Page](https://telekom.github.io/mltb2/)
+
+[`from mltb2.somajo import SoMaJoSentenceSplitter`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.SoMaJoSentenceSplitter)\
 Split texts into sentences. For German and English language.
 This is done with the [SoMaJo](https://github.com/tsproisl/SoMaJo) tool.
 
-[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/code-doc/somajo.html#mltb2.somajo.JaccardSimilarity)\
+[`from mltb2.somajo import JaccardSimilarity`](https://telekom.github.io/mltb2/api-reference/somajo.html#mltb2.somajo.JaccardSimilarity)\
 Calculate the [jaccard similarity](https://en.wikipedia.org/wiki/Jaccard_index).
 
-[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/code-doc/transformers.html#mltb2.transformers.TransformersTokenCounter)\
+[`from mltb2.transformers import TransformersTokenCounter`](https://telekom.github.io/mltb2/api-reference/transformers.html#mltb2.transformers.TransformersTokenCounter)\
 Count tokens made by a [Transformers](https://github.com/huggingface/transformers) tokenizer.
 
-[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/code-doc/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
+[`from mltb2.somajo_transformers import TextSplitter`](https://telekom.github.io/mltb2/api-reference/somajo_transformers.html#mltb2.somajo_transformers.TextSplitter)\
 Split the text into sections with a specified maximum token length.
 Does not divide words, but always whole sentences.
 
-[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/code-doc/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
+[`from mltb2.optuna import SignificanceRepeatedTrainingPruner`](https://telekom.github.io/mltb2/api-reference/optuna.html#mltb2.optuna.SignificanceRepeatedTrainingPruner)\
 An [Optuna pruner](https://optuna.readthedocs.io/en/stable/reference/pruners.html)
 to use statistical significance (a t-test which serves as a heuristic) to stop
 unpromising trials early, avoiding unnecessary repeated training during cross validation.
-Furthermore, there is a
-[detailed description and an example of use](https://telekom.github.io/mltb2/doc/SignificanceRepeatedTrainingPruner.html).
 
 ## Installation
 
 MLTB2 is available at [the Python Package Index (PyPI)](https://pypi.org/project/mltb2/).
 It can be installed with pip:
 
 ```bash
```

### Comparing `mltb2-0.0.2/setup.py` & `mltb2-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.2/tests/test_optuna.py` & `mltb2-0.0.3/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.2/tests/test_somajo.py` & `mltb2-0.0.3/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.2/tests/test_somajo_transformers.py` & `mltb2-0.0.3/tests/test_somajo_transformers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2023 Philip May
+# Copyright (c) 2023 Philip May, Deutsche Telekom AG
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 
 import pytest
 
 from mltb2.somajo import SoMaJoSentenceSplitter
@@ -24,19 +25,37 @@
     assert isinstance(split_text, list)
     assert len(split_text) == 3
     assert split_text[0] == "Satz 0 ist das. Satz 1 ist das."
     assert split_text[1] == "Satz 2 ist das. Satz 3 ist das."
     assert split_text[2] == "Satz 4 ist das."
 
 
-def test_TextSplitter_call_sentence_too_long():
+def test_TextSplitter_call_sentence_too_long_exception():
     somajo_sentence_splitter = SoMaJoSentenceSplitter("de_CMC")
     transformers_token_counter = TransformersTokenCounter("deepset/gbert-base")
     text_splitter = TextSplitter(
         max_token=3,
         somajo_sentence_splitter=somajo_sentence_splitter,
         transformers_token_counter=transformers_token_counter,
     )
     text = " ".join([f"Satz {i} ist das." for i in range(5)])
 
     with pytest.raises(ValueError):
         text_splitter(text)
+
+
+def test_TextSplitter_call_sentence_too_long_no_exception():
+    somajo_sentence_splitter = SoMaJoSentenceSplitter("de_CMC")
+    transformers_token_counter = TransformersTokenCounter("deepset/gbert-base")
+    text_splitter = TextSplitter(
+        max_token=3,
+        somajo_sentence_splitter=somajo_sentence_splitter,
+        transformers_token_counter=transformers_token_counter,
+        ignore_overly_long_sentences=True,
+    )
+    text = " ".join([f"Satz {i} ist das." for i in range(5)])
+    text = f"{text} Ja!"
+    split_text = text_splitter(text)
+
+    assert isinstance(split_text, list)
+    assert len(split_text) == 1
+    assert split_text[0] == "Ja!"
```

### Comparing `mltb2-0.0.2/tests/test_transformers.py` & `mltb2-0.0.3/tests/test_transformers.py`

 * *Files identical despite different names*

