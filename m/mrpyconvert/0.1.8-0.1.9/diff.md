# Comparing `tmp/mrpyconvert-0.1.8.tar.gz` & `tmp/mrpyconvert-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrpyconvert-0.1.8.tar", max compression
+gzip compressed data, was "mrpyconvert-0.1.9.tar", max compression
```

## Comparing `mrpyconvert-0.1.8.tar` & `mrpyconvert-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.8/LICENSE
--rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.8/README.md
--rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.8/mrpyconvert/__init__.py
--rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.8/mrpyconvert/dicom_sorter.py
--rw-r--r--   0        0        0    16365 2023-05-31 23:32:00.902474 mrpyconvert-0.1.8/mrpyconvert/mrpyconvert.py
--rw-r--r--   0        0        0      438 2023-06-02 18:37:58.976377 mrpyconvert-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 mrpyconvert-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.9/LICENSE
+-rw-r--r--   0        0        0       94 2023-06-05 20:59:06.936826 mrpyconvert-0.1.9/README.md
+-rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.9/mrpyconvert/__init__.py
+-rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.9/mrpyconvert/dicom_sorter.py
+-rw-r--r--   0        0        0    16741 2023-06-05 19:12:34.744765 mrpyconvert-0.1.9/mrpyconvert/mrpyconvert.py
+-rw-r--r--   0        0        0      456 2023-06-05 18:38:16.718413 mrpyconvert-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 mrpyconvert-0.1.9/PKG-INFO
```

### Comparing `mrpyconvert-0.1.8/LICENSE` & `mrpyconvert-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.8/mrpyconvert/dicom_sorter.py` & `mrpyconvert-0.1.9/mrpyconvert/dicom_sorter.py`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.8/mrpyconvert/mrpyconvert.py` & `mrpyconvert-0.1.9/mrpyconvert/mrpyconvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import re
 import json
 import os
 import pathlib
 import itertools
+import stat
+import tempfile
+import subprocess
+
 import pydicom
 
-# todo: a preview function!
+# todo: a preview function?
 
 # BIDS VERSION: 1.8.0
 # valid datatype information
 datatypes = ['anat', 'func', 'dwi', 'fmap', 'meg', 'eeg', 'ieeg', 'beh']
 
 entities = ['acq', 'ce', 'chunk', 'dir', 'echo', 'flip', 'hemi', 'inv', 'mod', 'mt', 'part', 'proc', 'rec', 'recording',
             'run', 'sample', 'ses', 'space', 'split', 'stain', 'task', 'trc']
@@ -140,22 +144,27 @@
                 print(f'More than one copy of {description} for at least one study')
 
     def set_names(self, bids_names: dict):
         for series in self.series:
             if series.orig_subject in bids_names:
                 series.subject = bids_names[series.orig_subject]
 
-    def generate_scripts(self, bids_path, script_ext=None, script_path=os.getcwd(), slurm=False,
+    def convert(self, bids_path):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            temp_scripts = self.generate_scripts(bids_path=bids_path, script_path=tmpdir)
+            for ts in temp_scripts:
+                print(f'Converting {pathlib.Path(ts).name}')
+                st = os.stat(ts)
+                os.chmod(ts, st.st_mode | stat.S_IEXEC)
+                subprocess.run(ts)
+
+    def generate_scripts(self, bids_path, script_ext='', script_path=os.getcwd(), slurm=False,
                          additional_commands=None, script_prefix=None):
+        script_names = []
 
-        if not script_ext:
-            if slurm:
-                script_ext = '.srun'
-            else:
-                script_ext = '.sh'
         # assign session numbers to series objects using dates
         if self.autosession:
             all_subjects = {x.subject for x in self.series}
             for subject in all_subjects:
                 s_series = [s for s in self.series if s.subject == subject]
                 s_series.sort(key = lambda x: (x.date, x.study_uid))
                 # get unique values, preserving order
@@ -249,21 +258,24 @@
 
             command.extend(self.generate_commands(entity))
 
             if not slurm:
                 command.append('done')
 
             script_name = pathlib.Path(script_path) / (script_name + script_ext)
-            print(script_name)
+
             # todo: write to stdout instead of file as option?
             with open(script_name, 'w') as f:
                 for line in command:
                     f.write(line)
                     f.write('\n')
 
+            script_names.append(script_name)
+        return script_names
+
     def set_autosession(self, autosession = True):
         self.autosession = autosession
         for e in self.entities:
             if autosession:
                 e.chain['ses'] = '${session}'
             else:
                 del e.chain['ses']
```

### Comparing `mrpyconvert-0.1.8/PKG-INFO` & `mrpyconvert-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mrpyconvert
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool to create scripts to convert dicom to bids
 License: MIT
 Author: Jolinda Smith
 Author-email: jolinda@uoregon.edu
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dcm2niix (>=1.0,<2.0)
 Requires-Dist: jq (>=1.0,<2.0)
 Requires-Dist: pydicom (>=2.2,<3.0)
 Description-Content-Type: text/markdown
 
-# MrPyConvert
+# mrpyconvert
 Python module for dicom to bids conversion  
 Creates scripts that call dcm2niix
```

