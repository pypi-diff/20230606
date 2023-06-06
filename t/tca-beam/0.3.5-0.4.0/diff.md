# Comparing `tmp/tca_beam-0.3.5.tar.gz` & `tmp/tca_beam-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tca_beam-0.3.5.tar", max compression
+gzip compressed data, was "tca_beam-0.4.0.tar", max compression
```

## Comparing `tca_beam-0.3.5.tar` & `tca_beam-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.3.5/README.md
--rw-r--r--   0        0        0      419 2023-06-05 16:56:48.721051 tca_beam-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.3.5/tca_beam/__init__.py
--rw-r--r--   0        0        0     6467 2023-06-05 14:40:07.483250 tca_beam-0.3.5/tca_beam/tca_beam.py
--rw-r--r--   0        0        0      526 2023-06-05 10:09:21.285125 tca_beam-0.3.5/tca_beam/templates/AllPreviews.swift
--rw-r--r--   0        0        0       86 2023-06-04 16:14:37.894614 tca_beam-0.3.5/tca_beam/templates/OneFile.swift
--rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.3.5/tca_beam/templates/TwoFile_ReducerPart.swift
--rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.3.5/tca_beam/templates/TwoFile_ViewPart.swift
--rw-r--r--   0        0        0      633 2023-06-05 09:48:58.421080 tca_beam-0.3.5/tca_beam/templates/View.swift
--rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.3.5/tca_beam/templates/ViewFeature.swift
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.3.5/setup.py
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 tca_beam-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-05 14:46:22.215862 tca_beam-0.4.0/README.md
+-rw-r--r--   0        0        0      425 2023-06-06 10:04:56.526747 tca_beam-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-05 13:50:29.564328 tca_beam-0.4.0/tca_beam/__init__.py
+-rw-r--r--   0        0        0      459 2023-06-06 09:39:44.292506 tca_beam-0.4.0/tca_beam/click_sample.py
+-rw-r--r--   0        0        0     1325 2023-06-06 08:44:16.962819 tca_beam-0.4.0/tca_beam/nogroup_demo.py
+-rw-r--r--   0        0        0     6703 2023-06-06 09:44:49.698473 tca_beam-0.4.0/tca_beam/tca_beam.py
+-rw-r--r--   0        0        0      526 2023-06-05 10:09:21.285125 tca_beam-0.4.0/tca_beam/templates/AllPreviews.swift
+-rw-r--r--   0        0        0       86 2023-06-04 16:14:37.894614 tca_beam-0.4.0/tca_beam/templates/OneFile.swift
+-rw-r--r--   0        0        0       52 2023-06-05 09:23:16.046676 tca_beam-0.4.0/tca_beam/templates/TwoFile_ReducerPart.swift
+-rw-r--r--   0        0        0       64 2023-06-04 21:52:01.190023 tca_beam-0.4.0/tca_beam/templates/TwoFile_ViewPart.swift
+-rw-r--r--   0        0        0      633 2023-06-05 09:48:58.421080 tca_beam-0.4.0/tca_beam/templates/View.swift
+-rw-r--r--   0        0        0      463 2023-06-04 22:08:47.296586 tca_beam-0.4.0/tca_beam/templates/ViewFeature.swift
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tca_beam-0.4.0/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 tca_beam-0.4.0/PKG-INFO
```

### Comparing `tca_beam-0.3.5/tca_beam/tca_beam.py` & `tca_beam-0.4.0/tca_beam/tca_beam.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 import sys
 from pathlib import Path
 from collections import namedtuple
 from jinja2 import Environment, FileSystemLoader
 import click
+from trogon import tui
 
 beam_version = "(beam is not packaged so no version)"
 
 try:
     from tca_beam import __version__
     beam_version = __version__
 except ImportError:
     pass
 
 # TODO:
-# -[ ] upload to main pyPi
+# [x] try trogon/textualize on tca-beam -- see results in my main TW -- might have to make explicit tca-beam 'make' command
+# -[x] upload to main pyPi
 # -[ ] make bbtests
 # -[x] option for preview-all
 # -[x] impl two files
 # -[x] flags for 'features in sub_dirs'
 # -[x] make script use abs path to the templates, no chdir!
 # -[x] --dry-run
 
@@ -142,23 +144,26 @@
     if preview_all:
         generate_all_preview(env, feature_names, script_dir, two_files, sub_dirs, preview_all, force_overwrite, dry_run, feature_name)
 
     p()
     p("Done")
     p()
 
-
-@click.command(no_args_is_help=True)
+@tui()
+@click.group(invoke_without_command=True)
+# @click.group()
 @click.option('--two-files', is_flag=True, help="Put view and reducer into separate files")
 @click.option('--sub-dirs', is_flag=True, help="Put each feature in a sub-directory")
 @click.option('--preview-all', is_flag=True, help="Generate a single View that previews all feature Views")
 @click.option('--force-overwrite', is_flag=True, help="Force overwriting any existing files")
 @click.option('--dry-run', is_flag=True, help="Don't generate files, just preview any actions")
 @click.option('--version', is_flag=True, help="Print version and exit")
 @click.argument('feature_names', nargs=-1)
+# @click.command(no_args_is_help=True)
+# @click.pass_context
 def start(two_files, sub_dirs, preview_all, force_overwrite, dry_run, version, feature_names):
 
     if version:
         p(beam_version)
         sys.exit(0)
 
     if len(feature_names) < 1:
```

### Comparing `tca_beam-0.3.5/tca_beam/templates/AllPreviews.swift` & `tca_beam-0.4.0/tca_beam/templates/AllPreviews.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.3.5/tca_beam/templates/View.swift` & `tca_beam-0.4.0/tca_beam/templates/View.swift`

 * *Files identical despite different names*

### Comparing `tca_beam-0.3.5/setup.py` & `tca_beam-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['click>=8.1.3,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tca-beam = tca_beam.tca_beam:start']}
 
 setup_kwargs = {
     'name': 'tca-beam',
-    'version': '0.3.5',
+    'version': '0.4.0',
     'description': 'Feature stub generation for The Composable Architecture',
     'long_description': 'TCA-beam, a helper for The Composable Architecture for creating Views and Reducers for new features.\n\nhttps://github.com/alexhunsley/tca-beam\n\n',
     'author': 'Alex Hunsley',
     'author_email': 'alex.hunsley@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.4,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `tca_beam-0.3.5/PKG-INFO` & `tca_beam-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: tca-beam
-Version: 0.3.5
+Version: 0.4.0
 Summary: Feature stub generation for The Composable Architecture
 Author: Alex Hunsley
 Author-email: alex.hunsley@gmail.com
-Requires-Python: >=3.4,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
```

