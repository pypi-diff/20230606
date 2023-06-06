# Comparing `tmp/apiiif-0.0.1.tar.gz` & `tmp/apiiif-0.0.2.tar.gz`

## Comparing `apiiif-0.0.1.tar` & `apiiif-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 apiiif-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.1/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.1/src/apiiif/__init__.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 apiiif-0.0.1/src/apiiif/factory.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.1/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 apiiif-0.0.1/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.1/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 apiiif-0.0.1/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 apiiif-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/factory.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 apiiif-0.0.2/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.2/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.2/PKG-INFO
```

### Comparing `apiiif-0.0.1/src/apiiif/factory.py` & `apiiif-0.0.2/src/apiiif/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def langugae_string(self, message: str):
         return LanguageString(**{self.auto_language: [message]})
 
     def requiredStatement(self, label: str, value: str):
         return LabelValue(label=self.langugae_string(label),
                           value=self.langugae_string(value))
 
-    def thumbnail(self, url: str, width: int, height: int):
+    def thumbnail(self, url: str, width: int = None, height: int = None):
         return Thumbnail(id=url, width=width, height=height)
 
     def logo(self, url: str, width: int, height: int):
         return Logo(id=url, width=width, height=height)
 
     def homepage(self, url: str, label: str):
         return Homepage(id=url,
```

### Comparing `apiiif-0.0.1/src/apiiif/resource_properties.py` & `apiiif-0.0.2/src/apiiif/resource_properties.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.1/src/apiiif/resource_types.py` & `apiiif-0.0.2/src/apiiif/resource_types.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.1/.gitignore` & `apiiif-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.1/LICENSE.txt` & `apiiif-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.1/pyproject.toml` & `apiiif-0.0.2/pyproject.toml`

 * *Files identical despite different names*

