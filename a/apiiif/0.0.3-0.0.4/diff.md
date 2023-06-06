# Comparing `tmp/apiiif-0.0.3.tar.gz` & `tmp/apiiif-0.0.4.tar.gz`

## Comparing `apiiif-0.0.3.tar` & `apiiif-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/__init__.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/factory.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 apiiif-0.0.3/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.3/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.3/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/factory.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 apiiif-0.0.4/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 apiiif-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.0.4/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 apiiif-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 apiiif-0.0.4/PKG-INFO
```

### Comparing `apiiif-0.0.3/src/apiiif/factory.py` & `apiiif-0.0.4/src/apiiif/factory.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.3/src/apiiif/resource_properties.py` & `apiiif-0.0.4/src/apiiif/resource_properties.py`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.3/src/apiiif/resource_types.py` & `apiiif-0.0.4/src/apiiif/resource_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 class IIIFImage(Image):
     format: str = 'image/jpeg'
     # as other services are defined, add them as options.
     service: list[ImageService] = []
 
 
 class Annotation(BaseModel):
-    context: str = Field('http://iiif.io/api/presentation/3/context.json',
-                         alias='@context')
+    context: str = Field(
+        default='http://iiif.io/api/presentation/3/context.json',
+        alias='@context')
     id: AnyUrl
     type: str = 'Annotation'
     motivation: str = 'painting'
     target: AnyUrl
     body: IIIFImage | Choice | None = None
 
     def add_image(self, image: IIIFImage):
```

### Comparing `apiiif-0.0.3/.gitignore` & `apiiif-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.3/LICENSE.txt` & `apiiif-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.3/README.md` & `apiiif-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.3/pyproject.toml` & `apiiif-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apiiif-0.0.3/PKG-INFO` & `apiiif-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

