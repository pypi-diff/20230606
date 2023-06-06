# Comparing `tmp/pycman_dna-0.0.5.tar.gz` & `tmp/pycman_dna-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycman_dna-0.0.5.tar", last modified: Tue Jun  6 13:10:38 2023, max compression
+gzip compressed data, was "pycman_dna-0.0.6.tar", last modified: Tue Jun  6 13:12:48 2023, max compression
```

## Comparing `pycman_dna-0.0.5.tar` & `pycman_dna-0.0.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:10:38.795235 pycman_dna-0.0.5/
--rw-rw-rw-   0        0        0      533 2023-06-06 13:10:38.794735 pycman_dna-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-06 12:04:16.000000 pycman_dna-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:10:38.753699 pycman_dna-0.0.5/pycman_dna/
--rw-rw-rw-   0        0        0     8713 2023-02-26 17:49:35.000000 pycman_dna-0.0.5/pycman_dna/Map.py
--rw-rw-rw-   0        0        0     8782 2023-02-26 19:15:52.000000 pycman_dna-0.0.5/pycman_dna/PacmanGame.py
--rw-rw-rw-   0        0        0      600 2023-06-06 13:10:09.000000 pycman_dna-0.0.5/pycman_dna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:10:38.770213 pycman_dna-0.0.5/pycman_dna/images/
--rw-rw-rw-   0        0        0     1017 2022-12-27 20:43:36.000000 pycman_dna-0.0.5/pycman_dna/images/PacmanDEAD.png
--rw-rw-rw-   0        0        0     1113 2022-12-27 20:42:03.000000 pycman_dna-0.0.5/pycman_dna/images/PacmanDOWN.png
--rw-rw-rw-   0        0        0     1075 2022-12-27 20:41:37.000000 pycman_dna-0.0.5/pycman_dna/images/PacmanLEFT.png
--rw-rw-rw-   0        0        0     1046 2022-12-27 20:41:03.000000 pycman_dna-0.0.5/pycman_dna/images/PacmanRIGHT.png
--rw-rw-rw-   0        0        0     1143 2022-12-27 20:42:21.000000 pycman_dna-0.0.5/pycman_dna/images/PacmanUP.png
--rw-rw-rw-   0        0        0     5042 2022-12-27 13:53:45.000000 pycman_dna-0.0.5/pycman_dna/images/dot.png
--rw-rw-rw-   0        0        0     6849 2022-12-29 13:05:19.000000 pycman_dna-0.0.5/pycman_dna/images/eatable_ghost.png
--rw-rw-rw-   0        0        0     7058 2022-12-29 13:05:23.000000 pycman_dna-0.0.5/pycman_dna/images/ghost.png
--rw-rw-rw-   0        0        0     9959 2023-01-08 22:17:03.000000 pycman_dna-0.0.5/pycman_dna/images/icon.png
--rw-rw-rw-   0        0        0     5684 2022-12-27 13:53:40.000000 pycman_dna-0.0.5/pycman_dna/images/pill.png
--rw-rw-rw-   0        0        0      650 2022-12-27 20:33:08.000000 pycman_dna-0.0.5/pycman_dna/images/wall.png
-drwxrwxrwx   0        0        0        0 2023-06-06 13:10:38.794235 pycman_dna-0.0.5/pycman_dna/maps/
--rw-rw-rw-   0        0        0      452 2022-12-28 15:29:03.000000 pycman_dna-0.0.5/pycman_dna/maps/all_along_the_watchtowers.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:30:08.000000 pycman_dna-0.0.5/pycman_dna/maps/all_along_the_watchtowers_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:45:47.000000 pycman_dna-0.0.5/pycman_dna/maps/bimble.map
--rw-rw-rw-   0        0        0      453 2023-01-21 16:43:24.000000 pycman_dna-0.0.5/pycman_dna/maps/blank.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:46:41.000000 pycman_dna-0.0.5/pycman_dna/maps/broken_line_1.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:47:27.000000 pycman_dna-0.0.5/pycman_dna/maps/broken_line_2.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:47:47.000000 pycman_dna-0.0.5/pycman_dna/maps/broken_line_3.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:48:13.000000 pycman_dna-0.0.5/pycman_dna/maps/central_cavern.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:48:54.000000 pycman_dna-0.0.5/pycman_dna/maps/central_cavern_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:49:18.000000 pycman_dna-0.0.5/pycman_dna/maps/dizzy.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:49:36.000000 pycman_dna-0.0.5/pycman_dna/maps/easy_does_it.map
--rw-rw-rw-   0        0        0      451 2022-12-29 12:17:24.000000 pycman_dna-0.0.5/pycman_dna/maps/first_steps.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:50:27.000000 pycman_dna-0.0.5/pycman_dna/maps/follow_the_yellow_brick_road.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:50:45.000000 pycman_dna-0.0.5/pycman_dna/maps/ghost_train.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:51:06.000000 pycman_dna-0.0.5/pycman_dna/maps/i_smell_your_fear.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:51:46.000000 pycman_dna-0.0.5/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:52:13.000000 pycman_dna-0.0.5/pycman_dna/maps/killing_time.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:53:04.000000 pycman_dna-0.0.5/pycman_dna/maps/maze.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:53:33.000000 pycman_dna-0.0.5/pycman_dna/maps/number_one_the_larch.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:53:59.000000 pycman_dna-0.0.5/pycman_dna/maps/on_the_outside.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:54:27.000000 pycman_dna-0.0.5/pycman_dna/maps/on_the_outside_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:54:49.000000 pycman_dna-0.0.5/pycman_dna/maps/ping_pong.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:55:12.000000 pycman_dna-0.0.5/pycman_dna/maps/sense_your_way.map
--rw-rw-rw-   0        0        0      454 2022-12-28 15:24:10.000000 pycman_dna-0.0.5/pycman_dna/maps/teeth.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:55:33.000000 pycman_dna-0.0.5/pycman_dna/maps/unbroken_line_1.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:55:57.000000 pycman_dna-0.0.5/pycman_dna/maps/unbroken_line_2.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:56:19.000000 pycman_dna-0.0.5/pycman_dna/maps/unbroken_line_3.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:56:41.000000 pycman_dna-0.0.5/pycman_dna/maps/valid_symbols.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:58:05.000000 pycman_dna-0.0.5/pycman_dna/maps/you_make_me_feel_like_dancing.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:57:35.000000 pycman_dna-0.0.5/pycman_dna/maps/you_will_blink_first.map
-drwxrwxrwx   0        0        0        0 2023-06-06 13:10:38.761705 pycman_dna-0.0.5/pycman_dna.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-06 13:10:38.000000 pycman_dna-0.0.5/pycman_dna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1694 2023-06-06 13:10:38.000000 pycman_dna-0.0.5/pycman_dna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:10:38.000000 pycman_dna-0.0.5/pycman_dna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 13:10:38.000000 pycman_dna-0.0.5/pycman_dna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 13:10:38.000000 pycman_dna-0.0.5/pycman_dna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 13:10:38.795235 pycman_dna-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1156 2023-06-06 13:10:26.000000 pycman_dna-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.629801 pycman_dna-0.0.6/
+-rw-rw-rw-   0        0        0      533 2023-06-06 13:12:48.629801 pycman_dna-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-06 12:04:16.000000 pycman_dna-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.587759 pycman_dna-0.0.6/pycman_dna/
+-rw-rw-rw-   0        0        0     8713 2023-02-26 17:49:35.000000 pycman_dna-0.0.6/pycman_dna/Map.py
+-rw-rw-rw-   0        0        0     8784 2023-06-06 13:12:11.000000 pycman_dna-0.0.6/pycman_dna/PacmanGame.py
+-rw-rw-rw-   0        0        0      600 2023-06-06 13:10:09.000000 pycman_dna-0.0.6/pycman_dna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.605776 pycman_dna-0.0.6/pycman_dna/images/
+-rw-rw-rw-   0        0        0     1017 2022-12-27 20:43:36.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanDEAD.png
+-rw-rw-rw-   0        0        0     1113 2022-12-27 20:42:03.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanDOWN.png
+-rw-rw-rw-   0        0        0     1075 2022-12-27 20:41:37.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanLEFT.png
+-rw-rw-rw-   0        0        0     1046 2022-12-27 20:41:03.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanRIGHT.png
+-rw-rw-rw-   0        0        0     1143 2022-12-27 20:42:21.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanUP.png
+-rw-rw-rw-   0        0        0     5042 2022-12-27 13:53:45.000000 pycman_dna-0.0.6/pycman_dna/images/dot.png
+-rw-rw-rw-   0        0        0     6849 2022-12-29 13:05:19.000000 pycman_dna-0.0.6/pycman_dna/images/eatable_ghost.png
+-rw-rw-rw-   0        0        0     7058 2022-12-29 13:05:23.000000 pycman_dna-0.0.6/pycman_dna/images/ghost.png
+-rw-rw-rw-   0        0        0     9959 2023-01-08 22:17:03.000000 pycman_dna-0.0.6/pycman_dna/images/icon.png
+-rw-rw-rw-   0        0        0     5684 2022-12-27 13:53:40.000000 pycman_dna-0.0.6/pycman_dna/images/pill.png
+-rw-rw-rw-   0        0        0      650 2022-12-27 20:33:08.000000 pycman_dna-0.0.6/pycman_dna/images/wall.png
+drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.628801 pycman_dna-0.0.6/pycman_dna/maps/
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:29:03.000000 pycman_dna-0.0.6/pycman_dna/maps/all_along_the_watchtowers.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:30:08.000000 pycman_dna-0.0.6/pycman_dna/maps/all_along_the_watchtowers_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:45:47.000000 pycman_dna-0.0.6/pycman_dna/maps/bimble.map
+-rw-rw-rw-   0        0        0      453 2023-01-21 16:43:24.000000 pycman_dna-0.0.6/pycman_dna/maps/blank.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:46:41.000000 pycman_dna-0.0.6/pycman_dna/maps/broken_line_1.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:47:27.000000 pycman_dna-0.0.6/pycman_dna/maps/broken_line_2.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:47:47.000000 pycman_dna-0.0.6/pycman_dna/maps/broken_line_3.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:48:13.000000 pycman_dna-0.0.6/pycman_dna/maps/central_cavern.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:48:54.000000 pycman_dna-0.0.6/pycman_dna/maps/central_cavern_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:49:18.000000 pycman_dna-0.0.6/pycman_dna/maps/dizzy.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:49:36.000000 pycman_dna-0.0.6/pycman_dna/maps/easy_does_it.map
+-rw-rw-rw-   0        0        0      451 2022-12-29 12:17:24.000000 pycman_dna-0.0.6/pycman_dna/maps/first_steps.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:50:27.000000 pycman_dna-0.0.6/pycman_dna/maps/follow_the_yellow_brick_road.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:50:45.000000 pycman_dna-0.0.6/pycman_dna/maps/ghost_train.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:51:06.000000 pycman_dna-0.0.6/pycman_dna/maps/i_smell_your_fear.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:51:46.000000 pycman_dna-0.0.6/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:52:13.000000 pycman_dna-0.0.6/pycman_dna/maps/killing_time.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:53:04.000000 pycman_dna-0.0.6/pycman_dna/maps/maze.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:53:33.000000 pycman_dna-0.0.6/pycman_dna/maps/number_one_the_larch.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:53:59.000000 pycman_dna-0.0.6/pycman_dna/maps/on_the_outside.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:54:27.000000 pycman_dna-0.0.6/pycman_dna/maps/on_the_outside_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:54:49.000000 pycman_dna-0.0.6/pycman_dna/maps/ping_pong.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:55:12.000000 pycman_dna-0.0.6/pycman_dna/maps/sense_your_way.map
+-rw-rw-rw-   0        0        0      454 2022-12-28 15:24:10.000000 pycman_dna-0.0.6/pycman_dna/maps/teeth.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:55:33.000000 pycman_dna-0.0.6/pycman_dna/maps/unbroken_line_1.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:55:57.000000 pycman_dna-0.0.6/pycman_dna/maps/unbroken_line_2.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:56:19.000000 pycman_dna-0.0.6/pycman_dna/maps/unbroken_line_3.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:56:41.000000 pycman_dna-0.0.6/pycman_dna/maps/valid_symbols.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:58:05.000000 pycman_dna-0.0.6/pycman_dna/maps/you_make_me_feel_like_dancing.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:57:35.000000 pycman_dna-0.0.6/pycman_dna/maps/you_will_blink_first.map
+drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.597268 pycman_dna-0.0.6/pycman_dna.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1694 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 13:12:48.630302 pycman_dna-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2023-06-06 13:12:42.000000 pycman_dna-0.0.6/setup.py
```

### Comparing `pycman_dna-0.0.5/PKG-INFO` & `pycman_dna-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman_dna
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.0.5/pycman_dna/Map.py` & `pycman_dna-0.0.6/pycman_dna/Map.py`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/PacmanGame.py` & `pycman_dna-0.0.6/pycman_dna/PacmanGame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from tkinter import simpledialog;
 import time;
 import threading, sys, os;
 
-from Map import Map;
-from Map import Direction;
+from .Map import Map;
+from .Map import Direction;
 
 class PacmanGame:
     """
     PacmanGame's base constructor method. Performs initial setup.
     """
     __update_rate = 0.25;
     __moves_taken = 0;
```

### Comparing `pycman_dna-0.0.5/pycman_dna/__init__.py` & `pycman_dna-0.0.6/pycman_dna/__init__.py`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/PacmanDEAD.png` & `pycman_dna-0.0.6/pycman_dna/images/PacmanDEAD.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/PacmanDOWN.png` & `pycman_dna-0.0.6/pycman_dna/images/PacmanDOWN.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/PacmanLEFT.png` & `pycman_dna-0.0.6/pycman_dna/images/PacmanLEFT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/PacmanRIGHT.png` & `pycman_dna-0.0.6/pycman_dna/images/PacmanRIGHT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/PacmanUP.png` & `pycman_dna-0.0.6/pycman_dna/images/PacmanUP.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/dot.png` & `pycman_dna-0.0.6/pycman_dna/images/dot.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/eatable_ghost.png` & `pycman_dna-0.0.6/pycman_dna/images/eatable_ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/ghost.png` & `pycman_dna-0.0.6/pycman_dna/images/ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/icon.png` & `pycman_dna-0.0.6/pycman_dna/images/icon.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/pill.png` & `pycman_dna-0.0.6/pycman_dna/images/pill.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna/images/wall.png` & `pycman_dna-0.0.6/pycman_dna/images/wall.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/pycman_dna.egg-info/PKG-INFO` & `pycman_dna-0.0.6/pycman_dna.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman-dna
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.0.5/pycman_dna.egg-info/SOURCES.txt` & `pycman_dna-0.0.6/pycman_dna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.5/setup.py` & `pycman_dna-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Python Pacman Tool'
 LONG_DESCRIPTION = 'A teaching tool based on arcade icon Pacman, written in Python.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="pycman_dna", 
         version=VERSION,
         author="Liam Burns",
         author_email="l.burns@dundeeandangus.ac.uk",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['pygame'], # add any additional packages that 
+        install_requires=['pygame', 'tkinter'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         include_package_data=True,
         package_data={'': ['maps/*', 'images/*']},
         
         keywords=['python', 'pacman'],
         classifiers= [
             "Development Status :: 3 - Alpha",
```

