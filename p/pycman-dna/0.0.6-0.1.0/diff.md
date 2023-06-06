# Comparing `tmp/pycman_dna-0.0.6.tar.gz` & `tmp/pycman_dna-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycman_dna-0.0.6.tar", last modified: Tue Jun  6 13:12:48 2023, max compression
+gzip compressed data, was "pycman_dna-0.1.0.tar", last modified: Tue Jun  6 15:26:03 2023, max compression
```

## Comparing `pycman_dna-0.0.6.tar` & `pycman_dna-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.629801 pycman_dna-0.0.6/
--rw-rw-rw-   0        0        0      533 2023-06-06 13:12:48.629801 pycman_dna-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-06 12:04:16.000000 pycman_dna-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.587759 pycman_dna-0.0.6/pycman_dna/
--rw-rw-rw-   0        0        0     8713 2023-02-26 17:49:35.000000 pycman_dna-0.0.6/pycman_dna/Map.py
--rw-rw-rw-   0        0        0     8784 2023-06-06 13:12:11.000000 pycman_dna-0.0.6/pycman_dna/PacmanGame.py
--rw-rw-rw-   0        0        0      600 2023-06-06 13:10:09.000000 pycman_dna-0.0.6/pycman_dna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.605776 pycman_dna-0.0.6/pycman_dna/images/
--rw-rw-rw-   0        0        0     1017 2022-12-27 20:43:36.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanDEAD.png
--rw-rw-rw-   0        0        0     1113 2022-12-27 20:42:03.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanDOWN.png
--rw-rw-rw-   0        0        0     1075 2022-12-27 20:41:37.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanLEFT.png
--rw-rw-rw-   0        0        0     1046 2022-12-27 20:41:03.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanRIGHT.png
--rw-rw-rw-   0        0        0     1143 2022-12-27 20:42:21.000000 pycman_dna-0.0.6/pycman_dna/images/PacmanUP.png
--rw-rw-rw-   0        0        0     5042 2022-12-27 13:53:45.000000 pycman_dna-0.0.6/pycman_dna/images/dot.png
--rw-rw-rw-   0        0        0     6849 2022-12-29 13:05:19.000000 pycman_dna-0.0.6/pycman_dna/images/eatable_ghost.png
--rw-rw-rw-   0        0        0     7058 2022-12-29 13:05:23.000000 pycman_dna-0.0.6/pycman_dna/images/ghost.png
--rw-rw-rw-   0        0        0     9959 2023-01-08 22:17:03.000000 pycman_dna-0.0.6/pycman_dna/images/icon.png
--rw-rw-rw-   0        0        0     5684 2022-12-27 13:53:40.000000 pycman_dna-0.0.6/pycman_dna/images/pill.png
--rw-rw-rw-   0        0        0      650 2022-12-27 20:33:08.000000 pycman_dna-0.0.6/pycman_dna/images/wall.png
-drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.628801 pycman_dna-0.0.6/pycman_dna/maps/
--rw-rw-rw-   0        0        0      452 2022-12-28 15:29:03.000000 pycman_dna-0.0.6/pycman_dna/maps/all_along_the_watchtowers.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:30:08.000000 pycman_dna-0.0.6/pycman_dna/maps/all_along_the_watchtowers_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:45:47.000000 pycman_dna-0.0.6/pycman_dna/maps/bimble.map
--rw-rw-rw-   0        0        0      453 2023-01-21 16:43:24.000000 pycman_dna-0.0.6/pycman_dna/maps/blank.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:46:41.000000 pycman_dna-0.0.6/pycman_dna/maps/broken_line_1.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:47:27.000000 pycman_dna-0.0.6/pycman_dna/maps/broken_line_2.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:47:47.000000 pycman_dna-0.0.6/pycman_dna/maps/broken_line_3.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:48:13.000000 pycman_dna-0.0.6/pycman_dna/maps/central_cavern.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:48:54.000000 pycman_dna-0.0.6/pycman_dna/maps/central_cavern_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:49:18.000000 pycman_dna-0.0.6/pycman_dna/maps/dizzy.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:49:36.000000 pycman_dna-0.0.6/pycman_dna/maps/easy_does_it.map
--rw-rw-rw-   0        0        0      451 2022-12-29 12:17:24.000000 pycman_dna-0.0.6/pycman_dna/maps/first_steps.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:50:27.000000 pycman_dna-0.0.6/pycman_dna/maps/follow_the_yellow_brick_road.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:50:45.000000 pycman_dna-0.0.6/pycman_dna/maps/ghost_train.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:51:06.000000 pycman_dna-0.0.6/pycman_dna/maps/i_smell_your_fear.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:51:46.000000 pycman_dna-0.0.6/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:52:13.000000 pycman_dna-0.0.6/pycman_dna/maps/killing_time.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:53:04.000000 pycman_dna-0.0.6/pycman_dna/maps/maze.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:53:33.000000 pycman_dna-0.0.6/pycman_dna/maps/number_one_the_larch.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:53:59.000000 pycman_dna-0.0.6/pycman_dna/maps/on_the_outside.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:54:27.000000 pycman_dna-0.0.6/pycman_dna/maps/on_the_outside_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:54:49.000000 pycman_dna-0.0.6/pycman_dna/maps/ping_pong.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:55:12.000000 pycman_dna-0.0.6/pycman_dna/maps/sense_your_way.map
--rw-rw-rw-   0        0        0      454 2022-12-28 15:24:10.000000 pycman_dna-0.0.6/pycman_dna/maps/teeth.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:55:33.000000 pycman_dna-0.0.6/pycman_dna/maps/unbroken_line_1.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:55:57.000000 pycman_dna-0.0.6/pycman_dna/maps/unbroken_line_2.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:56:19.000000 pycman_dna-0.0.6/pycman_dna/maps/unbroken_line_3.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:56:41.000000 pycman_dna-0.0.6/pycman_dna/maps/valid_symbols.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:58:05.000000 pycman_dna-0.0.6/pycman_dna/maps/you_make_me_feel_like_dancing.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:57:35.000000 pycman_dna-0.0.6/pycman_dna/maps/you_will_blink_first.map
-drwxrwxrwx   0        0        0        0 2023-06-06 13:12:48.597268 pycman_dna-0.0.6/pycman_dna.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1694 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 13:12:48.000000 pycman_dna-0.0.6/pycman_dna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 13:12:48.630302 pycman_dna-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1167 2023-06-06 13:12:42.000000 pycman_dna-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:26:03.614295 pycman_dna-0.1.0/
+-rw-rw-rw-   0        0        0      533 2023-06-06 15:26:03.613794 pycman_dna-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-06 12:04:16.000000 pycman_dna-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:26:03.569251 pycman_dna-0.1.0/pycman_dna/
+-rw-rw-rw-   0        0        0     9043 2023-06-06 15:25:31.000000 pycman_dna-0.1.0/pycman_dna/Map.py
+-rw-rw-rw-   0        0        0     8803 2023-06-06 13:20:34.000000 pycman_dna-0.1.0/pycman_dna/PacmanGame.py
+-rw-rw-rw-   0        0        0       78 2023-06-06 13:19:25.000000 pycman_dna-0.1.0/pycman_dna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:26:03.589268 pycman_dna-0.1.0/pycman_dna/images/
+-rw-rw-rw-   0        0        0     1017 2022-12-27 20:43:36.000000 pycman_dna-0.1.0/pycman_dna/images/PacmanDEAD.png
+-rw-rw-rw-   0        0        0     1113 2022-12-27 20:42:03.000000 pycman_dna-0.1.0/pycman_dna/images/PacmanDOWN.png
+-rw-rw-rw-   0        0        0     1075 2022-12-27 20:41:37.000000 pycman_dna-0.1.0/pycman_dna/images/PacmanLEFT.png
+-rw-rw-rw-   0        0        0     1046 2022-12-27 20:41:03.000000 pycman_dna-0.1.0/pycman_dna/images/PacmanRIGHT.png
+-rw-rw-rw-   0        0        0     1143 2022-12-27 20:42:21.000000 pycman_dna-0.1.0/pycman_dna/images/PacmanUP.png
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:43:53.000000 pycman_dna-0.1.0/pycman_dna/images/__init__.py
+-rw-rw-rw-   0        0        0     5042 2022-12-27 13:53:45.000000 pycman_dna-0.1.0/pycman_dna/images/dot.png
+-rw-rw-rw-   0        0        0     6849 2022-12-29 13:05:19.000000 pycman_dna-0.1.0/pycman_dna/images/eatable_ghost.png
+-rw-rw-rw-   0        0        0     7058 2022-12-29 13:05:23.000000 pycman_dna-0.1.0/pycman_dna/images/ghost.png
+-rw-rw-rw-   0        0        0     9959 2023-01-08 22:17:03.000000 pycman_dna-0.1.0/pycman_dna/images/icon.png
+-rw-rw-rw-   0        0        0     5684 2022-12-27 13:53:40.000000 pycman_dna-0.1.0/pycman_dna/images/pill.png
+-rw-rw-rw-   0        0        0      650 2022-12-27 20:33:08.000000 pycman_dna-0.1.0/pycman_dna/images/wall.png
+drwxrwxrwx   0        0        0        0 2023-06-06 15:26:03.612289 pycman_dna-0.1.0/pycman_dna/maps/
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:43:53.000000 pycman_dna-0.1.0/pycman_dna/maps/__init__.py
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:29:03.000000 pycman_dna-0.1.0/pycman_dna/maps/all_along_the_watchtowers.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:30:08.000000 pycman_dna-0.1.0/pycman_dna/maps/all_along_the_watchtowers_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:45:47.000000 pycman_dna-0.1.0/pycman_dna/maps/bimble.map
+-rw-rw-rw-   0        0        0      453 2023-01-21 16:43:24.000000 pycman_dna-0.1.0/pycman_dna/maps/blank.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:46:41.000000 pycman_dna-0.1.0/pycman_dna/maps/broken_line_1.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:47:27.000000 pycman_dna-0.1.0/pycman_dna/maps/broken_line_2.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:47:47.000000 pycman_dna-0.1.0/pycman_dna/maps/broken_line_3.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:48:13.000000 pycman_dna-0.1.0/pycman_dna/maps/central_cavern.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:48:54.000000 pycman_dna-0.1.0/pycman_dna/maps/central_cavern_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:49:18.000000 pycman_dna-0.1.0/pycman_dna/maps/dizzy.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:49:36.000000 pycman_dna-0.1.0/pycman_dna/maps/easy_does_it.map
+-rw-rw-rw-   0        0        0      451 2022-12-29 12:17:24.000000 pycman_dna-0.1.0/pycman_dna/maps/first_steps.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:50:27.000000 pycman_dna-0.1.0/pycman_dna/maps/follow_the_yellow_brick_road.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:50:45.000000 pycman_dna-0.1.0/pycman_dna/maps/ghost_train.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:51:06.000000 pycman_dna-0.1.0/pycman_dna/maps/i_smell_your_fear.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:51:46.000000 pycman_dna-0.1.0/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:52:13.000000 pycman_dna-0.1.0/pycman_dna/maps/killing_time.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:53:04.000000 pycman_dna-0.1.0/pycman_dna/maps/maze.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:53:33.000000 pycman_dna-0.1.0/pycman_dna/maps/number_one_the_larch.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:53:59.000000 pycman_dna-0.1.0/pycman_dna/maps/on_the_outside.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:54:27.000000 pycman_dna-0.1.0/pycman_dna/maps/on_the_outside_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:54:49.000000 pycman_dna-0.1.0/pycman_dna/maps/ping_pong.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:55:12.000000 pycman_dna-0.1.0/pycman_dna/maps/sense_your_way.map
+-rw-rw-rw-   0        0        0      454 2022-12-28 15:24:10.000000 pycman_dna-0.1.0/pycman_dna/maps/teeth.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:55:33.000000 pycman_dna-0.1.0/pycman_dna/maps/unbroken_line_1.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:55:57.000000 pycman_dna-0.1.0/pycman_dna/maps/unbroken_line_2.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:56:19.000000 pycman_dna-0.1.0/pycman_dna/maps/unbroken_line_3.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:56:41.000000 pycman_dna-0.1.0/pycman_dna/maps/valid_symbols.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:58:05.000000 pycman_dna-0.1.0/pycman_dna/maps/you_make_me_feel_like_dancing.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:57:35.000000 pycman_dna-0.1.0/pycman_dna/maps/you_will_blink_first.map
+drwxrwxrwx   0        0        0        0 2023-06-06 15:26:03.579760 pycman_dna-0.1.0/pycman_dna.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-06-06 15:26:03.000000 pycman_dna-0.1.0/pycman_dna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-06-06 15:26:03.000000 pycman_dna-0.1.0/pycman_dna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:26:03.000000 pycman_dna-0.1.0/pycman_dna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-06 15:26:03.000000 pycman_dna-0.1.0/pycman_dna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 15:26:03.000000 pycman_dna-0.1.0/pycman_dna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:26:03.614295 pycman_dna-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2023-06-06 15:25:51.000000 pycman_dna-0.1.0/setup.py
```

### Comparing `pycman_dna-0.0.6/PKG-INFO` & `pycman_dna-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman_dna
-Version: 0.0.6
+Version: 0.1.0
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.0.6/pycman_dna/Map.py` & `pycman_dna-0.1.0/pycman_dna/Map.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pygame;
+import importlib.resources as pkg_resources;
 from enum import Enum;
 from typing import List;
 
 class Obstacle(Enum):
     EMPTY = 1
     DOT = 2
     WALL = 3
@@ -50,31 +51,31 @@
                     case '.':
                         self.__dot_count += 1
                         self.__board_model[j][i] = Obstacle.DOT
                     case 'g':
                         self.__board_model[j][i] = Obstacle.GHOST
                         self.__ghost = Ghost()
                         self.__ghost.set_map_index(j, i)
-                        self.__ghost.sprite = pygame.image.load("images/ghost.png");
+                        self.__ghost.sprite = load_image("ghost.png");
                     case 'x':
                         self.__board_model[j][i] = Obstacle.PILL
                     case 'p':
                         self.__board_model[j][i] = Obstacle.PACMAN
                         self.__player.set_map_index(j, i)
-                        self.__player.sprite = pygame.image.load("images/PacmanUP.png");
+                        self.__player.sprite = load_image("PacmanUP.png");
                     case 'w':
                         self.__board_model[j][i]  = Obstacle.WALL
 
                 self.__build_map_view(i, j)  
     
 
     def __build_map_view(self, column : int, row : int) -> None:
         obstacleName = self.__board_model[row][column].name;
         if obstacleName.upper() != "PACMAN" and obstacleName.upper() != "GHOST" and obstacleName.upper() != "EMPTY":
-            self.__board_view[row][column] = pygame.image.load("images/" + obstacleName.lower() + ".png")
+            self.__board_view[row][column] = load_image(obstacleName.lower() + ".png")
         
 
     def draw_map(self, screen : pygame.Surface) -> None:
         pygame.draw.rect(screen, (255,255,255), rect=pygame.Rect(0, 0, 784, 50))
         screen.blit(self.__font.render(self.__game._PacmanGame__message, True, (0,0,0)), (8, 8))
 
         for i in range(0, self.__MAP_WIDTH):
@@ -145,25 +146,31 @@
         if row < 0 or column < 0 or row >= self.__MAP_HEIGHT or column >= self.__MAP_WIDTH:
             return Obstacle.VOID
         else:
             return self.__board_model[column][row]
 
     def __read_map(self, map_name : str) -> List[str]:
         lines = []
-        with open('maps/' + map_name + '.map') as f:
+        with open(get_map_path(map_name + '.map')) as f:
             lines = f.read().splitlines()
         return lines;
     
     def get_pacman(self) -> 'Pacman':
         return self.__player;
 
     def get_pacman_direction(self) -> Direction:
         return self.__player.direction;
 
 
+def load_image(package_path: str) -> pygame.Surface:
+        return pygame.image.load(pkg_resources.path('pycman_dna.images', package_path))
+
+def get_map_path(package_path: str) -> List[str]:
+    return pkg_resources.path('pycman_dna.maps', package_path)
+
 class Pacman:
     def __init__(self) -> None:
         self.map_index = [0, 0]
         self.position = []
         self.sprite_list = []
         self.create_sprite_list()
         self.set_direction(Direction.UP)
@@ -171,15 +178,16 @@
 
     def set_map_index(self, row : int, column : int) -> None:
         self.map_index = [row, column]
         self.position = [54 + (row * 32), 54 + (column * 32)]
 
     def create_sprite_list(self):
         for i in range(5):
-            self.sprite_list.append(pygame.image.load("images/Pacman" + Direction(i + 1).name + ".png"))
+            self.sprite_list.append(load_image("Pacman" + Direction(i + 1).name + ".png"))
+            #self.sprite_list.append(pygame.image.load("images/Pacman" + Direction(i + 1).name + ".png"))
         self.sprite = self.sprite_list[0]
 
     def set_direction(self, new_direction : Direction):
         self.direction = new_direction
         self.sprite = self.sprite_list[new_direction.value - 1]
 
 class Ghost:
@@ -193,12 +201,12 @@
         self.map_index = [row, column]
         self.position = [54 + (row * 32), 54 + (column * 32)]
 
     def toggle_edible_state(self) -> None:
         self.is_edible = not self.is_edible
 
         if self.is_edible:
-            self.sprite = pygame.image.load("images/eatable_ghost.png")
+            self.sprite = load_image("eatable_ghost.png")
         else:
-            self.sprite = pygame.image.load("images/ghost.png")
+            self.sprite = load_image("ghost.png")
```

### Comparing `pycman_dna-0.0.6/pycman_dna/PacmanGame.py` & `pycman_dna-0.1.0/pycman_dna/PacmanGame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from tkinter import simpledialog;
 import time;
 import threading, sys, os;
 
-from .Map import Map;
-from .Map import Direction;
+from pycman_dna.Map import Map
+from pycman_dna.Map import Direction;
 
 class PacmanGame:
     """
     PacmanGame's base constructor method. Performs initial setup.
     """
     __update_rate = 0.25;
     __moves_taken = 0;
```

### Comparing `pycman_dna-0.0.6/pycman_dna/images/PacmanDEAD.png` & `pycman_dna-0.1.0/pycman_dna/images/PacmanDEAD.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/PacmanDOWN.png` & `pycman_dna-0.1.0/pycman_dna/images/PacmanDOWN.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/PacmanLEFT.png` & `pycman_dna-0.1.0/pycman_dna/images/PacmanLEFT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/PacmanRIGHT.png` & `pycman_dna-0.1.0/pycman_dna/images/PacmanRIGHT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/PacmanUP.png` & `pycman_dna-0.1.0/pycman_dna/images/PacmanUP.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/dot.png` & `pycman_dna-0.1.0/pycman_dna/images/dot.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/eatable_ghost.png` & `pycman_dna-0.1.0/pycman_dna/images/eatable_ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/ghost.png` & `pycman_dna-0.1.0/pycman_dna/images/ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/icon.png` & `pycman_dna-0.1.0/pycman_dna/images/icon.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/pill.png` & `pycman_dna-0.1.0/pycman_dna/images/pill.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna/images/wall.png` & `pycman_dna-0.1.0/pycman_dna/images/wall.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.0.6/pycman_dna.egg-info/PKG-INFO` & `pycman_dna-0.1.0/pycman_dna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman-dna
-Version: 0.0.6
+Version: 0.1.0
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.0.6/pycman_dna.egg-info/SOURCES.txt` & `pycman_dna-0.1.0/pycman_dna.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 pycman_dna.egg-info/requires.txt
 pycman_dna.egg-info/top_level.txt
 pycman_dna/images/PacmanDEAD.png
 pycman_dna/images/PacmanDOWN.png
 pycman_dna/images/PacmanLEFT.png
 pycman_dna/images/PacmanRIGHT.png
 pycman_dna/images/PacmanUP.png
+pycman_dna/images/__init__.py
 pycman_dna/images/dot.png
 pycman_dna/images/eatable_ghost.png
 pycman_dna/images/ghost.png
 pycman_dna/images/icon.png
 pycman_dna/images/pill.png
 pycman_dna/images/wall.png
+pycman_dna/maps/__init__.py
 pycman_dna/maps/all_along_the_watchtowers.map
 pycman_dna/maps/all_along_the_watchtowers_revisited.map
 pycman_dna/maps/bimble.map
 pycman_dna/maps/blank.map
 pycman_dna/maps/broken_line_1.map
 pycman_dna/maps/broken_line_2.map
 pycman_dna/maps/broken_line_3.map
```

### Comparing `pycman_dna-0.0.6/setup.py` & `pycman_dna-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.1.0' 
 DESCRIPTION = 'Python Pacman Tool'
 LONG_DESCRIPTION = 'A teaching tool based on arcade icon Pacman, written in Python.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="pycman_dna",
```

