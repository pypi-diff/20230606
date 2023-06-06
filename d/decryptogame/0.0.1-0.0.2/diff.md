# Comparing `tmp/decryptogame-0.0.1.tar.gz` & `tmp/decryptogame-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decryptogame-0.0.1.tar", last modified: Mon Jun  5 21:20:41 2023, max compression
+gzip compressed data, was "decryptogame-0.0.2.tar", last modified: Tue Jun  6 09:28:45 2023, max compression
```

## Comparing `decryptogame-0.0.1.tar` & `decryptogame-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-05 21:20:41.610216 decryptogame-0.0.1/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-0.0.1/LICENSE
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1235 2023-06-05 21:20:41.609685 decryptogame-0.0.1/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      780 2023-06-05 20:31:50.000000 decryptogame-0.0.1/README.md
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      631 2023-06-05 20:40:47.000000 decryptogame-0.0.1/pyproject.toml
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-06-05 21:20:41.610347 decryptogame-0.0.1/setup.cfg
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-05 21:20:41.590975 decryptogame-0.0.1/src/
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-05 21:20:41.596370 decryptogame-0.0.1/src/decryptogame/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)        0 2023-06-04 09:04:03.000000 decryptogame-0.0.1/src/decryptogame/__init__.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      443 2023-06-05 16:47:56.000000 decryptogame-0.0.1/src/decryptogame/game.py
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-05 21:20:41.602738 decryptogame-0.0.1/src/decryptogame.egg-info/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1235 2023-06-05 21:20:41.000000 decryptogame-0.0.1/src/decryptogame.egg-info/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      265 2023-06-05 21:20:41.000000 decryptogame-0.0.1/src/decryptogame.egg-info/SOURCES.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-06-05 21:20:41.000000 decryptogame-0.0.1/src/decryptogame.egg-info/dependency_links.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-06-05 21:20:41.000000 decryptogame-0.0.1/src/decryptogame.egg-info/top_level.txt
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-05 21:20:41.603775 decryptogame-0.0.1/tests/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1104 2023-06-05 20:30:20.000000 decryptogame-0.0.1/tests/test_game.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.159469 decryptogame-0.0.2/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-0.0.2/LICENSE
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1344 2023-06-06 09:28:45.158337 decryptogame-0.0.2/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      842 2023-06-06 07:49:38.000000 decryptogame-0.0.2/README.md
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      672 2023-06-06 09:27:13.000000 decryptogame-0.0.2/pyproject.toml
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-06-06 09:28:45.159646 decryptogame-0.0.2/setup.cfg
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.141311 decryptogame-0.0.2/src/
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.146958 decryptogame-0.0.2/src/decryptogame/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)        0 2023-06-04 09:04:03.000000 decryptogame-0.0.2/src/decryptogame/__init__.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1044 2023-06-06 09:21:53.000000 decryptogame-0.0.2/src/decryptogame/game.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.153987 decryptogame-0.0.2/src/decryptogame.egg-info/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1344 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      265 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/SOURCES.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/dependency_links.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/top_level.txt
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.155337 decryptogame-0.0.2/tests/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2674 2023-06-06 09:20:50.000000 decryptogame-0.0.2/tests/test_game.py
```

### Comparing `decryptogame-0.0.1/LICENSE` & `decryptogame-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decryptogame-0.0.1/PKG-INFO` & `decryptogame-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 0.0.1
+Version: 0.0.2
 Summary: A non-official implementation of a Decrypto-style game
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decryptogame
 A non-official implementation of a Decrypto-style game
 
+# Source code
+
+https://github.com/YaBoiSkinnyP/decryptogame/
+
 # Official Authorization
 This implementation may be used so long as its usage satisfies the following criteria:
 
 - it does not use/reproduce, in any manner, Decrypto's logo, illustration or visual identity of the game
 
 - it does not use/reproduce, in any manner, Scorpion Masque’s logo
```

### Comparing `decryptogame-0.0.1/README.md` & `decryptogame-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # decryptogame
 A non-official implementation of a Decrypto-style game
 
+# Source code
+
+https://github.com/YaBoiSkinnyP/decryptogame/
+
 # Official Authorization
 This implementation may be used so long as its usage satisfies the following criteria:
 
 - it does not use/reproduce, in any manner, Decrypto's logo, illustration or visual identity of the game
 
 - it does not use/reproduce, in any manner, Scorpion Masque’s logo
```

### Comparing `decryptogame-0.0.1/pyproject.toml` & `decryptogame-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decryptogame"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jaden Rodriguez", email="jadenrodriguez7@gmail.com" },
 ]
 description = "A non-official implementation of a Decrypto-style game"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
+    "Development Status :: 1 - Planning"
 ]
 
 [tool.pytest.ini_options]
 pythonpath = [
   ".", "src",
 ]
 addopts = [
```

### Comparing `decryptogame-0.0.1/src/decryptogame.egg-info/PKG-INFO` & `decryptogame-0.0.2/src/decryptogame.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 0.0.1
+Version: 0.0.2
 Summary: A non-official implementation of a Decrypto-style game
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decryptogame
 A non-official implementation of a Decrypto-style game
 
+# Source code
+
+https://github.com/YaBoiSkinnyP/decryptogame/
+
 # Official Authorization
 This implementation may be used so long as its usage satisfies the following criteria:
 
 - it does not use/reproduce, in any manner, Decrypto's logo, illustration or visual identity of the game
 
 - it does not use/reproduce, in any manner, Scorpion Masque’s logo
```

