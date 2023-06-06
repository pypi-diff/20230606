# Comparing `tmp/angola-0.11.1.tar.gz` & `tmp/angola-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.11.1.tar", last modified: Tue May 30 04:56:37 2023, max compression
+gzip compressed data, was "angola-0.11.2.tar", last modified: Tue Jun  6 03:59:47 2023, max compression
```

## Comparing `angola-0.11.1.tar` & `angola-0.11.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.566597 angola-0.11.1/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.1/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.1/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-30 04:56:37.566666 angola-0.11.1/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.1/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-30 04:56:37.566915 angola-0.11.1/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-05-30 04:55:50.000000 angola-0.11.1/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.561551 angola-0.11.1/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.564200 angola-0.11.1/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.1/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    48027 2023-05-30 03:49:44.000000 angola-0.11.1/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    13959 2023-05-29 06:51:31.000000 angola-0.11.1/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.1/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    16742 2023-03-08 03:08:31.000000 angola-0.11.1/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    18685 2023-05-30 04:36:37.000000 angola-0.11.1/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.565050 angola-0.11.1/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.566484 angola-0.11.1/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.1/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.1/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.1/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.1/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.1/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.548185 angola-0.11.2/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.2/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.2/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-06 03:59:47.548263 angola-0.11.2/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.2/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-06 03:59:47.548534 angola-0.11.2/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-06 03:59:34.000000 angola-0.11.2/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.542195 angola-0.11.2/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.545549 angola-0.11.2/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.2/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    48027 2023-05-30 03:49:44.000000 angola-0.11.2/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.11.2/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.2/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.11.2/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    19000 2023-06-06 03:59:22.000000 angola-0.11.2/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.546494 angola-0.11.2/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-06 03:59:47.000000 angola-0.11.2/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-06 03:59:47.548015 angola-0.11.2/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.2/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.2/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.2/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.2/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.2/tests/test_query.py
```

### Comparing `angola-0.11.1/LICENSE` & `angola-0.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.11.1/PKG-INFO` & `angola-0.11.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.1
+Version: 0.11.2
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.11.1/README.md` & `angola-0.11.2/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.11.1/setup.py` & `angola-0.11.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.11.1"
+VERSION = "0.11.2"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.11.1/src/angola/database.py` & `angola-0.11.2/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.1/src/angola/dict_mutator.py` & `angola-0.11.2/src/angola/dict_mutator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 import copy
 import arrow
 import uuid
 from . import lib
 
 # ----
 
-def _j2_currdate(format_="YYYY-MM-DD", shifter=None):
+def _j2_currdate(format_="ISO_DATETIME", shifter=None):
     dt = _get_datetime()
     if shifter:
         dt = _arrow_date_shifter(dt=dt, stmt=shifter)
-    if format_.upper() == "ISODATE":
-        return dt
     return lib.arrow_date_format(dt, format_)
 
 # ----
 
 # Operators that work with list
 LISTTYPES_OPERATORS = ["xadd", "xadd_many", "xrem", "xrem_many", "xpush", "xpush_many", "xpushl", "xpushl_many"]
 
@@ -400,50 +398,15 @@
 
 def _values_to_mlist(value, many=False) -> list:
     """
     _values_to_mlist: Convert data multiple list items
     """
     return [value] if many is False else value if isinstance(value, (list, tuple)) else [value]
 
-def _arrow_date_shifter(dt: arrow.Arrow, stmt: str) -> arrow.Arrow:
-    """
-    To shift the Arrow date to future or past
-
-    Args:
-        dt:arrow.Arrow - 
-        stmt:str - 
-    Returns:
-        arrow.Arrow
-
-
-    Valid shift:
-        YEARS, MONTHS, DAYS, HOURS, MINUTES, SECONDS, WEEKS
-
-    Format: [[+/-][$NUMBER][$SHIFT][SPACE]... ]
-        +1Days
-        -3Hours 6Minutes
-        +1Days 2Hours 3Minutes
-        1Year 2Month +3Days 5Hours -6Minutes 3Seconds 5weeks
-    """
-    shifts = ["years", "months", "days",
-              "hours", "minutes", "seconds", "weeks"]
-
-    t = [t for t in stmt.split(" ") if t.strip(" ")]
-    t2 = [re.findall(r'((?:\+|\-)?(?:\d+))?(\w+)?', s)[0] for s in t if s]
-    t2 = [(t[1].lower(), int(t[0])) for t in t2 if t[0] and t[1]]
-    kw = {}
-    for k, v in t2:
-        if k in shifts or "%ss" % k in shifts:
-            k = k if k.endswith("s") else "%ss" % k
-            kw[k] = v
-    if kw:
-        dt = dt.shift(**kw)
-        return dt
-
-    return dt
+_arrow_date_shifter = lib.arrow_date_shifter
 
 def _get_datetime() -> arrow.Arrow:
     """
     Generates the current UTC datetime with Arrow date
 
     ISO FORMAT
     Date    2022-08-13
```

### Comparing `angola-0.11.1/src/angola/dict_query.py` & `angola-0.11.2/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.1/src/angola/lib.py` & `angola-0.11.2/src/angola/lib.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,24 @@
 import datetime
 from slugify import slugify
 from jinja2 import Template
 from functools import reduce
 from operator import itemgetter
 from typing import Iterator, Any
 
+# Date format
+FORMAT_ISO_DATE = "YYYY-MM-DD"
+FORMAT_ISO_TIME = "HH:mm:ss"
+FORMAT_ISO_DATETIME = "YYYY-MM-DD HH:mm:ss"
+
+DATES_FORMAT = {
+    "ISO_DATE": FORMAT_ISO_DATE,
+    "ISO_TIME": FORMAT_ISO_TIME,
+    "ISO_DATETIME": FORMAT_ISO_DATETIME
+}
 
 
 def get_sizeof(obj:Any) -> int:
     """
     Get the memory size of the object in byte.
 
     Note: make use of `sys.getsizeof` to get the size in memory. Do not use `len`
@@ -145,52 +155,64 @@
 
     Returns:
       Arrow UTC Now
     """
     return arrow.utcnow()
 
 
+_tsmapshifts = [
+    ("years", ["y", "year", "years"]),
+    ("months", ["m", "month", "months"]),
+    ("days", ["d", "day", "days"]),
+    ("hours", ["hh", "hr", "hrs", "hour", "hours"]),
+    ("minutes", ["mm", "min", "minute", "minutes"]),
+    ("seconds", ["ss", "sec", "second", "seconds"]),
+    ("weeks", ["wk", "wks", "week", "weeks"])
+]
+TS_MAP_SHIFTS =  {x:m[0] for m in _tsmapshifts for x in m[1]}
+VALID_SHIFTS = ["years", "months", "days", "hours", "minutes", "seconds", "weeks"]
+
 def arrow_date_shifter(dt: arrow.Arrow, stmt: str) -> arrow.Arrow:
     """
     To shift the Arrow date to future or past
 
     Args:
         dt:arrow.Arrow - 
         stmt:str - 
     Returns:
         arrow.Arrow
 
-
     Valid shift:
         YEARS, MONTHS, DAYS, HOURS, MINUTES, SECONDS, WEEKS
 
     Format: [[+/-][$NUMBER][$SHIFT][SPACE]... ]
         +1Days
         -3Hours 6Minutes
         +1Days 2Hours 3Minutes
         1Year 2Month +3Days 5Hours -6Minutes 3Seconds 5weeks
     """
-    shifts = ["years", "months", "days",
-              "hours", "minutes", "seconds", "weeks"]
 
     t = [t for t in stmt.split(" ") if t.strip(" ")]
     t2 = [re.findall(r'((?:\+|\-)?(?:\d+))?(\w+)?', s)[0] for s in t if s]
-    t2 = [(t[1].lower(), int(t[0])) for t in t2 if t[0] and t[1]]
-    kw = {}
-    for k, v in t2:
-        if k in shifts or "%ss" % k in shifts:
-            k = k if k.endswith("s") else "%ss" % k
-            kw[k] = v
-    if kw:
-        dt = dt.shift(**kw)
+    t3 = []
+    for l in [(t[1].lower(), int(t[0])) for t in t2 if t[0] and t[1]]:
+        if l[0] in VALID_SHIFTS:
+            t3.append(l)
+        elif l[0] in TS_MAP_SHIFTS:
+            t3.append((TS_MAP_SHIFTS.get(l[0]), l[1]))
+
+    if t3:
+        dt = dt.shift(**dict(t3))
         return dt
 
     return dt
 
 def arrow_date_format(dt:arrow.Arrow, format:str='YYYY-MM-DD HH:mm:ss ZZ') -> str:
+    if format in DATES_FORMAT:
+        format = DATES_FORMAT.get(format)
     return dt.format(format)
 
 
 def get_timestamp() -> int:
     """
     Generates the current UTC timestamp with datetime
     Returns:
```

### Comparing `angola-0.11.1/src/angola/lib_xql.py` & `angola-0.11.2/src/angola/lib_xql.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,41 +56,53 @@
         :re_match: regexp match the 
 
     Regex: 
 
 
     Example:
         {
-            "_created_at:$gt": "[[@MACRO:NOW, -3hours]]",
+            "_created_at:$gt": "[[@NOW:-3hh]]",
         }
 
     Format: [[@MACRO:NOW, shifter, format]]
     Regex: "^\[\[\@MACRO:NOW\s*,?\s*(.*)]]$",
         re_match[1]
     """
 
-    dt_format = "YYYY-MM-DD"
+    dt_format = "ISO_DATETIME"
     shifter = re_match[1]
-    if "," in shifter:
-        shifter, dt_format = shifter.split(",", 1)
+    if ";" in shifter:
+        shifter, dt_format = shifter.split(";", 1)
         shifter = shifter.strip()
         dt_format = dt_format.strip()
 
     now = lib.get_datetime()
     if shifter:
         now = lib.arrow_date_shifter(now, shifter)
-    return now.format(dt_format )
+    return now.format(lib.DATES_FORMAT.get(dt_format) if dt_format in lib.DATES_FORMAT else dt_format)
 
 MACROS_DEFS = [
+    {   
+        # TIME
+        # [[@T:]]
+        # [[@T:+2d;]]
+        # [[@T:+2d; YYYY-MM-DD HH:mm:ss]]
+        "name": "TIME",
+        "pattern": "^\[\[\@T:\s*(.*)]]$",
+        "func": _macro_now
+    },
     {
-        # [[@MACRO:NOW, +2Days, YYYY-MM-DD HH:mm:ss]]
-        "name": "NOW",
-        "pattern": "^\[\[\@MACRO:NOW\s*,?\s*(.*)]]$",
+        # NOW 
+        # [[@NOW:]]
+        # [[@NOW:+2d;]]
+        # [[@NOW:+2d; YYYY-MM-DD HH:mm:ss]]
+        "name": "NOW_ALIAS_T",
+        "pattern": "^\[\[\@NOW:\s*(.*)]]$",
         "func": _macro_now
-    }
+    },
 ]
 
 
 def eval_macros(value):
     for item in MACROS_DEFS:
         if isinstance(value, str) and (m := _re_match(item.get("pattern"), value)):
             return item.get("func")(m)
```

### Comparing `angola-0.11.1/src/angola.egg-info/PKG-INFO` & `angola-0.11.2/src/angola.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.1
+Version: 0.11.2
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.11.1/tests/test_database.py` & `angola-0.11.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.1/tests/test_dict_mutator.py` & `angola-0.11.2/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.1/tests/test_lib.py` & `angola-0.11.2/tests/test_lib.py`

 * *Files identical despite different names*

