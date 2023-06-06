# Comparing `tmp/metarace-tagreg-1.0.0.tar.gz` & `tmp/metarace-tagreg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ndf/dev/metarace/metarace-tagreg/dist/tmph9zu776d/metarace-tagreg-1.0.0.tar", last modified: Wed Nov 23 10:45:50 2022, max compression
+gzip compressed data, was "/home/ndf/dev/metarace/metarace-tagreg/dist/.tmp-x2gs8q9m/metarace-tagreg-1.0.1.tar", last modified: Tue Jun  6 07:37:31 2023, max compression
```

## Comparing `metarace-tagreg-1.0.0.tar` & `metarace-tagreg-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1063 2022-11-13 23:56:28.000000 metarace-tagreg-1.0.0/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)      894 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      385 2022-11-23 10:32:23.000000 metarace-tagreg-1.0.0/README.md
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)      894 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      278 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       39 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/entry_points.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        7 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/metarace_tagreg.egg-info/top_level.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)      679 2022-11-23 10:29:23.000000 metarace-tagreg-1.0.0/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2022-11-23 10:45:50.000000 metarace-tagreg-1.0.0/setup.cfg
--rw-r--r--   0 ndf       (1000) ndf       (1000)    35786 2022-11-23 10:13:34.000000 metarace-tagreg-1.0.0/tagreg.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1063 2022-11-13 23:56:28.000000 metarace-tagreg-1.0.1/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      897 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      388 2023-06-06 07:36:17.000000 metarace-tagreg-1.0.1/README.md
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      897 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      278 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       39 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/entry_points.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       16 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        7 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/metarace_tagreg.egg-info/top_level.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      686 2023-06-06 07:27:08.000000 metarace-tagreg-1.0.1/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-06-06 07:37:31.000000 metarace-tagreg-1.0.1/setup.cfg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    35530 2023-06-05 05:16:22.000000 metarace-tagreg-1.0.1/tagreg.py
```

### Comparing `metarace-tagreg-1.0.0/LICENSE` & `metarace-tagreg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metarace-tagreg-1.0.0/PKG-INFO` & `metarace-tagreg-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace-tagreg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Transponder allocation tool
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace-tagreg
 Keywords: transponder
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Other/Nonlisted Topic
@@ -20,20 +20,17 @@
 decoder.
 
 ![tagreg screenshot](screenshot.png "tagreg")
 
 ## Requirements
 
    - Gtk >= 3.0
-   - metarace >= 2.0
+   - metarace >= 2.1.0
 
 
 ## Installation
 
 [Install metarace](https://github.com/ndf-zz/metarace#installation)
-and the required system packages:
+and the required system packages then install tagreg using pip:
 
-	# apt install gir1.2-gtk-3.0
-
-Then install tagreg using pip:
-
-	$ pip3 install metarace-tagreg
+	$ sudo apt install gir1.2-gtk-3.0
+	$ pip install metarace-tagreg
```

### Comparing `metarace-tagreg-1.0.0/metarace_tagreg.egg-info/PKG-INFO` & `metarace-tagreg-1.0.1/metarace_tagreg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace-tagreg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Transponder allocation tool
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace-tagreg
 Keywords: transponder
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Other/Nonlisted Topic
@@ -20,20 +20,17 @@
 decoder.
 
 ![tagreg screenshot](screenshot.png "tagreg")
 
 ## Requirements
 
    - Gtk >= 3.0
-   - metarace >= 2.0
+   - metarace >= 2.1.0
 
 
 ## Installation
 
 [Install metarace](https://github.com/ndf-zz/metarace#installation)
-and the required system packages:
+and the required system packages then install tagreg using pip:
 
-	# apt install gir1.2-gtk-3.0
-
-Then install tagreg using pip:
-
-	$ pip3 install metarace-tagreg
+	$ sudo apt install gir1.2-gtk-3.0
+	$ pip install metarace-tagreg
```

### Comparing `metarace-tagreg-1.0.0/pyproject.toml` & `metarace-tagreg-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace-tagreg"
-version = "1.0.0"
+version = "1.0.1"
 description = "Transponder allocation tool"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text = "MIT"}
 keywords = ["transponder"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
@@ -16,15 +16,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Other/Nonlisted Topic",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "metarace",
+    "metarace>=2.1.0",
 ]
 [project.urls]
 homepage = "https://github.com/ndf-zz/metarace-tagreg"
 
 [project.scripts]
 tagreg = "tagreg:main"
```

### Comparing `metarace-tagreg-1.0.0/tagreg.py` & `metarace-tagreg-1.0.1/tagreg.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import sys
 import gi
 import logging
 import metarace
 import os
 import csv
+from time import sleep
 from metarace import tod
 from metarace.jsonconfig import config
 from metarace.riderdb import riderdb
 from metarace.decoder.rrs import rrs
 from metarace.decoder.rru import rru
 from metarace.decoder.thbc import thbc
 
@@ -445,21 +446,20 @@
         csvfile = chooseCsvFile(title='Export Chipfile or Rider List',
                                 mode=Gtk.FileChooserAction.SAVE,
                                 parent=self._window,
                                 path=os.getcwd(),
                                 hintfile='chipfile.csv')
         if csvfile is not None:
             try:
-                self._riderdb.save(
-                    csvfile, ['refid', 'no', 'series', 'first', 'last', 'cat'])
-                _log.info('Saved %d riders to %s', len(self._riderdb), csvfile)
+                count = self._riderdb.save_chipfile(csvfile)
+                _log.info('Saved %d refids to %s', count, csvfile)
 
             except Exception as e:
-                _log.error('%s writing to csv %s: %s', e.__class__.__name__,
-                           csvfile, e)
+                _log.error('%s writing chipfile csv %s: %s',
+                           e.__class__.__name__, csvfile, e)
             self._numberEntry.grab_focus()
 
 
 class tagreg(Gtk.Window):
     """Transponder reader and registration tool"""
 
     def __init__(self):
@@ -858,16 +858,16 @@
 
         self._decoderStat.update(bg=bg, label=nt.meridiem())
         return True
 
     def run(self):
         _log.debug('run')
         self._loadconfig()
-        with metarace.resource_file(metarace.LOGO) as f:
-            Gtk.Window.set_default_icon_from_file(str(f))
+        Gtk.Window.set_default_icon_from_file(
+            metarace.default_file(metarace.LOGO))
         self.show()
         GLib.idle_add(self._reconnect)
         GLib.timeout_add_seconds(1, self._timeout)
 
     def _loadconfig(self):
         """Check options and load state from current directory"""
         cr = config({
@@ -877,20 +877,15 @@
                 'mode': 0,
                 'checkout': {},
                 'checkin': {}
             }
         })
         cr.add_section('tagreg')
         cr.merge(metarace.sysconf, 'tagreg')
-        if os.path.exists(_CONFIGFILE):
-            try:
-                with open(_CONFIGFILE) as f:
-                    cr.read(f)
-            except Exception as e:
-                _log.error('%s reading config: %s', e.__class__.__name__, e)
+        cr.load(_CONFIGFILE)
 
         self._decoderSelect.set_active_id(
             cr.get_str('tagreg', 'decodertype', _DEFTYPE))
         self._decoderEntry.set_text(
             cr.get_str('tagreg', 'decoderport', _DEFPORT))
         self._modeBox.set_current_page(cr.get_posint('tagreg', 'mode', 0))
 
@@ -951,14 +946,15 @@
     configpath = metarace.config_path(configpath)
     if configpath is None:
         _log.error(u'Unable to open meet folder %r', sys.argv[1])
         sys.exit(1)
     lf = metarace.lockpath(configpath)
     if lf is None:
         _log.error(u'Unable to lock meet folder, already in use')
+        sleep(2)
         sys.exit(1)
     _log.debug(u'Entering meet folder %r', configpath)
     os.chdir(configpath)
     app = tagreg()
     app.run()
     return Gtk.main()
```

