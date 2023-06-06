# Comparing `tmp/cursesplus-2.3.2.tar.gz` & `tmp/cursesplus-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.2.tar", last modified: Sun Jun  4 23:47:50 2023, max compression
+gzip compressed data, was "cursesplus-2.3.3.tar", last modified: Tue Jun  6 20:28:36 2023, max compression
```

## Comparing `cursesplus-2.3.2.tar` & `cursesplus-2.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.2/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1491 2023-06-04 23:47:50.647888 cursesplus-2.3.2/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      888 2023-05-29 23:25:42.000000 cursesplus-2.3.2/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-04 23:47:15.000000 cursesplus-2.3.2/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-04 23:47:50.647888 cursesplus-2.3.2/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      317 2023-05-29 23:14:15.000000 cursesplus-2.3.2/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.2/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    15833 2023-06-04 23:47:11.000000 cursesplus-2.3.2/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.2/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.2/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-04 23:47:50.647888 cursesplus-2.3.2/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1491 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-04 23:47:50.000000 cursesplus-2.3.2/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.627800 cursesplus-2.3.3/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.3/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1479 2023-06-06 20:28:36.627800 cursesplus-2.3.3/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      876 2023-06-06 20:26:06.000000 cursesplus-2.3.3/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-06 20:25:24.000000 cursesplus-2.3.3/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-06 20:28:36.627800 cursesplus-2.3.3/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.617800 cursesplus-2.3.3/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      316 2023-06-06 20:27:17.000000 cursesplus-2.3.3/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.617800 cursesplus-2.3.3/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.3/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    16006 2023-06-06 20:28:03.000000 cursesplus-2.3.3/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.3/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.3/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.617800 cursesplus-2.3.3/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1479 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.2/LICENSE` & `cursesplus-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.2/PKG-INFO` & `cursesplus-2.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.2
+Version: 2.3.3
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.1:
+### Patch 2.3.3:
 
--Add character limit to new input
-
--Add more functionality
+-Add ability to press enter on one line inputs
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.2/README.md` & `cursesplus-2.3.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.1:
+### Patch 2.3.3:
 
--Add character limit to new input
-
--Add more functionality
+-Add ability to press enter on one line inputs
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.2/pyproject.toml` & `cursesplus-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.2"
+version = "2.3.3"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.2/src/cursesplus/__init__.py` & `cursesplus-2.3.3/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.2/src/cursesplus/cp.py` & `cursesplus-2.3.3/src/cursesplus/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         lnrectmaxy = lines+2
     text: list[list[str]] = [[] for _ in range(lines)]
     ln=0
     col=0
     xoffset = 0
     while True:
         filline(stdscr,0,set_colour(WHITE,BLACK))
-        stdscr.addstr(0,0,str(prompt+" (Press ctrl-D to submit)")[0:mx-2],set_colour(WHITE,BLACK))
+        stdscr.addstr(0,0,str(prompt+[" (Press ctrl-D to submit)" if lines != 1 else " (Press enter to submit)"][0])[0:mx-2],set_colour(WHITE,BLACK))
         rectangle(stdscr,1,0,lnrectmaxy,mx-1)
         chi = 1
         for chln in text:
             chi+= 1
             stdscr.addstr(chi,1,"".join(chln)[xoffset:xoffset+mx-3])
             if xoffset > 0:
                 stdscr.addstr(chi,0,"<",set_colour(BLUE,WHITE))
@@ -148,14 +148,17 @@
         
         if ERROR != "":
             ERROR = ""
         stdscr.refresh()
         ch = stdscr.getch()
         chn = curses.keyname(ch)
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER or ch == curses.KEY_DOWN:
+            if lines == 1:
+                stdscr.erase()
+                return "\n".join(["".join(t) for t in text])
             if ln == lines - 1:
                 ERROR = " You have reached the bottom of the page. "
                 curses.beep()
             else:
                 ln += 1
                 col = 0
         elif ch == curses.KEY_LEFT:
```

### Comparing `cursesplus-2.3.2/src/cursesplus/filedialog.py` & `cursesplus-2.3.3/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.2/src/cursesplus/messagebox.py` & `cursesplus-2.3.3/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.2/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.3/src/cursesplus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.2
+Version: 2.3.3
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.1:
+### Patch 2.3.3:
 
--Add character limit to new input
-
--Add more functionality
+-Add ability to press enter on one line inputs
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

