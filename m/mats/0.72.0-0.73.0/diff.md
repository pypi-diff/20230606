# Comparing `tmp/mats-0.72.0-py3-none-any.whl.zip` & `tmp/mats-0.73.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12531 bytes, number of entries: 10
--rw-r--r--  2.0 unx      660 b- defN 22-Jul-12 10:28 mats/__init__.py
--rw-r--r--  2.0 unx     9673 b- defN 22-Jul-12 10:28 mats/archiving.py
--rw-r--r--  2.0 unx     7432 b- defN 22-Jul-12 10:28 mats/test.py
--rw-r--r--  2.0 unx    13066 b- defN 22-Jul-12 10:28 mats/test_sequence.py
--rw-r--r--  2.0 unx     6936 b- defN 22-Jul-12 10:28 mats/tkwidgets.py
--rw-r--r--  2.0 unx       23 b- defN 22-Jul-12 10:28 mats/version.py
--rw-r--r--  2.0 unx     2747 b- defN 22-Jul-12 10:28 mats-0.72.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-12 10:28 mats-0.72.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 22-Jul-12 10:28 mats-0.72.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      727 b- defN 22-Jul-12 10:28 mats-0.72.0.dist-info/RECORD
-10 files, 41361 bytes uncompressed, 11313 bytes compressed:  72.6%
+Zip file size: 12800 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      660 b- defN 23-Jun-06 11:16 mats/__init__.py
+-rw-r--r--  2.0 unx    10574 b- defN 23-Jun-06 11:16 mats/archiving.py
+-rw-r--r--  2.0 unx     7475 b- defN 23-Jun-06 11:16 mats/test.py
+-rw-r--r--  2.0 unx    13151 b- defN 23-Jun-06 11:16 mats/test_sequence.py
+-rw-r--r--  2.0 unx     6936 b- defN 23-Jun-06 11:16 mats/tkwidgets.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-06 11:16 mats/version.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-Jun-06 11:17 mats-0.73.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 11:17 mats-0.73.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-06 11:17 mats-0.73.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      728 b- defN 23-Jun-06 11:17 mats-0.73.0.dist-info/RECORD
+10 files, 42372 bytes uncompressed, 11582 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: mats/tkwidgets.py
 Comment: 
 
 Filename: mats/version.py
 Comment: 
 
-Filename: mats-0.72.0.dist-info/METADATA
+Filename: mats-0.73.0.dist-info/METADATA
 Comment: 
 
-Filename: mats-0.72.0.dist-info/WHEEL
+Filename: mats-0.73.0.dist-info/WHEEL
 Comment: 
 
-Filename: mats-0.72.0.dist-info/top_level.txt
+Filename: mats-0.73.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mats-0.72.0.dist-info/RECORD
+Filename: mats-0.73.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mats/archiving.py

```diff
@@ -1,40 +1,54 @@
 from datetime import datetime
 import logging
 from os import remove
 from pathlib import Path
 from shutil import copy
-from typing import List
+from typing import Optional
 
 from mats.test import Test
 
 
 class ArchiveManager:
+    """
+    The default data manager that saves data in a text format which is very flexible, \
+    yet maintains simplicity and compatibility with analysis tools such as pandas.
+
+    :param path: a string or `Path` containing the path to the data file
+    :param fname: data file name
+    :param delimiter: the data delimiter
+    :param data_format: an integer that determines which data format
+    :param preamble: a string that may be appended to the beginning of a data file
+    :param loglevel: the logging level
+    """
+
     def __init__(
         self,
-        path=".",
-        fname="data.txt",
-        delimiter="\t",
+        path: str | Path = ".",
+        fname: str = "data.txt",
+        delimiter: str = "\t",
         data_format: int = 0,
+        preamble: Optional[str] = None,
         loglevel=logging.INFO,
     ):
         self._logger = logging.getLogger(self.__class__.__name__)
         self._logger.setLevel(loglevel)
 
         self._fname = fname
         self._path = Path(path)
         self._delimiter = delimiter
         self._format = data_format
+        self._preamble = preamble
 
     def aggregate(
         self,
         datetime: datetime,
         is_passing: bool,
-        failed: List["str"],
-        tests: List[Test],
+        failed: list[str],
+        tests: list[Test],
     ):
         """
         Collects data set from provided information and from the tests \
         and organizes the data into a dict in preparation for saving \
         a row of data.
 
         :param datetime: the datetime that the test started
@@ -123,15 +137,18 @@
                 if "min" in criteria.keys():
                     heading_fragments.append(f"min={criteria['min']}")
                 if "max" in criteria.keys():
                     heading_fragments.append(f"max={criteria['max']}")
 
                 heading_string += header + ":" + ",".join(heading_fragments) + "\n"
 
-        header_string = heading_string + f"\n{self._delimiter.join(headers)}\n"
+        preamble = '' if not self._preamble else f'{self._preamble}\n'
+        header_string = preamble \
+                        + heading_string \
+                        + f"\n{self._delimiter.join(headers)}\n"
 
         data = []
         for _, value in point.items():
             v = value.get("value")
             if isinstance(v, str):
                 data.append(v)
             elif isinstance(v, int):
@@ -168,15 +185,18 @@
                 if "pass_if" in criteria.keys():
                     header_string += f"{header} =\t"
                 if "min" in criteria.keys():
                     header_string += f"{header} >=\t"
                 if "max" in criteria.keys():
                     header_string += f"{header} <=\t"
 
-        header_string = header_string.strip() + "\n"
+        preamble = '' if not self._preamble else f'{self._preamble}\n\n'
+        header_string = preamble \
+                        + header_string.strip() \
+                        + "\n"
 
         data = []
         for header, value in point.items():
             v = value.get("value")
             if header == "failed":
                 # when header is "failed", then save each failed value into
                 # its own special semicolon-separated data_format
```

## mats/test.py

```diff
@@ -27,15 +27,15 @@
 
     def __init__(
         self,
         moniker: str,
         min_value: Optional[Number] = None,
         max_value: Optional[Number] = None,
         pass_if: Optional[Union[str, bool, int]] = None,
-        significant_figures=4,
+        significant_figures: int = 4,
         loglevel=logging.INFO,
     ):
         self._logger = logging.getLogger(self.__class__.__name__)
         self._logger.setLevel(loglevel)
 
         criteria = {}
         if pass_if is not None:
@@ -78,15 +78,15 @@
         """
         Causes current test status to abort
 
         :return: None
         """
         self.aborted = True
 
-    def _setup(self, is_passing):
+    def _setup(self, is_passing: bool):
         """
         Pre-execution method used for logging and housekeeping.
 
         :param is_passing: True if the test sequence is passing up to this \
         point, else False
         :return:
         """
@@ -96,15 +96,15 @@
         self.value = None
         self.status = "running" if not self.aborted else "aborted"
 
         self.aborted = False
         self.setup(is_passing=is_passing)
         self.status = "running" if not self.aborted else "aborted"
 
-    def _execute(self, is_passing):
+    def _execute(self, is_passing: bool):
         """
         Pre-execution method used for logging and housekeeping.
 
         :param is_passing: True if the test sequence is passing up to this \
         point, else False
         :return:
         """
@@ -164,15 +164,15 @@
                         f'"{self.__criteria["max"]}"'
                     )
 
         self.status = "running" if not self.aborted else "aborted"
 
         return self.value
 
-    def _teardown(self, is_passing):
+    def _teardown(self, is_passing: bool):
         """
         Pre-execution method used for logging and housekeeping.
 
         :param is_passing: True if the test sequence is passing up to \
         this point, else False
         :return:
         """
@@ -207,35 +207,35 @@
         """
         When called, will cause the test to fail.
 
         :return: None
         """
         self._test_is_passing = False
 
-    def setup(self, is_passing):
+    def setup(self, is_passing: bool):
         """
         Abstract method intended to be overridden by subclass
 
         :param is_passing: True if the test sequence is passing up to this \
         point, else False
         :return: None
         """
         pass
 
-    def execute(self, is_passing):
+    def execute(self, is_passing: bool):
         """
         Abstract method intended to be overridden by subclass
 
         :param is_passing: True if the test sequence is passing up to this \
         point, else False
         :return: value to be appended to the sequence dictionary
         """
         raise NotImplementedError
 
-    def teardown(self, is_passing):
+    def teardown(self, is_passing: bool):
         """
         Abstract method intended to be overridden by subclass
 
         :param is_passing: True if the test sequence is passing up to this \
         point, else False
         :return: None
         """
```

## mats/test_sequence.py

```diff
@@ -1,14 +1,14 @@
 import atexit
 from datetime import datetime
 import logging
 from threading import Thread
 import traceback
 from time import sleep
-from typing import List, Optional
+from typing import Optional
 
 from mats.test import Test
 from mats.archiving import ArchiveManager
 
 # State Machine - Using strings b/c we can relatively easily look
 # for valid substrings to give more information in a concise way.
 # For instance, one may be looking for the substring 'ready', but
@@ -48,15 +48,15 @@
     :param on_close: function to call when the functionality is complete; \
     for instance, when a GUI closes, test hardware may need to be de-allocated
     :param loglevel: the logging level
     """
 
     def __init__(
         self,
-        sequence: List[Test],
+        sequence: list[Test],
         archive_manager: Optional[ArchiveManager] = None,
         auto_run: Optional[int] = None,
         callback: Optional[callable] = None,
         setup: Optional[callable] = None,
         teardown: Optional[callable] = None,
         on_close: Optional[callable] = None,
         loglevel=logging.INFO,
@@ -125,83 +125,83 @@
 
         if test is not None:
             return test
 
         raise KeyError(f'test "{test_element}" does not appear to be defined')
 
     @property
-    def tests(self):
+    def tests(self) -> list[Test]:
         """
         Returns instances of all tests contained within the ``TestSequence``
 
         :return: all tests as a list
         """
         return [test for test in self._sequence]
 
     @property
-    def test_names(self):
+    def test_names(self) -> list[str]:
         """
         Returns the names of the tests contained within the ``TestSequence``
 
         :return: the names of the tests as a list
         """
         return [test.moniker for test in self._sequence]
 
     @property
-    def ready(self):
+    def ready(self) -> bool:
         """
         Returns True if the test sequence is ready for another go at it, \
         False if not
 
         :return: True or False
         """
         return "ready" in self._state
 
     @property
-    def is_passing(self):
+    def is_passing(self) -> bool:
         """
         Returns True if the test sequence is currently passing, else False
 
         :return: True or False
         """
         return self._test_data.get("pass")
 
     @property
-    def is_aborted(self):
+    def is_aborted(self) -> bool:
         """
         Returns True if the test sequence has been aborted, else False
 
         :return: True or False
         """
         return "abort" in self._state
 
     @property
-    def failed_tests(self):
+    def failed_tests(self) -> list[str]:
         """
         Return a list of the tests which failed.
 
         :return: list of tests that failed
         """
         return self._test_data.get("failed")
 
     @property
-    def progress(self):
+    def progress(self) -> tuple[int, int]:
         """
         Returns a tuple containing (current_test_number, total_tests) in \
         order to give an indication of the progress of the test sequence.
 
         :return: tuple containing (current_test_number, total_tests)
         """
         return (
             self._current_test_number,
             len([test.moniker for test in self._sequence]),
         )
 
     @property
-    def in_progress(self):
+    def in_progress(self) -> bool:
         """
         Returns True if the test sequence is currently in progress, else False.
 
         :return: True if the test sequence is currently in progress, else False
         """
         return "ready" not in self._state
 
@@ -210,15 +210,15 @@
         Allows higher level code to call the close functionality.
         """
         self._state = "exiting"
         if self._on_close is not None:
             self._on_close()
 
     @staticmethod
-    def __validate_sequence(sequence: List[Test]):
+    def __validate_sequence(sequence: list[Test]):
         moniker_set = set([t.moniker for t in sequence])
 
         if len(moniker_set) != len(sequence):
             return False
 
         return True
```

## mats/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.72.0"
+__version__ = "0.73.0"
```

## Comparing `mats-0.72.0.dist-info/METADATA` & `mats-0.73.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: mats
-Version: 0.72.0
+Version: 0.73.0
 Summary: Manufacturing Automated Test System, a framework for building device testing quickly and consistently
 Home-page: https://github.com/slightlynybbled/mats
 Author: Jason R. Jones
 Author-email: slightlynybbled@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Manufacturing
 Classifier: Natural Language :: English
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: coloredlogs (==15.0.1)
+Requires-Dist: coloredlogs (>=15.0.1)
 Requires-Dist: sigfig
 
 # Manufacturing Automated Test System (MATS)
 
 [![Test, Document, Publish](https://github.com/slightlynybbled/mats/actions/workflows/publish.yml/badge.svg)](https://github.com/slightlynybbled/mats/actions/workflows/publish.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/4b8a81bf06eb48279531756d90fe598f)](https://www.codacy.com/gh/slightlynybbled/mats/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=slightlynybbled/mats&amp;utm_campaign=Badge_Grade)
 
@@ -60,12 +59,10 @@
 identically.
 
 ![GUI](docs/images/tkmats-animation.gif)
 
 ## Contribution Guidelines
 
 Contribution guidelines are outlined in the 
-[documentation](https://mats.readthedocs.io/en/latest/pages/contribution_guidelines.html).
+[documentation](https://slightlynybbled.github.io/mats/pages/contribution_guidelines.html).
 
 Please read before contributing!
-
-
```

