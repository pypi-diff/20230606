# Comparing `tmp/cached_url-0.0.8.tar.gz` & `tmp/cached_url-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cached_url-0.0.8.tar", last modified: Sun Mar 15 16:11:11 2020, max compression
+gzip compressed data, was "dist/cached_url-0.0.9.tar", last modified: Thu Apr  9 11:59:53 2020, max compression
```

## Comparing `cached_url-0.0.8.tar` & `cached_url-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-15 16:11:11.000000 cached_url-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      766 2020-03-15 16:11:11.000000 cached_url-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      186 2019-12-31 03:47:38.000000 cached_url-0.0.8/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-15 16:11:11.000000 cached_url-0.0.8/cached_url/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1397 2020-03-15 16:10:44.000000 cached_url-0.0.8/cached_url/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-15 16:11:11.000000 cached_url-0.0.8/cached_url.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      766 2020-03-15 16:11:11.000000 cached_url-0.0.8/cached_url.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      177 2020-03-15 16:11:11.000000 cached_url-0.0.8/cached_url.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-03-15 16:11:11.000000 cached_url-0.0.8/cached_url.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       11 2020-03-15 16:11:11.000000 cached_url-0.0.8/cached_url.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-03-15 16:11:11.000000 cached_url-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      665 2020-03-15 16:10:53.000000 cached_url-0.0.8/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-04-09 11:59:53.000000 cached_url-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      766 2020-04-09 11:59:53.000000 cached_url-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      186 2019-12-31 03:47:38.000000 cached_url-0.0.9/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-04-09 11:59:53.000000 cached_url-0.0.9/cached_url/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1408 2020-04-09 11:59:44.000000 cached_url-0.0.9/cached_url/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-04-09 11:59:53.000000 cached_url-0.0.9/cached_url.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      766 2020-04-09 11:59:53.000000 cached_url-0.0.9/cached_url.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      177 2020-04-09 11:59:53.000000 cached_url-0.0.9/cached_url.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-04-09 11:59:53.000000 cached_url-0.0.9/cached_url.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       11 2020-04-09 11:59:53.000000 cached_url-0.0.9/cached_url.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-04-09 11:59:53.000000 cached_url-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      665 2020-04-09 11:59:48.000000 cached_url-0.0.9/setup.py
```

### Comparing `cached_url-0.0.8/PKG-INFO` & `cached_url-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached_url
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for get url content (cached when testing).
 Home-page: https://github.com/gaoyunzhi/cached_url
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # cached_url
```

### Comparing `cached_url-0.0.8/cached_url/__init__.py` & `cached_url-0.0.9/cached_url/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	if mode != 'b':
 		r.encoding = 'utf-8'
 		return r.text
 	return r.content
 	
 def getFileName(url):
 	h = hashlib.sha224(url.encode('utf-8')).hexdigest()[:3]
-	k = re.sub(r'\W+', '', url.split('/')[-1].split('.')[0])[:10]
+	k = re.sub(r'\W+', '', url.strip('/').split('/')[-1].split('.')[0])[:10]
 	return k + '_' + h
 
 def cachedContent(url, headers = {}, mode=''):
 	ext = os.path.splitext(url)[1] or '.html'
 	cache = 'tmp/' + getFileName(url) + ext
 	try:
 		with open(cache, 'r' + mode) as f:
```

### Comparing `cached_url-0.0.8/cached_url.egg-info/PKG-INFO` & `cached_url-0.0.9/cached_url.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached-url
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for get url content (cached when testing).
 Home-page: https://github.com/gaoyunzhi/cached_url
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # cached_url
```

### Comparing `cached_url-0.0.8/setup.py` & `cached_url-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cached_url",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Library for get url content (cached when testing).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/cached_url",
     packages=setuptools.find_packages(),
```

