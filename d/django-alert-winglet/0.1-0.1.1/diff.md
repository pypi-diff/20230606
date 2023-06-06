# Comparing `tmp/django-alert-winglet-0.1.tar.gz` & `tmp/django-alert-winglet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-alert-winglet-0.1.tar", last modified: Tue Jun  6 16:54:42 2023, max compression
+gzip compressed data, was "django-alert-winglet-0.1.1.tar", last modified: Tue Jun  6 17:09:08 2023, max compression
```

## Comparing `django-alert-winglet-0.1.tar` & `django-alert-winglet-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:54:42.790286 django-alert-winglet-0.1/
--rw-rw-rw-   0        0        0     1076 2023-06-06 16:54:37.000000 django-alert-winglet-0.1/LICENSE
--rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2444 2023-06-06 16:54:42.790286 django-alert-winglet-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1529 2023-06-06 16:54:37.000000 django-alert-winglet-0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-06 16:54:42.779379 django-alert-winglet-0.1/alert_wing/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1/alert_wing/__init__.py
--rw-rw-rw-   0        0        0      157 2023-06-06 12:24:22.000000 django-alert-winglet-0.1/alert_wing/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:54:42.781145 django-alert-winglet-0.1/alert_wing/managers/
--rw-rw-rw-   0        0        0        0 2023-06-06 08:42:15.000000 django-alert-winglet-0.1/alert_wing/managers/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-06 08:42:15.000000 django-alert-winglet-0.1/alert_wing/managers/base_manager.py
--rw-rw-rw-   0        0        0     4567 2023-06-06 11:35:44.000000 django-alert-winglet-0.1/alert_wing/managers/discord_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:54:42.782760 django-alert-winglet-0.1/alert_wing/senders/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1/alert_wing/senders/__init__.py
--rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1/alert_wing/senders/base.py
--rw-rw-rw-   0        0        0     4568 2023-06-06 11:35:44.000000 django-alert-winglet-0.1/alert_wing/senders/discord.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:54:42.790044 django-alert-winglet-0.1/django_alert_winglet.egg-info/
--rw-rw-rw-   0        0        0     2444 2023-06-06 16:54:42.000000 django-alert-winglet-0.1/django_alert_winglet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-06 16:54:42.000000 django-alert-winglet-0.1/django_alert_winglet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:54:42.000000 django-alert-winglet-0.1/django_alert_winglet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 16:54:42.000000 django-alert-winglet-0.1/django_alert_winglet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 16:54:42.000000 django-alert-winglet-0.1/django_alert_winglet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      990 2023-06-06 16:54:42.791287 django-alert-winglet-0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:08.585312 django-alert-winglet-0.1.1/
+-rw-rw-rw-   0        0        0     1076 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2446 2023-06-06 17:09:08.585610 django-alert-winglet-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1529 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:08.574559 django-alert-winglet-0.1.1/alert_wing/
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.1/alert_wing/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-06-06 12:24:22.000000 django-alert-winglet-0.1.1/alert_wing/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:08.576077 django-alert-winglet-0.1.1/alert_wing/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.1/alert_wing/managers/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.1/alert_wing/managers/base_manager.py
+-rw-rw-rw-   0        0        0     4562 2023-06-06 17:08:14.000000 django-alert-winglet-0.1.1/alert_wing/managers/discord_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:08.577466 django-alert-winglet-0.1.1/alert_wing/senders/
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.1/alert_wing/senders/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.1/alert_wing/senders/base.py
+-rw-rw-rw-   0        0        0     4563 2023-06-06 17:08:24.000000 django-alert-winglet-0.1.1/alert_wing/senders/discord.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:09:08.584540 django-alert-winglet-0.1.1/django_alert_winglet.egg-info/
+-rw-rw-rw-   0        0        0     2446 2023-06-06 17:09:08.000000 django-alert-winglet-0.1.1/django_alert_winglet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-06 17:09:08.000000 django-alert-winglet-0.1.1/django_alert_winglet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:09:08.000000 django-alert-winglet-0.1.1/django_alert_winglet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 17:09:08.000000 django-alert-winglet-0.1.1/django_alert_winglet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 17:09:08.000000 django-alert-winglet-0.1.1/django_alert_winglet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      992 2023-06-06 17:09:08.585749 django-alert-winglet-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1.1/setup.py
```

### Comparing `django-alert-winglet-0.1/LICENSE` & `django-alert-winglet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1/PKG-INFO` & `django-alert-winglet-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1
+Version: 0.1.1
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django-alert-winglet-0.1/README.rst` & `django-alert-winglet-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1/alert_wing/managers/discord_manager.py` & `django-alert-winglet-0.1.1/alert_wing/managers/discord_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import traceback
 
 import discord
 from discord import Embed
 from django.utils import timezone
 
-from apps.alert_wing.managers.base_manager import BaseManager
+from alert_wing.managers.base_manager import BaseManager
 
 
 class DiscordEmbedManager(BaseManager):
     """
     A class for managing Discord embed messages for exception handling.
 
     Args:
```

### Comparing `django-alert-winglet-0.1/alert_wing/senders/discord.py` & `django-alert-winglet-0.1.1/alert_wing/senders/discord.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Any
 
 import requests
 from django.conf import settings
 
-from apps.alert_wing.senders.base import BaseSender
+from alert_wing.senders.base import BaseSender
 
 
 class Discord(BaseSender):
     """
     A class for sending messages or files to a Discord webhook.
 
     Attributes:
```

### Comparing `django-alert-winglet-0.1/django_alert_winglet.egg-info/PKG-INFO` & `django-alert-winglet-0.1.1/django_alert_winglet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1
+Version: 0.1.1
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django-alert-winglet-0.1/django_alert_winglet.egg-info/SOURCES.txt` & `django-alert-winglet-0.1.1/django_alert_winglet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1/setup.cfg` & `django-alert-winglet-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 616c 6572 742d   = django-alert-
 00000020: 7769 6e67 6c65 740d 0a76 6572 7369 6f6e  winglet..version
-00000030: 203d 2030 2e31 0d0a 6465 7363 7269 7074   = 0.1..descript
-00000040: 696f 6e20 3d20 4120 446a 616e 676f 2061  ion = A Django a
-00000050: 7070 2074 6f20 7365 6e64 2061 6e79 2065  pp to send any e
-00000060: 7863 6570 7469 6f6e 2074 6f20 6469 7363  xception to disc
-00000070: 6f72 6420 6368 616e 6e65 6c2e 0d0a 6c6f  ord channel...lo
-00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-00000090: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000a0: 7874 2f78 2d72 7374 0d0a 6c6f 6e67 5f64  xt/x-rst..long_d
-000000b0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000c0: 653a 2052 4541 444d 452e 7273 740d 0a61  e: README.rst..a
-000000d0: 7574 686f 7220 3d20 4d6f 6a74 6162 610d  uthor = Mojtaba.
-000000e0: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-000000f0: 4d6f 6a74 6162 6164 6176 6931 3440 676d  Mojtabadavi14@gm
-00000100: 6169 6c2e 636f 6d0d 0a6c 6963 656e 7365  ail.com..license
-00000110: 203d 204d 4954 204c 6963 656e 7365 0d0a   = MIT License..
-00000120: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000130: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
-00000140: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
-00000150: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000160: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
-00000170: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
-00000180: 2e31 0d0a 0949 6e74 656e 6465 6420 4175  .1...Intended Au
-00000190: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-000001a0: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
-000001b0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000001c0: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
-000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001f0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
-00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000210: 686f 6e0d 0a09 5072 6f67 7261 6d6d 696e  hon...Programmin
-00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000230: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-00000260: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
-00000270: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000280: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002b0: 203a 3a20 332e 390d 0a09 546f 7069 6320   :: 3.9...Topic 
-000002c0: 3a3a 2049 6e74 6572 6e65 7420 3a3a 2057  :: Internet :: W
-000002d0: 5757 2f48 5454 500d 0a09 546f 7069 6320  WW/HTTP...Topic 
-000002e0: 3a3a 2049 6e74 6572 6e65 7420 3a3a 2057  :: Internet :: W
-000002f0: 5757 2f48 5454 5020 3a3a 2044 796e 616d  WW/HTTP :: Dynam
-00000300: 6963 2043 6f6e 7465 6e74 0d0a 0d0a 5b6f  ic Content....[o
-00000310: 7074 696f 6e73 5d0d 0a69 6e63 6c75 6465  ptions]..include
-00000320: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
-00000330: 7472 7565 0d0a 7061 636b 6167 6573 203d  true..packages =
-00000340: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000350: 6571 7569 7265 7320 3d20 7e3d 332e 3130  equires = ~=3.10
-00000360: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000370: 6573 203d 200d 0a09 446a 616e 676f 207e  es = ...Django ~
-00000380: 3d20 342e 312e 350d 0a09 6469 7363 6f72  = 4.1.5...discor
-00000390: 642e 7079 207e 3d32 2e32 2e33 0d0a 0972  d.py ~=2.2.3...r
-000003a0: 6571 7565 7374 7320 7e3d 322e 3238 2e32  equests ~=2.28.2
-000003b0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000003c0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000003d0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000030: 203d 2030 2e31 2e31 0d0a 6465 7363 7269   = 0.1.1..descri
+00000040: 7074 696f 6e20 3d20 4120 446a 616e 676f  ption = A Django
+00000050: 2061 7070 2074 6f20 7365 6e64 2061 6e79   app to send any
+00000060: 2065 7863 6570 7469 6f6e 2074 6f20 6469   exception to di
+00000070: 7363 6f72 6420 6368 616e 6e65 6c2e 0d0a  scord channel...
+00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000a0: 7465 7874 2f78 2d72 7374 0d0a 6c6f 6e67  text/x-rst..long
+000000b0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000c0: 696c 653a 2052 4541 444d 452e 7273 740d  ile: README.rst.
+000000d0: 0a61 7574 686f 7220 3d20 4d6f 6a74 6162  .author = Mojtab
+000000e0: 610d 0a61 7574 686f 725f 656d 6169 6c20  a..author_email 
+000000f0: 3d20 4d6f 6a74 6162 6164 6176 6931 3440  = Mojtabadavi14@
+00000100: 676d 6169 6c2e 636f 6d0d 0a6c 6963 656e  gmail.com..licen
+00000110: 7365 203d 204d 4954 204c 6963 656e 7365  se = MIT License
+00000120: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000130: 0d0a 0945 6e76 6972 6f6e 6d65 6e74 203a  ...Environment :
+00000140: 3a20 5765 6220 456e 7669 726f 6e6d 656e  : Web Environmen
+00000150: 740d 0a09 4672 616d 6577 6f72 6b20 3a3a  t...Framework ::
+00000160: 2044 6a61 6e67 6f0d 0a09 4672 616d 6577   Django...Framew
+00000170: 6f72 6b20 3a3a 2044 6a61 6e67 6f20 3a3a  ork :: Django ::
+00000180: 2034 2e31 0d0a 0949 6e74 656e 6465 6420   4.1...Intended 
+00000190: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+000001a0: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
+000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001c0: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
+000001d0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000001e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000001f0: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
+00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000210: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
+00000220: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000230: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
+00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000260: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
+00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000290: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002b0: 6f6e 203a 3a20 332e 390d 0a09 546f 7069  on :: 3.9...Topi
+000002c0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+000002d0: 2057 5757 2f48 5454 500d 0a09 546f 7069   WWW/HTTP...Topi
+000002e0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+000002f0: 2057 5757 2f48 5454 5020 3a3a 2044 796e   WWW/HTTP :: Dyn
+00000300: 616d 6963 2043 6f6e 7465 6e74 0d0a 0d0a  amic Content....
+00000310: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
+00000320: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000330: 3d20 7472 7565 0d0a 7061 636b 6167 6573  = true..packages
+00000340: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+00000350: 5f72 6571 7569 7265 7320 3d20 7e3d 332e  _requires = ~=3.
+00000360: 3130 0d0a 696e 7374 616c 6c5f 7265 7175  10..install_requ
+00000370: 6972 6573 203d 200d 0a09 446a 616e 676f  ires = ...Django
+00000380: 207e 3d20 342e 312e 350d 0a09 6469 7363   ~= 4.1.5...disc
+00000390: 6f72 642e 7079 207e 3d32 2e32 2e33 0d0a  ord.py ~=2.2.3..
+000003a0: 0972 6571 7565 7374 7320 7e3d 322e 3238  .requests ~=2.28
+000003b0: 2e32 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .2....[egg_info]
+000003c0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000003d0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

