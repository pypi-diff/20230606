# Comparing `tmp/shaggy-1.0.7.tar.gz` & `tmp/shaggy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaggy-1.0.7.tar", last modified: Sat Jun  3 06:56:14 2023, max compression
+gzip compressed data, was "shaggy-1.0.8.tar", last modified: Tue Jun  6 07:24:56 2023, max compression
```

## Comparing `shaggy-1.0.7.tar` & `shaggy-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:56:14.296829 shaggy-1.0.7/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:56:14.292829 shaggy-1.0.7/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2264 2023-06-03 06:14:32.000000 shaggy-1.0.7/README.md
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2023-06-03 06:56:14.296829 shaggy-1.0.7/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1203 2023-06-03 06:55:53.000000 shaggy-1.0.7/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:56:14.292829 shaggy-1.0.7/shaggy/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4870 2023-06-03 06:14:32.000000 shaggy-1.0.7/shaggy/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4187 2023-06-03 06:55:49.000000 shaggy-1.0.7/shaggy/hunt.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      337 2023-06-03 06:14:32.000000 shaggy-1.0.7/shaggy/output.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4110 2023-06-03 06:53:34.000000 shaggy-1.0.7/shaggy/sources.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:56:14.292829 shaggy-1.0.7/shaggy.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:56:14.000000 shaggy-1.0.7/shaggy.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      269 2023-06-03 06:56:14.000000 shaggy-1.0.7/shaggy.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-03 06:56:14.000000 shaggy-1.0.7/shaggy.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-06-03 06:56:14.000000 shaggy-1.0.7/shaggy.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-03 06:56:14.000000 shaggy-1.0.7/shaggy.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-03 06:56:14.000000 shaggy-1.0.7/shaggy.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 07:24:56.187555 shaggy-1.0.8/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-05-31 11:30:02.000000 shaggy-1.0.8/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3067 2023-06-06 07:24:56.187555 shaggy-1.0.8/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2264 2023-06-02 12:57:10.000000 shaggy-1.0.8/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-06 07:24:56.187555 shaggy-1.0.8/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1203 2023-06-06 07:23:17.000000 shaggy-1.0.8/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 07:24:56.183555 shaggy-1.0.8/shaggy/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4870 2023-06-06 07:20:48.000000 shaggy-1.0.8/shaggy/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4187 2023-06-06 07:20:48.000000 shaggy-1.0.8/shaggy/hunt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      337 2023-06-02 12:54:04.000000 shaggy-1.0.8/shaggy/output.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4144 2023-06-06 07:20:48.000000 shaggy-1.0.8/shaggy/sources.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-06 07:24:56.187555 shaggy-1.0.8/shaggy.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3067 2023-06-06 07:24:55.000000 shaggy-1.0.8/shaggy.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      277 2023-06-06 07:24:55.000000 shaggy-1.0.8/shaggy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-06 07:24:55.000000 shaggy-1.0.8/shaggy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-06-06 07:24:55.000000 shaggy-1.0.8/shaggy.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       63 2023-06-06 07:24:55.000000 shaggy-1.0.8/shaggy.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-06 07:24:55.000000 shaggy-1.0.8/shaggy.egg-info/top_level.txt
```

### Comparing `shaggy-1.0.7/PKG-INFO` & `shaggy-1.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 License: MIT
-Description: # Shaggy
-        
-        Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
-        
-        As you know sherlock's devs don't really care about the **important** websites, so we came and cut the **bs** to make your lifes easier. May the [shaggy](https://www.youtube.com/watch?v=6qQJvUfBDOQ) supremacy beggin.
-        
-        ~ **Sherlock, but better**
-        
-        ```
-        
-        ░░░░░░░░░░░░░░░░▄▄█▀▀██▄▄░░░░░░░
-        ░░░░░░░░░░░░░▄█▀▀░░░░░░░▀█░░░░░░
-        ░░░░░░░░░░░▄▀░░░░░░░░░░░░░█░░░░░
-        ░░░░░░░░░▄█░░░░░░░░░░░░░░░█░░░░░
-        ░░░░░░░██▀░░░░░░░▄▄▄░░▄░█▄█▄░░░░
-        ░░░░░▄▀░░░░░░░░░░████░█▄██░▀▄░░░
-        ░░░░█▀░░░░░░░░▄▄██▀░░█████░██░░░
-        ░░░█▀░░░░░░░░░▀█░▀█▀█▀▀▄██▄█▀░░░
-        ░░░██░░░░░░░░░░█░░█░█░░▀▀▄█▀░░░░
-        ░░░░█░░░░░█░░░▀█░░░░▄░░░░░▄█░░░░
-        ░░░░▀█░░░░███▄░█░░░░░░▄▄▄▄█▀█▄░░
-        ░░░░░▀██░░█▄▀▀██░░░░░░░░▄▄█░░▀▄░
-        ░░░░░░▀▀█▄░▀▄▄░▄░░░░░░░███▀░░▄██
-        ░░░░░░░░░▀▀▀███▀█▄░░░░░█▀░▀░░░▀█
-        ░░░░░░░░░░░░▄▀░░░▀█▄░░░░░▄▄░░▄█▀
-        ░░░▄▄▄▀▀▀▀▀█▀░░░░░█▄▀▄▄▄▄▄▄█▀▀░░
-        ░▄█░░░▄██▀░░░░░░░░░█▄░░░░░░░░░░░
-        █▀▀░▄█░░░░░░░░░░░░░░▀▀█▄░░░░░░░░
-        █░░░█░░░░░░░░░░░░░░░░░░█▄░░░░░░░
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Shaggy
+
+Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
+
+As you know sherlock's devs don't really care about the **important** websites, so we came and cut the **bs** to make your lifes easier. May the [shaggy](https://www.youtube.com/watch?v=6qQJvUfBDOQ) supremacy beggin.
+
+~ **Sherlock, but better**
+
+```
+
+░░░░░░░░░░░░░░░░▄▄█▀▀██▄▄░░░░░░░
+░░░░░░░░░░░░░▄█▀▀░░░░░░░▀█░░░░░░
+░░░░░░░░░░░▄▀░░░░░░░░░░░░░█░░░░░
+░░░░░░░░░▄█░░░░░░░░░░░░░░░█░░░░░
+░░░░░░░██▀░░░░░░░▄▄▄░░▄░█▄█▄░░░░
+░░░░░▄▀░░░░░░░░░░████░█▄██░▀▄░░░
+░░░░█▀░░░░░░░░▄▄██▀░░█████░██░░░
+░░░█▀░░░░░░░░░▀█░▀█▀█▀▀▄██▄█▀░░░
+░░░██░░░░░░░░░░█░░█░█░░▀▀▄█▀░░░░
+░░░░█░░░░░█░░░▀█░░░░▄░░░░░▄█░░░░
+░░░░▀█░░░░███▄░█░░░░░░▄▄▄▄█▀█▄░░
+░░░░░▀██░░█▄▀▀██░░░░░░░░▄▄█░░▀▄░
+░░░░░░▀▀█▄░▀▄▄░▄░░░░░░░███▀░░▄██
+░░░░░░░░░▀▀▀███▀█▄░░░░░█▀░▀░░░▀█
+░░░░░░░░░░░░▄▀░░░▀█▄░░░░░▄▄░░▄█▀
+░░░▄▄▄▀▀▀▀▀█▀░░░░░█▄▀▄▄▄▄▄▄█▀▀░░
+░▄█░░░▄██▀░░░░░░░░░█▄░░░░░░░░░░░
+█▀▀░▄█░░░░░░░░░░░░░░▀▀█▄░░░░░░░░
+█░░░█░░░░░░░░░░░░░░░░░░█▄░░░░░░░
+
+```
```

### Comparing `shaggy-1.0.7/README.md` & `shaggy-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.7/setup.py` & `shaggy-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='shaggy',
-    version='1.0.7',
+    version='1.0.8',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mauro Baladés',
     author_email='mauro.balades@tutanota.com',
     description='Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.',
     url='https://github.com/mauro-balades/shaggy',
     packages=["shaggy"],
```

### Comparing `shaggy-1.0.7/shaggy/__init__.py` & `shaggy-1.0.8/shaggy/__init__.py`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.7/shaggy/hunt.py` & `shaggy-1.0.8/shaggy/hunt.py`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.7/shaggy/sources.py` & `shaggy-1.0.8/shaggy/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 sources = {
     "Telegram": {
         "errorMsg": '<meta property="og:description" content="">',
         "url": "https://telegram.me/{}",
     },
     "Instagram": {
-         "errorMsg": "Sorry, this page isn't available",
+         "errorMsg": "Nothing found!",
          "url": "https://www.instagram.com/{}",
+         "api": "https://www.picuki.com/profile/{}"
     },
     "Facebook": {
         "url": "https://www.facebook.com/{}",
         "api": "https://graph.facebook.com/{}/picture",
     },
     "GitHub": {
         "url": "https://www.github.com/{}",
```

### Comparing `shaggy-1.0.7/shaggy.egg-info/PKG-INFO` & `shaggy-1.0.8/shaggy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 License: MIT
-Description: # Shaggy
-        
-        Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
-        
-        As you know sherlock's devs don't really care about the **important** websites, so we came and cut the **bs** to make your lifes easier. May the [shaggy](https://www.youtube.com/watch?v=6qQJvUfBDOQ) supremacy beggin.
-        
-        ~ **Sherlock, but better**
-        
-        ```
-        
-        ░░░░░░░░░░░░░░░░▄▄█▀▀██▄▄░░░░░░░
-        ░░░░░░░░░░░░░▄█▀▀░░░░░░░▀█░░░░░░
-        ░░░░░░░░░░░▄▀░░░░░░░░░░░░░█░░░░░
-        ░░░░░░░░░▄█░░░░░░░░░░░░░░░█░░░░░
-        ░░░░░░░██▀░░░░░░░▄▄▄░░▄░█▄█▄░░░░
-        ░░░░░▄▀░░░░░░░░░░████░█▄██░▀▄░░░
-        ░░░░█▀░░░░░░░░▄▄██▀░░█████░██░░░
-        ░░░█▀░░░░░░░░░▀█░▀█▀█▀▀▄██▄█▀░░░
-        ░░░██░░░░░░░░░░█░░█░█░░▀▀▄█▀░░░░
-        ░░░░█░░░░░█░░░▀█░░░░▄░░░░░▄█░░░░
-        ░░░░▀█░░░░███▄░█░░░░░░▄▄▄▄█▀█▄░░
-        ░░░░░▀██░░█▄▀▀██░░░░░░░░▄▄█░░▀▄░
-        ░░░░░░▀▀█▄░▀▄▄░▄░░░░░░░███▀░░▄██
-        ░░░░░░░░░▀▀▀███▀█▄░░░░░█▀░▀░░░▀█
-        ░░░░░░░░░░░░▄▀░░░▀█▄░░░░░▄▄░░▄█▀
-        ░░░▄▄▄▀▀▀▀▀█▀░░░░░█▄▀▄▄▄▄▄▄█▀▀░░
-        ░▄█░░░▄██▀░░░░░░░░░█▄░░░░░░░░░░░
-        █▀▀░▄█░░░░░░░░░░░░░░▀▀█▄░░░░░░░░
-        █░░░█░░░░░░░░░░░░░░░░░░█▄░░░░░░░
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Shaggy
+
+Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
+
+As you know sherlock's devs don't really care about the **important** websites, so we came and cut the **bs** to make your lifes easier. May the [shaggy](https://www.youtube.com/watch?v=6qQJvUfBDOQ) supremacy beggin.
+
+~ **Sherlock, but better**
+
+```
+
+░░░░░░░░░░░░░░░░▄▄█▀▀██▄▄░░░░░░░
+░░░░░░░░░░░░░▄█▀▀░░░░░░░▀█░░░░░░
+░░░░░░░░░░░▄▀░░░░░░░░░░░░░█░░░░░
+░░░░░░░░░▄█░░░░░░░░░░░░░░░█░░░░░
+░░░░░░░██▀░░░░░░░▄▄▄░░▄░█▄█▄░░░░
+░░░░░▄▀░░░░░░░░░░████░█▄██░▀▄░░░
+░░░░█▀░░░░░░░░▄▄██▀░░█████░██░░░
+░░░█▀░░░░░░░░░▀█░▀█▀█▀▀▄██▄█▀░░░
+░░░██░░░░░░░░░░█░░█░█░░▀▀▄█▀░░░░
+░░░░█░░░░░█░░░▀█░░░░▄░░░░░▄█░░░░
+░░░░▀█░░░░███▄░█░░░░░░▄▄▄▄█▀█▄░░
+░░░░░▀██░░█▄▀▀██░░░░░░░░▄▄█░░▀▄░
+░░░░░░▀▀█▄░▀▄▄░▄░░░░░░░███▀░░▄██
+░░░░░░░░░▀▀▀███▀█▄░░░░░█▀░▀░░░▀█
+░░░░░░░░░░░░▄▀░░░▀█▄░░░░░▄▄░░▄█▀
+░░░▄▄▄▀▀▀▀▀█▀░░░░░█▄▀▄▄▄▄▄▄█▀▀░░
+░▄█░░░▄██▀░░░░░░░░░█▄░░░░░░░░░░░
+█▀▀░▄█░░░░░░░░░░░░░░▀▀█▄░░░░░░░░
+█░░░█░░░░░░░░░░░░░░░░░░█▄░░░░░░░
+
+```
```

