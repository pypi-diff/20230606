# Comparing `tmp/hojichar-0.4.0.tar.gz` & `tmp/hojichar-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.4.0.tar", max compression
+gzip compressed data, was "hojichar-0.5.0.tar", max compression
```

## Comparing `hojichar-0.4.0.tar` & `hojichar-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-04-04 06:42:31.685857 hojichar-0.4.0/LICENSE
--rw-r--r--   0        0        0     2983 2023-04-04 06:42:31.685857 hojichar-0.4.0/README.md
--rw-r--r--   0        0        0      534 2023-04-04 06:42:56.001637 hojichar-0.4.0/hojichar/__init__.py
--rw-r--r--   0        0        0       42 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/core/__init__.py
--rw-r--r--   0        0        0     4504 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/core/composition.py
--rw-r--r--   0        0        0     3122 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     5031 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/core/inspection.py
--rw-r--r--   0        0        0      884 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-04-04 06:42:31.693857 hojichar-0.4.0/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    11980 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    20767 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1572 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2520 2023-04-04 06:42:31.697857 hojichar-0.4.0/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0     1501 2023-04-04 06:42:56.001637 hojichar-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 hojichar-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 08:34:59.514107 hojichar-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6564 2023-06-06 08:34:59.514107 hojichar-0.5.0/README.md
+-rw-r--r--   0        0        0      534 2023-06-06 08:35:23.373245 hojichar-0.5.0/hojichar/__init__.py
+-rw-r--r--   0        0        0     2715 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/__main__.py
+-rw-r--r--   0        0        0       42 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     4504 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/core/composition.py
+-rw-r--r--   0        0        0     3122 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     5031 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/core/inspection.py
+-rw-r--r--   0        0        0      884 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    11980 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    21705 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1572 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2520 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0     1716 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3335 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1299 2023-06-06 08:34:59.522107 hojichar-0.5.0/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1560 2023-06-06 08:35:23.369245 hojichar-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 hojichar-0.5.0/PKG-INFO
```

### Comparing `hojichar-0.4.0/LICENSE` & `hojichar-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/__init__.py` & `hojichar-0.5.0/hojichar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.4.0"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.5.0"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "Compose",
     "Filter",
     "TokenFilter",
```

### Comparing `hojichar-0.4.0/hojichar/core/composition.py` & `hojichar-0.5.0/hojichar/core/composition.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/core/filter_interface.py` & `hojichar-0.5.0/hojichar/core/filter_interface.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/core/inspection.py` & `hojichar-0.5.0/hojichar/core/inspection.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/core/models.py` & `hojichar-0.5.0/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.5.0/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.5.0/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.5.0/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.5.0/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.5.0/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/filters/__init__.py` & `hojichar-0.5.0/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/filters/deduplication.py` & `hojichar-0.5.0/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/filters/document_filters.py` & `hojichar-0.5.0/hojichar/filters/document_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import pathlib
 import re
+import time
 import unicodedata
 
 import hojichar
 from hojichar.core.filter_interface import Filter
 from hojichar.core.models import Document, Token
 
 BASE_PATH = pathlib.Path(hojichar.__path__[0])
@@ -79,14 +80,32 @@
         """
         if document.is_rejected:
             document.text = ""
 
         return document
 
 
+class Sleep(Filter):
+    """
+    デバッグ用のフィルタです. 指定秒スリープします.
+    """
+
+    def __init__(self, time: float = 1.0, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.time = time
+
+    def apply(self, document):
+        """
+        >>> Sleep(0.1)('hello')  # After 0.1 seconds,
+        'hello'
+        """
+        time.sleep(self.time)
+        return document
+
+
 class DocumentNormalizer(Filter):
     """
     Unicode の正規化をします.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -138,14 +157,30 @@
                 return document
             else:
                 raise e
 
         return document
 
 
+class JSONDumper(Filter):
+    """
+    Doucment.text の値を, エントリ名が "text" という名前の Json に格納します.
+    出力が json lines 欲しいときに Compose の出力前に使用します.
+    """
+
+    def apply(self, document: Document) -> Document:
+        """
+        >>> JSONDumper()("hojichar")
+        '{"text": "hojichar"}'
+        """
+        text = document.text
+        document.text = json.dumps({"text": text}, ensure_ascii=False)
+        return document
+
+
 class DocumentLengthFilter(Filter):
     """
     `min_doc_len`, `max_doc_len` で指定した上限・下限の範囲内にないドキュメントを破棄します.
     デフォルトでは 200字 以上 50000字以内のテキストが受理されます.
     """
 
     def __init__(self, min_doc_len=None, max_doc_len=None, *args, **kwargs):
```

### Comparing `hojichar-0.4.0/hojichar/filters/token_filters.py` & `hojichar-0.5.0/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/hojichar/filters/tokenization.py` & `hojichar-0.5.0/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.4.0/pyproject.toml` & `hojichar-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.4.0" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.5.0" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
 
+[tool.poetry.scripts]
+hojichar = "hojichar.__main__:main"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.23.4"
 mmh3 = "^3.0.0"
 
 [tool.poetry.group.dev]
 optional = true
```

