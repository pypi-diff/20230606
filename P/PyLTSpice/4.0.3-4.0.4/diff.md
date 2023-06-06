# Comparing `tmp/PyLTSpice-4.0.3.tar.gz` & `tmp/PyLTSpice-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-mre5943o\PyLTSpice-4.0.3.tar", last modified: Fri May 26 20:02:26 2023, max compression
+gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-ydkee3cw\PyLTSpice-4.0.4.tar", last modified: Tue Jun  6 07:12:14 2023, max compression
```

## Comparing `PyLTSpice-4.0.3.tar` & `PyLTSpice-4.0.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.906688 PyLTSpice-4.0.3/
--rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.3/LICENSE
--rw-rw-rw-   0        0        0    56816 2023-05-26 20:02:26.904687 PyLTSpice-4.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.750594 PyLTSpice-4.0.3/PyLTSpice/
--rw-rw-rw-   0        0        0     9679 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      362 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/LTSpiceBatch.py
--rw-rw-rw-   0        0        0      333 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/LTSpice_RawRead.py
--rw-rw-rw-   0        0        0      332 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/LTSpice_RawWrite.py
--rw-rw-rw-   0        0        0     6609 2023-05-26 19:49:19.000000 PyLTSpice-4.0.3/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0      293 2023-05-14 19:17:53.000000 PyLTSpice-4.0.3/PyLTSpice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.790504 PyLTSpice-4.0.3/PyLTSpice/client_server/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/__init__.py
--rw-rw-rw-   0        0        0     8400 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/sim_client.py
--rw-rw-rw-   0        0        0     5427 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/sim_server.py
--rw-rw-rw-   0        0        0     4737 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.801686 PyLTSpice-4.0.3/PyLTSpice/log/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/log/__init__.py
--rw-rw-rw-   0        0        0    29860 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/log/ltsteps.py
--rw-rw-rw-   0        0        0     6047 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.826656 PyLTSpice-4.0.3/PyLTSpice/raw/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/__init__.py
--rw-rw-rw-   0        0        0    14667 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_classes.py
--rw-rw-rw-   0        0        0     5609 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_convert.py
--rw-rw-rw-   0        0        0    36030 2023-05-26 19:50:13.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_read.py
--rw-rw-rw-   0        0        0    16752 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_write.py
--rw-rw-rw-   0        0        0     4014 2023-05-14 19:17:53.000000 PyLTSpice-4.0.3/PyLTSpice/rawplot.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.873530 PyLTSpice-4.0.3/PyLTSpice/sim/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/__init__.py
--rw-rw-rw-   0        0        0     8568 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/ltspice_simulator.py
--rw-rw-rw-   0        0        0     4636 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/ngspice_simulator.py
--rw-rw-rw-   0        0        0     1505 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/process_callback.py
--rw-rw-rw-   0        0        0     6059 2023-05-26 19:50:13.000000 PyLTSpice-4.0.3/PyLTSpice/sim/run_task.py
--rw-rw-rw-   0        0        0     4809 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_analysis.py
--rw-rw-rw-   0        0        0    10749 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_batch.py
--rw-rw-rw-   0        0        0    23686 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_runner.py
--rw-rw-rw-   0        0        0     9221 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     4652 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/simulator.py
--rw-rw-rw-   0        0        0    46631 2023-05-26 14:01:10.000000 PyLTSpice-4.0.3/PyLTSpice/sim/spice_editor.py
--rw-rw-rw-   0        0        0     7384 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/xyce_simulator.py
--rw-rw-rw-   0        0        0    21705 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim_batch.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.881748 PyLTSpice-4.0.3/PyLTSpice/utils/
--rw-rw-rw-   0        0        0     2935 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/utils/detect_encoding.py
--rw-rw-rw-   0        0        0    11563 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.774837 PyLTSpice-4.0.3/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    56816 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15035 2023-05-26 20:01:44.000000 PyLTSpice-4.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.886779 PyLTSpice-4.0.3/doc/
--rw-rw-rw-   0        0        0     2448 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/doc/conf.py
--rw-rw-rw-   0        0        0     1193 2023-05-26 19:59:48.000000 PyLTSpice-4.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 20:02:26.906688 PyLTSpice-4.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.890724 PyLTSpice-4.0.3/tests/
--rw-rw-rw-   0        0        0      801 2023-05-14 19:17:08.000000 PyLTSpice-4.0.3/tests/test_ltsteps.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.893716 PyLTSpice-4.0.3/tests/unittest/
-drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.899701 PyLTSpice-4.0.3/tests/unittest/sweep_iterators/
--rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.3/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.3/tests/unittest/test_pyltspice.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.262939 PyLTSpice-4.0.4/
+-rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.4/LICENSE
+-rw-rw-rw-   0        0        0    58218 2023-06-06 07:12:14.261743 PyLTSpice-4.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.146625 PyLTSpice-4.0.4/PyLTSpice/
+-rw-rw-rw-   0        0        0     9679 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/Histogram.py
+-rw-rw-rw-   0        0        0      362 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/LTSpiceBatch.py
+-rw-rw-rw-   0        0        0      333 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/LTSpice_RawRead.py
+-rw-rw-rw-   0        0        0      332 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/LTSpice_RawWrite.py
+-rw-rw-rw-   0        0        0     6743 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/LTSteps.py
+-rw-rw-rw-   0        0        0     1692 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.180377 PyLTSpice-4.0.4/PyLTSpice/client_server/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/__init__.py
+-rw-rw-rw-   0        0        0     8488 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     5570 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     4865 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.189063 PyLTSpice-4.0.4/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0    29997 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0     6047 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.203701 PyLTSpice-4.0.4/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0    14667 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     5609 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    36151 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0    16752 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/raw/raw_write.py
+-rw-rw-rw-   0        0        0     4014 2023-05-14 19:17:53.000000 PyLTSpice-4.0.4/PyLTSpice/rawplot.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.240743 PyLTSpice-4.0.4/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     8683 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     4738 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     1505 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0     7179 2023-06-04 10:41:26.000000 PyLTSpice-4.0.4/PyLTSpice/sim/run_task.py
+-rw-rw-rw-   0        0        0     4809 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_analysis.py
+-rw-rw-rw-   0        0        0    10823 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0    23309 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     9298 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     4652 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/sim/simulator.py
+-rw-rw-rw-   0        0        0    46624 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/spice_editor.py
+-rw-rw-rw-   0        0        0     7456 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim/xyce_simulator.py
+-rw-rw-rw-   0        0        0    21638 2023-06-02 14:46:46.000000 PyLTSpice-4.0.4/PyLTSpice/sim_batch.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.246771 PyLTSpice-4.0.4/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     2935 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0    11563 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/PyLTSpice/utils/sweep_iterators.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.167871 PyLTSpice-4.0.4/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    58218 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-06 07:12:13.000000 PyLTSpice-4.0.4/PyLTSpice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16437 2023-06-04 10:54:08.000000 PyLTSpice-4.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.249446 PyLTSpice-4.0.4/doc/
+-rw-rw-rw-   0        0        0     2448 2023-05-14 19:17:07.000000 PyLTSpice-4.0.4/doc/conf.py
+-rw-rw-rw-   0        0        0     1193 2023-06-04 10:50:02.000000 PyLTSpice-4.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:12:14.262939 PyLTSpice-4.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.252633 PyLTSpice-4.0.4/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-14 19:17:08.000000 PyLTSpice-4.0.4/tests/test_ltsteps.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.255247 PyLTSpice-4.0.4/tests/unittest/
+drwxrwxrwx   0        0        0        0 2023-06-06 07:12:14.257843 PyLTSpice-4.0.4/tests/unittest/sweep_iterators/
+-rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.4/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.4/tests/unittest/test_pyltspice.py
```

### Comparing `PyLTSpice-4.0.3/LICENSE` & `PyLTSpice-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PKG-INFO` & `PyLTSpice-4.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.3
+Version: 4.0.4
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -947,23 +947,49 @@
 ```
 
 ### SemiDevOpReader.py ###
 
 This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information. A more detailed
 documentation is directly included in the source file docstrings.
 
+## Debug Logging
+The library uses the standard `logging` module. Three convenience functions have been added for easily changing logging 
+settings across the entire library. `PyLTSpice.all_loggers()` returns a list of all the logger's names, `PyLTSpice.set_log_level(logging.DEBUG)` 
+would set the library's logging level to debug, and `PyLTSpice.add_log_handler(my_handler)` would add `my_handler` as a handler for 
+all loggers.
+
+### Single Module Logging
+It is also possible to set the logging settings for a single module by using its name acquired from the `PyLTSpice.all_loggers()` 
+function. For example:
+
+```python
+import logging
+logging.basicConfig(level=logging.INFO)  # Set up the root logger first
+
+import PyLTSpice  # Import PyLTSpice to set the logging levels
+PyLTSpice.set_log_level(logging.DEBUG)  # Set PyLTSpice's global log level
+logging.getLogger("PyLTSpice.RawRead").level = logging.WARNING  # Set the log level for only RawRead to warning
+```
+Would set only `PyLTSpice.RawRead` file's logging level to warning while the other modules would remain at debug level. 
+_Make sure to initialize the root logger before importing the library to be able to see the logs._
+
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.4\
+  Improved usage of the logging library. (Thanks TSprech@GitHub)\
+  Included RunTask number in the log messages.\ 
+  Included milliseconds in the time elapsed calculation.
+
 * Version 4.0.3\
-  Fixing issue in elapsed time calculation.
+  Fixing issue in elapsed time calculation.\
   Fixing issue with the import of LTSpiceLogReader from LTSteps.py
 
 * Version 4.0.2\
   Changing list of Library dependencies.
 
 * Version 4.0.1\
   Bug fix on CLI for the Histogram.py and LTSteps.py
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/Histogram.py` & `PyLTSpice-4.0.4/PyLTSpice/Histogram.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/LTSteps.py` & `PyLTSpice-4.0.4/PyLTSpice/LTSteps.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,61 +84,61 @@
 """
 __author__ = "Nuno Canto Brum <me@nunobrum.com>"
 __copyright__ = "Copyright 2023, Fribourg Switzerland"
 import os
 import sys
 
 from PyLTSpice.log.ltsteps import *
-
+import logging
+_logger = logging.getLogger("PyLTSpice.LTSteps")
 
 def main():
     """
     Main function for the LTSteps.py script
     """
-
     def valid_extension(filename):
         """A simple function to check if the filename has a valid extension"""
         return filename.endswith('.txt') or filename.endswith('.log') or filename.endswith('.mout')
 
     if len(sys.argv) > 1:
         filename = sys.argv[1]
         if not valid_extension(filename):
-            print("Invalid extension in filename '%s'" % filename)
-            print("This tool only supports the following extensions :'.txt','.log','.mout'")
+            _logger.error("Invalid extension in filename '%s'" % filename)
+            _logger.error("This tool only supports the following extensions :'.txt','.log','.mout'")
             exit(-1)
     else:
         filename = None
         newer_date = 0
         for f in os.listdir():
             date = os.path.getmtime(f)
             if date > newer_date and valid_extension(f):
                 newer_date = date
                 filename = f
     if filename is None:
-        print("File not found")
-        print("This tool only supports the following extensions :'.txt','.log','.mout'")
+        _logger.error("File not found")
+        _logger.error("This tool only supports the following extensions :'.txt','.log','.mout'")
         exit(-1)
 
     fname_out = None
     if filename.endswith('.txt'):
         fname_out = filename[:-len('txt')] + 'tsv'
     elif filename.endswith('.log'):
         fname_out = filename[:-len('log')] + 'tlog'
     elif filename.endswith('.mout'):
         fname_out = filename[:-len('mout')] + 'tmout'
     else:
-        print("Error in file type")
-        print("This tool only supports the following extensions :'.txt','.log','.mout'")
+        _logger.error("Error in file type")
+        _logger.error("This tool only supports the following extensions :'.txt','.log','.mout'")
         exit(-1)
 
     if fname_out is not None:
-        print("Processing File %s" % filename)
-        print("Creating File %s" % fname_out)
+        _logger.debug("Processing File %s" % filename)
+        _logger.debug("Creating File %s" % fname_out)
         if filename.endswith('txt'):
-            print("Processing Data File")
+            _logger.debug("Processing Data File")
             reformat_LTSpice_export(filename, fname_out)
         elif filename.endswith("log"):
             data = LTSpiceLogReader(filename)
             data.split_complex_values_on_datasets()
             data.export_data(fname_out)
         elif filename.endswith(".mout"):
             log_file = filename[:len('mout')] + 'log'
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/client_server/sim_client.py` & `PyLTSpice-4.0.4/PyLTSpice/client_server/sim_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 import zipfile
 import xmlrpc.client
 import io
 import pathlib
 import time
 from collections import OrderedDict
 from dataclasses import dataclass
-
+import logging
+_logger = logging.getLogger("PyLTSpice.SimClient")
 
 class SimClientInvalidRunId(LookupError):
     """Raised when asking for a run_no that doesn't exist"""
     ...
 
 @dataclass
 class JobInformation:
@@ -100,23 +101,23 @@
     NOTE: More elaborate algorithms such as managing multiple servers will be done on another class.
     """
 
     def __init__(self, host_address, port):
         self.server = xmlrpc.client.ServerProxy(f'{host_address}:{port}')
         # print(self.server.system.listMethods())
         self.session_id = self.server.start_session()
-        print("started ", self.session_id)
+        _logger.info("started ", self.session_id)
         self.started_jobs = OrderedDict()  # This list keeps track of started jobs on the server
         self.stored_jobs = OrderedDict()  # This list keeps track of finished simulations that haven't yet been transferred.
         self.completed_jobs = 0
         self.minimum_time_between_server_calls = 0.2  # Minimum time between server calls
         self._last_server_call = time.clock()
 
     def __del__(self):
-        print("closing session ", self.session_id)
+        _logger.info("closing session ", self.session_id)
         self.server.close_session(self.session_id)
 
     def run(self, circuit):
         """
         Sends the netlist identified with the argument "circuit" to the server, and it receives a run identifier
         (runno). Since the server can receive requests from different machines, this identifier is not guaranteed to be
         sequential.
@@ -143,15 +144,15 @@
             zip_data = zip_buffer.read()
 
             run_id = self.server.run(self.session_id, circuit_name, zip_data)
             job_info = JobInformation(run_number=run_id, file_dir=circuit_path.parent)
             self.started_jobs[job_info] = job_info
             return run_id
         else:
-            print(f"Circuit {circuit} doesn't exit")
+            _logger.error(f"Circuit {circuit} doesn't exit")
             return -1
         
     def get_runno_data(self, runno) -> str:
         """
         Returns the simulation output data inside a zip file name.
 
         :rtype: str
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/client_server/sim_server.py` & `PyLTSpice-4.0.4/PyLTSpice/client_server/sim_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #
 # Created:     23-02-2023
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 from typing import Tuple
 from xmlrpc.client import Binary
 from xmlrpc.server import SimpleXMLRPCServer
+import logging
+_logger = logging.getLogger("PyLTSpice.SimServer")
 
 import threading
 import zipfile
 import io
 from PyLTSpice.client_server.srv_sim_runner import ServerSimRunner
 import uuid
 
@@ -42,36 +44,36 @@
         self.server.register_instance(self)
         self.sessions = {}  # this will contain the session_id ids hashing their respective list of sim_tasks
         self.simulation_manager.start()
         self.server_thread = threading.Thread(target=self.server.serve_forever, name="ServerThread")
         self.server_thread.start()
 
     def run(self, session_id, circuit_name, zip_data):
-        print("Run ", session_id, circuit_name)
+        _logger.info("Run ", session_id, circuit_name)
         if session_id not in self.sessions:
             return -1  # This indicates that no job is started
         # Create a buffer from the zip data
         zip_buffer = io.BytesIO(zip_data.data)
-        print("Created the buffer")
+        _logger.debug("Created the buffer")
         # Extract the contents of the zip file
         with zipfile.ZipFile(zip_buffer, 'r') as zip_file:
-            print(zip_file.namelist())
+            _logger.debug(zip_file.namelist())
             zip_file.extract(circuit_name, self.output_folder)
 
-        print(f"Running simulation of {circuit_name}")
+        _logger.info(f"Running simulation of {circuit_name}")
         runno = self.simulation_manager.add_simulation(circuit_name)
         if runno != -1:
             self.sessions[session_id].append(runno)
         return runno
 
     def start_session(self):
         """Returns an unique key that represents the session. It will be later used to sort the sim_tasks belonging
         to the session."""
         session_id = str(uuid.uuid4())  # Needs to be a string, otherwise the rpc client can't handle it
-        print("Starting session ", session_id)
+        _logger.info("Starting session ", session_id)
         self.sessions[session_id] = []
         return session_id
 
     def status(self, session_id):
         """
         Returns a dictionary with task information. The key for the dictionary is the simulation identifier returned
         by the simulation start command. The value associated with each simulation identifier is another dictionary
@@ -79,23 +81,23 @@
 
             * 'completed' - whether the simulation is already finished
 
             * 'start' - time when the simulation was started
 
             * 'stop' - server time
         """
-        print("collecting status for ", session_id)
+        _logger.debug("collecting status for ", session_id)
         ret = []
         for task_info in self.simulation_manager.completed_tasks:
-            print(task_info)
+            _logger.debug(task_info)
             runno = task_info['runno']
             if runno in self.sessions[session_id]:
                 ret.append(runno)  # transfers the dictionary from the simulation_manager completed task
                 # to the return dictionary 
-        print("returning status", ret)
+        _logger.debug("returning status", ret)
         return ret
 
     def get_files(self, session_id, runno) -> Tuple[str, Binary]:
         if runno in self.sessions[session_id]:
 
             for task_info in self.simulation_manager.completed_tasks:
                 if runno == task_info['runno']:
@@ -113,16 +115,16 @@
     def close_session(self, session_id):
         """Cleans all the pending sim_tasks with """
         for runno in self.sessions[session_id]:
             self.simulation_manager.erase_files_of_runno(runno)
         return True  # Needs to return always something. None is not supported
 
     def stop_server(self):
-        print("stopping...ServerInterface")
+        _logger.info("stopping...ServerInterface")
         self.simulation_manager.stop()
         self.server.shutdown()
-        print("stopped...ServerInterface")
+        _logger.info("stopped...ServerInterface")
         return True  # Needs to return always something. None is not supported
 
     def running(self):
         return self.simulation_manager.running()
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/client_server/srv_sim_runner.py` & `PyLTSpice-4.0.4/PyLTSpice/client_server/srv_sim_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import threading
 import time
 from typing import Any, Callable, Union
 from pathlib import Path
 import zipfile
+import logging
+_logger = logging.getLogger("PyLTSpice.ServerSimRunner")
 
 from PyLTSpice.sim.sim_runner import SimRunner
 from PyLTSpice.sim.spice_editor import SpiceEditor
 
 
 def zip_files(raw_filename: Path, log_filename:Path):
     zip_filename = raw_filename.with_suffix('.zip')
@@ -67,34 +69,34 @@
                         'retcode': task.retcode,
                         'raw': task.raw_file,
                         'log': task.log_file,
                         'zipfile': zip_filename,
                         'start': task.start_time,
                         'stop': task.stop_time,
                     })
-                    print(task, "is finished")
+                    _logger.debug(task, "is finished")
                     del self.runner.sim_tasks[i]
-                    print(self.completed_tasks[-1])
-                    print(len(self.completed_tasks))
+                    _logger.debug(self.completed_tasks[-1])
+                    _logger.debug(len(self.completed_tasks))
 
             time.sleep(0.2)
             if self._stop is True:
                 break
         self.runner.wait_completion()
         self.runner.file_cleanup()
 
     def add_simulation(self, netlist: Union[str, Path, SpiceEditor], *, timeout: float = 600) -> int:
         """"""
-        print("starting ", netlist)
+        _logger.debug("starting ", netlist)
         task = self.runner.run(netlist, wait_resource=True, timeout=timeout, callback=zip_files)
         if task is None:
-            print("Failed to start task ", netlist)
+            _logger.error("Failed to start task ", netlist)
             return -1
         else:
-            print("Started task ", netlist, " with job_id", task.runno)
+            _logger.info("Started task ", netlist, " with job_id", task.runno)
             return task.runno
 
     def _erase_files_and_info(self, pos):
         task = self.completed_tasks[pos]
         for filename in ('log', 'raw', 'zipfile'):
             f = task[filename]
             if f.exists():
@@ -110,12 +112,12 @@
                 break
 
     def cleanup_completed(self):
         while len(self.completed_tasks):
             self._erase_files_and_info(0)
 
     def stop(self):
-        print("stopping...ServerSimRunner")
+        _logger.info("stopping...ServerSimRunner")
         self._stop = True
 
     def running(self):
         return self._stop is False
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/log/ltsteps.py` & `PyLTSpice-4.0.4/PyLTSpice/log/ltsteps.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 __copyright__ = "Copyright 2023, Fribourg Switzerland"
 
 import math
 import re
 from collections import OrderedDict
 from typing import Union, Iterable, List
 from ..utils.detect_encoding import detect_encoding
-
+import logging
+_logger = logging.getLogger("PyLTSpice.LTSteps")
 
 class LTComplex(object):
     """
     Class to represent complex numbers as exported by LTSpice
     """
     complex_match = re.compile(r"\((?P<mag>[^dB]*)(dB)?,(?P<ph>.*)°\)")
 
@@ -203,15 +204,15 @@
 
                 if go_header:
                     header_keys = []
                     for param in step.split():
                         header_keys.append(param.split('=')[0])
                     param_header = "\t".join(header_keys)
                     fout.write("Run\t%s\t%s" % (param_header, headers))
-                    print("Run\t%s\t%s" % (param_header, headers))
+                    _logger.debug("Run\t%s\t%s" % (param_header, headers))
                     go_header = False
                     # print("%s\t%s"% (run_no, param_values))
         else:
             fout.write("%s\t%s\t%s" % (run_no, param_values, line))
 
     fin.close()
     fout.close()
@@ -332,15 +333,15 @@
         # gain: vout_rms/vin_rms=1.99809 => Parameter
         # vout1m: v(out)=-0.0186257 at 0.001 => Point
         # fcutac=8.18166e+006 FROM 1.81834e+006 TO 1e+007 => AC Find Computation
         regx = re.compile(
                 r"^(?P<name>\w+)(:\s+.*)?=(?P<value>[\d\.E+\-\(\)dB,°]+)(( FROM (?P<from>[\d\.E+-]*) TO (?P<to>[\d\.E+-]*))|( at (?P<at>[\d\.E+-]*)))?",
                 re.IGNORECASE)
 
-        print("Processing LOG file", log_filename)
+        _logger.debug("Processing LOG file", log_filename)
         with open(log_filename, 'r', encoding=self.encoding) as fin:
             line = fin.readline()
 
             while line:
                 if line.startswith("N-Period"):
                     import pandas as pd
                     # Read number of periods
@@ -466,22 +467,22 @@
             measurements = []
             while line:
                 line = line.strip('\r\n')
                 if line.startswith("Measurement: "):
                     if dataname:  # If previous measurement was saved
                         # store the info
                         if len(measurements):
-                            print("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
+                            _logger.debug("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
                             self.measure_count += len(measurements)
                             for k, title in enumerate(headers):
                                 self.dataset[title] = [line[k] for line in measurements]
                         headers = []
                         measurements = []
                     dataname = line[13:]  # text which is after "Measurement: ". len("Measurement: ") -> 13
-                    print("Reading Measurement %s" % line[13:])
+                    _logger.debug("Reading Measurement %s" % line[13:])
                 else:
                     tokens = line.split("\t")
                     if len(tokens) >= 2:
                         try:
                             int(tokens[0])  # This instruction only serves to trigger the exception
                             meas = tokens[1:]  # [float(x) for x in tokens[1:]]
                             measurements.append(try_convert_values(meas))
@@ -490,28 +491,28 @@
                             if len(tokens) >= 3 and (tokens[2] == "FROM" or tokens[2] == 'at'):
                                 tokens[2] = dataname + '_' + tokens[2]
                             if len(tokens) >= 4 and tokens[3] == "TO":
                                 tokens[3] = dataname + "_TO"
                             headers = [dataname] + tokens[2:]
                             measurements = []
                     else:
-                        print("->", line)
+                        _logger.debug("->", line)
 
                 line = fin.readline()  # advance to the next line
 
             # storing the last data into the dataset
             if dataname:
-                print("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
+                _logger.debug("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
             if len(measurements):
                 self.measure_count += len(measurements)
                 for k, title in enumerate(headers):
                     self.dataset[title] = [line[k] for line in measurements]
 
-            print("%d measurements" % len(self.dataset))
-            print("Identified %d steps, read %d measurements" % (self.step_count, self.measure_count))
+            _logger.debug("%d measurements" % len(self.dataset))
+            _logger.info("Identified %d steps, read %d measurements" % (self.step_count, self.measure_count))
 
     def __getitem__(self, key):
         """
         __getitem__ implements
         :key: step or measurement name
         :return: step or measurement set
         :rtype: List[float]
@@ -639,15 +640,15 @@
         # print(tokens)
         if append_with_line_prefix is None:
             mode = 'w'  # rewrites the file
         else:
             mode = 'a'  # Appends an existing file
 
         if len(self.dataset) == 0:
-            print("Empty data set. Exiting without writing file.")
+            _logger.warning("Empty data set. Exiting without writing file.")
             return
 
         fout = open(export_file, mode, encoding=self.encoding)
 
         if append_with_line_prefix is not None:  # if an append it will write the filename first
             fout.write('user info\t')
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/log/semi_dev_op_reader.py` & `PyLTSpice-4.0.4/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/raw/raw_classes.py` & `PyLTSpice-4.0.4/PyLTSpice/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/raw/raw_convert.py` & `PyLTSpice-4.0.4/PyLTSpice/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/raw/raw_read.py` & `PyLTSpice-4.0.4/PyLTSpice/raw/raw_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,16 @@
 from pathlib import Path
 
 from .raw_classes import Axis, TraceRead, DummyTrace, SpiceReadException
 from ..utils.detect_encoding import detect_encoding
 
 import numpy as np
 from numpy import zeros, complex128, float32, float64, frombuffer, angle
-
+import logging
+_logger = logging.getLogger("PyLTSpice.RawRead")
 
 def read_float64(f):
     """
     Reads a 64-bit float value, normally associated with the plot X axis.
     The codification is done as follows:
 
     =====  === === === ===   === === === ===
@@ -375,15 +376,15 @@
         elif ch.decode(encoding='utf_16_le') == 'Tit':
             self.encoding = 'utf_16_le'
             sz_enc = 2
             line = 'Tit'
         else:
             raise RuntimeError("Unrecognized encoding")
         if self.verbose:
-            print("Reading the file with encoding ", self.encoding)
+            _logger.debug("Reading the file with encoding ", self.encoding)
         # Storing the filename as part of the dictionary
         self.raw_params = OrderedDict(Filename=raw_filename)  # Initializing the dict that contains all raw file info
         self.backannotations = []  # Storing backannotations
         header = []
         binary_start = 6
         while True:
             ch = raw_file.read(sz_enc).decode(encoding=self.encoding)
@@ -445,15 +446,15 @@
             return
 
         if kwargs.get("headeronly", False):
             raw_file.close()
             return
 
         if self.verbose:
-            print("File contains {} traces, reading {}".format(ivar,
+            _logger.info("File contains {} traces, reading {}".format(ivar,
                                                                len([trace for trace in self._traces
                                                                     if not isinstance(trace, DummyTrace)])))
 
         if self.raw_type == "Binary:":
             # Will start the reading of binary values
             # But first check whether how data is stored.
             self.block_size = (raw_file_size - binary_start) // self.nPoints
@@ -479,15 +480,15 @@
                             fun = consume4bytes
                         else:
                             fun = read_float32
                 scan_functions.append(fun)
 
             if "fastaccess" in self.raw_params["Flags"]:
                 if self.verbose:
-                    print("Binary RAW file with Fast access")
+                    _logger.debug("Binary RAW file with Fast access")
                 # Fast access means that the traces are grouped together.
                 for i, var in enumerate(self._traces):
                     if isinstance(var, DummyTrace):
                         # TODO: replace this by a seek
                         raw_file.read(self.nPoints * self.data_size)
                     else:
                         if self.data_size == 8:
@@ -502,36 +503,36 @@
                                 var.data = frombuffer(s, dtype=float64)
                             else:
                                 s = raw_file.read(self.nPoints * 4)
                                 var.data = frombuffer(s, dtype=float32)
 
             else:
                 if self.verbose:
-                    print("Binary RAW file with Normal access")
+                    _logger.debug("Binary RAW file with Normal access")
                 # This is the default save after a simulation where the traces are scattered
                 for point in range(self.nPoints):
                     for i, var in enumerate(self._traces):
                         value = scan_functions[i](raw_file)
                         if value is not None:
                             var.data[point] = value
 
         elif self.raw_type == "Values:":
             if self.verbose:
-                print("ASCII RAW File")
+                _logger.debug("ASCII RAW File")
             # Will start the reading of ASCII Values
             for point in range(self.nPoints):
                 first_var = True
                 for var in self._traces:
                     line = raw_file.readline().decode(encoding=self.encoding, errors='ignore')
                     if first_var:
                         first_var = False
                         s_point = line.split("\t", 1)[0]
 
                         if point != int(s_point):
-                            print("Error Reading File")
+                            _logger.error("Error Reading File")
                             break
                         value = line[len(s_point):-1]
                     else:
                         value = line[:-1]
                     if not isinstance(var, DummyTrace):
                         var.data[point] = float(value)
         else:
@@ -553,15 +554,15 @@
                 i += 1
 
         # Finally, Check for Step Information
         if "stepped" in self.raw_params["Flags"]:
             try:
                 self._load_step_information(raw_filename)
             except SpiceReadException:
-                print("LOG file not found or problems happened while reading it. Auto-detecting steps")
+                _logger.warning("LOG file not found or problems happened while reading it. Auto-detecting steps")
                 if has_axis:
                     number_of_steps = 0
                     for v in self.axis.data:
                         if v == self.axis.data[0]:
                             number_of_steps += 1
                 else:
                     number_of_steps = self.nPoints
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/raw/raw_write.py` & `PyLTSpice-4.0.4/PyLTSpice/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/rawplot.py` & `PyLTSpice-4.0.4/PyLTSpice/rawplot.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/ltspice_simulator.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/ltspice_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # Purpose:     Represents a LTspice tool and it's command line options
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     23-12-2016
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
-import logging
 import sys
 import os
 
 from pathlib import Path
 from typing import Union
+import logging
+_logger = logging.getLogger("PyLTSpice.LTSpiceSimulator")
 
 from .simulator import Simulator, run_function
 
 
 class LTspice(Simulator):
     """Stores the simulator location and command line options and is responsible for generating netlists and running
     simulations."""
@@ -46,24 +47,24 @@
         for exe in (  # Placed in order of preference. The first to be found will be used.
                 os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\LTspice.exe"),
                 r"C:\Program Files\ADI\LTspice\LTspice.exe",
                 r"C:\Program Files\LTC\LTspiceXVII\XVIIx64.exe",
                 r"C:\Program Files (x86)\LTC\LTspiceIV\scad3.exe",  # Legacy LTspice IV
         ):
             if os.path.exists(exe):
-                print(f"Using LTspice installed in : '{exe}' ")
+                _logger.debug(f"Using LTspice installed in : '{exe}' ")
                 spice_exe = [exe]
                 break
         else:
             spice_exe = []
-            print("================== ALERT! ====================")
-            print("Unable to find a LTSpice executable.")
-            print("A specific location of the LTSPICE can be set")
-            print("using the create_from(<location>) class method")
-            print("==============================================")
+            _logger.error("================== ALERT! ====================")
+            _logger.error("Unable to find a LTSpice executable.")
+            _logger.error("A specific location of the LTSPICE can be set")
+            _logger.error("using the create_from(<location>) class method")
+            _logger.error("==============================================")
 
         process_name = "XVIIx64.exe"
 
     ltspice_args = {
         'alt' : ['-alt'],  # Set solver to Alternate.
         'ascii'     : ['-ascii'],  # Use ASCII.raw files. Seriously degrades program performance.
         # 'batch': ['-b <path>'], # Used by run command: Run in batch mode.E.g. "ltspice.exe-b deck.cir" will leave the data infile deck.raw
@@ -166,13 +167,13 @@
         cmd_netlist = cls.spice_exe + ['-netlist'] + [circuit_file.as_posix()]
         # print(f'Creating netlist file from "{circuit_file}"', end='...')
         error = run_function(cmd_netlist)
 
         if error == 0:
             netlist = circuit_file.with_suffix('.net')
             if netlist.exists():
-                print("OK")
+                _logger.debug("OK")
                 return netlist
         msg = "Failed to create netlist"
         # print(msg)
         logging.error(msg)
         raise RuntimeError(msg)
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/ngspice_simulator.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/ngspice_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     23-02-2023
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 from pathlib import Path
+import logging
+_logger = logging.getLogger("PyLTSpice.NGSpiceSimulator")
 
 from .simulator import Simulator, run_function
 
 
 class NGspiceSimulator(Simulator):
     """Stores the simulator location and command line options and runs simulations."""
     spice_exe = ["C:/Apps/NGSpice64/bin/ngspice.exe"]
@@ -72,29 +74,29 @@
         :type parameter: str, optional
         :return: the correct formatting for the switch
         :rtype: list
         """
         ret = []  # This is an empty switch
         if switch in cls.ngspice_args:
             if switch in cls.default_run_switches:
-                print(f"Switch {switch} is already in the default switches")
+                _logger.info(f"Switch {switch} is already in the default switches")
                 return ret
             switch_list = cls.ngspice_args[switch]
             if len(switch_list) == 2:
                 param_token = switch_list[1]
                 if param_token == '<FILE>':
                     ret = [switch_list[0], parameter]
                 elif param_token == '<TERM>':
                     ret = [switch_list[0], parameter]
                 else:
-                    print(f"Invalid parameter {parameter} for switch '{switch}'")
+                    _logger.warning(f"Invalid parameter {parameter} for switch '{switch}'")
             else:
                 ret = switch_list
         else:
-            print(f"Invalid Switch {switch}")
+            _logger.warning(f"Invalid Switch {switch}")
         return ret
 
     @classmethod
     def run(cls, netlist_file, cmd_line_switches, timeout):
         logfile = Path(netlist_file).with_suffix('.log').as_posix()
         rawfile = Path(netlist_file).with_suffix('.raw').as_posix()
         cmd_run = cls.spice_exe + cmd_line_switches + ['-b'] + ['-o'] + [logfile] + ['-r'] + [rawfile] + [netlist_file]
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/process_callback.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/sim_analysis.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/sim_batch.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/sim_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,19 @@
 
 The callback function is optional. If  no callback function is given, the thread is terminated just after the
 simulation is finished.
 """
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2020, Fribourg Switzerland"
 
-import logging
 import os
 from pathlib import Path
 from typing import Callable, Any, Union
+import logging
+_logger = logging.getLogger("PyLTSpice.SimBatch")
 
 from ..sim.spice_editor import SpiceEditor
 from ..sim.simulator import Simulator
 from ..sim.run_task import RunTask
 from ..sim.sim_runner import SimRunner
 
 END_LINE_TERM = '\n'
@@ -214,21 +215,21 @@
             # ".step param run 1 2 1"
     )
     # do parameter sweep
     for res in range(5):
         # LTC.runs_to_do = range(2)
         LTC.set_parameters(ANA=res)
         raw, log = LTC.run().wait_results()
-        print("Raw file '%s' | Log File '%s'" % (raw, log))
+        _logger.debug("Raw file '%s' | Log File '%s'" % (raw, log))
     # Sim Statistics
-    print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
+    _logger.info('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
 
 
     def callback_function(raw_file, log_file):
-        print("Handling the simulation data of %s, log file %s" % (raw_file, log_file))
+        _logger.debug("Handling the simulation data of %s, log file %s" % (raw_file, log_file))
 
 
     LTC = SimCommander(meAbsPath + "\\test_files\\testfile.asc", parallel_sims=1)
     tstart = 0
     for tstop in (2, 5, 8, 10):
         tduration = tstop - tstart
         LTC.add_instruction(".tran {}".format(tduration), )
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/sim_runner.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/sim_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,21 +92,22 @@
 simulation is finished.
 """
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2020, Fribourg Switzerland"
 
 __all__ = ['SimRunner']
 
-import logging
 import os
 import shutil
 from pathlib import Path
 from time import sleep, thread_time as clock
 
 from typing import Callable, Union, Any, Type
+import logging
+_logger = logging.getLogger("PyLTSpice.SimRunner")
 
 from .process_callback import ProcessCallback
 from ..sim.run_task import RunTask
 from ..sim.simulator import Simulator
 from ..sim.spice_editor import SpiceEditor
 
 END_LINE_TERM = '\n'
@@ -160,22 +161,15 @@
             self.output_folder = None
 
         self.parallel_sims = parallel_sims
         self.sim_tasks = []
         # Create another logger for the SimRunner class
 
         # master_log_filename = self.circuit_radic + '.masterlog' TODO: create the JSON or YAML file
-        self.logger = logging.getLogger("SimRunner")
-        self.logger.setLevel(logging.INFO)
-        # redirect this logger to a file.
-        self.logger.addHandler(logging.FileHandler('SimRunner.log', mode='w'))
-        # if verbose is true, all log messages are also printed to the console
-        if verbose:
-            self.logger.addHandler(logging.StreamHandler())
-        self.logger.info("SimRunner started")
+        _logger.info("SimRunner started")
 
         self.runno = 0  # number of total runs
         self.failSim = 0  # number of failed simulations
         self.okSim = 0  # number of successful completed simulations
         # self.failParam = []  # collects for later user investigation of failed parameter sets
 
         # Gets a simulator.
@@ -187,17 +181,17 @@
         elif isinstance(simulator, (str, Path)):
             self.simulator = Simulator.create_from(simulator)
         else:
             raise TypeError("Invalid simulator type.")
 
     def __del__(self):
         """Class Destructor : Closes Everything"""
-        self.logger.debug("Waiting for all spawned sim_tasks to finish.")
+        _logger.debug("Waiting for all spawned sim_tasks to finish.")
         self.wait_completion(abort_all_on_timeout=True)  # Kill all pending simulations
-        self.logger.debug("Exiting SimCommander")
+        _logger.debug("Exiting SimCommander")
 
     def set_run_command(self, spice_tool: Union[str, Simulator]) -> None:
         """
         Manually setting the LTSpice run command
 
         :param spice_tool: String containing the path to the spice tool to be used, or alternatively the Simulator
             object.
@@ -272,18 +266,18 @@
 
     def create_netlist(self, asc_file: Union[str, Path]):
         """Creates a .net from an .asc using the LTSpice -netlist command line"""
         if not isinstance(asc_file, Path):
             asc_file = Path(asc_file)
         if asc_file.suffix == '.asc':
             if self.verbose:
-                self.logger.info("Creating Netlist")
+                _logger.info("Creating Netlist")
             return self.simulator.create_netlist(asc_file)
         else:
-            self.logger.info("Unable to create the Netlist from %s" % asc_file)
+            _logger.warning("Unable to create the Netlist from %s" % asc_file)
             return None
 
     def _prepare_sim(self, netlist: Union[str, Path, SpiceEditor], run_filename: str):
         """Internal function"""
         # update number of simulation
         self.runno += 1  # Incrementing internal simulation number
         # Harmonize the netlist into a Path object pointing to a netlist file on the right output folder
@@ -353,17 +347,17 @@
                             timeout=self.timeout, verbose=self.verbose)
                 self.sim_tasks.append(t)
                 t.start()
                 sleep(0.01)  # Give slack for the thread to start
                 return t  # Returns the task object
             sleep(0.1)  # Give Time for other simulations to end
         else:
-            self.logger.error("Timeout waiting for resources for simulation %d" % self.runno)
+            _logger.error("Timeout waiting for resources for simulation %d" % self.runno)
             if self.verbose:
-                self.logger.info("Timeout on launching simulation %d." % self.runno)
+                _logger.warning("Timeout on launching simulation %d." % self.runno)
             return None
 
     def run_now(self, netlist: Union[str, Path, SpiceEditor], *, switches=None, run_filename: str = None) -> (str, str):
         """
         Executes a simulation run with the conditions set by the user.
         Conditions are set by the set_parameter, set_component_value or add_instruction functions.
 
@@ -433,15 +427,15 @@
         simulator = Simulator
         process_name = simulator.process_name
         import psutil
         for proc in psutil.process_iter():
             # check whether the process name matches
 
             if proc.name() == process_name:
-                self.logger.info("killing ngspice", proc.pid)
+                _logger.info("killing ngspice", proc.pid)
                 proc.kill()
 
     def wait_completion(self, timeout=None, abort_all_on_timeout=False) -> bool:
         """
         This function will wait for the execution of all scheduled simulations to complete.
 
         :param timeout: Cancels the wait after the number of seconds specified by the timeout.
@@ -460,15 +454,15 @@
 
         while len(self.sim_tasks) > 0:
             sleep(1)
             self.updated_stats()
             if timeout is not None:
                 if sim_counters == (self.okSim, self.failSim):
                     timeout_counter += 1
-                    self.logger.info(timeout_counter, "timeout counter")
+                    _logger.info(timeout_counter, "timeout counter")
                 else:
                     timeout_counter = 0
 
                 if timeout_counter > timeout:
                     if abort_all_on_timeout:
                         self.kill_all_ltspice()
                     return False
@@ -483,30 +477,30 @@
         self.updated_stats()
         while len(self.workfiles):
             workfile = self.workfiles.pop(0)
             if workfile.suffix == '.net':
                 # Delete the log file if exists
                 logfile = workfile.with_suffix('.log')
                 if logfile.exists():
-                    self.logger.info("Deleting..." + logfile.name)
+                    _logger.info("Deleting..." + logfile.name)
                     logfile.unlink()
                 # Delete the raw file if exists
                 rawfile = workfile.with_suffix('.raw')
                 if rawfile.exists():
-                    self.logger.info("Deleting..." + rawfile.name)
+                    _logger.info("Deleting..." + rawfile.name)
                     rawfile.unlink()
 
                 # Delete the op.raw file if exists
                 oprawfile = workfile.with_suffix('.op.raw')
                 if oprawfile.exists():
-                    self.logger.info("Deleting..." + oprawfile.name)
+                    _logger.info("Deleting..." + oprawfile.name)
                     oprawfile.unlink()
 
             # Delete the file
-            self.logger.info("Deleting..." + workfile.name)
+            _logger.info("Deleting..." + workfile.name)
             workfile.unlink()
 
     def __iter__(self):
         return self
 
     def __next__(self):
         t0 = clock()
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/sim_stepping.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/sim_stepping.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 __copyright__ = "Copyright 2017, Fribourg Switzerland"
 
 import functools
 from typing import Callable, Any, Union
 from typing import Iterable
 import pathlib
 from functools import wraps
+import logging
+_logger = logging.getLogger("PyLTSpice.SimStepper")
 from .spice_editor import SpiceEditor
 from .sim_runner import SimRunner
 
 
 class StepInfo(object):
     def __init__(self, what: str, elem: str, iterable: Iterable):
         self.what = what
@@ -143,15 +145,15 @@
         """Returns the total number of simulations foreseen."""
         total = 1
         for step in self.iter_list:
             l = len(step)
             if l:
                 total *= l
             else:
-                print(step, " is empty")
+                _logger.debug(step, " is empty")
         return total
 
     def run_all(self, callback: Callable[[str, str], Any] = None, use_loadbias='Auto'):
         assert use_loadbias in ('Auto', 'Yes', 'No'), "use_loadbias argument must be 'Auto', 'Yes' or 'No'"
         if (use_loadbias == 'Auto' and self.total_number_of_simulations() > 10) or use_loadbias == 'Yes':
             # It will choose to use .SAVEBIAS/.LOADBIAS if the number of simulaitons is higher than 10
             # TODO: Make a first simulation and storing the bias
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/simulator.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/spice_editor.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/spice_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import os
 from pathlib import Path
 import traceback
 import re
 import logging
+_logger = logging.getLogger("PyLTSpice.SpiceEditor")
 from math import log, floor
 from typing import Union, List, Callable, Any
 from ..utils.detect_encoding import detect_encoding
 
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2021, Fribourg Switzerland"
 
@@ -277,29 +278,28 @@
 
     This class serves as subclass to the SpiceEditor class.
     """
 
     def __init__(self):
         self.subcircuits = {}
         self.netlist = []
-        self.logger = logging.getLogger("SpiceCircuit")
 
     def _getline_startingwith(self, substr: str) -> int:
         """Internal function. Do not use."""
         # This function returns the line number that starts with the substr string.
         # If the line is not found, then -1 is returned.
         substr_upper = substr.upper()
         for line_no, line in enumerate(self.netlist):
             if isinstance(line, SpiceCircuit):  # If it is a subcircuit it will simply ignore it.
                 continue
             line_upcase = _first_token_upped(line)
             if line_upcase == substr_upper:
                 return line_no
         error_msg = "line starting with '%s' not found in netlist" % substr
-        self.logger.error(error_msg)
+        _logger.error(error_msg)
         raise ComponentNotFoundError(error_msg)
 
     def _add_lines(self, line_iter):
         """Internal function. Do not use.
         Add a list of lines to the netlist."""
         for line in line_iter:
             cmd = get_line_command(line)
@@ -416,16 +416,16 @@
 
     def _set_model_and_value(self, component, value):
         """Internal function. Do not use."""
         prefix = component[0]  # Using the first letter of the component to identify what is it
         regex = component_replace_regexs.get(prefix, None)  # Obtain RegX to make the update
 
         if regex is None:
-            print("Component must start with one of these letters:\n", ','.join(REPLACE_REGXES.keys()))
-            print("Got '{}'".format(component))
+            _logger.error("Component must start with one of these letters:\n", ','.join(REPLACE_REGXES.keys()))
+            _logger.error("Got '{}'".format(component))
             return
 
         if isinstance(value, (int, float)):
             value = format_eng(value)
 
         line_no = self._getline_startingwith(component)
 
@@ -525,24 +525,24 @@
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX. NotImplementedError of there
                  isn't an associated regular expression for the component prefix.
         """
         prefix = component[0]  # Using the first letter of the component to identify what is it
         regex = component_replace_regexs.get(prefix, None)  # Obtain RegX to make the update
 
         if regex is None:
-            self.logger.warning("Component must start with one of these letters:\n", ','.join(REPLACE_REGXES.keys()))
-            self.logger.warning("Got '{}'".format(component))
+            _logger.warning("Component must start with one of these letters:\n", ','.join(REPLACE_REGXES.keys()))
+            _logger.warning("Got '{}'".format(component))
             raise NotImplementedError("Unsuported prefix {}".format(prefix))
 
         line_no = self._getline_startingwith(component)
         line = self.netlist[line_no]
         m = regex.match(line)
         if m is None:
             error_msg = 'Unsupported line "{}"\nExpected format is "{}"'.format(line, REPLACE_REGXES[prefix])
-            self.logger.error(error_msg)
+            _logger.error(error_msg)
             raise UnrecognizedSyntaxError(line, REPLACE_REGXES[prefix])
 
         info = m.groupdict()
         info['line'] = line_no  # adding the line number to the component information
         return info
 
     def get_parameter(self, param: str) -> str:
@@ -980,15 +980,15 @@
                 finished = self._add_lines(lines)
                 if not finished:
                     raise SyntaxError("Netlist with missing .END or .ENDS statements")
                 # else:
                 #     for _ in lines:  # Consuming the rest of the file.
                 #         pass  # print("Ignoring %s" % _)
         else:
-            self.logger.error("Netlist file not found")
+            _logger.error("Netlist file not found")
 
     @staticmethod
     def find_subckt_in_lib(library, subckt_name) -> Union['SpiceCircuit', None]:
         """
         Finds returns a Subckt from a library file.
 
         :param library: path to the library to search
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim/xyce_simulator.py` & `PyLTSpice-4.0.4/PyLTSpice/sim/xyce_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     14-03-2023
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
-import logging
 import sys
 import os
 
 from pathlib import Path
 from typing import Union
-
+import logging
+_logger = logging.getLogger("PyLTSpice.XYCESimulator")
 from .simulator import Simulator, run_function
 
 
 class XyceSimulator(Simulator):
     """Stores the simulator location and command line options and runs simulations."""
     spice_exe = ["C:/Program Files/Xyce 7.6 NORAD/bin/xyce.exe"]
     process_name = "XVIIx64.exe"
@@ -115,19 +115,19 @@
                     try:
                         int(parameter)
                     except ValueError:
                         pass
                     else:
                         ret = [switch_list[0], parameter]
                 else:
-                    print(f"Invalid parameter {parameter} for switch '{switch}'")
+                    _logger.warning(f"Invalid parameter {parameter} for switch '{switch}'")
             else:
                 ret = switch_list
         else:
-            print(f"Invalid Switch {switch}")
+            _logger.error(f"Invalid Switch {switch}")
         return ret
 
     @classmethod
     def run(cls, netlist_file, cmd_line_switches, timeout):
         cmd_run = cls.spice_exe + cmd_line_switches + [netlist_file]
         # start execution
         return run_function(cmd_run, timeout=timeout)
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/sim_batch.py` & `PyLTSpice-4.0.4/PyLTSpice/sim_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,23 +91,24 @@
 
 The callback function is optional. If  no callback function is given, the thread is terminated just after the
 simulation is finished.
 """
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2020, Fribourg Switzerland"
 
-import logging
 import os
 import pathlib
 import threading
 import time
 import traceback
 from time import sleep
 from typing import Callable, Union, Any, Tuple
 from warnings import warn
+import logging
+_logger = logging.getLogger("PyLTSpice.SimBatch")
 
 from .SpiceEditor import SpiceEditor
 from .simulator import clock_function, Simulator
 
 END_LINE_TERM = '\n'
 
 logging.basicConfig(filename='SpiceBatch.log', level=logging.INFO)
@@ -129,18 +130,14 @@
         self.netlist_file = netlist_file
         self.callback = callback
         self.retcode = -1  # Signals an error by default
         self.raw_file = None
         self.log_file = None
 
     def run(self):
-        # Setting up
-        logger = logging.getLogger("sim%d" % self.run_no)
-        logger.setLevel(logging.INFO)
-
         # Running the Simulation
 
         self.start_time = clock_function()
         if self.verbose:
             print(time.asctime(), ": Starting simulation %d" % self.run_no)
 
         # start execution
@@ -150,38 +147,38 @@
         sim_time = time.strftime("%H:%M:%S", time.gmtime(clock_function() - self.start_time))
         netlist_radic, extension = os.path.splitext(self.netlist_file)
         self.log_file = netlist_radic + '.log'
 
         # Cleanup everything
         if self.retcode == 0:
             # simulation successful
-            logger.info("Simulation Successful. Time elapsed: %s" % sim_time)
+            _logger.info("Simulation Successful. Time elapsed: %s" % sim_time)
             if self.verbose:
                 print(time.asctime() + ": Simulation Successful. Time elapsed %s:%s" % (sim_time, END_LINE_TERM))
 
             self.raw_file = netlist_radic + '.raw'
 
             if os.path.exists(self.raw_file) and os.path.exists(self.log_file):
                 if self.callback:
                     if self.verbose:
                         print("Calling the callback function")
                     try:
                         self.callback(self.raw_file, self.log_file)
                     except Exception as err:
                         error = traceback.format_tb(err)
-                        logger.error(error)
+                        _logger.error(error)
                 else:
                     if self.verbose:
                         print('No Callback')
             else:
-                logger.error("Simulation Raw file or Log file were not found")
+                _logger.error("Simulation Raw file or Log file were not found")
         else:
             # simulation failed
 
-            logger.warning(time.asctime() + ": Simulation Failed. Time elapsed %s:%s" % (sim_time, END_LINE_TERM))
+            _logger.warning(time.asctime() + ": Simulation Failed. Time elapsed %s:%s" % (sim_time, END_LINE_TERM))
             if os.path.exists(self.log_file):
                 old_log_file = self.log_file
                 self.log_file = netlist_radic + '.fail'
                 os.rename(old_log_file, self.log_file)
 
     def wait_results(self) -> Tuple[str, str]:
         """
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice/utils/detect_encoding.py` & `PyLTSpice-4.0.4/PyLTSpice/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice/utils/sweep_iterators.py` & `PyLTSpice-4.0.4/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/PyLTSpice.egg-info/PKG-INFO` & `PyLTSpice-4.0.4/PyLTSpice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.3
+Version: 4.0.4
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -947,23 +947,49 @@
 ```
 
 ### SemiDevOpReader.py ###
 
 This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information. A more detailed
 documentation is directly included in the source file docstrings.
 
+## Debug Logging
+The library uses the standard `logging` module. Three convenience functions have been added for easily changing logging 
+settings across the entire library. `PyLTSpice.all_loggers()` returns a list of all the logger's names, `PyLTSpice.set_log_level(logging.DEBUG)` 
+would set the library's logging level to debug, and `PyLTSpice.add_log_handler(my_handler)` would add `my_handler` as a handler for 
+all loggers.
+
+### Single Module Logging
+It is also possible to set the logging settings for a single module by using its name acquired from the `PyLTSpice.all_loggers()` 
+function. For example:
+
+```python
+import logging
+logging.basicConfig(level=logging.INFO)  # Set up the root logger first
+
+import PyLTSpice  # Import PyLTSpice to set the logging levels
+PyLTSpice.set_log_level(logging.DEBUG)  # Set PyLTSpice's global log level
+logging.getLogger("PyLTSpice.RawRead").level = logging.WARNING  # Set the log level for only RawRead to warning
+```
+Would set only `PyLTSpice.RawRead` file's logging level to warning while the other modules would remain at debug level. 
+_Make sure to initialize the root logger before importing the library to be able to see the logs._
+
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.4\
+  Improved usage of the logging library. (Thanks TSprech@GitHub)\
+  Included RunTask number in the log messages.\ 
+  Included milliseconds in the time elapsed calculation.
+
 * Version 4.0.3\
-  Fixing issue in elapsed time calculation.
+  Fixing issue in elapsed time calculation.\
   Fixing issue with the import of LTSpiceLogReader from LTSteps.py
 
 * Version 4.0.2\
   Changing list of Library dependencies.
 
 * Version 4.0.1\
   Bug fix on CLI for the Histogram.py and LTSteps.py
```

### Comparing `PyLTSpice-4.0.3/PyLTSpice.egg-info/SOURCES.txt` & `PyLTSpice-4.0.4/PyLTSpice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/README.md` & `PyLTSpice-4.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -258,23 +258,49 @@
 ```
 
 ### SemiDevOpReader.py ###
 
 This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information. A more detailed
 documentation is directly included in the source file docstrings.
 
+## Debug Logging
+The library uses the standard `logging` module. Three convenience functions have been added for easily changing logging 
+settings across the entire library. `PyLTSpice.all_loggers()` returns a list of all the logger's names, `PyLTSpice.set_log_level(logging.DEBUG)` 
+would set the library's logging level to debug, and `PyLTSpice.add_log_handler(my_handler)` would add `my_handler` as a handler for 
+all loggers.
+
+### Single Module Logging
+It is also possible to set the logging settings for a single module by using its name acquired from the `PyLTSpice.all_loggers()` 
+function. For example:
+
+```python
+import logging
+logging.basicConfig(level=logging.INFO)  # Set up the root logger first
+
+import PyLTSpice  # Import PyLTSpice to set the logging levels
+PyLTSpice.set_log_level(logging.DEBUG)  # Set PyLTSpice's global log level
+logging.getLogger("PyLTSpice.RawRead").level = logging.WARNING  # Set the log level for only RawRead to warning
+```
+Would set only `PyLTSpice.RawRead` file's logging level to warning while the other modules would remain at debug level. 
+_Make sure to initialize the root logger before importing the library to be able to see the logs._
+
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.4\
+  Improved usage of the logging library. (Thanks TSprech@GitHub)\
+  Included RunTask number in the log messages.\ 
+  Included milliseconds in the time elapsed calculation.
+
 * Version 4.0.3\
-  Fixing issue in elapsed time calculation.
+  Fixing issue in elapsed time calculation.\
   Fixing issue with the import of LTSpiceLogReader from LTSteps.py
 
 * Version 4.0.2\
   Changing list of Library dependencies.
 
 * Version 4.0.1\
   Bug fix on CLI for the Histogram.py and LTSteps.py
```

### Comparing `PyLTSpice-4.0.3/doc/conf.py` & `PyLTSpice-4.0.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/pyproject.toml` & `PyLTSpice-4.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PyLTSpice"
-version = "4.0.3"
+version = "4.0.4"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate LTSpice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `PyLTSpice-4.0.3/tests/test_ltsteps.py` & `PyLTSpice-4.0.4/tests/test_ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/tests/unittest/sweep_iterators/sweep_iterators_unittest.py` & `PyLTSpice-4.0.4/tests/unittest/sweep_iterators/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.3/tests/unittest/test_pyltspice.py` & `PyLTSpice-4.0.4/tests/unittest/test_pyltspice.py`

 * *Files identical despite different names*

