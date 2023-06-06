# Comparing `tmp/fps_contents-0.1.8.tar.gz` & `tmp/fps_contents-0.1.9.tar.gz`

## Comparing `fps_contents-0.1.8.tar` & `fps_contents-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.8/fps_contents/__init__.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 fps_contents-0.1.8/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.8/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.8/fps_contents/py.typed
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 fps_contents-0.1.8/fps_contents/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.8/COPYING.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.8/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/py.typed
+-rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 fps_contents-0.1.9/fps_contents/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.9/COPYING.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.9/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.9/PKG-INFO
```

### Comparing `fps_contents-0.1.8/fps_contents/fileid.py` & `fps_contents-0.1.9/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.8/fps_contents/routes.py` & `fps_contents-0.1.9/fps_contents/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import json
 import os
 import shutil
 from datetime import datetime
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Union, cast
@@ -133,32 +134,36 @@
         user: User,
     ):
         rename_content = RenameContent(**(await request.json()))
         Path(path).rename(rename_content.path)
         return await self.read_content(rename_content.path, False)
 
     async def read_content(
-        self, path: Union[str, Path], get_content: bool, as_json: bool = False
+        self, path: Union[str, Path], get_content: bool, file_format: Optional[str] = None
     ) -> Content:
         if isinstance(path, str):
             path = Path(path)
         content: Optional[Union[str, Dict, List[Dict]]] = None
         if get_content:
             if path.is_dir():
                 content = [
                     (await self.read_content(subpath, get_content=False)).dict()
                     for subpath in path.iterdir()
                     if not subpath.name.startswith(".")
                 ]
             elif path.is_file() or path.is_symlink():
                 try:
-                    async with await open_file(path) as f:
-                        content = await f.read()
-                    if as_json:
-                        content = json.loads(content)
+                    async with await open_file(path, mode="rb") as f:
+                        content_bytes = await f.read()
+                    if file_format == "base64":
+                        content = base64.b64encode(content_bytes).decode("ascii")
+                    elif file_format == "json":
+                        content = json.loads(content_bytes)
+                    else:
+                        content = content_bytes.decode()
                 except Exception:
                     raise HTTPException(status_code=404, detail="Item not found")
         format: Optional[str] = None
         if path.is_dir():
             size = None
             type = "directory"
             format = "json"
@@ -167,25 +172,25 @@
             size = get_file_size(path)
             if path.suffix == ".ipynb":
                 type = "notebook"
                 format = None
                 mimetype = None
                 if content is not None:
                     nb: dict
-                    if as_json:
+                    if file_format == "json":
                         content = cast(Dict, content)
                         nb = content
                     else:
                         content = cast(str, content)
                         nb = json.loads(content)
                     for cell in nb["cells"]:
                         if "metadata" not in cell:
                             cell["metadata"] = {}
                         cell["metadata"].update({"trusted": False})
-                    if not as_json:
+                    if file_format != "json":
                         content = json.dumps(nb)
             elif path.suffix == ".json":
                 type = "json"
                 format = "text"
                 mimetype = "application/json"
             else:
                 type = "file"
@@ -208,32 +213,41 @@
                 "type": type,
             }
         )
 
     async def write_content(self, content: Union[SaveContent, Dict]) -> None:
         if not isinstance(content, SaveContent):
             content = SaveContent(**content)
-        async with await open_file(content.path, "w") as f:
-            if content.format == "json":
-                dict_content = cast(Dict, content.content)
-                if content.type == "notebook":
-                    # see https://github.com/jupyterlab/jupyterlab/issues/11005
-                    if "metadata" in dict_content and "orig_nbformat" in dict_content["metadata"]:
-                        del dict_content["metadata"]["orig_nbformat"]
-                await f.write(json.dumps(dict_content, indent=2))
-            else:
+        if content.format == "base64":
+            async with await open_file(content.path, "wb") as f:
                 content.content = cast(str, content.content)
-                await f.write(content.content)
+                content_bytes = content.content.encode("ascii")
+                await f.write(content_bytes)
+        else:
+            async with await open_file(content.path, "wt") as f:
+                if content.format == "json":
+                    dict_content = cast(Dict, content.content)
+                    if content.type == "notebook":
+                        # see https://github.com/jupyterlab/jupyterlab/issues/11005
+                        if (
+                            "metadata" in dict_content
+                            and "orig_nbformat" in dict_content["metadata"]
+                        ):
+                            del dict_content["metadata"]["orig_nbformat"]
+                    await f.write(json.dumps(dict_content, indent=2))
+                else:
+                    content.content = cast(str, content.content)
+                    await f.write(content.content)
 
     @property
     def file_id_manager(self):
         return FileIdManager()
 
 
-def get_available_path(path: Path, sep: str = ""):
+def get_available_path(path: Path, sep: str = "") -> Path:
     directory = path.parent
     name = Path(path.name)
     i = None
     while True:
         if i is None:
             i_str = ""
             i = 1
```

### Comparing `fps_contents-0.1.8/.gitignore` & `fps_contents-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.8/COPYING.md` & `fps_contents-0.1.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.8/pyproject.toml` & `fps_contents-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.8/PKG-INFO` & `fps_contents-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_contents
-Version: 0.1.8
+Version: 0.1.9
 Summary: An FPS plugin for the contents API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

