# Comparing `tmp/afex-audit-trail-0.1.5.tar.gz` & `tmp/afex-audit-trail-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-audit-trail-0.1.5.tar", last modified: Mon Apr 17 16:19:37 2023, max compression
+gzip compressed data, was "afex-audit-trail-0.1.6.tar", last modified: Tue Jun  6 08:37:27 2023, max compression
```

## Comparing `afex-audit-trail-0.1.5.tar` & `afex-audit-trail-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:19:37.474349 afex-audit-trail-0.1.5/
--rw-rw-rw-   0        0        0     1061 2023-04-04 12:20:36.000000 afex-audit-trail-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2023-04-17 16:19:37.474349 afex-audit-trail-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-17 16:19:37.450256 afex-audit-trail-0.1.5/afex_audit_trail.egg-info/
--rw-rw-rw-   0        0        0     6661 2023-04-17 16:19:37.000000 afex-audit-trail-0.1.5/afex_audit_trail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-04-17 16:19:37.000000 afex-audit-trail-0.1.5/afex_audit_trail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:19:37.000000 afex-audit-trail-0.1.5/afex_audit_trail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-17 16:19:37.000000 afex-audit-trail-0.1.5/afex_audit_trail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 16:19:37.000000 afex-audit-trail-0.1.5/afex_audit_trail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 16:19:37.466598 afex-audit-trail-0.1.5/audit_trails/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.5/audit_trails/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.5/audit_trails/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:19:37.474349 afex-audit-trail-0.1.5/audit_trails/api/
--rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.5/audit_trails/api/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.5/audit_trails/api/serializers.py
--rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.5/audit_trails/api/urls.py
--rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.5/audit_trails/api/views.py
--rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.5/audit_trails/apps.py
--rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.5/audit_trails/logger.py
--rw-rw-rw-   0        0        0     3280 2023-04-17 16:19:17.000000 afex-audit-trail-0.1.5/audit_trails/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:19:37.474349 afex-audit-trail-0.1.5/audit_trails/migrations/
--rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.5/audit_trails/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.5/audit_trails/migrations/__init__.py
--rw-rw-rw-   0        0        0     3438 2023-04-04 08:39:29.000000 afex-audit-trail-0.1.5/audit_trails/models.py
--rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.5/audit_trails/signals.py
--rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.5/audit_trails/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.5/audit_trails/urls.py
--rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.5/audit_trails/views.py
--rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      987 2023-04-17 16:19:37.474349 afex-audit-trail-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:27.014074 afex-audit-trail-0.1.6/
+-rw-rw-rw-   0        0        0     1062 2023-04-25 08:05:26.000000 afex-audit-trail-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2023-06-06 08:37:27.014074 afex-audit-trail-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:26.962006 afex-audit-trail-0.1.6/afex_audit_trail.egg-info/
+-rw-rw-rw-   0        0        0     6661 2023-06-06 08:37:26.000000 afex-audit-trail-0.1.6/afex_audit_trail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-06-06 08:37:26.000000 afex-audit-trail-0.1.6/afex_audit_trail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 08:37:26.000000 afex-audit-trail-0.1.6/afex_audit_trail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-06 08:37:26.000000 afex-audit-trail-0.1.6/afex_audit_trail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 08:37:26.000000 afex-audit-trail-0.1.6/afex_audit_trail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:27.000073 afex-audit-trail-0.1.6/audit_trails/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.6/audit_trails/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.6/audit_trails/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:27.008072 afex-audit-trail-0.1.6/audit_trails/api/
+-rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.6/audit_trails/api/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.6/audit_trails/api/serializers.py
+-rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.6/audit_trails/api/urls.py
+-rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.6/audit_trails/api/views.py
+-rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.6/audit_trails/apps.py
+-rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.6/audit_trails/logger.py
+-rw-rw-rw-   0        0        0     3280 2023-04-17 16:19:17.000000 afex-audit-trail-0.1.6/audit_trails/middleware.py
+drwxrwxrwx   0        0        0        0 2023-06-06 08:37:27.013088 afex-audit-trail-0.1.6/audit_trails/migrations/
+-rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.6/audit_trails/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.6/audit_trails/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-06-06 08:15:12.000000 afex-audit-trail-0.1.6/audit_trails/models.py
+-rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.6/audit_trails/signals.py
+-rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.6/audit_trails/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.6/audit_trails/urls.py
+-rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.6/audit_trails/views.py
+-rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      987 2023-06-06 08:37:27.018072 afex-audit-trail-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.6/setup.py
```

### Comparing `afex-audit-trail-0.1.5/LICENSE` & `afex-audit-trail-0.1.6/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Copyright 2023 AFEX
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is he`reby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `afex-audit-trail-0.1.5/PKG-INFO` & `afex-audit-trail-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
         
@@ -167,9 +167,9 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
+Requires-Python: >=4.0
 Description-Content-Type: text/markdown
```

### Comparing `afex-audit-trail-0.1.5/afex_audit_trail.egg-info/PKG-INFO` & `afex-audit-trail-0.1.6/afex_audit_trail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
         
@@ -167,9 +167,9 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
+Requires-Python: >=4.0
 Description-Content-Type: text/markdown
```

### Comparing `afex-audit-trail-0.1.5/afex_audit_trail.egg-info/SOURCES.txt` & `afex-audit-trail-0.1.6/afex_audit_trail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/api/serializers.py` & `afex-audit-trail-0.1.6/audit_trails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/api/urls.py` & `afex-audit-trail-0.1.6/audit_trails/api/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/api/views.py` & `afex-audit-trail-0.1.6/audit_trails/api/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/logger.py` & `afex-audit-trail-0.1.6/audit_trails/logger.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/middleware.py` & `afex-audit-trail-0.1.6/audit_trails/middleware.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/migrations/0001_initial.py` & `afex-audit-trail-0.1.6/audit_trails/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/models.py` & `afex-audit-trail-0.1.6/audit_trails/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,19 +55,22 @@
 class Notification(models.Model):
     level = models.CharField(max_length=50, choices=LEVEL_CHOICES)
     recipient = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
         related_name='notifications'
     )
-    actor = models.ForeignKey(
-        settings.AUTH_USER_MODEL,
-        on_delete=models.CASCADE,
-
+    actor_object_id = models.CharField(max_length=255)
+    actor_object_type = models.ForeignKey(
+        ContentType,
+        on_delete=models.SET_NULL,
+        null=True,
+        blank=True
     )
+    actor = GenericForeignKey('actor_object_type', 'actor_object_id')
     action = models.CharField(max_length=255)
     action_object_type = models.ForeignKey(
         ContentType,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name='notification_objects'
```

### Comparing `afex-audit-trail-0.1.5/audit_trails/signals.py` & `afex-audit-trail-0.1.6/audit_trails/signals.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/urls.py` & `afex-audit-trail-0.1.6/audit_trails/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/audit_trails/views.py` & `afex-audit-trail-0.1.6/audit_trails/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.5/setup.cfg` & `afex-audit-trail-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6665 782d 6175 6469 742d 7472   = afex-audit-tr
 00000020: 6169 6c0d 0a76 6572 7369 6f6e 203d 2030  ail..version = 0
-00000030: 2e31 2e35 0d0a 6465 7363 7269 7074 696f  .1.5..descriptio
+00000030: 2e31 2e36 0d0a 6465 7363 7269 7074 696f  .1.6..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6372 6561 7465 2073 6572 7665   to create serve
 00000060: 7220 6c6f 6773 2061 6e64 2075 7365 7273  r logs and users
 00000070: 2720 6e6f 7469 6669 6361 7469 6f6e 2e0d  ' notification..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
@@ -46,17 +46,17 @@
 000002d0: 3a3a 2057 5757 2f48 5454 5020 3a3a 2044  :: WWW/HTTP :: D
 000002e0: 796e 616d 6963 2043 6f6e 7465 6e74 0d0a  ynamic Content..
 000002f0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a69 6e63  ..[options]..inc
 00000300: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
 00000310: 6120 3d20 7472 7565 0d0a 7061 636b 6167  a = true..packag
 00000320: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
 00000330: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000340: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
+00000340: 342e 300d 0a69 6e73 7461 6c6c 5f72 6571  4.0..install_req
 00000350: 7569 7265 7320 3d20 0d0a 0964 6a61 6e67  uires = ...djang
-00000360: 6f20 3e3d 2034 2e31 0d0a 0964 6a61 6e67  o >= 4.1...djang
+00000360: 6f20 3e3d 2033 2e37 0d0a 0964 6a61 6e67  o >= 3.7...djang
 00000370: 6f72 6573 7466 7261 6d65 776f 726b 203e  orestframework >
 00000380: 3d20 332e 3134 0d0a 0964 6a61 6e67 6f72  = 3.14...djangor
 00000390: 6573 7466 7261 6d65 776f 726b 2d73 696d  estframework-sim
 000003a0: 706c 656a 7774 203e 3d20 352e 320d 0a0d  plejwt >= 5.2...
 000003b0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
 000003c0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
 000003d0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

