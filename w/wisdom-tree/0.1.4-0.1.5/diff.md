# Comparing `tmp/wisdom-tree-0.1.4.tar.gz` & `tmp/wisdom-tree-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisdom-tree-0.1.4.tar", last modified: Fri Nov 19 06:57:14 2021, max compression
+gzip compressed data, was "wisdom-tree-0.1.5.tar", last modified: Tue Jun  6 17:22:57 2023, max compression
```

## Comparing `wisdom-tree-0.1.4.tar` & `wisdom-tree-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 hacker097  (1000) hacker097  (1000)        0 2021-11-19 06:57:14.203550 wisdom-tree-0.1.4/
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)     1066 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/LICENSE
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)      117 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/MANIFEST.in
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)     5623 2021-11-19 06:57:14.203550 wisdom-tree-0.1.4/PKG-INFO
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)     3584 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/README.md
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       38 2021-11-19 06:57:14.203550 wisdom-tree-0.1.4/setup.cfg
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)     8553 2021-11-19 06:56:46.000000 wisdom-tree-0.1.4/setup.py
-drwxrwxr-x   0 hacker097  (1000) hacker097  (1000)        0 2021-11-19 06:57:14.183558 wisdom-tree-0.1.4/wisdom_tree/
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       44 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/__init__.py
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)     4211 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/edit_quotes.py
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)    33082 2021-11-19 06:54:09.000000 wisdom-tree-0.1.4/wisdom_tree/main.py
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)   302977 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/qts.txt
-drwxrwxr-x   0 hacker097  (1000) hacker097  (1000)        0 2021-11-19 06:57:14.203550 wisdom-tree-0.1.4/wisdom_tree/res/
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)  1325622 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/alarm.wav
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)   738851 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/forest.ogg
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)   828761 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/forest2.ogg
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)  1116740 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/growth.waw
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)    84480 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/logo_512x512.png
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)        4 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p1.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)        7 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p2.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)        8 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p3.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       15 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p4.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       26 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p5.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       46 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p6.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)      102 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p7.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)      205 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p8.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)      244 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/p9.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)   924377 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/rain.ogg
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)      865 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/rain1.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)        4 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/seed.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)   493892 2021-11-19 06:50:46.000000 wisdom-tree-0.1.4/wisdom_tree/res/timerstart.wav
-drwxrwxr-x   0 hacker097  (1000) hacker097  (1000)        0 2021-11-19 06:57:14.187556 wisdom-tree-0.1.4/wisdom_tree.egg-info/
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)     5623 2021-11-19 06:57:12.000000 wisdom-tree-0.1.4/wisdom_tree.egg-info/PKG-INFO
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)      796 2021-11-19 06:57:12.000000 wisdom-tree-0.1.4/wisdom_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)        1 2021-11-19 06:57:12.000000 wisdom-tree-0.1.4/wisdom_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       53 2021-11-19 06:57:12.000000 wisdom-tree-0.1.4/wisdom_tree.egg-info/entry_points.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       18 2021-11-19 06:57:12.000000 wisdom-tree-0.1.4/wisdom_tree.egg-info/requires.txt
--rw-rw-r--   0 hacker097  (1000) hacker097  (1000)       12 2021-11-19 06:57:12.000000 wisdom-tree-0.1.4/wisdom_tree.egg-info/top_level.txt
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:22:57.437276 wisdom-tree-0.1.5/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     1066 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/LICENSE
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      117 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/MANIFEST.in
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4933 2023-06-06 17:22:57.437276 wisdom-tree-0.1.5/PKG-INFO
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4008 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/README.md
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       38 2023-06-06 17:22:57.437276 wisdom-tree-0.1.5/setup.cfg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     8553 2023-06-06 17:19:59.000000 wisdom-tree-0.1.5/setup.py
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:22:57.397276 wisdom-tree-0.1.5/wisdom_tree/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       44 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/__init__.py
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4211 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/edit_quotes.py
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)    33094 2023-06-06 17:06:34.000000 wisdom-tree-0.1.5/wisdom_tree/main.py
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   302977 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/qts.txt
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:22:57.433943 wisdom-tree-0.1.5/wisdom_tree/res/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)  1325622 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/alarm.wav
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   738851 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/forest.ogg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   828761 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/forest2.ogg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)  1116740 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/growth.waw
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)    84480 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/logo_512x512.png
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        4 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p1.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        7 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p2.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        8 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p3.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       15 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p4.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       26 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p5.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       46 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p6.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      102 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p7.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      205 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p8.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      244 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/p9.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   924377 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/rain.ogg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      865 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/rain1.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        4 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/seed.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   493892 2023-06-06 15:22:14.000000 wisdom-tree-0.1.5/wisdom_tree/res/timerstart.wav
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:22:57.400609 wisdom-tree-0.1.5/wisdom_tree.egg-info/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4933 2023-06-06 17:22:57.000000 wisdom-tree-0.1.5/wisdom_tree.egg-info/PKG-INFO
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      796 2023-06-06 17:22:57.000000 wisdom-tree-0.1.5/wisdom_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        1 2023-06-06 17:22:57.000000 wisdom-tree-0.1.5/wisdom_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       52 2023-06-06 17:22:57.000000 wisdom-tree-0.1.5/wisdom_tree.egg-info/entry_points.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       18 2023-06-06 17:22:57.000000 wisdom-tree-0.1.5/wisdom_tree.egg-info/requires.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       12 2023-06-06 17:22:57.000000 wisdom-tree-0.1.5/wisdom_tree.egg-info/top_level.txt
```

### Comparing `wisdom-tree-0.1.4/LICENSE` & `wisdom-tree-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/README.md` & `wisdom-tree-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 <h3 align="center"><img src="wisdom_tree/res/logo_512x512.png" alt="wisdom-tree"><br>Wisdom Tree</h3>
 
+<p align="center">
+
+[![Downloads](https://pepy.tech/badge/wisdom-tree)](https://pepy.tech/project/wisdom-tree)
+[![Downloads](https://pepy.tech/badge/wisdom-tree/month)](https://pepy.tech/project/wisdom-tree)
+[![Downloads](https://pepy.tech/badge/wisdom-tree/week)](https://pepy.tech/project/wisdom-tree)
+
+</p>
 
 Wisdom Tree is a tui concentration app. Inspired by the wisdom tree in Plants vs. Zombies which gives in-game tips when it grows, Wisdom Tree gives you real life tips when it grows. How can you grow the tree? by concentrating!
 
+# Showcase
+https://user-images.githubusercontent.com/38581702/235925233-1abe0e76-da53-41a7-9219-48686aab879c.mp4
+
 
 # Screenshots
 ![alt text](https://imgur.com/nFw46EN.png)
 ![alt text](https://imgur.com/Q1rGccM.png)
 ![alt text](https://imgur.com/VvRaLYd.png)
 ![alt text](https://imgur.com/MJCkdMb.png)
```

### Comparing `wisdom-tree-0.1.4/setup.py` & `wisdom-tree-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PE 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.4',  # Required
+    version='0.1.5',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A tui concentration app',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `wisdom-tree-0.1.4/wisdom_tree/edit_quotes.py` & `wisdom-tree-0.1.5/wisdom_tree/edit_quotes.py`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/main.py` & `wisdom-tree-0.1.5/wisdom_tree/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import random
 import pickle
 from pathlib import Path
 from pytube import YouTube, Playlist
 import re
 import urllib.request
 import threading
+import asyncio
 import vlc
 
 os.environ['VLC_VERBOSE'] = '-1'
 
 RES_FOLDER = Path(__file__).parent / "res"
 QUOTE_FOLDER = Path(__file__).parent
 QUOTE_FILE_NAME = "qts.txt"
@@ -187,63 +188,89 @@
             tree1.radiomode = False
             tree1.music_list_num += 1
             if tree1.music_list_num > len(tree1.music_list) - 1:
                 tree1.music_list_num = len(tree1.music_list) - 1
             tree1.media.stop()
             tree1.media = vlc.MediaPlayer(tree1.music_list[tree1.music_list_num])
             tree1.media.play()
-            tree1.show_music = True
-            tree1.musichidetime = int(time.time()) + 5
+            if os.name == "posix":
+                tree1.notifystring = (
+                    "Playing: "
+                    + str(tree1.music_list[tree1.music_list_num]).split("/")[-1]
+                )
+            else:
+                tree1.notifystring = (
+                    "Playing: "
+                    + str(tree1.music_list[tree1.music_list_num]).split('\\')[-1]
+                )
 
+            tree1.notifyendtime = int(time.time()) + 5
+            tree1.isnotify = True
+            
     if key in (curses.KEY_LEFT, ord("h")):
         if tree1.showtimer:
             tree1.selectedtimer = 0
             tree1.currentmenu = "timer"
         else:
             tree1.radiomode = False
             tree1.music_list_num -= 1
             if tree1.music_list_num < 0:
                 tree1.music_list_num = 0
             tree1.media.stop()
             tree1.media = vlc.MediaPlayer(tree1.music_list[tree1.music_list_num])
             tree1.media.play()
-            tree1.show_music = True
-            tree1.musichidetime = int(time.time()) + 5
+            if os.name == "posix":
+                tree1.notifystring = (
+                    "Playing: "
+                    + str(tree1.music_list[tree1.music_list_num]).split("/")[-1]
+                )
+            else:
+                tree1.notifystring = (
+                    "Playing: "
+                    + str(tree1.music_list[tree1.music_list_num]).split('\\')[-1]
+                )
+
+            tree1.notifyendtime = int(time.time()) + 5
+            tree1.isnotify = True
 
     if key == ord(" "):
         if tree1.media.is_playing():
             tree1.media.pause()
         tree1.pause = True
         tree1.pausetime = time.time()
 
-    if key == ord("m"):
-        tree1.media.pause()
+        if key == ord("m"):
+            tree1.media.pause()
 
     if not tree1.isloading and key == ord("n"):
         tree1.lofiradio()
 
     if key == ord("]"):
-        tree1.media.audio_set_volume(min(100, tree1.media.audio_get_volume()+1))
+        new_volume = tree1.media.audio_get_volume()+1
+        
+        tree1.media.audio_set_volume(min(100, new_volume))
         tree1.notifyendtime = int(time.time()) + 2
-        volume = str(round(tree1.media.audio_get_volume())) + "%"
-        tree1.notifystring = " "*round(maxx*(tree1.media.audio_get_volume()/100)-len(volume)-2) + volume
+        volumeStr = str(round(new_volume)) + "%"
+
+        tree1.notifystring = " "*round(maxx*(new_volume/100)-len(volumeStr)-2) + volumeStr
         tree1.invert = True
         tree1.isnotify = True
 
     if key == ord("["):
-        tree1.media.audio_set_volume(max(0, tree1.media.audio_get_volume()-1))
+        new_volume = tree1.media.audio_get_volume()-1
+        
+        tree1.media.audio_set_volume(min(100, new_volume))
         tree1.notifyendtime = int(time.time()) + 2
-        volume = str(round(tree1.media.audio_get_volume())) + "%"
-        tree1.notifystring = " "*round(maxx*(tree1.media.audio_get_volume()/100)-len(volume)-2) + volume
+        volumeStr = str(round(new_volume)) + "%"
 
+        tree1.notifystring = " "*round(maxx*(new_volume/100)-len(volumeStr)-2) + volumeStr
         tree1.invert = True
         tree1.isnotify = True
-        tree1.media.audio_set_volume(max(0, tree1.media.audio_get_volume()-1))
-        tree1.notifyendtime = int(time.time()) + 2
 
+        
     if key == ord("}"):
         effect_volume = min(100, effect_volume+1)
 
         tree1.notifyendtime = int(time.time()) + 2
 
         volume = str(effect_volume) + "%"
         tree1.notifystring = " "*round(maxx*(effect_volume/100)-len(volume)-2) + volume
@@ -366,15 +393,14 @@
         ]
         self.currentmenu = "timer"
         self.selectedtimer = 0
         self.istimer = False
         self.isbreak = False
         self.breakover = False
         self.timerhidetime = 0
-        self.musichidetime = 0
         random.seed(int(time.time() / (60 * 60 * 24)))
         self.season = random.choice(
             ["rain", "heavy_rain", "light_rain", "snow", "windy"]
         )
         random.seed()
         self.youtubedisplay = False
         self.downloaddisplay = False
@@ -687,15 +713,15 @@
             stdscr.addstr(1,1, "GETTING AUDIO  " + spinner[int(self.spinnerstate)])
 
 
 
     def youtube(self, stdscr, maxx):
         if self.youtubedisplay:
             curses.textpad.rectangle(stdscr, 0,0,2, maxx-1)
-            stdscr.addstr(1,1, "ENTER SEARCH QUERY/LINK : ")
+            stdscr.addstr(1,1, "SEARCH [type 'q' to exit]: ")
             stdscr.refresh()
 
             if not "songinput" in locals():
 
                 curses.echo()
                 curses.nocbreak()
                 stdscr.nodelay(False)
@@ -706,28 +732,27 @@
 
                 curses.noecho()
                 curses.cbreak()
                 stdscr.nodelay(True)
                 stdscr.keypad(True)
                 curses.curs_set(0)
 
+            if not songinput == "q":
+                stdscr.addstr(1,1, "GETTING AUDIO")
 
-            stdscr.addstr(1,1, "GETTING AUDIO")
-
-            getsongthread = threading.Thread(target=self.playyoutube, args=(songinput,))
-            getsongthread.daemon = True
-            getsongthread.start()
+                getsongthread = threading.Thread(target=self.playyoutube, args=(songinput,))
+                getsongthread.daemon = True
+                getsongthread.start()
 
-            self.youtubedisplay = False
-
-            self.downloaddisplay = True
+                self.downloaddisplay = True
 
             del songinput
 
-
+            self.youtubedisplay = False
+            
 
         if self.downloaddisplay:
             self.loading(stdscr, maxx)
 
 
     def playyoutube(self, songinput):
 
@@ -773,53 +798,47 @@
             self.notifystring = "UNABLE TO CONNECT, PLEASE CHECK INTERNET CONNECTION"
             self.invert = False
             self.isnotify = True
             self.radiomode = False
             exit()
       
 
-    def lofiradio(self):
-         #lofi playlist from youtube
-
+    def lofiradio(self): #lofi playlist from youtube
+        if self.isloading:
+            return 
+        
         self.media.stop()
 
         self.isloading = True
         self.radiomode = True
 
         radiothread = threading.Thread(target=self.actuallofiradio)
         radiothread.daemon = True
         radiothread.start()
 
 
     def actuallofiradio(self):
-
-
         if not hasattr(self, "lofisong"):
             self.lofisong = self.getlofisong()
 
         if self.lofisong == "ERROR":
             exit()
 
-
         self.media = vlc.MediaPlayer(self.lofisong)
         self.media.play()
-
+        
         self.notifyendtime = int(time.time()) + 10
         self.notifystring = "Playing: " + YouTube(self.lofilink).title
         self.invert = False
         self.isnotify = True
 
         self.lofisong = self.getlofisong()
 
         self.isloading = False
 
-
-
-
-
 def main():
     run = True
     stdscr = curses.initscr()
     stdscr.nodelay(True)
     stdscr.keypad(True)
     curses.curs_set(0)
     curses.start_color()
@@ -856,15 +875,15 @@
     music_volume_max = 1
 
     quote = getqt()
     play_sound(GROWTH_SOUND)
 
     tree1 = tree(stdscr, 1)
     tree1.media.play()
-
+    
     try:
 
         treedata_in = open(RES_FOLDER/ "treedata", "rb")
         tree1.age = pickle.load(treedata_in)
 
     except:
 
@@ -880,42 +899,22 @@
                 stdscr.erase()
                 maxy, maxx = stdscr.getmaxyx()
 
                 addtext(int(maxx / 2), int(maxy * 5 / 6), quote, anilen, stdscr, 2)
                 anilen += anispeed
                 if anilen > 150:
                     anilen = 150
-
+                    
                 if (seconds % (100 * 60 * 10) == 0):  # show another quote every 5 min, and grow tree
                     quote = getqt()
                     tree1.age += 1
                     anilen = 1
                     play_sound(GROWTH_SOUND)
 
-                if tree1.musichidetime <= int(time.time()):
-                    tree1.show_music = False
-
-                if tree1.show_music:
-                    if os.name == "posix":
-                        showtext = (
-                            "Playing: "
-                            + str(tree1.music_list[tree1.music_list_num]).split("/")[-1]
-                        )
-                    else:
-                        showtext = (
-                            "Playing: "
-                            + str(tree1.music_list[tree1.music_list_num]).split('\\')[-1]
-                        )
-                    stdscr.addstr(
-                        int(maxy / 10),
-                        int(maxx / 2 - len(showtext) / 2),
-                        showtext,
-                        curses.A_BOLD,
-                    )
-
+      
                 tree1.display(maxx, maxy, seconds)
 
                 tree1.seasons(maxx, maxy, seconds)
 
                 tree1.menudisplay(stdscr, maxy, maxx)
 
                 tree1.youtube(stdscr, maxx)
@@ -954,14 +953,15 @@
                         tree1.pause = False
                         tree1.media.play()
                         stdscr.refresh()
                         if tree1.istimer:
                             tree1.workendtime += time.time() - tree1.pausetime
 
                     if key == ord("q"):
+
                         treedata = open(RES_FOLDER / "treedata", "wb")
                         pickle.dump(tree1.age, treedata, protocol=None)
                         treedata.close()
                         exit()
 
                     time.sleep(0.1)
```

### Comparing `wisdom-tree-0.1.4/wisdom_tree/qts.txt` & `wisdom-tree-0.1.5/wisdom_tree/qts.txt`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/alarm.wav` & `wisdom-tree-0.1.5/wisdom_tree/res/alarm.wav`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/forest.ogg` & `wisdom-tree-0.1.5/wisdom_tree/res/forest.ogg`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/forest2.ogg` & `wisdom-tree-0.1.5/wisdom_tree/res/forest2.ogg`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/growth.waw` & `wisdom-tree-0.1.5/wisdom_tree/res/growth.waw`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/logo_512x512.png` & `wisdom-tree-0.1.5/wisdom_tree/res/logo_512x512.png`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/rain.ogg` & `wisdom-tree-0.1.5/wisdom_tree/res/rain.ogg`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree/res/timerstart.wav` & `wisdom-tree-0.1.5/wisdom_tree/res/timerstart.wav`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.4/wisdom_tree.egg-info/SOURCES.txt` & `wisdom-tree-0.1.5/wisdom_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

