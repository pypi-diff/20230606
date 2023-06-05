# Comparing `tmp/tornado_cliff_walking-0.0.2.tar.gz` & `tmp/tornado_cliff_walking-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tornado_cliff_walking-0.0.2.tar", max compression
+gzip compressed data, was "tornado_cliff_walking-0.0.3.tar", max compression
```

## Comparing `tornado_cliff_walking-0.0.2.tar` & `tornado_cliff_walking-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1075 2023-06-05 18:18:55.957733 tornado_cliff_walking-0.0.2/LICENSE
--rw-r--r--   0        0        0     3354 2023-06-05 22:27:58.629280 tornado_cliff_walking-0.0.2/README.md
--rw-r--r--   0        0        0     1347 2023-06-05 23:11:33.488961 tornado_cliff_walking-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    14488 2023-05-19 20:38:14.123693 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/font/Minecraft.ttf
--rw-r--r--   0        0        0     3455 2023-05-19 20:38:14.139751 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/cookie.png
--rw-r--r--   0        0        0      935 2023-05-19 20:38:14.139927 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_down.png
--rw-r--r--   0        0        0      872 2023-05-19 20:38:14.140033 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_left.png
--rw-r--r--   0        0        0      858 2023-05-19 20:38:14.140144 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_right.png
--rw-r--r--   0        0        0      842 2023-05-19 20:38:14.140271 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_up.png
--rw-r--r--   0        0        0      651 2023-05-19 20:38:14.141640 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_bg1.png
--rw-r--r--   0        0        0      643 2023-05-19 20:38:14.141734 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_bg2.png
--rw-r--r--   0        0        0      165 2023-05-19 21:25:43.576643 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_cliff.png
--rw-r--r--   0        0        0      706 2023-05-19 20:38:14.141951 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_near-cliff1.png
--rw-r--r--   0        0        0      704 2023-05-19 20:38:14.142058 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_near-cliff2.png
--rw-r--r--   0        0        0      651 2023-05-19 21:22:39.402261 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/stool.png
--rw-r--r--   0        0        0     2065 2023-05-19 21:33:25.825331 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/tornado.png
--rw-r--r--   0        0        0    17889 2023-06-05 23:01:20.780056 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/tornadocliffenv.py
--rw-r--r--   0        0        0  1864000 2023-06-05 19:13:20.501098 tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/vid/example.gif
--rw-r--r--   0        0        0     4256 1970-01-01 00:00:00.000000 tornado_cliff_walking-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-05 18:18:55.957733 tornado_cliff_walking-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3358 2023-06-05 23:25:04.754364 tornado_cliff_walking-0.0.3/README.md
+-rw-r--r--   0        0        0     1343 2023-06-05 23:26:16.680795 tornado_cliff_walking-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-05 23:21:16.965275 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/__init__.py
+-rw-r--r--   0        0        0    14488 2023-05-19 20:38:14.123693 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/font/Minecraft.ttf
+-rw-r--r--   0        0        0     3455 2023-05-19 20:38:14.139751 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/cookie.png
+-rw-r--r--   0        0        0      935 2023-05-19 20:38:14.139927 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_down.png
+-rw-r--r--   0        0        0      872 2023-05-19 20:38:14.140033 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_left.png
+-rw-r--r--   0        0        0      858 2023-05-19 20:38:14.140144 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_right.png
+-rw-r--r--   0        0        0      842 2023-05-19 20:38:14.140271 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_up.png
+-rw-r--r--   0        0        0      651 2023-05-19 20:38:14.141640 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_bg1.png
+-rw-r--r--   0        0        0      643 2023-05-19 20:38:14.141734 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_bg2.png
+-rw-r--r--   0        0        0      165 2023-05-19 21:25:43.576643 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_cliff.png
+-rw-r--r--   0        0        0      706 2023-05-19 20:38:14.141951 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_near-cliff1.png
+-rw-r--r--   0        0        0      704 2023-05-19 20:38:14.142058 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_near-cliff2.png
+-rw-r--r--   0        0        0      651 2023-05-19 21:22:39.402261 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/stool.png
+-rw-r--r--   0        0        0     2065 2023-05-19 21:33:25.825331 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/tornado.png
+-rw-r--r--   0        0        0    17889 2023-06-05 23:01:20.780056 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/tornadocliffenv.py
+-rw-r--r--   0        0        0  1864000 2023-06-05 19:13:20.501098 tornado_cliff_walking-0.0.3/src/tornado_cliff_env/vid/example.gif
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 tornado_cliff_walking-0.0.3/PKG-INFO
```

### Comparing `tornado_cliff_walking-0.0.2/LICENSE` & `tornado_cliff_walking-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/README.md` & `tornado_cliff_walking-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # **Tornado Cliff Walking**
 
 <p align="center">
-  <img src="src/tornado_cliff/vid/example.gif" alt="Sublime's custom image" height="240"/>
+  <img src="src/tornado_cliff/vid/example.gif" alt="TonadoCliffWalking Example" height="240"/>
 </p>
 
 
 Cliff Walking with Tornados is a variation of the original Cliff Walking environment.
 It involves crossing a grid world while simultaneously avoiding falling off a cliff
 and encountering a tornado which blows away the character to a random square in the
 grid (including the cliff).
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # **Tornado Cliff Walking**
-                           [Sublime's custom image]
+                         [TonadoCliffWalking Example]
 Cliff Walking with Tornados is a variation of the original Cliff Walking
 environment. It involves crossing a grid world while simultaneously avoiding
 falling off a cliff and encountering a tornado which blows away the character
 to a random square in the grid (including the cliff). ## Description The game
 starts with the Elf at the top left corner of a gridworld (`i.e. [0,0]`). The
 goal location is always at the bottom right corner (`i.e. [-1,-1]`), and if the
 Elf reaches the goal the episode ends. A cliff runs along the middle of the
```

### Comparing `tornado_cliff_walking-0.0.2/pyproject.toml` & `tornado_cliff_walking-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "tornado-cliff-walking"
-version = "0.0.2"
+version = "0.0.3"
 description = "A variation of Gymnasium's CliffWalking enviroment."
 authors = ["Daniel Ávila Vera <davera.017@gmail.com>"]
 repository = "https://github.com/davera-017/TornadoCliffWalking"
 documentation = "https://github.com/davera-017/TornadoCliffWalking"
 readme = "README.md"
 license = "MIT"
 keywords = ["Reinforcement Learning", "CliffWalking", "gymnasium"]
-packages = [{ include = "tornado-cliff-walking", from = "src" }]
+packages = [{ include = "tornado_cliff_env", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "1.24.3"
 gymnasium = {extras = ["toy-text"], version = "0.28.1"}
 pygame = "2.1.3"
```

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/font/Minecraft.ttf` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/font/Minecraft.ttf`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/cookie.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/cookie.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_down.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_down.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_left.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_left.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_right.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_right.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/elf_up.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/elf_up.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_bg1.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_bg1.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_bg2.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_bg2.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_near-cliff1.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_near-cliff1.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/mountain_near-cliff2.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/mountain_near-cliff2.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/stool.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/stool.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/img/tornado.png` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/img/tornado.png`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/tornadocliffenv.py` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/tornadocliffenv.py`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/src/tornado-cliff-walking/vid/example.gif` & `tornado_cliff_walking-0.0.3/src/tornado_cliff_env/vid/example.gif`

 * *Files identical despite different names*

### Comparing `tornado_cliff_walking-0.0.2/PKG-INFO` & `tornado_cliff_walking-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tornado-cliff-walking
-Version: 0.0.2
+Version: 0.0.3
 Summary: A variation of Gymnasium's CliffWalking enviroment.
 Home-page: https://github.com/davera-017/TornadoCliffWalking
 License: MIT
 Keywords: Reinforcement Learning,CliffWalking,gymnasium
 Author: Daniel Ávila Vera
 Author-email: davera.017@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,15 +19,15 @@
 Project-URL: Documentation, https://github.com/davera-017/TornadoCliffWalking
 Project-URL: Repository, https://github.com/davera-017/TornadoCliffWalking
 Description-Content-Type: text/markdown
 
 # **Tornado Cliff Walking**
 
 <p align="center">
-  <img src="src/tornado_cliff/vid/example.gif" alt="Sublime's custom image" height="240"/>
+  <img src="src/tornado_cliff/vid/example.gif" alt="TonadoCliffWalking Example" height="240"/>
 </p>
 
 
 Cliff Walking with Tornados is a variation of the original Cliff Walking environment.
 It involves crossing a grid world while simultaneously avoiding falling off a cliff
 and encountering a tornado which blows away the character to a random square in the
 grid (including the cliff).
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: tornado-cliff-walking Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: tornado-cliff-walking Version: 0.0.3 Summary: A
 variation of Gymnasium's CliffWalking enviroment. Home-page: https://
 github.com/davera-017/TornadoCliffWalking License: MIT Keywords: Reinforcement
 Learning,CliffWalking,gymnasium Author: Daniel Ãvila Vera Author-email:
 davera.017@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gymnasium[toy-text] (==0.28.1) Requires-Dist: numpy (==1.24.3)
 Requires-Dist: pygame (==2.1.3) Project-URL: Documentation, https://github.com/
 davera-017/TornadoCliffWalking Project-URL: Repository, https://github.com/
 davera-017/TornadoCliffWalking Description-Content-Type: text/markdown #
 **Tornado Cliff Walking**
-                           [Sublime's custom image]
+                         [TonadoCliffWalking Example]
 Cliff Walking with Tornados is a variation of the original Cliff Walking
 environment. It involves crossing a grid world while simultaneously avoiding
 falling off a cliff and encountering a tornado which blows away the character
 to a random square in the grid (including the cliff). ## Description The game
 starts with the Elf at the top left corner of a gridworld (`i.e. [0,0]`). The
 goal location is always at the bottom right corner (`i.e. [-1,-1]`), and if the
 Elf reaches the goal the episode ends. A cliff runs along the middle of the
```

