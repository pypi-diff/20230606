# Comparing `tmp/apiiif-0.0.2.tar.gz` & `tmp/apiiif-0.0.3.tar.gz`

## Comparing `apiiif-0.0.2.tar` & `apiiif-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/__init__.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/factory.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.2/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.2/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/factory.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.3/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.3/PKG-INFO
```

### Comparing `apiiif-0.0.2/src/apiiif/factory.py` & `apiiif-0.0.3/src/apiiif/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 
     def __init__(self, auto_language: str = 'en'):
         self.auto_language = auto_language
 
     def langugae_string(self, message: str):
         return LanguageString(**{self.auto_language: [message]})
 
-    def requiredStatement(self, label: str, value: str):
+    def label_value(self, label: str, value: str):
         return LabelValue(label=self.langugae_string(label),
                           value=self.langugae_string(value))
 
+    def requiredStatement(self, label: str, value: str):
+        return self.label_value(label, value)
+
     def thumbnail(self, url: str, width: int = None, height: int = None):
         return Thumbnail(id=url, width=width, height=height)
 
     def logo(self, url: str, width: int, height: int):
         return Logo(id=url, width=width, height=height)
 
     def homepage(self, url: str, label: str):
```

### Comparing `apiiif-0.0.2/src/apiiif/resource_properties.py` & `apiiif-0.0.3/src/apiiif/resource_properties.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.2/src/apiiif/resource_types.py` & `apiiif-0.0.3/src/apiiif/resource_types.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.2/.gitignore` & `apiiif-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.2/LICENSE.txt` & `apiiif-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.2/README.md` & `apiiif-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.2/pyproject.toml` & `apiiif-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.2/PKG-INFO` & `apiiif-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

