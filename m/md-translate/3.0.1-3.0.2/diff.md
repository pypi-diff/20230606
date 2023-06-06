# Comparing `tmp/md_translate-3.0.1.tar.gz` & `tmp/md_translate-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_translate-3.0.1.tar", max compression
+gzip compressed data, was "md_translate-3.0.2.tar", max compression
```

## Comparing `md_translate-3.0.1.tar` & `md_translate-3.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-03 19:58:43.303453 md_translate-3.0.1/LICENSE
--rw-r--r--   0        0        0     5353 2023-06-03 19:58:43.303453 md_translate-3.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/__init__.py
--rw-r--r--   0        0        0     4457 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/application.py
--rw-r--r--   0        0        0      230 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/blocks.py
--rw-r--r--   0        0        0     5960 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/document.py
--rw-r--r--   0        0        0     3654 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/parser.py
--rw-r--r--   0        0        0      905 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/exceptions.py
--rw-r--r--   0        0        0      737 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/main.py
--rw-r--r--   0        0        0      157 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/settings/__init__.py
--rw-r--r--   0        0        0     5909 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/settings/_base_settings.py
--rw-r--r--   0        0        0     2687 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/settings/_settings_to_cli.py
--rw-r--r--   0        0        0      439 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/__init__.py
--rw-r--r--   0        0        0      687 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/_base_translator.py
--rw-r--r--   0        0        0     4960 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/_selenium_base.py
--rw-r--r--   0        0        0     1517 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/bing.py
--rw-r--r--   0        0        0     2059 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/deepl.py
--rw-r--r--   0        0        0     1839 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/google.py
--rw-r--r--   0        0        0        0 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/randomizer/__init__.py
--rw-r--r--   0        0        0     6618 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/randomizer/const.py
--rw-r--r--   0        0        0     1107 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/randomizer/randomizer.py
--rw-r--r--   0        0        0     1675 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/yandex.py
--rw-r--r--   0        0        0     2214 2023-06-03 19:58:43.303453 md_translate-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 md_translate-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-06 15:27:15.366243 md_translate-3.0.2/LICENSE
+-rw-r--r--   0        0        0     5353 2023-06-06 15:27:15.366243 md_translate-3.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/__init__.py
+-rw-r--r--   0        0        0     4457 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/application.py
+-rw-r--r--   0        0        0      230 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/blocks.py
+-rw-r--r--   0        0        0     5960 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/document.py
+-rw-r--r--   0        0        0     3654 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/document/parser.py
+-rw-r--r--   0        0        0      905 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/exceptions.py
+-rw-r--r--   0        0        0      737 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/main.py
+-rw-r--r--   0        0        0      157 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/settings/__init__.py
+-rw-r--r--   0        0        0     5931 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/settings/_base_settings.py
+-rw-r--r--   0        0        0     2687 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/settings/_settings_to_cli.py
+-rw-r--r--   0        0        0      439 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/__init__.py
+-rw-r--r--   0        0        0      687 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/_base_translator.py
+-rw-r--r--   0        0        0     4960 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/_selenium_base.py
+-rw-r--r--   0        0        0     1517 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/bing.py
+-rw-r--r--   0        0        0     2059 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/deepl.py
+-rw-r--r--   0        0        0     1839 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/google.py
+-rw-r--r--   0        0        0        0 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/randomizer/__init__.py
+-rw-r--r--   0        0        0     6618 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/randomizer/const.py
+-rw-r--r--   0        0        0     1107 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/randomizer/randomizer.py
+-rw-r--r--   0        0        0     1675 2023-06-06 15:27:15.366243 md_translate-3.0.2/md_translate/translators/yandex.py
+-rw-r--r--   0        0        0     2214 2023-06-06 15:27:15.366243 md_translate-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 md_translate-3.0.2/PKG-INFO
```

### Comparing `md_translate-3.0.1/LICENSE` & `md_translate-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/README.md` & `md_translate-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/application.py` & `md_translate-3.0.2/md_translate/application.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/document/blocks.py` & `md_translate-3.0.2/md_translate/document/blocks.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/document/document.py` & `md_translate-3.0.2/md_translate/document/document.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/document/parser.py` & `md_translate-3.0.2/md_translate/document/parser.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/exceptions.py` & `md_translate-3.0.2/md_translate/exceptions.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/main.py` & `md_translate-3.0.2/md_translate/main.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/settings/_base_settings.py` & `md_translate-3.0.2/md_translate/settings/_base_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
     @classmethod
     def __get_not_default_params(cls, params: dict[str, Any]) -> dict[str, Any]:
         not_default_params = {}
         for option_name, value in params.items():
             if option_name not in cls.__fields__:
                 raise ValueError(f'Unknown option: {option_name}')
-            if value != cls.__fields__[option_name].default:
+            if value != cls.__fields__[option_name].default and value is not None:
                 not_default_params[option_name] = value
         return not_default_params
 
     def dump_settings(self) -> None:
         print(
             self.json(
                 indent=4,
```

### Comparing `md_translate-3.0.1/md_translate/settings/_settings_to_cli.py` & `md_translate-3.0.2/md_translate/settings/_settings_to_cli.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/_base_translator.py` & `md_translate-3.0.2/md_translate/translators/_base_translator.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/_selenium_base.py` & `md_translate-3.0.2/md_translate/translators/_selenium_base.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/bing.py` & `md_translate-3.0.2/md_translate/translators/bing.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/deepl.py` & `md_translate-3.0.2/md_translate/translators/deepl.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/google.py` & `md_translate-3.0.2/md_translate/translators/google.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/randomizer/const.py` & `md_translate-3.0.2/md_translate/translators/randomizer/const.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/randomizer/randomizer.py` & `md_translate-3.0.2/md_translate/translators/randomizer/randomizer.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/md_translate/translators/yandex.py` & `md_translate-3.0.2/md_translate/translators/yandex.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.1/pyproject.toml` & `md_translate-3.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md_translate"
-version = "3.0.1"
+version = "3.0.2"
 description = "CLI tool to translate markdown files"
 authors = ["Ilya Chichak <ilyachch@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/ilyachch/md_docs-trans-app"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `md_translate-3.0.1/PKG-INFO` & `md_translate-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-translate
-Version: 3.0.1
+Version: 3.0.2
 Summary: CLI tool to translate markdown files
 Home-page: https://github.com/ilyachch/md_docs-trans-app
 License: MIT
 Author: Ilya Chichak
 Author-email: ilyachch@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

