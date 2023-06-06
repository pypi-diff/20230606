# Comparing `tmp/pycman_dna-0.3.5.tar.gz` & `tmp/pycman_dna-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycman_dna-0.3.5.tar", last modified: Tue Jun  6 17:00:17 2023, max compression
+gzip compressed data, was "pycman_dna-0.4.0.tar", last modified: Tue Jun  6 17:50:32 2023, max compression
```

## Comparing `pycman_dna-0.3.5.tar` & `pycman_dna-0.4.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:00:17.776934 pycman_dna-0.3.5/
--rw-rw-rw-   0        0        0      564 2023-06-06 17:00:17.776433 pycman_dna-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-06 12:04:16.000000 pycman_dna-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 17:00:17.736854 pycman_dna-0.3.5/pycman_dna/
--rw-rw-rw-   0        0        0       81 2023-06-06 15:54:08.000000 pycman_dna-0.3.5/pycman_dna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:00:17.752889 pycman_dna-0.3.5/pycman_dna/images/
--rw-rw-rw-   0        0        0     1017 2022-12-27 20:43:36.000000 pycman_dna-0.3.5/pycman_dna/images/PacmanDEAD.png
--rw-rw-rw-   0        0        0     1113 2022-12-27 20:42:03.000000 pycman_dna-0.3.5/pycman_dna/images/PacmanDOWN.png
--rw-rw-rw-   0        0        0     1075 2022-12-27 20:41:37.000000 pycman_dna-0.3.5/pycman_dna/images/PacmanLEFT.png
--rw-rw-rw-   0        0        0     1046 2022-12-27 20:41:03.000000 pycman_dna-0.3.5/pycman_dna/images/PacmanRIGHT.png
--rw-rw-rw-   0        0        0     1143 2022-12-27 20:42:21.000000 pycman_dna-0.3.5/pycman_dna/images/PacmanUP.png
--rw-rw-rw-   0        0        0        0 2023-06-06 13:43:53.000000 pycman_dna-0.3.5/pycman_dna/images/__init__.py
--rw-rw-rw-   0        0        0     5042 2022-12-27 13:53:45.000000 pycman_dna-0.3.5/pycman_dna/images/dot.png
--rw-rw-rw-   0        0        0     6849 2022-12-29 13:05:19.000000 pycman_dna-0.3.5/pycman_dna/images/eatable_ghost.png
--rw-rw-rw-   0        0        0     7058 2022-12-29 13:05:23.000000 pycman_dna-0.3.5/pycman_dna/images/ghost.png
--rw-rw-rw-   0        0        0     9959 2023-01-08 22:17:03.000000 pycman_dna-0.3.5/pycman_dna/images/icon.png
--rw-rw-rw-   0        0        0     5684 2022-12-27 13:53:40.000000 pycman_dna-0.3.5/pycman_dna/images/pill.png
--rw-rw-rw-   0        0        0      650 2022-12-27 20:33:08.000000 pycman_dna-0.3.5/pycman_dna/images/wall.png
--rw-rw-rw-   0        0        0     9038 2023-06-06 16:59:45.000000 pycman_dna-0.3.5/pycman_dna/map.py
--rw-rw-rw-   0        0        0      537 2022-12-28 16:08:28.000000 pycman_dna-0.3.5/pycman_dna/map_names.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 17:00:17.775433 pycman_dna-0.3.5/pycman_dna/maps/
--rw-rw-rw-   0        0        0        0 2023-06-06 13:43:53.000000 pycman_dna-0.3.5/pycman_dna/maps/__init__.py
--rw-rw-rw-   0        0        0      452 2022-12-28 15:29:03.000000 pycman_dna-0.3.5/pycman_dna/maps/all_along_the_watchtowers.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:30:08.000000 pycman_dna-0.3.5/pycman_dna/maps/all_along_the_watchtowers_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:45:47.000000 pycman_dna-0.3.5/pycman_dna/maps/bimble.map
--rw-rw-rw-   0        0        0      453 2023-01-21 16:43:24.000000 pycman_dna-0.3.5/pycman_dna/maps/blank.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:46:41.000000 pycman_dna-0.3.5/pycman_dna/maps/broken_line_1.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:47:27.000000 pycman_dna-0.3.5/pycman_dna/maps/broken_line_2.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:47:47.000000 pycman_dna-0.3.5/pycman_dna/maps/broken_line_3.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:48:13.000000 pycman_dna-0.3.5/pycman_dna/maps/central_cavern.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:48:54.000000 pycman_dna-0.3.5/pycman_dna/maps/central_cavern_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:49:18.000000 pycman_dna-0.3.5/pycman_dna/maps/dizzy.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:49:36.000000 pycman_dna-0.3.5/pycman_dna/maps/easy_does_it.map
--rw-rw-rw-   0        0        0      451 2022-12-29 12:17:24.000000 pycman_dna-0.3.5/pycman_dna/maps/first_steps.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:50:27.000000 pycman_dna-0.3.5/pycman_dna/maps/follow_the_yellow_brick_road.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:50:45.000000 pycman_dna-0.3.5/pycman_dna/maps/ghost_train.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:51:06.000000 pycman_dna-0.3.5/pycman_dna/maps/i_smell_your_fear.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:51:46.000000 pycman_dna-0.3.5/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:52:13.000000 pycman_dna-0.3.5/pycman_dna/maps/killing_time.map
--rw-rw-rw-   0        0        0      451 2022-12-28 15:53:04.000000 pycman_dna-0.3.5/pycman_dna/maps/maze.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:53:33.000000 pycman_dna-0.3.5/pycman_dna/maps/number_one_the_larch.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:53:59.000000 pycman_dna-0.3.5/pycman_dna/maps/on_the_outside.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:54:27.000000 pycman_dna-0.3.5/pycman_dna/maps/on_the_outside_revisited.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:54:49.000000 pycman_dna-0.3.5/pycman_dna/maps/ping_pong.map
--rw-rw-rw-   0        0        0      452 2022-12-28 15:55:12.000000 pycman_dna-0.3.5/pycman_dna/maps/sense_your_way.map
--rw-rw-rw-   0        0        0      454 2022-12-28 15:24:10.000000 pycman_dna-0.3.5/pycman_dna/maps/teeth.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:55:33.000000 pycman_dna-0.3.5/pycman_dna/maps/unbroken_line_1.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:55:57.000000 pycman_dna-0.3.5/pycman_dna/maps/unbroken_line_2.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:56:19.000000 pycman_dna-0.3.5/pycman_dna/maps/unbroken_line_3.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:56:41.000000 pycman_dna-0.3.5/pycman_dna/maps/valid_symbols.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:58:05.000000 pycman_dna-0.3.5/pycman_dna/maps/you_make_me_feel_like_dancing.map
--rw-rw-rw-   0        0        0      453 2022-12-28 15:57:35.000000 pycman_dna-0.3.5/pycman_dna/maps/you_will_blink_first.map
--rw-rw-rw-   0        0        0     9359 2023-06-06 16:46:57.000000 pycman_dna-0.3.5/pycman_dna/pacman_game.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:00:17.743871 pycman_dna-0.3.5/pycman_dna.egg-info/
--rw-rw-rw-   0        0        0      564 2023-06-06 17:00:17.000000 pycman_dna-0.3.5/pycman_dna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1778 2023-06-06 17:00:17.000000 pycman_dna-0.3.5/pycman_dna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:00:17.000000 pycman_dna-0.3.5/pycman_dna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 17:00:17.000000 pycman_dna-0.3.5/pycman_dna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 17:00:17.000000 pycman_dna-0.3.5/pycman_dna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 17:00:17.776934 pycman_dna-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-06 17:00:00.000000 pycman_dna-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:50:32.138057 pycman_dna-0.4.0/
+-rw-rw-rw-   0        0        0      564 2023-06-06 17:50:32.137556 pycman_dna-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-06 12:04:16.000000 pycman_dna-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:50:32.019951 pycman_dna-0.4.0/pycman_dna/
+-rw-rw-rw-   0        0        0       81 2023-06-06 15:54:08.000000 pycman_dna-0.4.0/pycman_dna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:50:32.038968 pycman_dna-0.4.0/pycman_dna/images/
+-rw-rw-rw-   0        0        0     1017 2022-12-27 20:43:36.000000 pycman_dna-0.4.0/pycman_dna/images/PacmanDEAD.png
+-rw-rw-rw-   0        0        0     1113 2022-12-27 20:42:03.000000 pycman_dna-0.4.0/pycman_dna/images/PacmanDOWN.png
+-rw-rw-rw-   0        0        0     1075 2022-12-27 20:41:37.000000 pycman_dna-0.4.0/pycman_dna/images/PacmanLEFT.png
+-rw-rw-rw-   0        0        0     1046 2022-12-27 20:41:03.000000 pycman_dna-0.4.0/pycman_dna/images/PacmanRIGHT.png
+-rw-rw-rw-   0        0        0     1143 2022-12-27 20:42:21.000000 pycman_dna-0.4.0/pycman_dna/images/PacmanUP.png
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:43:53.000000 pycman_dna-0.4.0/pycman_dna/images/__init__.py
+-rw-rw-rw-   0        0        0     5042 2022-12-27 13:53:45.000000 pycman_dna-0.4.0/pycman_dna/images/dot.png
+-rw-rw-rw-   0        0        0     6849 2022-12-29 13:05:19.000000 pycman_dna-0.4.0/pycman_dna/images/eatable_ghost.png
+-rw-rw-rw-   0        0        0     7058 2022-12-29 13:05:23.000000 pycman_dna-0.4.0/pycman_dna/images/ghost.png
+-rw-rw-rw-   0        0        0     9959 2023-01-08 22:17:03.000000 pycman_dna-0.4.0/pycman_dna/images/icon.png
+-rw-rw-rw-   0        0        0     5684 2022-12-27 13:53:40.000000 pycman_dna-0.4.0/pycman_dna/images/pill.png
+-rw-rw-rw-   0        0        0      650 2022-12-27 20:33:08.000000 pycman_dna-0.4.0/pycman_dna/images/wall.png
+-rw-rw-rw-   0        0        0     8997 2023-06-06 17:49:45.000000 pycman_dna-0.4.0/pycman_dna/map.py
+-rw-rw-rw-   0        0        0      537 2022-12-28 16:08:28.000000 pycman_dna-0.4.0/pycman_dna/map_names.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 17:50:32.136555 pycman_dna-0.4.0/pycman_dna/maps/
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:43:53.000000 pycman_dna-0.4.0/pycman_dna/maps/__init__.py
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:29:03.000000 pycman_dna-0.4.0/pycman_dna/maps/all_along_the_watchtowers.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:30:08.000000 pycman_dna-0.4.0/pycman_dna/maps/all_along_the_watchtowers_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:45:47.000000 pycman_dna-0.4.0/pycman_dna/maps/bimble.map
+-rw-rw-rw-   0        0        0      453 2023-01-21 16:43:24.000000 pycman_dna-0.4.0/pycman_dna/maps/blank.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:46:41.000000 pycman_dna-0.4.0/pycman_dna/maps/broken_line_1.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:47:27.000000 pycman_dna-0.4.0/pycman_dna/maps/broken_line_2.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:47:47.000000 pycman_dna-0.4.0/pycman_dna/maps/broken_line_3.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:48:13.000000 pycman_dna-0.4.0/pycman_dna/maps/central_cavern.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:48:54.000000 pycman_dna-0.4.0/pycman_dna/maps/central_cavern_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:49:18.000000 pycman_dna-0.4.0/pycman_dna/maps/dizzy.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:49:36.000000 pycman_dna-0.4.0/pycman_dna/maps/easy_does_it.map
+-rw-rw-rw-   0        0        0      451 2022-12-29 12:17:24.000000 pycman_dna-0.4.0/pycman_dna/maps/first_steps.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:50:27.000000 pycman_dna-0.4.0/pycman_dna/maps/follow_the_yellow_brick_road.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:50:45.000000 pycman_dna-0.4.0/pycman_dna/maps/ghost_train.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:51:06.000000 pycman_dna-0.4.0/pycman_dna/maps/i_smell_your_fear.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:51:46.000000 pycman_dna-0.4.0/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:52:13.000000 pycman_dna-0.4.0/pycman_dna/maps/killing_time.map
+-rw-rw-rw-   0        0        0      451 2022-12-28 15:53:04.000000 pycman_dna-0.4.0/pycman_dna/maps/maze.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:53:33.000000 pycman_dna-0.4.0/pycman_dna/maps/number_one_the_larch.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:53:59.000000 pycman_dna-0.4.0/pycman_dna/maps/on_the_outside.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:54:27.000000 pycman_dna-0.4.0/pycman_dna/maps/on_the_outside_revisited.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:54:49.000000 pycman_dna-0.4.0/pycman_dna/maps/ping_pong.map
+-rw-rw-rw-   0        0        0      452 2022-12-28 15:55:12.000000 pycman_dna-0.4.0/pycman_dna/maps/sense_your_way.map
+-rw-rw-rw-   0        0        0      454 2022-12-28 15:24:10.000000 pycman_dna-0.4.0/pycman_dna/maps/teeth.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:55:33.000000 pycman_dna-0.4.0/pycman_dna/maps/unbroken_line_1.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:55:57.000000 pycman_dna-0.4.0/pycman_dna/maps/unbroken_line_2.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:56:19.000000 pycman_dna-0.4.0/pycman_dna/maps/unbroken_line_3.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:56:41.000000 pycman_dna-0.4.0/pycman_dna/maps/valid_symbols.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:58:05.000000 pycman_dna-0.4.0/pycman_dna/maps/you_make_me_feel_like_dancing.map
+-rw-rw-rw-   0        0        0      453 2022-12-28 15:57:35.000000 pycman_dna-0.4.0/pycman_dna/maps/you_will_blink_first.map
+-rw-rw-rw-   0        0        0     9359 2023-06-06 16:46:57.000000 pycman_dna-0.4.0/pycman_dna/pacman_game.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:50:32.030461 pycman_dna-0.4.0/pycman_dna.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-06-06 17:50:31.000000 pycman_dna-0.4.0/pycman_dna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1778 2023-06-06 17:50:31.000000 pycman_dna-0.4.0/pycman_dna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:50:31.000000 pycman_dna-0.4.0/pycman_dna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 17:50:31.000000 pycman_dna-0.4.0/pycman_dna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 17:50:31.000000 pycman_dna-0.4.0/pycman_dna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:50:32.138057 pycman_dna-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-06 17:50:20.000000 pycman_dna-0.4.0/setup.py
```

### Comparing `pycman_dna-0.3.5/PKG-INFO` & `pycman_dna-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman_dna
-Version: 0.3.5
+Version: 0.4.0
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.3.5/pycman_dna/images/PacmanDEAD.png` & `pycman_dna-0.4.0/pycman_dna/images/PacmanDEAD.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/PacmanDOWN.png` & `pycman_dna-0.4.0/pycman_dna/images/PacmanDOWN.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/PacmanLEFT.png` & `pycman_dna-0.4.0/pycman_dna/images/PacmanLEFT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/PacmanRIGHT.png` & `pycman_dna-0.4.0/pycman_dna/images/PacmanRIGHT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/PacmanUP.png` & `pycman_dna-0.4.0/pycman_dna/images/PacmanUP.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/dot.png` & `pycman_dna-0.4.0/pycman_dna/images/dot.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/eatable_ghost.png` & `pycman_dna-0.4.0/pycman_dna/images/eatable_ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/ghost.png` & `pycman_dna-0.4.0/pycman_dna/images/ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/icon.png` & `pycman_dna-0.4.0/pycman_dna/images/icon.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/pill.png` & `pycman_dna-0.4.0/pycman_dna/images/pill.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/images/wall.png` & `pycman_dna-0.4.0/pycman_dna/images/wall.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/map.py` & `pycman_dna-0.4.0/pycman_dna/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pygame;
-import importlib.resources as pkg_resources;
+import os
 from enum import Enum;
 from typing import List;
 
 class Obstacle(Enum):
     EMPTY = 1
     DOT = 2
     WALL = 3
@@ -158,18 +158,18 @@
         return self.__player;
 
     def get_pacman_direction(self) -> Direction:
         return self.__player.direction;
 
 
 def load_image(package_path: str) -> pygame.Surface:
-        return pygame.image.load(str(pkg_resources.path('pycman_dna.images', package_path)))
+        return pygame.image.load(os.path.dirname(__file__) + "\\images\\" + package_path)
 
 def get_map_path(package_path: str) -> List[str]:
-    return str(pkg_resources.path('pycman_dna.maps', package_path))
+    return os.path.dirname(__file__) + "\\maps\\" + package_path
 
 class Pacman:
     def __init__(self) -> None:
         self.map_index = [0, 0]
         self.position = []
         self.sprite_list = []
         self.create_sprite_list()
```

### Comparing `pycman_dna-0.3.5/pycman_dna/map_names.txt` & `pycman_dna-0.4.0/pycman_dna/map_names.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna/pacman_game.py` & `pycman_dna-0.4.0/pycman_dna/pacman_game.py`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/pycman_dna.egg-info/PKG-INFO` & `pycman_dna-0.4.0/pycman_dna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman-dna
-Version: 0.3.5
+Version: 0.4.0
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.3.5/pycman_dna.egg-info/SOURCES.txt` & `pycman_dna-0.4.0/pycman_dna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.3.5/setup.py` & `pycman_dna-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.5' 
+VERSION = '0.4.0' 
 DESCRIPTION = 'Python Pacman Tool'
 LONG_DESCRIPTION = 'A teaching tool based on arcade icon Pacman, written in Python. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="pycman_dna",
```

