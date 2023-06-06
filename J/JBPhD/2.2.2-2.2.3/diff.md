# Comparing `tmp/JBPhD-2.2.2.tar.gz` & `tmp/JBPhD-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.2.2.tar", last modified: Wed May 24 16:15:55 2023, max compression
+gzip compressed data, was "JBPhD-2.2.3.tar", last modified: Tue Jun  6 14:57:56 2023, max compression
```

## Comparing `JBPhD-2.2.2.tar` & `JBPhD-2.2.3.tar`

### file list

```diff
@@ -1,86 +1,111 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      257 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1931 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-24 16:15:54.000000 JBPhD-2.2.2/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      257 2023-05-24 16:15:56.000000 JBPhD-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/Task/
--rw-rw-rw-   0        0        0     2489 2023-05-18 22:38:28.000000 JBPhD-2.2.2/Task/Analysis.py
--rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.2/Task/Api.json
--rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.2/Task/Api2.json
--rw-rw-rw-   0        0        0   256511 2023-05-07 17:28:42.000000 JBPhD-2.2.2/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.2/Task/Consent Form.docx
--rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.2/Task/Dependencies.py
--rw-rw-rw-   0        0        0    12380 2023-05-24 14:20:54.000000 JBPhD-2.2.2/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.2/Task/Email Output.py
--rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.2.2/Task/Experimental Run Trial.py
--rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.2/Task/Export.py
--rw-rw-rw-   0        0        0   249107 2023-05-07 17:28:42.000000 JBPhD-2.2.2/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-05-07 17:28:42.000000 JBPhD-2.2.2/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0     1184 2023-05-15 13:38:26.000000 JBPhD-2.2.2/Task/Gradient Background.py
--rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.2/Task/Graph.py
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256274 2023-05-07 17:28:42.000000 JBPhD-2.2.2/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0      384 2023-04-24 19:08:56.000000 JBPhD-2.2.2/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.2/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.2.2/Task/N-Back Revision.py
--rw-rw-rw-   0        0        0        1 2023-05-24 13:46:22.000000 JBPhD-2.2.2/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    19276 2023-05-18 19:25:40.000000 JBPhD-2.2.2/Task/N-Back.py
--rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.2.2/Task/PIS.docx
--rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.2.2/Task/PIS.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/Task/Participant 1/
--rw-rw-rw-   0        0        0    21860 2023-05-24 16:11:00.000000 JBPhD-2.2.2/Task/Participant 1/1 - Combined Reaction Times.csv
--rw-rw-rw-   0        0        0    14483 2023-05-24 16:11:00.000000 JBPhD-2.2.2/Task/Participant 1/1 - Combined Scores.csv
--rw-rw-rw-   0        0        0    21894 2023-05-24 16:11:00.000000 JBPhD-2.2.2/Task/Participant 1/1 - RT Reaction Times.csv
--rw-rw-rw-   0        0        0    14515 2023-05-24 16:11:00.000000 JBPhD-2.2.2/Task/Participant 1/1 - RT Score.csv
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/Task/Participant 2/
--rw-rw-rw-   0        0        0     1231 2023-05-24 13:46:00.000000 JBPhD-2.2.2/Task/Participant 2/2 - Consent.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/Task/Participant 90210/
--rw-rw-rw-   0        0        0     3063 2023-05-18 22:28:16.000000 JBPhD-2.2.2/Task/Participant 90210/90210 - Combined Reaction Times.csv
--rw-rw-rw-   0        0        0     2640 2023-05-18 22:09:26.000000 JBPhD-2.2.2/Task/Participant 90210/90210 - Combined Scores.csv
--rw-rw-rw-   0        0        0     4421 2023-05-18 19:19:36.000000 JBPhD-2.2.2/Task/Participant 90210/90210 - N-Back Reaction Times.csv
--rw-rw-rw-   0        0        0     2650 2023-05-18 19:19:36.000000 JBPhD-2.2.2/Task/Participant 90210/90210 - N-Back Score.csv
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.2/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.2/Task/README.txt.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 16:10:30.000000 JBPhD-2.2.2/Task/RT count.txt
--rw-rw-rw-   0        0        0    20186 2023-05-24 16:13:32.000000 JBPhD-2.2.2/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.2/Task/Suffix.bat
--rw-rw-rw-   0        0        0        1 2023-05-24 13:46:26.000000 JBPhD-2.2.2/Task/Switch Count.txt
--rw-rw-rw-   0        0        0    24157 2023-05-15 10:24:58.000000 JBPhD-2.2.2/Task/Switching.py
--rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.2.2/Task/Task.py
--rw-rw-rw-   0        0        0     6625 2023-05-18 22:04:18.000000 JBPhD-2.2.2/Task/Trial.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:15:54.000000 JBPhD-2.2.2/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.2/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.2.2/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      696 2023-05-04 10:46:06.000000 JBPhD-2.2.2/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    18767 2023-05-07 22:15:14.000000 JBPhD-2.2.2/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.2/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/circle.jpg
--rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/greendot.png
--rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/greentick.png
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.2/Task/help.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:13:26.000000 JBPhD-2.2.2/Task/participant number.txt
--rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.2/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.2/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.2/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.2/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.2/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       19 2023-05-24 14:13:56.000000 JBPhD-2.2.2/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.2/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.2/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.2/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.2/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-05-24 16:15:56.000000 JBPhD-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-05-24 16:14:26.000000 JBPhD-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-06 14:57:56.000000 JBPhD-2.2.3/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      269 2023-06-06 14:57:58.000000 JBPhD-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/Task/
+-rw-rw-rw-   0        0        0     3897 2023-06-06 11:15:00.000000 JBPhD-2.2.3/Task/1 - Combined RT Output.csv
+-rw-rw-rw-   0        0        0     2366 2023-06-06 11:15:00.000000 JBPhD-2.2.3/Task/1 - Combined Score Output.csv
+-rw-rw-rw-   0        0        0     2623 2023-06-06 11:15:00.000000 JBPhD-2.2.3/Task/1 - N-Back RT Output.csv
+-rw-rw-rw-   0        0        0     1092 2023-06-06 11:15:00.000000 JBPhD-2.2.3/Task/1 - N-Back Score Output.csv
+-rw-rw-rw-   0        0        0     2489 2023-05-18 22:38:28.000000 JBPhD-2.2.3/Task/Analysis.py
+-rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.3/Task/Api.json
+-rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.3/Task/Api2.json
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.2.3/Task/BL.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.2.3/Task/BR.PNG
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.2.3/Task/Back_Left.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.2.3/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.3/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.2.3/Task/Consent.py
+-rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.3/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    12380 2023-05-24 14:20:54.000000 JBPhD-2.2.3/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0      156 2023-05-25 21:19:50.000000 JBPhD-2.2.3/Task/Email Errors.txt
+-rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.3/Task/Email Output.py
+-rw-rw-rw-   0        0        0      202 2023-05-07 16:32:10.000000 JBPhD-2.2.3/Task/Experimental Run Trial.py
+-rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.3/Task/Export.py
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.2.3/Task/FL.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.2.3/Task/FR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.2.3/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.2.3/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0     1184 2023-05-15 13:38:26.000000 JBPhD-2.2.3/Task/Gradient Background.py
+-rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.3/Task/Graph.py
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.2.3/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.2.3/Task/Inverse_Back_Right.PNG
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.2.3/Task/Inverse_Front_Left.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.2.3/Task/Inverse_Front_Right.PNG
+-rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.2.3/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.3/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.2.3/Task/N-Back Revision.py
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:32:10.000000 JBPhD-2.2.3/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    20165 2023-06-06 14:33:40.000000 JBPhD-2.2.3/Task/N-Back.py
+-rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.2.3/Task/PIS.docx
+-rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.2.3/Task/PIS.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/Task/Participant 1/
+-rw-rw-rw-   0        0        0    43356 2023-06-06 14:14:26.000000 JBPhD-2.2.3/Task/Participant 1/1 - Combined Reaction Times.csv
+-rw-rw-rw-   0        0        0    27987 2023-06-06 14:14:26.000000 JBPhD-2.2.3/Task/Participant 1/1 - Combined Scores.csv
+-rw-rw-rw-   0        0        0       40 2023-06-06 14:14:26.000000 JBPhD-2.2.3/Task/Participant 1/1 - N-Back Reaction Times.csv
+-rw-rw-rw-   0        0        0       24 2023-06-06 14:14:26.000000 JBPhD-2.2.3/Task/Participant 1/1 - N-Back Score.csv
+-rw-rw-rw-   0        0        0    21894 2023-05-24 16:11:00.000000 JBPhD-2.2.3/Task/Participant 1/1 - RT Reaction Times.csv
+-rw-rw-rw-   0        0        0    14515 2023-05-24 16:11:00.000000 JBPhD-2.2.3/Task/Participant 1/1 - RT Score.csv
+-rw-rw-rw-   0        0        0       89 2023-06-06 13:44:36.000000 JBPhD-2.2.3/Task/Participant 1/1 - Switching Reaction Times.csv
+-rw-rw-rw-   0        0        0       56 2023-06-06 13:44:36.000000 JBPhD-2.2.3/Task/Participant 1/1 - Switching Score.csv
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/Task/Participant 2/
+-rw-rw-rw-   0        0        0     1231 2023-05-24 13:46:00.000000 JBPhD-2.2.3/Task/Participant 2/2 - Consent.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/Task/Participant 90210/
+-rw-rw-rw-   0        0        0     3063 2023-05-18 22:28:16.000000 JBPhD-2.2.3/Task/Participant 90210/90210 - Combined Reaction Times.csv
+-rw-rw-rw-   0        0        0     2640 2023-05-18 22:09:26.000000 JBPhD-2.2.3/Task/Participant 90210/90210 - Combined Scores.csv
+-rw-rw-rw-   0        0        0     4421 2023-05-18 19:19:36.000000 JBPhD-2.2.3/Task/Participant 90210/90210 - N-Back Reaction Times.csv
+-rw-rw-rw-   0        0        0     2650 2023-05-18 19:19:36.000000 JBPhD-2.2.3/Task/Participant 90210/90210 - N-Back Score.csv
+-rw-rw-rw-   0        0        0    13007 2023-06-02 21:35:24.000000 JBPhD-2.2.3/Task/Posh App - my version.py
+-rw-rw-rw-   0        0        0    10462 2023-05-24 22:04:12.000000 JBPhD-2.2.3/Task/Posh App.py
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.3/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.3/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 16:10:30.000000 JBPhD-2.2.3/Task/RT count.txt
+-rw-rw-rw-   0        0        0    20169 2023-06-06 13:44:44.000000 JBPhD-2.2.3/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.3/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        2 2023-06-06 13:44:06.000000 JBPhD-2.2.3/Task/Switch Count.txt
+-rw-rw-rw-   0        0        0    29945 2023-06-06 13:44:38.000000 JBPhD-2.2.3/Task/Switching.py
+-rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.2.3/Task/Task.py
+-rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.2.3/Task/Trial.py
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.2.3/Task/UBL.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.2.3/Task/UBR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.2.3/Task/UFL.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.2.3/Task/UFR.PNG
+drwxrwxrwx   0        0        0        0 2023-06-06 14:57:56.000000 JBPhD-2.2.3/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.3/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.2.3/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.2.3/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.2.3/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.3/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/circle.jpg
+-rw-rw-rw-   0        0        0    12363 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/greendot.png
+-rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/greentick.png
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.3/Task/help.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 21:33:54.000000 JBPhD-2.2.3/Task/participant number.txt
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.3/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.3/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.3/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.3/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.3/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 21:26:30.000000 JBPhD-2.2.3/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.3/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.3/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.3/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.3/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-06-06 14:57:58.000000 JBPhD-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-06-06 14:57:10.000000 JBPhD-2.2.3/setup.py
```

### Comparing `JBPhD-2.2.2/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.2.3/JBPhD.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,74 @@
+LICENSE.txt
 MANIFEST.in
 README.txt
 setup.py
 JBPhD.egg-info/PKG-INFO
 JBPhD.egg-info/SOURCES.txt
 JBPhD.egg-info/dependency_links.txt
 JBPhD.egg-info/entry_points.txt
 JBPhD.egg-info/requires.txt
 JBPhD.egg-info/top_level.txt
+Task/1 - Combined RT Output.csv
+Task/1 - Combined Score Output.csv
+Task/1 - N-Back RT Output.csv
+Task/1 - N-Back Score Output.csv
 Task/Analysis.py
 Task/Api.json
 Task/Api2.json
+Task/BL.PNG
+Task/BR.PNG
+Task/Back_Left.PNG
 Task/Back_Right.PNG
 Task/Consent Form.docx
+Task/Consent.py
 Task/Dependencies.py
 Task/Dependency Installation.py
+Task/Email Errors.txt
 Task/Email Output.py
 Task/Experimental Run Trial.py
 Task/Export.py
+Task/FL.PNG
+Task/FR.PNG
 Task/Front_Left.PNG
 Task/Front_Right.PNG
 Task/Gradient Background.py
 Task/Graph.py
 Task/ImageSample.PNG
 Task/Inverse_Back_Left.PNG
+Task/Inverse_Back_Right.PNG
+Task/Inverse_Front_Left.PNG
+Task/Inverse_Front_Right.PNG
 Task/Location.py
 Task/MANIFEST.in.txt
 Task/Manikin Back Down Left.png
 Task/Manikin Back Up Right.png
 Task/Manikin front Down Right.png
 Task/Manikin front Up Right.png
 Task/N-Back Revision.py
 Task/N-Back count.txt
 Task/N-Back.py
 Task/PIS.docx
 Task/PIS.txt
+Task/Posh App - my version.py
+Task/Posh App.py
 Task/Python Install.bat
 Task/README.txt.txt
 Task/RT count.txt
 Task/Reaction Time Task - Copy.py
 Task/Suffix.bat
 Task/Switch Count.txt
 Task/Switch count.txt
 Task/Switching.py
 Task/Task.py
 Task/Trial.py
+Task/UBL.PNG
+Task/UBR.PNG
+Task/UFL.PNG
+Task/UFR.PNG
 Task/asterisk.png
 Task/circle.jpg
 Task/greendot.png
 Task/greentick.png
 Task/help.txt
 Task/participant number.txt
 Task/pins.csv
@@ -60,16 +81,20 @@
 Task/suffix.txt
 Task/trial.jpeg
 Task/uop.ico
 Task/uop.jpeg
 Task/uop.png
 Task/Participant 1/1 - Combined Reaction Times.csv
 Task/Participant 1/1 - Combined Scores.csv
+Task/Participant 1/1 - N-Back Reaction Times.csv
+Task/Participant 1/1 - N-Back Score.csv
 Task/Participant 1/1 - RT Reaction Times.csv
 Task/Participant 1/1 - RT Score.csv
+Task/Participant 1/1 - Switching Reaction Times.csv
+Task/Participant 1/1 - Switching Score.csv
 Task/Participant 2/2 - Consent.txt
 Task/Participant 90210/90210 - Combined Reaction Times.csv
 Task/Participant 90210/90210 - Combined Scores.csv
 Task/Participant 90210/90210 - N-Back Reaction Times.csv
 Task/Participant 90210/90210 - N-Back Score.csv
 Task/__pycache__/Dependencies.cpython-311.pyc
 Task/__pycache__/Export.cpython-311.pyc
```

### Comparing `JBPhD-2.2.2/Task/Analysis.py` & `JBPhD-2.2.3/Task/Analysis.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Api.json` & `JBPhD-2.2.3/Task/Api.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Api2.json` & `JBPhD-2.2.3/Task/Api2.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Back_Right.PNG` & `JBPhD-2.2.3/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Consent Form.docx` & `JBPhD-2.2.3/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Dependencies.py` & `JBPhD-2.2.3/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Dependency Installation.py` & `JBPhD-2.2.3/Task/Dependency Installation.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Email Output.py` & `JBPhD-2.2.3/Task/Email Output.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Export.py` & `JBPhD-2.2.3/Task/Export.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Front_Left.PNG` & `JBPhD-2.2.3/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Front_Right.PNG` & `JBPhD-2.2.3/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Gradient Background.py` & `JBPhD-2.2.3/Task/Gradient Background.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Graph.py` & `JBPhD-2.2.3/Task/Graph.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/ImageSample.PNG` & `JBPhD-2.2.3/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Inverse_Back_Left.PNG` & `JBPhD-2.2.3/Task/Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Manikin Back Down Left.png` & `JBPhD-2.2.3/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Manikin Back Up Right.png` & `JBPhD-2.2.3/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Manikin front Down Right.png` & `JBPhD-2.2.3/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Manikin front Up Right.png` & `JBPhD-2.2.3/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/N-Back Revision.py` & `JBPhD-2.2.3/Task/N-Back Revision.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/N-Back.py` & `JBPhD-2.2.3/Task/N-Back.py`

 * *Files 8% similar despite different names*

```diff
@@ -214,16 +214,14 @@
     pygame.display.update()
     
 def generate_sequence(length):
     return [random.randint(0, 9) for _ in range(length)]
 
 def play_n_back(n, length):
     sequence = generate_sequence(length)
-    #print(f"Sequence: {sequence}")
-    #print(f"Starting n-back game with n={n}...")
     for i in range(n, length):
         if sequence[i] == sequence[i - n]:
             print(f"Match! Current digit is {sequence[i]}")
         else:
             print(f"No match. Current digit is {sequence[i]}")
         time.sleep(1)
 
@@ -238,20 +236,20 @@
 import os
 import time
 from datetime import datetime
 import random
 
 def generate_sequence(length):
     sequence = []
-    guaranteed_twobacks = random.sample(range(1, length-1), 2)  # Generate two random indices for guaranteed 2-backs
+    guaranteed_twobacks = random.sample(range(1, length-1), 2)
     for i in range(length):
         if i in guaranteed_twobacks:
-            sequence.append(sequence[i-2])  # Add the digit from two steps back
+            sequence.append(sequence[i-2]) 
         else:
-            sequence.append(random.randint(0, 9))  # Add a random digit
+            sequence.append(random.randint(0, 9))
     return sequence
 
 def introduction():
     pygame.font.init()
     os.environ["SDL_VIDEO_CENTERED"] = "1"
     score = 0
     font = pygame.font.Font(None, 32)
@@ -319,18 +317,15 @@
                         if KEY_MAPPING[event.key]:
                             print("J - Non-2-Back")
                             incorrect()
                             
                         else:
                         #J
                             print("F - Non-2-Back")
-                            correct()
-                            
-
-                            
+                            correct()                         
 
         pygame.display.update()
         screen.fill(WHITE)
         pygame.time.wait(1000)
         screen.fill(WHITE)
         pygame.time.wait(2000)
         
@@ -369,21 +364,21 @@
 
             with open(filename4, mode="a+") as file:
                 file.write(f"{date_time_string}, {count}, {score}, N-Back\n")
 
             with open(filename3, mode="a+") as file:
                 file.write(f"{date_time_string}, {count}, {RT}, N-Back\n")
 
-
             pygame.display.update()
         print(score)
 
         screen.fill(WHITE)
 
         draw_text(str(sequence[current_index]), (WINDOW_SIZE[0] // 2, WINDOW_SIZE[1] // 2), BLACK)
+        print(sequence)
         pygame.time.wait(1000)
         now = datetime.now()
         pygame.display.update()
 
         outputtime = now.strftime("%H:%M:%S")
 
         current_index += 1
@@ -397,15 +392,14 @@
 
     pygame.font.init()
 
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     score = 0
 
-    # font
     font = pygame.font.Font(None, 32)
 
     order = 1
 
     start_time = pygame.time.get_ticks()
 
     Game_Running = True
@@ -414,49 +408,46 @@
     screen = pygame.display.set_mode(size, pygame.FULLSCREEN)
     screen.fill(WHITE)
     pygame.display.set_caption("Welcome to the Task")
     font = pygame.font.Font(None, 60)
     text = font.render("Welcome to the Task", True, BLACK)
     text_rect = text.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2))
     screen.blit(text, text_rect)
-
     
     correctinterval = pygame.image.load("greentick.png")
     correctintervaldimensions = correctinterval.get_rect(center=screen.get_rect().center) 
 
     incorrectinterval = pygame.image.load("redcross.png")
     incorrectintervaldimensions = incorrectinterval.get_rect(center=screen.get_rect().center)# Set up the game
     n = 2
     sequence_length = 12
     sequence = generate_sequence(sequence_length)
     current_index = n
     score = 0
-    # Start the game loop
     running = True
 
     def incorrect():
         endRT = time.time()
         draw_text("Incorrect!", (WINDOW_SIZE[0] // 2, FONT_SIZE * 2), BLACK)
         screen.fill(WHITE)
         pygame.time.wait(1000)
         pygame.display.update()
-        #print("Incorrect")
         score = 0
 
     def correct():
         endRT = time.time()
         draw_text("Incorrect!", (WINDOW_SIZE[0] // 2, FONT_SIZE * 2), BLACK)
         screen.fill(WHITE)
         pygame.time.wait(1000)
         pygame.display.update()
-        #print("Correct")
         score = 1
 
+    starterRT = time.time()
     while running:
-        starterRT = time.time()# Handle events
+
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
             elif event.type == pygame.KEYDOWN:
                 if event.key in KEY_MAPPING:
                     if sequence[current_index] == sequence[current_index - n]:
                         print("2-Back")
@@ -471,18 +462,14 @@
                             correct()
               
                         else:
                             incorrect()
 
                         endRT = time.time()
                         RT = (endRT - starterRT)
-                    #print("--------------------------")
-                    #print(f'Start RT: {starterRT}')
-                    #print(f'End RT: {endRT}')
-                    #print(f'Reaction time: {RT}')
 
                     print(f'Score: {score}')                                        
                     with open(filename, mode="a+") as file:
                         file.write(f"{date_time_string}, {count}, {score}, N-Back\n")
 
                     with open(filename2, mode="a+") as file:
                         file.write(f"{date_time_string}, {count}, {RT}, N-Back\n")
@@ -500,43 +487,90 @@
         pygame.time.wait(2000)
 
         draw_text(str(sequence[current_index]), (WINDOW_SIZE[0] // 2, WINDOW_SIZE[1] // 2), BLACK)
         now = datetime.now()
 
         outputtime = now.strftime("%H:%M:%S")
 
-        #print(f'Stimulus Presentation Time {outputtime}')        
-
-
-        #draw_text(f"Score: {score}", (WINDOW_SIZE[0] // 2, FONT_SIZE), BLACK)
-
         pygame.display.update()
 
         current_index += 1
         if current_index >= sequence_length:
             running = False
 
-        #time.sleep(1)
-
-    # End the game
     pygame.quit()
 
+def intertrial():
+    
+    pygame.font.init()
+
+    os.environ["SDL_VIDEO_CENTERED"] = "1"
+
+    score = 0
+
+    font = pygame.font.Font(None, 32)
+
+    order = 1
+
+    start_time = pygame.time.get_ticks()
+
+    Game_Running = True
+
+    starterRT = time.time()
+
+    size = [SCREEN_WIDTH, SCREEN_HEIGHT]
+    screen = pygame.display.set_mode(size, pygame.FULLSCREEN)
+    screen.fill(WHITE)
+    pygame.display.set_caption("")
+    font = pygame.font.Font(None, 60)
+    intertext = "The actual task will start now"
+    intertext2 = "Remember to be fast and accurate!"
+
+    timeout = 3
+
+    running = True
+    while running:
+        for event in pygame.event.get():
+            if event.type == pygame.QUIT:
+                running = False
+
+        elapsed_time = (pygame.time.get_ticks() - start_time) // 1000
+        remaining_time = timeout - elapsed_time
+        if remaining_time < 0:
+            running = False
+            remaining_time = 0
+
+        text4 = font.render(str(remaining_time), True, BLACK)
+        text_rect4 = text4.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2 + 300))
+        screen.fill(WHITE)
+        text = font.render(intertext, True, BLACK)
+        text_rect = text.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2))
+        text3 = font.render(intertext2, True, BLACK)
+        text_rect3 = text3.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2+100))
+
+        screen.blit(text3, text_rect3)
+        screen.blit(text, text_rect)
+        screen.blit(text4, text_rect4)
+
+        pygame.display.update()
+
+    pygame.time.wait(500)
+    pygame.display.update()
+
 def exitscreen():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     df = pd.read_csv(filename2, usecols=[2], header=None)
     mean = df.mean().values[0]
 
     accuracydf = pd.read_csv(filename, usecols=[2], header=None)
     accuracydf = accuracydf.round(1)
 
     counter = accuracydf.count().values[0]
     formatted_num = "{:.2f}".format(mean)
-    ##print(formatted_num)
-
 
     totalscore = accuracydf.sum().values[0]
 
     ##print(totalscore,counter)
     finalscore = totalscore / counter * 100
     ##print("Percentage" , finalscore)
 
@@ -572,12 +606,13 @@
     pygame.time.delay(10000)
 
 if __name__ == "__main__":
     
     show_welcome_screen()
     instructions()
     introduction()
-    '''main()
+    intertrial()
+    main()
     exitscreen()
     subprocess.run([python_path, 'Export.py'], check=True)
     subprocess.run([python_path, 'Export.py'], check=True)
-    sysexit()'''
+    sysexit()
```

### Comparing `JBPhD-2.2.2/Task/PIS.docx` & `JBPhD-2.2.3/Task/PIS.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/PIS.txt` & `JBPhD-2.2.3/Task/PIS.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Participant 1/1 - Combined Reaction Times.csv` & `JBPhD-2.2.3/Task/Participant 1/1 - RT Reaction Times.csv`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 24-05-23, 6, 1.0071587562561035, Reaction Time
 24-05-23, 6, 1.0059690475463867, Reaction Time
 24-05-23, 6, 1.006563425064087, Reaction Time
 24-05-23, 6, 0.002013683319091797, Reaction Time
 24-05-23, 14, 2.013089179992676, Reaction Time
 24-05-23, 14, 1.0074832439422607, Reaction Time
 24-05-23, 14, 2.0139002799987793, Reaction Time
+24-05-23, 16, 0.0, Reaction Time
 24-05-23, 17, 0.0, Reaction Time
 24-05-23, 17, 0.0, Reaction Time
 24-05-23, 17, 0.0, Reaction Time
 24-05-23, 18, 0.0021135807037353516, Reaction Time
 24-05-23, 18, 0.002226114273071289, Reaction Time
 24-05-23, 18, 0.0017604827880859375, Reaction Time
 24-05-23, 18, 0.0, Reaction Time
```

### Comparing `JBPhD-2.2.2/Task/Participant 1/1 - Combined Scores.csv` & `JBPhD-2.2.3/Task/Participant 1/1 - RT Score.csv`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 24-05-23, 22, 0, Reaction Time
 24-05-23, 22, 0, Reaction Time
 24-05-23, 22, 0, Reaction Time
 24-05-23, 22, 0, Reaction Time
 24-05-23, 23, 0, Reaction Time
 24-05-23, 23, 1, Reaction Time
 24-05-23, 24, 1, Reaction Time
+24-05-23, 32, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
 24-05-23, 33, 0, Reaction Time
```

### Comparing `JBPhD-2.2.2/Task/Participant 2/2 - Consent.txt` & `JBPhD-2.2.3/Task/Participant 2/2 - Consent.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Participant 90210/90210 - Combined Reaction Times.csv` & `JBPhD-2.2.3/Task/Participant 90210/90210 - Combined Reaction Times.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Participant 90210/90210 - Combined Scores.csv` & `JBPhD-2.2.3/Task/Participant 90210/90210 - Combined Scores.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Participant 90210/90210 - N-Back Reaction Times.csv` & `JBPhD-2.2.3/Task/Participant 90210/90210 - N-Back Reaction Times.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Participant 90210/90210 - N-Back Score.csv` & `JBPhD-2.2.3/Task/Participant 90210/90210 - N-Back Score.csv`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Python Install.bat` & `JBPhD-2.2.3/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Reaction Time Task - Copy.py` & `JBPhD-2.2.3/Task/Reaction Time Task - Copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,16 +385,14 @@
     text_rect = text.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2 + 50))
     screen.blit(text, text_rect)
 
     pygame.display.update()
     # pygame.time.delay(500)
     pygame.time.delay(10000)
     
-
-
 global ast
 global cir
 ast = 0
 cir = 0
 
 def task():
 
@@ -518,16 +516,15 @@
             pygame.display.update()
             pygame.time.wait(500)
             end = time.time()
             score = 0
             elapse = start - end
             # can bin off any triggers of 16, suggests missed trials
             print(f'Elapsed: {elapse}')
-            break      
-        
+            break   
 
         pygame.display.update()
         pygame.time.delay(1000)
 
     with open(filename, mode="a+") as file:
         file.write(f"{date_time_string}, {count}, {score}, Reaction Time\n")
```

### Comparing `JBPhD-2.2.2/Task/Switching.py` & `JBPhD-2.2.3/Task/Switching.py`

 * *Files 20% similar despite different names*

```diff
@@ -490,42 +490,56 @@
         screen.blit(text, text_rect)
 
         # Update the display
         pygame.display.update()
 
     pygame.display.update()
 
+global lowercount
+global highercount
+lowercount = 0
+highercount = 0
 
-def nback():
+def maths():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
     score = 0
+    global lowercount
+    global highercount
 
     # font
     font = pygame.font.Font(None, 48)
 
     order = 1
 
+    a = random.randint(1, 10)
+    b = random.randint(1, 10)
+    op = random.choice(["+", "-"])
+    if op == "+":
+        result = a + b
+    else:
+        result = a - b
+
+    if result > 5:
+        highercount += 1
+
+    if result < 5:
+        lowercount += 1
+
     Game_Running = True
 
     starterRT = time.time()
 
     while Game_Running:
         # Set the screen background
         screen.fill(WHITE)
 
         starterRT = time.time()
 
         # Generate random addition or subtraction problem
-        a = random.randint(1, 10)
-        b = random.randint(1, 10)
-        op = random.choice(["+", "-"])
-        if op == "+":
-            result = a + b
-        else:
-            result = a - b
+
 
         # Display problem on the screen
         screen.fill(WHITE)
         problem_text = f" {a} {op} {b}?"
         text = font.render(problem_text, True, BLACK)
         text_rect = text.get_rect(center=(SCREEN_WIDTH / 2, 80))
         screen.blit(text, text_rect)
@@ -590,18 +604,48 @@
         file.write(date_time_string + ',' + str(score) + ',' + str("Reaction Time"))
         file.write("\n")
 
     with open(str(participant_number) + " - Combined RT Output.csv", mode="a+") as file:
         file.write(date_time_string + ',' + str(RT) + ',' + str("Reaction Time"))
         file.write("\n")
 
+global ballcount
+global FL
+global FR
+global BL
+global BR
+global UFL
+global UFR
+global UBL
+global UBR
+
+FL = 0
+FR = 0
+BL = 0
+BR = 0
+UFL = 0
+UFR = 0
+UBL = 0
+UBR = 0
+ballcount = 0
 
-def nbackball():
+def ball():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
+    global ballcount
+    global FL
+    global FR
+    global BL
+    global BR
+    global UFL
+    global UFR
+    global UBL
+    global UBR    
+
 
+    
     score = 0
 
     # Loop until the user clicks the close button.
     done = False
 
     clock = pygame.time.Clock()
 
@@ -619,35 +663,140 @@
     display_instructions = True
     instruction_page = 1
 
     DISPLAYSURF = pygame.display.set_mode(
         (SCREEN_WIDTH, SCREEN_HEIGHT), pygame.FULLSCREEN
     )
 
-    # DISPLAYSURF.fill(WHITE)
+    import random
+
+    available_orders = []
+
+    if UFR < 8:
+        available_orders.append(1)
+        available_orders.append(1)
+        available_orders.append(1)
+        available_orders.append(1)        
+
+    if UFL < 8:
+        available_orders.append(2)
+        available_orders.append(2)
+        available_orders.append(2)
+        available_orders.append(2)
+
+    if UBR < 8:
+        available_orders.append(3)
+        available_orders.append(3)
+        available_orders.append(3)
+        available_orders.append(3)
+
+
+    if UBL < 8:
+        available_orders.append(4)
+        available_orders.append(4)
+        available_orders.append(4)
+        available_orders.append(4)
+
+
+    if FR < 8:
+        available_orders.append(5)
+        available_orders.append(5)
+        available_orders.append(5)
+        available_orders.append(5)
+
+
+    if FL < 8:
+        available_orders.append(6)
+        available_orders.append(6)
+        available_orders.append(6)
+        available_orders.append(6)
+
+
+    if BR < 8:
+        available_orders.append(7)
+        available_orders.append(7)
+        available_orders.append(7)
+        available_orders.append(7)
+
+    if BL < 8:
+        available_orders.append(8)
+        available_orders.append(8)
+        available_orders.append(8)
+        available_orders.append(8)
+        
+
+    print(available_orders)
+
+    if available_orders:
+        order = random.choice(available_orders)
+
+        if order == 1:
+            ImageSample = pygame.image.load("UFR.png")
+            UFR += 1
+        elif order == 2:
+            ImageSample = pygame.image.load("UFL.png")
+            UFL += 1
+        elif order == 3:
+            ImageSample = pygame.image.load("UBR.png")
+            UBR += 1
+        elif order == 4:
+            ImageSample = pygame.image.load("UBL.png")
+            UBL += 1
+        elif order == 5:
+            ImageSample = pygame.image.load("FR.png")
+            FR += 1
+        elif order == 6:
+            ImageSample = pygame.image.load("FL.png")
+            FL += 1
+        elif order == 7:
+            ImageSample = pygame.image.load("BR.png")
+            BR += 1
+        elif order == 8:
+            ImageSample = pygame.image.load("BL.png")
+            BL += 1
+
+        if UFR > 8:
+            available_orders.remove(1)
+
+        if UFL > 8:
+            available_orders.remove(2)
+
+        if UBR > 8:
+            available_orders.remove(3)
+
+        if UBL > 8:
+            available_orders.remove(4)
+
+        if FR > 8:
+            available_orders.remove(5)
+
+        if FL > 8:
+            available_orders.remove(6)
+
+        if BR > 8:
+            available_orders.remove(7)
+
+        if BL > 8:
+            available_orders.remove(8)
 
-    order = random.randint(1, 4)
+    else:
+        ImageSample = pygame.Surface((0, 0))
 
     Game_Running = True
 
     starterRT = time.time()
 
-    while Game_Running:
-        # Set the screen background
-        screen.fill(WHITE)
+    timeout = 3
 
-        if order == 4:
-            ImageSample = pygame.image.load("Front_Right.png")
-        if order == 1:
-            ImageSample = pygame.image.load("Inverse_Back_Left.png")
-        if order == 3:
-            ImageSample = pygame.image.load("Front_Right.png")
-        if order == 2:
-            ImageSample = pygame.image.load("Back_Right.png")
+    while Game_Running:
 
+        timenow = time.time()
+        
+        screen.fill(WHITE)
+        
         ImageSample_rect = ImageSample.get_rect(
             center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2 + 50)
         )
         screen.blit(ImageSample, ImageSample_rect)
 
         incorrectinterval = pygame.image.load("redcross.png")
         incorrectintervaldimensions = incorrectinterval.get_rect(
@@ -658,51 +807,69 @@
         correctintervaldimensions = correctinterval.get_rect(
             center=screen.get_rect().center
         )
 
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 Game_Running = False
+                
             pygame.event.pump()
 
             if event.type == pygame.KEYDOWN:
-                if event.key == pygame.K_f and order == 1:
+                if event.key == pygame.K_f and order in (2,4,6,8):
                     endRT = time.time()
                     RT = endRT - starterRT
 
                     screen.fill(WHITE)
                     score += 1
                     screen.blit(correctinterval, correctintervaldimensions)
                     pygame.time.wait(1000)
                     pygame.display.update()
                     pygame.time.wait(1000)
                     Game_Running = False
 
-                elif event.key == pygame.K_j and order in (2, 3, 4):
+                elif event.key == pygame.K_j and order in (1,3,5,7):
                     endRT = time.time()
                     RT = endRT - starterRT
 
                     screen.fill(WHITE)
                     score += 1
                     screen.blit(correctinterval, correctintervaldimensions)
                     pygame.time.wait(1000)
                     pygame.display.update()
                     pygame.time.wait(1000)
                     Game_Running = False
 
-                else:  # if incorrect key was pressed
+                elif event.key == pygame.K_f and order in (1,3,5,7) or event.key == pygame.K_j and order in (2,4,6,8):
                     endRT = time.time()
                     RT = endRT - starterRT
                     screen.fill(WHITE)
                     screen.blit(incorrectinterval, incorrectintervaldimensions)
                     pygame.time.wait(1000)
                     pygame.display.update()
                     pygame.time.wait(1000)
                     Game_Running = False
 
+        overalltime = timenow - starterRT
+        #print(overalltime)
+
+        if overalltime > 3:
+            Game_Running = False
+            RT = overalltime
+            DISPLAYSURF.fill(WHITE)
+            pygame.time.wait(500)
+            pygame.display.update()
+            pygame.time.wait(500)
+            end = time.time()
+            score = 0
+           
+            # can bin off any triggers of 16, suggests missed trials
+            
+            break
+        
         pygame.display.update()
         pygame.time.delay(500)
 
     with open(filename, mode="a+") as file:
         file.write(f"{date_time_string}, {count}, {score}, Switching\n")
 
     with open(filename2, mode="a+") as file:
@@ -710,14 +877,73 @@
 
     with open(filename4, mode="a+") as file:
         file.write(f"{date_time_string}, {count}, {score}, Switching\n")
 
     with open(filename3, mode="a+") as file:
         file.write(f"{date_time_string}, {count}, {RT}, Switching\n")
 
+    ballcount += 1
+
+def intertrial():
+    
+    pygame.font.init()
+
+    os.environ["SDL_VIDEO_CENTERED"] = "1"
+
+    score = 0
+
+    font = pygame.font.Font(None, 32)
+
+    order = 1
+
+    start_time = pygame.time.get_ticks()
+
+    Game_Running = True
+
+    starterRT = time.time()
+
+    size = [SCREEN_WIDTH, SCREEN_HEIGHT]
+    screen = pygame.display.set_mode(size, pygame.FULLSCREEN)
+    screen.fill(WHITE)
+    pygame.display.set_caption("")
+    font = pygame.font.Font(None, 60)
+    intertext = "The actual task will start now"
+    intertext2 = "Remember to be fast and accurate!"
+
+    timeout = 3
+
+    running = True
+    while running:
+        for event in pygame.event.get():
+            if event.type == pygame.QUIT:
+                running = False
+
+        elapsed_time = (pygame.time.get_ticks() - start_time) // 1000
+        remaining_time = timeout - elapsed_time
+        if remaining_time < 0:
+            running = False
+            remaining_time = 0
+
+        text4 = font.render(str(remaining_time), True, BLACK)
+        text_rect4 = text4.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2 + 300))
+        screen.fill(WHITE)
+        text = font.render(intertext, True, BLACK)
+        text_rect = text.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2))
+        text3 = font.render(intertext2, True, BLACK)
+        text_rect3 = text3.get_rect(center=(SCREEN_WIDTH / 2, SCREEN_HEIGHT / 2+100))
+
+        screen.blit(text3, text_rect3)
+        screen.blit(text, text_rect)
+        screen.blit(text4, text_rect4)
+
+        pygame.display.update()
+
+    pygame.time.wait(500)
+    pygame.display.update()
+
 def exitscreen():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     df = pd.read_csv(filename2, usecols=[2], header=None)
     mean = df.mean().values[0]
 
     accuracydf = pd.read_csv(filename, usecols=[2], header=None)
@@ -762,26 +988,42 @@
     screen.blit(text, text_rect)
 
     pygame.display.update()
     # pygame.time.delay(500)
     pygame.time.delay(10000)
 
 def trialorder():
-    for i in range(0, 40):
+    for i in range(0, 46):
         torder = random.randint(1, 2)
         if torder == 1:
-            nback()
+            maths()
+            print("Lower Count: ",lowercount)
+            print("Higher Count: ",highercount)
+            
         else:
-            nbackball()
+            ball()
+
+            print("Total Count ",ballcount)
+            print("Front Left ", FL)
+            print("Front Right ", FR)
+            print("Back Left", BL)
+            print("Back Right ",BR)
+            print("Upside Front Left ",UFL)
+            print("Upside Front Right ",UFR) 
+            print("Upside Back Left ",UBL)
+            print("Upside Back Right ", UBR)
+            print("\n\n")
+
 
  
 trialcounter = 0
 
 fileremoval()
 show_welcome_screen()
 intro()
 introR()
 mathsintro()
+intertrial()
 trialorder()
 exitscreen()
 import Export
 pygame.quit()
```

### Comparing `JBPhD-2.2.2/Task/Task.py` & `JBPhD-2.2.3/Task/Task.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/Trial.py` & `JBPhD-2.2.3/Task/Trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         messagebox.showerror("Error", errortext)
         subprocess.run([python_path, 'Export.py'], check=True)
     else:
         file_path = "N-Back.py"
         subprocess.run([python_path, file_path], check=True)
         subprocess.run([python_path, 'Export.py'], check=True)
     
-nback = tk.Button(nback_frame, text="N-Back", command=nbrun, font=fontsize, anchor="center")
+nback = tk.Button(nback_frame, text="2-Back", command=nbrun, font=fontsize, anchor="center")
 nback.pack(side=tk.TOP, pady=5)
 
 if nbcount == 1:
     text = f"You have completed this {nbcount} time so far"
 else:
     text = f"You have completed this {nbcount} times so far"
 nback_label = tk.Label(nback_frame, text=text, font=fontsize2)
@@ -172,15 +172,15 @@
     else:
         file_path = "Reaction Time Task - Copy.py"
         subprocess.run([python_path, file_path], check=True)
         subprocess.run([python_path, 'Export.py'], check=True)
 
 button3_frame = tk.Frame(root)
 button3_frame.pack(side=tk.TOP, padx=30, pady=10, anchor="center")
-button3 = tk.Button(button3_frame, text="2-Type Reaction Time", command=consent, font=fontsize, anchor="center")
+button3 = tk.Button(button3_frame, text="2-Choice Reaction Time", command=consent, font=fontsize, anchor="center")
 button3.pack(side=tk.TOP, pady=5)
 
 if rtcount == 1:
     text = f"You have completed this {rtcount} time so far"
 else:
     text = f"You have completed this {rtcount} times so far"
 button3_label = tk.Label(button3_frame, text=text, font=fontsize2)
```

### Comparing `JBPhD-2.2.2/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.2.3/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.2.3/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.2.3/Task/__pycache__/Location.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc8d34664 (Mon Apr 24 19:08:56 2023 UTC)
-files sz: 384
+moddate:  0x2c926f64 (Thu May 25 16:51:56 2023 UTC)
+files sz: 382
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x97000200650064006401a6020000ab02000000000000000035005a0165
@@ -40,15 +40,15 @@
                118 STORE_NAME               5 (first_word)
    
      8         120 LOAD_NAME                5 (first_word)
                122 LOAD_CONST               3 ('uni.ds.port.ac.uk')
                124 COMPARE_OP               2 (==)
                130 POP_JUMP_FORWARD_IF_FALSE     3 (to 138)
    
-     9         132 LOAD_CONST               4 ('\nConnected from a University device')
+     9         132 LOAD_CONST               4 ('Connected from a University device')
                134 STORE_NAME               6 (loc)
                136 JUMP_FORWARD             2 (to 142)
    
     12     >>  138 LOAD_CONST               5 ('Connected from a non-University device')
                140 STORE_NAME               6 (loc)
    
      2     >>  142 LOAD_CONST               6 (None)
@@ -77,18 +77,18 @@
      168 to 174 -> 176 [3] lasti
      182 to 182 -> 176 [3] lasti
    consts
       'Suffix.txt'
       'r'
       0
       'uni.ds.port.ac.uk'
-      '\nConnected from a University device'
+      'Connected from a University device'
       'Connected from a non-University device'
       None
    names      ('open', 'f', 'readline', 'split', 'first_line_words', 'first_word', 'loc')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'H:\\Task Development\\Stimuli\\Location.py'
+   filename   'D:\\Task Development\\Stimuli\\Task\\Location.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02021a024c0210020c01060304f6
```

### Comparing `JBPhD-2.2.2/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.2.3/Task/__pycache__/Task.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,78 +1,77 @@
 magic:    0xa70d0d0a
-moddate:  0xaa0a5864 (Sun May  7 20:31:38 2023 UTC)
-files sz: 12958
+moddate:  0x00496664 (Thu May 18 15:49:20 2023 UTC)
+files sz: 13650
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c015a02640064
       016c035a03640284005a0402006504a6000000ab00000000000000000090
-      03725964035a0565036a060000000000000000a007000000000000000000
+      03723f64035a0565036a060000000000000000a007000000000000000000
       00000000000000000000006404a6010000ab010000000000000000720364
       035a086e69640064016c015a02640064016c095a09640064056c016d0a5a
       0a6d0b5a0b0100640064016c035a0302004700640684006407a6020000ab
       0200000000000000005a0c650d64086b02000000007242020065026a0e00
       00000000000000a6000000ab0000000000000000005a0f0200650c650fa6
       010000ab0100000000000000000100650fa0100000000000000000000000
       000000000000000000a6000000ab0000000000000000000100650fa01100
       00000000000000000000000000000000000000a6000000ab000000000000
       0000000100640064016c125a1202006513640965126a1400000000000000
       009b00640a9d03a6010000ab0100000000000000000100640064016c155a
-      15640064016c165a16640064016c035a0365166a1700000000000000005a
-      1865185a1965036a1a0000000000000000640b7802780219000000000000
-      00000065036a1b000000000000000065197a0000007a0d0000630363023c
-      00000064045a1c0200651d651c640ca6020000ab02000000000000000035
-      005a1e651ea01f0000000000000000000000000000000000000000a60000
-      00ab0000000000000000005a206520a02100000000000000000000000000
-      00000000000000a6000000ab0000000000000000005a2264015a14652244
-      005d215a236523a0240000000000000000000000000000000000000000a6
-      000000ab000000000000000000720b020065256523a6010000ab01000000
-      00000000005a148c220900640164016401a6020000ab0200000000000000
-      0001006e0b23003100730477027803590077010100590001000100640d65
-      149b009d025a260900020065036a2700000000000000006526a6010000ab
-      010000000000000000010002006513640e65269b00640f9d03a6010000ab
-      01000000000000000001006e16230065282400720e0100020065136410a6
-      010000ab010000000000000000010059006e047700780359007701020065
-      156a2900000000000000006411670164036403ac12a6030000ab03000000
-      00000000005a2a640064016c2b5a2b640064016c2c5a2c020065156a2d00
-      00000000000000651964136702a6010000ab0100000000000000005a2e64
-      0064016c2f5a2f640064016c305a30640064016c015a02640064016c315a
-      31640064146c015400640064156c326d335a336d345a340100640064166c
-      356d355a350100640064176c016d365a360100640064056c016d0a5a0a6d
-      0b5a0b0100640064016c375a3764185a3864195a390200651d6539640ca6
-      020000ab02000000000000000035005a1e651ea01f000000000000000000
-      0000000000000000000000a6000000ab0000000000000000005a206520a0
-      210000000000000000000000000000000000000000a6000000ab00000000
-      00000000005a2264015a3a652244005d215a236523a02400000000000000
-      00000000000000000000000000a6000000ab000000000000000000720b02
-      0065256523a6010000ab0100000000000000005a3a8c2209006401640164
-      01a6020000ab02000000000000000001006e0b2300310073047702780359
-      0077010100590001000100641a5a3b0200651d653b640ca6020000ab0200
-      0000000000000035005a1e651ea01f000000000000000000000000000000
-      0000000000a6000000ab0000000000000000005a206520a0210000000000
-      000000000000000000000000000000a6000000ab0000000000000000005a
-      2264015a3c652244005d215a236523a02400000000000000000000000000
-      00000000000000a6000000ab000000000000000000720b020065256523a6
-      010000ab0100000000000000005a3c8c220900640164016401a6020000ab
-      02000000000000000001006e0b2300310073047702780359007701010059
-      0001000100641b5a3d0200651d653d640ca6020000ab0200000000000000
-      0035005a1e651ea01f0000000000000000000000000000000000000000a6
-      000000ab0000000000000000005a206520a0210000000000000000000000
-      000000000000000000a6000000ab0000000000000000005a2264015a3e65
-      2244005d215a236523a02400000000000000000000000000000000000000
-      00a6000000ab000000000000000000720b020065256523a6010000ab0100
-      000000000000005a3e8c220900640164016401a6020000ab020000000000
-      00000001006e0b2300310073047702780359007701010059000100010064
-      0064016c125a12641c84005a3f0200653fa6000000ab0000000000000000
-      00010064015300640064016c015a02641d5a40641e5a41641f5a4264205a
-      43640064056c016d0a5a0a6d0b5a0b01000200650b6a4400000000000000
-      0064216540a6020000ab020000000000000000010064015300
+      15640064016c165a1665166a1700000000000000005a1865185a1965036a
+      1a0000000000000000640b780278021900000000000000000065036a1b00
+      0000000000000065197a0000007a0d0000630363023c00000064045a1c02
+      00651d651c640ca6020000ab02000000000000000035005a1e651ea01f00
+      00000000000000000000000000000000000000a6000000ab000000000000
+      0000005a206520a0210000000000000000000000000000000000000000a6
+      000000ab0000000000000000005a2264015a14652244005d215a236523a0
+      240000000000000000000000000000000000000000a6000000ab00000000
+      0000000000720b020065256523a6010000ab0100000000000000005a148c
+      220900640164016401a6020000ab02000000000000000001006e0b230031
+      00730477027803590077010100590001000100640d65149b009d025a2609
+      00020065036a2700000000000000006526a6010000ab0100000000000000
+      00010002006513640e65269b00640f9d03a6010000ab0100000000000000
+      0001006e16230065282400720e0100020065136410a6010000ab01000000
+      0000000000010059006e047700780359007701020065156a290000000000
+      0000006411670164036403ac12a6030000ab0300000000000000005a2a64
+      0064016c2b5a2b640064016c2c5a2c640064016c2d5a2d640064016c015a
+      02640064016c2e5a2e640064136c015400640064146c2f6d305a306d315a
+      310100640064156c326d325a320100640064166c016d335a330100640064
+      056c016d0a5a0a6d0b5a0b0100640064016c345a3464175a3564185a3602
+      00651d6536640ca6020000ab02000000000000000035005a1e651ea01f00
+      00000000000000000000000000000000000000a6000000ab000000000000
+      0000005a206520a0210000000000000000000000000000000000000000a6
+      000000ab0000000000000000005a2264015a37652244005d215a236523a0
+      240000000000000000000000000000000000000000a6000000ab00000000
+      0000000000720b020065256523a6010000ab0100000000000000005a378c
+      220900640164016401a6020000ab02000000000000000001006e0b230031
+      0073047702780359007701010059000100010064195a380200651d653864
+      0ca6020000ab02000000000000000035005a1e651ea01f00000000000000
+      00000000000000000000000000a6000000ab0000000000000000005a2065
+      20a0210000000000000000000000000000000000000000a6000000ab0000
+      000000000000005a2264015a39652244005d215a236523a0240000000000
+      000000000000000000000000000000a6000000ab00000000000000000072
+      0b020065256523a6010000ab0100000000000000005a398c220900640164
+      016401a6020000ab02000000000000000001006e0b230031007304770278
+      03590077010100590001000100641a5a3a0200651d653a640ca6020000ab
+      02000000000000000035005a1e651ea01f00000000000000000000000000
+      00000000000000a6000000ab0000000000000000005a206520a021000000
+      0000000000000000000000000000000000a6000000ab0000000000000000
+      005a2264015a3b652244005d215a236523a0240000000000000000000000
+      000000000000000000a6000000ab000000000000000000720b0200652565
+      23a6010000ab0100000000000000005a3b8c220900640164016401a60200
+      00ab02000000000000000001006e0b230031007304770278035900770101
+      00590001000100640064016c125a12641b84005a3c0200653ca6000000ab
+      000000000000000000010064015300640064016c015a02641c5a3d641d5a
+      3e641e5a3f641f5a40640064056c016d0a5a0a6d0b5a0b01000200650b6a
+      4100000000000000006420653da6020000ab020000000000000000010064
+      015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (socket)
                  8 STORE_NAME               0 (socket)
    
@@ -87,640 +86,620 @@
                 24 STORE_NAME               2 (tk)
    
      4          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               1 (None)
                 30 IMPORT_NAME              3 (os)
                 32 STORE_NAME               3 (os)
    
-     6          34 LOAD_CONST               2 (<code object is_connected, file "D:\Task Development\Stimuli\Task\Task.py", line 6>)
+     6          34 LOAD_CONST               2 (<code object is_connected, file "H:\Task Development\Stimuli\Task\Task.py", line 6>)
                 36 MAKE_FUNCTION            0
                 38 STORE_NAME               4 (is_connected)
    
     16          40 PUSH_NULL
                 42 LOAD_NAME                4 (is_connected)
                 44 PRECALL                  0
                 48 CALL                     0
                 58 EXTENDED_ARG             3
-                60 POP_JUMP_FORWARD_IF_FALSE   857 (to 1776)
+                60 POP_JUMP_FORWARD_IF_FALSE   831 (to 1724)
    
-    17          62 LOAD_CONST               3 (True)
+    18          62 LOAD_CONST               3 (True)
                 64 STORE_NAME               5 (Connected)
    
-    19          66 LOAD_NAME                3 (os)
+    20          66 LOAD_NAME                3 (os)
                 68 LOAD_ATTR                6 (path)
                 78 LOAD_METHOD              7 (exists)
                100 LOAD_CONST               4 ('participant number.txt')
                102 PRECALL                  1
                106 CALL                     1
                116 POP_JUMP_FORWARD_IF_FALSE     3 (to 124)
    
-    20         118 LOAD_CONST               3 (True)
+    21         118 LOAD_CONST               3 (True)
                120 STORE_NAME               8 (pathnum)
                122 JUMP_FORWARD           105 (to 334)
    
-    24     >>  124 LOAD_CONST               0 (0)
+    25     >>  124 LOAD_CONST               0 (0)
                126 LOAD_CONST               1 (None)
                128 IMPORT_NAME              1 (tkinter)
                130 STORE_NAME               2 (tk)
    
-    25         132 LOAD_CONST               0 (0)
+    26         132 LOAD_CONST               0 (0)
                134 LOAD_CONST               1 (None)
                136 IMPORT_NAME              9 (csv)
                138 STORE_NAME               9 (csv)
    
-    26         140 LOAD_CONST               0 (0)
+    27         140 LOAD_CONST               0 (0)
                142 LOAD_CONST               5 (('simpledialog', 'messagebox'))
                144 IMPORT_NAME              1 (tkinter)
                146 IMPORT_FROM             10 (simpledialog)
                148 STORE_NAME              10 (simpledialog)
                150 IMPORT_FROM             11 (messagebox)
                152 STORE_NAME              11 (messagebox)
                154 POP_TOP
    
-    27         156 LOAD_CONST               0 (0)
+    28         156 LOAD_CONST               0 (0)
                158 LOAD_CONST               1 (None)
                160 IMPORT_NAME              3 (os)
                162 STORE_NAME               3 (os)
    
-    29         164 PUSH_NULL
+    30         164 PUSH_NULL
                166 LOAD_BUILD_CLASS
-               168 LOAD_CONST               6 (<code object PinSystem, file "D:\Task Development\Stimuli\Task\Task.py", line 29>)
+               168 LOAD_CONST               6 (<code object PinSystem, file "H:\Task Development\Stimuli\Task\Task.py", line 30>)
                170 MAKE_FUNCTION            0
                172 LOAD_CONST               7 ('PinSystem')
                174 PRECALL                  2
                178 CALL                     2
                188 STORE_NAME              12 (PinSystem)
    
-    72         190 LOAD_NAME               13 (__name__)
+    74         190 LOAD_NAME               13 (__name__)
                192 LOAD_CONST               8 ('__main__')
                194 COMPARE_OP               2 (==)
                200 POP_JUMP_FORWARD_IF_FALSE    66 (to 334)
    
-    74         202 PUSH_NULL
+    76         202 PUSH_NULL
                204 LOAD_NAME                2 (tk)
                206 LOAD_ATTR               14 (Tk)
                216 PRECALL                  0
                220 CALL                     0
                230 STORE_NAME              15 (root)
    
-    75         232 PUSH_NULL
+    77         232 PUSH_NULL
                234 LOAD_NAME               12 (PinSystem)
                236 LOAD_NAME               15 (root)
                238 PRECALL                  1
                242 CALL                     1
                252 POP_TOP
    
-    76         254 LOAD_NAME               15 (root)
+    78         254 LOAD_NAME               15 (root)
                256 LOAD_METHOD             16 (mainloop)
                278 PRECALL                  0
                282 CALL                     0
                292 POP_TOP
    
-    77         294 LOAD_NAME               15 (root)
+    79         294 LOAD_NAME               15 (root)
                296 LOAD_METHOD             17 (quit)
                318 PRECALL                  0
                322 CALL                     0
                332 POP_TOP
    
-    79     >>  334 LOAD_CONST               0 (0)
+    81     >>  334 LOAD_CONST               0 (0)
                336 LOAD_CONST               1 (None)
                338 IMPORT_NAME             18 (spwf)
                340 STORE_NAME              18 (spwf)
    
-    81         342 PUSH_NULL
+    83         342 PUSH_NULL
                344 LOAD_NAME               19 (print)
                346 LOAD_CONST               9 ('Welcome to the task! Thank you for your interest in the study.\n\nYou are participant number ')
                348 LOAD_NAME               18 (spwf)
                350 LOAD_ATTR               20 (participant_number)
                360 FORMAT_VALUE             0
                362 LOAD_CONST              10 ('.\n\nThe task is now loading, it may take a short while to load.')
                364 BUILD_STRING             3
                366 PRECALL                  1
                370 CALL                     1
                380 POP_TOP
    
-    83         382 LOAD_CONST               0 (0)
+    85         382 LOAD_CONST               0 (0)
                384 LOAD_CONST               1 (None)
                386 IMPORT_NAME             21 (subprocess)
                388 STORE_NAME              21 (subprocess)
    
-    84         390 LOAD_CONST               0 (0)
+    86         390 LOAD_CONST               0 (0)
                392 LOAD_CONST               1 (None)
                394 IMPORT_NAME             22 (sys)
                396 STORE_NAME              22 (sys)
    
-    85         398 LOAD_CONST               0 (0)
-               400 LOAD_CONST               1 (None)
-               402 IMPORT_NAME              3 (os)
-               404 STORE_NAME               3 (os)
-   
-    87         406 LOAD_NAME               22 (sys)
-               408 LOAD_ATTR               23 (executable)
-               418 STORE_NAME              24 (pythonpath)
-   
-    88         420 LOAD_NAME               24 (pythonpath)
-               422 STORE_NAME              25 (python_path)
-   
-    89         424 LOAD_NAME                3 (os)
-               426 LOAD_ATTR               26 (environ)
-               436 LOAD_CONST              11 ('PATH')
-               438 COPY                     2
-               440 COPY                     2
-               442 BINARY_SUBSCR
-               452 LOAD_NAME                3 (os)
-               454 LOAD_ATTR               27 (pathsep)
-               464 LOAD_NAME               25 (python_path)
-               466 BINARY_OP                0 (+)
-               470 BINARY_OP               13 (+=)
-               474 SWAP                     3
-               476 SWAP                     2
-               478 STORE_SUBSCR
-   
-    91         482 LOAD_CONST               4 ('participant number.txt')
-               484 STORE_NAME              28 (filename)
-   
-    93         486 PUSH_NULL
-               488 LOAD_NAME               29 (open)
-               490 LOAD_NAME               28 (filename)
-               492 LOAD_CONST              12 ('r')
-               494 PRECALL                  2
-               498 CALL                     2
-               508 BEFORE_WITH
-               510 STORE_NAME              30 (f)
-   
-    94         512 LOAD_NAME               30 (f)
-               514 LOAD_METHOD             31 (readline)
-               536 PRECALL                  0
-               540 CALL                     0
-               550 STORE_NAME              32 (first_line)
-   
-    95         552 LOAD_NAME               32 (first_line)
-               554 LOAD_METHOD             33 (split)
-               576 PRECALL                  0
-               580 CALL                     0
-               590 STORE_NAME              34 (words)
-   
-    96         592 LOAD_CONST               1 (None)
-               594 STORE_NAME              20 (participant_number)
-   
-    97         596 LOAD_NAME               34 (words)
-               598 GET_ITER
-           >>  600 FOR_ITER                33 (to 668)
-               602 STORE_NAME              35 (word)
-   
-    98         604 LOAD_NAME               35 (word)
-               606 LOAD_METHOD             36 (isdigit)
-               628 PRECALL                  0
-               632 CALL                     0
-               642 POP_JUMP_FORWARD_IF_FALSE    11 (to 666)
-   
-    99         644 PUSH_NULL
-               646 LOAD_NAME               37 (int)
-               648 LOAD_NAME               35 (word)
-               650 PRECALL                  1
-               654 CALL                     1
-               664 STORE_NAME              20 (participant_number)
-           >>  666 JUMP_BACKWARD           34 (to 600)
-   
-    97     >>  668 NOP
-   
-    93         670 LOAD_CONST               1 (None)
-               672 LOAD_CONST               1 (None)
-               674 LOAD_CONST               1 (None)
-               676 PRECALL                  2
-               680 CALL                     2
-               690 POP_TOP
-               692 JUMP_FORWARD            11 (to 716)
-           >>  694 PUSH_EXC_INFO
-               696 WITH_EXCEPT_START
-               698 POP_JUMP_FORWARD_IF_TRUE     4 (to 708)
-               700 RERAISE                  2
-           >>  702 COPY                     3
-               704 POP_EXCEPT
-               706 RERAISE                  1
-           >>  708 POP_TOP
-               710 POP_EXCEPT
-               712 POP_TOP
-               714 POP_TOP
-   
-   100     >>  716 LOAD_CONST              13 ('Participant ')
-               718 LOAD_NAME               20 (participant_number)
-               720 FORMAT_VALUE             0
-               722 BUILD_STRING             2
-               724 STORE_NAME              38 (folder_name)
-   
-   102         726 NOP
-   
-   103         728 PUSH_NULL
-               730 LOAD_NAME                3 (os)
-               732 LOAD_ATTR               39 (mkdir)
-               742 LOAD_NAME               38 (folder_name)
-               744 PRECALL                  1
-               748 CALL                     1
-               758 POP_TOP
-   
-   104         760 PUSH_NULL
-               762 LOAD_NAME               19 (print)
-               764 LOAD_CONST              14 ("Created folder '")
-               766 LOAD_NAME               38 (folder_name)
-               768 FORMAT_VALUE             0
-               770 LOAD_CONST              15 ("'")
-               772 BUILD_STRING             3
-               774 PRECALL                  1
-               778 CALL                     1
-               788 POP_TOP
-               790 JUMP_FORWARD            22 (to 836)
-           >>  792 PUSH_EXC_INFO
-   
-   106         794 LOAD_NAME               40 (FileExistsError)
-               796 CHECK_EXC_MATCH
-               798 POP_JUMP_FORWARD_IF_FALSE    14 (to 828)
-               800 POP_TOP
-   
-   107         802 PUSH_NULL
-               804 LOAD_NAME               19 (print)
-               806 LOAD_CONST              16 ('')
-               808 PRECALL                  1
-               812 CALL                     1
-               822 POP_TOP
+    88         398 LOAD_NAME               22 (sys)
+               400 LOAD_ATTR               23 (executable)
+               410 STORE_NAME              24 (pythonpath)
+   
+    89         412 LOAD_NAME               24 (pythonpath)
+               414 STORE_NAME              25 (python_path)
+   
+    90         416 LOAD_NAME                3 (os)
+               418 LOAD_ATTR               26 (environ)
+               428 LOAD_CONST              11 ('PATH')
+               430 COPY                     2
+               432 COPY                     2
+               434 BINARY_SUBSCR
+               444 LOAD_NAME                3 (os)
+               446 LOAD_ATTR               27 (pathsep)
+               456 LOAD_NAME               25 (python_path)
+               458 BINARY_OP                0 (+)
+               462 BINARY_OP               13 (+=)
+               466 SWAP                     3
+               468 SWAP                     2
+               470 STORE_SUBSCR
+   
+    92         474 LOAD_CONST               4 ('participant number.txt')
+               476 STORE_NAME              28 (filename)
+   
+    94         478 PUSH_NULL
+               480 LOAD_NAME               29 (open)
+               482 LOAD_NAME               28 (filename)
+               484 LOAD_CONST              12 ('r')
+               486 PRECALL                  2
+               490 CALL                     2
+               500 BEFORE_WITH
+               502 STORE_NAME              30 (f)
+   
+    95         504 LOAD_NAME               30 (f)
+               506 LOAD_METHOD             31 (readline)
+               528 PRECALL                  0
+               532 CALL                     0
+               542 STORE_NAME              32 (first_line)
+   
+    96         544 LOAD_NAME               32 (first_line)
+               546 LOAD_METHOD             33 (split)
+               568 PRECALL                  0
+               572 CALL                     0
+               582 STORE_NAME              34 (words)
+   
+    97         584 LOAD_CONST               1 (None)
+               586 STORE_NAME              20 (participant_number)
+   
+    98         588 LOAD_NAME               34 (words)
+               590 GET_ITER
+           >>  592 FOR_ITER                33 (to 660)
+               594 STORE_NAME              35 (word)
+   
+    99         596 LOAD_NAME               35 (word)
+               598 LOAD_METHOD             36 (isdigit)
+               620 PRECALL                  0
+               624 CALL                     0
+               634 POP_JUMP_FORWARD_IF_FALSE    11 (to 658)
+   
+   100         636 PUSH_NULL
+               638 LOAD_NAME               37 (int)
+               640 LOAD_NAME               35 (word)
+               642 PRECALL                  1
+               646 CALL                     1
+               656 STORE_NAME              20 (participant_number)
+           >>  658 JUMP_BACKWARD           34 (to 592)
+   
+    98     >>  660 NOP
+   
+    94         662 LOAD_CONST               1 (None)
+               664 LOAD_CONST               1 (None)
+               666 LOAD_CONST               1 (None)
+               668 PRECALL                  2
+               672 CALL                     2
+               682 POP_TOP
+               684 JUMP_FORWARD            11 (to 708)
+           >>  686 PUSH_EXC_INFO
+               688 WITH_EXCEPT_START
+               690 POP_JUMP_FORWARD_IF_TRUE     4 (to 700)
+               692 RERAISE                  2
+           >>  694 COPY                     3
+               696 POP_EXCEPT
+               698 RERAISE                  1
+           >>  700 POP_TOP
+               702 POP_EXCEPT
+               704 POP_TOP
+               706 POP_TOP
+   
+   101     >>  708 LOAD_CONST              13 ('Participant ')
+               710 LOAD_NAME               20 (participant_number)
+               712 FORMAT_VALUE             0
+               714 BUILD_STRING             2
+               716 STORE_NAME              38 (folder_name)
+   
+   103         718 NOP
+   
+   104         720 PUSH_NULL
+               722 LOAD_NAME                3 (os)
+               724 LOAD_ATTR               39 (mkdir)
+               734 LOAD_NAME               38 (folder_name)
+               736 PRECALL                  1
+               740 CALL                     1
+               750 POP_TOP
+   
+   105         752 PUSH_NULL
+               754 LOAD_NAME               19 (print)
+               756 LOAD_CONST              14 ("Created folder '")
+               758 LOAD_NAME               38 (folder_name)
+               760 FORMAT_VALUE             0
+               762 LOAD_CONST              15 ("'")
+               764 BUILD_STRING             3
+               766 PRECALL                  1
+               770 CALL                     1
+               780 POP_TOP
+               782 JUMP_FORWARD            22 (to 828)
+           >>  784 PUSH_EXC_INFO
+   
+   107         786 LOAD_NAME               40 (FileExistsError)
+               788 CHECK_EXC_MATCH
+               790 POP_JUMP_FORWARD_IF_FALSE    14 (to 820)
+               792 POP_TOP
+   
+   108         794 PUSH_NULL
+               796 LOAD_NAME               19 (print)
+               798 LOAD_CONST              16 ('')
+               800 PRECALL                  1
+               804 CALL                     1
+               814 POP_TOP
+               816 POP_EXCEPT
+               818 JUMP_FORWARD             4 (to 828)
+   
+   107     >>  820 RERAISE                  0
+           >>  822 COPY                     3
                824 POP_EXCEPT
-               826 JUMP_FORWARD             4 (to 836)
+               826 RERAISE                  1
    
-   106     >>  828 RERAISE                  0
-           >>  830 COPY                     3
-               832 POP_EXCEPT
-               834 RERAISE                  1
-   
-   108     >>  836 PUSH_NULL
-               838 LOAD_NAME               21 (subprocess)
-               840 LOAD_ATTR               41 (run)
-               850 LOAD_CONST              17 ('Suffix.bat')
-               852 BUILD_LIST               1
-               854 LOAD_CONST               3 (True)
-               856 LOAD_CONST               3 (True)
-               858 KW_NAMES                18
-               860 PRECALL                  3
-               864 CALL                     3
-               874 STORE_NAME              42 (result)
+   109     >>  828 PUSH_NULL
+               830 LOAD_NAME               21 (subprocess)
+               832 LOAD_ATTR               41 (run)
+               842 LOAD_CONST              17 ('Suffix.bat')
+               844 BUILD_LIST               1
+               846 LOAD_CONST               3 (True)
+               848 LOAD_CONST               3 (True)
+               850 KW_NAMES                18
+               852 PRECALL                  3
+               856 CALL                     3
+               866 STORE_NAME              42 (result)
+   
+   110         868 LOAD_CONST               0 (0)
+               870 LOAD_CONST               1 (None)
+               872 IMPORT_NAME             43 (Location)
+               874 STORE_NAME              43 (Location)
    
-   109         876 LOAD_CONST               0 (0)
+   111         876 LOAD_CONST               0 (0)
                878 LOAD_CONST               1 (None)
-               880 IMPORT_NAME             43 (Location)
-               882 STORE_NAME              43 (Location)
+               880 IMPORT_NAME             44 (random)
+               882 STORE_NAME              44 (random)
    
-   110         884 LOAD_CONST               0 (0)
+   112         884 LOAD_CONST               0 (0)
                886 LOAD_CONST               1 (None)
-               888 IMPORT_NAME             44 (Dependencies)
-               890 STORE_NAME              44 (Dependencies)
+               888 IMPORT_NAME             45 (platform)
+               890 STORE_NAME              45 (platform)
    
-   111         892 PUSH_NULL
-               894 LOAD_NAME               21 (subprocess)
-               896 LOAD_ATTR               45 (Popen)
-               906 LOAD_NAME               25 (python_path)
-               908 LOAD_CONST              19 ('cputask.py')
-               910 BUILD_LIST               2
-               912 PRECALL                  1
-               916 CALL                     1
-               926 STORE_NAME              46 (cpurun)
-   
-   112         928 LOAD_CONST               0 (0)
-               930 LOAD_CONST               1 (None)
-               932 IMPORT_NAME             47 (random)
-               934 STORE_NAME              47 (random)
-   
-   113         936 LOAD_CONST               0 (0)
-               938 LOAD_CONST               1 (None)
-               940 IMPORT_NAME             48 (platform)
-               942 STORE_NAME              48 (platform)
+   113         892 LOAD_CONST               0 (0)
+               894 LOAD_CONST               1 (None)
+               896 IMPORT_NAME              1 (tkinter)
+               898 STORE_NAME               2 (tk)
+   
+   114         900 LOAD_CONST               0 (0)
+               902 LOAD_CONST               1 (None)
+               904 IMPORT_NAME             46 (time)
+               906 STORE_NAME              46 (time)
+   
+   115         908 LOAD_CONST               0 (0)
+               910 LOAD_CONST              19 (('*',))
+               912 IMPORT_NAME              1 (tkinter)
+               914 IMPORT_STAR
+   
+   116         916 LOAD_CONST               0 (0)
+               918 LOAD_CONST              20 (('Image', 'ImageTk'))
+               920 IMPORT_NAME             47 (PIL)
+               922 IMPORT_FROM             48 (Image)
+               924 STORE_NAME              48 (Image)
+               926 IMPORT_FROM             49 (ImageTk)
+               928 STORE_NAME              49 (ImageTk)
+               930 POP_TOP
+   
+   117         932 LOAD_CONST               0 (0)
+               934 LOAD_CONST              21 (('datetime',))
+               936 IMPORT_NAME             50 (datetime)
+               938 IMPORT_FROM             50 (datetime)
+               940 STORE_NAME              50 (datetime)
+               942 POP_TOP
    
-   114         944 LOAD_CONST               0 (0)
-               946 LOAD_CONST               1 (None)
+   118         944 LOAD_CONST               0 (0)
+               946 LOAD_CONST              22 (('filedialog',))
                948 IMPORT_NAME              1 (tkinter)
-               950 STORE_NAME               2 (tk)
+               950 IMPORT_FROM             51 (filedialog)
+               952 STORE_NAME              51 (filedialog)
+               954 POP_TOP
+   
+   119         956 LOAD_CONST               0 (0)
+               958 LOAD_CONST               5 (('simpledialog', 'messagebox'))
+               960 IMPORT_NAME              1 (tkinter)
+               962 IMPORT_FROM             10 (simpledialog)
+               964 STORE_NAME              10 (simpledialog)
+               966 IMPORT_FROM             11 (messagebox)
+               968 STORE_NAME              11 (messagebox)
+               970 POP_TOP
+   
+   120         972 LOAD_CONST               0 (0)
+               974 LOAD_CONST               1 (None)
+               976 IMPORT_NAME             52 (glob)
+               978 STORE_NAME              52 (glob)
+   
+   122         980 LOAD_CONST              23 ('Dependency Installation.py')
+               982 STORE_NAME              53 (file_path)
+   
+   124         984 LOAD_CONST              24 ('RT count.txt')
+               986 STORE_NAME              54 (RTcount)
+   
+   126         988 PUSH_NULL
+               990 LOAD_NAME               29 (open)
+               992 LOAD_NAME               54 (RTcount)
+               994 LOAD_CONST              12 ('r')
+               996 PRECALL                  2
+              1000 CALL                     2
+              1010 BEFORE_WITH
+              1012 STORE_NAME              30 (f)
+   
+   127        1014 LOAD_NAME               30 (f)
+              1016 LOAD_METHOD             31 (readline)
+              1038 PRECALL                  0
+              1042 CALL                     0
+              1052 STORE_NAME              32 (first_line)
+   
+   128        1054 LOAD_NAME               32 (first_line)
+              1056 LOAD_METHOD             33 (split)
+              1078 PRECALL                  0
+              1082 CALL                     0
+              1092 STORE_NAME              34 (words)
+   
+   129        1094 LOAD_CONST               1 (None)
+              1096 STORE_NAME              55 (rtcount)
+   
+   130        1098 LOAD_NAME               34 (words)
+              1100 GET_ITER
+           >> 1102 FOR_ITER                33 (to 1170)
+              1104 STORE_NAME              35 (word)
    
-   115         952 LOAD_CONST               0 (0)
-               954 LOAD_CONST               1 (None)
-               956 IMPORT_NAME             49 (time)
-               958 STORE_NAME              49 (time)
-   
-   116         960 LOAD_CONST               0 (0)
-               962 LOAD_CONST              20 (('*',))
-               964 IMPORT_NAME              1 (tkinter)
-               966 IMPORT_STAR
-   
-   117         968 LOAD_CONST               0 (0)
-               970 LOAD_CONST              21 (('Image', 'ImageTk'))
-               972 IMPORT_NAME             50 (PIL)
-               974 IMPORT_FROM             51 (Image)
-               976 STORE_NAME              51 (Image)
-               978 IMPORT_FROM             52 (ImageTk)
-               980 STORE_NAME              52 (ImageTk)
-               982 POP_TOP
-   
-   118         984 LOAD_CONST               0 (0)
-               986 LOAD_CONST              22 (('datetime',))
-               988 IMPORT_NAME             53 (datetime)
-               990 IMPORT_FROM             53 (datetime)
-               992 STORE_NAME              53 (datetime)
-               994 POP_TOP
-   
-   119         996 LOAD_CONST               0 (0)
-               998 LOAD_CONST              23 (('filedialog',))
-              1000 IMPORT_NAME              1 (tkinter)
-              1002 IMPORT_FROM             54 (filedialog)
-              1004 STORE_NAME              54 (filedialog)
-              1006 POP_TOP
-   
-   120        1008 LOAD_CONST               0 (0)
-              1010 LOAD_CONST               5 (('simpledialog', 'messagebox'))
-              1012 IMPORT_NAME              1 (tkinter)
-              1014 IMPORT_FROM             10 (simpledialog)
-              1016 STORE_NAME              10 (simpledialog)
-              1018 IMPORT_FROM             11 (messagebox)
-              1020 STORE_NAME              11 (messagebox)
-              1022 POP_TOP
-   
-   121        1024 LOAD_CONST               0 (0)
-              1026 LOAD_CONST               1 (None)
-              1028 IMPORT_NAME             55 (glob)
-              1030 STORE_NAME              55 (glob)
-   
-   123        1032 LOAD_CONST              24 ('Dependency Installation.py')
-              1034 STORE_NAME              56 (file_path)
-   
-   125        1036 LOAD_CONST              25 ('RT count.txt')
-              1038 STORE_NAME              57 (RTcount)
-   
-   127        1040 PUSH_NULL
-              1042 LOAD_NAME               29 (open)
-              1044 LOAD_NAME               57 (RTcount)
-              1046 LOAD_CONST              12 ('r')
-              1048 PRECALL                  2
-              1052 CALL                     2
-              1062 BEFORE_WITH
-              1064 STORE_NAME              30 (f)
-   
-   128        1066 LOAD_NAME               30 (f)
-              1068 LOAD_METHOD             31 (readline)
-              1090 PRECALL                  0
-              1094 CALL                     0
-              1104 STORE_NAME              32 (first_line)
-   
-   129        1106 LOAD_NAME               32 (first_line)
-              1108 LOAD_METHOD             33 (split)
+   131        1106 LOAD_NAME               35 (word)
+              1108 LOAD_METHOD             36 (isdigit)
               1130 PRECALL                  0
               1134 CALL                     0
-              1144 STORE_NAME              34 (words)
-   
-   130        1146 LOAD_CONST               1 (None)
-              1148 STORE_NAME              58 (rtcount)
+              1144 POP_JUMP_FORWARD_IF_FALSE    11 (to 1168)
    
-   131        1150 LOAD_NAME               34 (words)
-              1152 GET_ITER
-           >> 1154 FOR_ITER                33 (to 1222)
-              1156 STORE_NAME              35 (word)
-   
-   132        1158 LOAD_NAME               35 (word)
-              1160 LOAD_METHOD             36 (isdigit)
-              1182 PRECALL                  0
-              1186 CALL                     0
-              1196 POP_JUMP_FORWARD_IF_FALSE    11 (to 1220)
-   
-   133        1198 PUSH_NULL
-              1200 LOAD_NAME               37 (int)
-              1202 LOAD_NAME               35 (word)
-              1204 PRECALL                  1
-              1208 CALL                     1
-              1218 STORE_NAME              58 (rtcount)
-           >> 1220 JUMP_BACKWARD           34 (to 1154)
-   
-   131     >> 1222 NOP
-   
-   127        1224 LOAD_CONST               1 (None)
-              1226 LOAD_CONST               1 (None)
-              1228 LOAD_CONST               1 (None)
+   132        1146 PUSH_NULL
+              1148 LOAD_NAME               37 (int)
+              1150 LOAD_NAME               35 (word)
+              1152 PRECALL                  1
+              1156 CALL                     1
+              1166 STORE_NAME              55 (rtcount)
+           >> 1168 JUMP_BACKWARD           34 (to 1102)
+   
+   130     >> 1170 NOP
+   
+   126        1172 LOAD_CONST               1 (None)
+              1174 LOAD_CONST               1 (None)
+              1176 LOAD_CONST               1 (None)
+              1178 PRECALL                  2
+              1182 CALL                     2
+              1192 POP_TOP
+              1194 JUMP_FORWARD            11 (to 1218)
+           >> 1196 PUSH_EXC_INFO
+              1198 WITH_EXCEPT_START
+              1200 POP_JUMP_FORWARD_IF_TRUE     4 (to 1210)
+              1202 RERAISE                  2
+           >> 1204 COPY                     3
+              1206 POP_EXCEPT
+              1208 RERAISE                  1
+           >> 1210 POP_TOP
+              1212 POP_EXCEPT
+              1214 POP_TOP
+              1216 POP_TOP
+   
+   134     >> 1218 LOAD_CONST              25 ('N-Back count.txt')
+              1220 STORE_NAME              56 (NBcount)
+   
+   136        1222 PUSH_NULL
+              1224 LOAD_NAME               29 (open)
+              1226 LOAD_NAME               56 (NBcount)
+              1228 LOAD_CONST              12 ('r')
               1230 PRECALL                  2
               1234 CALL                     2
-              1244 POP_TOP
-              1246 JUMP_FORWARD            11 (to 1270)
-           >> 1248 PUSH_EXC_INFO
-              1250 WITH_EXCEPT_START
-              1252 POP_JUMP_FORWARD_IF_TRUE     4 (to 1262)
-              1254 RERAISE                  2
-           >> 1256 COPY                     3
-              1258 POP_EXCEPT
-              1260 RERAISE                  1
-           >> 1262 POP_TOP
-              1264 POP_EXCEPT
-              1266 POP_TOP
-              1268 POP_TOP
-   
-   135     >> 1270 LOAD_CONST              26 ('N-Back count.txt')
-              1272 STORE_NAME              59 (NBcount)
-   
-   137        1274 PUSH_NULL
-              1276 LOAD_NAME               29 (open)
-              1278 LOAD_NAME               59 (NBcount)
-              1280 LOAD_CONST              12 ('r')
-              1282 PRECALL                  2
-              1286 CALL                     2
-              1296 BEFORE_WITH
-              1298 STORE_NAME              30 (f)
-   
-   138        1300 LOAD_NAME               30 (f)
-              1302 LOAD_METHOD             31 (readline)
-              1324 PRECALL                  0
-              1328 CALL                     0
-              1338 STORE_NAME              32 (first_line)
+              1244 BEFORE_WITH
+              1246 STORE_NAME              30 (f)
    
-   139        1340 LOAD_NAME               32 (first_line)
-              1342 LOAD_METHOD             33 (split)
+   137        1248 LOAD_NAME               30 (f)
+              1250 LOAD_METHOD             31 (readline)
+              1272 PRECALL                  0
+              1276 CALL                     0
+              1286 STORE_NAME              32 (first_line)
+   
+   138        1288 LOAD_NAME               32 (first_line)
+              1290 LOAD_METHOD             33 (split)
+              1312 PRECALL                  0
+              1316 CALL                     0
+              1326 STORE_NAME              34 (words)
+   
+   139        1328 LOAD_CONST               1 (None)
+              1330 STORE_NAME              57 (nbcount)
+   
+   140        1332 LOAD_NAME               34 (words)
+              1334 GET_ITER
+           >> 1336 FOR_ITER                33 (to 1404)
+              1338 STORE_NAME              35 (word)
+   
+   141        1340 LOAD_NAME               35 (word)
+              1342 LOAD_METHOD             36 (isdigit)
               1364 PRECALL                  0
               1368 CALL                     0
-              1378 STORE_NAME              34 (words)
-   
-   140        1380 LOAD_CONST               1 (None)
-              1382 STORE_NAME              60 (nbcount)
+              1378 POP_JUMP_FORWARD_IF_FALSE    11 (to 1402)
    
-   141        1384 LOAD_NAME               34 (words)
-              1386 GET_ITER
-           >> 1388 FOR_ITER                33 (to 1456)
-              1390 STORE_NAME              35 (word)
-   
-   142        1392 LOAD_NAME               35 (word)
-              1394 LOAD_METHOD             36 (isdigit)
-              1416 PRECALL                  0
-              1420 CALL                     0
-              1430 POP_JUMP_FORWARD_IF_FALSE    11 (to 1454)
-   
-   143        1432 PUSH_NULL
-              1434 LOAD_NAME               37 (int)
-              1436 LOAD_NAME               35 (word)
-              1438 PRECALL                  1
-              1442 CALL                     1
-              1452 STORE_NAME              60 (nbcount)
-           >> 1454 JUMP_BACKWARD           34 (to 1388)
-   
-   141     >> 1456 NOP
-   
-   137        1458 LOAD_CONST               1 (None)
-              1460 LOAD_CONST               1 (None)
-              1462 LOAD_CONST               1 (None)
+   142        1380 PUSH_NULL
+              1382 LOAD_NAME               37 (int)
+              1384 LOAD_NAME               35 (word)
+              1386 PRECALL                  1
+              1390 CALL                     1
+              1400 STORE_NAME              57 (nbcount)
+           >> 1402 JUMP_BACKWARD           34 (to 1336)
+   
+   140     >> 1404 NOP
+   
+   136        1406 LOAD_CONST               1 (None)
+              1408 LOAD_CONST               1 (None)
+              1410 LOAD_CONST               1 (None)
+              1412 PRECALL                  2
+              1416 CALL                     2
+              1426 POP_TOP
+              1428 JUMP_FORWARD            11 (to 1452)
+           >> 1430 PUSH_EXC_INFO
+              1432 WITH_EXCEPT_START
+              1434 POP_JUMP_FORWARD_IF_TRUE     4 (to 1444)
+              1436 RERAISE                  2
+           >> 1438 COPY                     3
+              1440 POP_EXCEPT
+              1442 RERAISE                  1
+           >> 1444 POP_TOP
+              1446 POP_EXCEPT
+              1448 POP_TOP
+              1450 POP_TOP
+   
+   144     >> 1452 LOAD_CONST              26 ('Switch count.txt')
+              1454 STORE_NAME              58 (switchcount)
+   
+   146        1456 PUSH_NULL
+              1458 LOAD_NAME               29 (open)
+              1460 LOAD_NAME               58 (switchcount)
+              1462 LOAD_CONST              12 ('r')
               1464 PRECALL                  2
               1468 CALL                     2
-              1478 POP_TOP
-              1480 JUMP_FORWARD            11 (to 1504)
-           >> 1482 PUSH_EXC_INFO
-              1484 WITH_EXCEPT_START
-              1486 POP_JUMP_FORWARD_IF_TRUE     4 (to 1496)
-              1488 RERAISE                  2
-           >> 1490 COPY                     3
-              1492 POP_EXCEPT
-              1494 RERAISE                  1
-           >> 1496 POP_TOP
-              1498 POP_EXCEPT
-              1500 POP_TOP
-              1502 POP_TOP
-   
-   145     >> 1504 LOAD_CONST              27 ('Switch count.txt')
-              1506 STORE_NAME              61 (switchcount)
-   
-   147        1508 PUSH_NULL
-              1510 LOAD_NAME               29 (open)
-              1512 LOAD_NAME               61 (switchcount)
-              1514 LOAD_CONST              12 ('r')
-              1516 PRECALL                  2
-              1520 CALL                     2
-              1530 BEFORE_WITH
-              1532 STORE_NAME              30 (f)
-   
-   148        1534 LOAD_NAME               30 (f)
-              1536 LOAD_METHOD             31 (readline)
-              1558 PRECALL                  0
-              1562 CALL                     0
-              1572 STORE_NAME              32 (first_line)
+              1478 BEFORE_WITH
+              1480 STORE_NAME              30 (f)
    
-   149        1574 LOAD_NAME               32 (first_line)
-              1576 LOAD_METHOD             33 (split)
+   147        1482 LOAD_NAME               30 (f)
+              1484 LOAD_METHOD             31 (readline)
+              1506 PRECALL                  0
+              1510 CALL                     0
+              1520 STORE_NAME              32 (first_line)
+   
+   148        1522 LOAD_NAME               32 (first_line)
+              1524 LOAD_METHOD             33 (split)
+              1546 PRECALL                  0
+              1550 CALL                     0
+              1560 STORE_NAME              34 (words)
+   
+   149        1562 LOAD_CONST               1 (None)
+              1564 STORE_NAME              59 (scount)
+   
+   150        1566 LOAD_NAME               34 (words)
+              1568 GET_ITER
+           >> 1570 FOR_ITER                33 (to 1638)
+              1572 STORE_NAME              35 (word)
+   
+   151        1574 LOAD_NAME               35 (word)
+              1576 LOAD_METHOD             36 (isdigit)
               1598 PRECALL                  0
               1602 CALL                     0
-              1612 STORE_NAME              34 (words)
-   
-   150        1614 LOAD_CONST               1 (None)
-              1616 STORE_NAME              62 (scount)
+              1612 POP_JUMP_FORWARD_IF_FALSE    11 (to 1636)
    
-   151        1618 LOAD_NAME               34 (words)
-              1620 GET_ITER
-           >> 1622 FOR_ITER                33 (to 1690)
-              1624 STORE_NAME              35 (word)
-   
-   152        1626 LOAD_NAME               35 (word)
-              1628 LOAD_METHOD             36 (isdigit)
-              1650 PRECALL                  0
-              1654 CALL                     0
-              1664 POP_JUMP_FORWARD_IF_FALSE    11 (to 1688)
-   
-   153        1666 PUSH_NULL
-              1668 LOAD_NAME               37 (int)
-              1670 LOAD_NAME               35 (word)
-              1672 PRECALL                  1
-              1676 CALL                     1
-              1686 STORE_NAME              62 (scount)
-           >> 1688 JUMP_BACKWARD           34 (to 1622)
-   
-   151     >> 1690 NOP
-   
-   147        1692 LOAD_CONST               1 (None)
-              1694 LOAD_CONST               1 (None)
-              1696 LOAD_CONST               1 (None)
-              1698 PRECALL                  2
-              1702 CALL                     2
-              1712 POP_TOP
-              1714 JUMP_FORWARD            11 (to 1738)
-           >> 1716 PUSH_EXC_INFO
-              1718 WITH_EXCEPT_START
-              1720 POP_JUMP_FORWARD_IF_TRUE     4 (to 1730)
-              1722 RERAISE                  2
-           >> 1724 COPY                     3
-              1726 POP_EXCEPT
-              1728 RERAISE                  1
-           >> 1730 POP_TOP
-              1732 POP_EXCEPT
-              1734 POP_TOP
-              1736 POP_TOP
-   
-   155     >> 1738 LOAD_CONST               0 (0)
-              1740 LOAD_CONST               1 (None)
-              1742 IMPORT_NAME             18 (spwf)
-              1744 STORE_NAME              18 (spwf)
-   
-   156        1746 LOAD_CONST              28 (<code object main, file "D:\Task Development\Stimuli\Task\Task.py", line 156>)
-              1748 MAKE_FUNCTION            0
-              1750 STORE_NAME              63 (main)
-   
-   327        1752 PUSH_NULL
-              1754 LOAD_NAME               63 (main)
-              1756 PRECALL                  0
-              1760 CALL                     0
-              1770 POP_TOP
-              1772 LOAD_CONST               1 (None)
-              1774 RETURN_VALUE
-   
-   330     >> 1776 LOAD_CONST               0 (0)
-              1778 LOAD_CONST               1 (None)
-              1780 IMPORT_NAME              1 (tkinter)
-              1782 STORE_NAME               2 (tk)
-   
-   331        1784 LOAD_CONST              29 ('Your device is not connected to the internet, please connect to the internet to continue the task\n\nThe task must ensure that you have the correct files installed, which requires an active internet connection')
-              1786 STORE_NAME              64 (errortext)
-   
-   335        1788 LOAD_CONST              30 (('Helvetica', 18))
-              1790 STORE_NAME              65 (fontsize)
-   
-   336        1792 LOAD_CONST              31 (('Helvetica', 22))
-              1794 STORE_NAME              66 (fontsize1)
-   
-   337        1796 LOAD_CONST              32 (('Helvetica', 12))
-              1798 STORE_NAME              67 (fontsize2)
-   
-   340        1800 LOAD_CONST               0 (0)
-              1802 LOAD_CONST               5 (('simpledialog', 'messagebox'))
-              1804 IMPORT_NAME              1 (tkinter)
-              1806 IMPORT_FROM             10 (simpledialog)
-              1808 STORE_NAME              10 (simpledialog)
-              1810 IMPORT_FROM             11 (messagebox)
-              1812 STORE_NAME              11 (messagebox)
-              1814 POP_TOP
-   
-   342        1816 PUSH_NULL
-              1818 LOAD_NAME               11 (messagebox)
-              1820 LOAD_ATTR               68 (showerror)
-              1830 LOAD_CONST              33 ('Error')
-              1832 LOAD_NAME               64 (errortext)
-              1834 PRECALL                  2
-              1838 CALL                     2
-              1848 POP_TOP
-              1850 LOAD_CONST               1 (None)
-              1852 RETURN_VALUE
+   152        1614 PUSH_NULL
+              1616 LOAD_NAME               37 (int)
+              1618 LOAD_NAME               35 (word)
+              1620 PRECALL                  1
+              1624 CALL                     1
+              1634 STORE_NAME              59 (scount)
+           >> 1636 JUMP_BACKWARD           34 (to 1570)
+   
+   150     >> 1638 NOP
+   
+   146        1640 LOAD_CONST               1 (None)
+              1642 LOAD_CONST               1 (None)
+              1644 LOAD_CONST               1 (None)
+              1646 PRECALL                  2
+              1650 CALL                     2
+              1660 POP_TOP
+              1662 JUMP_FORWARD            11 (to 1686)
+           >> 1664 PUSH_EXC_INFO
+              1666 WITH_EXCEPT_START
+              1668 POP_JUMP_FORWARD_IF_TRUE     4 (to 1678)
+              1670 RERAISE                  2
+           >> 1672 COPY                     3
+              1674 POP_EXCEPT
+              1676 RERAISE                  1
+           >> 1678 POP_TOP
+              1680 POP_EXCEPT
+              1682 POP_TOP
+              1684 POP_TOP
+   
+   154     >> 1686 LOAD_CONST               0 (0)
+              1688 LOAD_CONST               1 (None)
+              1690 IMPORT_NAME             18 (spwf)
+              1692 STORE_NAME              18 (spwf)
+   
+   156        1694 LOAD_CONST              27 (<code object main, file "H:\Task Development\Stimuli\Task\Task.py", line 156>)
+              1696 MAKE_FUNCTION            0
+              1698 STORE_NAME              60 (main)
+   
+   350        1700 PUSH_NULL
+              1702 LOAD_NAME               60 (main)
+              1704 PRECALL                  0
+              1708 CALL                     0
+              1718 POP_TOP
+              1720 LOAD_CONST               1 (None)
+              1722 RETURN_VALUE
+   
+   353     >> 1724 LOAD_CONST               0 (0)
+              1726 LOAD_CONST               1 (None)
+              1728 IMPORT_NAME              1 (tkinter)
+              1730 STORE_NAME               2 (tk)
+   
+   354        1732 LOAD_CONST              28 ('Your device is not connected to the internet, please connect to the internet to continue the task\n\nThe task must ensure that you have the correct files installed, which requires an active internet connection')
+              1734 STORE_NAME              61 (errortext)
+   
+   356        1736 LOAD_CONST              29 (('Helvetica', 18))
+              1738 STORE_NAME              62 (fontsize)
+   
+   357        1740 LOAD_CONST              30 (('Helvetica', 22))
+              1742 STORE_NAME              63 (fontsize1)
+   
+   358        1744 LOAD_CONST              31 (('Helvetica', 12))
+              1746 STORE_NAME              64 (fontsize2)
+   
+   360        1748 LOAD_CONST               0 (0)
+              1750 LOAD_CONST               5 (('simpledialog', 'messagebox'))
+              1752 IMPORT_NAME              1 (tkinter)
+              1754 IMPORT_FROM             10 (simpledialog)
+              1756 STORE_NAME              10 (simpledialog)
+              1758 IMPORT_FROM             11 (messagebox)
+              1760 STORE_NAME              11 (messagebox)
+              1762 POP_TOP
+   
+   362        1764 PUSH_NULL
+              1766 LOAD_NAME               11 (messagebox)
+              1768 LOAD_ATTR               65 (showerror)
+              1778 LOAD_CONST              32 ('Error')
+              1780 LOAD_NAME               61 (errortext)
+              1782 PRECALL                  2
+              1786 CALL                     2
+              1796 POP_TOP
+              1798 LOAD_CONST               1 (None)
+              1800 RETURN_VALUE
    ExceptionTable:
-     510 to 666 -> 694 [1] lasti
-     694 to 700 -> 702 [3] lasti
-     708 to 708 -> 702 [3] lasti
-     728 to 788 -> 792 [0]
-     792 to 822 -> 830 [1] lasti
-     828 to 828 -> 830 [1] lasti
-     1064 to 1220 -> 1248 [1] lasti
-     1248 to 1254 -> 1256 [3] lasti
-     1262 to 1262 -> 1256 [3] lasti
-     1298 to 1454 -> 1482 [1] lasti
-     1482 to 1488 -> 1490 [3] lasti
-     1496 to 1496 -> 1490 [3] lasti
-     1532 to 1688 -> 1716 [1] lasti
-     1716 to 1722 -> 1724 [3] lasti
-     1730 to 1730 -> 1724 [3] lasti
+     502 to 658 -> 686 [1] lasti
+     686 to 692 -> 694 [3] lasti
+     700 to 700 -> 694 [3] lasti
+     720 to 780 -> 784 [0]
+     784 to 814 -> 822 [1] lasti
+     820 to 820 -> 822 [1] lasti
+     1012 to 1168 -> 1196 [1] lasti
+     1196 to 1202 -> 1204 [3] lasti
+     1210 to 1210 -> 1204 [3] lasti
+     1246 to 1402 -> 1430 [1] lasti
+     1430 to 1436 -> 1438 [3] lasti
+     1444 to 1444 -> 1438 [3] lasti
+     1480 to 1636 -> 1664 [1] lasti
+     1664 to 1670 -> 1672 [3] lasti
+     1678 to 1678 -> 1672 [3] lasti
    consts
       0
       None
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 5
@@ -784,47 +763,47 @@
             80
             True
             False
          names      ('socket', 'create_connection', 'OSError')
          varnames   ('websites', 'website')
          freevars   ()
          cellvars   ()
-         filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+         filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
          name       'is_connected'
          firstlineno 6
          lnotab 0x02010801080102012c010801120104ff0802
       True
       'participant number.txt'
       ('simpledialog', 'messagebox')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-          29           0 RESUME                   0
+          30           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PinSystem')
                        8 STORE_NAME               2 (__qualname__)
          
-          30          10 LOAD_CONST               1 (<code object __init__, file "D:\Task Development\Stimuli\Task\Task.py", line 30>)
+          31          10 LOAD_CONST               1 (<code object __init__, file "H:\Task Development\Stimuli\Task\Task.py", line 31>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          57          16 LOAD_CONST               2 (<code object submit_pin, file "D:\Task Development\Stimuli\Task\Task.py", line 57>)
+          60          16 LOAD_CONST               2 (<code object submit_pin, file "H:\Task Development\Stimuli\Task\Task.py", line 60>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (submit_pin)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'PinSystem'
             code
                argcount  : 2
-               nlocals   : 9
+               nlocals   : 11
                stacksize : 6
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c006a000000000000000000a0
                   0100000000000000000000000000000000000000006401a6010000ab0100
                   0000000000000001007c006a000000000000000000a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000007d027c
@@ -842,290 +821,324 @@
                   000000000000000100740f000000000000000000006a0b00000000000000
                   007c006a000000000000000000a6010000ab0100000000000000007c005f
                   0c00000000000000007c006a0c0000000000000000a00a00000000000000
                   00000000000000000000000000a6000000ab000000000000000000010074
                   0f000000000000000000006a0d00000000000000007c006a000000000000
                   00000064087c006a0e0000000000000000ac09a6030000ab030000000000
                   0000007c005f0f00000000000000007c006a0f0000000000000000a00a00
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  000000010069007c005f1000000000000000007423000000000000000000
-                  00640aa6010000ab01000000000000000035007d06742500000000000000
-                  0000006a1300000000000000007c06a6010000ab0100000000000000007d
-                  077c0744005d187d087c08640b190000000000000000007c006a10000000
-                  00000000007c08640c190000000000000000003c0000008c190900640064
-                  006400a6020000ab02000000000000000001006400530023003100730477
-                  02780359007701010059000100010064005300
-                30           0 RESUME                   0
+                  00000000000000000000000000000000000000640aac0ba6010000ab0100
+                  00000000000000010069007c005f10000000000000000074220000000000
+                  00000000006a120000000000000000a01300000000000000000000000000
+                  000000000000007422000000000000000000006a120000000000000000a0
+                  140000000000000000000000000000000000000000742a00000000000000
+                  000000a6010000ab010000000000000000a6010000ab0100000000000000
+                  007d067422000000000000000000006a120000000000000000a016000000
+                  00000000000000000000000000000000007c06640ca6020000ab02000000
+                  00000000007d07742f000000000000000000007c07a6010000ab01000000
+                  000000000035007d087431000000000000000000006a1900000000000000
+                  007c08a6010000ab0100000000000000007d097c0944005d187d0a7c0a64
+                  0d190000000000000000007c006a1000000000000000007c0a640e190000
+                  000000000000003c0000008c190900640064006400a6020000ab02000000
+                  000000000001006400530023003100730477027803590077010100590001
+                  00010064005300
+                31           0 RESUME                   0
                
-                31           2 LOAD_FAST                1 (master)
+                32           2 LOAD_FAST                1 (master)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (master)
                
-                32          16 LOAD_FAST                0 (self)
+                33          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                0 (master)
                             28 LOAD_METHOD              1 (title)
                             50 LOAD_CONST               1 ('PIN Entry')
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                
-                34          68 LOAD_FAST                0 (self)
+                35          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                0 (master)
                             80 LOAD_METHOD              2 (winfo_screenwidth)
                            102 PRECALL                  0
                            106 CALL                     0
                            116 STORE_FAST               2 (screen_width)
                
-                35         118 LOAD_FAST                0 (self)
+                36         118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                0 (master)
                            130 LOAD_METHOD              3 (winfo_screenheight)
                            152 PRECALL                  0
                            156 CALL                     0
                            166 STORE_FAST               3 (screen_height)
                
-                37         168 LOAD_GLOBAL              9 (NULL + int)
+                38         168 LOAD_GLOBAL              9 (NULL + int)
                            180 LOAD_FAST                2 (screen_width)
                            182 LOAD_CONST               2 (2)
                            184 BINARY_OP               11 (/)
                            188 LOAD_CONST               3 (300.0)
                            190 BINARY_OP               10 (-)
                            194 PRECALL                  1
                            198 CALL                     1
                            208 STORE_FAST               4 (x)
                
-                38         210 LOAD_GLOBAL              9 (NULL + int)
+                39         210 LOAD_GLOBAL              9 (NULL + int)
                            222 LOAD_FAST                3 (screen_height)
                            224 LOAD_CONST               2 (2)
                            226 BINARY_OP               11 (/)
                            230 LOAD_CONST               4 (75.0)
                            232 BINARY_OP               10 (-)
                            236 PRECALL                  1
                            240 CALL                     1
                            250 STORE_FAST               5 (y)
                
-                40         252 LOAD_FAST                0 (self)
+                41         252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                0 (master)
                            264 LOAD_METHOD              5 (geometry)
                            286 LOAD_CONST               5 ('600x150+{}+{}')
                            288 LOAD_METHOD              6 (format)
                            310 LOAD_FAST                4 (x)
                            312 LOAD_FAST                5 (y)
                            314 PRECALL                  2
                            318 CALL                     2
                            328 PRECALL                  1
                            332 CALL                     1
                            342 POP_TOP
                
-                42         344 LOAD_GLOBAL             15 (NULL + tk)
+                43         344 LOAD_GLOBAL             15 (NULL + tk)
                            356 LOAD_ATTR                8 (Label)
                            366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR                0 (master)
                            378 LOAD_CONST               6 ('Welcome to the task\n\nTo begin, please enter your PIN. This will have been sent to you via email.\n\nEnter your PIN:')
                            380 KW_NAMES                 7
                            382 PRECALL                  2
                            386 CALL                     2
                            396 LOAD_FAST                0 (self)
                            398 STORE_ATTR               9 (pin_label)
                
-                43         408 LOAD_FAST                0 (self)
+                44         408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR                9 (pin_label)
                            420 LOAD_METHOD             10 (pack)
                            442 PRECALL                  0
                            446 CALL                     0
                            456 POP_TOP
                
-                45         458 LOAD_GLOBAL             15 (NULL + tk)
+                46         458 LOAD_GLOBAL             15 (NULL + tk)
                            470 LOAD_ATTR               11 (Entry)
                            480 LOAD_FAST                0 (self)
                            482 LOAD_ATTR                0 (master)
                            492 PRECALL                  1
                            496 CALL                     1
                            506 LOAD_FAST                0 (self)
                            508 STORE_ATTR              12 (pin_entry)
                
-                46         518 LOAD_FAST                0 (self)
+                47         518 LOAD_FAST                0 (self)
                            520 LOAD_ATTR               12 (pin_entry)
                            530 LOAD_METHOD             10 (pack)
                            552 PRECALL                  0
                            556 CALL                     0
                            566 POP_TOP
                
-                48         568 LOAD_GLOBAL             15 (NULL + tk)
+                49         568 LOAD_GLOBAL             15 (NULL + tk)
                            580 LOAD_ATTR               13 (Button)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                0 (master)
                            602 LOAD_CONST               8 ('Submit')
                            604 LOAD_FAST                0 (self)
                            606 LOAD_ATTR               14 (submit_pin)
                            616 KW_NAMES                 9
                            618 PRECALL                  3
                            622 CALL                     3
                            632 LOAD_FAST                0 (self)
                            634 STORE_ATTR              15 (submit_button)
                
-                49         644 LOAD_FAST                0 (self)
+                50         644 LOAD_FAST                0 (self)
                            646 LOAD_ATTR               15 (submit_button)
                            656 LOAD_METHOD             10 (pack)
-                           678 PRECALL                  0
-                           682 CALL                     0
-                           692 POP_TOP
-               
-                51         694 BUILD_MAP                0
-                           696 LOAD_FAST                0 (self)
-                           698 STORE_ATTR              16 (pins)
-               
-                52         708 LOAD_GLOBAL             35 (NULL + open)
-                           720 LOAD_CONST              10 ('pins.csv')
-                           722 PRECALL                  1
-                           726 CALL                     1
-                           736 BEFORE_WITH
-                           738 STORE_FAST               6 (f)
-               
-                53         740 LOAD_GLOBAL             37 (NULL + csv)
-                           752 LOAD_ATTR               19 (reader)
-                           762 LOAD_FAST                6 (f)
-                           764 PRECALL                  1
-                           768 CALL                     1
-                           778 STORE_FAST               7 (reader)
-               
-                54         780 LOAD_FAST                7 (reader)
-                           782 GET_ITER
-                       >>  784 FOR_ITER                24 (to 834)
-                           786 STORE_FAST               8 (row)
-               
-                55         788 LOAD_FAST                8 (row)
-                           790 LOAD_CONST              11 (1)
-                           792 BINARY_SUBSCR
-                           802 LOAD_FAST                0 (self)
-                           804 LOAD_ATTR               16 (pins)
-                           814 LOAD_FAST                8 (row)
-                           816 LOAD_CONST              12 (0)
-                           818 BINARY_SUBSCR
-                           828 STORE_SUBSCR
-                           832 JUMP_BACKWARD           25 (to 784)
-               
-                54     >>  834 NOP
-               
-                52         836 LOAD_CONST               0 (None)
-                           838 LOAD_CONST               0 (None)
-                           840 LOAD_CONST               0 (None)
-                           842 PRECALL                  2
-                           846 CALL                     2
-                           856 POP_TOP
-                           858 LOAD_CONST               0 (None)
-                           860 RETURN_VALUE
-                       >>  862 PUSH_EXC_INFO
-                           864 WITH_EXCEPT_START
-                           866 POP_JUMP_FORWARD_IF_TRUE     4 (to 876)
-                           868 RERAISE                  2
-                       >>  870 COPY                     3
-                           872 POP_EXCEPT
-                           874 RERAISE                  1
-                       >>  876 POP_TOP
-                           878 POP_EXCEPT
-                           880 POP_TOP
-                           882 POP_TOP
-                           884 LOAD_CONST               0 (None)
-                           886 RETURN_VALUE
+                           678 LOAD_CONST              10 (15)
+                           680 KW_NAMES                11
+                           682 PRECALL                  1
+                           686 CALL                     1
+                           696 POP_TOP
+               
+                52         698 BUILD_MAP                0
+                           700 LOAD_FAST                0 (self)
+                           702 STORE_ATTR              16 (pins)
+               
+                53         712 LOAD_GLOBAL             34 (os)
+                           724 LOAD_ATTR               18 (path)
+                           734 LOAD_METHOD             19 (dirname)
+                           756 LOAD_GLOBAL             34 (os)
+                           768 LOAD_ATTR               18 (path)
+                           778 LOAD_METHOD             20 (abspath)
+                           800 LOAD_GLOBAL             42 (__file__)
+                           812 PRECALL                  1
+                           816 CALL                     1
+                           826 PRECALL                  1
+                           830 CALL                     1
+                           840 STORE_FAST               6 (script_dir)
+               
+                54         842 LOAD_GLOBAL             34 (os)
+                           854 LOAD_ATTR               18 (path)
+                           864 LOAD_METHOD             22 (join)
+                           886 LOAD_FAST                6 (script_dir)
+                           888 LOAD_CONST              12 ('pins.csv')
+                           890 PRECALL                  2
+                           894 CALL                     2
+                           904 STORE_FAST               7 (csv_path)
+               
+                55         906 LOAD_GLOBAL             47 (NULL + open)
+                           918 LOAD_FAST                7 (csv_path)
+                           920 PRECALL                  1
+                           924 CALL                     1
+                           934 BEFORE_WITH
+                           936 STORE_FAST               8 (f)
+               
+                56         938 LOAD_GLOBAL             49 (NULL + csv)
+                           950 LOAD_ATTR               25 (reader)
+                           960 LOAD_FAST                8 (f)
+                           962 PRECALL                  1
+                           966 CALL                     1
+                           976 STORE_FAST               9 (reader)
+               
+                57         978 LOAD_FAST                9 (reader)
+                           980 GET_ITER
+                       >>  982 FOR_ITER                24 (to 1032)
+                           984 STORE_FAST              10 (row)
+               
+                58         986 LOAD_FAST               10 (row)
+                           988 LOAD_CONST              13 (1)
+                           990 BINARY_SUBSCR
+                          1000 LOAD_FAST                0 (self)
+                          1002 LOAD_ATTR               16 (pins)
+                          1012 LOAD_FAST               10 (row)
+                          1014 LOAD_CONST              14 (0)
+                          1016 BINARY_SUBSCR
+                          1026 STORE_SUBSCR
+                          1030 JUMP_BACKWARD           25 (to 982)
+               
+                57     >> 1032 NOP
+               
+                55        1034 LOAD_CONST               0 (None)
+                          1036 LOAD_CONST               0 (None)
+                          1038 LOAD_CONST               0 (None)
+                          1040 PRECALL                  2
+                          1044 CALL                     2
+                          1054 POP_TOP
+                          1056 LOAD_CONST               0 (None)
+                          1058 RETURN_VALUE
+                       >> 1060 PUSH_EXC_INFO
+                          1062 WITH_EXCEPT_START
+                          1064 POP_JUMP_FORWARD_IF_TRUE     4 (to 1074)
+                          1066 RERAISE                  2
+                       >> 1068 COPY                     3
+                          1070 POP_EXCEPT
+                          1072 RERAISE                  1
+                       >> 1074 POP_TOP
+                          1076 POP_EXCEPT
+                          1078 POP_TOP
+                          1080 POP_TOP
+                          1082 LOAD_CONST               0 (None)
+                          1084 RETURN_VALUE
                ExceptionTable:
-                 738 to 832 -> 862 [1] lasti
-                 862 to 868 -> 870 [3] lasti
-                 876 to 876 -> 870 [3] lasti
+                 936 to 1030 -> 1060 [1] lasti
+                 1060 to 1066 -> 1068 [3] lasti
+                 1074 to 1074 -> 1068 [3] lasti
                consts
                   None
                   'PIN Entry'
                   2
                   300.0
                   75.0
                   '600x150+{}+{}'
                   'Welcome to the task\n\nTo begin, please enter your PIN. This will have been sent to you via email.\n\nEnter your PIN:'
                   ('text',)
                   'Submit'
                   ('text', 'command')
+                  15
+                  ('pady',)
                   'pins.csv'
                   1
                   0
-               names      ('master', 'title', 'winfo_screenwidth', 'winfo_screenheight', 'int', 'geometry', 'format', 'tk', 'Label', 'pin_label', 'pack', 'Entry', 'pin_entry', 'Button', 'submit_pin', 'submit_button', 'pins', 'open', 'csv', 'reader')
-               varnames   ('self', 'master', 'screen_width', 'screen_height', 'x', 'y', 'f', 'reader', 'row')
+               names      ('master', 'title', 'winfo_screenwidth', 'winfo_screenheight', 'int', 'geometry', 'format', 'tk', 'Label', 'pin_label', 'pack', 'Entry', 'pin_entry', 'Button', 'submit_pin', 'submit_button', 'pins', 'os', 'path', 'dirname', 'abspath', '__file__', 'join', 'open', 'csv', 'reader')
+               varnames   ('self', 'master', 'screen_width', 'screen_height', 'x', 'y', 'script_dir', 'csv_path', 'f', 'reader', 'row')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       '__init__'
-               firstlineno 30
+               firstlineno 31
                lnotab
-                  0x02010e013402320132022a012a025c02400132023c0132024c0132020e
-                  012001280108012eff02fe
+                  0x02010e013402320132022a012a025c02400132023c0132024c0136020e
+                  01820140012001280108012eff02fe
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d017c017c006a0200
                   000000000000007600726a7c006a0200000000000000007c011900000000
                   00000000007d0264017c029b0064029d037d037407000000000000000000
                   0064036404a6020000ab02000000000000000035007d047c04a004000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
-                  0000000100740a00000000000000000000a0060000000000000000000000
+                  00000001007c006a050000000000000000a0060000000000000000000000
                   000000000000000000a6000000ab00000000000000000001006400640064
                   00a6020000ab02000000000000000001006e0b2300310073047702780359
                   00770101005900010001006e0264057d03740e000000000000000000006a
                   080000000000000000a00900000000000000000000000000000000000000
                   0064067c03a6020000ab020000000000000000010064005300
-                57           0 RESUME                   0
+                60           0 RESUME                   0
                
-                58           2 LOAD_FAST                0 (self)
+                61           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (pin_entry)
                             14 LOAD_METHOD              1 (get)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 STORE_FAST               1 (pin)
                
-                60          52 LOAD_FAST                1 (pin)
+                63          52 LOAD_FAST                1 (pin)
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (pins)
                             66 CONTAINS_OP              0
                             68 POP_JUMP_FORWARD_IF_FALSE   106 (to 282)
                
-                61          70 LOAD_FAST                0 (self)
+                64          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (pins)
                             82 LOAD_FAST                1 (pin)
                             84 BINARY_SUBSCR
                             94 STORE_FAST               2 (participant_num)
                
-                62          96 LOAD_CONST               1 ('Correct PIN\n\nYour participant number is ')
+                65          96 LOAD_CONST               1 ('Correct PIN\n\nYour participant number is ')
                             98 LOAD_FAST                2 (participant_num)
                            100 FORMAT_VALUE             0
                            102 LOAD_CONST               2 ('.\n\nThe task will now load')
                            104 BUILD_STRING             3
                            106 STORE_FAST               3 (message)
                
-                64         108 LOAD_GLOBAL              7 (NULL + open)
+                66         108 LOAD_GLOBAL              7 (NULL + open)
                            120 LOAD_CONST               3 ('participant number.txt')
                            122 LOAD_CONST               4 ('w')
                            124 PRECALL                  2
                            128 CALL                     2
                            138 BEFORE_WITH
                            140 STORE_FAST               4 (outfile)
                
-                65         142 LOAD_FAST                4 (outfile)
+                67         142 LOAD_FAST                4 (outfile)
                            144 LOAD_METHOD              4 (write)
                            166 LOAD_FAST                2 (participant_num)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 POP_TOP
                
-                66         184 LOAD_GLOBAL             10 (root)
-                           196 LOAD_METHOD              6 (quit)
+                68         184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                5 (master)
+                           196 LOAD_METHOD              6 (destroy)
                            218 PRECALL                  0
                            222 CALL                     0
                            232 POP_TOP
                
-                64         234 LOAD_CONST               0 (None)
+                66         234 LOAD_CONST               0 (None)
                            236 LOAD_CONST               0 (None)
                            238 LOAD_CONST               0 (None)
                            240 PRECALL                  2
                            244 CALL                     2
                            254 POP_TOP
                            256 JUMP_FORWARD            11 (to 280)
                        >>  258 PUSH_EXC_INFO
@@ -1137,18 +1150,18 @@
                            270 RERAISE                  1
                        >>  272 POP_TOP
                            274 POP_EXCEPT
                            276 POP_TOP
                            278 POP_TOP
                        >>  280 JUMP_FORWARD             2 (to 286)
                
-                68     >>  282 LOAD_CONST               5 ('Invalid PIN.')
+                70     >>  282 LOAD_CONST               5 ('Invalid PIN.')
                            284 STORE_FAST               3 (message)
                
-                70     >>  286 LOAD_GLOBAL             14 (tk)
+                72     >>  286 LOAD_GLOBAL             14 (tk)
                            298 LOAD_ATTR                8 (messagebox)
                            308 LOAD_METHOD              9 (showinfo)
                            330 LOAD_CONST               6 ('Result')
                            332 LOAD_FAST                3 (message)
                            334 PRECALL                  2
                            338 CALL                     2
                            348 POP_TOP
@@ -1162,1333 +1175,1587 @@
                   None
                   'Correct PIN\n\nYour participant number is '
                   '.\n\nThe task will now load'
                   'participant number.txt'
                   'w'
                   'Invalid PIN.'
                   'Result'
-               names      ('pin_entry', 'get', 'pins', 'open', 'write', 'root', 'quit', 'tk', 'messagebox', 'showinfo')
+               names      ('pin_entry', 'get', 'pins', 'open', 'write', 'master', 'destroy', 'tk', 'messagebox', 'showinfo')
                varnames   ('self', 'pin', 'participant_num', 'message', 'outfile')
                freevars   ()
                cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       'submit_pin'
-               firstlineno 57
-               lnotab 0x0201320212011a010c0222012a0132fe30040402
+               firstlineno 60
+               lnotab 0x0201320212011a010c0122012a0132fe30040402
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'submit_pin')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+         filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
          name       'PinSystem'
-         firstlineno 29
-         lnotab 0x0a01061b
+         firstlineno 30
+         lnotab 0x0a01061d
       'PinSystem'
       '__main__'
       'Welcome to the task! Thank you for your interest in the study.\n\nYou are participant number '
       '.\n\nThe task is now loading, it may take a short while to load.'
       'PATH'
       'r'
       'Participant '
       "Created folder '"
       "'"
       ''
       'Suffix.bat'
       ('capture_output', 'text')
-      'cputask.py'
       ('*',)
       ('Image', 'ImageTk')
       ('datetime',)
       ('filedialog',)
       'Dependency Installation.py'
       'RT count.txt'
       'N-Back count.txt'
       'Switch count.txt'
       code
          argcount  : 0
-         nlocals   : 34
+         nlocals   : 51
          stacksize : 7
          flags     : 3
          code
-            0x8722872387248725872697007401000000000000000000006a01000000
-            0000000000a6000000ab0000000000000000007d007c00a0020000000000
-            000000000000000000000000000000a6000000ab0000000000000000007d
-            017c00a0030000000000000000000000000000000000000000a6000000ab
-            0000000000000000007d0264017c029b0064027c019b009d047d037c0164
-            037a0200007d0464048a2364058a227409000000000000000000006a0400
-            00000000000000740a0000000000000000000064067a000000a6010000ab
-            01000000000000000090057232740c000000000000000000006a07000000
-            00000000007d05740c000000000000000000006a0800000000000000007d
-            0688246601640784087d07640884008a24882288236602640984087d0864
-            0a7d09640b7d0a640c7d0b7c00a009000000000000000000000000000000
-            0000000000640d640ea6020000ab02000000000000000001007401000000
-            000000000000006a0a00000000000000007c00640f7c09ac10a6030000ab
-            0300000000000000008a25882588266602641184088a268925a00b000000
-            00000000000000000000000000000000007400000000000000000000006a
-            0c0000000000000000641264046413ac14a6040000ab0400000000000000
-            0001007401000000000000000000006a0d00000000000000007c00a60100
-            00ab0100000000000000007d0c7c0ca00b00000000000000000000000000
-            000000000000007400000000000000000000006a0c000000000000000074
-            00000000000000000000006a0e0000000000000000ac15a6020000ab0200
-            0000000000000001007401000000000000000000006a0a00000000000000
-            007c0c64167c0aac10a6030000ab0300000000000000007d0d7c0da00b00
-            000000000000000000000000000000000000007c04ac17a6010000ab0100
-            0000000000000001007401000000000000000000006a0d00000000000000
-            007c00a6010000ab0100000000000000007d0e7c0ea00b00000000000000
-            000000000000000000000000007400000000000000000000006a0c000000
-            00000000007400000000000000000000006a0e0000000000000000ac15a6
-            020000ab02000000000000000001007401000000000000000000006a0a00
-            000000000000007c0c64187c09ac10a6030000ab0300000000000000007d
-            0f7c0fa00b00000000000000000000000000000000000000007c04ac17a6
-            010000ab01000000000000000001007401000000000000000000006a0d00
-            000000000000007c00a6010000ab0100000000000000007d107c10a00b00
-            000000000000000000000000000000000000007400000000000000000000
-            006a0c00000000000000006419641a641bac14a6040000ab040000000000
-            0000000100882288236602641c84087d117401000000000000000000006a
-            0f00000000000000007c10641d7c117c09641bac1ea6050000ab05000000
-            00000000007d127c12a00b00000000000000000000000000000000000000
-            007400000000000000000000006a0c0000000000000000641aac1fa60200
-            00ab020000000000000000010074200000000000000000000064206b0200
-            000000720c64217420000000000000000000009b0064229d037d136e0b64
-            217420000000000000000000009b0064239d037d13740100000000000000
-            0000006a0a00000000000000007c107c137c0bac10a6030000ab03000000
-            00000000007d147c14a00b00000000000000000000000000000000000000
-            007400000000000000000000006a0c0000000000000000641a641bac24a6
-            030000ab03000000000000000001007401000000000000000000006a0d00
-            000000000000007c00a6010000ab0100000000000000007d157c15a00b00
-            000000000000000000000000000000000000007400000000000000000000
-            006a0c00000000000000006419641a641bac14a6040000ab040000000000
-            00000001007401000000000000000000006a0d00000000000000007c00a6
-            010000ab0100000000000000007d167c16a00b0000000000000000000000
-            0000000000000000007400000000000000000000006a0c00000000000000
-            006419641a641bac14a6040000ab04000000000000000001007401000000
-            000000000000006a0f00000000000000007c1664257c087c09641bac1ea6
-            050000ab0500000000000000007d177c17a00b0000000000000000000000
-            0000000000000000007400000000000000000000006a0c00000000000000
-            00641aac1fa6020000ab0200000000000000000100742200000000000000
-            00000064206b0200000000720c64217422000000000000000000009b0064
-            229d037d136e0b64217422000000000000000000009b0064239d037d1374
-            01000000000000000000006a0a00000000000000007c167c137c0bac10a6
-            030000ab0300000000000000007d187c18a00b0000000000000000000000
-            0000000000000000007400000000000000000000006a0c00000000000000
-            00641aac1fa6020000ab0200000000000000000100882288236602642684
-            087d197401000000000000000000006a0d00000000000000007c00a60100
-            00ab0100000000000000007d1a7c1aa00b00000000000000000000000000
-            000000000000007400000000000000000000006a0c000000000000000064
-            196404641bac14a6040000ab040000000000000000010074010000000000
-            00000000006a0f00000000000000007c1a64277c197c09641bac1ea60500
-            00ab0500000000000000007d1b7c1ba00b00000000000000000000000000
-            000000000000007400000000000000000000006a0c000000000000000064
-            1aac1fa6020000ab02000000000000000001007424000000000000000000
-            0064206b0200000000720c64217424000000000000000000009b0064229d
-            037d136e0b64217424000000000000000000009b0064239d037d13740100
-            0000000000000000006a0a00000000000000007c1a7c137c0bac10a60300
-            00ab0300000000000000007d1c7c1ca00b00000000000000000000000000
-            000000000000007400000000000000000000006a0c000000000000000064
-            1a641bac24a6030000ab0300000000000000000100740100000000000000
-            0000006a0d00000000000000007c00a6010000ab0100000000000000007d
-            1d7c1da00b00000000000000000000000000000000000000007400000000
-            000000000000006a130000000000000000641964126428ac14a6040000ab
-            04000000000000000001007401000000000000000000006a0f0000000000
-            0000007c1d64297c077c09ac2aa6040000ab0400000000000000007d1e7c
-            1ea00b000000000000000000000000000000000000000074000000000000
-            00000000006a1400000000000000006404ac1fa6020000ab020000000000
-            0000000100742b000000000000000000006a160000000000000000642ba6
-            010000ab0100000000000000007d1f742f000000000000000000006a1800
-            000000000000007c1fa6010000ab0100000000000000007d207401000000
-            000000000000006a0a00000000000000007c007c20ac2ca6020000ab0200
-            000000000000007d217c21a0190000000000000000000000000000000000
-            0000006420642d642e642f6412ac30a6050000ab05000000000000000001
-            0002008926a6000000ab00000000000000000001007c00a01a0000000000
-            000000000000000000000000000000a6000000ab00000000000000000001
-            007c00a01b0000000000000000000000000000000000000000a6000000ab
-            0000000000000000000100743800000000000000000000a01d0000000000
-            000000000000000000000000000000a6000000ab00000000000000000001
-            00743d000000000000000000006a1f000000000000000074400000000000
-            000000000064316702640eac32a6020000ab020000000000000000010064
-            005300743800000000000000000000a01d00000000000000000000000000
-            00000000000000a6000000ab0000000000000000000100743d0000000000
-            00000000006a1f0000000000000000744000000000000000000000643167
-            02640eac32a6020000ab0200000000000000000100743d00000000000000
-            0000006a1f00000000000000007440000000000000000000007442000000
-            000000000000006702640eac32a6020000ab020000000000000000010064
-            005300
-                       0 MAKE_CELL               34 (errortext)
-                       2 MAKE_CELL               35 (runcount)
-                       4 MAKE_CELL               36 (send_email)
-                       6 MAKE_CELL               37 (time_label)
-                       8 MAKE_CELL               38 (update_time)
-         
-         156          10 RESUME                   0
-         
-         158          12 LOAD_GLOBAL              1 (NULL + tk)
-                      24 LOAD_ATTR                1 (Tk)
-                      34 PRECALL                  0
-                      38 CALL                     0
-                      48 STORE_FAST               0 (root)
-         
-         159          50 LOAD_FAST                0 (root)
-                      52 LOAD_METHOD              2 (winfo_screenheight)
-                      74 PRECALL                  0
-                      78 CALL                     0
-                      88 STORE_FAST               1 (screen_height)
-         
-         160          90 LOAD_FAST                0 (root)
-                      92 LOAD_METHOD              3 (winfo_screenwidth)
-                     114 PRECALL                  0
-                     118 CALL                     0
-                     128 STORE_FAST               2 (screen_width)
-         
-         162         130 LOAD_CONST               1 ('Dimensions: ')
-                     132 LOAD_FAST                2 (screen_width)
-                     134 FORMAT_VALUE             0
-                     136 LOAD_CONST               2 (' x ')
-                     138 LOAD_FAST                1 (screen_height)
-                     140 FORMAT_VALUE             0
-                     142 BUILD_STRING             4
-                     144 STORE_FAST               3 (dimensions)
-         
-         163         146 LOAD_FAST                1 (screen_height)
-                     148 LOAD_CONST               3 (25)
-                     150 BINARY_OP                2 (//)
-                     154 STORE_FAST               4 (position)
-         
-         164         156 LOAD_CONST               4 (10)
-                     158 STORE_DEREF             35 (runcount)
-         
-         165         160 LOAD_CONST               5 ('We all have our favourites, but this task has been run too many times. \n\nPlease select another task to enjoy.')
-                     162 STORE_DEREF             34 (errortext)
-         
-         167         164 LOAD_GLOBAL              9 (NULL + glob)
-                     176 LOAD_ATTR                4 (glob)
-                     186 LOAD_GLOBAL             10 (folder_name)
-                     198 LOAD_CONST               6 ('/*Consent.txt')
-                     200 BINARY_OP                0 (+)
-                     204 PRECALL                  1
-                     208 CALL                     1
-                     218 EXTENDED_ARG             5
-                     220 POP_JUMP_FORWARD_IF_FALSE  1330 (to 2882)
-         
-         169         222 LOAD_GLOBAL             12 (spwf)
-                     234 LOAD_ATTR                7 (emailadd)
-                     244 STORE_FAST               5 (USERNAME)
-         
-         170         246 LOAD_GLOBAL             12 (spwf)
-                     258 LOAD_ATTR                8 (password)
-                     268 STORE_FAST               6 (PASSWORD)
-         
-         172         270 LOAD_CLOSURE            36 (send_email)
-                     272 BUILD_TUPLE              1
-                     274 LOAD_CONST               7 (<code object emailsupport, file "D:\Task Development\Stimuli\Task\Task.py", line 172>)
-                     276 MAKE_FUNCTION            8 (closure)
-                     278 STORE_FAST               7 (emailsupport)
-         
-         182         280 LOAD_CONST               8 (<code object send_email, file "D:\Task Development\Stimuli\Task\Task.py", line 182>)
-                     282 MAKE_FUNCTION            0
-                     284 STORE_DEREF             36 (send_email)
-         
-         203         286 LOAD_CLOSURE            34 (errortext)
-                     288 LOAD_CLOSURE            35 (runcount)
-                     290 BUILD_TUPLE              2
-                     292 LOAD_CONST               9 (<code object pis, file "D:\Task Development\Stimuli\Task\Task.py", line 203>)
-                     294 MAKE_FUNCTION            8 (closure)
-                     296 STORE_FAST               8 (pis)
-         
-         214         298 LOAD_CONST              10 (('Helvetica', 18))
-                     300 STORE_FAST               9 (fontsize)
-         
-         215         302 LOAD_CONST              11 (('Helvetica', 22))
-                     304 STORE_FAST              10 (fontsize1)
-         
-         216         306 LOAD_CONST              12 (('Helvetica', 12))
-                     308 STORE_FAST              11 (fontsize2)
-         
-         218         310 LOAD_FAST                0 (root)
-                     312 LOAD_METHOD              9 (attributes)
-                     334 LOAD_CONST              13 ('-fullscreen')
-                     336 LOAD_CONST              14 (True)
-                     338 PRECALL                  2
-                     342 CALL                     2
-                     352 POP_TOP
-         
-         220         354 LOAD_GLOBAL              1 (NULL + tk)
-                     366 LOAD_ATTR               10 (Label)
-                     376 LOAD_FAST                0 (root)
-                     378 LOAD_CONST              15 ('')
-                     380 LOAD_FAST                9 (fontsize)
-                     382 KW_NAMES                16
-                     384 PRECALL                  3
-                     388 CALL                     3
-                     398 STORE_DEREF             37 (time_label)
-         
-         222         400 LOAD_CLOSURE            37 (time_label)
-                     402 LOAD_CLOSURE            38 (update_time)
-                     404 BUILD_TUPLE              2
-                     406 LOAD_CONST              17 (<code object update_time, file "D:\Task Development\Stimuli\Task\Task.py", line 222>)
-                     408 MAKE_FUNCTION            8 (closure)
-                     410 STORE_DEREF             38 (update_time)
-         
-         227         412 LOAD_DEREF              37 (time_label)
-                     414 LOAD_METHOD             11 (pack)
-                     436 LOAD_GLOBAL              0 (tk)
-                     448 LOAD_ATTR               12 (TOP)
-                     458 LOAD_CONST              18 (20)
-                     460 LOAD_CONST               4 (10)
-                     462 LOAD_CONST              19 ('nw')
-                     464 KW_NAMES                20
-                     466 PRECALL                  4
-                     470 CALL                     4
-                     480 POP_TOP
-         
-         229         482 LOAD_GLOBAL              1 (NULL + tk)
-                     494 LOAD_ATTR               13 (Frame)
-                     504 LOAD_FAST                0 (root)
-                     506 PRECALL                  1
-                     510 CALL                     1
-                     520 STORE_FAST              12 (welcome_frame)
-         
-         230         522 LOAD_FAST               12 (welcome_frame)
-                     524 LOAD_METHOD             11 (pack)
-                     546 LOAD_GLOBAL              0 (tk)
-                     558 LOAD_ATTR               12 (TOP)
-                     568 LOAD_GLOBAL              0 (tk)
-                     580 LOAD_ATTR               14 (X)
-                     590 KW_NAMES                21
-                     592 PRECALL                  2
-                     596 CALL                     2
-                     606 POP_TOP
-         
-         232         608 LOAD_GLOBAL              1 (NULL + tk)
-                     620 LOAD_ATTR               10 (Label)
-                     630 LOAD_FAST               12 (welcome_frame)
-                     632 LOAD_CONST              22 ('Welcome back!')
-                     634 LOAD_FAST               10 (fontsize1)
-                     636 KW_NAMES                16
-                     638 PRECALL                  3
-                     642 CALL                     3
-                     652 STORE_FAST              13 (welcome_label)
-         
-         233         654 LOAD_FAST               13 (welcome_label)
-                     656 LOAD_METHOD             11 (pack)
-                     678 LOAD_FAST                4 (position)
-                     680 KW_NAMES                23
-                     682 PRECALL                  1
-                     686 CALL                     1
-                     696 POP_TOP
-         
-         235         698 LOAD_GLOBAL              1 (NULL + tk)
-                     710 LOAD_ATTR               13 (Frame)
-                     720 LOAD_FAST                0 (root)
-                     722 PRECALL                  1
-                     726 CALL                     1
-                     736 STORE_FAST              14 (text_frame)
-         
-         236         738 LOAD_FAST               14 (text_frame)
-                     740 LOAD_METHOD             11 (pack)
-                     762 LOAD_GLOBAL              0 (tk)
-                     774 LOAD_ATTR               12 (TOP)
-                     784 LOAD_GLOBAL              0 (tk)
-                     796 LOAD_ATTR               14 (X)
-                     806 KW_NAMES                21
-                     808 PRECALL                  2
-                     812 CALL                     2
-                     822 POP_TOP
-         
-         238         824 LOAD_GLOBAL              1 (NULL + tk)
-                     836 LOAD_ATTR               10 (Label)
-                     846 LOAD_FAST               12 (welcome_frame)
-                     848 LOAD_CONST              24 ('Please now select a task to perform')
-                     850 LOAD_FAST                9 (fontsize)
-                     852 KW_NAMES                16
-                     854 PRECALL                  3
-                     858 CALL                     3
-                     868 STORE_FAST              15 (text_label)
-         
-         239         870 LOAD_FAST               15 (text_label)
-                     872 LOAD_METHOD             11 (pack)
-                     894 LOAD_FAST                4 (position)
-                     896 KW_NAMES                23
-                     898 PRECALL                  1
-                     902 CALL                     1
-                     912 POP_TOP
-         
-         241         914 LOAD_GLOBAL              1 (NULL + tk)
-                     926 LOAD_ATTR               13 (Frame)
-                     936 LOAD_FAST                0 (root)
-                     938 PRECALL                  1
-                     942 CALL                     1
-                     952 STORE_FAST              16 (nback_frame)
-         
-         242         954 LOAD_FAST               16 (nback_frame)
-                     956 LOAD_METHOD             11 (pack)
-                     978 LOAD_GLOBAL              0 (tk)
-                     990 LOAD_ATTR               12 (TOP)
-                    1000 LOAD_CONST              25 (30)
-                    1002 LOAD_CONST              26 (5)
-                    1004 LOAD_CONST              27 ('center')
-                    1006 KW_NAMES                20
-                    1008 PRECALL                  4
-                    1012 CALL                     4
-                    1022 POP_TOP
-         
-         244        1024 LOAD_CLOSURE            34 (errortext)
-                    1026 LOAD_CLOSURE            35 (runcount)
-                    1028 BUILD_TUPLE              2
-                    1030 LOAD_CONST              28 (<code object nbrun, file "D:\Task Development\Stimuli\Task\Task.py", line 244>)
-                    1032 MAKE_FUNCTION            8 (closure)
-                    1034 STORE_FAST              17 (nbrun)
-         
-         254        1036 LOAD_GLOBAL              1 (NULL + tk)
-                    1048 LOAD_ATTR               15 (Button)
-                    1058 LOAD_FAST               16 (nback_frame)
-                    1060 LOAD_CONST              29 ('N-Back')
-                    1062 LOAD_FAST               17 (nbrun)
-                    1064 LOAD_FAST                9 (fontsize)
-                    1066 LOAD_CONST              27 ('center')
-                    1068 KW_NAMES                30
-                    1070 PRECALL                  5
-                    1074 CALL                     5
-                    1084 STORE_FAST              18 (nback)
-         
-         255        1086 LOAD_FAST               18 (nback)
-                    1088 LOAD_METHOD             11 (pack)
-                    1110 LOAD_GLOBAL              0 (tk)
-                    1122 LOAD_ATTR               12 (TOP)
-                    1132 LOAD_CONST              26 (5)
-                    1134 KW_NAMES                31
-                    1136 PRECALL                  2
-                    1140 CALL                     2
-                    1150 POP_TOP
-         
-         257        1152 LOAD_GLOBAL             32 (nbcount)
-                    1164 LOAD_CONST              32 (1)
-                    1166 COMPARE_OP               2 (==)
-                    1172 POP_JUMP_FORWARD_IF_FALSE    12 (to 1198)
-         
-         258        1174 LOAD_CONST              33 ('You have completed this ')
-                    1176 LOAD_GLOBAL             32 (nbcount)
-                    1188 FORMAT_VALUE             0
-                    1190 LOAD_CONST              34 (' time so far')
-                    1192 BUILD_STRING             3
-                    1194 STORE_FAST              19 (text)
-                    1196 JUMP_FORWARD            11 (to 1220)
-         
-         260     >> 1198 LOAD_CONST              33 ('You have completed this ')
-                    1200 LOAD_GLOBAL             32 (nbcount)
-                    1212 FORMAT_VALUE             0
-                    1214 LOAD_CONST              35 (' times so far')
-                    1216 BUILD_STRING             3
-                    1218 STORE_FAST              19 (text)
-         
-         261     >> 1220 LOAD_GLOBAL              1 (NULL + tk)
-                    1232 LOAD_ATTR               10 (Label)
-                    1242 LOAD_FAST               16 (nback_frame)
-                    1244 LOAD_FAST               19 (text)
-                    1246 LOAD_FAST               11 (fontsize2)
-                    1248 KW_NAMES                16
-                    1250 PRECALL                  3
-                    1254 CALL                     3
-                    1264 STORE_FAST              20 (nback_label)
-         
-         262        1266 LOAD_FAST               20 (nback_label)
-                    1268 LOAD_METHOD             11 (pack)
-                    1290 LOAD_GLOBAL              0 (tk)
-                    1302 LOAD_ATTR               12 (TOP)
-                    1312 LOAD_CONST              26 (5)
-                    1314 LOAD_CONST              27 ('center')
-                    1316 KW_NAMES                36
-                    1318 PRECALL                  3
-                    1322 CALL                     3
-                    1332 POP_TOP
-         
-         265        1334 LOAD_GLOBAL              1 (NULL + tk)
-                    1346 LOAD_ATTR               13 (Frame)
-                    1356 LOAD_FAST                0 (root)
-                    1358 PRECALL                  1
-                    1362 CALL                     1
-                    1372 STORE_FAST              21 (button1_frame)
-         
-         266        1374 LOAD_FAST               21 (button1_frame)
-                    1376 LOAD_METHOD             11 (pack)
-                    1398 LOAD_GLOBAL              0 (tk)
-                    1410 LOAD_ATTR               12 (TOP)
-                    1420 LOAD_CONST              25 (30)
-                    1422 LOAD_CONST              26 (5)
-                    1424 LOAD_CONST              27 ('center')
-                    1426 KW_NAMES                20
-                    1428 PRECALL                  4
-                    1432 CALL                     4
-                    1442 POP_TOP
-         
-         268        1444 LOAD_GLOBAL              1 (NULL + tk)
-                    1456 LOAD_ATTR               13 (Frame)
-                    1466 LOAD_FAST                0 (root)
-                    1468 PRECALL                  1
-                    1472 CALL                     1
-                    1482 STORE_FAST              22 (button2_frame)
-         
-         269        1484 LOAD_FAST               22 (button2_frame)
-                    1486 LOAD_METHOD             11 (pack)
-                    1508 LOAD_GLOBAL              0 (tk)
-                    1520 LOAD_ATTR               12 (TOP)
-                    1530 LOAD_CONST              25 (30)
-                    1532 LOAD_CONST              26 (5)
-                    1534 LOAD_CONST              27 ('center')
-                    1536 KW_NAMES                20
-                    1538 PRECALL                  4
-                    1542 CALL                     4
-                    1552 POP_TOP
-         
-         271        1554 LOAD_GLOBAL              1 (NULL + tk)
-                    1566 LOAD_ATTR               15 (Button)
-                    1576 LOAD_FAST               22 (button2_frame)
-                    1578 LOAD_CONST              37 ('Switching Task')
-                    1580 LOAD_FAST                8 (pis)
-                    1582 LOAD_FAST                9 (fontsize)
-                    1584 LOAD_CONST              27 ('center')
-                    1586 KW_NAMES                30
-                    1588 PRECALL                  5
-                    1592 CALL                     5
-                    1602 STORE_FAST              23 (button2)
-         
-         272        1604 LOAD_FAST               23 (button2)
-                    1606 LOAD_METHOD             11 (pack)
-                    1628 LOAD_GLOBAL              0 (tk)
-                    1640 LOAD_ATTR               12 (TOP)
-                    1650 LOAD_CONST              26 (5)
-                    1652 KW_NAMES                31
-                    1654 PRECALL                  2
-                    1658 CALL                     2
-                    1668 POP_TOP
-         
-         274        1670 LOAD_GLOBAL             34 (scount)
-                    1682 LOAD_CONST              32 (1)
-                    1684 COMPARE_OP               2 (==)
-                    1690 POP_JUMP_FORWARD_IF_FALSE    12 (to 1716)
-         
-         275        1692 LOAD_CONST              33 ('You have completed this ')
-                    1694 LOAD_GLOBAL             34 (scount)
-                    1706 FORMAT_VALUE             0
-                    1708 LOAD_CONST              34 (' time so far')
-                    1710 BUILD_STRING             3
-                    1712 STORE_FAST              19 (text)
-                    1714 JUMP_FORWARD            11 (to 1738)
-         
-         277     >> 1716 LOAD_CONST              33 ('You have completed this ')
-                    1718 LOAD_GLOBAL             34 (scount)
-                    1730 FORMAT_VALUE             0
-                    1732 LOAD_CONST              35 (' times so far')
-                    1734 BUILD_STRING             3
-                    1736 STORE_FAST              19 (text)
-         
-         278     >> 1738 LOAD_GLOBAL              1 (NULL + tk)
-                    1750 LOAD_ATTR               10 (Label)
-                    1760 LOAD_FAST               22 (button2_frame)
-                    1762 LOAD_FAST               19 (text)
-                    1764 LOAD_FAST               11 (fontsize2)
-                    1766 KW_NAMES                16
-                    1768 PRECALL                  3
-                    1772 CALL                     3
-                    1782 STORE_FAST              24 (button2_label)
-         
-         279        1784 LOAD_FAST               24 (button2_label)
-                    1786 LOAD_METHOD             11 (pack)
-                    1808 LOAD_GLOBAL              0 (tk)
-                    1820 LOAD_ATTR               12 (TOP)
-                    1830 LOAD_CONST              26 (5)
-                    1832 KW_NAMES                31
-                    1834 PRECALL                  2
-                    1838 CALL                     2
-                    1848 POP_TOP
-         
-         281        1850 LOAD_CLOSURE            34 (errortext)
-                    1852 LOAD_CLOSURE            35 (runcount)
-                    1854 BUILD_TUPLE              2
-                    1856 LOAD_CONST              38 (<code object consent, file "D:\Task Development\Stimuli\Task\Task.py", line 281>)
-                    1858 MAKE_FUNCTION            8 (closure)
-                    1860 STORE_FAST              25 (consent)
-         
-         291        1862 LOAD_GLOBAL              1 (NULL + tk)
-                    1874 LOAD_ATTR               13 (Frame)
-                    1884 LOAD_FAST                0 (root)
-                    1886 PRECALL                  1
-                    1890 CALL                     1
-                    1900 STORE_FAST              26 (button3_frame)
-         
-         292        1902 LOAD_FAST               26 (button3_frame)
-                    1904 LOAD_METHOD             11 (pack)
-                    1926 LOAD_GLOBAL              0 (tk)
-                    1938 LOAD_ATTR               12 (TOP)
-                    1948 LOAD_CONST              25 (30)
-                    1950 LOAD_CONST               4 (10)
-                    1952 LOAD_CONST              27 ('center')
-                    1954 KW_NAMES                20
-                    1956 PRECALL                  4
-                    1960 CALL                     4
-                    1970 POP_TOP
-         
-         293        1972 LOAD_GLOBAL              1 (NULL + tk)
-                    1984 LOAD_ATTR               15 (Button)
-                    1994 LOAD_FAST               26 (button3_frame)
-                    1996 LOAD_CONST              39 ('2-Type Reaction Time')
-                    1998 LOAD_FAST               25 (consent)
-                    2000 LOAD_FAST                9 (fontsize)
-                    2002 LOAD_CONST              27 ('center')
-                    2004 KW_NAMES                30
-                    2006 PRECALL                  5
-                    2010 CALL                     5
-                    2020 STORE_FAST              27 (button3)
-         
-         294        2022 LOAD_FAST               27 (button3)
-                    2024 LOAD_METHOD             11 (pack)
-                    2046 LOAD_GLOBAL              0 (tk)
-                    2058 LOAD_ATTR               12 (TOP)
-                    2068 LOAD_CONST              26 (5)
-                    2070 KW_NAMES                31
-                    2072 PRECALL                  2
-                    2076 CALL                     2
-                    2086 POP_TOP
-         
-         296        2088 LOAD_GLOBAL             36 (rtcount)
-                    2100 LOAD_CONST              32 (1)
-                    2102 COMPARE_OP               2 (==)
-                    2108 POP_JUMP_FORWARD_IF_FALSE    12 (to 2134)
-         
-         297        2110 LOAD_CONST              33 ('You have completed this ')
-                    2112 LOAD_GLOBAL             36 (rtcount)
-                    2124 FORMAT_VALUE             0
-                    2126 LOAD_CONST              34 (' time so far')
-                    2128 BUILD_STRING             3
-                    2130 STORE_FAST              19 (text)
-                    2132 JUMP_FORWARD            11 (to 2156)
-         
-         299     >> 2134 LOAD_CONST              33 ('You have completed this ')
-                    2136 LOAD_GLOBAL             36 (rtcount)
-                    2148 FORMAT_VALUE             0
-                    2150 LOAD_CONST              35 (' times so far')
-                    2152 BUILD_STRING             3
-                    2154 STORE_FAST              19 (text)
-         
-         300     >> 2156 LOAD_GLOBAL              1 (NULL + tk)
-                    2168 LOAD_ATTR               10 (Label)
-                    2178 LOAD_FAST               26 (button3_frame)
-                    2180 LOAD_FAST               19 (text)
-                    2182 LOAD_FAST               11 (fontsize2)
-                    2184 KW_NAMES                16
-                    2186 PRECALL                  3
-                    2190 CALL                     3
-                    2200 STORE_FAST              28 (button3_label)
-         
-         301        2202 LOAD_FAST               28 (button3_label)
-                    2204 LOAD_METHOD             11 (pack)
-                    2226 LOAD_GLOBAL              0 (tk)
-                    2238 LOAD_ATTR               12 (TOP)
-                    2248 LOAD_CONST              26 (5)
-                    2250 LOAD_CONST              27 ('center')
-                    2252 KW_NAMES                36
-                    2254 PRECALL                  3
-                    2258 CALL                     3
-                    2268 POP_TOP
-         
-         303        2270 LOAD_GLOBAL              1 (NULL + tk)
-                    2282 LOAD_ATTR               13 (Frame)
-                    2292 LOAD_FAST                0 (root)
-                    2294 PRECALL                  1
-                    2298 CALL                     1
-                    2308 STORE_FAST              29 (button12_frame)
-         
-         304        2310 LOAD_FAST               29 (button12_frame)
-                    2312 LOAD_METHOD             11 (pack)
-                    2334 LOAD_GLOBAL              0 (tk)
-                    2346 LOAD_ATTR               19 (BOTTOM)
-                    2356 LOAD_CONST              25 (30)
-                    2358 LOAD_CONST              18 (20)
-                    2360 LOAD_CONST              40 ('sw')
-                    2362 KW_NAMES                20
-                    2364 PRECALL                  4
-                    2368 CALL                     4
-                    2378 POP_TOP
-         
-         306        2380 LOAD_GLOBAL              1 (NULL + tk)
-                    2392 LOAD_ATTR               15 (Button)
-                    2402 LOAD_FAST               29 (button12_frame)
-                    2404 LOAD_CONST              41 ('Email for assistance or queries')
-                    2406 LOAD_FAST                7 (emailsupport)
-                    2408 LOAD_FAST                9 (fontsize)
-                    2410 KW_NAMES                42
-                    2412 PRECALL                  4
-                    2416 CALL                     4
-                    2426 STORE_FAST              30 (button12)
-         
-         307        2428 LOAD_FAST               30 (button12)
-                    2430 LOAD_METHOD             11 (pack)
-                    2452 LOAD_GLOBAL              0 (tk)
-                    2464 LOAD_ATTR               20 (LEFT)
-                    2474 LOAD_CONST               4 (10)
-                    2476 KW_NAMES                31
-                    2478 PRECALL                  2
-                    2482 CALL                     2
-                    2492 POP_TOP
-         
-         309        2494 LOAD_GLOBAL             43 (NULL + Image)
-                    2506 LOAD_ATTR               22 (open)
-                    2516 LOAD_CONST              43 ('uop.png')
-                    2518 PRECALL                  1
-                    2522 CALL                     1
-                    2532 STORE_FAST              31 (image_file)
-         
-         310        2534 LOAD_GLOBAL             47 (NULL + ImageTk)
-                    2546 LOAD_ATTR               24 (PhotoImage)
-                    2556 LOAD_FAST               31 (image_file)
-                    2558 PRECALL                  1
-                    2562 CALL                     1
-                    2572 STORE_FAST              32 (image2)
-         
-         311        2574 LOAD_GLOBAL              1 (NULL + tk)
-                    2586 LOAD_ATTR               10 (Label)
-                    2596 LOAD_FAST                0 (root)
-                    2598 LOAD_FAST               32 (image2)
-                    2600 KW_NAMES                44
-                    2602 PRECALL                  2
-                    2606 CALL                     2
-                    2616 STORE_FAST              33 (image_label)
-         
-         312        2618 LOAD_FAST               33 (image_label)
-                    2620 LOAD_METHOD             25 (place)
-                    2642 LOAD_CONST              32 (1)
-                    2644 LOAD_CONST              45 (0)
-                    2646 LOAD_CONST              46 ('ne')
-                    2648 LOAD_CONST              47 (-20)
-                    2650 LOAD_CONST              18 (20)
-                    2652 KW_NAMES                48
-                    2654 PRECALL                  5
-                    2658 CALL                     5
-                    2668 POP_TOP
-         
-         313        2670 PUSH_NULL
-                    2672 LOAD_DEREF              38 (update_time)
-                    2674 PRECALL                  0
-                    2678 CALL                     0
-                    2688 POP_TOP
-         
-         315        2690 LOAD_FAST                0 (root)
-                    2692 LOAD_METHOD             26 (mainloop)
-                    2714 PRECALL                  0
-                    2718 CALL                     0
-                    2728 POP_TOP
-         
-         317        2730 LOAD_FAST                0 (root)
-                    2732 LOAD_METHOD             27 (quit)
-                    2754 PRECALL                  0
-                    2758 CALL                     0
-                    2768 POP_TOP
-         
-         318        2770 LOAD_GLOBAL             56 (cpurun)
-                    2782 LOAD_METHOD             29 (terminate)
-                    2804 PRECALL                  0
-                    2808 CALL                     0
-                    2818 POP_TOP
-         
-         319        2820 LOAD_GLOBAL             61 (NULL + subprocess)
-                    2832 LOAD_ATTR               31 (run)
-                    2842 LOAD_GLOBAL             64 (python_path)
-                    2854 LOAD_CONST              49 ('Export.py')
-                    2856 BUILD_LIST               2
-                    2858 LOAD_CONST              14 (True)
-                    2860 KW_NAMES                50
-                    2862 PRECALL                  2
-                    2866 CALL                     2
-                    2876 POP_TOP
-                    2878 LOAD_CONST               0 (None)
-                    2880 RETURN_VALUE
-         
-         323     >> 2882 LOAD_GLOBAL             56 (cpurun)
-                    2894 LOAD_METHOD             29 (terminate)
-                    2916 PRECALL                  0
-                    2920 CALL                     0
-                    2930 POP_TOP
-         
-         324        2932 LOAD_GLOBAL             61 (NULL + subprocess)
-                    2944 LOAD_ATTR               31 (run)
-                    2954 LOAD_GLOBAL             64 (python_path)
-                    2966 LOAD_CONST              49 ('Export.py')
-                    2968 BUILD_LIST               2
-                    2970 LOAD_CONST              14 (True)
-                    2972 KW_NAMES                50
-                    2974 PRECALL                  2
-                    2978 CALL                     2
-                    2988 POP_TOP
-         
-         325        2990 LOAD_GLOBAL             61 (NULL + subprocess)
-                    3002 LOAD_ATTR               31 (run)
-                    3012 LOAD_GLOBAL             64 (python_path)
-                    3024 LOAD_GLOBAL             66 (file_path)
-                    3036 BUILD_LIST               2
-                    3038 LOAD_CONST              14 (True)
-                    3040 KW_NAMES                50
-                    3042 PRECALL                  2
-                    3046 CALL                     2
-                    3056 POP_TOP
-                    3058 LOAD_CONST               0 (None)
-                    3060 RETURN_VALUE
+            0x8733873487358736873787388739873a873b873c873d873e873f970064
+            0164006c008a3b640164006c017d00640164006c027d01640164006c037d
+            02640164006c047d037c036a0500000000000000008a37640164006c068a
+            3a640164006c078a3e640164006c088a3c640164026c096d0a7d046d0b7d
+            050100640164036c0c6d0c7d060100640164046c076d0d7d070100640164
+            056c076d0e7d086d0f8a360100640164006c107d09640164066c116d128a
+            340100640164076c136d148a336d157d0a6d167d0b6d177d0c6d187d0d6d
+            197d0e01000200893e6a1a0000000000000000a6000000ab000000000000
+            0000008a388938a01b0000000000000000000000000000000000000000a6
+            000000ab0000000000000000007d0f8938a01c0000000000000000000000
+            000000000000000000a6000000ab0000000000000000007d1064087c109b
+            0064097c0f9b009d047d117c0f640a7a0200007d12640b8a39640c8a3574
+            3b000000000000000000006a1d0000000000000000743c00000000000000
+            000000640d7a000000a6010000ab010000000000000000900472b5893a6a
+            1f00000000000000007d13893a6a2000000000000000007d148833883488
+            3a883e6604640e84087d158835883688378839883b6605640f84087d1664
+            107d1764117d1864127d1964127d1a8938a0210000000000000000000000
+            00000000000000000064136414a6020000ab020000000000000000010089
+            38a021000000000000000000000000000000000000000064156416a60200
+            00ab020000000000000000010088386601641784087d1b0200893e6a2200
+            00000000000000893864187c1b7c1aac19a6040000ab0400000000000000
+            007d1c7c1ca0230000000000000000000000000000000000000000641a64
+            1b640b641cac1da6040000ab04000000000000000001000200893e6a2400
+            000000000000008938641e7c17ac1fa6030000ab0300000000000000008a
+            3d883c883d883f6603642084088a3f893da0230000000000000000000000
+            000000000000000000893e6a250000000000000000642164016422ac23a6
+            040000ab04000000000000000001000200893e6a26000000000000000089
+            38a6010000ab0100000000000000007d1d7c1da023000000000000000000
+            0000000000000000000000893e6a250000000000000000893e6a27000000
+            0000000000ac24a6020000ab02000000000000000001000200893e6a2400
+            000000000000007c1d64257c18ac1fa6030000ab0300000000000000007d
+            1e7c1ea02300000000000000000000000000000000000000007c12ac26a6
+            010000ab01000000000000000001000200893e6a26000000000000000089
+            38a6010000ab0100000000000000007d1f7c1fa023000000000000000000
+            0000000000000000000000893e6a250000000000000000893e6a27000000
+            0000000000ac24a6020000ab02000000000000000001000200893e6a2400
+            000000000000007c1d64277c17ac1fa6030000ab0300000000000000007d
+            207c20a02300000000000000000000000000000000000000007c12ac26a6
+            010000ab01000000000000000001000200893e6a26000000000000000089
+            38a6010000ab0100000000000000007d217c21a023000000000000000000
+            0000000000000000000000893e6a2500000000000000006428641c6429ac
+            23a6040000ab04000000000000000001008835883688378839883b660564
+            2a84087d220200893e6a2200000000000000007c21642b7c227c176429ac
+            2ca6050000ab0500000000000000007d237c23a023000000000000000000
+            0000000000000000000000893e6a250000000000000000641cac2da60200
+            00ab0200000000000000000100745000000000000000000000642e6b0200
+            000000720c642f7450000000000000000000009b0064309d037d246e0b64
+            2f7450000000000000000000009b0064319d037d240200893e6a24000000
+            00000000007c217c247c19ac1fa6030000ab0300000000000000007d257c
+            25a0230000000000000000000000000000000000000000893e6a25000000
+            0000000000641c6429ac32a6030000ab0300000000000000000100020089
+            3e6a2600000000000000008938a6010000ab0100000000000000007d267c
+            26a0230000000000000000000000000000000000000000893e6a25000000
+            00000000006428641c6429ac23a6040000ab040000000000000000010002
+            00893e6a2600000000000000008938a6010000ab0100000000000000007d
+            277c27a0230000000000000000000000000000000000000000893e6a2500
+            000000000000006428641c6429ac23a6040000ab04000000000000000001
+            000200893e6a2200000000000000007c2764337c167c176429ac2ca60500
+            00ab0500000000000000007d287c28a02300000000000000000000000000
+            00000000000000893e6a250000000000000000641cac2da6020000ab0200
+            000000000000000100745200000000000000000000642e6b020000000072
+            0c642f7452000000000000000000009b0064309d037d246e0b642f745200
+            0000000000000000009b0064319d037d240200893e6a2400000000000000
+            007c277c247c19ac1fa6030000ab0300000000000000007d297c29a02300
+            00000000000000000000000000000000000000893e6a2500000000000000
+            00641cac2da6020000ab0200000000000000000100883588368837883988
+            3b6605643484087d2a0200893e6a2600000000000000008938a6010000ab
+            0100000000000000007d2b7c2ba023000000000000000000000000000000
+            0000000000893e6a2500000000000000006428640b6429ac23a6040000ab
+            04000000000000000001000200893e6a2200000000000000007c2b64357c
+            2a7c176429ac2ca6050000ab0500000000000000007d2c7c2ca023000000
+            0000000000000000000000000000000000893e6a25000000000000000064
+            1cac2da6020000ab02000000000000000001007454000000000000000000
+            00642e6b0200000000720c642f7454000000000000000000009b0064309d
+            037d246e0b642f7454000000000000000000009b0064319d037d24020089
+            3e6a2400000000000000007c2b7c247c19ac1fa6030000ab030000000000
+            0000007d2d7c2da023000000000000000000000000000000000000000089
+            3e6a250000000000000000641c6429ac32a6030000ab0300000000000000
+            0001000200893e6a2600000000000000008938a6010000ab010000000000
+            0000007d2e7c2ea023000000000000000000000000000000000000000089
+            3e6a2b0000000000000000642864216436ac23a6040000ab040000000000
+            00000001000200893e6a2200000000000000007c2e64377c157c17ac19a6
+            040000ab0400000000000000007d2f7c2fa0230000000000000000000000
+            000000000000000000893e6a2c0000000000000000640bac2da6020000ab
+            020000000000000000010002007c046a2d00000000000000006438a60100
+            00ab0100000000000000007d3002007c056a2e00000000000000007c30a6
+            010000ab0100000000000000007d310200893e6a24000000000000000089
+            387c31ac39a6020000ab0200000000000000007d327c32a02f0000000000
+            000000000000000000000000000000642e6401641b643a643bac3ca60500
+            00ab05000000000000000001000200893fa6000000ab0000000000000000
+            0001000200893b6a3000000000000000008937643d67026414ac3ea60200
+            00ab02000000000000000001008938a03100000000000000000000000000
+            00000000000000a6000000ab00000000000000000001008938a032000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            000100640053000200893b6a3000000000000000008937643d67026414ac
+            3ea6020000ab02000000000000000001000200893b6a3000000000000000
+            00893774660000000000000000000067026414ac3ea6020000ab02000000
+            0000000000010064005300
+                       0 MAKE_CELL               51 (Mail)
+                       2 MAKE_CELL               52 (SendGridAPIClient)
+                       4 MAKE_CELL               53 (errortext)
+                       6 MAKE_CELL               54 (messagebox)
+                       8 MAKE_CELL               55 (python_path)
+                      10 MAKE_CELL               56 (root)
+                      12 MAKE_CELL               57 (runcount)
+                      14 MAKE_CELL               58 (spwf)
+                      16 MAKE_CELL               59 (subprocess)
+                      18 MAKE_CELL               60 (time)
+                      20 MAKE_CELL               61 (time_label)
+                      22 MAKE_CELL               62 (tk)
+                      24 MAKE_CELL               63 (update_time)
+         
+         156          26 RESUME                   0
+         
+         159          28 LOAD_CONST               1 (0)
+                      30 LOAD_CONST               0 (None)
+                      32 IMPORT_NAME              0 (subprocess)
+                      34 STORE_DEREF             59 (subprocess)
+         
+         160          36 LOAD_CONST               1 (0)
+                      38 LOAD_CONST               0 (None)
+                      40 IMPORT_NAME              1 (random)
+                      42 STORE_FAST               0 (random)
+         
+         161          44 LOAD_CONST               1 (0)
+                      46 LOAD_CONST               0 (None)
+                      48 IMPORT_NAME              2 (platform)
+                      50 STORE_FAST               1 (platform)
+         
+         162          52 LOAD_CONST               1 (0)
+                      54 LOAD_CONST               0 (None)
+                      56 IMPORT_NAME              3 (os)
+                      58 STORE_FAST               2 (os)
+         
+         163          60 LOAD_CONST               1 (0)
+                      62 LOAD_CONST               0 (None)
+                      64 IMPORT_NAME              4 (sys)
+                      66 STORE_FAST               3 (sys)
+         
+         164          68 LOAD_FAST                3 (sys)
+                      70 LOAD_ATTR                5 (executable)
+                      80 STORE_DEREF             55 (python_path)
+         
+         166          82 LOAD_CONST               1 (0)
+                      84 LOAD_CONST               0 (None)
+                      86 IMPORT_NAME              6 (spwf)
+                      88 STORE_DEREF             58 (spwf)
+         
+         167          90 LOAD_CONST               1 (0)
+                      92 LOAD_CONST               0 (None)
+                      94 IMPORT_NAME              7 (tkinter)
+                      96 STORE_DEREF             62 (tk)
+         
+         168          98 LOAD_CONST               1 (0)
+                     100 LOAD_CONST               0 (None)
+                     102 IMPORT_NAME              8 (time)
+                     104 STORE_DEREF             60 (time)
+         
+         169         106 LOAD_CONST               1 (0)
+                     108 LOAD_CONST               2 (('Image', 'ImageTk'))
+                     110 IMPORT_NAME              9 (PIL)
+                     112 IMPORT_FROM             10 (Image)
+                     114 STORE_FAST               4 (Image)
+                     116 IMPORT_FROM             11 (ImageTk)
+                     118 STORE_FAST               5 (ImageTk)
+                     120 POP_TOP
+         
+         170         122 LOAD_CONST               1 (0)
+                     124 LOAD_CONST               3 (('datetime',))
+                     126 IMPORT_NAME             12 (datetime)
+                     128 IMPORT_FROM             12 (datetime)
+                     130 STORE_FAST               6 (datetime)
+                     132 POP_TOP
+         
+         171         134 LOAD_CONST               1 (0)
+                     136 LOAD_CONST               4 (('filedialog',))
+                     138 IMPORT_NAME              7 (tkinter)
+                     140 IMPORT_FROM             13 (filedialog)
+                     142 STORE_FAST               7 (filedialog)
+                     144 POP_TOP
+         
+         172         146 LOAD_CONST               1 (0)
+                     148 LOAD_CONST               5 (('simpledialog', 'messagebox'))
+                     150 IMPORT_NAME              7 (tkinter)
+                     152 IMPORT_FROM             14 (simpledialog)
+                     154 STORE_FAST               8 (simpledialog)
+                     156 IMPORT_FROM             15 (messagebox)
+                     158 STORE_DEREF             54 (messagebox)
+                     160 POP_TOP
+         
+         173         162 LOAD_CONST               1 (0)
+                     164 LOAD_CONST               0 (None)
+                     166 IMPORT_NAME             16 (Location)
+                     168 STORE_FAST               9 (Location)
+         
+         174         170 LOAD_CONST               1 (0)
+                     172 LOAD_CONST               6 (('SendGridAPIClient',))
+                     174 IMPORT_NAME             17 (sendgrid)
+                     176 IMPORT_FROM             18 (SendGridAPIClient)
+                     178 STORE_DEREF             52 (SendGridAPIClient)
+                     180 POP_TOP
+         
+         175         182 LOAD_CONST               1 (0)
+                     184 LOAD_CONST               7 (('Mail', 'Attachment', 'FileContent', 'FileName', 'FileType', 'Disposition'))
+                     186 IMPORT_NAME             19 (sendgrid.helpers.mail)
+                     188 IMPORT_FROM             20 (Mail)
+                     190 STORE_DEREF             51 (Mail)
+                     192 IMPORT_FROM             21 (Attachment)
+                     194 STORE_FAST              10 (Attachment)
+                     196 IMPORT_FROM             22 (FileContent)
+                     198 STORE_FAST              11 (FileContent)
+                     200 IMPORT_FROM             23 (FileName)
+                     202 STORE_FAST              12 (FileName)
+                     204 IMPORT_FROM             24 (FileType)
+                     206 STORE_FAST              13 (FileType)
+                     208 IMPORT_FROM             25 (Disposition)
+                     210 STORE_FAST              14 (Disposition)
+                     212 POP_TOP
+         
+         178         214 PUSH_NULL
+                     216 LOAD_DEREF              62 (tk)
+                     218 LOAD_ATTR               26 (Tk)
+                     228 PRECALL                  0
+                     232 CALL                     0
+                     242 STORE_DEREF             56 (root)
+         
+         179         244 LOAD_DEREF              56 (root)
+                     246 LOAD_METHOD             27 (winfo_screenheight)
+                     268 PRECALL                  0
+                     272 CALL                     0
+                     282 STORE_FAST              15 (screen_height)
+         
+         180         284 LOAD_DEREF              56 (root)
+                     286 LOAD_METHOD             28 (winfo_screenwidth)
+                     308 PRECALL                  0
+                     312 CALL                     0
+                     322 STORE_FAST              16 (screen_width)
+         
+         182         324 LOAD_CONST               8 ('Dimensions: ')
+                     326 LOAD_FAST               16 (screen_width)
+                     328 FORMAT_VALUE             0
+                     330 LOAD_CONST               9 (' x ')
+                     332 LOAD_FAST               15 (screen_height)
+                     334 FORMAT_VALUE             0
+                     336 BUILD_STRING             4
+                     338 STORE_FAST              17 (dimensions)
+         
+         183         340 LOAD_FAST               15 (screen_height)
+                     342 LOAD_CONST              10 (25)
+                     344 BINARY_OP                2 (//)
+                     348 STORE_FAST              18 (position)
+         
+         184         350 LOAD_CONST              11 (10)
+                     352 STORE_DEREF             57 (runcount)
+         
+         185         354 LOAD_CONST              12 ('We all have our favourites, but this task has been run too many times. \n\nPlease select another task to enjoy.')
+                     356 STORE_DEREF             53 (errortext)
+         
+         187         358 LOAD_GLOBAL             59 (NULL + glob)
+                     370 LOAD_ATTR               29 (glob)
+                     380 LOAD_GLOBAL             60 (folder_name)
+                     392 LOAD_CONST              13 ('/*Consent.txt')
+                     394 BINARY_OP                0 (+)
+                     398 PRECALL                  1
+                     402 CALL                     1
+                     412 EXTENDED_ARG             4
+                     414 POP_JUMP_FORWARD_IF_FALSE  1205 (to 2826)
+         
+         189         416 LOAD_DEREF              58 (spwf)
+                     418 LOAD_ATTR               31 (emailadd)
+                     428 STORE_FAST              19 (USERNAME)
+         
+         190         430 LOAD_DEREF              58 (spwf)
+                     432 LOAD_ATTR               32 (password)
+                     442 STORE_FAST              20 (PASSWORD)
+         
+         192         444 LOAD_CLOSURE            51 (Mail)
+                     446 LOAD_CLOSURE            52 (SendGridAPIClient)
+                     448 LOAD_CLOSURE            58 (spwf)
+                     450 LOAD_CLOSURE            62 (tk)
+                     452 BUILD_TUPLE              4
+                     454 LOAD_CONST              14 (<code object emailsupport, file "H:\Task Development\Stimuli\Task\Task.py", line 192>)
+                     456 MAKE_FUNCTION            8 (closure)
+                     458 STORE_FAST              21 (emailsupport)
+         
+         221         460 LOAD_CLOSURE            53 (errortext)
+                     462 LOAD_CLOSURE            54 (messagebox)
+                     464 LOAD_CLOSURE            55 (python_path)
+                     466 LOAD_CLOSURE            57 (runcount)
+                     468 LOAD_CLOSURE            59 (subprocess)
+                     470 BUILD_TUPLE              5
+                     472 LOAD_CONST              15 (<code object pis, file "H:\Task Development\Stimuli\Task\Task.py", line 221>)
+                     474 MAKE_FUNCTION            8 (closure)
+                     476 STORE_FAST              22 (pis)
+         
+         229         478 LOAD_CONST              16 (('Helvetica', 18))
+                     480 STORE_FAST              23 (fontsize)
+         
+         230         482 LOAD_CONST              17 (('Helvetica', 22))
+                     484 STORE_FAST              24 (fontsize1)
+         
+         231         486 LOAD_CONST              18 (('Helvetica', 12))
+                     488 STORE_FAST              25 (fontsize2)
+         
+         232         490 LOAD_CONST              18 (('Helvetica', 12))
+                     492 STORE_FAST              26 (fontsizesmall)
+         
+         234         494 LOAD_DEREF              56 (root)
+                     496 LOAD_METHOD             33 (attributes)
+                     518 LOAD_CONST              19 ('-fullscreen')
+                     520 LOAD_CONST              20 (True)
+                     522 PRECALL                  2
+                     526 CALL                     2
+                     536 POP_TOP
+         
+         235         538 LOAD_DEREF              56 (root)
+                     540 LOAD_METHOD             33 (attributes)
+                     562 LOAD_CONST              21 ('-topmost')
+                     564 LOAD_CONST              22 (False)
+                     566 PRECALL                  2
+                     570 CALL                     2
+                     580 POP_TOP
+         
+         237         582 LOAD_CLOSURE            56 (root)
+                     584 BUILD_TUPLE              1
+                     586 LOAD_CONST              23 (<code object exit_program, file "H:\Task Development\Stimuli\Task\Task.py", line 237>)
+                     588 MAKE_FUNCTION            8 (closure)
+                     590 STORE_FAST              27 (exit_program)
+         
+         240         592 PUSH_NULL
+                     594 LOAD_DEREF              62 (tk)
+                     596 LOAD_ATTR               34 (Button)
+                     606 LOAD_DEREF              56 (root)
+                     608 LOAD_CONST              24 ('Exit')
+                     610 LOAD_FAST               27 (exit_program)
+                     612 LOAD_FAST               26 (fontsizesmall)
+                     614 KW_NAMES                25
+                     616 PRECALL                  4
+                     620 CALL                     4
+                     630 STORE_FAST              28 (exit_button)
+         
+         241         632 LOAD_FAST               28 (exit_button)
+                     634 LOAD_METHOD             35 (pack)
+                     656 LOAD_CONST              26 ('top')
+                     658 LOAD_CONST              27 ('ne')
+                     660 LOAD_CONST              11 (10)
+                     662 LOAD_CONST              28 (5)
+                     664 KW_NAMES                29
+                     666 PRECALL                  4
+                     670 CALL                     4
+                     680 POP_TOP
+         
+         243         682 PUSH_NULL
+                     684 LOAD_DEREF              62 (tk)
+                     686 LOAD_ATTR               36 (Label)
+                     696 LOAD_DEREF              56 (root)
+                     698 LOAD_CONST              30 ('')
+                     700 LOAD_FAST               23 (fontsize)
+                     702 KW_NAMES                31
+                     704 PRECALL                  3
+                     708 CALL                     3
+                     718 STORE_DEREF             61 (time_label)
+         
+         245         720 LOAD_CLOSURE            60 (time)
+                     722 LOAD_CLOSURE            61 (time_label)
+                     724 LOAD_CLOSURE            63 (update_time)
+                     726 BUILD_TUPLE              3
+                     728 LOAD_CONST              32 (<code object update_time, file "H:\Task Development\Stimuli\Task\Task.py", line 245>)
+                     730 MAKE_FUNCTION            8 (closure)
+                     732 STORE_DEREF             63 (update_time)
+         
+         250         734 LOAD_DEREF              61 (time_label)
+                     736 LOAD_METHOD             35 (pack)
+                     758 LOAD_DEREF              62 (tk)
+                     760 LOAD_ATTR               37 (TOP)
+                     770 LOAD_CONST              33 (20)
+                     772 LOAD_CONST               1 (0)
+                     774 LOAD_CONST              34 ('nw')
+                     776 KW_NAMES                35
+                     778 PRECALL                  4
+                     782 CALL                     4
+                     792 POP_TOP
+         
+         252         794 PUSH_NULL
+                     796 LOAD_DEREF              62 (tk)
+                     798 LOAD_ATTR               38 (Frame)
+                     808 LOAD_DEREF              56 (root)
+                     810 PRECALL                  1
+                     814 CALL                     1
+                     824 STORE_FAST              29 (welcome_frame)
+         
+         253         826 LOAD_FAST               29 (welcome_frame)
+                     828 LOAD_METHOD             35 (pack)
+                     850 LOAD_DEREF              62 (tk)
+                     852 LOAD_ATTR               37 (TOP)
+                     862 LOAD_DEREF              62 (tk)
+                     864 LOAD_ATTR               39 (X)
+                     874 KW_NAMES                36
+                     876 PRECALL                  2
+                     880 CALL                     2
+                     890 POP_TOP
+         
+         255         892 PUSH_NULL
+                     894 LOAD_DEREF              62 (tk)
+                     896 LOAD_ATTR               36 (Label)
+                     906 LOAD_FAST               29 (welcome_frame)
+                     908 LOAD_CONST              37 ('Welcome back!')
+                     910 LOAD_FAST               24 (fontsize1)
+                     912 KW_NAMES                31
+                     914 PRECALL                  3
+                     918 CALL                     3
+                     928 STORE_FAST              30 (welcome_label)
+         
+         256         930 LOAD_FAST               30 (welcome_label)
+                     932 LOAD_METHOD             35 (pack)
+                     954 LOAD_FAST               18 (position)
+                     956 KW_NAMES                38
+                     958 PRECALL                  1
+                     962 CALL                     1
+                     972 POP_TOP
+         
+         258         974 PUSH_NULL
+                     976 LOAD_DEREF              62 (tk)
+                     978 LOAD_ATTR               38 (Frame)
+                     988 LOAD_DEREF              56 (root)
+                     990 PRECALL                  1
+                     994 CALL                     1
+                    1004 STORE_FAST              31 (text_frame)
+         
+         259        1006 LOAD_FAST               31 (text_frame)
+                    1008 LOAD_METHOD             35 (pack)
+                    1030 LOAD_DEREF              62 (tk)
+                    1032 LOAD_ATTR               37 (TOP)
+                    1042 LOAD_DEREF              62 (tk)
+                    1044 LOAD_ATTR               39 (X)
+                    1054 KW_NAMES                36
+                    1056 PRECALL                  2
+                    1060 CALL                     2
+                    1070 POP_TOP
+         
+         261        1072 PUSH_NULL
+                    1074 LOAD_DEREF              62 (tk)
+                    1076 LOAD_ATTR               36 (Label)
+                    1086 LOAD_FAST               29 (welcome_frame)
+                    1088 LOAD_CONST              39 ('Please now select a task to perform')
+                    1090 LOAD_FAST               23 (fontsize)
+                    1092 KW_NAMES                31
+                    1094 PRECALL                  3
+                    1098 CALL                     3
+                    1108 STORE_FAST              32 (text_label)
+         
+         262        1110 LOAD_FAST               32 (text_label)
+                    1112 LOAD_METHOD             35 (pack)
+                    1134 LOAD_FAST               18 (position)
+                    1136 KW_NAMES                38
+                    1138 PRECALL                  1
+                    1142 CALL                     1
+                    1152 POP_TOP
+         
+         264        1154 PUSH_NULL
+                    1156 LOAD_DEREF              62 (tk)
+                    1158 LOAD_ATTR               38 (Frame)
+                    1168 LOAD_DEREF              56 (root)
+                    1170 PRECALL                  1
+                    1174 CALL                     1
+                    1184 STORE_FAST              33 (nback_frame)
+         
+         265        1186 LOAD_FAST               33 (nback_frame)
+                    1188 LOAD_METHOD             35 (pack)
+                    1210 LOAD_DEREF              62 (tk)
+                    1212 LOAD_ATTR               37 (TOP)
+                    1222 LOAD_CONST              40 (30)
+                    1224 LOAD_CONST              28 (5)
+                    1226 LOAD_CONST              41 ('center')
+                    1228 KW_NAMES                35
+                    1230 PRECALL                  4
+                    1234 CALL                     4
+                    1244 POP_TOP
+         
+         267        1246 LOAD_CLOSURE            53 (errortext)
+                    1248 LOAD_CLOSURE            54 (messagebox)
+                    1250 LOAD_CLOSURE            55 (python_path)
+                    1252 LOAD_CLOSURE            57 (runcount)
+                    1254 LOAD_CLOSURE            59 (subprocess)
+                    1256 BUILD_TUPLE              5
+                    1258 LOAD_CONST              42 (<code object nbrun, file "H:\Task Development\Stimuli\Task\Task.py", line 267>)
+                    1260 MAKE_FUNCTION            8 (closure)
+                    1262 STORE_FAST              34 (nbrun)
+         
+         277        1264 PUSH_NULL
+                    1266 LOAD_DEREF              62 (tk)
+                    1268 LOAD_ATTR               34 (Button)
+                    1278 LOAD_FAST               33 (nback_frame)
+                    1280 LOAD_CONST              43 ('N-Back')
+                    1282 LOAD_FAST               34 (nbrun)
+                    1284 LOAD_FAST               23 (fontsize)
+                    1286 LOAD_CONST              41 ('center')
+                    1288 KW_NAMES                44
+                    1290 PRECALL                  5
+                    1294 CALL                     5
+                    1304 STORE_FAST              35 (nback)
+         
+         278        1306 LOAD_FAST               35 (nback)
+                    1308 LOAD_METHOD             35 (pack)
+                    1330 LOAD_DEREF              62 (tk)
+                    1332 LOAD_ATTR               37 (TOP)
+                    1342 LOAD_CONST              28 (5)
+                    1344 KW_NAMES                45
+                    1346 PRECALL                  2
+                    1350 CALL                     2
+                    1360 POP_TOP
+         
+         280        1362 LOAD_GLOBAL             80 (nbcount)
+                    1374 LOAD_CONST              46 (1)
+                    1376 COMPARE_OP               2 (==)
+                    1382 POP_JUMP_FORWARD_IF_FALSE    12 (to 1408)
+         
+         281        1384 LOAD_CONST              47 ('You have completed this ')
+                    1386 LOAD_GLOBAL             80 (nbcount)
+                    1398 FORMAT_VALUE             0
+                    1400 LOAD_CONST              48 (' time so far')
+                    1402 BUILD_STRING             3
+                    1404 STORE_FAST              36 (text)
+                    1406 JUMP_FORWARD            11 (to 1430)
+         
+         283     >> 1408 LOAD_CONST              47 ('You have completed this ')
+                    1410 LOAD_GLOBAL             80 (nbcount)
+                    1422 FORMAT_VALUE             0
+                    1424 LOAD_CONST              49 (' times so far')
+                    1426 BUILD_STRING             3
+                    1428 STORE_FAST              36 (text)
+         
+         284     >> 1430 PUSH_NULL
+                    1432 LOAD_DEREF              62 (tk)
+                    1434 LOAD_ATTR               36 (Label)
+                    1444 LOAD_FAST               33 (nback_frame)
+                    1446 LOAD_FAST               36 (text)
+                    1448 LOAD_FAST               25 (fontsize2)
+                    1450 KW_NAMES                31
+                    1452 PRECALL                  3
+                    1456 CALL                     3
+                    1466 STORE_FAST              37 (nback_label)
+         
+         285        1468 LOAD_FAST               37 (nback_label)
+                    1470 LOAD_METHOD             35 (pack)
+                    1492 LOAD_DEREF              62 (tk)
+                    1494 LOAD_ATTR               37 (TOP)
+                    1504 LOAD_CONST              28 (5)
+                    1506 LOAD_CONST              41 ('center')
+                    1508 KW_NAMES                50
+                    1510 PRECALL                  3
+                    1514 CALL                     3
+                    1524 POP_TOP
+         
+         288        1526 PUSH_NULL
+                    1528 LOAD_DEREF              62 (tk)
+                    1530 LOAD_ATTR               38 (Frame)
+                    1540 LOAD_DEREF              56 (root)
+                    1542 PRECALL                  1
+                    1546 CALL                     1
+                    1556 STORE_FAST              38 (button1_frame)
+         
+         289        1558 LOAD_FAST               38 (button1_frame)
+                    1560 LOAD_METHOD             35 (pack)
+                    1582 LOAD_DEREF              62 (tk)
+                    1584 LOAD_ATTR               37 (TOP)
+                    1594 LOAD_CONST              40 (30)
+                    1596 LOAD_CONST              28 (5)
+                    1598 LOAD_CONST              41 ('center')
+                    1600 KW_NAMES                35
+                    1602 PRECALL                  4
+                    1606 CALL                     4
+                    1616 POP_TOP
+         
+         291        1618 PUSH_NULL
+                    1620 LOAD_DEREF              62 (tk)
+                    1622 LOAD_ATTR               38 (Frame)
+                    1632 LOAD_DEREF              56 (root)
+                    1634 PRECALL                  1
+                    1638 CALL                     1
+                    1648 STORE_FAST              39 (button2_frame)
+         
+         292        1650 LOAD_FAST               39 (button2_frame)
+                    1652 LOAD_METHOD             35 (pack)
+                    1674 LOAD_DEREF              62 (tk)
+                    1676 LOAD_ATTR               37 (TOP)
+                    1686 LOAD_CONST              40 (30)
+                    1688 LOAD_CONST              28 (5)
+                    1690 LOAD_CONST              41 ('center')
+                    1692 KW_NAMES                35
+                    1694 PRECALL                  4
+                    1698 CALL                     4
+                    1708 POP_TOP
+         
+         294        1710 PUSH_NULL
+                    1712 LOAD_DEREF              62 (tk)
+                    1714 LOAD_ATTR               34 (Button)
+                    1724 LOAD_FAST               39 (button2_frame)
+                    1726 LOAD_CONST              51 ('Switching Task')
+                    1728 LOAD_FAST               22 (pis)
+                    1730 LOAD_FAST               23 (fontsize)
+                    1732 LOAD_CONST              41 ('center')
+                    1734 KW_NAMES                44
+                    1736 PRECALL                  5
+                    1740 CALL                     5
+                    1750 STORE_FAST              40 (button2)
+         
+         295        1752 LOAD_FAST               40 (button2)
+                    1754 LOAD_METHOD             35 (pack)
+                    1776 LOAD_DEREF              62 (tk)
+                    1778 LOAD_ATTR               37 (TOP)
+                    1788 LOAD_CONST              28 (5)
+                    1790 KW_NAMES                45
+                    1792 PRECALL                  2
+                    1796 CALL                     2
+                    1806 POP_TOP
+         
+         297        1808 LOAD_GLOBAL             82 (scount)
+                    1820 LOAD_CONST              46 (1)
+                    1822 COMPARE_OP               2 (==)
+                    1828 POP_JUMP_FORWARD_IF_FALSE    12 (to 1854)
+         
+         298        1830 LOAD_CONST              47 ('You have completed this ')
+                    1832 LOAD_GLOBAL             82 (scount)
+                    1844 FORMAT_VALUE             0
+                    1846 LOAD_CONST              48 (' time so far')
+                    1848 BUILD_STRING             3
+                    1850 STORE_FAST              36 (text)
+                    1852 JUMP_FORWARD            11 (to 1876)
+         
+         300     >> 1854 LOAD_CONST              47 ('You have completed this ')
+                    1856 LOAD_GLOBAL             82 (scount)
+                    1868 FORMAT_VALUE             0
+                    1870 LOAD_CONST              49 (' times so far')
+                    1872 BUILD_STRING             3
+                    1874 STORE_FAST              36 (text)
+         
+         301     >> 1876 PUSH_NULL
+                    1878 LOAD_DEREF              62 (tk)
+                    1880 LOAD_ATTR               36 (Label)
+                    1890 LOAD_FAST               39 (button2_frame)
+                    1892 LOAD_FAST               36 (text)
+                    1894 LOAD_FAST               25 (fontsize2)
+                    1896 KW_NAMES                31
+                    1898 PRECALL                  3
+                    1902 CALL                     3
+                    1912 STORE_FAST              41 (button2_label)
+         
+         302        1914 LOAD_FAST               41 (button2_label)
+                    1916 LOAD_METHOD             35 (pack)
+                    1938 LOAD_DEREF              62 (tk)
+                    1940 LOAD_ATTR               37 (TOP)
+                    1950 LOAD_CONST              28 (5)
+                    1952 KW_NAMES                45
+                    1954 PRECALL                  2
+                    1958 CALL                     2
+                    1968 POP_TOP
+         
+         304        1970 LOAD_CLOSURE            53 (errortext)
+                    1972 LOAD_CLOSURE            54 (messagebox)
+                    1974 LOAD_CLOSURE            55 (python_path)
+                    1976 LOAD_CLOSURE            57 (runcount)
+                    1978 LOAD_CLOSURE            59 (subprocess)
+                    1980 BUILD_TUPLE              5
+                    1982 LOAD_CONST              52 (<code object consent, file "H:\Task Development\Stimuli\Task\Task.py", line 304>)
+                    1984 MAKE_FUNCTION            8 (closure)
+                    1986 STORE_FAST              42 (consent)
+         
+         314        1988 PUSH_NULL
+                    1990 LOAD_DEREF              62 (tk)
+                    1992 LOAD_ATTR               38 (Frame)
+                    2002 LOAD_DEREF              56 (root)
+                    2004 PRECALL                  1
+                    2008 CALL                     1
+                    2018 STORE_FAST              43 (button3_frame)
+         
+         315        2020 LOAD_FAST               43 (button3_frame)
+                    2022 LOAD_METHOD             35 (pack)
+                    2044 LOAD_DEREF              62 (tk)
+                    2046 LOAD_ATTR               37 (TOP)
+                    2056 LOAD_CONST              40 (30)
+                    2058 LOAD_CONST              11 (10)
+                    2060 LOAD_CONST              41 ('center')
+                    2062 KW_NAMES                35
+                    2064 PRECALL                  4
+                    2068 CALL                     4
+                    2078 POP_TOP
+         
+         316        2080 PUSH_NULL
+                    2082 LOAD_DEREF              62 (tk)
+                    2084 LOAD_ATTR               34 (Button)
+                    2094 LOAD_FAST               43 (button3_frame)
+                    2096 LOAD_CONST              53 ('2-Type Reaction Time')
+                    2098 LOAD_FAST               42 (consent)
+                    2100 LOAD_FAST               23 (fontsize)
+                    2102 LOAD_CONST              41 ('center')
+                    2104 KW_NAMES                44
+                    2106 PRECALL                  5
+                    2110 CALL                     5
+                    2120 STORE_FAST              44 (button3)
+         
+         317        2122 LOAD_FAST               44 (button3)
+                    2124 LOAD_METHOD             35 (pack)
+                    2146 LOAD_DEREF              62 (tk)
+                    2148 LOAD_ATTR               37 (TOP)
+                    2158 LOAD_CONST              28 (5)
+                    2160 KW_NAMES                45
+                    2162 PRECALL                  2
+                    2166 CALL                     2
+                    2176 POP_TOP
+         
+         319        2178 LOAD_GLOBAL             84 (rtcount)
+                    2190 LOAD_CONST              46 (1)
+                    2192 COMPARE_OP               2 (==)
+                    2198 POP_JUMP_FORWARD_IF_FALSE    12 (to 2224)
+         
+         320        2200 LOAD_CONST              47 ('You have completed this ')
+                    2202 LOAD_GLOBAL             84 (rtcount)
+                    2214 FORMAT_VALUE             0
+                    2216 LOAD_CONST              48 (' time so far')
+                    2218 BUILD_STRING             3
+                    2220 STORE_FAST              36 (text)
+                    2222 JUMP_FORWARD            11 (to 2246)
+         
+         322     >> 2224 LOAD_CONST              47 ('You have completed this ')
+                    2226 LOAD_GLOBAL             84 (rtcount)
+                    2238 FORMAT_VALUE             0
+                    2240 LOAD_CONST              49 (' times so far')
+                    2242 BUILD_STRING             3
+                    2244 STORE_FAST              36 (text)
+         
+         323     >> 2246 PUSH_NULL
+                    2248 LOAD_DEREF              62 (tk)
+                    2250 LOAD_ATTR               36 (Label)
+                    2260 LOAD_FAST               43 (button3_frame)
+                    2262 LOAD_FAST               36 (text)
+                    2264 LOAD_FAST               25 (fontsize2)
+                    2266 KW_NAMES                31
+                    2268 PRECALL                  3
+                    2272 CALL                     3
+                    2282 STORE_FAST              45 (button3_label)
+         
+         324        2284 LOAD_FAST               45 (button3_label)
+                    2286 LOAD_METHOD             35 (pack)
+                    2308 LOAD_DEREF              62 (tk)
+                    2310 LOAD_ATTR               37 (TOP)
+                    2320 LOAD_CONST              28 (5)
+                    2322 LOAD_CONST              41 ('center')
+                    2324 KW_NAMES                50
+                    2326 PRECALL                  3
+                    2330 CALL                     3
+                    2340 POP_TOP
+         
+         326        2342 PUSH_NULL
+                    2344 LOAD_DEREF              62 (tk)
+                    2346 LOAD_ATTR               38 (Frame)
+                    2356 LOAD_DEREF              56 (root)
+                    2358 PRECALL                  1
+                    2362 CALL                     1
+                    2372 STORE_FAST              46 (button12_frame)
+         
+         327        2374 LOAD_FAST               46 (button12_frame)
+                    2376 LOAD_METHOD             35 (pack)
+                    2398 LOAD_DEREF              62 (tk)
+                    2400 LOAD_ATTR               43 (BOTTOM)
+                    2410 LOAD_CONST              40 (30)
+                    2412 LOAD_CONST              33 (20)
+                    2414 LOAD_CONST              54 ('sw')
+                    2416 KW_NAMES                35
+                    2418 PRECALL                  4
+                    2422 CALL                     4
+                    2432 POP_TOP
+         
+         329        2434 PUSH_NULL
+                    2436 LOAD_DEREF              62 (tk)
+                    2438 LOAD_ATTR               34 (Button)
+                    2448 LOAD_FAST               46 (button12_frame)
+                    2450 LOAD_CONST              55 ('Email for assistance or queries')
+                    2452 LOAD_FAST               21 (emailsupport)
+                    2454 LOAD_FAST               23 (fontsize)
+                    2456 KW_NAMES                25
+                    2458 PRECALL                  4
+                    2462 CALL                     4
+                    2472 STORE_FAST              47 (button12)
+         
+         330        2474 LOAD_FAST               47 (button12)
+                    2476 LOAD_METHOD             35 (pack)
+                    2498 LOAD_DEREF              62 (tk)
+                    2500 LOAD_ATTR               44 (LEFT)
+                    2510 LOAD_CONST              11 (10)
+                    2512 KW_NAMES                45
+                    2514 PRECALL                  2
+                    2518 CALL                     2
+                    2528 POP_TOP
+         
+         332        2530 PUSH_NULL
+                    2532 LOAD_FAST                4 (Image)
+                    2534 LOAD_ATTR               45 (open)
+                    2544 LOAD_CONST              56 ('uop.png')
+                    2546 PRECALL                  1
+                    2550 CALL                     1
+                    2560 STORE_FAST              48 (image_file)
+         
+         333        2562 PUSH_NULL
+                    2564 LOAD_FAST                5 (ImageTk)
+                    2566 LOAD_ATTR               46 (PhotoImage)
+                    2576 LOAD_FAST               48 (image_file)
+                    2578 PRECALL                  1
+                    2582 CALL                     1
+                    2592 STORE_FAST              49 (image2)
+         
+         334        2594 PUSH_NULL
+                    2596 LOAD_DEREF              62 (tk)
+                    2598 LOAD_ATTR               36 (Label)
+                    2608 LOAD_DEREF              56 (root)
+                    2610 LOAD_FAST               49 (image2)
+                    2612 KW_NAMES                57
+                    2614 PRECALL                  2
+                    2618 CALL                     2
+                    2628 STORE_FAST              50 (image_label)
+         
+         335        2630 LOAD_FAST               50 (image_label)
+                    2632 LOAD_METHOD             47 (place)
+                    2654 LOAD_CONST              46 (1)
+                    2656 LOAD_CONST               1 (0)
+                    2658 LOAD_CONST              27 ('ne')
+                    2660 LOAD_CONST              58 (-20)
+                    2662 LOAD_CONST              59 (40)
+                    2664 KW_NAMES                60
+                    2666 PRECALL                  5
+                    2670 CALL                     5
+                    2680 POP_TOP
+         
+         336        2682 PUSH_NULL
+                    2684 LOAD_DEREF              63 (update_time)
+                    2686 PRECALL                  0
+                    2690 CALL                     0
+                    2700 POP_TOP
+         
+         338        2702 PUSH_NULL
+                    2704 LOAD_DEREF              59 (subprocess)
+                    2706 LOAD_ATTR               48 (run)
+                    2716 LOAD_DEREF              55 (python_path)
+                    2718 LOAD_CONST              61 ('Export.py')
+                    2720 BUILD_LIST               2
+                    2722 LOAD_CONST              20 (True)
+                    2724 KW_NAMES                62
+                    2726 PRECALL                  2
+                    2730 CALL                     2
+                    2740 POP_TOP
+         
+         340        2742 LOAD_DEREF              56 (root)
+                    2744 LOAD_METHOD             49 (mainloop)
+                    2766 PRECALL                  0
+                    2770 CALL                     0
+                    2780 POP_TOP
+         
+         342        2782 LOAD_DEREF              56 (root)
+                    2784 LOAD_METHOD             50 (quit)
+                    2806 PRECALL                  0
+                    2810 CALL                     0
+                    2820 POP_TOP
+                    2822 LOAD_CONST               0 (None)
+                    2824 RETURN_VALUE
+         
+         347     >> 2826 PUSH_NULL
+                    2828 LOAD_DEREF              59 (subprocess)
+                    2830 LOAD_ATTR               48 (run)
+                    2840 LOAD_DEREF              55 (python_path)
+                    2842 LOAD_CONST              61 ('Export.py')
+                    2844 BUILD_LIST               2
+                    2846 LOAD_CONST              20 (True)
+                    2848 KW_NAMES                62
+                    2850 PRECALL                  2
+                    2854 CALL                     2
+                    2864 POP_TOP
+         
+         348        2866 PUSH_NULL
+                    2868 LOAD_DEREF              59 (subprocess)
+                    2870 LOAD_ATTR               48 (run)
+                    2880 LOAD_DEREF              55 (python_path)
+                    2882 LOAD_GLOBAL            102 (file_path)
+                    2894 BUILD_LIST               2
+                    2896 LOAD_CONST              20 (True)
+                    2898 KW_NAMES                62
+                    2900 PRECALL                  2
+                    2904 CALL                     2
+                    2914 POP_TOP
+                    2916 LOAD_CONST               0 (None)
+                    2918 RETURN_VALUE
          consts
             None
+            0
+            ('Image', 'ImageTk')
+            ('datetime',)
+            ('filedialog',)
+            ('simpledialog', 'messagebox')
+            ('SendGridAPIClient',)
+            ('Mail', 'Attachment', 'FileContent', 'FileName', 'FileType', 'Disposition')
             'Dimensions: '
             ' x '
             25
             10
             'We all have our favourites, but this task has been run too many times. \n\nPlease select another task to enjoy.'
             '/*Consent.txt'
             code
                argcount  : 0
                nlocals   : 2
                stacksize : 7
                flags     : 19
                code
-                  0x95018702870397007401000000000000000000006a0100000000000000
-                  00a6000000ab0000000000000000008a038903a002000000000000000000
-                  00000000000000000000006401a6010000ab010000000000000000010074
-                  01000000000000000000006a03000000000000000089036402ac03a60200
-                  00ab0200000000000000007d007c00a00400000000000000000000000000
-                  000000000000007400000000000000000000006a05000000000000000064
-                  046404ac05a6030000ab0300000000000000000100740100000000000000
-                  0000006a06000000000000000089037400000000000000000000006a0700
-                  00000000000000ac06a6020000ab0200000000000000008a028902a00400
-                  000000000000000000000000000000000000007400000000000000000000
-                  006a05000000000000000064046404ac05a6030000ab0300000000000000
-                  0001007401000000000000000000006a0800000000000000008903640788
-                  0288038804660364088408ac09a6030000ab0300000000000000007d017c
-                  01a004000000000000000000000000000000000000000074000000000000
-                  00000000006a05000000000000000064046404ac05a6030000ab03000000
-                  0000000000010064005300
-                             0 COPY_FREE_VARS           1
+                  0x95048702870387049700020089086a000000000000000000a6000000ab
+                  0000000000000000008a038903a001000000000000000000000000000000
+                  00000000006401a6010000ab0100000000000000000100020089086a0200
+                  0000000000000089036402ac03a6020000ab0200000000000000007d007c
+                  00a00300000000000000000000000000000000000000006404640589086a
+                  04000000000000000064066406ac07a6050000ab05000000000000000001
+                  00020089086a050000000000000000890389086a060000000000000000ac
+                  08a6020000ab0200000000000000008a028902a003000000000000000000
+                  00000000000000000000006404640589086a040000000000000000640664
+                  06ac07a6050000ab05000000000000000001008805880688038807660464
+                  0984088a04020089086a0700000000000000008903640a88028804880866
+                  03640b8408ac0ca6030000ab0300000000000000007d017c01a003000000
+                  0000000000000000000000000000000000640589086a0400000000000000
+                  0064066406ac0da6040000ab040000000000000000010064005300
+                             0 COPY_FREE_VARS           4
                              2 MAKE_CELL                2 (body_text)
                              4 MAKE_CELL                3 (email_window)
+                             6 MAKE_CELL                4 (send_email)
                
-               172           6 RESUME                   0
+               192           8 RESUME                   0
                
-               173           8 LOAD_GLOBAL              1 (NULL + tk)
-                            20 LOAD_ATTR                1 (Toplevel)
-                            30 PRECALL                  0
-                            34 CALL                     0
-                            44 STORE_DEREF              3 (email_window)
-               
-               174          46 LOAD_DEREF               3 (email_window)
-                            48 LOAD_METHOD              2 (title)
-                            70 LOAD_CONST               1 ('Compose Email')
-                            72 PRECALL                  1
-                            76 CALL                     1
-                            86 POP_TOP
-               
-               175          88 LOAD_GLOBAL              1 (NULL + tk)
-                           100 LOAD_ATTR                3 (Label)
-                           110 LOAD_DEREF               3 (email_window)
-                           112 LOAD_CONST               2 ('Please describe your issue/query in as much detail as possible \n\nThis will be reviewed as soon as possible, and support will be provided')
-                           114 KW_NAMES                 3
-                           116 PRECALL                  2
-                           120 CALL                     2
-                           130 STORE_FAST               0 (body_label)
-               
-               176         132 LOAD_FAST                0 (body_label)
-                           134 LOAD_METHOD              4 (pack)
-                           156 LOAD_GLOBAL              0 (tk)
-                           168 LOAD_ATTR                5 (TOP)
-                           178 LOAD_CONST               4 (5)
-                           180 LOAD_CONST               4 (5)
-                           182 KW_NAMES                 5
-                           184 PRECALL                  3
-                           188 CALL                     3
-                           198 POP_TOP
-               
-               177         200 LOAD_GLOBAL              1 (NULL + tk)
-                           212 LOAD_ATTR                6 (Text)
-                           222 LOAD_DEREF               3 (email_window)
-                           224 LOAD_GLOBAL              0 (tk)
-                           236 LOAD_ATTR                7 (WORD)
-                           246 KW_NAMES                 6
-                           248 PRECALL                  2
-                           252 CALL                     2
-                           262 STORE_DEREF              2 (body_text)
-               
-               178         264 LOAD_DEREF               2 (body_text)
-                           266 LOAD_METHOD              4 (pack)
-                           288 LOAD_GLOBAL              0 (tk)
-                           300 LOAD_ATTR                5 (TOP)
-                           310 LOAD_CONST               4 (5)
-                           312 LOAD_CONST               4 (5)
-                           314 KW_NAMES                 5
-                           316 PRECALL                  3
-                           320 CALL                     3
-                           330 POP_TOP
-               
-               179         332 LOAD_GLOBAL              1 (NULL + tk)
-                           344 LOAD_ATTR                8 (Button)
-                           354 LOAD_DEREF               3 (email_window)
-                           356 LOAD_CONST               7 ('Send')
-                           358 LOAD_CLOSURE             2 (body_text)
-                           360 LOAD_CLOSURE             3 (email_window)
-                           362 LOAD_CLOSURE             4 (send_email)
-                           364 BUILD_TUPLE              3
-                           366 LOAD_CONST               8 (<code object <lambda>, file "D:\Task Development\Stimuli\Task\Task.py", line 179>)
-                           368 MAKE_FUNCTION            8 (closure)
-                           370 KW_NAMES                 9
-                           372 PRECALL                  3
-                           376 CALL                     3
-                           386 STORE_FAST               1 (submit_button)
-               
-               180         388 LOAD_FAST                1 (submit_button)
-                           390 LOAD_METHOD              4 (pack)
-                           412 LOAD_GLOBAL              0 (tk)
-                           424 LOAD_ATTR                5 (TOP)
-                           434 LOAD_CONST               4 (5)
-                           436 LOAD_CONST               4 (5)
-                           438 KW_NAMES                 5
-                           440 PRECALL                  3
-                           444 CALL                     3
-                           454 POP_TOP
-                           456 LOAD_CONST               0 (None)
-                           458 RETURN_VALUE
+               193          10 PUSH_NULL
+                            12 LOAD_DEREF               8 (tk)
+                            14 LOAD_ATTR                0 (Toplevel)
+                            24 PRECALL                  0
+                            28 CALL                     0
+                            38 STORE_DEREF              3 (email_window)
+               
+               194          40 LOAD_DEREF               3 (email_window)
+                            42 LOAD_METHOD              1 (title)
+                            64 LOAD_CONST               1 ('Compose Email')
+                            66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+               
+               195          82 PUSH_NULL
+                            84 LOAD_DEREF               8 (tk)
+                            86 LOAD_ATTR                2 (Label)
+                            96 LOAD_DEREF               3 (email_window)
+                            98 LOAD_CONST               2 ('Please describe your issue/query in as much detail as possible')
+                           100 KW_NAMES                 3
+                           102 PRECALL                  2
+                           106 CALL                     2
+                           116 STORE_FAST               0 (body_label)
+               
+               196         118 LOAD_FAST                0 (body_label)
+                           120 LOAD_METHOD              3 (pack)
+                           142 LOAD_CONST               4 ('both')
+                           144 LOAD_CONST               5 (False)
+                           146 LOAD_DEREF               8 (tk)
+                           148 LOAD_ATTR                4 (TOP)
+                           158 LOAD_CONST               6 (5)
+                           160 LOAD_CONST               6 (5)
+                           162 KW_NAMES                 7
+                           164 PRECALL                  5
+                           168 CALL                     5
+                           178 POP_TOP
+               
+               197         180 PUSH_NULL
+                           182 LOAD_DEREF               8 (tk)
+                           184 LOAD_ATTR                5 (Text)
+                           194 LOAD_DEREF               3 (email_window)
+                           196 LOAD_DEREF               8 (tk)
+                           198 LOAD_ATTR                6 (WORD)
+                           208 KW_NAMES                 8
+                           210 PRECALL                  2
+                           214 CALL                     2
+                           224 STORE_DEREF              2 (body_text)
+               
+               198         226 LOAD_DEREF               2 (body_text)
+                           228 LOAD_METHOD              3 (pack)
+                           250 LOAD_CONST               4 ('both')
+                           252 LOAD_CONST               5 (False)
+                           254 LOAD_DEREF               8 (tk)
+                           256 LOAD_ATTR                4 (TOP)
+                           266 LOAD_CONST               6 (5)
+                           268 LOAD_CONST               6 (5)
+                           270 KW_NAMES                 7
+                           272 PRECALL                  5
+                           276 CALL                     5
+                           286 POP_TOP
+               
+               200         288 LOAD_CLOSURE             5 (Mail)
+                           290 LOAD_CLOSURE             6 (SendGridAPIClient)
+                           292 LOAD_CLOSURE             3 (email_window)
+                           294 LOAD_CLOSURE             7 (spwf)
+                           296 BUILD_TUPLE              4
+                           298 LOAD_CONST               9 (<code object send_email, file "H:\Task Development\Stimuli\Task\Task.py", line 200>)
+                           300 MAKE_FUNCTION            8 (closure)
+                           302 STORE_DEREF              4 (send_email)
+               
+               218         304 PUSH_NULL
+                           306 LOAD_DEREF               8 (tk)
+                           308 LOAD_ATTR                7 (Button)
+                           318 LOAD_DEREF               3 (email_window)
+                           320 LOAD_CONST              10 ('Send')
+                           322 LOAD_CLOSURE             2 (body_text)
+                           324 LOAD_CLOSURE             4 (send_email)
+                           326 LOAD_CLOSURE             8 (tk)
+                           328 BUILD_TUPLE              3
+                           330 LOAD_CONST              11 (<code object <lambda>, file "H:\Task Development\Stimuli\Task\Task.py", line 218>)
+                           332 MAKE_FUNCTION            8 (closure)
+                           334 KW_NAMES                12
+                           336 PRECALL                  3
+                           340 CALL                     3
+                           350 STORE_FAST               1 (submit_button)
+               
+               219         352 LOAD_FAST                1 (submit_button)
+                           354 LOAD_METHOD              3 (pack)
+                           376 LOAD_CONST               5 (False)
+                           378 LOAD_DEREF               8 (tk)
+                           380 LOAD_ATTR                4 (TOP)
+                           390 LOAD_CONST               6 (5)
+                           392 LOAD_CONST               6 (5)
+                           394 KW_NAMES                13
+                           396 PRECALL                  4
+                           400 CALL                     4
+                           410 POP_TOP
+                           412 LOAD_CONST               0 (None)
+                           414 RETURN_VALUE
                consts
                   None
                   'Compose Email'
-                  'Please describe your issue/query in as much detail as possible \n\nThis will be reviewed as soon as possible, and support will be provided'
+                  'Please describe your issue/query in as much detail as possible'
                   ('text',)
+                  'both'
+                  False
                   5
-                  ('side', 'padx', 'pady')
+                  ('fill', 'expand', 'side', 'padx', 'pady')
                   ('wrap',)
+                  code
+                     argcount  : 1
+                     nlocals   : 6
+                     stacksize : 8
+                     flags     : 19
+                     code
+                        0x950497000200890789096a000000000000000000ac01a6010000ab0100
+                        000000000000007d010200890689096a01000000000000000089096a0100
+                        00000000000000640289096a0200000000000000009b009d0264037c009b
+                        0064049d03ac05a6040000ab0400000000000000007d0209007c01a00300
+                        000000000000000000000000000000000000007c02a6010000ab01000000
+                        00000000007d038908a00400000000000000000000000000000000000000
+                        00a6000000ab00000000000000000001006e6f2300740a00000000000000
+                        000000240072627d04740d00000000000000000000740e00000000000000
+                        00000064067a000000a6010000ab01000000000000000035007d05741000
+                        000000000000000000a00900000000000000000000000000000000000000
+                        007c04a6010000ab0100000000000000000100640064006400a6020000ab
+                        02000000000000000001006e0b2300310073047702780359007701010059
+                        00010001007415000000000000000000007c04a6010000ab010000000000
+                        0000000100590064007d047e046e0864007d047e04770177007803590077
+                        018908a0040000000000000000000000000000000000000000a6000000ab
+                        000000000000000000010064005300
+                                   0 COPY_FREE_VARS           4
+                     
+                     200           2 RESUME                   0
+                     
+                     201           4 PUSH_NULL
+                                   6 LOAD_DEREF               7 (SendGridAPIClient)
+                                   8 LOAD_DEREF               9 (spwf)
+                                  10 LOAD_ATTR                0 (key)
+                                  20 KW_NAMES                 1
+                                  22 PRECALL                  1
+                                  26 CALL                     1
+                                  36 STORE_FAST               1 (sg)
+                     
+                     202          38 PUSH_NULL
+                                  40 LOAD_DEREF               6 (Mail)
+                     
+                     203          42 LOAD_DEREF               9 (spwf)
+                                  44 LOAD_ATTR                1 (output)
+                     
+                     204          54 LOAD_DEREF               9 (spwf)
+                                  56 LOAD_ATTR                1 (output)
+                     
+                     205          66 LOAD_CONST               2 ('Email from Participant ')
+                                  68 LOAD_DEREF               9 (spwf)
+                                  70 LOAD_ATTR                2 (participant_number)
+                                  80 FORMAT_VALUE             0
+                                  82 BUILD_STRING             2
+                     
+                     206          84 LOAD_CONST               3 ('<strong>')
+                                  86 LOAD_FAST                0 (body)
+                                  88 FORMAT_VALUE             0
+                                  90 LOAD_CONST               4 ('</strong>')
+                                  92 BUILD_STRING             3
+                     
+                     202          94 KW_NAMES                 5
+                                  96 PRECALL                  4
+                                 100 CALL                     4
+                                 110 STORE_FAST               2 (message)
+                     
+                     209         112 NOP
+                     
+                     210         114 LOAD_FAST                1 (sg)
+                                 116 LOAD_METHOD              3 (send)
+                                 138 LOAD_FAST                2 (message)
+                                 140 PRECALL                  1
+                                 144 CALL                     1
+                                 154 STORE_FAST               3 (response)
+                     
+                     211         156 LOAD_DEREF               8 (email_window)
+                                 158 LOAD_METHOD              4 (destroy)
+                                 180 PRECALL                  0
+                                 184 CALL                     0
+                                 194 POP_TOP
+                                 196 JUMP_FORWARD           111 (to 420)
+                             >>  198 PUSH_EXC_INFO
+                     
+                     212         200 LOAD_GLOBAL             10 (Exception)
+                                 212 CHECK_EXC_MATCH
+                                 214 POP_JUMP_FORWARD_IF_FALSE    98 (to 412)
+                                 216 STORE_FAST               4 (e)
+                     
+                     213         218 LOAD_GLOBAL             13 (NULL + open)
+                                 230 LOAD_GLOBAL             14 (folder_name)
+                                 242 LOAD_CONST               6 ('/Email Errors.txt')
+                                 244 BINARY_OP                0 (+)
+                                 248 PRECALL                  1
+                                 252 CALL                     1
+                                 262 BEFORE_WITH
+                                 264 STORE_FAST               5 (emailerror)
+                     
+                     214         266 LOAD_GLOBAL             16 (emailerrorr)
+                                 278 LOAD_METHOD              9 (write)
+                                 300 LOAD_FAST                4 (e)
+                                 302 PRECALL                  1
+                                 306 CALL                     1
+                                 316 POP_TOP
+                     
+                     213         318 LOAD_CONST               0 (None)
+                                 320 LOAD_CONST               0 (None)
+                                 322 LOAD_CONST               0 (None)
+                                 324 PRECALL                  2
+                                 328 CALL                     2
+                                 338 POP_TOP
+                                 340 JUMP_FORWARD            11 (to 364)
+                             >>  342 PUSH_EXC_INFO
+                                 344 WITH_EXCEPT_START
+                                 346 POP_JUMP_FORWARD_IF_TRUE     4 (to 356)
+                                 348 RERAISE                  2
+                             >>  350 COPY                     3
+                                 352 POP_EXCEPT
+                                 354 RERAISE                  1
+                             >>  356 POP_TOP
+                                 358 POP_EXCEPT
+                                 360 POP_TOP
+                                 362 POP_TOP
+                     
+                     215     >>  364 LOAD_GLOBAL             21 (NULL + print)
+                                 376 LOAD_FAST                4 (e)
+                                 378 PRECALL                  1
+                                 382 CALL                     1
+                                 392 POP_TOP
+                                 394 POP_EXCEPT
+                                 396 LOAD_CONST               0 (None)
+                                 398 STORE_FAST               4 (e)
+                                 400 DELETE_FAST              4 (e)
+                                 402 JUMP_FORWARD             8 (to 420)
+                             >>  404 LOAD_CONST               0 (None)
+                                 406 STORE_FAST               4 (e)
+                                 408 DELETE_FAST              4 (e)
+                                 410 RERAISE                  1
+                     
+                     212     >>  412 RERAISE                  0
+                             >>  414 COPY                     3
+                                 416 POP_EXCEPT
+                                 418 RERAISE                  1
+                     
+                     216     >>  420 LOAD_DEREF               8 (email_window)
+                                 422 LOAD_METHOD              4 (destroy)
+                                 444 PRECALL                  0
+                                 448 CALL                     0
+                                 458 POP_TOP
+                                 460 LOAD_CONST               0 (None)
+                                 462 RETURN_VALUE
+                     ExceptionTable:
+                       114 to 194 -> 198 [0]
+                       198 to 216 -> 414 [1] lasti
+                       218 to 262 -> 404 [1] lasti
+                       264 to 316 -> 342 [2] lasti
+                       318 to 340 -> 404 [1] lasti
+                       342 to 348 -> 350 [4] lasti
+                       350 to 354 -> 404 [1] lasti
+                       356 to 356 -> 350 [4] lasti
+                       358 to 392 -> 404 [1] lasti
+                       404 to 412 -> 414 [1] lasti
+                     consts
+                        None
+                        ('api_key',)
+                        'Email from Participant '
+                        '<strong>'
+                        '</strong>'
+                        ('from_email', 'to_emails', 'subject', 'html_content')
+                        '/Email Errors.txt'
+                     names      ('key', 'output', 'participant_number', 'send', 'destroy', 'Exception', 'open', 'folder_name', 'emailerrorr', 'write', 'print')
+                     varnames   ('body', 'sg', 'message', 'response', 'e', 'emailerror')
+                     freevars   ('Mail', 'SendGridAPIClient', 'email_window', 'spwf')
+                     cellvars   ()
+                     filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
+                     name       'send_email'
+                     firstlineno 200
+                     lnotab
+                        0x0401220104010c010c0112010afc120702012a012c011201300134ff2e
+                        0230fd0804
                   'Send'
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 6
                      flags     : 19
                      code
-                        0x95039700020089028900a0000000000000000000000000000000000000
-                        00000064017402000000000000000000006a020000000000000000a60200
-                        00ab0200000000000000008901a6020000ab0200000000000000005300
+                        0x95039700020089018900a0000000000000000000000000000000000000
+                        000000640189026a010000000000000000a6020000ab0200000000000000
+                        00a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           3
                      
-                     179           2 RESUME                   0
+                     218           2 RESUME                   0
                                    4 PUSH_NULL
-                                   6 LOAD_DEREF               2 (send_email)
+                                   6 LOAD_DEREF               1 (send_email)
                                    8 LOAD_DEREF               0 (body_text)
                                   10 LOAD_METHOD              0 (get)
                                   32 LOAD_CONST               1 ('1.0')
-                                  34 LOAD_GLOBAL              2 (tk)
-                                  46 LOAD_ATTR                2 (END)
-                                  56 PRECALL                  2
-                                  60 CALL                     2
-                                  70 LOAD_DEREF               1 (email_window)
-                                  72 PRECALL                  2
-                                  76 CALL                     2
-                                  86 RETURN_VALUE
+                                  34 LOAD_DEREF               2 (tk)
+                                  36 LOAD_ATTR                1 (END)
+                                  46 PRECALL                  2
+                                  50 CALL                     2
+                                  60 PRECALL                  1
+                                  64 CALL                     1
+                                  74 RETURN_VALUE
                      consts
                         None
                         '1.0'
-                     names      ('get', 'tk', 'END')
+                     names      ('get', 'END')
                      varnames   ()
-                     freevars   ('body_text', 'email_window', 'send_email')
+                     freevars   ('body_text', 'send_email', 'tk')
                      cellvars   ()
-                     filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+                     filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                      name       '<lambda>'
-                     firstlineno 179
+                     firstlineno 218
                      lnotab 0x
                   ('text', 'command')
-               names      ('tk', 'Toplevel', 'title', 'Label', 'pack', 'TOP', 'Text', 'WORD', 'Button')
+                  ('expand', 'side', 'padx', 'pady')
+               names      ('Toplevel', 'title', 'Label', 'pack', 'TOP', 'Text', 'WORD', 'Button')
                varnames   ('body_label', 'submit_button')
-               freevars   ('send_email',)
-               cellvars   ('body_text', 'email_window')
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               freevars   ('Mail', 'SendGridAPIClient', 'spwf', 'tk')
+               cellvars   ('body_text', 'email_window', 'send_email')
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       'emailsupport'
-               firstlineno 172
-               lnotab 0x080126012a012c014401400144013801
-            code
-               argcount  : 2
-               nlocals   : 9
-               stacksize : 8
-               flags     : 19
-               code
-                  0x9700640164006c007d02640164026c016d027d030100640164036c036d
-                  047d04010002007c04740a000000000000000000006a0600000000000000
-                  00740a000000000000000000006a0600000000000000006404740a000000
-                  000000000000006a0700000000000000009b009d0264057c009b0064069d
-                  03ac07a6040000ab0400000000000000007d0502007c03740a0000000000
-                  00000000006a080000000000000000ac08a6010000ab0100000000000000
-                  007d0609007c06a00900000000000000000000000000000000000000007c
-                  05a6010000ab0100000000000000007d0774150000000000000000000064
-                  097c076a0b00000000000000009b009d02a6010000ab0100000000000000
-                  0001007c01a00c0000000000000000000000000000000000000000a60000
-                  00ab0000000000000000000100640053002300741a000000000000000000
-                  002400721a7d087415000000000000000000007c08a6010000ab01000000
-                  00000000000100590064007d087e086400530064007d087e087701770078
-                  0359007701
-               182           0 RESUME                   0
-               
-               183           2 LOAD_CONST               1 (0)
-                             4 LOAD_CONST               0 (None)
-                             6 IMPORT_NAME              0 (os)
-                             8 STORE_FAST               2 (os)
-               
-               184          10 LOAD_CONST               1 (0)
-                            12 LOAD_CONST               2 (('SendGridAPIClient',))
-                            14 IMPORT_NAME              1 (sendgrid)
-                            16 IMPORT_FROM              2 (SendGridAPIClient)
-                            18 STORE_FAST               3 (SendGridAPIClient)
-                            20 POP_TOP
-               
-               185          22 LOAD_CONST               1 (0)
-                            24 LOAD_CONST               3 (('Mail',))
-                            26 IMPORT_NAME              3 (sendgrid.helpers.mail)
-                            28 IMPORT_FROM              4 (Mail)
-                            30 STORE_FAST               4 (Mail)
-                            32 POP_TOP
-               
-               187          34 PUSH_NULL
-                            36 LOAD_FAST                4 (Mail)
-               
-               188          38 LOAD_GLOBAL             10 (spwf)
-                            50 LOAD_ATTR                6 (output)
-               
-               189          60 LOAD_GLOBAL             10 (spwf)
-                            72 LOAD_ATTR                6 (output)
-               
-               190          82 LOAD_CONST               4 ('Email from Participant ')
-                            84 LOAD_GLOBAL             10 (spwf)
-                            96 LOAD_ATTR                7 (participant_number)
-                           106 FORMAT_VALUE             0
-                           108 BUILD_STRING             2
-               
-               191         110 LOAD_CONST               5 ('<strong>')
-                           112 LOAD_FAST                0 (body)
-                           114 FORMAT_VALUE             0
-                           116 LOAD_CONST               6 ('</strong>')
-                           118 BUILD_STRING             3
-               
-               187         120 KW_NAMES                 7
-                           122 PRECALL                  4
-                           126 CALL                     4
-                           136 STORE_FAST               5 (message)
-               
-               193         138 PUSH_NULL
-                           140 LOAD_FAST                3 (SendGridAPIClient)
-                           142 LOAD_GLOBAL             10 (spwf)
-                           154 LOAD_ATTR                8 (key)
-                           164 KW_NAMES                 8
-                           166 PRECALL                  1
-                           170 CALL                     1
-                           180 STORE_FAST               6 (sg)
-               
-               195         182 NOP
-               
-               196         184 LOAD_FAST                6 (sg)
-                           186 LOAD_METHOD              9 (send)
-                           208 LOAD_FAST                5 (message)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 STORE_FAST               7 (response)
-               
-               197         226 LOAD_GLOBAL             21 (NULL + print)
-                           238 LOAD_CONST               9 ('Email sent with status code: ')
-                           240 LOAD_FAST                7 (response)
-                           242 LOAD_ATTR               11 (status_code)
-                           252 FORMAT_VALUE             0
-                           254 BUILD_STRING             2
-                           256 PRECALL                  1
-                           260 CALL                     1
-                           270 POP_TOP
-               
-               198         272 LOAD_FAST                1 (email_window)
-                           274 LOAD_METHOD             12 (destroy)
-                           296 PRECALL                  0
-                           300 CALL                     0
-                           310 POP_TOP
-                           312 LOAD_CONST               0 (None)
-                           314 RETURN_VALUE
-                       >>  316 PUSH_EXC_INFO
-               
-               199         318 LOAD_GLOBAL             26 (Exception)
-                           330 CHECK_EXC_MATCH
-                           332 POP_JUMP_FORWARD_IF_FALSE    26 (to 386)
-                           334 STORE_FAST               8 (e)
-               
-               200         336 LOAD_GLOBAL             21 (NULL + print)
-                           348 LOAD_FAST                8 (e)
-                           350 PRECALL                  1
-                           354 CALL                     1
-                           364 POP_TOP
-                           366 POP_EXCEPT
-                           368 LOAD_CONST               0 (None)
-                           370 STORE_FAST               8 (e)
-                           372 DELETE_FAST              8 (e)
-                           374 LOAD_CONST               0 (None)
-                           376 RETURN_VALUE
-                       >>  378 LOAD_CONST               0 (None)
-                           380 STORE_FAST               8 (e)
-                           382 DELETE_FAST              8 (e)
-                           384 RERAISE                  1
-               
-               199     >>  386 RERAISE                  0
-                       >>  388 COPY                     3
-                           390 POP_EXCEPT
-                           392 RERAISE                  1
-               ExceptionTable:
-                 184 to 310 -> 316 [0]
-                 316 to 334 -> 388 [1] lasti
-                 336 to 364 -> 378 [1] lasti
-                 378 to 386 -> 388 [1] lasti
-               consts
-                  None
-                  0
-                  ('SendGridAPIClient',)
-                  ('Mail',)
-                  'Email from Participant '
-                  '<strong>'
-                  '</strong>'
-                  ('from_email', 'to_emails', 'subject', 'html_content')
-                  ('api_key',)
-                  'Email sent with status code: '
-               names      ('os', 'sendgrid', 'SendGridAPIClient', 'sendgrid.helpers.mail', 'Mail', 'spwf', 'output', 'participant_number', 'key', 'send', 'print', 'status_code', 'destroy', 'Exception')
-               varnames   ('body', 'email_window', 'os', 'SendGridAPIClient', 'Mail', 'message', 'sg', 'response', 'e')
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
-               name       'send_email'
-               firstlineno 182
-               lnotab
-                  0x020108010c010c020401160116011c010afc12062c0202012a012e012e
-                  01120132ff
+               firstlineno 192
+               lnotab 0x0a011e012a0124013e012e013e0210123001
             code
                argcount  : 0
                nlocals   : 1
                stacksize : 4
                flags     : 19
                code
-                  0x9502970074000000000000000000000089026b04000000007217740300
-                  0000000000000000006a02000000000000000064018901a6020000ab0200
-                  0000000000000001006400530064027d007407000000000000000000006a
-                  040000000000000000740a000000000000000000007c0067026403ac04a6
-                  020000ab02000000000000000001007407000000000000000000006a0400
-                  00000000000000740a00000000000000000000640567026403ac04a60200
-                  00ab020000000000000000010064005300
-                             0 COPY_FREE_VARS           2
+                  0x9505970074000000000000000000000089046b04000000007213020089
+                  026a01000000000000000064018901a6020000ab02000000000000000001
+                  006400530064027d00020089056a02000000000000000089037c00670264
+                  03ac04a6020000ab0200000000000000000100020089056a020000000000
+                  0000008903640567026403ac04a6020000ab020000000000000000010064
+                  005300
+                             0 COPY_FREE_VARS           5
                
-               203           2 RESUME                   0
+               221           2 RESUME                   0
                
-               204           4 LOAD_GLOBAL              0 (scount)
-                            16 LOAD_DEREF               2 (runcount)
+               222           4 LOAD_GLOBAL              0 (scount)
+                            16 LOAD_DEREF               4 (runcount)
                             18 COMPARE_OP               4 (>)
-                            24 POP_JUMP_FORWARD_IF_FALSE    23 (to 72)
-               
-               205          26 LOAD_GLOBAL              3 (NULL + messagebox)
-                            38 LOAD_ATTR                2 (showerror)
-                            48 LOAD_CONST               1 ('Error')
-                            50 LOAD_DEREF               1 (errortext)
-                            52 PRECALL                  2
-                            56 CALL                     2
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+                            24 POP_JUMP_FORWARD_IF_FALSE    19 (to 64)
                
-               207     >>   72 LOAD_CONST               2 ('Switching.py')
-                            74 STORE_FAST               0 (file_path)
-               
-               208          76 LOAD_GLOBAL              7 (NULL + subprocess)
-                            88 LOAD_ATTR                4 (run)
-                            98 LOAD_GLOBAL             10 (python_path)
-                           110 LOAD_FAST                0 (file_path)
-                           112 BUILD_LIST               2
-                           114 LOAD_CONST               3 (True)
-                           116 KW_NAMES                 4
-                           118 PRECALL                  2
-                           122 CALL                     2
-                           132 POP_TOP
-               
-               209         134 LOAD_GLOBAL              7 (NULL + subprocess)
-                           146 LOAD_ATTR                4 (run)
-                           156 LOAD_GLOBAL             10 (python_path)
-                           168 LOAD_CONST               5 ('Export.py')
-                           170 BUILD_LIST               2
-                           172 LOAD_CONST               3 (True)
-                           174 KW_NAMES                 4
-                           176 PRECALL                  2
-                           180 CALL                     2
-                           190 POP_TOP
-                           192 LOAD_CONST               0 (None)
-                           194 RETURN_VALUE
+               223          26 PUSH_NULL
+                            28 LOAD_DEREF               2 (messagebox)
+                            30 LOAD_ATTR                1 (showerror)
+                            40 LOAD_CONST               1 ('Error')
+                            42 LOAD_DEREF               1 (errortext)
+                            44 PRECALL                  2
+                            48 CALL                     2
+                            58 POP_TOP
+                            60 LOAD_CONST               0 (None)
+                            62 RETURN_VALUE
+               
+               225     >>   64 LOAD_CONST               2 ('Switching.py')
+                            66 STORE_FAST               0 (file_path)
+               
+               226          68 PUSH_NULL
+                            70 LOAD_DEREF               5 (subprocess)
+                            72 LOAD_ATTR                2 (run)
+                            82 LOAD_DEREF               3 (python_path)
+                            84 LOAD_FAST                0 (file_path)
+                            86 BUILD_LIST               2
+                            88 LOAD_CONST               3 (True)
+                            90 KW_NAMES                 4
+                            92 PRECALL                  2
+                            96 CALL                     2
+                           106 POP_TOP
+               
+               227         108 PUSH_NULL
+                           110 LOAD_DEREF               5 (subprocess)
+                           112 LOAD_ATTR                2 (run)
+                           122 LOAD_DEREF               3 (python_path)
+                           124 LOAD_CONST               5 ('Export.py')
+                           126 BUILD_LIST               2
+                           128 LOAD_CONST               3 (True)
+                           130 KW_NAMES                 4
+                           132 PRECALL                  2
+                           136 CALL                     2
+                           146 POP_TOP
+                           148 LOAD_CONST               0 (None)
+                           150 RETURN_VALUE
                consts
                   None
                   'Error'
                   'Switching.py'
                   True
                   ('check',)
                   'Export.py'
-               names      ('scount', 'messagebox', 'showerror', 'subprocess', 'run', 'python_path')
+               names      ('scount', 'showerror', 'run')
                varnames   ('file_path',)
-               freevars   ('errortext', 'runcount')
+               freevars   ('errortext', 'messagebox', 'python_path', 'runcount', 'subprocess')
                cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       'pis'
-               firstlineno 203
-               lnotab 0x040116012e0204013a01
+               firstlineno 221
+               lnotab 0x04011601260204012801
             ('Helvetica', 18)
             ('Helvetica', 22)
             ('Helvetica', 12)
             '-fullscreen'
             True
+            '-topmost'
+            False
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 2
+               flags     : 19
+               code
+                  0x950197008900a0000000000000000000000000000000000000000000a6
+                  000000ab000000000000000000010064005300
+                             0 COPY_FREE_VARS           1
+               
+               237           2 RESUME                   0
+               
+               238           4 LOAD_DEREF               0 (root)
+                             6 LOAD_METHOD              0 (destroy)
+                            28 PRECALL                  0
+                            32 CALL                     0
+                            42 POP_TOP
+                            44 LOAD_CONST               0 (None)
+                            46 RETURN_VALUE
+               consts
+                  None
+               names      ('destroy',)
+               varnames   ()
+               freevars   ('root',)
+               cellvars   ()
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
+               name       'exit_program'
+               firstlineno 237
+               lnotab 0x0401
+            'Exit'
+            ('text', 'command', 'font')
+            'top'
+            'ne'
+            5
+            ('side', 'anchor', 'padx', 'pady')
             ''
             ('text', 'font')
             code
                argcount  : 0
                nlocals   : 1
                stacksize : 4
                flags     : 19
                code
-                  0x950297007401000000000000000000006a0100000000000000006401a6
-                  010000ab0100000000000000007d008901a0020000000000000000000000
-                  0000000000000000007c00ac02a6010000ab010000000000000000010089
-                  01a003000000000000000000000000000000000000000064038902a60200
-                  00ab020000000000000000010064005300
-                             0 COPY_FREE_VARS           2
-               
-               222           2 RESUME                   0
-               
-               223           4 LOAD_GLOBAL              1 (NULL + time)
-                            16 LOAD_ATTR                1 (strftime)
-                            26 LOAD_CONST               1 ('%H:%M:%S')
-                            28 PRECALL                  1
-                            32 CALL                     1
-                            42 STORE_FAST               0 (current_time)
-               
-               224          44 LOAD_DEREF               1 (time_label)
-                            46 LOAD_METHOD              2 (config)
-                            68 LOAD_FAST                0 (current_time)
-                            70 KW_NAMES                 2
-                            72 PRECALL                  1
-                            76 CALL                     1
-                            86 POP_TOP
-               
-               225          88 LOAD_DEREF               1 (time_label)
-                            90 LOAD_METHOD              3 (after)
-                           112 LOAD_CONST               3 (1000)
-                           114 LOAD_DEREF               2 (update_time)
-                           116 PRECALL                  2
-                           120 CALL                     2
-                           130 POP_TOP
-                           132 LOAD_CONST               0 (None)
-                           134 RETURN_VALUE
+                  0x95039700020089016a0000000000000000006401a6010000ab01000000
+                  00000000007d008902a00100000000000000000000000000000000000000
+                  007c00ac02a6010000ab01000000000000000001008902a0020000000000
+                  00000000000000000000000000000064038903a6020000ab020000000000
+                  000000010064005300
+                             0 COPY_FREE_VARS           3
+               
+               245           2 RESUME                   0
+               
+               246           4 PUSH_NULL
+                             6 LOAD_DEREF               1 (time)
+                             8 LOAD_ATTR                0 (strftime)
+                            18 LOAD_CONST               1 ('%H:%M:%S')
+                            20 PRECALL                  1
+                            24 CALL                     1
+                            34 STORE_FAST               0 (current_time)
+               
+               247          36 LOAD_DEREF               2 (time_label)
+                            38 LOAD_METHOD              1 (config)
+                            60 LOAD_FAST                0 (current_time)
+                            62 KW_NAMES                 2
+                            64 PRECALL                  1
+                            68 CALL                     1
+                            78 POP_TOP
+               
+               248          80 LOAD_DEREF               2 (time_label)
+                            82 LOAD_METHOD              2 (after)
+                           104 LOAD_CONST               3 (1000)
+                           106 LOAD_DEREF               3 (update_time)
+                           108 PRECALL                  2
+                           112 CALL                     2
+                           122 POP_TOP
+                           124 LOAD_CONST               0 (None)
+                           126 RETURN_VALUE
                consts
                   None
                   '%H:%M:%S'
                   ('text',)
                   1000
-               names      ('time', 'strftime', 'config', 'after')
+               names      ('strftime', 'config', 'after')
                varnames   ('current_time',)
-               freevars   ('time_label', 'update_time')
+               freevars   ('time', 'time_label', 'update_time')
                cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       'update_time'
-               firstlineno 222
-               lnotab 0x040128012c01
+               firstlineno 245
+               lnotab 0x040120012c01
             20
             'nw'
             ('side', 'padx', 'pady', 'anchor')
             ('side', 'fill')
             'Welcome back!'
             ('pady',)
             'Please now select a task to perform'
             30
-            5
             'center'
             code
                argcount  : 0
                nlocals   : 1
                stacksize : 4
                flags     : 19
                code
-                  0x9502970074000000000000000000000089026b04000000007234740300
-                  0000000000000000006a02000000000000000064018901a6020000ab0200
-                  0000000000000001007407000000000000000000006a0400000000000000
-                  00740a00000000000000000000640267026403ac04a6020000ab02000000
-                  000000000001006400530064057d007407000000000000000000006a0400
-                  00000000000000740a000000000000000000007c0067026403ac04a60200
-                  00ab02000000000000000001007407000000000000000000006a04000000
-                  0000000000740a00000000000000000000640267026403ac04a6020000ab
-                  020000000000000000010064005300
-                             0 COPY_FREE_VARS           2
+                  0x9505970074000000000000000000000089046b04000000007227020089
+                  026a01000000000000000064018901a6020000ab02000000000000000001
+                  00020089056a0200000000000000008903640267026403ac04a6020000ab
+                  02000000000000000001006400530064057d00020089056a020000000000
+                  00000089037c0067026403ac04a6020000ab020000000000000000010002
+                  0089056a0200000000000000008903640267026403ac04a6020000ab0200
+                  00000000000000010064005300
+                             0 COPY_FREE_VARS           5
                
-               244           2 RESUME                   0
+               267           2 RESUME                   0
                
-               246           4 LOAD_GLOBAL              0 (nbcount)
-                            16 LOAD_DEREF               2 (runcount)
+               269           4 LOAD_GLOBAL              0 (nbcount)
+                            16 LOAD_DEREF               4 (runcount)
                             18 COMPARE_OP               4 (>)
-                            24 POP_JUMP_FORWARD_IF_FALSE    52 (to 130)
-               
-               247          26 LOAD_GLOBAL              3 (NULL + messagebox)
-                            38 LOAD_ATTR                2 (showerror)
-                            48 LOAD_CONST               1 ('Error')
-                            50 LOAD_DEREF               1 (errortext)
-                            52 PRECALL                  2
-                            56 CALL                     2
-                            66 POP_TOP
+                            24 POP_JUMP_FORWARD_IF_FALSE    39 (to 104)
                
-               248          68 LOAD_GLOBAL              7 (NULL + subprocess)
-                            80 LOAD_ATTR                4 (run)
-                            90 LOAD_GLOBAL             10 (python_path)
-                           102 LOAD_CONST               2 ('Export.py')
-                           104 BUILD_LIST               2
-                           106 LOAD_CONST               3 (True)
-                           108 KW_NAMES                 4
-                           110 PRECALL                  2
-                           114 CALL                     2
-                           124 POP_TOP
-                           126 LOAD_CONST               0 (None)
-                           128 RETURN_VALUE
-               
-               250     >>  130 LOAD_CONST               5 ('N-Back.py')
-                           132 STORE_FAST               0 (file_path)
-               
-               251         134 LOAD_GLOBAL              7 (NULL + subprocess)
-                           146 LOAD_ATTR                4 (run)
-                           156 LOAD_GLOBAL             10 (python_path)
-                           168 LOAD_FAST                0 (file_path)
-                           170 BUILD_LIST               2
-                           172 LOAD_CONST               3 (True)
-                           174 KW_NAMES                 4
-                           176 PRECALL                  2
-                           180 CALL                     2
-                           190 POP_TOP
-               
-               252         192 LOAD_GLOBAL              7 (NULL + subprocess)
-                           204 LOAD_ATTR                4 (run)
-                           214 LOAD_GLOBAL             10 (python_path)
-                           226 LOAD_CONST               2 ('Export.py')
-                           228 BUILD_LIST               2
-                           230 LOAD_CONST               3 (True)
-                           232 KW_NAMES                 4
-                           234 PRECALL                  2
-                           238 CALL                     2
-                           248 POP_TOP
-                           250 LOAD_CONST               0 (None)
-                           252 RETURN_VALUE
+               270          26 PUSH_NULL
+                            28 LOAD_DEREF               2 (messagebox)
+                            30 LOAD_ATTR                1 (showerror)
+                            40 LOAD_CONST               1 ('Error')
+                            42 LOAD_DEREF               1 (errortext)
+                            44 PRECALL                  2
+                            48 CALL                     2
+                            58 POP_TOP
+               
+               271          60 PUSH_NULL
+                            62 LOAD_DEREF               5 (subprocess)
+                            64 LOAD_ATTR                2 (run)
+                            74 LOAD_DEREF               3 (python_path)
+                            76 LOAD_CONST               2 ('Export.py')
+                            78 BUILD_LIST               2
+                            80 LOAD_CONST               3 (True)
+                            82 KW_NAMES                 4
+                            84 PRECALL                  2
+                            88 CALL                     2
+                            98 POP_TOP
+                           100 LOAD_CONST               0 (None)
+                           102 RETURN_VALUE
+               
+               273     >>  104 LOAD_CONST               5 ('N-Back.py')
+                           106 STORE_FAST               0 (file_path)
+               
+               274         108 PUSH_NULL
+                           110 LOAD_DEREF               5 (subprocess)
+                           112 LOAD_ATTR                2 (run)
+                           122 LOAD_DEREF               3 (python_path)
+                           124 LOAD_FAST                0 (file_path)
+                           126 BUILD_LIST               2
+                           128 LOAD_CONST               3 (True)
+                           130 KW_NAMES                 4
+                           132 PRECALL                  2
+                           136 CALL                     2
+                           146 POP_TOP
+               
+               275         148 PUSH_NULL
+                           150 LOAD_DEREF               5 (subprocess)
+                           152 LOAD_ATTR                2 (run)
+                           162 LOAD_DEREF               3 (python_path)
+                           164 LOAD_CONST               2 ('Export.py')
+                           166 BUILD_LIST               2
+                           168 LOAD_CONST               3 (True)
+                           170 KW_NAMES                 4
+                           172 PRECALL                  2
+                           176 CALL                     2
+                           186 POP_TOP
+                           188 LOAD_CONST               0 (None)
+                           190 RETURN_VALUE
                consts
                   None
                   'Error'
                   'Export.py'
                   True
                   ('check',)
                   'N-Back.py'
-               names      ('nbcount', 'messagebox', 'showerror', 'subprocess', 'run', 'python_path')
+               names      ('nbcount', 'showerror', 'run')
                varnames   ('file_path',)
-               freevars   ('errortext', 'runcount')
+               freevars   ('errortext', 'messagebox', 'python_path', 'runcount', 'subprocess')
                cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       'nbrun'
-               firstlineno 244
-               lnotab 0x040216012a013e0204013a01
+               firstlineno 267
+               lnotab 0x0402160122012c0204012801
             'N-Back'
             ('text', 'command', 'font', 'anchor')
             ('side', 'pady')
             1
             'You have completed this '
             ' time so far'
             ' times so far'
@@ -2496,133 +2763,134 @@
             'Switching Task'
             code
                argcount  : 0
                nlocals   : 1
                stacksize : 4
                flags     : 19
                code
-                  0x9502970074000000000000000000000089026b04000000007234740300
-                  0000000000000000006a02000000000000000064018901a6020000ab0200
-                  0000000000000001007407000000000000000000006a0400000000000000
-                  00740a00000000000000000000640267026403ac04a6020000ab02000000
-                  000000000001006400530064057d007407000000000000000000006a0400
-                  00000000000000740a000000000000000000007c0067026403ac04a60200
-                  00ab02000000000000000001007407000000000000000000006a04000000
-                  0000000000740a00000000000000000000640267026403ac04a6020000ab
-                  020000000000000000010064005300
-                             0 COPY_FREE_VARS           2
+                  0x9505970074000000000000000000000089046b04000000007227020089
+                  026a01000000000000000064018901a6020000ab02000000000000000001
+                  00020089056a0200000000000000008903640267026403ac04a6020000ab
+                  02000000000000000001006400530064057d00020089056a020000000000
+                  00000089037c0067026403ac04a6020000ab020000000000000000010002
+                  0089056a0200000000000000008903640267026403ac04a6020000ab0200
+                  00000000000000010064005300
+                             0 COPY_FREE_VARS           5
                
-               281           2 RESUME                   0
+               304           2 RESUME                   0
                
-               283           4 LOAD_GLOBAL              0 (rtcount)
-                            16 LOAD_DEREF               2 (runcount)
+               306           4 LOAD_GLOBAL              0 (rtcount)
+                            16 LOAD_DEREF               4 (runcount)
                             18 COMPARE_OP               4 (>)
-                            24 POP_JUMP_FORWARD_IF_FALSE    52 (to 130)
-               
-               284          26 LOAD_GLOBAL              3 (NULL + messagebox)
-                            38 LOAD_ATTR                2 (showerror)
-                            48 LOAD_CONST               1 ('Error')
-                            50 LOAD_DEREF               1 (errortext)
-                            52 PRECALL                  2
-                            56 CALL                     2
-                            66 POP_TOP
+                            24 POP_JUMP_FORWARD_IF_FALSE    39 (to 104)
                
-               285          68 LOAD_GLOBAL              7 (NULL + subprocess)
-                            80 LOAD_ATTR                4 (run)
-                            90 LOAD_GLOBAL             10 (python_path)
-                           102 LOAD_CONST               2 ('Export.py')
-                           104 BUILD_LIST               2
-                           106 LOAD_CONST               3 (True)
-                           108 KW_NAMES                 4
-                           110 PRECALL                  2
-                           114 CALL                     2
-                           124 POP_TOP
-                           126 LOAD_CONST               0 (None)
-                           128 RETURN_VALUE
-               
-               287     >>  130 LOAD_CONST               5 ('Reaction Time Task - Copy.py')
-                           132 STORE_FAST               0 (file_path)
-               
-               288         134 LOAD_GLOBAL              7 (NULL + subprocess)
-                           146 LOAD_ATTR                4 (run)
-                           156 LOAD_GLOBAL             10 (python_path)
-                           168 LOAD_FAST                0 (file_path)
-                           170 BUILD_LIST               2
-                           172 LOAD_CONST               3 (True)
-                           174 KW_NAMES                 4
-                           176 PRECALL                  2
-                           180 CALL                     2
-                           190 POP_TOP
-               
-               289         192 LOAD_GLOBAL              7 (NULL + subprocess)
-                           204 LOAD_ATTR                4 (run)
-                           214 LOAD_GLOBAL             10 (python_path)
-                           226 LOAD_CONST               2 ('Export.py')
-                           228 BUILD_LIST               2
-                           230 LOAD_CONST               3 (True)
-                           232 KW_NAMES                 4
-                           234 PRECALL                  2
-                           238 CALL                     2
-                           248 POP_TOP
-                           250 LOAD_CONST               0 (None)
-                           252 RETURN_VALUE
+               307          26 PUSH_NULL
+                            28 LOAD_DEREF               2 (messagebox)
+                            30 LOAD_ATTR                1 (showerror)
+                            40 LOAD_CONST               1 ('Error')
+                            42 LOAD_DEREF               1 (errortext)
+                            44 PRECALL                  2
+                            48 CALL                     2
+                            58 POP_TOP
+               
+               308          60 PUSH_NULL
+                            62 LOAD_DEREF               5 (subprocess)
+                            64 LOAD_ATTR                2 (run)
+                            74 LOAD_DEREF               3 (python_path)
+                            76 LOAD_CONST               2 ('Export.py')
+                            78 BUILD_LIST               2
+                            80 LOAD_CONST               3 (True)
+                            82 KW_NAMES                 4
+                            84 PRECALL                  2
+                            88 CALL                     2
+                            98 POP_TOP
+                           100 LOAD_CONST               0 (None)
+                           102 RETURN_VALUE
+               
+               310     >>  104 LOAD_CONST               5 ('Reaction Time Task - Copy.py')
+                           106 STORE_FAST               0 (file_path)
+               
+               311         108 PUSH_NULL
+                           110 LOAD_DEREF               5 (subprocess)
+                           112 LOAD_ATTR                2 (run)
+                           122 LOAD_DEREF               3 (python_path)
+                           124 LOAD_FAST                0 (file_path)
+                           126 BUILD_LIST               2
+                           128 LOAD_CONST               3 (True)
+                           130 KW_NAMES                 4
+                           132 PRECALL                  2
+                           136 CALL                     2
+                           146 POP_TOP
+               
+               312         148 PUSH_NULL
+                           150 LOAD_DEREF               5 (subprocess)
+                           152 LOAD_ATTR                2 (run)
+                           162 LOAD_DEREF               3 (python_path)
+                           164 LOAD_CONST               2 ('Export.py')
+                           166 BUILD_LIST               2
+                           168 LOAD_CONST               3 (True)
+                           170 KW_NAMES                 4
+                           172 PRECALL                  2
+                           176 CALL                     2
+                           186 POP_TOP
+                           188 LOAD_CONST               0 (None)
+                           190 RETURN_VALUE
                consts
                   None
                   'Error'
                   'Export.py'
                   True
                   ('check',)
                   'Reaction Time Task - Copy.py'
-               names      ('rtcount', 'messagebox', 'showerror', 'subprocess', 'run', 'python_path')
+               names      ('rtcount', 'showerror', 'run')
                varnames   ('file_path',)
-               freevars   ('errortext', 'runcount')
+               freevars   ('errortext', 'messagebox', 'python_path', 'runcount', 'subprocess')
                cellvars   ()
-               filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+               filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
                name       'consent'
-               firstlineno 281
-               lnotab 0x040216012a013e0204013a01
+               firstlineno 304
+               lnotab 0x0402160122012c0204012801
             '2-Type Reaction Time'
             'sw'
             'Email for assistance or queries'
-            ('text', 'command', 'font')
             'uop.png'
             ('image',)
-            0
-            'ne'
             -20
+            40
             ('relx', 'rely', 'anchor', 'x', 'y')
             'Export.py'
             ('check',)
-         names      ('tk', 'Tk', 'winfo_screenheight', 'winfo_screenwidth', 'glob', 'folder_name', 'spwf', 'emailadd', 'password', 'attributes', 'Label', 'pack', 'TOP', 'Frame', 'X', 'Button', 'nbcount', 'scount', 'rtcount', 'BOTTOM', 'LEFT', 'Image', 'open', 'ImageTk', 'PhotoImage', 'place', 'mainloop', 'quit', 'cpurun', 'terminate', 'subprocess', 'run', 'python_path', 'file_path')
-         varnames   ('root', 'screen_height', 'screen_width', 'dimensions', 'position', 'USERNAME', 'PASSWORD', 'emailsupport', 'pis', 'fontsize', 'fontsize1', 'fontsize2', 'welcome_frame', 'welcome_label', 'text_frame', 'text_label', 'nback_frame', 'nbrun', 'nback', 'text', 'nback_label', 'button1_frame', 'button2_frame', 'button2', 'button2_label', 'consent', 'button3_frame', 'button3', 'button3_label', 'button12_frame', 'button12', 'image_file', 'image2', 'image_label')
+         names      ('subprocess', 'random', 'platform', 'os', 'sys', 'executable', 'spwf', 'tkinter', 'time', 'PIL', 'Image', 'ImageTk', 'datetime', 'filedialog', 'simpledialog', 'messagebox', 'Location', 'sendgrid', 'SendGridAPIClient', 'sendgrid.helpers.mail', 'Mail', 'Attachment', 'FileContent', 'FileName', 'FileType', 'Disposition', 'Tk', 'winfo_screenheight', 'winfo_screenwidth', 'glob', 'folder_name', 'emailadd', 'password', 'attributes', 'Button', 'pack', 'Label', 'TOP', 'Frame', 'X', 'nbcount', 'scount', 'rtcount', 'BOTTOM', 'LEFT', 'open', 'PhotoImage', 'place', 'run', 'mainloop', 'quit', 'file_path')
+         varnames   ('random', 'platform', 'os', 'sys', 'Image', 'ImageTk', 'datetime', 'filedialog', 'simpledialog', 'Location', 'Attachment', 'FileContent', 'FileName', 'FileType', 'Disposition', 'screen_height', 'screen_width', 'dimensions', 'position', 'USERNAME', 'PASSWORD', 'emailsupport', 'pis', 'fontsize', 'fontsize1', 'fontsize2', 'fontsizesmall', 'exit_program', 'exit_button', 'welcome_frame', 'welcome_label', 'text_frame', 'text_label', 'nback_frame', 'nbrun', 'nback', 'text', 'nback_label', 'button1_frame', 'button2_frame', 'button2', 'button2_label', 'consent', 'button3_frame', 'button3', 'button3_label', 'button12_frame', 'button12', 'image_file', 'image2', 'image_label')
          freevars   ()
-         cellvars   ('errortext', 'runcount', 'send_email', 'time_label', 'update_time')
-         filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+         cellvars   ('Mail', 'SendGridAPIClient', 'errortext', 'messagebox', 'python_path', 'root', 'runcount', 'spwf', 'subprocess', 'time', 'time_label', 'tk', 'update_time')
+         filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
          name       'main'
          firstlineno 156
          lnotab
-            0x0c0226012801280210010a01040104023a02180118020a0a06150c0b04
-            01040104022c022e020c054602280156022e012c02280156022e012c0228
-            0146020c0a320142021601180216012e0144032801460228014602320142
-            021601180216012e0142020c0a28014601320142021601180216012e0144
-            022801460230014202280128012c01340114022802280132013e0432013a
-            01
+            0x1c03080108010801080108010e0208010801080110010c010c01100108
+            010c0120031e012801280210010a01040104023a020e010e02101d120804
+            010401040104022c012c020a032801320226020e053c022001420226012c
+            022001420226012c0220013c02120a2a01380216011802160126013a0320
+            013c0220013c022a01380216011802160126013802120a20013c012a0138
+            0216011802160126013a0220013c02280138022001200124013401140228
+            0228022c052801
       'Your device is not connected to the internet, please connect to the internet to continue the task\n\nThe task must ensure that you have the correct files installed, which requires an active internet connection'
       ('Helvetica', 18)
       ('Helvetica', 22)
       ('Helvetica', 12)
       'Error'
-   names      ('socket', 'tkinter', 'tk', 'os', 'is_connected', 'Connected', 'path', 'exists', 'pathnum', 'csv', 'simpledialog', 'messagebox', 'PinSystem', '__name__', 'Tk', 'root', 'mainloop', 'quit', 'spwf', 'print', 'participant_number', 'subprocess', 'sys', 'executable', 'pythonpath', 'python_path', 'environ', 'pathsep', 'filename', 'open', 'f', 'readline', 'first_line', 'split', 'words', 'word', 'isdigit', 'int', 'folder_name', 'mkdir', 'FileExistsError', 'run', 'result', 'Location', 'Dependencies', 'Popen', 'cpurun', 'random', 'platform', 'time', 'PIL', 'Image', 'ImageTk', 'datetime', 'filedialog', 'glob', 'file_path', 'RTcount', 'rtcount', 'NBcount', 'nbcount', 'switchcount', 'scount', 'main', 'errortext', 'fontsize', 'fontsize1', 'fontsize2', 'showerror')
+   names      ('socket', 'tkinter', 'tk', 'os', 'is_connected', 'Connected', 'path', 'exists', 'pathnum', 'csv', 'simpledialog', 'messagebox', 'PinSystem', '__name__', 'Tk', 'root', 'mainloop', 'quit', 'spwf', 'print', 'participant_number', 'subprocess', 'sys', 'executable', 'pythonpath', 'python_path', 'environ', 'pathsep', 'filename', 'open', 'f', 'readline', 'first_line', 'split', 'words', 'word', 'isdigit', 'int', 'folder_name', 'mkdir', 'FileExistsError', 'run', 'result', 'Location', 'random', 'platform', 'time', 'PIL', 'Image', 'ImageTk', 'datetime', 'filedialog', 'glob', 'file_path', 'RTcount', 'rtcount', 'NBcount', 'nbcount', 'switchcount', 'scount', 'main', 'errortext', 'fontsize', 'fontsize1', 'fontsize2', 'showerror')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Task Development\\Stimuli\\Task\\Task.py'
+   filename   'H:\\Task Development\\Stimuli\\Task\\Task.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080108010802060a160104023401060408010801100108
-      021a2b0c021e01160128012802080228020801080108020e0104013a0204
-      021a012801280104010801280118fe02fc2e070a0202012001220208011a
-      ff080228010801080124010801080108010801080110010c010c01100108
-      02040204021a012801280104010801280118fe02fc2e0804021a01280128
-      0104010801280118fe02fc2e0804021a012801280104010801280118fe02
-      fc2e080801067f002c1803080104040401040104031002
+      0x00ff02010801080108010802060a160204023401060408010801100108
+      021a2c0c021e0116012801280208022802080108020e0104013a0204021a
+      012801280104010801280118fe02fc2e070a0202012001220208011aff08
+      02280108010801080108010801080110010c010c0110010802040204021a
+      012801280104010801280118fe02fc2e0804021a01280128010401080128
+      0118fe02fc2e0804021a012801280104010801280118fe02fc2e08080206
+      7f00431803080104020401040104021002
```

### Comparing `JBPhD-2.2.2/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.2.3/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/asterisk.png` & `JBPhD-2.2.3/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/circle.jpg` & `JBPhD-2.2.3/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/greendot.png` & `JBPhD-2.2.3/Task/greendot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/greentick.png` & `JBPhD-2.2.3/Task/greentick.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/redcross.png` & `JBPhD-2.2.3/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/reddot.png` & `JBPhD-2.2.3/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/setup.py` & `JBPhD-2.2.3/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/trial.jpeg` & `JBPhD-2.2.3/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/uop.ico` & `JBPhD-2.2.3/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/uop.jpeg` & `JBPhD-2.2.3/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/Task/uop.png` & `JBPhD-2.2.3/Task/uop.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.2/setup.py` & `JBPhD-2.2.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 packagereqs = ['sendgrid', 'plyer', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='JBPhD',
-    version='2.2.2',
+    version='2.2.3',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
     description=long_description,
     classifiers=[
         'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved',
         'Operating System :: OS Independent',
     ],
     include_package_data=True,
-    data_files=[('.', ['README.txt', 'MANIFEST.in'])],
+    data_files=[('.', ['LICENSE.txt','README.txt', 'MANIFEST.in'])],
 )
```

