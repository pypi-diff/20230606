# Comparing `tmp/jdReplace-4.0.tar.gz` & `tmp/jdReplace-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdReplace-4.0.tar", last modified: Tue May 30 13:22:36 2023, max compression
+gzip compressed data, was "jdReplace-4.1.tar", last modified: Tue Jun  6 07:15:17 2023, max compression
```

## Comparing `jdReplace-4.0.tar` & `jdReplace-4.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/
--rw-r--r--   0 root         (0) root         (0)     2202 2023-05-30 13:15:47.000000 jdReplace-4.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35075 2023-05-30 13:15:47.000000 jdReplace-4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-30 13:15:47.000000 jdReplace-4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-30 13:22:36.702765 jdReplace-4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3243 2023-05-30 13:15:47.000000 jdReplace-4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/jdReplace/
--rw-r--r--   0 root         (0) root         (0)     9169 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/Logo.svg
--rwxr-xr-x   0 root         (0) root         (0)    11037 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/jdReplace/translations/
--rw-r--r--   0 root         (0) root         (0)     4476 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/translations/jdReplace_de.ts
--rw-r--r--   0 root         (0) root         (0)     4448 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/translations/jdReplace_nl.ts
--rw-r--r--   0 root         (0) root         (0)        3 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/jdReplace.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1715 2023-05-30 13:15:47.000000 jdReplace-4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:22:36.702765 jdReplace-4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 07:15:17.654125 jdReplace-4.1/
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-06-06 07:13:02.000000 jdReplace-4.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35075 2023-06-06 07:13:02.000000 jdReplace-4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-06 07:13:02.000000 jdReplace-4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4725 2023-06-06 07:15:17.654125 jdReplace-4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-06 07:13:02.000000 jdReplace-4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 07:15:17.654125 jdReplace-4.1/jdReplace/
+-rw-r--r--   0 root         (0) root         (0)     9169 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/Logo.svg
+-rwxr-xr-x   0 root         (0) root         (0)    11293 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 07:15:17.654125 jdReplace-4.1/jdReplace/translations/
+-rw-r--r--   0 root         (0) root         (0)     4476 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/translations/jdReplace_de.ts
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/translations/jdReplace_it.ts
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/translations/jdReplace_nl.ts
+-rw-r--r--   0 root         (0) root         (0)        3 2023-06-06 07:13:02.000000 jdReplace-4.1/jdReplace/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 07:15:17.654125 jdReplace-4.1/jdReplace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4725 2023-06-06 07:15:17.000000 jdReplace-4.1/jdReplace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-06 07:15:17.000000 jdReplace-4.1/jdReplace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 07:15:17.000000 jdReplace-4.1/jdReplace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-06 07:15:17.000000 jdReplace-4.1/jdReplace.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-06 07:15:17.000000 jdReplace-4.1/jdReplace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-06 07:15:17.000000 jdReplace-4.1/jdReplace.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-06-06 07:13:02.000000 jdReplace-4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 07:15:17.654125 jdReplace-4.1/setup.cfg
```

### Comparing `jdReplace-4.0/BuildBackend.py` & `jdReplace-4.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdReplace-4.0/LICENSE` & `jdReplace-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdReplace-4.0/PKG-INFO` & `jdReplace-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdReplace
-Version: 4.0
+Version: 4.1
 Summary: With jdReplace you can replace a text in all files of a directory
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdReplace
 Project-URL: Issues, https://codeberg.org/JakobDev/jdReplace/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdReplace
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -33,15 +33,15 @@
 License-File: LICENSE
 
 <h1 align="center">jdReplace</h1>
 
 <h3 align="center">With jdReplace you can replace a text in all files of a directorys</h3>
 
 <p align="center">
-    <img alt="jdReplace" src="screenshots/MainWindow.png"/>
+    <img alt="jdReplace" src="screenshots/MainWindow_en.png"/>
 </p>
 
 jdReplace is a simple mass search and replace tool.
 You set a directory, a text to replace, the replacement and click OK.
 jdReplace will do the rest.
 
 ## Install
```

### Comparing `jdReplace-4.0/README.md` & `jdReplace-4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="center">jdReplace</h1>
 
 <h3 align="center">With jdReplace you can replace a text in all files of a directorys</h3>
 
 <p align="center">
-    <img alt="jdReplace" src="screenshots/MainWindow.png"/>
+    <img alt="jdReplace" src="screenshots/MainWindow_en.png"/>
 </p>
 
 jdReplace is a simple mass search and replace tool.
 You set a directory, a text to replace, the replacement and click OK.
 jdReplace will do the rest.
 
 ## Install
```

### Comparing `jdReplace-4.0/jdReplace/Logo.svg` & `jdReplace-4.1/jdReplace/Logo.svg`

 * *Files identical despite different names*

### Comparing `jdReplace-4.0/jdReplace/__init__.py` & `jdReplace-4.1/jdReplace/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #!/usr/bin/env python3
 from PyQt6.QtWidgets import QMessageBox, QApplication, QWidget, QLabel, QPlainTextEdit, QPushButton, QHBoxLayout, QVBoxLayout, QLineEdit, QCheckBox, QProgressBar, QFileDialog
 from PyQt6.QtCore import QDir, QLocale, Qt, QThread, QCoreApplication, QTranslator, QLibraryInfo, pyqtSignal
 from PyQt6.QtGui import QFont, QIcon
+from typing import Optional
 import webbrowser
+import argparse
 import sys
 import os
 
 
 logo = QIcon(os.path.join(os.path.dirname(__file__), "Logo.svg"))
 currentDir = os.path.dirname(os.path.realpath(__file__))
 
 
 with open(os.path.join(currentDir, "version.txt"), "r", encoding="utf-8") as f:
     version = f.read().strip()
 
 
 class AboutWindow(QWidget):
-    def setup(self):
+    def __init__(self):
+        super().__init__()
+
         logoLabel = QLabel()
         logoLabel.setPixmap(logo.pixmap(64, 64))
 
         self.titleLabel = QLabel("jdReplace " + version)
         self.descriptionLabel = QLabel(QCoreApplication.translate("AboutWindow", "With this program you can search and replace a text in all files of a folder"))
         self.copyrightLabel = QLabel("Copyright © 2019-2023 JakobDev")
         self.licenseLabel = QLabel(QCoreApplication.translate("AboutWindow", "This program is licensed under GNU GPL 3"))
@@ -120,17 +124,18 @@
             except Exception:
                 print(QCoreApplication.translate("ReplaceThread", "Could not replace text in {{path}}. Maybe it's a binary file.").replace("{{path}}", filename), file=sys.stderr)
             progressCount += 1
             self.progress.emit(progressCount)
 
 
 class StartWindow(QWidget):
-    def setup(self):
+    def __init__(self, startDirectory: Optional[str]):
+        super().__init__()
+
         self.about = AboutWindow()
-        self.about.setup()
         self.thread = ReplaceThread()
 
         self.directoryLabel = QLabel(QCoreApplication.translate("StartWindow", "Directory:"))
         self.directoryEdit = QLineEdit()
         self.directoryButton = QPushButton(QCoreApplication.translate("StartWindow", "Browse"))
         self.inputTextLabel = QLabel(QCoreApplication.translate("StartWindow", "Search for:"))
         self.inputTextEdit = QPlainTextEdit()
@@ -142,15 +147,15 @@
         self.progressBar = QProgressBar()
         self.aboutButton = QPushButton(QCoreApplication.translate("StartWindow", "About"))
         self.okButton = QPushButton(QCoreApplication.translate("StartWindow", "OK"))
 
         self.directoryButton.setIcon(QIcon.fromTheme("folder"))
         self.aboutButton.setIcon(QIcon.fromTheme("help-about"))
 
-        self.directoryEdit.setText(QDir.currentPath())
+        self.directoryEdit.setText(startDirectory or QDir.currentPath())
         self.inputTextEdit.setLineWrapMode(QPlainTextEdit.LineWrapMode.NoWrap)
         self.outputTextEdit.setLineWrapMode(QPlainTextEdit.LineWrapMode.NoWrap)
         self.directoryButton.clicked.connect(self.browse)
         self.aboutButton.clicked.connect(self.showAbout)
         self.okButton.clicked.connect(self.replaceFiles)
         self.thread.count.connect(self.setMax)
         self.thread.progress.connect(self.setProgress)
@@ -237,18 +242,21 @@
 def main():
     app = QApplication(sys.argv)
 
     app.setDesktopFileName("page.codeberg.JakobDev.jdReplace")
     app.setApplicationName("jdReplace")
     app.setWindowIcon(logo)
 
+    parser = argparse.ArgumentParser()
+    parser.add_argument("directory", nargs="?")
+    args = parser.parse_known_args()[0]
+
     qt_translator = QTranslator()
     app_translator = QTranslator()
     system_language = QLocale.system().name().split("_")[0]
     qt_translator.load(os.path.join(QLibraryInfo.path(QLibraryInfo.LibraryPath.TranslationsPath), "qt_" + system_language + ".qm"))
     app_translator.load(os.path.join(currentDir, "translations", "jdReplace_" + system_language + ".qm"))
     app.installTranslator(app_translator)
     app.installTranslator(qt_translator)
 
-    w = StartWindow()
-    w.setup()
+    w = StartWindow(args.directory)
     sys.exit(app.exec())
```

### Comparing `jdReplace-4.0/jdReplace/translations/jdReplace_de.ts` & `jdReplace-4.1/jdReplace/translations/jdReplace_de.ts`

 * *Files 4% similar despite different names*

#### Comparing `jdReplace-4.0/jdReplace/translations/jdReplace_de.ts` & `jdReplace-4.1/jdReplace/translations/jdReplace_de.ts`

```diff
@@ -1,124 +1,124 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1" language="de">
   <context>
     <name>AboutWindow</name>
     <message>
-      <location filename="../__init__.py" line="23"/>
+      <location filename="../__init__.py" line="28"/>
       <source>With this program you can search and replace a text in all files of a folder</source>
       <translation>jdReplace sucht und ersetzt einen Text in allen Dateien eines Ordners</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="25"/>
+      <location filename="../__init__.py" line="30"/>
       <source>This program is licensed under GNU GPL 3</source>
       <translation>Dieses Programm wurde unter GNU GPL 3 lizenziert</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="26"/>
+      <location filename="../__init__.py" line="31"/>
       <source>View Source</source>
       <translation>Quelltext ansehen</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="27"/>
+      <location filename="../__init__.py" line="32"/>
       <source>Close</source>
       <translation>Schließen</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="64"/>
+      <location filename="../__init__.py" line="69"/>
       <source>About</source>
       <translation>Über</translation>
     </message>
   </context>
   <context>
     <name>ReplaceThread</name>
     <message>
-      <location filename="../__init__.py" line="90"/>
+      <location filename="../__init__.py" line="95"/>
       <source>Searching {{path}}...</source>
       <translation>Durchsuche {{path}}...</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="120"/>
+      <location filename="../__init__.py" line="125"/>
       <source>Could not replace text in {{path}}. Maybe it's a binary file.</source>
       <translation>Konnte Text in {{path}} nicht ersetzen. Möglicherweise ist es eine Binärdatei.</translation>
     </message>
   </context>
   <context>
     <name>StartWindow</name>
     <message>
-      <location filename="../__init__.py" line="131"/>
+      <location filename="../__init__.py" line="137"/>
       <source>Directory:</source>
       <translation>Verzeichnis:</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="196"/>
-      <location filename="../__init__.py" line="133"/>
+      <location filename="../__init__.py" line="202"/>
+      <location filename="../__init__.py" line="139"/>
       <source>Browse</source>
       <translation>Durchsuchen</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="134"/>
+      <location filename="../__init__.py" line="140"/>
       <source>Search for:</source>
       <translation>Suche nach:</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="136"/>
+      <location filename="../__init__.py" line="142"/>
       <source>Replace with:</source>
       <translation>Ersetze durch:</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="138"/>
+      <location filename="../__init__.py" line="144"/>
       <source>Search Subdirectories</source>
       <translation>Unterverzeichnisse durchsuchen</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="139"/>
+      <location filename="../__init__.py" line="145"/>
       <source>Skip Hidden</source>
       <translation>Keine Versteckten</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="140"/>
+      <location filename="../__init__.py" line="146"/>
       <source>Follow Symlinks</source>
       <translation>Symbolischen Verknüpfungen folgen</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="142"/>
+      <location filename="../__init__.py" line="148"/>
       <source>About</source>
       <translation>Über</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="143"/>
+      <location filename="../__init__.py" line="149"/>
       <source>OK</source>
       <translation>OK</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="217"/>
+      <location filename="../__init__.py" line="223"/>
       <source>Finished</source>
       <translation>Fertig</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="217"/>
+      <location filename="../__init__.py" line="223"/>
       <source>The text has been successfully replaced in all files</source>
       <translation>Der Text wurde in allen Dateien erfolgreich ersetzt</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="222"/>
+      <location filename="../__init__.py" line="228"/>
       <source>Not a directory</source>
       <translation>Kein Verzeichnis</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="222"/>
+      <location filename="../__init__.py" line="228"/>
       <source>'{{path}}' is not a directory!</source>
       <translation>'{{path}}' ist kein Verzeichnis!</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="227"/>
+      <location filename="../__init__.py" line="233"/>
       <source>No search text</source>
       <translation>Kein Suchtext</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="227"/>
+      <location filename="../__init__.py" line="233"/>
       <source>Please enter a text to search for</source>
       <translation>Bitte gib einen Text ein, nach dem gesucht werden soll</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdReplace-4.0/jdReplace/translations/jdReplace_nl.ts` & `jdReplace-4.1/jdReplace/translations/jdReplace_it.ts`

 * *Files 5% similar despite different names*

#### Comparing `jdReplace-4.0/jdReplace/translations/jdReplace_nl.ts` & `jdReplace-4.1/jdReplace/translations/jdReplace_it.ts`

```diff
@@ -1,124 +1,124 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="nl">
+<TS version="2.1" language="it">
   <context>
     <name>AboutWindow</name>
     <message>
-      <location filename="../__init__.py" line="23"/>
+      <location filename="../__init__.py" line="28"/>
       <source>With this program you can search and replace a text in all files of a folder</source>
-      <translation>Zoek naar en vervang tekst in alle bestanden binnen een map</translation>
+      <translation>Con questo programma puoi cercare e sostituire un testo in tutti i file di una cartella</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="25"/>
+      <location filename="../__init__.py" line="30"/>
       <source>This program is licensed under GNU GPL 3</source>
-      <translation>Dit programma is uitgebracht onder de GNU GPLv3-licentie</translation>
+      <translation>Questo programma è concesso in licenza con GNU GPL 3</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="26"/>
+      <location filename="../__init__.py" line="31"/>
       <source>View Source</source>
-      <translation>Broncode bekijken</translation>
+      <translation>Vedi sorgente</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="27"/>
+      <location filename="../__init__.py" line="32"/>
       <source>Close</source>
-      <translation>Sluiten</translation>
+      <translation>Chiudi</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="64"/>
+      <location filename="../__init__.py" line="69"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Informazioni</translation>
     </message>
   </context>
   <context>
     <name>ReplaceThread</name>
     <message>
-      <location filename="../__init__.py" line="90"/>
+      <location filename="../__init__.py" line="95"/>
       <source>Searching {{path}}...</source>
-      <translation>Bezig met zoeken naar ‘{{path}}’…</translation>
+      <translation>Ricerca {{path}}...</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="120"/>
+      <location filename="../__init__.py" line="125"/>
       <source>Could not replace text in {{path}}. Maybe it's a binary file.</source>
-      <translation>De tekst in ‘{{path}}’ kan niet worden vervangen. Is het een uitvoerbaar bestand.</translation>
+      <translation>Ricerca {{path}}... Impossibile sostituire il testo in {{path}}. Forse è un file binario..</translation>
     </message>
   </context>
   <context>
     <name>StartWindow</name>
     <message>
-      <location filename="../__init__.py" line="131"/>
+      <location filename="../__init__.py" line="137"/>
       <source>Directory:</source>
-      <translation>Map:</translation>
+      <translation>Directory:</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="196"/>
-      <location filename="../__init__.py" line="133"/>
+      <location filename="../__init__.py" line="202"/>
+      <location filename="../__init__.py" line="139"/>
       <source>Browse</source>
-      <translation>Bladeren</translation>
+      <translation>Sfoglia</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="134"/>
+      <location filename="../__init__.py" line="140"/>
       <source>Search for:</source>
-      <translation>Zoeken naar:</translation>
+      <translation>Ricerca per:</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="136"/>
+      <location filename="../__init__.py" line="142"/>
       <source>Replace with:</source>
-      <translation>Vervangen door:</translation>
+      <translation>Sostituisci con:</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="138"/>
+      <location filename="../__init__.py" line="144"/>
       <source>Search Subdirectories</source>
-      <translation>Ook onderliggende mappen doorzoeken</translation>
+      <translation>Sottodirecotry</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="139"/>
+      <location filename="../__init__.py" line="145"/>
       <source>Skip Hidden</source>
-      <translation>Verborgen bestanden/mappen overslaan</translation>
+      <translation>Salta nascosto</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="140"/>
+      <location filename="../__init__.py" line="146"/>
       <source>Follow Symlinks</source>
-      <translation>Snelkoppelingen negeren</translation>
+      <translation>Segui i link simbolici</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="142"/>
+      <location filename="../__init__.py" line="148"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Informazioni</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="143"/>
+      <location filename="../__init__.py" line="149"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>OK</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="217"/>
+      <location filename="../__init__.py" line="223"/>
       <source>Finished</source>
-      <translation>Afgerond</translation>
+      <translation>Finito</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="217"/>
+      <location filename="../__init__.py" line="223"/>
       <source>The text has been successfully replaced in all files</source>
-      <translation>De tekst is in alle bestanden vervangen</translation>
+      <translation>Il testo è stato sostituito con successo in tutti i file</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="222"/>
+      <location filename="../__init__.py" line="228"/>
       <source>Not a directory</source>
-      <translation>Geen map</translation>
+      <translation>Non una directory</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="222"/>
+      <location filename="../__init__.py" line="228"/>
       <source>'{{path}}' is not a directory!</source>
-      <translation>‘{{path}}’ is geen map!</translation>
+      <translation>'{{path}}' non è una directory!</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="227"/>
+      <location filename="../__init__.py" line="233"/>
       <source>No search text</source>
-      <translation>Geen zoekopdracht</translation>
+      <translation>Nessun testo di ricerca</translation>
     </message>
     <message>
-      <location filename="../__init__.py" line="227"/>
+      <location filename="../__init__.py" line="233"/>
       <source>Please enter a text to search for</source>
-      <translation>Voer een zoekopdracht in</translation>
+      <translation>Inserisci un testo da cercare</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdReplace-4.0/jdReplace.egg-info/PKG-INFO` & `jdReplace-4.1/jdReplace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdReplace
-Version: 4.0
+Version: 4.1
 Summary: With jdReplace you can replace a text in all files of a directory
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdReplace
 Project-URL: Issues, https://codeberg.org/JakobDev/jdReplace/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdReplace
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -33,15 +33,15 @@
 License-File: LICENSE
 
 <h1 align="center">jdReplace</h1>
 
 <h3 align="center">With jdReplace you can replace a text in all files of a directorys</h3>
 
 <p align="center">
-    <img alt="jdReplace" src="screenshots/MainWindow.png"/>
+    <img alt="jdReplace" src="screenshots/MainWindow_en.png"/>
 </p>
 
 jdReplace is a simple mass search and replace tool.
 You set a directory, a text to replace, the replacement and click OK.
 jdReplace will do the rest.
 
 ## Install
```

### Comparing `jdReplace-4.0/pyproject.toml` & `jdReplace-4.1/pyproject.toml`

 * *Files identical despite different names*

