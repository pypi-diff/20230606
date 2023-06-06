# Comparing `tmp/apiiif-0.0.4.tar.gz` & `tmp/apiiif-0.0.5.tar.gz`

## Comparing `apiiif-0.0.4.tar` & `apiiif-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/__init__.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/factory.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.4/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.4/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/factory.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 apiiif-0.0.5/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.5/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.5/PKG-INFO
```

### Comparing `apiiif-0.0.4/src/apiiif/factory.py` & `apiiif-0.0.5/src/apiiif/factory.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.4/src/apiiif/resource_properties.py` & `apiiif-0.0.5/src/apiiif/resource_properties.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.4/src/apiiif/resource_types.py` & `apiiif-0.0.5/src/apiiif/resource_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,17 @@
         elif isinstance(self.body, Choice):
             self.body.items.append(image)
         else:
             self.body = Choice(items=[self.body, image])
 
 
 class AnnotationPage(BaseModel):
-    context: str = Field('http://iiif.io/api/presentation/3/context.json',
-                         alias='@context')
+    context: str = Field(
+        default='http://iiif.io/api/presentation/3/context.json',
+        alias='@context')
     id: AnyUrl
     type: str = 'AnnotationPage'
     items: list[Annotation] = []
 
     def add_annotation(self, annotation: Annotation):
         self.items.append(annotation)
 
@@ -57,16 +58,17 @@
 # Range should be defined here, but the collections site does not yet support it.
 # Use a range for creating a table of contents within the client (Mirador viewer).
 # For example, printed books could be broken into chapters, and manuscripts could
 # be devided into books or major sections since many manuscripts have non-biblical texts
 
 
 class Manifest(BaseModel):
-    context: str = Field('http://iiif.io/api/presentation/3/context.json',
-                         alias='@context')
+    context: str = Field(
+        default='http://iiif.io/api/presentation/3/context.json',
+        alias='@context')
     id: AnyUrl
     type: str = 'Manifest'
     label: LanguageString
     metadata: list[LabelValue] = []
     summary: LanguageString | None
     thumbnail: Thumbnail | None
     viewingDirection: str = 'left-to-right'
@@ -79,16 +81,17 @@
     items: list = []
 
     def add_canvas(self, canvas: Canvas):
         self.items.append(canvas)
 
 
 class Collection(BaseModel):
-    context: str = Field('http://iiif.io/api/presentation/3/context.json',
-                         alias='@context')
+    context: str = Field(
+        default='http://iiif.io/api/presentation/3/context.json',
+        alias='@context')
     id: AnyUrl
     type: str = 'Collection'
     label: LanguageString
     requiredStatement: LabelValue | None
     items: list = []
 
     def add_manifest(self, manifest: Manifest):
```

### Comparing `apiiif-0.0.4/.gitignore` & `apiiif-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.4/LICENSE.txt` & `apiiif-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.4/README.md` & `apiiif-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.4/pyproject.toml` & `apiiif-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.4/PKG-INFO` & `apiiif-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

