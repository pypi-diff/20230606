# Comparing `tmp/cursesplus-2.3.4.tar.gz` & `tmp/cursesplus-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.4.tar", last modified: Tue Jun  6 20:33:55 2023, max compression
+gzip compressed data, was "cursesplus-2.3.5.tar", last modified: Tue Jun  6 20:37:32 2023, max compression
```

## Comparing `cursesplus-2.3.4.tar` & `cursesplus-2.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.017798 cursesplus-2.3.4/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.4/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1494 2023-06-06 20:33:55.007798 cursesplus-2.3.4/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      891 2023-06-06 20:33:46.000000 cursesplus-2.3.4/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-06 20:33:00.000000 cursesplus-2.3.4/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-06 20:33:55.017798 cursesplus-2.3.4/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.007798 cursesplus-2.3.4/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      320 2023-06-06 20:31:54.000000 cursesplus-2.3.4/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.007798 cursesplus-2.3.4/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.4/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    16322 2023-06-06 20:32:41.000000 cursesplus-2.3.4/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.4/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.4/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.007798 cursesplus-2.3.4/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1494 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:37:32.277797 cursesplus-2.3.5/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.5/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1499 2023-06-06 20:37:32.277797 cursesplus-2.3.5/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      896 2023-06-06 20:37:23.000000 cursesplus-2.3.5/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-06 20:36:58.000000 cursesplus-2.3.5/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-06 20:37:32.277797 cursesplus-2.3.5/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:37:32.277797 cursesplus-2.3.5/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      316 2023-06-06 20:35:39.000000 cursesplus-2.3.5/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:37:32.277797 cursesplus-2.3.5/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.5/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    16455 2023-06-06 20:36:36.000000 cursesplus-2.3.5/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.5/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.5/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:37:32.277797 cursesplus-2.3.5/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1499 2023-06-06 20:37:32.000000 cursesplus-2.3.5/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-06 20:37:32.000000 cursesplus-2.3.5/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-06 20:37:32.000000 cursesplus-2.3.5/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-06 20:37:32.000000 cursesplus-2.3.5/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.4/LICENSE` & `cursesplus-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.4/PKG-INFO` & `cursesplus-2.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.4
+Version: 2.3.5
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.4:
+### Patch 2.3.5:
 
--Add ability to use password characters instead of plain text
+-Add ability to not include empty newlines in multiline text input
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.4/README.md` & `cursesplus-2.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.4:
+### Patch 2.3.5:
 
--Add ability to use password characters instead of plain text
+-Add ability to not include empty newlines in multiline text input
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.4/pyproject.toml` & `cursesplus-2.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.4"
+version = "2.3.5"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.4/src/cursesplus/__init__.py` & `cursesplus-2.3.5/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.4/src/cursesplus/cp.py` & `cursesplus-2.3.5/src/cursesplus/cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,17 @@
     return [l for l in input if str(l) != ""]  
 def __calc_nbl_list(input:list)->int:
     x = 0
     for ls in input:
         x += len(ls)
     return x
 
-def cursesinput(stdscr,prompt: str,lines=1,maxlen=0,passwordchar:str|None=None) -> str:
+def cursesinput(stdscr,prompt: str,lines=1,maxlen=0,passwordchar:str|None=None,retremptylines=False) -> str:
     """
-    Get input from the user. Set maxlen to 0 for no maximum. Set passwordchar to None for no password entry
+    Get input from the user. Set maxlen to 0 for no maximum. Set passwordchar to None for no password entry. Retremptylines is if the program should return newlines even if the lines are empty
     """
     ERROR = ""
     if passwordchar is not None:
         passworduse = True
     else:
         passworduse = False
 
@@ -207,15 +207,15 @@
                 ERROR = " You have reached the top of the text "
                 curses.beep()
         else:
             if len(chn) > 1:
                 #Special char
                 if chn == b"^D":
                     stdscr.erase()
-                    return "\n".join(["".join(t) for t in text])
+                    return "\n".join([lx for lx in ["".join(t) for t in text] if lx != ""])
                 elif chn == b"^K":
                     text = [[] for _ in range(lines)]#Delete
                     ln = 0
                     col = 0
                     stdscr.erase()
             else:
                 #append
```

### Comparing `cursesplus-2.3.4/src/cursesplus/filedialog.py` & `cursesplus-2.3.5/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.4/src/cursesplus/messagebox.py` & `cursesplus-2.3.5/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.4/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.5/src/cursesplus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.4
+Version: 2.3.5
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.4:
+### Patch 2.3.5:
 
--Add ability to use password characters instead of plain text
+-Add ability to not include empty newlines in multiline text input
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

