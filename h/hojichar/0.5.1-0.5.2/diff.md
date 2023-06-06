# Comparing `tmp/hojichar-0.5.1.tar.gz` & `tmp/hojichar-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.5.1.tar", max compression
+gzip compressed data, was "hojichar-0.5.2.tar", max compression
```

## Comparing `hojichar-0.5.1.tar` & `hojichar-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-06-06 08:38:11.799020 hojichar-0.5.1/LICENSE
--rw-r--r--   0        0        0    11137 2023-06-06 08:38:11.799020 hojichar-0.5.1/README.md
--rw-r--r--   0        0        0      534 2023-06-06 08:38:35.763343 hojichar-0.5.1/hojichar/__init__.py
--rw-r--r--   0        0        0     2715 2023-06-06 08:38:11.799020 hojichar-0.5.1/hojichar/__main__.py
--rw-r--r--   0        0        0       42 2023-06-06 08:38:11.799020 hojichar-0.5.1/hojichar/core/__init__.py
--rw-r--r--   0        0        0     4504 2023-06-06 08:38:11.799020 hojichar-0.5.1/hojichar/core/composition.py
--rw-r--r--   0        0        0     3122 2023-06-06 08:38:11.799020 hojichar-0.5.1/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     5031 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/core/inspection.py
--rw-r--r--   0        0        0      884 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    11980 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    21705 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1572 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2520 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0      595 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3335 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1299 2023-06-06 08:38:11.803020 hojichar-0.5.1/hojichar/utils/process.py
--rw-r--r--   0        0        0     1560 2023-06-06 08:38:35.763343 hojichar-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11881 1970-01-01 00:00:00.000000 hojichar-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 09:25:45.483870 hojichar-0.5.2/LICENSE
+-rw-r--r--   0        0        0    11137 2023-06-06 09:25:45.483870 hojichar-0.5.2/README.md
+-rw-r--r--   0        0        0      534 2023-06-06 09:26:12.123529 hojichar-0.5.2/hojichar/__init__.py
+-rw-r--r--   0        0        0     2761 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/__main__.py
+-rw-r--r--   0        0        0       42 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     4504 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/core/composition.py
+-rw-r--r--   0        0        0     3122 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     5031 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/core/inspection.py
+-rw-r--r--   0        0        0      884 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    11980 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    21705 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1572 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2520 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0      595 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3335 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1299 2023-06-06 09:25:45.487870 hojichar-0.5.2/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1560 2023-06-06 09:26:12.123529 hojichar-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    11881 1970-01-01 00:00:00.000000 hojichar-0.5.2/PKG-INFO
```

### Comparing `hojichar-0.5.1/LICENSE` & `hojichar-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/README.md` & `hojichar-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/__init__.py` & `hojichar-0.5.2/hojichar/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.5.1"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.5.2"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "Compose",
     "Filter",
     "TokenFilter",
```

### Comparing `hojichar-0.5.1/hojichar/__main__.py` & `hojichar-0.5.2/hojichar/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         default=None,
         help="Specifies the path for the output file. Defaults to standard output.",
     )
     parser.add_argument(
         "--dump-stats",
         default=None,
         metavar="<path to stats.json>",
-        help="Dump statistics to a file.",
+        help="Dump statistics to file. If the file exists, it will be appended.",
     )
     parser.add_argument(
         "--exit-on-error",
         action="store_true",
         help="Exit if an exception occurs during filtering.\
             Useful for debugging custom filters.",
     )
@@ -88,13 +88,13 @@
     if args.output:
         with open(args.output, "w") as fp:
             fileout_from_iter(out_str_iter, fp)
     else:
         stdout_from_iter(out_str_iter)
     finalize()
     if args.dump_stats:
-        with open(args.dump_stats, "w") as fp:
-            fp.write(json.dumps(FILTER.statistics))
+        with open(args.dump_stats, "a") as fp:
+            fp.write(json.dumps(FILTER.statistics) + "\n")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hojichar-0.5.1/hojichar/core/composition.py` & `hojichar-0.5.2/hojichar/core/composition.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/core/filter_interface.py` & `hojichar-0.5.2/hojichar/core/filter_interface.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/core/inspection.py` & `hojichar-0.5.2/hojichar/core/inspection.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/core/models.py` & `hojichar-0.5.2/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.5.2/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.5.2/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.5.2/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.5.2/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.5.2/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/filters/__init__.py` & `hojichar-0.5.2/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/filters/deduplication.py` & `hojichar-0.5.2/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/filters/document_filters.py` & `hojichar-0.5.2/hojichar/filters/document_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/filters/token_filters.py` & `hojichar-0.5.2/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/filters/tokenization.py` & `hojichar-0.5.2/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/utils/__init__.py` & `hojichar-0.5.2/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/utils/io_iter.py` & `hojichar-0.5.2/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/utils/load_compose.py` & `hojichar-0.5.2/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/hojichar/utils/process.py` & `hojichar-0.5.2/hojichar/utils/process.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.1/pyproject.toml` & `hojichar-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.5.1" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.5.2" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
```

### Comparing `hojichar-0.5.1/PKG-INFO` & `hojichar-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.5.1
+Version: 0.5.2
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

