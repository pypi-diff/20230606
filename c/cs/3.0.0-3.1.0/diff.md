# Comparing `tmp/cs-3.0.0.tar.gz` & `tmp/cs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs-3.0.0.tar", last modified: Fri Apr 17 14:31:48 2020, max compression
+gzip compressed data, was "cs-3.1.0.tar", last modified: Tue Jun  6 12:56:58 2023, max compression
```

## Comparing `cs-3.0.0.tar` & `cs-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2020-04-17 14:31:48.138101 cs-3.0.0/
--rw-r--r--   0 brute     (1000) brute     (1000)     1501 2016-01-05 15:33:24.000000 cs-3.0.0/LICENSE
--rw-r--r--   0 brute     (1000) brute     (1000)       42 2018-05-17 12:55:37.000000 cs-3.0.0/MANIFEST.in
--rw-r--r--   0 brute     (1000) brute     (1000)    10413 2020-04-17 14:31:48.138101 cs-3.0.0/PKG-INFO
--rw-r--r--   0 brute     (1000) brute     (1000)     7579 2020-04-15 13:20:58.000000 cs-3.0.0/README.rst
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2020-04-17 14:31:48.138101 cs-3.0.0/cs/
--rw-r--r--   0 brute     (1000) brute     (1000)     4473 2020-04-15 13:20:58.000000 cs-3.0.0/cs/__init__.py
--rw-r--r--   0 brute     (1000) brute     (1000)       59 2017-10-06 13:11:06.000000 cs-3.0.0/cs/__main__.py
--rw-r--r--   0 brute     (1000) brute     (1000)     4634 2019-07-10 06:45:55.000000 cs-3.0.0/cs/_async.py
--rw-r--r--   0 brute     (1000) brute     (1000)    18349 2020-04-15 13:20:58.000000 cs-3.0.0/cs/client.py
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2020-04-17 14:31:48.138101 cs-3.0.0/cs.egg-info/
--rw-r--r--   0 brute     (1000) brute     (1000)    10413 2020-04-17 14:31:48.000000 cs-3.0.0/cs.egg-info/PKG-INFO
--rw-r--r--   0 brute     (1000) brute     (1000)      288 2020-04-17 14:31:48.000000 cs-3.0.0/cs.egg-info/SOURCES.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        1 2020-04-17 14:31:48.000000 cs-3.0.0/cs.egg-info/dependency_links.txt
--rw-r--r--   0 brute     (1000) brute     (1000)       32 2020-04-17 14:31:48.000000 cs-3.0.0/cs.egg-info/entry_points.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        1 2016-02-25 16:19:07.000000 cs-3.0.0/cs.egg-info/not-zip-safe
--rw-r--r--   0 brute     (1000) brute     (1000)       53 2020-04-17 14:31:48.000000 cs-3.0.0/cs.egg-info/requires.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        3 2020-04-17 14:31:48.000000 cs-3.0.0/cs.egg-info/top_level.txt
--rw-r--r--   0 brute     (1000) brute     (1000)      227 2020-04-17 14:31:48.138101 cs-3.0.0/setup.cfg
--rw-r--r--   0 brute     (1000) brute     (1000)     1666 2020-04-17 14:30:59.000000 cs-3.0.0/setup.py
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-06 12:56:58.609463 cs-3.1.0/
+-rw-r--r--   0 brute     (1000) brute     (1000)     1501 2023-06-06 12:23:45.000000 cs-3.1.0/LICENSE
+-rw-r--r--   0 brute     (1000) brute     (1000)       42 2023-06-06 12:23:45.000000 cs-3.1.0/MANIFEST.in
+-rw-r--r--   0 brute     (1000) brute     (1000)     8187 2023-06-06 12:56:58.609463 cs-3.1.0/PKG-INFO
+-rw-r--r--   0 brute     (1000) brute     (1000)     7517 2023-06-06 12:23:45.000000 cs-3.1.0/README.rst
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-06 12:56:58.609463 cs-3.1.0/cs/
+-rw-r--r--   0 brute     (1000) brute     (1000)     4473 2023-06-06 12:23:45.000000 cs-3.1.0/cs/__init__.py
+-rw-r--r--   0 brute     (1000) brute     (1000)       59 2023-06-06 12:23:45.000000 cs-3.1.0/cs/__main__.py
+-rw-r--r--   0 brute     (1000) brute     (1000)     4634 2023-06-06 12:23:45.000000 cs-3.1.0/cs/_async.py
+-rw-r--r--   0 brute     (1000) brute     (1000)    18524 2023-06-06 12:55:58.000000 cs-3.1.0/cs/client.py
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-06-06 12:56:58.609463 cs-3.1.0/cs.egg-info/
+-rw-r--r--   0 brute     (1000) brute     (1000)     8187 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/PKG-INFO
+-rw-r--r--   0 brute     (1000) brute     (1000)      288 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/SOURCES.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/dependency_links.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)       31 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/entry_points.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/not-zip-safe
+-rw-r--r--   0 brute     (1000) brute     (1000)       53 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/requires.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        3 2023-06-06 12:56:58.000000 cs-3.1.0/cs.egg-info/top_level.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)     1173 2023-06-06 12:56:58.612796 cs-3.1.0/setup.cfg
+-rw-r--r--   0 brute     (1000) brute     (1000)      140 2023-06-06 12:23:45.000000 cs-3.1.0/setup.py
```

### Comparing `cs-3.0.0/LICENSE` & `cs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cs-3.0.0/README.rst` & `cs-3.1.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,30 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/cs.svg
    :alt: Python versions
    :target: https://pypi.org/project/cs/
 
 A simple, yet powerful CloudStack API client for python and the command-line.
 
-* Python 2.7+ and 3.4+ support.
-* Async support for Python 3.5+.
+* Async support.
 * All present and future CloudStack API calls and parameters are supported.
 * Syntax highlight in the command-line client if Pygments is installed.
 * BSD license.
 
 Installation
 ------------
 
 ::
 
     pip install cs
 
     # with the colored output
     pip install cs[highlight]
 
-    # with the async support (Python 3.5+)
+    # with the async support
     pip install cs[async]
 
     # with both
     pip install cs[async,highlight]
 
 Usage
 -----
```

### Comparing `cs-3.0.0/cs/__init__.py` & `cs-3.1.0/cs/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-3.0.0/cs/_async.py` & `cs-3.1.0/cs/_async.py`

 * *Files identical despite different names*

### Comparing `cs-3.0.0/cs/client.py` & `cs-3.1.0/cs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,23 +49,33 @@
 TIMEOUT = 10
 PAGE_SIZE = 500
 POLL_INTERVAL = 2.0
 EXPIRATION = timedelta(minutes=10)
 EXPIRES_FORMAT = "%Y-%m-%dT%H:%M:%S%z"
 
 REQUIRED_CONFIG_KEYS = {"endpoint", "key", "secret", "method", "timeout"}
-ALLOWED_CONFIG_KEYS = {"verify", "cert", "retry", "theme", "expiration",
-                       "poll_interval", "trace", "dangerous_no_tls_verify",
-                       "header_*"}
+ALLOWED_CONFIG_KEYS = {
+    "verify",
+    "cert",
+    "cert_key",
+    "retry",
+    "theme",
+    "expiration",
+    "poll_interval",
+    "trace",
+    "dangerous_no_tls_verify",
+    "header_*",
+}
 DEFAULT_CONFIG = {
     "timeout": 10,
     "method": "get",
     "retry": 0,
     "verify": None,
     "cert": None,
+    "cert_key": None,
     "name": None,
     "expiration": 600,
     "poll_interval": POLL_INTERVAL,
     "trace": None,
     "dangerous_no_tls_verify": False,
 }
 
@@ -159,51 +169,68 @@
                             params[k] = text_type(v)
         else:
             raise ValueError(type(value))
 
 
 class CloudStackException(Exception):
     """Exception nicely wrapping a request response."""
+
     def __init__(self, *args, **kwargs):
-        self.response = kwargs.pop('response')
+        self.response = kwargs.pop("response")
         super(CloudStackException, self).__init__(*args, **kwargs)
 
 
 class CloudStackApiException(CloudStackException):
     def __init__(self, *args, **kwargs):
-        self.error = kwargs.pop('error')
+        self.error = kwargs.pop("error")
         super(CloudStackApiException, self).__init__(*args, **kwargs)
 
     def __str__(self):
-        return '{0}, error: {1}'.format(
-            super(CloudStackApiException, self).__str__(),
-            self.error
+        return "{0}, error: {1}".format(
+            super(CloudStackApiException, self).__str__(), self.error
         )
 
 
 class CloudStack(object):
-    def __init__(self, endpoint, key, secret, timeout=10, method='get',
-                 verify=None, cert=None, name=None, retry=0,
-                 job_timeout=None, poll_interval=POLL_INTERVAL,
-                 expiration=timedelta(minutes=10), trace=False,
-                 dangerous_no_tls_verify=False, headers=None,
-                 session=None, fetch_result=False):
+    def __init__(
+        self,
+        endpoint,
+        key,
+        secret,
+        timeout=10,
+        method="get",
+        verify=None,
+        cert=None,
+        cert_key=None,
+        name=None,
+        retry=0,
+        job_timeout=None,
+        poll_interval=POLL_INTERVAL,
+        expiration=timedelta(minutes=10),
+        trace=False,
+        dangerous_no_tls_verify=False,
+        headers=None,
+        session=None,
+        fetch_result=False,
+    ):
         self.endpoint = endpoint
         self.key = key
         self.secret = secret
         self.timeout = int(timeout)
         self.method = method.lower()
         if verify:
             self.verify = verify
         else:
             self.verify = not dangerous_no_tls_verify
         if headers is None:
             headers = {}
         self.headers = headers
         self.session = session if session is not None else requests.Session()
+        if cert and cert_key:
+            cert = (cert, cert_key)
         self.cert = cert
         self.name = name
         self.retry = int(retry)
         self.job_timeout = int(job_timeout) if job_timeout else None
         self.poll_interval = float(poll_interval)
         if not hasattr(expiration, "seconds"):
             expiration = timedelta(seconds=int(expiration))
```

