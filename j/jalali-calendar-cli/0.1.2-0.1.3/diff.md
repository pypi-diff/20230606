# Comparing `tmp/jalali_calendar_cli-0.1.2.tar.gz` & `tmp/jalali_calendar_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jalali_calendar_cli-0.1.2.tar", max compression
+gzip compressed data, was "jalali_calendar_cli-0.1.3.tar", max compression
```

## Comparing `jalali_calendar_cli-0.1.2.tar` & `jalali_calendar_cli-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.2/jalali_calendar_cli/__init__.py
--rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.2/jalali_calendar_cli/holidays.json
--rwxr-xr-x   0        0        0    13770 2023-06-06 07:08:11.081221 jalali_calendar_cli-0.1.2/jalali_calendar_cli/jalali_calendar.py
--rw-r--r--   0        0        0      567 2023-06-06 07:17:14.580430 jalali_calendar_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3230 2023-06-06 07:17:29.955783 jalali_calendar_cli-0.1.2/readme.org
--rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.2/setup.py
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.3/jalali_calendar_cli/__init__.py
+-rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.3/jalali_calendar_cli/holidays.json
+-rwxr-xr-x   0        0        0    13776 2023-06-06 08:18:04.466189 jalali_calendar_cli-0.1.3/jalali_calendar_cli/jalali_calendar.py
+-rw-r--r--   0        0        0      567 2023-06-06 08:17:52.932757 jalali_calendar_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3755 2023-06-06 08:19:58.571203 jalali_calendar_cli-0.1.3/readme.org
+-rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.3/setup.py
+-rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.3/PKG-INFO
```

### Comparing `jalali_calendar_cli-0.1.2/jalali_calendar_cli/holidays.json` & `jalali_calendar_cli-0.1.3/jalali_calendar_cli/holidays.json`

 * *Files identical despite different names*

### Comparing `jalali_calendar_cli-0.1.2/jalali_calendar_cli/jalali_calendar.py` & `jalali_calendar_cli-0.1.3/jalali_calendar_cli/jalali_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,20 +169,20 @@
     for day in range(1, num_days + 1):
         weekday = (day + first_day_of_month) % 7
         day_str = str(day)
         day_str = day_str.rjust(indentation - last_indentation_debt)
         last_indentation_debt = 0
 
         if day in holidays:
-            footnotes.append(f"{day}: {holidays[day]}")
+            footnotes.append(f"{day:2d}: {holidays[day]}")
 
             if (
                 False
             ):  #: @cruft no need to use footnotes when the days can act as indices already
-                footnotes.append(f"{len(footnotes)+1}: {holidays[day]}")
+                footnotes.append(f"{len(footnotes)+1:2d}: {holidays[day]}")
                 footnote_num_str = str(len(footnotes))
                 if unicode_p:
                     footnote_num_str = footnote_num_str.translate(superscript_map)
                 else:
                     footnote_num_str = f"[{footnote_num_str}]"
 
                 last_indentation_debt += len(footnote_num_str)
```

### Comparing `jalali_calendar_cli-0.1.2/pyproject.toml` & `jalali_calendar_cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jalali-calendar-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "Jalali (Shamsi) calendar in your terminal, with holidays"
 authors = ["NightMachinery <feraidoonmehri@gmail.com>"]
 readme = "readme.org"
 packages = [{include = "jalali_calendar_cli"}]
 
 
 [tool.poetry.scripts]
```

### Comparing `jalali_calendar_cli-0.1.2/readme.org` & `jalali_calendar_cli-0.1.3/readme.org`

 * *Files 12% similar despite different names*

```diff
@@ -74,14 +74,33 @@
                   1    2    3    4
    5    6    7    8    9   10   11
   12   13   14   15   16   17   18
   19   20   21   22   23   24   25
   26   27   28   29
 
  Holidays:
-   6: Birthday of Imam Mahdi
+    6: Birthday of Imam Mahdi
    29: Nationalization of the Oil Industry
 #+end_example
 
+#+begin_example bash
+jcal 7 1402
+#+end_example
+
+#+begin_example
+             1402 Mehr            
+ Sat  Sun  Mon  Tue  Wed  Thu  Fri
+   1    2    3    4    5    6    7
+   8    9   10   11   12   13   14
+  15   16   17   18   19   20   21
+  22   23   24   25   26   27   28
+  29   30
+
+ Holidays:
+    2: Martyrdom of Imam Hassan Askari and Start of Imamate of Imam Mahdi
+   11: Birthday of Prophet Muhammad and Imam Sadiq
+#+end_example
+
 * Holidays Data
-The default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date, but you can always supply your own.
+The default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date for the upcoming years, but you can always supply your own.
 
+The holiday data of previous years (≤1401) has not been added.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jalali_calendar_cli-0.1.2/setup.py` & `jalali_calendar_cli-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 entry_points = \
 {'console_scripts': ['jalali-calendar = '
                      'jalali_calendar_cli.jalali_calendar:main',
                      'jcal = jalali_calendar_cli.jalali_calendar:main']}
 
 setup_kwargs = {
     'name': 'jalali-calendar-cli',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Jalali (Shamsi) calendar in your terminal, with holidays',
-    'long_description': '#+TITLE: jalali-calendar-cli\n\nJalali (Shamsi) calendar in your terminal, with holidays\n\n* Install\n#+begin_example bash\npip install -U jalali-calendar-cli\n#+end_example\n\n* Usage\n#+ATTR_HTML: :width 884\n[[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_103928_zRAerD.png]]\n\n#+begin_example bash\nusage: jalali-calendar [-h] [--color {auto,always,never}]\n                       [--true-color | --no-true-color]\n                       [--footnotes | --no-footnotes]\n                       [--indentation INDENTATION]\n                       [--holidays-json-path HOLIDAYS_JSON_PATH]\n                       [--color-preset COLOR_PRESET]\n                       [--weekend-true-color WEEKEND_TRUE_COLOR]\n                       [--holiday-true-color HOLIDAY_TRUE_COLOR]\n                       [--header-true-color HEADER_TRUE_COLOR]\n                       [--weekend-color WEEKEND_COLOR]\n                       [--holiday-color HOLIDAY_COLOR]\n                       [--header-color HEADER_COLOR]\n                       [month] [year]\n\npositional arguments:\n  month                 month in Jalali calendar (default: current month)\n  year                  year in Jalali calendar (default: current year)\n\noptions:\n  -h, --help            show this help message and exit\n  --color {auto,always,never}\n                        colorize the output\n  --true-color, --no-true-color\n                        enable true color support for output (default: False)\n  --footnotes, --no-footnotes\n                        show footnotes in the output (default: True)\n  --indentation INDENTATION\n                        number of spaces for indentation (default: 5)\n  --holidays-json-path HOLIDAYS_JSON_PATH\n                        path to JSON file containing holiday data\n  --color-preset COLOR_PRESET\n                        color preset for the calendar output (default: light)\n\n24-bit True Color Options:\n  --weekend-true-color WEEKEND_TRUE_COLOR\n                        RGB values for weekend color in 24-bit True Color\n  --holiday-true-color HOLIDAY_TRUE_COLOR\n                        RGB values for holiday color in 24-bit True Color\n  --header-true-color HEADER_TRUE_COLOR\n                        RGB values for header color in 24-bit True Color\n\nColorama 256 Color Options:\n  --weekend-color WEEKEND_COLOR\n                        Colorama color name for weekend color\n  --holiday-color HOLIDAY_COLOR\n                        Colorama color name for holiday color\n  --header-color HEADER_COLOR\n                        Colorama color name for header color\n#+end_example\n\n#+begin_example bash\njcal 12\n#+end_example\n\n#+begin_example\n            1402 Esfand           \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n                  1    2    3    4\n   5    6    7    8    9   10   11\n  12   13   14   15   16   17   18\n  19   20   21   22   23   24   25\n  26   27   28   29\n\n Holidays:\n   6: Birthday of Imam Mahdi\n   29: Nationalization of the Oil Industry\n#+end_example\n\n* Holidays Data\nThe default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date, but you can always supply your own.\n\n',
+    'long_description': '#+TITLE: jalali-calendar-cli\n\nJalali (Shamsi) calendar in your terminal, with holidays\n\n* Install\n#+begin_example bash\npip install -U jalali-calendar-cli\n#+end_example\n\n* Usage\n#+ATTR_HTML: :width 884\n[[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_103928_zRAerD.png]]\n\n#+begin_example bash\nusage: jalali-calendar [-h] [--color {auto,always,never}]\n                       [--true-color | --no-true-color]\n                       [--footnotes | --no-footnotes]\n                       [--indentation INDENTATION]\n                       [--holidays-json-path HOLIDAYS_JSON_PATH]\n                       [--color-preset COLOR_PRESET]\n                       [--weekend-true-color WEEKEND_TRUE_COLOR]\n                       [--holiday-true-color HOLIDAY_TRUE_COLOR]\n                       [--header-true-color HEADER_TRUE_COLOR]\n                       [--weekend-color WEEKEND_COLOR]\n                       [--holiday-color HOLIDAY_COLOR]\n                       [--header-color HEADER_COLOR]\n                       [month] [year]\n\npositional arguments:\n  month                 month in Jalali calendar (default: current month)\n  year                  year in Jalali calendar (default: current year)\n\noptions:\n  -h, --help            show this help message and exit\n  --color {auto,always,never}\n                        colorize the output\n  --true-color, --no-true-color\n                        enable true color support for output (default: False)\n  --footnotes, --no-footnotes\n                        show footnotes in the output (default: True)\n  --indentation INDENTATION\n                        number of spaces for indentation (default: 5)\n  --holidays-json-path HOLIDAYS_JSON_PATH\n                        path to JSON file containing holiday data\n  --color-preset COLOR_PRESET\n                        color preset for the calendar output (default: light)\n\n24-bit True Color Options:\n  --weekend-true-color WEEKEND_TRUE_COLOR\n                        RGB values for weekend color in 24-bit True Color\n  --holiday-true-color HOLIDAY_TRUE_COLOR\n                        RGB values for holiday color in 24-bit True Color\n  --header-true-color HEADER_TRUE_COLOR\n                        RGB values for header color in 24-bit True Color\n\nColorama 256 Color Options:\n  --weekend-color WEEKEND_COLOR\n                        Colorama color name for weekend color\n  --holiday-color HOLIDAY_COLOR\n                        Colorama color name for holiday color\n  --header-color HEADER_COLOR\n                        Colorama color name for header color\n#+end_example\n\n#+begin_example bash\njcal 12\n#+end_example\n\n#+begin_example\n            1402 Esfand           \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n                  1    2    3    4\n   5    6    7    8    9   10   11\n  12   13   14   15   16   17   18\n  19   20   21   22   23   24   25\n  26   27   28   29\n\n Holidays:\n    6: Birthday of Imam Mahdi\n   29: Nationalization of the Oil Industry\n#+end_example\n\n#+begin_example bash\njcal 7 1402\n#+end_example\n\n#+begin_example\n             1402 Mehr            \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n   1    2    3    4    5    6    7\n   8    9   10   11   12   13   14\n  15   16   17   18   19   20   21\n  22   23   24   25   26   27   28\n  29   30\n\n Holidays:\n    2: Martyrdom of Imam Hassan Askari and Start of Imamate of Imam Mahdi\n   11: Birthday of Prophet Muhammad and Imam Sadiq\n#+end_example\n\n* Holidays Data\nThe default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date for the upcoming years, but you can always supply your own.\n\nThe holiday data of previous years (≤1401) has not been added.\n',
     'author': 'NightMachinery',
     'author_email': 'feraidoonmehri@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jalali_calendar_cli-0.1.2/PKG-INFO` & `jalali_calendar_cli-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jalali-calendar-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jalali (Shamsi) calendar in your terminal, with holidays
 Author: NightMachinery
 Author-email: feraidoonmehri@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -88,15 +88,34 @@
                   1    2    3    4
    5    6    7    8    9   10   11
   12   13   14   15   16   17   18
   19   20   21   22   23   24   25
   26   27   28   29
 
  Holidays:
-   6: Birthday of Imam Mahdi
+    6: Birthday of Imam Mahdi
    29: Nationalization of the Oil Industry
 #+end_example
 
+#+begin_example bash
+jcal 7 1402
+#+end_example
+
+#+begin_example
+             1402 Mehr            
+ Sat  Sun  Mon  Tue  Wed  Thu  Fri
+   1    2    3    4    5    6    7
+   8    9   10   11   12   13   14
+  15   16   17   18   19   20   21
+  22   23   24   25   26   27   28
+  29   30
+
+ Holidays:
+    2: Martyrdom of Imam Hassan Askari and Start of Imamate of Imam Mahdi
+   11: Birthday of Prophet Muhammad and Imam Sadiq
+#+end_example
+
 * Holidays Data
-The default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date, but you can always supply your own.
+The default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date for the upcoming years, but you can always supply your own.
 
+The holiday data of previous years (≤1401) has not been added.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

