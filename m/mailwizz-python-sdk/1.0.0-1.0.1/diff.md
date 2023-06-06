# Comparing `tmp/mailwizz-python-sdk-1.0.0.tar.gz` & `tmp/mailwizz-python-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailwizz-python-sdk-1.0.0.tar", last modified: Mon Jul 22 10:03:16 2019, max compression
+gzip compressed data, was "mailwizz-python-sdk-1.0.1.tar", last modified: Tue Jun  6 08:38:08 2023, max compression
```

## Comparing `mailwizz-python-sdk-1.0.0.tar` & `mailwizz-python-sdk-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 cristi     (502) staff       (20)        0 2019-07-22 10:03:16.000000 mailwizz-python-sdk-1.0.0/
--rw-r--r--   0 cristi     (502) staff       (20)     1527 2019-07-22 10:03:16.000000 mailwizz-python-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 cristi     (502) staff       (20)      891 2019-07-22 09:59:29.000000 mailwizz-python-sdk-1.0.0/README.md
-drwxr-xr-x   0 cristi     (502) staff       (20)        0 2019-07-22 10:03:16.000000 mailwizz-python-sdk-1.0.0/mailwizz/
--rw-r--r--   0 cristi     (502) staff       (20)        0 2019-07-22 08:25:48.000000 mailwizz-python-sdk-1.0.0/mailwizz/__init__.py
--rw-r--r--   0 cristi     (502) staff       (20)     1395 2019-07-22 08:25:48.000000 mailwizz-python-sdk-1.0.0/mailwizz/base.py
--rw-r--r--   0 cristi     (502) staff       (20)     2726 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/client.py
--rw-r--r--   0 cristi     (502) staff       (20)     1466 2019-07-22 09:09:01.000000 mailwizz-python-sdk-1.0.0/mailwizz/config.py
-drwxr-xr-x   0 cristi     (502) staff       (20)        0 2019-07-22 10:03:16.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/
--rw-r--r--   0 cristi     (502) staff       (20)        0 2019-07-22 08:25:48.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/__init__.py
--rw-r--r--   0 cristi     (502) staff       (20)     1220 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/campaign_bounces.py
--rw-r--r--   0 cristi     (502) staff       (20)     4585 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/campaigns.py
--rw-r--r--   0 cristi     (502) staff       (20)     2223 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/campaigns_tracking.py
--rw-r--r--   0 cristi     (502) staff       (20)     1183 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/countries.py
--rw-r--r--   0 cristi     (502) staff       (20)     1401 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/customers.py
--rw-r--r--   0 cristi     (502) staff       (20)      576 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/list_fields.py
--rw-r--r--   0 cristi     (502) staff       (20)      728 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/list_segments.py
--rw-r--r--   0 cristi     (502) staff       (20)     8910 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/list_subscribers.py
--rw-r--r--   0 cristi     (502) staff       (20)     2563 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/lists.py
--rw-r--r--   0 cristi     (502) staff       (20)     3736 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/templates.py
--rw-r--r--   0 cristi     (502) staff       (20)     2642 2019-07-22 09:10:45.000000 mailwizz-python-sdk-1.0.0/mailwizz/endpoint/transactional_emails.py
--rw-r--r--   0 cristi     (502) staff       (20)     3695 2019-07-22 09:09:01.000000 mailwizz-python-sdk-1.0.0/mailwizz/request.py
-drwxr-xr-x   0 cristi     (502) staff       (20)        0 2019-07-22 10:03:16.000000 mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/
--rw-r--r--   0 cristi     (502) staff       (20)     1527 2019-07-22 10:03:15.000000 mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 cristi     (502) staff       (20)      735 2019-07-22 10:03:15.000000 mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 cristi     (502) staff       (20)        1 2019-07-22 10:03:15.000000 mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 cristi     (502) staff       (20)       67 2019-07-22 10:03:15.000000 mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/requires.txt
--rw-r--r--   0 cristi     (502) staff       (20)        9 2019-07-22 10:03:15.000000 mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 cristi     (502) staff       (20)       38 2019-07-22 10:03:16.000000 mailwizz-python-sdk-1.0.0/setup.cfg
--rw-r--r--   0 cristi     (502) staff       (20)      789 2019-07-22 10:01:10.000000 mailwizz-python-sdk-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:38:08.214841 mailwizz-python-sdk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-06 08:38:08.214841 mailwizz-python-sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:38:08.210842 mailwizz-python-sdk-1.0.1/mailwizz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:38:08.214841 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/campaign_bounces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/campaigns_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/list_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/list_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/list_subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/endpoint/transactional_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/mailwizz/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:38:08.214841 mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-06 08:38:08.000000 mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-06 08:38:08.000000 mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:38:08.000000 mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 08:38:08.000000 mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 08:38:08.000000 mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:38:08.214841 mailwizz-python-sdk-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 08:37:55.000000 mailwizz-python-sdk-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mailwizz-python-sdk-1.0.0/README.md` & `mailwizz-python-sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/base.py` & `mailwizz-python-sdk-1.0.1/mailwizz/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,16 @@
             default = {
                 'general': {},
                 'defaults': {},
                 'notifications': {},
                 'company': {},
                 'options': {},
                 'template': {},
-                'filter': {}
+                'filter': {},
+                'details': {}
             }
 
         data = {**default, **data}
 
         d = {}
 
         for _id in default.keys():
```

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/client.py` & `mailwizz-python-sdk-1.0.1/mailwizz/client.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/config.py` & `mailwizz-python-sdk-1.0.1/mailwizz/config.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/campaign_bounces.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/campaign_bounces.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/campaigns.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/campaigns.py`

 * *Files 10% similar despite different names*

```diff
@@ -137,29 +137,35 @@
         :param default:
         :return:
         """
 
         try:
             content = data['template']['content']
             if content is not None:
-                data['template']['content'] = base64.b64encode(bytes(data['template']['content']))
+                if type(content) is str:
+                    content = bytes(content, 'utf-8')
+                data['template']['content'] = base64.b64encode(content)
         except KeyError:
             pass
 
         try:
             archive = data['template']['archive']
             if archive is not None:
-                data['template']['archive'] = base64.b64encode(bytes(data['template']['archive']))
+                if type(archive) is str:
+                    archive = bytes(archive, 'utf-8')
+                data['template']['archive'] = base64.b64encode(archive)
         except KeyError:
             pass
 
         try:
             text = data['template']['plain_text']
             if text is not None:
-                data['template']['plain_text'] = base64.b64encode(bytes(data['template']['plain_text']))
+                if type(text) is str:
+                    text = bytes(text, 'utf-8')
+                data['template']['plain_text'] = base64.b64encode(text)
         except KeyError:
             pass
 
         if default is None:
             default = {
                 'campaign[options]': {},
                 'campaign[template]': {},
```

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/campaigns_tracking.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/campaigns_tracking.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/countries.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/countries.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/customers.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/customers.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/list_fields.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/list_fields.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/list_segments.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/list_segments.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/list_subscribers.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/list_subscribers.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         :param data:
         :return:
         """
 
         client = Client({
             'method': Client.METHOD_POST,
             'url': self.config.get_api_url('lists/{list_uid}/subscribers'.format(list_uid=list_uid)),
-            'params_post': data
+            'params_post': super()._prepare_body(data)
         })
 
         return client.request()
 
     def create_bulk(self, list_uid: str, data):
         """
         Create subscribers in bulk in the given list
```

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/lists.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/lists.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/templates.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/templates.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,24 +118,28 @@
         Builds the body of the data. Python cannot encode the data so it can be read correctly on the API side
         :param data:
         :param default:
         :return:
         """
 
         try:
-            content = data['template']['content']
+            content = data['content']
             if content is not None:
-                data['template']['content'] = base64.b64encode(bytes(data['template']['content']))
+                if type(content) is str:
+                    content = bytes(content, 'utf-8')
+                data['content'] = base64.b64encode(content)
         except KeyError:
             pass
 
         try:
-            archive = data['template']['archive']
+            archive = data['archive']
             if archive is not None:
-                data['template']['archive'] = base64.b64encode(bytes(data['template']['archive']))
+                if type(archive) is str:
+                    archive = bytes(archive, 'utf-8')
+                data['archive'] = base64.b64encode(archive)
         except KeyError:
             pass
 
         d = {}
 
         for key in data.keys():
             d['template[' + key + ']'] = data[key]
```

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/endpoint/transactional_emails.py` & `mailwizz-python-sdk-1.0.1/mailwizz/endpoint/transactional_emails.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,24 +77,28 @@
         Builds the body of the data. Python cannot encode the data so it can be read correctly on the API side
         :param data:
         :param default:
         :return:
         """
 
         try:
-            content = data['email']['body']
+            content = data['body']
             if content is not None:
-                data['email']['body'] = base64.b64encode(bytes(data['email']['body']))
+                if type(content) is str:
+                    content = bytes(content, 'utf-8')
+                data['body'] = base64.b64encode(content)
         except KeyError:
             pass
 
         try:
-            archive = data['email']['plain_text']
+            archive = data['plain_text']
             if archive is not None:
-                data['email']['plain_text'] = base64.b64encode(bytes(data['email']['plain_text']))
+                if type(archive) is str:
+                    archive = bytes(archive, 'utf-8')
+                data['plain_text'] = base64.b64encode(archive)
         except KeyError:
             pass
 
         d = {}
 
         for key in data.keys():
             d['email[' + key + ']'] = data[key]
```

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz/request.py` & `mailwizz-python-sdk-1.0.1/mailwizz/request.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.0/mailwizz_python_sdk.egg-info/SOURCES.txt` & `mailwizz-python-sdk-1.0.1/mailwizz_python_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 mailwizz/__init__.py
 mailwizz/base.py
 mailwizz/client.py
 mailwizz/config.py
 mailwizz/request.py
```

### Comparing `mailwizz-python-sdk-1.0.0/setup.py` & `mailwizz-python-sdk-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mailwizz-python-sdk',
-    version='1.0.0',
+    version='1.0.1',
     packages=setuptools.find_packages(),
     url='https://www.mailwizz.com',
     license='MIT',
     author='twisted1919',
     author_email='support@mailwizz.com',
     description='This repository contains the Python SDK for MailWizz EMA.',
     long_description=long_description,
```

