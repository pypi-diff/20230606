# Comparing `tmp/line_async_webhook-1.0.0.tar.gz` & `tmp/line_async_webhook-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line_async_webhook-1.0.0.tar", max compression
+gzip compressed data, was "line_async_webhook-1.0.1.tar", max compression
```

## Comparing `line_async_webhook-1.0.0.tar` & `line_async_webhook-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-1.0.0/README.md
--rw-r--r--   0        0        0     5172 2023-06-06 01:47:55.883947 line_async_webhook-1.0.0/line_async_webhook/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-1.0.0/line_async_webhook/py.typed
--rw-r--r--   0        0        0      421 2023-06-06 01:48:13.855127 line_async_webhook-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-1.0.1/README.md
+-rw-r--r--   0        0        0     5172 2023-06-06 01:51:09.400444 line_async_webhook-1.0.1/line_async_webhook/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-1.0.1/line_async_webhook/py.typed
+-rw-r--r--   0        0        0      421 2023-06-06 01:52:01.952629 line_async_webhook-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-1.0.1/PKG-INFO
```

### Comparing `line_async_webhook-1.0.0/LICENSE` & `line_async_webhook-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `line_async_webhook-1.0.0/line_async_webhook/__init__.py` & `line_async_webhook-1.0.1/line_async_webhook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 key = self._WebhookHandler__get_handler_key(event.__class__)
                 func = self._handlers.get(key, None)
 
             if func is None:
                 func = self._default
 
             if func is None:
-                logger.info('No handler of ' + key + ' and no default handler')
+                LOGGER.info('No handler of ' + key + ' and no default handler')
             else:
                 if inspect.iscoroutinefunction(func):
                     task_group.soonify(self.__invoke_func_async)(func, event, payload)
                 else:
                     self.__invoke_func(func, event, payload)
```

