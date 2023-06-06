# Comparing `tmp/python-printr-2.8.tar.gz` & `tmp/python-printr-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-printr-2.8.tar", last modified: Tue May 30 12:55:46 2023, max compression
+gzip compressed data, was "python-printr-2.9.tar", last modified: Tue Jun  6 13:18:28 2023, max compression
```

## Comparing `python-printr-2.8.tar` & `python-printr-2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:55:46.375472 python-printr-2.8/
--rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-2.8/.gitignore
--rw-rw-rw-   0        0        0     3350 2023-05-30 12:55:46.375472 python-printr-2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3092 2023-03-11 18:19:37.000000 python-printr-2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 12:55:46.369478 python-printr-2.8/printr/
--rw-rw-rw-   0        0        0     7818 2023-05-30 12:55:28.000000 python-printr-2.8/printr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:55:46.374473 python-printr-2.8/python_printr.egg-info/
--rw-rw-rw-   0        0        0     3350 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-30 12:55:46.000000 python-printr-2.8/python_printr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 12:55:45.000000 python-printr-2.8/python_printr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-30 12:55:46.375472 python-printr-2.8/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-05-30 12:55:41.000000 python-printr-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:18:28.671469 python-printr-2.9/
+-rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-2.9/.gitignore
+-rw-rw-rw-   0        0        0     3350 2023-06-06 13:18:28.671469 python-printr-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3092 2023-03-11 18:19:37.000000 python-printr-2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 13:18:28.666472 python-printr-2.9/printr/
+-rw-rw-rw-   0        0        0     7817 2023-06-06 13:18:18.000000 python-printr-2.9/printr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:18:28.670469 python-printr-2.9/python_printr.egg-info/
+-rw-rw-rw-   0        0        0     3350 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-06 13:18:28.672469 python-printr-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-06-06 13:18:24.000000 python-printr-2.9/setup.py
```

### Comparing `python-printr-2.8/PKG-INFO` & `python-printr-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 2.8
+Version: 2.9
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

### Comparing `python-printr-2.8/README.md` & `python-printr-2.9/README.md`

 * *Files identical despite different names*

### Comparing `python-printr-2.8/printr/__init__.py` & `python-printr-2.9/printr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,33 @@
         self.filename = filename
         if not log_filepath:
             log_filepath = f'{os.getcwd()}/{filename}.txt'
         self.log_filepath = log_filepath
         self.max_lines = max_lines
         self.log_to_file = log_to_file
 
+        if level == 'info':
+            self.level = logging.INFO
+        elif level == 'debug':
+            self.level = logging.DEBUG
+
         logger = logging.getLogger(__name__)
-        logger.setLevel(logging.DEBUG)
+        logger.setLevel(self.level)
 
         if log_to_file:
             log_file = logging.FileHandler(log_filepath, encoding='utf-8')
             log_format = logging.Formatter(fmt='%(message)s')
             log_file.setFormatter(log_format)
             logger.addHandler(log_file)
             self.log_file = log_file
             
             logger.info('') # add line break in between runs in log file
             log_format = logging.Formatter(fmt='%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
             log_file.setFormatter(log_format)
 
-        if level == 'info':
-            self.level = logging.INFO
-        elif level == 'debug':
-            self.level = logging.DEBUG
         coloredlogs.install(level=self.level, logger=logger, fmt='%(message)s')
         self.logger = logger
 
         self.indent = ''
         
         if not name:
             name = filename
```

### Comparing `python-printr-2.8/python_printr.egg-info/PKG-INFO` & `python-printr-2.9/python_printr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 2.8
+Version: 2.9
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
```

