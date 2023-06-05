# Comparing `tmp/lamadava-1.0.5.tar.gz` & `tmp/lamadava-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamadava-1.0.5.tar", last modified: Mon May 22 11:48:35 2023, max compression
+gzip compressed data, was "lamadava-1.0.6.tar", last modified: Mon Jun  5 21:57:42 2023, max compression
```

## Comparing `lamadava-1.0.5.tar` & `lamadava-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:48:35.311477 lamadava-1.0.5/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.5/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1706 2023-05-22 11:48:35.311354 lamadava-1.0.5/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      656 2023-05-22 11:28:17.000000 lamadava-1.0.5/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:48:35.310652 lamadava-1.0.5/lamadava/
--rw-r--r--   0 adw0rd     (501) staff       (20)      186 2023-05-22 11:46:49.000000 lamadava-1.0.5/lamadava/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-05-22 11:46:04.000000 lamadava-1.0.5/lamadava/__version__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    28872 2023-05-22 11:00:16.000000 lamadava-1.0.5/lamadava/api.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    30127 2023-05-22 11:00:16.000000 lamadava-1.0.5/lamadava/asyncapi.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4045 2023-05-22 10:57:32.000000 lamadava-1.0.5/lamadava/base.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-05-22 11:48:35.311190 lamadava-1.0.5/lamadava.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1706 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       14 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-05-22 11:48:35.000000 lamadava-1.0.5/lamadava.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-05-22 11:48:35.311511 lamadava-1.0.5/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     1783 2023-05-22 11:37:03.000000 lamadava-1.0.5/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-06-05 21:57:42.034883 lamadava-1.0.6/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.6/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1720 2023-06-05 21:57:42.034760 lamadava-1.0.6/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      670 2023-05-22 11:50:12.000000 lamadava-1.0.6/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-06-05 21:57:42.034063 lamadava-1.0.6/lamadava/
+-rw-r--r--   0 adw0rd     (501) staff       (20)      451 2023-06-05 21:44:38.000000 lamadava-1.0.6/lamadava/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-06-05 21:56:56.000000 lamadava-1.0.6/lamadava/__version__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    30131 2023-06-05 21:45:48.000000 lamadava-1.0.6/lamadava/api.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    31422 2023-06-05 21:45:48.000000 lamadava-1.0.6/lamadava/asyncapi.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4913 2023-06-05 21:44:38.000000 lamadava-1.0.6/lamadava/base.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-06-05 21:57:42.034593 lamadava-1.0.6/lamadava.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1720 2023-06-05 21:57:42.000000 lamadava-1.0.6/lamadava.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-06-05 21:57:42.000000 lamadava-1.0.6/lamadava.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-06-05 21:57:42.000000 lamadava-1.0.6/lamadava.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       14 2023-06-05 21:57:42.000000 lamadava-1.0.6/lamadava.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-06-05 21:57:42.000000 lamadava-1.0.6/lamadava.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-06-05 21:57:42.034919 lamadava-1.0.6/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1783 2023-05-22 11:37:03.000000 lamadava-1.0.6/setup.py
```

### Comparing `lamadava-1.0.5/LICENSE` & `lamadava-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.5/PKG-INFO` & `lamadava-1.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.5
+Version: 1.0.6
 Summary: Lamadava client, for Python 3.
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# lamadava-python
+# Lamadava client, for Python 3
 
 ![PyPI](https://img.shields.io/pypi/v/lamadava)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lamadava)
 
 [![Downloads](https://pepy.tech/badge/lamadava)](https://pepy.tech/project/lamadava)
 [![Downloads](https://pepy.tech/badge/lamadava/month)](https://pepy.tech/project/lamadava)
 [![Downloads](https://pepy.tech/badge/lamadava/week)](https://pepy.tech/project/lamadava)
```

### Comparing `lamadava-1.0.5/README.md` & `lamadava-1.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# lamadava-python
+# Lamadava client, for Python 3
 
 ![PyPI](https://img.shields.io/pypi/v/lamadava)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lamadava)
 
 [![Downloads](https://pepy.tech/badge/lamadava)](https://pepy.tech/project/lamadava)
 [![Downloads](https://pepy.tech/badge/lamadava/month)](https://pepy.tech/project/lamadava)
 [![Downloads](https://pepy.tech/badge/lamadava/week)](https://pepy.tech/project/lamadava)
```

### Comparing `lamadava-1.0.5/lamadava/api.py` & `lamadava-1.0.6/lamadava/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,58 +460,58 @@
         return self._request("get", "/v2/user/stories/by/username", params=params)
 
     def user_medias_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''User Medias. Get user medias. Results paginated.'''
         params = {"user_id": user_id, "page_id": page_id}
         return self._request("get", "/v2/user/medias", params=params)
 
-    def user_medias(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    def user_medias(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''User Medias. Get user medias. Results paginated.'''
         params = {"user_id": user_id, "page_id": page_id}
-        return self._paging_request("/v2/user/medias", params=params, count=count, container=container)
+        return self._paging_request("/v2/user/medias", params=params, count=count, container=container, max_requests=max_requests)
 
     def user_clips_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''User Clips. Get user clips.'''
         params = {"user_id": user_id, "page_id": page_id}
         return self._request("get", "/v2/user/clips", params=params)
 
-    def user_clips(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    def user_clips(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''User Clips. Get user clips.'''
         params = {"user_id": user_id, "page_id": page_id}
-        return self._paging_request("/v2/user/clips", params=params, count=count, container=container)
+        return self._paging_request("/v2/user/clips", params=params, count=count, container=container, max_requests=max_requests)
 
     def user_videos_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''User Videos. Get part of user videos with cursor (default 50 media per request)'''
         params = {"user_id": user_id, "page_id": page_id}
         return self._request("get", "/v2/user/videos", params=params)
 
-    def user_videos(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    def user_videos(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''User Videos. Get part of user videos with cursor (default 50 media per request)'''
         params = {"user_id": user_id, "page_id": page_id}
-        return self._paging_request("/v2/user/videos", params=params, count=count, container=container)
+        return self._paging_request("/v2/user/videos", params=params, count=count, container=container, max_requests=max_requests)
 
     def user_following_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''Get a user following (one request required). Get part (one page) of following users'''
         params = {"user_id": user_id, "page_id": page_id}
         return self._request("get", "/v2/user/following", params=params)
 
-    def user_following(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    def user_following(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''Get a user following (one request required). Get part (one page) of following users'''
         params = {"user_id": user_id, "page_id": page_id}
-        return self._paging_request("/v2/user/following", params=params, count=count, container=container)
+        return self._paging_request("/v2/user/following", params=params, count=count, container=container, max_requests=max_requests)
 
     def user_followers_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''Get a user followers (one request required). Get part (one page) of followers users with cursor'''
         params = {"user_id": user_id, "page_id": page_id}
         return self._request("get", "/v2/user/followers", params=params)
 
-    def user_followers(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    def user_followers(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''Get a user followers (one request required). Get part (one page) of followers users with cursor'''
         params = {"user_id": user_id, "page_id": page_id}
-        return self._paging_request("/v2/user/followers", params=params, count=count, container=container)
+        return self._paging_request("/v2/user/followers", params=params, count=count, container=container, max_requests=max_requests)
 
     def media_by_id_v2(self, id: str) -> Dict:
         '''Media By Id. Get media object'''
         params = {"id": id}
         return self._request("get", "/v2/media/by/id", params=params)
 
     def media_by_code_v2(self, code: str) -> Dict:
@@ -525,7 +525,21 @@
         return self._request("get", "/v2/media/by/url", params=params)
 
     def media_likers_v2(self, id: str) -> Dict:
         '''Media Likers. Get user's likers'''
         params = {"id": id}
         return self._request("get", "/v2/media/likers", params=params)
 
+    def track_by_canonical_id_v2(self, canonical_id: str) -> Dict:
+        '''Track By Canonical Id. Get music track object by canonical_id'''
+        params = {"canonical_id": canonical_id}
+        return self._request("get", "/v2/track/by/canonical/id", params=params)
+
+    def track_by_id_v2(self, track_id: str) -> Dict:
+        '''Track By Id. Get music track object by id'''
+        params = {"track_id": track_id}
+        return self._request("get", "/v2/track/by/id", params=params)
+
+    def media_likers(self, media_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
+        '''Get likers on media'''
+        params = {"media_id": media_id, "end_cursor": page_id}
+        return self._paging_request("/gql/media/likers/chunk", params=params, count=count, container=container, page_key="end_cursor", max_requests=max_requests)
```

### Comparing `lamadava-1.0.5/lamadava/asyncapi.py` & `lamadava-1.0.6/lamadava/asyncapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,58 +460,58 @@
         return await self._request("get", "/v2/user/stories/by/username", params=params)
 
     async def user_medias_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''User Medias. Get user medias. Results paginated.'''
         params = {"user_id": user_id, "page_id": page_id}
         return await self._request("get", "/v2/user/medias", params=params)
 
-    async def user_medias(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    async def user_medias(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''User Medias. Get user medias. Results paginated.'''
         params = {"user_id": user_id, "page_id": page_id}
-        return await self._paging_request("/v2/user/medias", params=params, count=count, container=container)
+        return await self._paging_request("/v2/user/medias", params=params, count=count, container=container, max_requests=max_requests)
 
     async def user_clips_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''User Clips. Get user clips.'''
         params = {"user_id": user_id, "page_id": page_id}
         return await self._request("get", "/v2/user/clips", params=params)
 
-    async def user_clips(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    async def user_clips(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''User Clips. Get user clips.'''
         params = {"user_id": user_id, "page_id": page_id}
-        return await self._paging_request("/v2/user/clips", params=params, count=count, container=container)
+        return await self._paging_request("/v2/user/clips", params=params, count=count, container=container, max_requests=max_requests)
 
     async def user_videos_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''User Videos. Get part of user videos with cursor (default 50 media per request)'''
         params = {"user_id": user_id, "page_id": page_id}
         return await self._request("get", "/v2/user/videos", params=params)
 
-    async def user_videos(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    async def user_videos(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''User Videos. Get part of user videos with cursor (default 50 media per request)'''
         params = {"user_id": user_id, "page_id": page_id}
-        return await self._paging_request("/v2/user/videos", params=params, count=count, container=container)
+        return await self._paging_request("/v2/user/videos", params=params, count=count, container=container, max_requests=max_requests)
 
     async def user_following_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''Get a user following (one request required). Get part (one page) of following users'''
         params = {"user_id": user_id, "page_id": page_id}
         return await self._request("get", "/v2/user/following", params=params)
 
-    async def user_following(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    async def user_following(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''Get a user following (one request required). Get part (one page) of following users'''
         params = {"user_id": user_id, "page_id": page_id}
-        return await self._paging_request("/v2/user/following", params=params, count=count, container=container)
+        return await self._paging_request("/v2/user/following", params=params, count=count, container=container, max_requests=max_requests)
 
     async def user_followers_v2(self, user_id: str, page_id: Optional[str] = None) -> Dict:
         '''Get a user followers (one request required). Get part (one page) of followers users with cursor'''
         params = {"user_id": user_id, "page_id": page_id}
         return await self._request("get", "/v2/user/followers", params=params)
 
-    async def user_followers(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None) -> List[Dict]:
+    async def user_followers(self, user_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
         '''Get a user followers (one request required). Get part (one page) of followers users with cursor'''
         params = {"user_id": user_id, "page_id": page_id}
-        return await self._paging_request("/v2/user/followers", params=params, count=count, container=container)
+        return await self._paging_request("/v2/user/followers", params=params, count=count, container=container, max_requests=max_requests)
 
     async def media_by_id_v2(self, id: str) -> Dict:
         '''Media By Id. Get media object'''
         params = {"id": id}
         return await self._request("get", "/v2/media/by/id", params=params)
 
     async def media_by_code_v2(self, code: str) -> Dict:
@@ -525,7 +525,21 @@
         return await self._request("get", "/v2/media/by/url", params=params)
 
     async def media_likers_v2(self, id: str) -> Dict:
         '''Media Likers. Get user's likers'''
         params = {"id": id}
         return await self._request("get", "/v2/media/likers", params=params)
 
+    async def track_by_canonical_id_v2(self, canonical_id: str) -> Dict:
+        '''Track By Canonical Id. Get music track object by canonical_id'''
+        params = {"canonical_id": canonical_id}
+        return await self._request("get", "/v2/track/by/canonical/id", params=params)
+
+    async def track_by_id_v2(self, track_id: str) -> Dict:
+        '''Track By Id. Get music track object by id'''
+        params = {"track_id": track_id}
+        return await self._request("get", "/v2/track/by/id", params=params)
+
+    async def media_likers(self, media_id: str, page_id: Optional[str] = None, count: Optional[int] = None, container: Optional[List[Dict]] = None, max_requests: Optional[int] = None) -> List[Dict]:
+        '''Get likers on media'''
+        params = {"media_id": media_id, "end_cursor": page_id}
+        return await self._paging_request("/gql/media/likers/chunk", params=params, count=count, container=container, page_key="end_cursor", max_requests=max_requests)
```

### Comparing `lamadava-1.0.5/lamadava/base.py` & `lamadava-1.0.6/lamadava/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,32 +50,43 @@
 
     def _paging_request(
         self,
         path: str,
         params: Optional[Dict[str, Any]],
         count: Optional[int] = None,
         container: Optional[List[Dict]] = None,
+        page_key: str = "page_id",
+        max_requests: Optional[int] = None,
     ) -> List[Dict]:
         if params is None:
             params = {}
         if container is None:
             container = []
+        work_count = 0
+        request_count = 0
         while True:
             res = self._request("GET", path, params=params)
-            items = res["response"]["items"]
+            request_count += 1
+            if isinstance(res, list) and len(res) == 2:
+                items, npid = res
+            else:
+                items = res["response"].get("items", res["response"].get("users"))
+                npid = res.get("next_page_id")
             if count is not None:
-                rest = count - len(container)
+                rest = count - work_count
                 items = items[:rest]
             container.extend(items)
-            npid = res.get("next_page_id")
+            work_count += len(items)
             if not npid:
                 break
-            if count is not None and len(container) == count:
+            if count is not None and work_count == count:
                 break
-            params["page_id"] = npid
+            if max_requests is not None and max_requests >= request_count:
+                break
+            params[page_key] = npid
         return container
 
 
 class BaseAsyncClient(BaseClient):
     def __init__(self, token: Optional[str] = None, timeout: Optional[float] = 10):
         super().__init__(token=token, timeout=timeout)
         self._client = httpx.AsyncClient()
@@ -102,32 +113,43 @@
 
     async def _paging_request(
         self,
         path: str,
         params: Optional[Dict[str, Any]],
         count: Optional[int] = None,
         container: Optional[List[Dict]] = None,
+        page_key: str = "page_id",
+        max_requests: Optional[int] = None,
     ) -> List[Dict]:
         if params is None:
             params = {}
         if container is None:
             container = []
+        work_count = 0
+        request_count = 0
         while True:
             res = await self._request("GET", path, params=params)
-            items = res["response"]["items"]
+            request_count += 1
+            if isinstance(res, list) and len(res) == 2:
+                items, npid = res
+            else:
+                items = res["response"].get("items", res["response"].get("users"))
+                npid = res.get("next_page_id")
             if count is not None:
-                rest = count - len(container)
+                rest = count - work_count
                 items = items[:rest]
             container.extend(items)
-            npid = res.get("next_page_id")
+            work_count += len(items)
             if not npid:
                 break
-            if count is not None and len(container) == count:
+            if count is not None and work_count == count:
+                break
+            if max_requests is not None and max_requests >= request_count:
                 break
-            params["page_id"] = npid
+            params[page_key] = npid
         return container
 
     async def aclose(self) -> None:
         """
         Close client.
         """
         await self._client.aclose()
```

### Comparing `lamadava-1.0.5/lamadava.egg-info/PKG-INFO` & `lamadava-1.0.6/lamadava.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.5
+Version: 1.0.6
 Summary: Lamadava client, for Python 3.
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# lamadava-python
+# Lamadava client, for Python 3
 
 ![PyPI](https://img.shields.io/pypi/v/lamadava)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lamadava)
 
 [![Downloads](https://pepy.tech/badge/lamadava)](https://pepy.tech/project/lamadava)
 [![Downloads](https://pepy.tech/badge/lamadava/month)](https://pepy.tech/project/lamadava)
 [![Downloads](https://pepy.tech/badge/lamadava/week)](https://pepy.tech/project/lamadava)
```

### Comparing `lamadava-1.0.5/setup.py` & `lamadava-1.0.6/setup.py`

 * *Files identical despite different names*

