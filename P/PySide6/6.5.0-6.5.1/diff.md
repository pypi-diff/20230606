# Comparing `tmp/PySide6-6.5.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/PySide6-6.5.1-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7242 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     5537 b- defN 23-Apr-04 05:14 PySide6/__init__.py
--rw-rw-rw-  2.0 fat      796 b- defN 23-Apr-04 05:14 PySide6/_config.py
--rw-rw-rw-  2.0 fat      676 b- defN 23-Apr-04 05:14 PySide6/_git_pyside_version.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-Apr-04 05:39 PySide6-6.5.0.dist-info/LicenseRef-Qt-Commercial.txt
--rw-rw-rw-  2.0 fat     5307 b- defN 23-Apr-04 05:39 PySide6-6.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-04 05:39 PySide6-6.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-04 05:39 PySide6-6.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      643 b- defN 23-Apr-04 05:39 PySide6-6.5.0.dist-info/RECORD
-8 files, 13559 bytes uncompressed, 6118 bytes compressed:  54.9%
+Zip file size: 7244 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     5537 b- defN 23-May-26 07:54 PySide6/__init__.py
+-rw-rw-rw-  2.0 fat      796 b- defN 23-May-26 07:54 PySide6/_config.py
+-rw-rw-rw-  2.0 fat      676 b- defN 23-May-26 07:54 PySide6/_git_pyside_version.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-May-26 08:10 PySide6-6.5.1.dist-info/LicenseRef-Qt-Commercial.txt
+-rw-rw-rw-  2.0 fat     5307 b- defN 23-May-26 08:10 PySide6-6.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-26 08:10 PySide6-6.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 08:10 PySide6-6.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      643 b- defN 23-May-26 08:10 PySide6-6.5.1.dist-info/RECORD
+8 files, 13559 bytes uncompressed, 6120 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: PySide6/_config.py
 Comment: 
 
 Filename: PySide6/_git_pyside_version.py
 Comment: 
 
-Filename: PySide6-6.5.0.dist-info/LicenseRef-Qt-Commercial.txt
+Filename: PySide6-6.5.1.dist-info/LicenseRef-Qt-Commercial.txt
 Comment: 
 
-Filename: PySide6-6.5.0.dist-info/METADATA
+Filename: PySide6-6.5.1.dist-info/METADATA
 Comment: 
 
-Filename: PySide6-6.5.0.dist-info/WHEEL
+Filename: PySide6-6.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: PySide6-6.5.0.dist-info/top_level.txt
+Filename: PySide6-6.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: PySide6-6.5.0.dist-info/RECORD
+Filename: PySide6-6.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySide6/__init__.py

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 from textwrap import dedent
 
 # __all__ is also corrected below.
 __all__ = list("Qt" + body for body in
     "Core;Gui;Widgets;PrintSupport;Sql;Network;Test;Concurrent;Designer;Xml;Help;Multimedia;MultimediaWidgets;OpenGL;OpenGLWidgets;Pdf;PdfWidgets;Positioning;Location;NetworkAuth;Nfc;Qml;Quick;Quick3D;QuickControls2;QuickWidgets;RemoteObjects;Scxml;Sensors;SerialPort;SerialBus;StateMachine;TextToSpeech;Charts;SpatialAudio;Svg;SvgWidgets;DataVisualization;Bluetooth;UiTools;AxContainer;WebChannel;WebEngineCore;WebEngineWidgets;WebEngineQuick;WebSockets;3DCore;3DRender;3DInput;3DLogic;3DAnimation;3DExtras"
     .split(";"))
-__version__ = "6.5.0"
-__version_info__ = (6, 5, 0, "", "")
+__version__ = "6.5.1"
+__version_info__ = (6, 5, 1, "", "")
 
 
 def _additional_dll_directories(package_dir):
     # Find shiboken6 relative to the package directory.
     root = Path(package_dir).parent
     # Check for a flat .zip as deployed by cx_free(PYSIDE-1257)
     if root.suffix == '.zip':
```

## PySide6/_config.py

```diff
@@ -1,16 +1,16 @@
 built_modules = list(name for name in
     "Core;Gui;Widgets;PrintSupport;Sql;Network;Test;Concurrent;Designer;Xml;Help;Multimedia;MultimediaWidgets;OpenGL;OpenGLWidgets;Pdf;PdfWidgets;Positioning;Location;NetworkAuth;Nfc;Qml;Quick;Quick3D;QuickControls2;QuickWidgets;RemoteObjects;Scxml;Sensors;SerialPort;SerialBus;StateMachine;TextToSpeech;Charts;SpatialAudio;Svg;SvgWidgets;DataVisualization;Bluetooth;UiTools;AxContainer;WebChannel;WebEngineCore;WebEngineWidgets;WebEngineQuick;WebSockets;3DCore;3DRender;3DInput;3DLogic;3DAnimation;3DExtras"
     .split(";"))
 
 shiboken_library_soversion = str(6.5)
 pyside_library_soversion = str(6.5)
 
-version = "6.5.0"
-version_info = (6, 5, 0, "", "")
+version = "6.5.1"
+version_info = (6, 5, 1, "", "")
 
-__build_date__ = '2023-04-04T05:14:40+00:00'
+__build_date__ = '2023-05-26T07:54:14+00:00'
 
 
 
 
-__setup_py_package_version__ = '6.5.0'
+__setup_py_package_version__ = '6.5.1'
```

## PySide6/_git_pyside_version.py

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2022 The Qt Company Ltd.
 # SPDX-License-Identifier: LicenseRef-Qt-Commercial OR LGPL-3.0-only OR GPL-2.0-only OR GPL-3.0-only
 
 major_version = "6"
 minor_version = "5"
-patch_version = "0"
+patch_version = "1"
 
 # For example: "a", "b", "rc"
 # (which means "alpha", "beta", "release candidate").
 # An empty string means the generated package will be an official release.
 release_version_type = ""
 
 # For example: "1", "2" (which means "beta1", "beta2", if type is "b").
```

## Comparing `PySide6-6.5.0.dist-info/METADATA` & `PySide6-6.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6
-Version: 6.5.0
+Version: 6.5.1
 Summary: Python bindings for the Qt cross-platform application and UI framework
 Home-page: https://www.pyside.org
 Download-URL: https://download.qt.io/official_releases/QtForPython
 Author: Qt for Python Team
 Author-email: pyside@qt-project.org
 License: LGPL
 Keywords: Qt
@@ -34,17 +34,17 @@
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 License-File: LicenseRef-Qt-Commercial.txt
-Requires-Dist: shiboken6 (==6.5.0)
-Requires-Dist: PySide6-Essentials (==6.5.0)
-Requires-Dist: PySide6-Addons (==6.5.0)
+Requires-Dist: shiboken6 (==6.5.1)
+Requires-Dist: PySide6-Essentials (==6.5.1)
+Requires-Dist: PySide6-Addons (==6.5.1)
 
 # PySide6
 
 ### Introduction
 
 **Important:** for Qt5 compatibility, check [PySide2](https://pypi.org/project/PySide2)
```

