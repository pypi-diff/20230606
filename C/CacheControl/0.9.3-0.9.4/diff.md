# Comparing `tmp/CacheControl-0.9.3.tar.gz` & `tmp/CacheControl-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CacheControl-0.9.3.tar", last modified: Thu Mar 13 00:05:16 2014, max compression
+gzip compressed data, was "dist/CacheControl-0.9.4.tar", last modified: Thu Apr 24 03:43:53 2014, max compression
```

## Comparing `CacheControl-0.9.3.tar` & `CacheControl-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-03-13 00:05:15.000000 CacheControl-0.9.3/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-03-13 00:05:15.000000 CacheControl-0.9.3/CacheControl.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)       13 2014-03-13 00:05:15.000000 CacheControl-0.9.3/CacheControl.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) eric      (1000)     1775 2014-03-13 00:05:15.000000 CacheControl-0.9.3/CacheControl.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)      485 2014-03-13 00:05:15.000000 CacheControl-0.9.3/CacheControl.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2014-03-13 00:05:15.000000 CacheControl-0.9.3/CacheControl.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        8 2014-03-13 00:05:15.000000 CacheControl-0.9.3/CacheControl.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) eric      (1000)      924 2014-03-05 22:46:29.000000 CacheControl-0.9.3/README.rst
--rw-r--r--   0 eric      (1000) eric      (1000)      107 2014-03-13 00:05:15.000000 CacheControl-0.9.3/setup.cfg
--rw-r--r--   0 eric      (1000) eric      (1000)      861 2014-03-13 00:05:12.000000 CacheControl-0.9.3/setup.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-03-13 00:05:15.000000 CacheControl-0.9.3/cachecontrol/
--rw-r--r--   0 eric      (1000) eric      (1000)     8764 2014-03-12 22:45:27.000000 CacheControl-0.9.3/cachecontrol/controller.py
--rw-r--r--   0 eric      (1000) eric      (1000)      793 2014-03-05 22:46:29.000000 CacheControl-0.9.3/cachecontrol/cache.py
--rw-r--r--   0 eric      (1000) eric      (1000)      301 2014-03-05 22:46:29.000000 CacheControl-0.9.3/cachecontrol/wrapper.py
--rw-r--r--   0 eric      (1000) eric      (1000)      256 2014-03-05 22:46:29.000000 CacheControl-0.9.3/cachecontrol/compat.py
--rw-r--r--   0 eric      (1000) eric      (1000)      388 2014-03-05 22:46:29.000000 CacheControl-0.9.3/cachecontrol/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     1292 2014-03-05 22:46:29.000000 CacheControl-0.9.3/cachecontrol/patch_requests.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-03-13 00:05:15.000000 CacheControl-0.9.3/cachecontrol/caches/
--rw-r--r--   0 eric      (1000) eric      (1000)     1105 2014-03-12 23:58:22.000000 CacheControl-0.9.3/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 eric      (1000) eric      (1000)      987 2014-03-12 22:41:58.000000 CacheControl-0.9.3/cachecontrol/caches/file_cache.py
--rw-r--r--   0 eric      (1000) eric      (1000)      407 2014-03-05 22:46:29.000000 CacheControl-0.9.3/cachecontrol/caches/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2674 2014-03-12 22:58:09.000000 CacheControl-0.9.3/cachecontrol/adapter.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     1775 2014-03-13 00:05:15.000000 CacheControl-0.9.3/PKG-INFO
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-04-24 03:43:53.000000 CacheControl-0.9.4/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-04-24 03:43:53.000000 CacheControl-0.9.4/CacheControl.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)       13 2014-04-24 03:43:52.000000 CacheControl-0.9.4/CacheControl.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)     1795 2014-04-24 03:43:52.000000 CacheControl-0.9.4/CacheControl.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)      508 2014-04-24 03:43:52.000000 CacheControl-0.9.4/CacheControl.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2014-04-24 03:43:52.000000 CacheControl-0.9.4/CacheControl.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        8 2014-04-24 03:43:52.000000 CacheControl-0.9.4/CacheControl.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      944 2014-04-24 02:52:27.000000 CacheControl-0.9.4/README.rst
+-rw-r--r--   0 eric      (1000) eric      (1000)      107 2014-04-24 03:43:53.000000 CacheControl-0.9.4/setup.cfg
+-rw-r--r--   0 eric      (1000) eric      (1000)      861 2014-04-24 03:43:50.000000 CacheControl-0.9.4/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-04-24 03:43:53.000000 CacheControl-0.9.4/cachecontrol/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8768 2014-04-23 15:39:07.000000 CacheControl-0.9.4/cachecontrol/controller.py
+-rw-r--r--   0 eric      (1000) eric      (1000)      793 2014-03-05 22:46:29.000000 CacheControl-0.9.4/cachecontrol/cache.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3139 2014-04-23 14:21:54.000000 CacheControl-0.9.4/cachecontrol/serialize.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      384 2014-04-23 14:21:54.000000 CacheControl-0.9.4/cachecontrol/wrapper.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      986 2014-04-23 15:39:06.000000 CacheControl-0.9.4/cachecontrol/filewrapper.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      703 2014-04-23 14:21:54.000000 CacheControl-0.9.4/cachecontrol/compat.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      220 2014-04-23 14:21:54.000000 CacheControl-0.9.4/cachecontrol/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2014-04-24 03:43:53.000000 CacheControl-0.9.4/cachecontrol/caches/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      920 2014-04-23 14:21:54.000000 CacheControl-0.9.4/cachecontrol/caches/redis_cache.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2686 2014-04-24 02:52:27.000000 CacheControl-0.9.4/cachecontrol/caches/file_cache.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      369 2014-04-22 04:32:49.000000 CacheControl-0.9.4/cachecontrol/caches/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3136 2014-04-23 14:21:54.000000 CacheControl-0.9.4/cachecontrol/adapter.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1795 2014-04-24 03:43:53.000000 CacheControl-0.9.4/PKG-INFO
```

### Comparing `CacheControl-0.9.3/CacheControl.egg-info/PKG-INFO` & `CacheControl-0.9.4/CacheControl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: CacheControl
-Version: 0.9.3
+Version: 0.9.4
 Summary: httplib2 caching for requests
 Home-page: https://github.com/ionrock/cachecontrol
 Author: Eric Larson
 Author-email: eric@ionrock.org
 License: MIT
 Description: ==============
          CacheControl
@@ -17,15 +17,15 @@
         mitigated by its lack of threadsafety. The same is true of requests in
         terms of caching.
         
         
         Quickstart
         ==========
         
-        ::
+        .. code-block:: python
         
           import requests
         
           from cachecontrol import CacheControl
         
         
           sess = requests.session()
```

### Comparing `CacheControl-0.9.3/README.rst` & `CacheControl-0.9.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 mitigated by its lack of threadsafety. The same is true of requests in
 terms of caching.
 
 
 Quickstart
 ==========
 
-::
+.. code-block:: python
 
   import requests
 
   from cachecontrol import CacheControl
 
 
   sess = requests.session()
```

### Comparing `CacheControl-0.9.3/setup.py` & `CacheControl-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 long_description = open('README.rst').read()
 
-VERSION = '0.9.3'
+VERSION = '0.9.4'
 
 setup_params = dict(
     name='CacheControl',
     version=VERSION,
     author='Eric Larson',
     author_email='eric@ionrock.org',
     license='MIT',
```

### Comparing `CacheControl-0.9.3/cachecontrol/controller.py` & `CacheControl-0.9.4/cachecontrol/controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 The httplib2 algorithms ported for use with requests.
 """
 import re
 import calendar
 import time
 
-from cachecontrol.cache import DictCache
-from cachecontrol.compat import parsedate_tz
+from requests.structures import CaseInsensitiveDict
+
+from .cache import DictCache
+from .compat import parsedate_tz
+from .serialize import Serializer
 
 
 URI = re.compile(r"^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?")
 
 
 def parse_uri(uri):
     """Parses a URI using the regex given in Appendix B of RFC 3986.
@@ -20,17 +23,18 @@
     groups = URI.match(uri).groups()
     return (groups[1], groups[3], groups[4], groups[6], groups[8])
 
 
 class CacheController(object):
     """An interface to see if request should cached or not.
     """
-    def __init__(self, cache=None, cache_etags=True):
+    def __init__(self, cache=None, cache_etags=True, serializer=None):
         self.cache = cache or DictCache()
         self.cache_etags = cache_etags
+        self.serializer = serializer or Serializer()
 
     def _urlnorm(self, uri):
         """Normalize the URL to create a safe key for the cache"""
         (scheme, authority, path, query, fragment) = parse_uri(uri)
         if not scheme or not authority:
             raise Exception("Only absolute URIs are allowed. uri = %s" % uri)
         authority = authority.lower()
@@ -66,70 +70,55 @@
                 tuple([x.strip().lower() for x in part.split("=", 1)])
                 for part in parts if -1 != part.find("=")]
             parts_wo_args = [(name.strip().lower(), 1)
                              for name in parts if -1 == name.find("=")]
             retval = dict(parts_with_args + parts_wo_args)
         return retval
 
-    def cached_request(self, url, headers):
-        cache_url = self.cache_url(url)
-        cc = self.parse_cache_control(headers)
+    def cached_request(self, request):
+        cache_url = self.cache_url(request.url)
+        cc = self.parse_cache_control(request.headers)
 
         # non-caching states
         no_cache = True if 'no-cache' in cc else False
         if 'max-age' in cc and cc['max-age'] == 0:
             no_cache = True
 
-        # see if it is in the cache anyways
-        in_cache = self.cache.get(cache_url)
-        if no_cache or not in_cache:
+        # Bail out if no-cache was set
+        if no_cache:
             return False
 
         # It is in the cache, so lets see if it is going to be
         # fresh enough
-        resp = self.cache.get(cache_url)
+        resp = self.serializer.loads(request, self.cache.get(cache_url))
 
-        # Check our Vary header to make sure our request headers match
-        # up. We don't delete it from the though, we just don't return
-        # our cached value.
-        #
-        # NOTE: Because httplib2 stores raw content, it denotes
-        #       headers that were sent in the original response by
-        #       adding -varied-$name. We don't have to do that b/c we
-        #       are storing the object which has a reference to the
-        #       original request. If that changes, then I'd propose
-        #       using the varied headers in the cache key to avoid the
-        #       situation all together.
-        if 'vary' in resp.headers:
-            varied_headers = resp.headers['vary'].replace(' ', '').split(',')
-            original_headers = resp.request.headers
-            for header in varied_headers:
-                # If our headers don't match for the headers listed in
-                # the vary header, then don't use the cached response
-                if headers.get(header, None) != original_headers.get(header):
-                    return False
+        # Check to see if we have a cached object
+        if not resp:
+            return False
+
+        headers = CaseInsensitiveDict(resp.headers)
 
         now = time.time()
         date = calendar.timegm(
-            parsedate_tz(resp.headers['date'])
+            parsedate_tz(headers['date'])
         )
         current_age = max(0, now - date)
 
         # TODO: There is an assumption that the result will be a
-        # requests response object. This may not be best since we
+        # urllib3 response object. This may not be best since we
         # could probably avoid instantiating or constructing the
         # response until we know we need it.
-        resp_cc = self.parse_cache_control(resp.headers)
+        resp_cc = self.parse_cache_control(headers)
 
         # determine freshness
         freshness_lifetime = 0
         if 'max-age' in resp_cc and resp_cc['max-age'].isdigit():
             freshness_lifetime = int(resp_cc['max-age'])
-        elif 'expires' in resp.headers:
-            expires = parsedate_tz(resp.headers['expires'])
+        elif 'expires' in headers:
+            expires = parsedate_tz(headers['expires'])
             if expires is not None:
                 expire_time = calendar.timegm(expires) - date
                 freshness_lifetime = max(0, expire_time)
 
         # determine if we are setting freshness limit in the req
         if 'max-age' in cc:
             try:
@@ -145,103 +134,124 @@
             # adjust our current age by our min fresh
             current_age += min_fresh
 
         # see how fresh we actually are
         fresh = (freshness_lifetime > current_age)
 
         if fresh:
-            # make sure we set the from_cache to true
-            resp.from_cache = True
             return resp
 
         # we're not fresh. If we don't have an Etag, clear it out
-        if 'etag' not in resp.headers:
+        if 'etag' not in headers:
             self.cache.delete(cache_url)
 
-        if 'etag' in resp.headers:
-            headers['If-None-Match'] = resp.headers['ETag']
-
-        if 'last-modified' in resp.headers:
-            headers['If-Modified-Since'] = resp.headers['Last-Modified']
-
         # return the original handler
         return False
 
-    def add_headers(self, url):
-        resp = self.cache.get(url)
-        if resp and 'etag' in resp.headers:
-            return {'If-None-Match': resp.headers['etag']}
-        return {}
+    def conditional_headers(self, request):
+        cache_url = self.cache_url(request.url)
+        resp = self.serializer.loads(request, self.cache.get(cache_url))
+        new_headers = {}
+
+        if resp:
+            headers = CaseInsensitiveDict(resp.headers)
 
-    def cache_response(self, request, resp):
+            if 'etag' in headers:
+                new_headers['If-None-Match'] = headers['ETag']
+
+            if 'last-modified' in headers:
+                new_headers['If-Modified-Since'] = headers['Last-Modified']
+
+        return new_headers
+
+    def cache_response(self, request, response, body=None):
         """
         Algorithm for caching requests.
 
         This assumes a requests Response object.
         """
         # From httplib2: Don't cache 206's since we aren't going to
         # handle byte range requests
-        if resp.status_code not in [200, 203]:
+        if response.status not in [200, 203]:
             return
 
+        response_headers = CaseInsensitiveDict(response.headers)
+
         cc_req = self.parse_cache_control(request.headers)
-        cc = self.parse_cache_control(resp.headers)
+        cc = self.parse_cache_control(response_headers)
 
         cache_url = self.cache_url(request.url)
 
         # Delete it from the cache if we happen to have it stored there
         no_store = cc.get('no-store') or cc_req.get('no-store')
         if no_store and self.cache.get(cache_url):
             self.cache.delete(cache_url)
 
         # If we've been given an etag, then keep the response
-        if self.cache_etags and 'etag' in resp.headers:
-            self.cache.set(cache_url, resp)
+        if self.cache_etags and 'etag' in response_headers:
+            self.cache.set(
+                cache_url,
+                self.serializer.dumps(request, response, body=body),
+            )
 
         # Add to the cache if the response headers demand it. If there
         # is no date header then we can't do anything about expiring
         # the cache.
-        elif 'date' in resp.headers:
+        elif 'date' in response_headers:
             # cache when there is a max-age > 0
             if cc and cc.get('max-age'):
                 if int(cc['max-age']) > 0:
-                    self.cache.set(cache_url, resp)
+                    self.cache.set(
+                        cache_url,
+                        self.serializer.dumps(request, response, body=body),
+                    )
 
             # If the request can expire, it means we should cache it
             # in the meantime.
-            elif 'expires' in resp.headers:
-                if resp.headers['expires']:
-                    self.cache.set(cache_url, resp)
+            elif 'expires' in response_headers:
+                if response_headers['expires']:
+                    self.cache.set(
+                        cache_url,
+                        self.serializer.dumps(request, response, body=body),
+                    )
 
     def update_cached_response(self, request, response):
         """On a 304 we will get a new set of headers that we want to
         update our cached value with, assuming we have one.
 
         This should only ever be called when we've sent an ETag and
         gotten a 304 as the response.
         """
         cache_url = self.cache_url(request.url)
 
-        resp = self.cache.get(cache_url)
+        cached_response = self.serializer.loads(request, self.cache.get(cache_url))
 
-        if not resp:
+        if not cached_response:
             # we didn't have a cached response
             return response
 
-        # did so lets update our headers
-        resp.headers.update(resp.headers)
+        # Lets update our headers with the headers from the new request:
+        # http://tools.ietf.org/html/draft-ietf-httpbis-p4-conditional-26#section-4.1
+        #
+        # The server isn't supposed to send headers that would make
+        # the cached body invalid. But... just in case, we'll be sure
+        # to strip out ones we know that might be problmatic due to
+        # typical assumptions.
+        excluded_headers = [
+            "content-length",
+        ]
+
+        cached_response.headers.update(
+            dict((k, v) for k, v in response.headers.items()
+                 if k.lower() not in excluded_headers)
+        )
 
         # we want a 200 b/c we have content via the cache
-        request.status_code = 200
-
-        # update the request as it has the if-none-match header + any
-        # other headers that the server might have updated (ie Date,
-        # Cache-Control, Expires, etc.)
-        resp.request = request
+        cached_response.status = 200
 
         # update our cache
-        self.cache.set(cache_url, resp)
-
-        # Let everyone know this was from the cache.
-        resp.from_cache = True
+        self.cache.set(
+            cache_url,
+            self.serializer.dumps(request, cached_response),
+        )
 
-        return resp
+        return cached_response
```

### Comparing `CacheControl-0.9.3/cachecontrol/cache.py` & `CacheControl-0.9.4/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `CacheControl-0.9.3/cachecontrol/caches/redis_cache.py` & `CacheControl-0.9.4/cachecontrol/caches/redis_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from __future__ import division
 
 from datetime import datetime
 
-try:
-    from cPickle import loads, dumps
-except ImportError:  # Python 3.x
-    from pickle import loads, dumps
-
 
 def total_seconds(td):
     """Python 2.6 compatability"""
     if hasattr(td, 'total_seconds'):
         return td.total_seconds()
 
     ms = td.microseconds
@@ -20,22 +15,19 @@
 
 class RedisCache(object):
 
     def __init__(self, conn):
         self.conn = conn
 
     def get(self, key):
-        val = self.conn.get(key)
-        if val:
-            return loads(val)
-        return None
+        return self.conn.get(key)
 
     def set(self, key, value, expires=None):
         if not expires:
-            self.conn.set(key, dumps(value))
+            self.conn.set(key, value)
         else:
             expires = expires - datetime.now()
             self.conn.setex(key, total_seconds(expires), value)
 
     def delete(self, key):
         self.conn.delete(key)
```

### Comparing `CacheControl-0.9.3/cachecontrol/adapter.py` & `CacheControl-0.9.4/cachecontrol/adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,87 @@
+import functools
+
 from requests.adapters import HTTPAdapter
 
-from cachecontrol.controller import CacheController
-from cachecontrol.cache import DictCache
+from .controller import CacheController
+from .cache import DictCache
+from .filewrapper import CallbackFileWrapper
 
 
 class CacheControlAdapter(HTTPAdapter):
     invalidating_methods = set(['PUT', 'DELETE'])
 
-    def __init__(self, cache=None, cache_etags=True, *args, **kw):
+    def __init__(self, cache=None, cache_etags=True, controller_class=None,
+                 serializer=None, *args, **kw):
         super(CacheControlAdapter, self).__init__(*args, **kw)
         self.cache = cache or DictCache()
-        self.controller = CacheController(self.cache, cache_etags=cache_etags)
+
+        controller_factory = controller_class or CacheController
+        self.controller = controller_factory(
+            self.cache,
+            cache_etags=cache_etags,
+            serializer=serializer,
+        )
 
     def send(self, request, **kw):
-        """Send a request. Use the request information to see if it
-        exists in the cache.
+        """
+        Send a request. Use the request information to see if it
+        exists in the cache and cache the response if we need to and can.
         """
         if request.method == 'GET':
-            cached_response = self.controller.cached_request(
-                request.url, request.headers
-            )
+            cached_response = self.controller.cached_request(request)
             if cached_response:
-                # Cached responses should not have a raw field since
-                # they *cannot* be created from some stream.
-                cached_response.raw = None
-                return cached_response
+                return self.build_response(request, cached_response, from_cache=True)
 
             # check for etags and add headers if appropriate
-            headers = self.controller.add_headers(request.url)
-            request.headers.update(headers)
+            request.headers.update(self.controller.conditional_headers(request))
 
         resp = super(CacheControlAdapter, self).send(request, **kw)
+
         return resp
 
-    def build_response(self, request, response):
-        """Build a response by making a request or using the cache.
+    def build_response(self, request, response, from_cache=False):
+        """
+        Build a response by making a request or using the cache.
 
         This will end up calling send and returning a potentially
         cached response
         """
-        resp = super(CacheControlAdapter, self).build_response(
-            request, response
-        )
-
-        # See if we should invalidate the cache.
-        if request.method in self.invalidating_methods and resp.ok:
-            cache_url = self.controller.cache_url(request.url)
-            self.cache.delete(cache_url)
-
-        # Try to store the response if it is a GET
-        elif request.method == 'GET':
+        if not from_cache and request.method == 'GET':
             if response.status == 304:
                 # We must have sent an ETag request. This could mean
                 # that we've been expired already or that we simply
                 # have an etag. In either case, we want to try and
                 # update the cache if that is the case.
-                resp = self.controller.update_cached_response(
+                cached_response = self.controller.update_cached_response(
                     request, response
                 )
+
+                if cached_response is not response:
+                    from_cache = True
+
+                response = cached_response
             else:
-                # try to cache the response
-                self.controller.cache_response(request, resp)
+                # Wrap the response file with a wrapper that will cache the
+                #   response when the stream has been consumed.
+                response._fp = CallbackFileWrapper(
+                    response._fp,
+                    functools.partial(
+                        self.controller.cache_response,
+                        request,
+                        response,
+                    )
+                )
+
+        resp = super(CacheControlAdapter, self).build_response(
+            request, response
+        )
+
+        # See if we should invalidate the cache.
+        if request.method in self.invalidating_methods and resp.ok:
+            cache_url = self.controller.cache_url(request.url)
+            self.cache.delete(cache_url)
 
         # Give the request a from_cache attr to let people use it
-        # rather than testing for hasattr.
-        if not hasattr(resp, 'from_cache'):
-            resp.from_cache = False
+        resp.from_cache = from_cache
 
         return resp
```

### Comparing `CacheControl-0.9.3/PKG-INFO` & `CacheControl-0.9.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: CacheControl
-Version: 0.9.3
+Version: 0.9.4
 Summary: httplib2 caching for requests
 Home-page: https://github.com/ionrock/cachecontrol
 Author: Eric Larson
 Author-email: eric@ionrock.org
 License: MIT
 Description: ==============
          CacheControl
@@ -17,15 +17,15 @@
         mitigated by its lack of threadsafety. The same is true of requests in
         terms of caching.
         
         
         Quickstart
         ==========
         
-        ::
+        .. code-block:: python
         
           import requests
         
           from cachecontrol import CacheControl
         
         
           sess = requests.session()
```

