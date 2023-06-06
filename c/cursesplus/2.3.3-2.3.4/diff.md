# Comparing `tmp/cursesplus-2.3.3.tar.gz` & `tmp/cursesplus-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.3.tar", last modified: Tue Jun  6 20:28:36 2023, max compression
+gzip compressed data, was "cursesplus-2.3.4.tar", last modified: Tue Jun  6 20:33:55 2023, max compression
```

## Comparing `cursesplus-2.3.3.tar` & `cursesplus-2.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.627800 cursesplus-2.3.3/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.3/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1479 2023-06-06 20:28:36.627800 cursesplus-2.3.3/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      876 2023-06-06 20:26:06.000000 cursesplus-2.3.3/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-06 20:25:24.000000 cursesplus-2.3.3/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-06 20:28:36.627800 cursesplus-2.3.3/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.617800 cursesplus-2.3.3/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      316 2023-06-06 20:27:17.000000 cursesplus-2.3.3/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.617800 cursesplus-2.3.3/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.3/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    16006 2023-06-06 20:28:03.000000 cursesplus-2.3.3/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.3/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.3/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:28:36.617800 cursesplus-2.3.3/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1479 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-06 20:28:36.000000 cursesplus-2.3.3/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.017798 cursesplus-2.3.4/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.4/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1494 2023-06-06 20:33:55.007798 cursesplus-2.3.4/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      891 2023-06-06 20:33:46.000000 cursesplus-2.3.4/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-06 20:33:00.000000 cursesplus-2.3.4/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-06 20:33:55.017798 cursesplus-2.3.4/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.007798 cursesplus-2.3.4/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      320 2023-06-06 20:31:54.000000 cursesplus-2.3.4/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.007798 cursesplus-2.3.4/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.4/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    16322 2023-06-06 20:32:41.000000 cursesplus-2.3.4/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.4/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.4/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-06 20:33:55.007798 cursesplus-2.3.4/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1494 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-06 20:33:54.000000 cursesplus-2.3.4/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.3/LICENSE` & `cursesplus-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.3/PKG-INFO` & `cursesplus-2.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.3
+Version: 2.3.4
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
 
-### Patch 2.3.3:
+### Patch 2.3.4:
 
--Add ability to press enter on one line inputs
+-Add ability to use password characters instead of plain text
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.3/README.md` & `cursesplus-2.3.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ### SPECIAL INSTRUCTIONS FOR WINDOWS
 
 For Windows you need to also install ```windows-curses``` or related program
 to provide the basic curses functionality
 
 ## What's New?
 
-### Patch 2.3.3:
+### Patch 2.3.4:
 
--Add ability to press enter on one line inputs
+-Add ability to use password characters instead of plain text
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

### Comparing `cursesplus-2.3.3/pyproject.toml` & `cursesplus-2.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.3"
+version = "2.3.4"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.3/src/cursesplus/__init__.py` & `cursesplus-2.3.4/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.3/src/cursesplus/cp.py` & `cursesplus-2.3.4/src/cursesplus/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,24 @@
     return [l for l in input if str(l) != ""]  
 def __calc_nbl_list(input:list)->int:
     x = 0
     for ls in input:
         x += len(ls)
     return x
 
-def cursesinput(stdscr,prompt: str,lines=1,maxlen=0) -> str:
+def cursesinput(stdscr,prompt: str,lines=1,maxlen=0,passwordchar:str|None=None) -> str:
     """
-    Get input from the user. Set maxlen to 0 for no maximum
+    Get input from the user. Set maxlen to 0 for no maximum. Set passwordchar to None for no password entry
     """
     ERROR = ""
+    if passwordchar is not None:
+        passworduse = True
+    else:
+        passworduse = False
+
     stdscr.erase()
     mx,my = os.get_terminal_size()
     extoffscr = lines > my-3
     if extoffscr:
         lnrectmaxy = my-2
     else:
         lnrectmaxy = lines+2
@@ -133,15 +138,18 @@
     while True:
         filline(stdscr,0,set_colour(WHITE,BLACK))
         stdscr.addstr(0,0,str(prompt+[" (Press ctrl-D to submit)" if lines != 1 else " (Press enter to submit)"][0])[0:mx-2],set_colour(WHITE,BLACK))
         rectangle(stdscr,1,0,lnrectmaxy,mx-1)
         chi = 1
         for chln in text:
             chi+= 1
-            stdscr.addstr(chi,1,"".join(chln)[xoffset:xoffset+mx-3])
+            if passworduse:
+                stdscr.addstr(chi,1,(passwordchar*len(chln))[xoffset:xoffset+mx-3])
+            else:
+                stdscr.addstr(chi,1,"".join(chln)[xoffset:xoffset+mx-3])
             if xoffset > 0:
                 stdscr.addstr(chi,0,"<",set_colour(BLUE,WHITE))
             if len(text[chi-2]) > xoffset + mx - 3:
                 stdscr.addstr(chi,mx-1,">",set_colour(GREEN,WHITE))
         stdscr.addstr(0,mx-10,f"{ln},{col}",set_colour(WHITE,BLACK))
         stdscr.addstr(0,30,ERROR,set_colour(WHITE,RED))
         stdscr.move(ln+2,col-xoffset+1)
```

### Comparing `cursesplus-2.3.3/src/cursesplus/filedialog.py` & `cursesplus-2.3.4/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.3/src/cursesplus/messagebox.py` & `cursesplus-2.3.4/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.3/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.3.4/src/cursesplus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.3.3
+Version: 2.3.4
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
 
-### Patch 2.3.3:
+### Patch 2.3.4:
 
--Add ability to press enter on one line inputs
+-Add ability to use password characters instead of plain text
 
 ### Version 2.3: New Input
 
 -Rewrite cursesinput function
 
 -Remains backwards-compatible
```

