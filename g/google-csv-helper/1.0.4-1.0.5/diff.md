# Comparing `tmp/google-csv-helper-1.0.4.tar.gz` & `tmp/google-csv-helper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-csv-helper-1.0.4.tar", last modified: Mon Jun  5 15:48:17 2023, max compression
+gzip compressed data, was "google-csv-helper-1.0.5.tar", last modified: Tue Jun  6 18:33:15 2023, max compression
```

## Comparing `google-csv-helper-1.0.4.tar` & `google-csv-helper-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:48:17.260429 google-csv-helper-1.0.4/
--rw-r--r--   0 changyy    (501) admin       (80)     3091 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/.gitignore
--rw-r--r--   0 changyy    (501) admin       (80)     1070 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/LICENSE
--rw-r--r--   0 changyy    (501) admin       (80)     3899 2023-06-05 15:48:17.260277 google-csv-helper-1.0.4/PKG-INFO
--rw-r--r--   0 changyy    (501) admin       (80)     3276 2023-06-05 14:36:39.000000 google-csv-helper-1.0.4/README.md
--rw-r--r--   0 changyy    (501) admin       (80)      177 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/build.py
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:48:17.259291 google-csv-helper-1.0.4/google_csv_helper/
--rw-r--r--   0 changyy    (501) admin       (80)      312 2023-06-05 15:44:58.000000 google-csv-helper-1.0.4/google_csv_helper/__init__.py
--rw-r--r--   0 changyy    (501) admin       (80)     7389 2023-06-05 15:36:22.000000 google-csv-helper-1.0.4/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 changyy    (501) admin       (80)     2490 2023-06-05 14:13:19.000000 google-csv-helper-1.0.4/google_csv_helper/cmd.py
--rw-r--r--   0 changyy    (501) admin       (80)     2778 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/google_csv_helper/csv_common.py
--rw-r--r--   0 changyy    (501) admin       (80)     9958 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/google_csv_helper/csv_helper.py
-drwxr-xr-x   0 changyy    (501) admin       (80)        0 2023-06-05 15:48:17.260084 google-csv-helper-1.0.4/google_csv_helper.egg-info/
--rw-r--r--   0 changyy    (501) admin       (80)     3899 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 changyy    (501) admin       (80)      470 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 changyy    (501) admin       (80)        1 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 changyy    (501) admin       (80)       65 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/entry_points.txt
--rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 changyy    (501) admin       (80)       18 2023-06-05 15:48:17.000000 google-csv-helper-1.0.4/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 changyy    (501) admin       (80)       91 2023-06-05 12:27:39.000000 google-csv-helper-1.0.4/requirements.txt
--rw-r--r--   0 changyy    (501) admin       (80)       38 2023-06-05 15:48:17.260472 google-csv-helper-1.0.4/setup.cfg
--rw-r--r--   0 changyy    (501) admin       (80)     2064 2023-06-05 15:48:16.000000 google-csv-helper-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:15.888971 google-csv-helper-1.0.5/google_csv_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/csv_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/google_csv_helper/csv_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/google_csv_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 18:33:15.000000 google-csv-helper-1.0.5/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 18:33:15.892971 google-csv-helper-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-06 18:33:04.000000 google-csv-helper-1.0.5/setup.py
```

### Comparing `google-csv-helper-1.0.4/LICENSE` & `google-csv-helper-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google-csv-helper-1.0.4/PKG-INFO` & `google-csv-helper-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # google-csv-helper
 
+[![Upload Python Package](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml)
+
 A simple tool for parsing google csv files.
 
 # Installation
 
 ```
 % pip install google-csv-helper
 ```
```

### Comparing `google-csv-helper-1.0.4/README.md` & `google-csv-helper-1.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # google-csv-helper
 
+[![Upload Python Package](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml)
+
 A simple tool for parsing google csv files.
 
 # Installation
 
 ```
 % pip install google-csv-helper
 ```
```

### Comparing `google-csv-helper-1.0.4/google_csv_helper/adsense_csv_helper.py` & `google-csv-helper-1.0.5/google_csv_helper/adsense_csv_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,18 +86,32 @@
         output["output"]["date"]["duration"]["end"] = DateFilterEnd
         output["output"]["date"]["previous"]["begin"] = prevDateFilterBegin
         output["output"]["date"]["previous"]["end"] = prevDateFilterEnd
 
 
         for k, v in self.getAllResult().items():
             target = k
-            if k.find("adsense") > 0:
-                target = "Adsense China" if k.find("cn") > 0 or k.find("china") > 0 else "Adsense Global"
-            elif k.find("admob") > 0:
-                target = "Admob China" if k.find("cn") > 0 or k.find("china") > 0 else "Admob Global"
+            #if k.find("adsense") > 0:
+            #    target = "Adsense China" if k.find("cn") > 0 or k.find("china") > 0 else "Adsense Global"
+            #elif k.find("admob") > 0:
+            #    target = "Admob China" if k.find("cn") > 0 or k.find("china") > 0 else "Admob Global"
+
+            # Check Format
+            if "Date" not in v:
+                if self.debugMode:
+                    print(f"Skip by checking 'Date': {target}")
+                continue
+            if "Date" not in v["Date"].columns:
+                if self.debugMode:
+                    print(f"Skip by checking columns['Date']['Date']: {target}")
+                continue
+            if 'Estimated earnings (USD)' not in v["Date"].columns:
+                if self.debugMode:
+                    print(f"Skip by checking columns['Date']['Estimated earnings (USD)']: {target}")
+                continue
     
             prevItemInfo = self.getDateRangeReport(v["Date"], 'Date', prevDateFilterBegin, prevDateFilterEnd, '%Y-%m-%d', '%m/%d %a')
             item = self.getDateRangeReport(v["Date"], 'Date', DateFilterBegin, DateFilterEnd, '%Y-%m-%d', '%m/%d %a')
     
             compareInfo = {}
             for lookup in csv_common.CSV_OUTPUT_REPORT_COMPARISON_INFO:
                 if lookup not in item or lookup not in prevItemInfo:
@@ -127,15 +141,15 @@
         return output
 
     def getDailyMarkDownReport(self, pickedDate: datetime.date, pickedReportKeyword: list[str]) -> str:
         data = self.getDailySummaryReport(pickedDate, pickedReportKeyword)
 
         output = [ 
             f"### Date Range: {data['output']['date']['duration']['begin']} ~ {data['output']['date']['duration']['end']}",
-            f"#### compare: {data['output']['date']['previous']['begin']} ~ {data['output']['date']['previous']['end']}",
+            f"#### Compare to previous period: {data['output']['date']['previous']['begin']} ~ {data['output']['date']['previous']['end']}",
             f"| Item | Cumulative Revenue | Average Daily Revenue | Average CPC | Min Daily Revenue | Max Daily Revenue ",
             f"| -- | --: | --: | --: | --: | --: ",
         ]
 
         for item in data["output"]["csv"]["data"]:
             output.append( f"| {item[0]} | {item[1]:,.2f} | {item[3]:,.2f} ({item[4]:.2f}%) | {item[5]:.4f} ({item[6]:.2f}%) | {item[7]:,.2f} [{item[8]}] | {item[9]:,.2f} [{item[10]}] " )
```

### Comparing `google-csv-helper-1.0.4/google_csv_helper/cmd.py` & `google-csv-helper-1.0.5/google_csv_helper/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- encoding: utf-8 -*-
 import sys
 import argparse
 import datetime
 
-from google_csv_helper import * 
+from google_csv_helper import __version__
+from google_csv_helper import adsense_csv_helper
 
 def main():
     def valid_date(data: str):
         output = datetime.date.today()
         if data != "today":
             try:
                 return datetime.datetime.strptime(data, "%Y-%m-%d")
@@ -30,15 +31,15 @@
 
     for p in args.adsense_filename_keyword.split(','):
         csv_filename_pattern.append( str(p).strip() )
     for p in args.admob_filename_keyword.split(','):
         csv_filename_pattern.append( str(p).strip() )
 
     if args.version:
-        print(version)
+        print(__version__)
         sys.exit(0)
 
     if len(args.csv_dir) == 0:
         parser.print_help()
         sys.exit(0)
 
     obj = adsense_csv_helper.AdsenseCSVHelper(args.csv_dir)
```

### Comparing `google-csv-helper-1.0.4/google_csv_helper/csv_common.py` & `google-csv-helper-1.0.5/google_csv_helper/csv_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     "週次" : "Week",
     "月份" : "Month",
     "預估收益 (USD)" : "Estimated earnings (USD)",
     "曝光" : "Impressions",
     "觀察到的有效千次曝光出價 (USD)": "Impression RPM (USD)",
     "點擊次數": "Clicks",
     "點閱率 (%) (%)" : "CTR%",
+
+    # GA3 zh-TW
+    "日索引": "Date",
+    "使用者": "User",
 }
 
 CSV_FIELD_VALUE_TRANSFORM = {
     "CTR%" : {
         "handlerType": "function",
         "handler": lambda x: str(float(x.replace('%',''))*0.01),
         "newFieldName": "CTR",
@@ -71,14 +75,18 @@
     "CPC (USD)": 1.0,
 }
 
 CSV_OUTPUT_ADSENSE_FIELDS = [
     'Estimated earnings (USD)', 'Impressions', 'Impression RPM (USD)', 'Clicks', 'CTR', 'CPC (USD)',
 ]
 
+CSV_OUTPUT_GA_FIELDS = [
+    'User',
+]
+
 CSV_INPUT_CHECK_MAIN_FIELD = [
     'Date', 'Week', 'Month',
 ]
 
 CSV_OUTPUT_REPORT_COMPARISON_INFO = [
 	'Estimated earnings (USD)', 'Average earnings (USD)' , 'Average CPC',
 ]
```

### Comparing `google-csv-helper-1.0.4/google_csv_helper.egg-info/PKG-INFO` & `google-csv-helper-1.0.5/google_csv_helper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # google-csv-helper
 
+[![Upload Python Package](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/changyy/google-csv-helper/actions/workflows/python-publish.yml)
+
 A simple tool for parsing google csv files.
 
 # Installation
 
 ```
 % pip install google-csv-helper
 ```
```

### Comparing `google-csv-helper-1.0.4/setup.py` & `google-csv-helper-1.0.5/setup.py`

 * *Files identical despite different names*

