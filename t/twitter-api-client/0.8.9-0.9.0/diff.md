# Comparing `tmp/twitter-api-client-0.8.9.tar.gz` & `tmp/twitter-api-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.9.tar", last modified: Tue Jun  6 19:10:38 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.0.tar", last modified: Tue Jun  6 20:45:14 2023, max compression
```

## Comparing `twitter-api-client-0.8.9.tar` & `twitter-api-client-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 19:10:38.844102 twitter-api-client-0.8.9/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.9/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 19:10:38.844102 twitter-api-client-0.8.9/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 19:10:38.845102 twitter-api-client-0.8.9/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 19:09:50.000000 twitter-api-client-0.8.9/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 19:10:38.841102 twitter-api-client-0.8.9/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.9/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28299 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.9/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    28404 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.8.9/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9625 2023-06-04 17:08:22.000000 twitter-api-client-0.8.9/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 19:10:38.844102 twitter-api-client-0.8.9/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 19:10:38.000000 twitter-api-client-0.8.9/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.0/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-06 20:43:37.000000 twitter-api-client-0.9.0/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 20:45:14.448000 twitter-api-client-0.9.0/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.0/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23524 2023-06-06 19:05:18.000000 twitter-api-client-0.9.0/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28299 2023-06-06 19:05:18.000000 twitter-api-client-0.9.0/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.9.0/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    28214 2023-06-06 20:39:28.000000 twitter-api-client-0.9.0/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6123 2023-06-06 19:05:18.000000 twitter-api-client-0.9.0/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9683 2023-06-06 20:42:23.000000 twitter-api-client-0.9.0/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-06 20:45:14.449000 twitter-api-client-0.9.0/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-06 20:45:14.000000 twitter-api-client-0.9.0/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.9/LICENSE` & `twitter-api-client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.9/PKG-INFO` & `twitter-api-client-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.9
+Version: 0.9.0
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.8.9/setup.py` & `twitter-api-client-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.9",
+    version="0.9.0",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.8.9/twitter/account.py` & `twitter-api-client-0.9.0/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.9/twitter/constants.py` & `twitter-api-client-0.9.0/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.9/twitter/login.py` & `twitter-api-client-0.9.0/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.9/twitter/scraper.py` & `twitter-api-client-0.9.0/twitter/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,33 +347,28 @@
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
                 return await asyncio.gather(*(get(c, key) for key in keys))
 
         return asyncio.run(process())
 
     def _run(self, operation: tuple[dict, str, str], queries: set | list[int | str | dict], **kwargs):
         keys, qid, name = operation
-        op = kwargs.pop('res', 'json')
-        ops = {
-            None: lambda x: x,  # return raw response
-            'json': lambda x: list(filter(None, (get_json(r, **kwargs) for r in x))),
-            'text': lambda x: [r.text for r in x],
-        }
-
         # stay within rate-limits
         if (l := len(queries)) > 500:
             self.logger.warning(f'Got {l} queries, truncating to first 500.')
             queries = list(queries)[:500]
 
         if all(isinstance(q, dict) for q in queries):
-            return ops[op](asyncio.run(self._process(operation, list(queries), **kwargs)))
+            data = asyncio.run(self._process(operation, list(queries), **kwargs))
+            return get_json(data, **kwargs)
 
         # queries are of type set | list[int|str], need to convert to list[dict]
         _queries = [{k: q} for q in queries for k, v in keys.items()]
-        res = ops[op](asyncio.run(self._process(operation, _queries, **kwargs)))
-        return res.pop() if kwargs.get('cursor') else flatten(res)
+        res = asyncio.run(self._process(operation, _queries, **kwargs))
+        data = get_json(res, **kwargs)
+        return data.pop() if kwargs.get('cursor') else flatten(data)
 
     async def _query(self, client: AsyncClient, operation: tuple, **kwargs) -> Response:
         keys, qid, name = operation
         params = {
             'variables': Operation.default_variables | keys | kwargs,
             'features': Operation.default_features,
         }
```

### Comparing `twitter-api-client-0.8.9/twitter/search.py` & `twitter-api-client-0.9.0/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.9/twitter/util.py` & `twitter-api-client-0.9.0/twitter/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,26 +63,30 @@
         if isinstance(e, list | tuple):
             flat.extend(flatten(e))
         else:
             flat.append(e)
     return flat
 
 
-def get_json(res: list[Response], **kwargs) -> dict | tuple:
+def get_json(res: list[Response], **kwargs) -> list:
     cursor = kwargs.get('cursor')
     temp = res
     if any(isinstance(r, (list, tuple)) for r in res):
         temp = flatten(res)
+    results = []
     for r in temp:
         try:
             data = r.json()
-            # parentheses very important
-            return (data, cursor) if cursor else data
+            if cursor:
+                results.append([data, cursor])
+            else:
+                results.append(data)
         except Exception as e:
             print('Cannot parse JSON response', e)
+    return results
 
 
 def set_qs(url: str, qs: dict, update=False, **kwargs) -> str:
     *_, q, f = urlsplit(url)
     return urlunsplit((*_, urlencode(qs | parse_qs(q) if update else qs, doseq=True, quote_via=quote,
                                      safe=kwargs.get('safe', '')), f))
```

### Comparing `twitter-api-client-0.8.9/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.0/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.9
+Version: 0.9.0
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

