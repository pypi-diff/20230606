# Comparing `tmp/fps_yjs-0.1.8.tar.gz` & `tmp/fps_yjs-0.1.9.tar.gz`

## Comparing `fps_yjs-0.1.8.tar` & `fps_yjs-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/fps_yjs/py.typed
--rw-r--r--   0        0        0    14935 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/fps_yjs/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/COPYING.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fps_yjs-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/py.typed
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/fps_yjs/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/COPYING.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fps_yjs-0.1.9/PKG-INFO
```

### Comparing `fps_yjs-0.1.8/fps_yjs/main.py` & `fps_yjs-0.1.9/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.8/fps_yjs/routes.py` & `fps_yjs-0.1.9/fps_yjs/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,17 +171,16 @@
                 # cancel that since there is a new client
                 self.cleaners[room].cancel()
             if not room.ready:
                 file_path = await self.contents.file_id_manager.get_path(file_id)
                 logger.info(f"Opening collaboration room: {websocket.path} ({file_path})")
                 document = YDOCS.get(file_type, YFILE)(room.ydoc)
                 self.documents[websocket.path] = document
-                is_notebook = file_type == "notebook"
                 async with self.lock:
-                    model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+                    model = await self.contents.read_content(file_path, True, file_format)
                 assert model.last_modified is not None
                 self.last_modified[file_id] = to_datetime(model.last_modified)
                 if not room.ready:
                     # try to apply Y updates from the YStore for this document
                     try:
                         await room.ystore.apply_updates(room.ydoc)
                         read_from_source = False
@@ -197,19 +196,21 @@
                     if read_from_source:
                         document.source = model.content
                         await room.ystore.encode_state_as_update(room.ydoc)
 
                     document.dirty = False
                     room.ready = True
                     # save the document to file when changed
-                    document.observe(partial(self.on_document_change, file_id, file_type, document))
+                    document.observe(
+                        partial(self.on_document_change, file_id, file_type, file_format, document)
+                    )
                     # update the document when file changes
                     if file_id not in self.watchers:
                         self.watchers[file_id] = asyncio.create_task(
-                            self.watch_file(file_type, file_id, document)
+                            self.watch_file(file_format, file_id, document)
                         )
 
         await self.websocket_server.serve(websocket)
 
         if is_stored_document and not room.clients:
             # no client in this room after we disconnect
             self.cleaners[room] = asyncio.create_task(self.maybe_clean_room(room, websocket.path))
@@ -241,91 +242,92 @@
         file_path = await self.contents.file_id_manager.get_path(file_id)
         if file_path is None:
             return
         if file_path != document.path:
             document.path = file_path
         return file_path
 
-    async def watch_file(self, file_type: str, file_id: str, document: YBaseDoc) -> None:
+    async def watch_file(self, file_format: str, file_id: str, document: YBaseDoc) -> None:
         file_path = await self.get_file_path(file_id, document)
         assert file_path is not None
         logger.debug(f"Watching file: {file_path}")
         while True:
             watcher = self.contents.file_id_manager.watch(file_path)
             async for changes in watcher:
                 new_file_path = await self.get_file_path(file_id, document)
                 if new_file_path is None:
                     continue
                 if new_file_path != file_path:
                     # file was renamed
                     self.contents.file_id_manager.unwatch(file_path, watcher)
                     file_path = new_file_path
                     # break
-                await self.maybe_load_file(file_type, file_path, file_id)
+                await self.maybe_load_file(file_format, file_path, file_id)
 
-    async def maybe_load_file(self, file_type: str, file_path: str, file_id: str) -> None:
+    async def maybe_load_file(self, file_format: str, file_path: str, file_id: str) -> None:
         async with self.lock:
             model = await self.contents.read_content(file_path, False)
         # do nothing if the file was saved by us
         assert model.last_modified is not None
         if self.last_modified[file_id] < to_datetime(model.last_modified):
             # the file was not saved by us, update the shared document(s)
-            is_notebook = file_type == "notebook"
             async with self.lock:
-                model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+                model = await self.contents.read_content(file_path, True, file_format)
             assert model.last_modified is not None
             documents = [v for k, v in self.documents.items() if k.split(":", 2)[2] == file_id]
             for document in documents:
                 document.source = model.content
             self.last_modified[file_id] = to_datetime(model.last_modified)
 
     def on_document_change(
-        self, file_id: str, file_type: str, document: YBaseDoc, target, event
+        self, file_id: str, file_type: str, file_format: str, document: YBaseDoc, target, event
     ) -> None:
         if target == "state" and "dirty" in event.keys:
             dirty = event.keys["dirty"]["newValue"]
             if not dirty:
                 # we cleared the dirty flag, nothing to save
                 return
         # unobserve and observe again because the structure of the document may have changed
         # e.g. a new cell added to a notebook
         document.unobserve()
-        document.observe(partial(self.on_document_change, file_id, file_type, document))
+        document.observe(
+            partial(self.on_document_change, file_id, file_type, file_format, document)
+        )
         if file_id in self.savers:
             self.savers[file_id].cancel()
         self.savers[file_id] = asyncio.create_task(
-            self.maybe_save_document(file_id, file_type, document)
+            self.maybe_save_document(file_id, file_type, file_format, document)
         )
 
-    async def maybe_save_document(self, file_id: str, file_type: str, document: YBaseDoc) -> None:
+    async def maybe_save_document(
+        self, file_id: str, file_type: str, file_format: str, document: YBaseDoc
+    ) -> None:
         # save after 1 second of inactivity to prevent too frequent saving
         await asyncio.sleep(1)  # FIXME: pass in config
         # if the room cannot be found, don't save
         try:
             file_path = await self.get_file_path(file_id, document)
         except BaseException:
             return
         assert file_path is not None
-        is_notebook = file_type == "notebook"
         async with self.lock:
-            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+            model = await self.contents.read_content(file_path, True, file_format)
         assert model.last_modified is not None
         if self.last_modified[file_id] < to_datetime(model.last_modified):
             # file changed on disk, let's revert
             document.source = model.content
             self.last_modified[file_id] = to_datetime(model.last_modified)
             return
         if model.content != document.source:
             # don't save if not needed
             # this also prevents the dirty flag from bouncing between windows of
             # the same document opened as different types (e.g. notebook/text editor)
-            format = "json" if file_type == "notebook" else "text"
             content = {
                 "content": document.source,
-                "format": format,
+                "format": file_format,
                 "path": file_path,
                 "type": file_type,
             }
             async with self.lock:
                 await self.contents.write_content(content)
                 model = await self.contents.read_content(file_path, False)
             assert model.last_modified is not None
```

### Comparing `fps_yjs-0.1.8/.gitignore` & `fps_yjs-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.8/COPYING.md` & `fps_yjs-0.1.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.8/pyproject.toml` & `fps_yjs-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.8/PKG-INFO` & `fps_yjs-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_yjs
-Version: 0.1.8
+Version: 0.1.9
 Summary: An FPS plugin for the Yjs API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

