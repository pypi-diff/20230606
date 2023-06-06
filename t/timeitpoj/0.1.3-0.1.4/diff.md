# Comparing `tmp/timeitpoj-0.1.3.tar.gz` & `tmp/timeitpoj-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeitpoj-0.1.3.tar", max compression
+gzip compressed data, was "timeitpoj-0.1.4.tar", max compression
```

## Comparing `timeitpoj-0.1.3.tar` & `timeitpoj-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1948 2023-06-06 06:50:58.042514 timeitpoj-0.1.3/README.md
--rwxr-xr-x   0        0        0      960 2023-06-06 07:03:09.969381 timeitpoj-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0       35 2023-06-06 06:50:58.047770 timeitpoj-0.1.3/timeitpoj/__init__.py
--rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.3/timeitpoj/task_report.py
--rwxr-xr-x   0        0        0     9594 2023-06-06 06:50:38.356402 timeitpoj-0.1.3/timeitpoj/timeit.py
--rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.3/timeitpoj/utils/__init__.py
--rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.3/timeitpoj/utils/constants.py
--rwxr-xr-x   0        0        0     1141 2023-06-05 12:28:55.956023 timeitpoj-0.1.3/timeitpoj/utils/misc.py
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 timeitpoj-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1944 2023-06-06 07:05:21.764410 timeitpoj-0.1.4/README.md
+-rwxr-xr-x   0        0        0      960 2023-06-06 07:05:28.342170 timeitpoj-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0       35 2023-06-06 06:50:58.047770 timeitpoj-0.1.4/timeitpoj/__init__.py
+-rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.4/timeitpoj/task_report.py
+-rwxr-xr-x   0        0        0     9594 2023-06-06 06:50:38.356402 timeitpoj-0.1.4/timeitpoj/timeit.py
+-rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.4/timeitpoj/utils/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.4/timeitpoj/utils/constants.py
+-rwxr-xr-x   0        0        0     1141 2023-06-05 12:28:55.956023 timeitpoj-0.1.4/timeitpoj/utils/misc.py
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 timeitpoj-0.1.4/PKG-INFO
```

### Comparing `timeitpoj-0.1.3/README.md` & `timeitpoj-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python Timeit
+# Timeitpoj
 
 yet another random library for measuring python performance
 
 ## Usage in production
 
 if you do not need to measure performance of your code in a production environment, simply set the environment
 variable `TIME_IT` to`false`
```

### Comparing `timeitpoj-0.1.3/pyproject.toml` & `timeitpoj-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeitpoj"
-version = "0.1.3"
+version = "0.1.4"
 description = "yet another random library for measuring python performance"
 authors = ["Jari Van Melckebeke <jarivanmelckebeke@gmail.com>"]
 maintainers = ["Jari Van Melckebeke <jarivanmelckebeke@gmail.com>"]
 repository = "https://github.com/jvanmelckebeke/timeitpoj"
 homepage = "https://github.com/jvanmelckebeke/timeitpoj"
```

### Comparing `timeitpoj-0.1.3/timeitpoj/task_report.py` & `timeitpoj-0.1.4/timeitpoj/task_report.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.3/timeitpoj/timeit.py` & `timeitpoj-0.1.4/timeitpoj/timeit.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.3/timeitpoj/utils/misc.py` & `timeitpoj-0.1.4/timeitpoj/utils/misc.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.3/PKG-INFO` & `timeitpoj-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeitpoj
-Version: 0.1.3
+Version: 0.1.4
 Summary: yet another random library for measuring python performance
 Home-page: https://github.com/jvanmelckebeke/timeitpoj
 License: MIT
 Keywords: timeit,performance,benchmark,time,measure
 Author: Jari Van Melckebeke
 Author-email: jarivanmelckebeke@gmail.com
 Maintainer: Jari Van Melckebeke
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/jvanmelckebeke/timeitpoj
 Description-Content-Type: text/markdown
 
-# Python Timeit
+# Timeitpoj
 
 yet another random library for measuring python performance
 
 ## Usage in production
 
 if you do not need to measure performance of your code in a production environment, simply set the environment
 variable `TIME_IT` to`false`
```

