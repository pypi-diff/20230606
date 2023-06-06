# Comparing `tmp/textarium-0.1.2.tar.gz` & `tmp/textarium-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textarium-0.1.2.tar", max compression
+gzip compressed data, was "textarium-0.1.3.tar", max compression
```

## Comparing `textarium-0.1.2.tar` & `textarium-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-06-05 15:11:50.925595 textarium-0.1.2/LICENSE
--rw-r--r--   0        0        0     1486 2023-06-05 15:11:50.925595 textarium-0.1.2/README.md
--rw-r--r--   0        0        0      602 2023-06-05 15:11:50.929596 textarium-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/.DS_Store
--rw-r--r--   0        0        0     1829 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/__init__.py
--rw-r--r--   0        0        0     5229 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/en_stopwords.txt
--rw-r--r--   0        0        0     4536 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/ru_stopwords.txt
--rw-r--r--   0        0        0      305 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/collections/stopwords.py
--rw-r--r--   0        0        0     1509 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/extraction.py
--rw-r--r--   0        0        0      216 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/models.py
--rw-r--r--   0        0        0     4655 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/preprocessing.py
--rw-r--r--   0        0        0        0 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/__init__.py
--rw-r--r--   0        0        0      283 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test__all__.py
--rw-r--r--   0        0        0      431 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_collections.py
--rw-r--r--   0        0        0     2243 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_extraction.py
--rw-r--r--   0        0        0     2935 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_preprocessing.py
--rw-r--r--   0        0        0     1638 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/tests/test_text.py
--rw-r--r--   0        0        0     1092 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/text.py
--rw-r--r--   0        0        0      567 2023-06-05 15:11:50.929596 textarium-0.1.2/textarium/utils.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 textarium-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-06 20:22:21.061879 textarium-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1486 2023-06-06 20:22:21.065879 textarium-0.1.3/README.md
+-rw-r--r--   0        0        0      602 2023-06-06 20:22:21.065879 textarium-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/.DS_Store
+-rw-r--r--   0        0        0     1870 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/__init__.py
+-rw-r--r--   0        0        0     5229 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/en_stopwords.txt
+-rw-r--r--   0        0        0     4536 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/ru_stopwords.txt
+-rw-r--r--   0        0        0      305 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/stopwords.py
+-rw-r--r--   0        0        0      786 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/corpus.py
+-rw-r--r--   0        0        0     1509 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/extraction.py
+-rw-r--r--   0        0        0      216 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/models.py
+-rw-r--r--   0        0        0     4655 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test__all__.py
+-rw-r--r--   0        0        0      415 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_collections.py
+-rw-r--r--   0        0        0      809 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_corpus.py
+-rw-r--r--   0        0        0     2243 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_extraction.py
+-rw-r--r--   0        0        0     2935 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     1638 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_text.py
+-rw-r--r--   0        0        0     1092 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/text.py
+-rw-r--r--   0        0        0      567 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/utils.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 textarium-0.1.3/PKG-INFO
```

### Comparing `textarium-0.1.2/LICENSE` & `textarium-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/README.md` & `textarium-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 
 s = "This a text example. You can preprocess and analyze it with this package."
 text = Text(s, lang='en')
 text.prepare()
 
 print(text.prepared_text)
 ```
-## License
-[MIT](LICENSE)
 
 ## Documentation
-The official documentation is hosted on Github.io: https://6b656b.github.io/textarium
+The official documentation is hosted on Github.io: https://6b656b.github.io/textarium
+## License
+[MIT](LICENSE)
```

### Comparing `textarium-0.1.2/pyproject.toml` & `textarium-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textarium"
-version = "0.1.2"
+version = "0.1.3"
 description = "Textarium is a Python package for text analysis"
 authors = ["6b656b"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `textarium-0.1.2/textarium/.DS_Store` & `textarium-0.1.3/textarium/.DS_Store`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/__init__.py` & `textarium-0.1.3/textarium/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     remove_punctuation,
     remove_urls,
     remove_words,
     make_lowercase,
     lemmatize
 )
 from .text import Text
+from .corpus import Corpus
 
 __all__ = [
     "extract_words",
     "extract_urls",
     "extract_sentences",
     "remove_extra_spaces",
     "remove_charset",
@@ -65,8 +66,9 @@
     "remove_html",
     "remove_punctuation",
     "remove_urls",
     "remove_words",
     "make_lowercase",
     "lemmatize",
     "Text",
+    "Corpus",
 ]
```

### Comparing `textarium-0.1.2/textarium/collections/en_stopwords.txt` & `textarium-0.1.3/textarium/collections/en_stopwords.txt`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/collections/ru_stopwords.txt` & `textarium-0.1.3/textarium/collections/ru_stopwords.txt`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/extraction.py` & `textarium-0.1.3/textarium/extraction.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/preprocessing.py` & `textarium-0.1.3/textarium/preprocessing.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/tests/test_extraction.py` & `textarium-0.1.3/textarium/tests/test_extraction.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/tests/test_preprocessing.py` & `textarium-0.1.3/textarium/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/tests/test_text.py` & `textarium-0.1.3/textarium/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/textarium/text.py` & `textarium-0.1.3/textarium/text.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 """
 
 from typing import List
 from textarium.utils import pipeline
 import textarium.preprocessing as tp
 
 class Text:
-    def __init__(self, text: str, lang: str = 'ru'):
+    def __init__(self, text: str, lang: str = 'en'):
+        self.lang = lang
         self.raw_text = text
         self.prepared_text = None
-        self.lang = lang
 
     def prepare(self, lemmatize: bool = True, stopwords: List[str] = None):
         """Prepares text for analysis and ML modeling:
             - Removes punctuation, digits and extra spaces
             - Removes stopwords, html-tags and urls
             - Lemmatizes all words
```

### Comparing `textarium-0.1.2/textarium/utils.py` & `textarium-0.1.3/textarium/utils.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.2/PKG-INFO` & `textarium-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textarium
-Version: 0.1.2
+Version: 0.1.3
 Summary: Textarium is a Python package for text analysis
 License: MIT
 Author: 6b656b
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -50,12 +50,12 @@
 
 s = "This a text example. You can preprocess and analyze it with this package."
 text = Text(s, lang='en')
 text.prepare()
 
 print(text.prepared_text)
 ```
-## License
-[MIT](LICENSE)
 
 ## Documentation
 The official documentation is hosted on Github.io: https://6b656b.github.io/textarium
+## License
+[MIT](LICENSE)
```

