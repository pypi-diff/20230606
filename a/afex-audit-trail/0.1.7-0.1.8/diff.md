# Comparing `tmp/afex-audit-trail-0.1.7.tar.gz` & `tmp/afex-audit-trail-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-audit-trail-0.1.7.tar", last modified: Tue Jun  6 08:43:25 2023, max compression
+gzip compressed data, was "afex-audit-trail-0.1.8.tar", last modified: Tue Jun  6 10:53:21 2023, max compression
```

## Comparing `afex-audit-trail-0.1.7.tar` & `afex-audit-trail-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 08:43:24.986477 afex-audit-trail-0.1.7/
--rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2023-06-06 08:43:24.986477 afex-audit-trail-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-06 08:43:24.954357 afex-audit-trail-0.1.7/afex_audit_trail.egg-info/
--rw-rw-rw-   0        0        0     6661 2023-06-06 08:43:24.000000 afex-audit-trail-0.1.7/afex_audit_trail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-06-06 08:43:24.000000 afex-audit-trail-0.1.7/afex_audit_trail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 08:43:24.000000 afex-audit-trail-0.1.7/afex_audit_trail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-06 08:43:24.000000 afex-audit-trail-0.1.7/afex_audit_trail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 08:43:24.000000 afex-audit-trail-0.1.7/afex_audit_trail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 08:43:24.970444 afex-audit-trail-0.1.7/audit_trails/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.7/audit_trails/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.7/audit_trails/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:43:24.986477 afex-audit-trail-0.1.7/audit_trails/api/
--rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.7/audit_trails/api/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.7/audit_trails/api/serializers.py
--rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.7/audit_trails/api/urls.py
--rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.7/audit_trails/api/views.py
--rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.7/audit_trails/apps.py
--rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.7/audit_trails/logger.py
--rw-rw-rw-   0        0        0     3280 2023-04-17 16:19:17.000000 afex-audit-trail-0.1.7/audit_trails/middleware.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:43:24.986477 afex-audit-trail-0.1.7/audit_trails/migrations/
--rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.7/audit_trails/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.7/audit_trails/migrations/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-06-06 08:15:12.000000 afex-audit-trail-0.1.7/audit_trails/models.py
--rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.7/audit_trails/signals.py
--rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.7/audit_trails/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.7/audit_trails/urls.py
--rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.7/audit_trails/views.py
--rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      987 2023-06-06 08:43:24.986477 afex-audit-trail-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:53:21.084374 afex-audit-trail-0.1.8/
+-rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2023-06-06 10:53:21.084374 afex-audit-trail-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-06 10:53:21.068726 afex-audit-trail-0.1.8/afex_audit_trail.egg-info/
+-rw-rw-rw-   0        0        0     6661 2023-06-06 10:53:20.000000 afex-audit-trail-0.1.8/afex_audit_trail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-06-06 10:53:20.000000 afex-audit-trail-0.1.8/afex_audit_trail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:53:20.000000 afex-audit-trail-0.1.8/afex_audit_trail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-06 10:53:20.000000 afex-audit-trail-0.1.8/afex_audit_trail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 10:53:20.000000 afex-audit-trail-0.1.8/afex_audit_trail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 10:53:21.084374 afex-audit-trail-0.1.8/audit_trails/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.8/audit_trails/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.8/audit_trails/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:53:21.084374 afex-audit-trail-0.1.8/audit_trails/api/
+-rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.8/audit_trails/api/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.8/audit_trails/api/serializers.py
+-rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.8/audit_trails/api/urls.py
+-rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.8/audit_trails/api/views.py
+-rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.8/audit_trails/apps.py
+-rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.8/audit_trails/logger.py
+-rw-rw-rw-   0        0        0     3280 2023-04-17 16:19:17.000000 afex-audit-trail-0.1.8/audit_trails/middleware.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:53:21.084374 afex-audit-trail-0.1.8/audit_trails/migrations/
+-rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.8/audit_trails/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.8/audit_trails/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-06-06 08:15:12.000000 afex-audit-trail-0.1.8/audit_trails/models.py
+-rw-rw-rw-   0        0        0     1280 2023-06-06 10:36:38.000000 afex-audit-trail-0.1.8/audit_trails/signals.py
+-rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.8/audit_trails/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.8/audit_trails/urls.py
+-rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.8/audit_trails/views.py
+-rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      987 2023-06-06 10:53:21.084374 afex-audit-trail-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.8/setup.py
```

### Comparing `afex-audit-trail-0.1.7/LICENSE` & `afex-audit-trail-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/PKG-INFO` & `afex-audit-trail-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.7/afex_audit_trail.egg-info/PKG-INFO` & `afex-audit-trail-0.1.8/afex_audit_trail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.7/afex_audit_trail.egg-info/SOURCES.txt` & `afex-audit-trail-0.1.8/afex_audit_trail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/api/serializers.py` & `afex-audit-trail-0.1.8/audit_trails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/api/urls.py` & `afex-audit-trail-0.1.8/audit_trails/api/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/api/views.py` & `afex-audit-trail-0.1.8/audit_trails/api/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/logger.py` & `afex-audit-trail-0.1.8/audit_trails/logger.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/middleware.py` & `afex-audit-trail-0.1.8/audit_trails/middleware.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/migrations/0001_initial.py` & `afex-audit-trail-0.1.8/audit_trails/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/models.py` & `afex-audit-trail-0.1.8/audit_trails/models.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/signals.py` & `afex-audit-trail-0.1.8/audit_trails/signals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from django.dispatch import Signal
 
 from audit_trails.models import Notification
 
 
 class Notify:
 
-    def info(self, actor, recipients, **kwargs):
+    def info(self, actor_object_type, actor_object_id, recipients, **kwargs):
         Notification.objects.bulk_create([
-            Notification(actor=actor, recipient=recipient, level='info', **kwargs)
+            Notification(actor_object_type, actor_object_id, recipient=recipient, level='info', **kwargs)
             for recipient in recipients
         ])
 
-    def success(self, actor, recipients, **kwargs):
+    def success(self, actor_object_type, actor_object_id, recipients, **kwargs):
         Notification.objects.bulk_create([
-            Notification(actor=actor, recipient=recipient, level='success', **kwargs)
+            Notification(actor_object_type, actor_object_id, recipient=recipient, level='success', **kwargs)
             for recipient in recipients
         ])
 
-    def warning(self, actor, recipients, **kwargs):
+    def warning(self, actor_object_type, actor_object_id, recipients, **kwargs):
         Notification.objects.bulk_create([
-            Notification(actor=actor, recipient=recipient, level='warning', **kwargs)
+            Notification(actor_object_type, actor_object_id, recipient=recipient, level='warning', **kwargs)
             for recipient in recipients
         ])
 
-    def error(self, actor, recipients, **kwargs):
+    def error(self, actor_object_type, actor_object_id, recipients, **kwargs):
         Notification.objects.bulk_create([
-            Notification(actor=actor, recipient=recipient, level='error', **kwargs)
+            Notification(actor_object_type, actor_object_id, recipient=recipient, level='error', **kwargs)
             for recipient in recipients
         ])
 
 
 notify = Notify()
```

### Comparing `afex-audit-trail-0.1.7/audit_trails/urls.py` & `afex-audit-trail-0.1.8/audit_trails/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/audit_trails/views.py` & `afex-audit-trail-0.1.8/audit_trails/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.7/setup.cfg` & `afex-audit-trail-0.1.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6665 782d 6175 6469 742d 7472   = afex-audit-tr
 00000020: 6169 6c0d 0a76 6572 7369 6f6e 203d 2030  ail..version = 0
-00000030: 2e31 2e37 0d0a 6465 7363 7269 7074 696f  .1.7..descriptio
+00000030: 2e31 2e38 0d0a 6465 7363 7269 7074 696f  .1.8..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6372 6561 7465 2073 6572 7665   to create serve
 00000060: 7220 6c6f 6773 2061 6e64 2075 7365 7273  r logs and users
 00000070: 2720 6e6f 7469 6669 6361 7469 6f6e 2e0d  ' notification..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
```

