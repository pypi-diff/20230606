# Comparing `tmp/qosd-20230529.tar.gz` & `tmp/qosd-20230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qosd-20230529.tar", last modified: Mon May 29 10:39:57 2023, max compression
+gzip compressed data, was "qosd-20230530.tar", last modified: Tue Jun  6 21:18:53 2023, max compression
```

## Comparing `qosd-20230529.tar` & `qosd-20230530.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 10:39:57.911336 qosd-20230529/
--rw-rw-r--   0 l         (1000) l         (1000)     2087 2023-05-29 10:39:57.911336 qosd-20230529/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)     1782 2023-05-29 10:37:44.000000 qosd-20230529/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      605 2023-05-18 15:02:10.000000 qosd-20230529/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-05-29 10:39:57.911336 qosd-20230529/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 10:39:57.911336 qosd-20230529/src/
--rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-18 08:26:03.000000 qosd-20230529/src/__init__.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-05-29 10:39:57.911336 qosd-20230529/src/qosd.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     2087 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      246 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       35 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       54 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)       14 2023-05-29 10:39:57.000000 qosd-20230529/src/qosd.egg-info/top_level.txt
--rwxrwxr-x   0 l         (1000) l         (1000)     8150 2023-05-29 10:33:05.000000 qosd-20230529/src/qosd.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-06-06 21:18:53.172199 qosd-20230530/
+-rw-rw-r--   0 l         (1000) l         (1000)     2087 2023-06-06 21:18:53.172199 qosd-20230530/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)     1782 2023-05-29 10:37:44.000000 qosd-20230530/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      605 2023-05-18 15:02:10.000000 qosd-20230530/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-06-06 21:18:53.172199 qosd-20230530/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-06-06 21:18:53.172199 qosd-20230530/src/
+-rw-rw-r--   0 l         (1000) l         (1000)        0 2023-05-18 08:26:03.000000 qosd-20230530/src/__init__.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-06-06 21:18:53.172199 qosd-20230530/src/qosd.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     2087 2023-06-06 21:18:53.000000 qosd-20230530/src/qosd.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      246 2023-06-06 21:18:53.000000 qosd-20230530/src/qosd.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-06-06 21:18:53.000000 qosd-20230530/src/qosd.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       35 2023-06-06 21:18:53.000000 qosd-20230530/src/qosd.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       54 2023-06-06 21:18:53.000000 qosd-20230530/src/qosd.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       14 2023-06-06 21:18:53.000000 qosd-20230530/src/qosd.egg-info/top_level.txt
+-rwxrwxr-x   0 l         (1000) l         (1000)     8496 2023-05-30 18:57:13.000000 qosd-20230530/src/qosd.py
```

### Comparing `qosd-20230529/PKG-INFO` & `qosd-20230530/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qosd
-Version: 20230529
+Version: 20230530
 Summary: QOSD for python
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/qosd
 Keywords: osd,on-screen-display,tail
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `qosd-20230529/README.md` & `qosd-20230530/README.md`

 * *Files identical despite different names*

### Comparing `qosd-20230529/pyproject.toml` & `qosd-20230530/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qosd-20230529/src/qosd.egg-info/PKG-INFO` & `qosd-20230530/src/qosd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qosd
-Version: 20230529
+Version: 20230530
 Summary: QOSD for python
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/qosd
 Keywords: osd,on-screen-display,tail
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `qosd-20230529/src/qosd.py` & `qosd-20230530/src/qosd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-VERSION = "20230529"
+VERSION = "20230530"
 DESCRIPTION = "display text over your Xorg screen"
 EXAMPLES = """examples:
 $ qosd hello
 $ tail -f /var/log/{messages,auth.log} | qosd -
 """
 
 from pathlib import Path
@@ -76,14 +76,15 @@
             x, y = sdim.width() - (w + ox), (sdim.height() / 2 - h / 2) + oy
         self.move(x, y)
         self.resize(w, h)
 
 class Qosd(object):
     TIMEOUT = 3
     MAXLINES = 30
+    STDIN_REFRESH_DELAY = 0.1 * 1000
 
     def __init__(self, style, opacity, timeout=TIMEOUT, maxlines=MAXLINES, position=Qosd_win.POSITION, offset=(0,0), no_input=False):
         self.maxlines = maxlines
         self.app = QtWidgets.QApplication([])
         self.win = Qosd_win(self, style, opacity, position, offset, no_input)
         self.text_log = ""
         self.win.show()
@@ -113,14 +114,16 @@
 
     def text_stdin(self):
         flags = fcntl.fcntl(sys.stdin, fcntl.F_GETFL)
         fcntl.fcntl(sys.stdin, fcntl.F_SETFL, flags | os.O_NONBLOCK)
         self.stdin = QtCore.QSocketNotifier(sys.stdin.fileno(), QtCore.QSocketNotifier.Read, self.win)
         self.stdin.activated.connect(self._cb_read_stdin)
         self.stdin.setEnabled(True)
+        self.next_stdin = QtCore.QTimer()
+        self.next_stdin.timeout.connect(self._cb_next_stdin)
 
     def run(self):
         self.app.exec()
 
     def exit(self):
         self.win.close()
         self.app.exit()
@@ -144,28 +147,35 @@
             self.hide_to.start(int(self.hide_timeout * 1000))
 
     def hide_to_stop(self):
         if self.hide_to:
             self.hide_to.stop()
 
     def _cb_read_stdin(self):
+        text = ""
         while True:
             try:
                 data = os.read(sys.stdin.fileno(), 1024)
             except Exception as e:
                 # nothing to read
                 break
             if not data:
                 # stdin is closed, disable self.stdin SocketNotifier
                 self.stdin.setEnabled(False)
                 self.stdin = None
                 break
-            text = data.decode(errors='ignore')
-            self.text(text)
+            text += data.decode(errors='ignore')
+        self.text(text)
         self.show()
+        self.stdin.setEnabled(False)
+        self.next_stdin.start(self.STDIN_REFRESH_DELAY)
+
+    def _cb_next_stdin(self):
+        self.next_stdin.stop()
+        self.stdin.setEnabled(True)
 
     @classmethod
     def clear_session(cls, session_name):
         pidfile = Path("/tmp") / (session_name + ".pid")
         pidfile.unlink()
 
     @classmethod
```

