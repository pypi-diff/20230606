# Comparing `tmp/ensta-0.4.tar.gz` & `tmp/ensta-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-0.4.tar", last modified: Tue Jun  6 16:16:39 2023, max compression
+gzip compressed data, was "ensta-0.5.tar", last modified: Tue Jun  6 16:20:02 2023, max compression
```

## Comparing `ensta-0.4.tar` & `ensta-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:39.272200 ensta-0.4/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1687 2023-06-06 16:16:39.272200 ensta-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:39.251585 ensta-0.4/ensta/
--rw-rw-rw-   0        0        0    15634 2023-06-06 16:13:03.000000 ensta-0.4/ensta/Guest.py
--rw-rw-rw-   0        0        0     6417 2023-06-06 16:13:08.000000 ensta-0.4/ensta/Host.py
--rw-rw-rw-   0        0        0       58 2023-06-06 15:20:49.000000 ensta-0.4/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:16:39.272200 ensta-0.4/ensta.egg-info/
--rw-rw-rw-   0        0        0     1687 2023-06-06 16:16:39.000000 ensta-0.4/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-06 16:16:39.000000 ensta-0.4/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:16:39.000000 ensta-0.4/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 16:16:39.000000 ensta-0.4/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 16:16:39.000000 ensta-0.4/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-06 16:16:39.272200 ensta-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-06-06 16:16:08.000000 ensta-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:20:02.275548 ensta-0.5/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1687 2023-06-06 16:20:02.275548 ensta-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-06-06 15:54:53.000000 ensta-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:20:02.259920 ensta-0.5/ensta/
+-rw-rw-rw-   0        0        0    15635 2023-06-06 16:19:18.000000 ensta-0.5/ensta/Guest.py
+-rw-rw-rw-   0        0        0     6419 2023-06-06 16:19:26.000000 ensta-0.5/ensta/Host.py
+-rw-rw-rw-   0        0        0       58 2023-06-06 15:20:49.000000 ensta-0.5/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:20:02.275548 ensta-0.5/ensta.egg-info/
+-rw-rw-rw-   0        0        0     1687 2023-06-06 16:20:02.000000 ensta-0.5/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-06 16:20:02.000000 ensta-0.5/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:20:02.000000 ensta-0.5/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 16:20:02.000000 ensta-0.5/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 16:20:02.000000 ensta-0.5/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-06 16:20:02.275548 ensta-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-06-06 16:19:38.000000 ensta-0.5/setup.py
```

### Comparing `ensta-0.4/LICENSE.txt` & `ensta-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-0.4/PKG-INFO` & `ensta-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.4
+Version: 0.5
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-0.4/README.md` & `ensta-0.5/README.md`

 * *Files identical despite different names*

### Comparing `ensta-0.4/ensta/Guest.py` & `ensta-0.5/ensta/Guest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from json import JSONDecodeError
 import base64
 import random
 import requests
 import requests.cookies
-from lib import commons
+from .lib import commons
 
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
```

### Comparing `ensta-0.4/ensta/Host.py` & `ensta-0.5/ensta/Host.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import requests.cookies
-from lib import exceptions
+from .lib import exceptions
 from json import JSONDecodeError
 import random
 import string
 from Guest import Guest
-from lib import commons
+from .lib import commons
 
 
 class Host:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     preferred_color_scheme: str = "dark"
```

### Comparing `ensta-0.4/ensta.egg-info/PKG-INFO` & `ensta-0.5/ensta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 0.4
+Version: 0.5
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v0.1.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-0.4/setup.py` & `ensta-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
     packages=["ensta"],
-    version="0.4",
+    version="0.5",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
```

