# Comparing `tmp/vmt-0.0.0b7.tar.gz` & `tmp/vmt-0.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmt-0.0.0b7.tar", last modified: Mon Jun  5 19:51:16 2023, max compression
+gzip compressed data, was "vmt-0.0.0b8.tar", last modified: Tue Jun  6 19:16:29 2023, max compression
```

## Comparing `vmt-0.0.0b7.tar` & `vmt-0.0.0b8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-05 19:51:16.887674 vmt-0.0.0b7/
--rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 vmt-0.0.0b7/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-05 19:51:16.887674 vmt-0.0.0b7/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     9847 2022-09-22 03:13:29.000000 vmt-0.0.0b7/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      570 2023-06-05 19:50:31.000000 vmt-0.0.0b7/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-05 19:51:16.887674 vmt-0.0.0b7/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-05 19:51:16.887674 vmt-0.0.0b7/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-05 19:51:16.887674 vmt-0.0.0b7/src/vmt/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 vmt-0.0.0b7/src/vmt/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1628 2022-09-22 02:48:23.000000 vmt-0.0.0b7/src/vmt/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6218 2022-09-22 02:48:23.000000 vmt-0.0.0b7/src/vmt/build.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6418 2023-06-05 19:50:19.000000 vmt-0.0.0b7/src/vmt/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 vmt-0.0.0b7/src/vmt/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3515 2023-05-01 04:19:25.000000 vmt-0.0.0b7/src/vmt/media.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4987 2022-07-11 05:05:28.000000 vmt-0.0.0b7/src/vmt/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1669 2023-04-22 05:55:06.000000 vmt-0.0.0b7/src/vmt/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2250 2022-09-22 02:48:23.000000 vmt-0.0.0b7/src/vmt/search.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1070 2022-10-09 04:34:45.000000 vmt-0.0.0b7/src/vmt/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2091 2022-09-22 02:48:23.000000 vmt-0.0.0b7/src/vmt/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-05 19:51:16.887674 vmt-0.0.0b7/src/vmt.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-05 19:51:16.000000 vmt-0.0.0b7/src/vmt.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      428 2023-06-05 19:51:16.000000 vmt-0.0.0b7/src/vmt.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-05 19:51:16.000000 vmt-0.0.0b7/src/vmt.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-06-05 19:51:16.000000 vmt-0.0.0b7/src/vmt.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-06-05 19:51:16.000000 vmt-0.0.0b7/src/vmt.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-06-05 19:51:16.000000 vmt-0.0.0b7/src/vmt.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34742 2022-07-14 19:37:15.000000 vmt-0.0.0b8/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-06 19:16:29.952933 vmt-0.0.0b8/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     9847 2022-09-22 03:13:29.000000 vmt-0.0.0b8/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      570 2023-06-06 19:14:37.000000 vmt-0.0.0b8/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-06 19:16:29.952933 vmt-0.0.0b8/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/src/vmt/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1628 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6168 2023-06-06 19:14:23.000000 vmt-0.0.0b8/src/vmt/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6418 2023-06-05 19:50:19.000000 vmt-0.0.0b8/src/vmt/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     3515 2023-05-01 04:19:25.000000 vmt-0.0.0b8/src/vmt/media.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4987 2022-07-11 05:05:28.000000 vmt-0.0.0b8/src/vmt/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1669 2023-04-22 05:55:06.000000 vmt-0.0.0b8/src/vmt/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2250 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1070 2022-10-09 04:34:45.000000 vmt-0.0.0b8/src/vmt/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2091 2022-09-22 02:48:23.000000 vmt-0.0.0b8/src/vmt/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-06 19:16:29.952933 vmt-0.0.0b8/src/vmt.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)    10185 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      428 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       37 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-06-06 19:16:29.000000 vmt-0.0.0b8/src/vmt.egg-info/top_level.txt
```

### Comparing `vmt-0.0.0b7/LICENSE` & `vmt-0.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/PKG-INFO` & `vmt-0.0.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmt
-Version: 0.0.0b7
+Version: 0.0.0b8
 Summary: Video Media Tracker. Local, and simple method for watching and tracking a video media library.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/vmt
 Keywords: mpv
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vmt-0.0.0b7/README.md` & `vmt-0.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/pyproject.toml` & `vmt-0.0.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vmt"
-version = "0.0.0.b7"
+version = "0.0.0.b8"
 description = "Video Media Tracker. Local, and simple method for watching and tracking a video media library."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "mpv" ]
 dependencies = [
     "python-magic",
     "loadconf",
```

### Comparing `vmt-0.0.0b7/src/vmt/__main__.py` & `vmt-0.0.0b8/src/vmt/__main__.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/build.py` & `vmt-0.0.0b8/src/vmt/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,18 @@
     Optionally recursive
     """
     user_system = system()
 
     def recursive_filter():
         escape_dir = re.escape(dir)
         for item in filters:
+            escape_item = re.escape(item)
             if user_system == "Windows":
-                escape_item = re.escape(item)
-                escape_item = f"{escape_item}\\\\"
+                escape_item = escape_item + "\\\\"
             else:
-                escape_item = re.escape(item)
                 escape_item = f"{escape_item}/"
 
             if re.search(escape_item, escape_dir):
                 return True
         return False
 
     def non_recursive_filter():
@@ -174,15 +173,15 @@
                 continue
             else:
                 skip_dir = False
                 break
         if skip_dir:
             continue
         if user_system == "Windows":
-            add_dir = dirpath.replace(f'{user.settings["base_dir"]}\\', "")
+            add_dir = dirpath.replace(user.settings["base_dir"] + "\\", "")
         else:
             add_dir = dirpath.replace(f'{user.settings["base_dir"]}/', "")
         if filter_directory(add_dir, user.stored["filters_file"], args):
             continue
         valid_dirs[add_dir] = {}
         valid_dirs[add_dir]["watching"] = None
         title = auto_title(add_dir, user_system)
```

### Comparing `vmt-0.0.0b7/src/vmt/config.py` & `vmt-0.0.0b8/src/vmt/config.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/media.py` & `vmt-0.0.0b8/src/vmt/media.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/options.py` & `vmt-0.0.0b8/src/vmt/options.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/prompts.py` & `vmt-0.0.0b8/src/vmt/prompts.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/search.py` & `vmt-0.0.0b8/src/vmt/search.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/system.py` & `vmt-0.0.0b8/src/vmt/system.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt/utils.py` & `vmt-0.0.0b8/src/vmt/utils.py`

 * *Files identical despite different names*

### Comparing `vmt-0.0.0b7/src/vmt.egg-info/PKG-INFO` & `vmt-0.0.0b8/src/vmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmt
-Version: 0.0.0b7
+Version: 0.0.0b8
 Summary: Video Media Tracker. Local, and simple method for watching and tracking a video media library.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/vmt
 Keywords: mpv
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

