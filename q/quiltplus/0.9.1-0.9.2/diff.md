# Comparing `tmp/quiltplus-0.9.1.tar.gz` & `tmp/quiltplus-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltplus-0.9.1.tar", max compression
+gzip compressed data, was "quiltplus-0.9.2.tar", max compression
```

## Comparing `quiltplus-0.9.1.tar` & `quiltplus-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.1/LICENSE.md
--rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.1/README.md
--rw-r--r--   0        0        0      908 2023-06-03 15:47:57.984367 quiltplus-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      468 2023-06-03 22:59:04.000000 quiltplus-0.9.1/quiltplus/__init__.py
--rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.1/quiltplus/ignore.py
--rw-r--r--   0        0        0     2219 2023-06-03 15:46:39.662073 quiltplus-0.9.1/quiltplus/local.py
--rw-r--r--   0        0        0     3189 2023-06-03 15:46:39.662850 quiltplus-0.9.1/quiltplus/package.py
--rw-r--r--   0        0        0      523 2023-06-03 15:46:39.663694 quiltplus-0.9.1/quiltplus/path.py
--rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.1/quiltplus/property.py
--rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.1/quiltplus/py.typed
--rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.1/quiltplus/registry.py
--rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.1/quiltplus/resource.py
--rw-r--r--   0        0        0      366 2023-05-31 14:03:42.579049 quiltplus-0.9.1/quiltplus/root.py
--rw-r--r--   0        0        0     1186 2023-06-03 15:46:39.667587 quiltplus-0.9.1/quiltplus/type.py
--rw-r--r--   0        0        0     1459 2023-06-03 15:46:39.668475 quiltplus-0.9.1/quiltplus/uri.py
--rw-r--r--   0        0        0      589 2023-06-03 15:46:39.669427 quiltplus-0.9.1/quiltplus/versions.py
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.2/LICENSE.md
+-rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.2/README.md
+-rw-r--r--   0        0        0      908 2023-06-06 02:31:19.767034 quiltplus-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-06-05 00:41:34.765649 quiltplus-0.9.2/quiltplus/__init__.py
+-rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.2/quiltplus/ignore.py
+-rw-r--r--   0        0        0     3697 2023-06-06 02:31:19.767775 quiltplus-0.9.2/quiltplus/local.py
+-rw-r--r--   0        0        0     3960 2023-06-06 02:31:19.768805 quiltplus-0.9.2/quiltplus/package.py
+-rw-r--r--   0        0        0      518 2023-06-06 02:31:19.769900 quiltplus-0.9.2/quiltplus/path.py
+-rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.2/quiltplus/property.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.2/quiltplus/py.typed
+-rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.2/quiltplus/registry.py
+-rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.2/quiltplus/resource.py
+-rw-r--r--   0        0        0      366 2023-05-31 14:03:42.579049 quiltplus-0.9.2/quiltplus/root.py
+-rw-r--r--   0        0        0     1220 2023-06-06 02:31:19.770765 quiltplus-0.9.2/quiltplus/type.py
+-rw-r--r--   0        0        0     1708 2023-06-06 02:31:19.771443 quiltplus-0.9.2/quiltplus/uri.py
+-rw-r--r--   0        0        0      589 2023-06-03 15:46:39.669427 quiltplus-0.9.2/quiltplus/versions.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.2/PKG-INFO
```

### Comparing `quiltplus-0.9.1/LICENSE.md` & `quiltplus-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.1/README.md` & `quiltplus-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.1/pyproject.toml` & `quiltplus-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltplus"
-version = "0.9.1"
+version = "0.9.2"
 description = "Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["yaml", "api", "resource", "quilt"]
 packages = [
    { include = "quiltplus" }
```

### Comparing `quiltplus-0.9.1/quiltplus/ignore.py` & `quiltplus-0.9.2/quiltplus/ignore.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.1/quiltplus/local.py` & `quiltplus-0.9.2/quiltplus/local.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,68 @@
 import logging
 import os
 import platform
 import subprocess
 from collections.abc import Generator
+from filecmp import dircmp
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
+from quilt3.backends import get_package_registry  # type: ignore
+
 from .root import QuiltRoot
 
 
 class QuiltLocal(QuiltRoot):
     @staticmethod
     def TempDir() -> Generator[Path, None, None]:
+        test_dir = os.environ.get("GITHUB_WORKSPACE")
         with TemporaryDirectory(ignore_cleanup_errors=True) as tmpdirname:
             tmpdir = Path(tmpdirname)
-            yield (tmpdir)
+            if not test_dir:
+                # logging.info(f"Creating {tmpdirname} on {platform.system()}")
+                yield tmpdir
+            else:
+                temp_dir = Path(test_dir) / tmpdir.name
+                # logging.info(f"Creating {temp_dir} on {platform.system()}")
+                temp_dir.mkdir(parents=True, exist_ok=True)
+                yield temp_dir
             logging.debug(f"Removing {tmpdirname} on {platform.system()}")
 
     @staticmethod
     def OpenDesktop(dest: str):
         if platform.system() == "Windows":
             os.startfile(dest)  # type: ignore
         elif platform.system() == "Darwin":
             subprocess.Popen(["open", "-R", dest])
         else:
             subprocess.Popen(["xdg-open", dest])
         return dest
 
     def __init__(self, attrs: dict):
         super().__init__(attrs)
+        self.local_registry = get_package_registry()
         for tmp in QuiltLocal.TempDir():
+            logging.info(f"Package using QuiltLocal.TempDir: {tmp}")
             self.last_path = tmp
 
     def check_dir(self, path: Path | None = None):
         if not path:
             return self.last_path
 
         self.last_path = path
         if not path.exists():
-            logging.warn(f"Path does not exist: {path}")
+            logging.warning(f"Path does not exist: {path}")
             path.mkdir(parents=True, exist_ok=True)
         elif not path.is_dir():
             raise ValueError(f"Path is not a directory: {path}")
         return path
 
     def check_path(self, opts: dict):
         path = opts.get(QuiltLocal.K_PTH)
-        print(path)
         return self.check_dir(path)
 
     def local_path(self, *paths: str):
         p = self.check_dir()
         for path in paths:
             p = p / path
 
@@ -64,14 +76,39 @@
             for (dir, dirs, files) in os.walk(root)
             for file in files
         ]
 
     def dest(self):
         return str(self.local_path())  # + "/"
 
+    def local_cache(self) -> Path:
+        base_path = Path(self.local_registry.base.path)
+        if not base_path.exists():
+            logging.warning(f"local_cache does not exist: {base_path}")
+        return base_path / self.package
+
+    def _diff(self) -> dict[str, str]:
+        """Compare files in local_path to local cache"""
+        cache = self.local_cache()
+        if not cache.exists():
+            logging.warning(f"_diff: local_cache[{cache}] does not exist")
+            return {}
+        diff = dircmp(str(cache), self.dest())
+        # logging.debug(f"_diff.diff: {diff}")
+        results = {
+            "add": diff.right_only,
+            "rm": diff.left_only,
+            "touch": diff.diff_files,
+        }
+        return {
+            filename: stage
+            for stage, sublist in results.items()
+            for filename in sublist
+        }
+
     def write_text(self, text: str, file: str, *paths: str):
         dir = self.local_path(*paths)
         p = dir / file
         p.write_text(text)
         return p
 
     def open(self):
```

### Comparing `quiltplus-0.9.1/quiltplus/path.py` & `quiltplus-0.9.2/quiltplus/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 
+from pathlib import Path
+
 from .package import QuiltPackage
 
 
 class QuiltPath(QuiltPackage):
     def __init__(self, attrs: dict):
         super().__init__(attrs)
         self.path = attrs[QuiltPath.K_PTH]
         logging.debug(f"QuiltPath {self.path} @ {self.uri}")
 
-    def dest(self):
-        return str(self.local_path() / self.path)
-
     async def get(self, opts: dict = {}):
-        dest = self.check_path(opts)
+        dir_dest = self.check_path(opts)
+        dest = dir_dest / self.path
         q = await self.remote_pkg()
         qp = q[self.path]
         qp.fetch(dest=dest)
         return [self.uri]
```

### Comparing `quiltplus-0.9.1/quiltplus/registry.py` & `quiltplus-0.9.2/quiltplus/registry.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.1/quiltplus/resource.py` & `quiltplus-0.9.2/quiltplus/resource.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.1/quiltplus/type.py` & `quiltplus-0.9.2/quiltplus/type.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 from tzlocal import get_localzone
 from un_yaml import UnUri
 
 
 class QuiltType:
     PREFIX = "quilt+"
     K_BKT = UnUri.K_HOST
+    K_FORCE = "force"
+    K_REG = "registry"
 
     # Fragments
     K_PKG = "package"
     K_PTH = "path"
     K_PRP = "property"
     K_CAT = "catalog"
     FRAG_KEYS = [K_PRP, K_PTH, K_PKG]
 
     # Decomposed Package Name
     SEP_HASH = "@"
     SEP_TAG = ":"
     K_HASH = "_hash"
     K_TAG = "_tag"
     K_VER = "_version"
-    SEP = {
-        K_HASH: SEP_HASH,
-        K_TAG: SEP_TAG,
-    }
+    SEP = {K_HASH: SEP_HASH, K_TAG: SEP_TAG, K_PKG: "/"}
 
     @staticmethod
     def BaseType(attrs: dict) -> str:
         for key in QuiltType.FRAG_KEYS:
             if key in attrs:
                 return key
         return UnUri.K_HOST
```

### Comparing `quiltplus-0.9.1/quiltplus/uri.py` & `quiltplus-0.9.2/quiltplus/uri.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Create Quilt URI from UnURI attributes
 
-from un_yaml.un_uri import UnUri
+from un_yaml import UnUri
 
 from .type import QuiltType
 
 
 class QuiltUri(QuiltType):
     @classmethod
     def FromUnUri(cls, un: UnUri) -> "QuiltUri":
@@ -20,35 +20,39 @@
         un = UnUri(uri)
         return un.attrs
 
     def __init__(self, attrs: dict):
         self.attrs = attrs
         self.uri = attrs.get(UnUri.K_URI)
         self.registry = f"{attrs.get(UnUri.K_PROT)}://{attrs.get(UnUri.K_HOST)}"
-        self.package = self.parse_package()
+        package = self.parse_package()
+        self.package: str = package if isinstance(package, str) else ""
 
     def __repr__(self):
         return f"QuiltUri({self.uri})"
 
     def __eq__(self, other: object):
         if not isinstance(other, QuiltUri):
             return NotImplemented
         return self.registry == other.registry and self.package == other.package
 
-    def full_package(self):
-        return self.attrs.get(QuiltUri.K_PKG)
+    def full_package(self) -> str | bool:
+        return self.attrs.get(QuiltUri.K_PKG) or False
 
-    def split_package(self, key):
-        sep = QuiltUri.SEP.get(key)
+    def split_package(self, key) -> str | bool:
+        sep = QuiltUri.SEP[key]
         pkg = self.full_package()
-        if not pkg or sep not in pkg:
-            return None
-        s = pkg.split(sep)
-        self.attrs[key] = s[1]
-        return s[0]
+        if isinstance(pkg, str) and sep in pkg:
+            s = pkg.split(sep)
+            self.attrs[key] = s[1]
+            return s[0]
+        return False
 
-    def parse_package(self):
+    def parse_package(self) -> str | bool:
         return (
             self.split_package(QuiltUri.K_HASH)
             or self.split_package(QuiltUri.K_TAG)
             or self.full_package()
         )
+
+    def has_package(self) -> bool:
+        return QuiltUri.SEP[QuiltUri.K_PKG] in self.package if self.package else False
```

### Comparing `quiltplus-0.9.1/quiltplus/versions.py` & `quiltplus-0.9.2/quiltplus/versions.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.1/PKG-INFO` & `quiltplus-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltplus
-Version: 0.9.1
+Version: 0.9.2
 Summary: Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform
 License: MIT
 Keywords: yaml,api,resource,quilt
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

