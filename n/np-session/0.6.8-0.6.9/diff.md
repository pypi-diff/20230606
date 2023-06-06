# Comparing `tmp/np-session-0.6.8.tar.gz` & `tmp/np-session-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.6.8.tar", last modified: Sat May 20 00:40:14 2023, max compression
+gzip compressed data, was "np-session-0.6.9.tar", last modified: Sat May 20 01:30:37 2023, max compression
```

## Comparing `np-session-0.6.8.tar` & `np-session-0.6.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2289 2023-05-20 00:40:09.810704 np-session-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.8/README.md
--rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.8/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.8/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.8/src/np_session/components/info.py
--rw-r--r--   0        0        0     9199 2023-05-11 17:07:49.659610 np-session-0.6.8/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.8/src/np_session/components/mixins.py
--rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.8/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.8/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.8/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.8/src/np_session/components/state.py
--rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.8/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.8/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.8/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.8/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.8/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.8/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.8/src/np_session/exceptions.py
--rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.8/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.8/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.8/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.8/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0     8942 2023-05-04 00:08:23.244576 np-session-0.6.8/src/np_session/session.py
--rw-r--r--   0        0        0      279 2023-05-04 19:21:42.017380 np-session-0.6.8/src/np_session/subclasses/__init__.py
--rw-r--r--   0        0        0     5019 2023-05-20 00:39:37.188536 np-session-0.6.8/src/np_session/subclasses/dynamic_routing_pilot.py
--rw-r--r--   0        0        0    21567 2023-05-04 02:17:18.728472 np-session-0.6.8/src/np_session/subclasses/pipeline.py
--rw-r--r--   0        0        0     8112 2023-05-20 00:39:55.835196 np-session-0.6.8/src/np_session/subclasses/templeton_pilot.py
--rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.8/src/np_session/tasks.py
--rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.8/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.8/tests/__init__.py
--rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.8/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.8/tests/test_platform_json.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     2289 2023-05-20 01:30:32.487449 np-session-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1605 2023-05-02 04:42:52.044238 np-session-0.6.9/README.md
+-rw-r--r--   0        0        0      276 2023-05-02 22:17:18.666545 np-session-0.6.9/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.6.9/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8194 2023-05-02 22:17:19.062889 np-session-0.6.9/src/np_session/components/info.py
+-rw-r--r--   0        0        0     9199 2023-05-11 17:07:49.659610 np-session-0.6.9/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0      741 2023-05-02 22:17:18.814019 np-session-0.6.9/src/np_session/components/mixins.py
+-rw-r--r--   0        0        0     1414 2023-05-02 22:17:18.821357 np-session-0.6.9/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10728 2023-05-02 22:17:19.293122 np-session-0.6.9/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5180 2023-05-02 22:17:19.147807 np-session-0.6.9/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      694 2023-05-02 22:17:18.860357 np-session-0.6.9/src/np_session/components/state.py
+-rw-r--r--   0        0        0      189 2023-05-02 22:20:56.738951 np-session-0.6.9/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21669 2023-05-02 22:17:19.697830 np-session-0.6.9/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2703 2023-05-02 22:17:19.019844 np-session-0.6.9/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12195 2023-05-02 22:17:19.487228 np-session-0.6.9/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12810 2023-05-02 22:17:19.559056 np-session-0.6.9/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3698 2023-05-02 22:17:19.137808 np-session-0.6.9/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0      275 2023-05-02 00:13:24.627489 np-session-0.6.9/src/np_session/exceptions.py
+-rw-r--r--   0        0        0       85 2023-05-02 22:17:18.659546 np-session-0.6.9/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-02 22:17:18.723321 np-session-0.6.9/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.6.9/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      554 2023-05-02 22:17:18.701772 np-session-0.6.9/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0     9041 2023-05-20 01:29:16.750061 np-session-0.6.9/src/np_session/session.py
+-rw-r--r--   0        0        0      279 2023-05-04 19:21:42.017380 np-session-0.6.9/src/np_session/subclasses/__init__.py
+-rw-r--r--   0        0        0     5191 2023-05-20 01:30:12.006374 np-session-0.6.9/src/np_session/subclasses/dynamic_routing_pilot.py
+-rw-r--r--   0        0        0    21567 2023-05-04 02:17:18.728472 np-session-0.6.9/src/np_session/subclasses/pipeline.py
+-rw-r--r--   0        0        0     8265 2023-05-20 01:30:21.985660 np-session-0.6.9/src/np_session/subclasses/templeton_pilot.py
+-rw-r--r--   0        0        0     5058 2023-05-02 22:17:19.095808 np-session-0.6.9/src/np_session/tasks.py
+-rw-r--r--   0        0        0     7630 2023-05-02 22:17:19.141810 np-session-0.6.9/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.6.9/tests/__init__.py
+-rw-r--r--   0        0        0      924 2023-05-02 04:37:54.692561 np-session-0.6.9/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.6.9/tests/test_platform_json.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 np-session-0.6.9/PKG-INFO
```

### Comparing `np-session-0.6.8/pyproject.toml` & `np-session-0.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.6.8"
+version = "0.6.9"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-session-0.6.8/README.md` & `np-session-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/info.py` & `np-session-0.6.9/src/np_session/components/info.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/lims_manifests.py` & `np-session-0.6.9/src/np_session/components/lims_manifests.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/mixins.py` & `np-session-0.6.9/src/np_session/components/mixins.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/paths.py` & `np-session-0.6.9/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/platform_json.py` & `np-session-0.6.9/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/settings_xml.py` & `np-session-0.6.9/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/components/state.py` & `np-session-0.6.9/src/np_session/components/state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/databases/data_getters.py` & `np-session-0.6.9/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/databases/firebase_state.py` & `np-session-0.6.9/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/databases/lims2.py` & `np-session-0.6.9/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/databases/mtrain.py` & `np-session-0.6.9/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/databases/redis_state.py` & `np-session-0.6.9/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/jobs/lims_upload.py` & `np-session-0.6.9/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/jobs/sessions.json` & `np-session-0.6.9/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/jobs/sync_states.py` & `np-session-0.6.9/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/session.py` & `np-session-0.6.9/src/np_session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,14 @@
     """Unique identifier for the session, e.g. lims ecephys session ID"""
     folder: str
     """Folder name for the session, e.g. '1116941914_576323_20210721'"""
     project: str | Project
     """Project name for the session, e.g. 'NeuropixelVisualBehavior'"""
     rig: Optional[str | np_config.Rig] = None
     """Rig ID, e.g. 'NP.0'"""
-    user: Optional[str | User] = None
-    """Operator for the session"""
     lims: Optional[dict | LIMS2SessionInfo] = None
     mtrain: Optional[mtrain.MTrain] = None
     foraging_id: Optional[str] = None
 
     @staticmethod
     def get_folder(path: str | int | PathLike) -> str:
         """Extract the session folder from a path or session ID"""
@@ -187,15 +185,21 @@
         )
         return date
 
     @property
     def npexp_path(self) -> pathlib.Path:
         """np-exp root / folder (may not exist)"""
         return NPEXP_ROOT / self.folder
-
+    
+    @property
+    def user(self) -> str | User | None:
+        """Operator for the session"""
+        if hasattr(self, '_user'):
+            return self._user
+    
     @property
     def mouse(self) -> str | Mouse:
         if not hasattr(self, '_mouse'):
             self._mouse = Mouse(self.folder.split('_')[1])
         return self._mouse
 
     is_ecephys: Optional[bool] = None
```

### Comparing `np-session-0.6.8/src/np_session/subclasses/dynamic_routing_pilot.py` & `np-session-0.6.9/src/np_session/subclasses/dynamic_routing_pilot.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,20 +118,25 @@
         if session_folders:
             return session_folders[0]
 
     @classmethod
     def new(
         cls,
         mouse_labtracks_id: int | str | Mouse,
+        user: Optional[str | User] = None,
         *args,
         **kwargs,
     ) -> Self:
         """Create a new session folder for a mouse."""
         path = cls.storage_dirs[0] / f'DRpilot_{mouse_labtracks_id}_{datetime.date.today().strftime("%Y%m%d")}'
         path.mkdir(parents=True, exist_ok=True)
+        session = cls(path)
+        if user:
+            session._user = user
+        session._mouse = Mouse(mouse_labtracks_id)
         return cls(path, *args, **kwargs)
     
     @property
     def npexp_path(self) -> pathlib.Path:
         with contextlib.suppress(AttributeError):
             return self._npexp_path
         for _ in self.storage_dirs:
```

### Comparing `np-session-0.6.8/src/np_session/subclasses/pipeline.py` & `np-session-0.6.9/src/np_session/subclasses/pipeline.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/subclasses/templeton_pilot.py` & `np-session-0.6.9/src/np_session/subclasses/templeton_pilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,21 +190,26 @@
         if cls.get_extant_path(path):
             return cls.info_to_session_folder(info)
             
     @classmethod
     def new(
         cls,
         mouse_labtracks_id: int | str | Mouse,
+        user: Optional[str | User] = None,
         *args,
         **kwargs,
     ) -> Self:
         """Create a new session folder for a mouse."""
         path = cls.storage_dirs[0] / f'{datetime.datetime.now().strftime(f"{cls.ephys_date_format}_{cls.ephys_time_format}")}_{mouse_labtracks_id}'
         path.mkdir(parents=True, exist_ok=True)
-        return cls(path, *args, **kwargs)
+        session = cls(path)
+        if user:
+            session._user = user
+        session._mouse = Mouse(mouse_labtracks_id)
+        return session
     
     @property
     def npexp_path(self) -> pathlib.Path:
         with contextlib.suppress(AttributeError):
             return self._npexp_path
         
         raise FileNotFoundError(f'Could not find {self.folder} of {self.id} in {self.storage_dirs}')
```

### Comparing `np-session-0.6.8/src/np_session/tasks.py` & `np-session-0.6.9/src/np_session/tasks.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/src/np_session/utils.py` & `np-session-0.6.9/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/tests/test_np_session.py` & `np-session-0.6.9/tests/test_np_session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/tests/test_platform_json.py` & `np-session-0.6.9/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.6.8/PKG-INFO` & `np-session-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.6.8
+Version: 0.6.9
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```

