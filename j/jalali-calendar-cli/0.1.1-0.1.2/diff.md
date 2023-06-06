# Comparing `tmp/jalali_calendar_cli-0.1.1.tar.gz` & `tmp/jalali_calendar_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jalali_calendar_cli-0.1.1.tar", max compression
+gzip compressed data, was "jalali_calendar_cli-0.1.2.tar", max compression
```

## Comparing `jalali_calendar_cli-0.1.1.tar` & `jalali_calendar_cli-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.1/jalali_calendar_cli/__init__.py
--rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.1/jalali_calendar_cli/holidays.json
--rwxr-xr-x   0        0        0     9457 2023-05-23 21:10:13.875113 jalali_calendar_cli-0.1.1/jalali_calendar_cli/jalali_calendar.py
--rw-r--r--   0        0        0      567 2023-05-23 21:10:50.110443 jalali_calendar_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1820 2023-05-23 21:10:29.983258 jalali_calendar_cli-0.1.1/readme.org
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.1/setup.py
--rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.2/jalali_calendar_cli/__init__.py
+-rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.2/jalali_calendar_cli/holidays.json
+-rwxr-xr-x   0        0        0    13770 2023-06-06 07:08:11.081221 jalali_calendar_cli-0.1.2/jalali_calendar_cli/jalali_calendar.py
+-rw-r--r--   0        0        0      567 2023-06-06 07:17:14.580430 jalali_calendar_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3230 2023-06-06 07:17:29.955783 jalali_calendar_cli-0.1.2/readme.org
+-rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.2/setup.py
+-rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.2/PKG-INFO
```

### Comparing `jalali_calendar_cli-0.1.1/jalali_calendar_cli/holidays.json` & `jalali_calendar_cli-0.1.2/jalali_calendar_cli/holidays.json`

 * *Files identical despite different names*

### Comparing `jalali_calendar_cli-0.1.1/jalali_calendar_cli/jalali_calendar.py` & `jalali_calendar_cli-0.1.2/jalali_calendar_cli/jalali_calendar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 ##
-# * @todo
-# ** Make the true color customizable.
-# *** Add a preset color theme for dark themes
-##
 import pathlib
 from typing import List
 import sys
 import jdatetime
 import datetime
 import json
 import os
 import argparse
+import colorama
 from colorama import Fore, Style, init
 
 try:
     from icecream import ic, colorize as ic_colorize
 
     ic.configureOutput(outputFunction=lambda s: print(ic_colorize(s)))
 except ImportError:
     ic = lambda *a: None if not a else (a[0] if len(a) == 1 else a)
 
 
 init(autoreset=False)
 
 
+# Color presets for different themes
+COLOR_PRESETS = {
+    "light": {
+        "weekend": {"name": "LIGHTMAGENTA_EX", "true": (85, 26, 139)},
+        "holiday": {"name": "LIGHTRED_EX", "true": (230, 69, 0)},
+        "footnote": {"name": "LIGHTBLACK_EX", "true": (170, 170, 170)},
+        "header": {"name": "BLACK", "true": (50, 50, 50)},
+    },
+    "dark": {
+        "weekend": {"name": "LIGHTMAGENTA_EX", "true": (255, 0, 255)},
+        "holiday": {"name": "LIGHTRED_EX", "true": (255, 0, 0)},
+        "footnote": {"name": "LIGHTBLACK_EX", "true": (128, 128, 128)},
+        "header": {"name": "WHITE", "true": (255, 255, 255)},
+    },
+}
+
+
 def jmonth_name(month: int) -> str:
     month_names = [
         "Farvardin",
         "Ordibehesht",
         "Khordad",
         "Tir",
         "Mordad",
@@ -100,14 +114,19 @@
     first_day_of_month: int,
     num_days: int,
     holidays: dict,
     indentation: int = 5,
     color: bool = False,
     unicode_p: bool = True,
     true_color: bool = False,
+    color_preset: str = "light",
+    weekend_color=None,
+    holiday_color=None,
+    footnote_color=None,
+    header_color=None,
 ) -> List[str]:
     assert indentation >= 4
 
     weekdays = [
         "Sat",
         "Sun",
         "Mon",
@@ -118,36 +137,36 @@
     ]
     header_indentation_len = indentation - 3
     blank1 = " " * indentation
     calendar = [blank1 * (first_day_of_month)]
     footnotes = []
     superscript_map = str.maketrans("0123456789", "⁰¹²³⁴⁵⁶⁷⁸⁹")
 
-    blue_start = (
-        generate_true_color_code(85, 26, 139)
-        if true_color
-        else (Fore.BLUE if color else "")
-    )
-    red_start = (
-        generate_true_color_code(230, 69, 0)
-        if true_color
-        else (Fore.RED if color else "")
-    )
-    gray_start = (
-        generate_true_color_code(170, 170, 170)
-        if true_color
-        else (Fore.LIGHTBLACK_EX if color else "")
-    )
-    black_start = (
-        generate_true_color_code(50, 50, 50)
-        if true_color
-        else (Fore.WHITE if color else "")
-        #: White themes should have set WHITE to the color black, and dark themes to white.
-    )
-    bold_start = Style.BRIGHT if color else ""
+    # Get color preset
+    preset = COLOR_PRESETS[color_preset]
+
+    # Determine color options
+    weekend_color = weekend_color if weekend_color else preset["weekend"]
+    holiday_color = holiday_color if holiday_color else preset["holiday"]
+    footnote_color = footnote_color if footnote_color else preset["footnote"]
+    header_color = header_color if header_color else preset["header"]
+
+    # Determine color start values
+    if true_color:
+        weekend_color_ansi = generate_true_color_code(*weekend_color["true"])
+        holiday_color_ansi = generate_true_color_code(*holiday_color["true"])
+        footnote_color_ansi = generate_true_color_code(*footnote_color["true"])
+        header_color_ansi = generate_true_color_code(*header_color["true"])
+    else:
+        weekend_color_ansi = getattr(colorama.Fore, weekend_color["name"])
+        holiday_color_ansi = getattr(colorama.Fore, holiday_color["name"])
+        footnote_color_ansi = getattr(colorama.Fore, footnote_color["name"])
+        header_color_ansi = getattr(colorama.Fore, header_color["name"])
+
+    bold_ansi = Style.BRIGHT if color else ""
     reset_color = Style.RESET_ALL if color else ""
 
     last_indentation_debt = header_indentation_len
     for day in range(1, num_days + 1):
         weekday = (day + first_day_of_month) % 7
         day_str = str(day)
         day_str = day_str.rjust(indentation - last_indentation_debt)
@@ -166,34 +185,34 @@
                 else:
                     footnote_num_str = f"[{footnote_num_str}]"
 
                 last_indentation_debt += len(footnote_num_str)
             else:
                 footnote_num_str = ""
 
-            day_str = f"{bold_start}{red_start}{day_str}{reset_color}"
+            day_str = f"{bold_ansi}{holiday_color_ansi}{day_str}{reset_color}"
             if footnote_num_str:
-                day_str += f"{gray_start}{footnote_num_str}{reset_color}"
+                day_str += f"{footnote_color_ansi}{footnote_num_str}{reset_color}"
 
         elif weekday == 0:
-            day_str = f"{blue_start}{day_str}{reset_color}"
+            day_str = f"{weekend_color_ansi}{day_str}{reset_color}"
 
         # ic(indentation, day_str, day_str.rjust(indentation))
         calendar.append(day_str)
 
         if weekday == 0:
             calendar.append("\n")
             last_indentation_debt = header_indentation_len
 
     headers_weekdays = (" " * header_indentation_len).join(weekdays)
 
     headers = ""
     year_month_str = f"{year} {jmonth_name(month)}"
-    headers += f"{bold_start}{black_start}{center_justify(year_month_str, len(headers_weekdays))}{reset_color}\n"
-    headers += f"{bold_start}{headers_weekdays}{reset_color}"
+    headers += f"{bold_ansi}{header_color_ansi}{center_justify(year_month_str, len(headers_weekdays))}{reset_color}\n"
+    headers += f"{bold_ansi}{headers_weekdays}{reset_color}"
 
     return f"{headers}\n{''.join(calendar)}", "\n".join(footnotes)
 
 
 def load_holidays(holidays_data, year: int, month: int) -> dict:
     year_str = str(year)
     if year_str in holidays_data:
@@ -213,14 +232,19 @@
     month: int,
     color: bool,
     unicode_p: bool,
     indentation: int,
     true_color: bool,
     holidays_data,
     footnotes_p: bool = True,
+    color_preset: str = "light",
+    weekend_color=None,
+    holiday_color=None,
+    footnote_color=None,
+    header_color=None,
 ) -> None:
     j_date = jdatetime.date(year, month, 1)
     first_day_of_month = j_date.weekday()
     num_days = get_jalali_days(year, month)
     holidays = load_holidays(holidays_data, year, month)
     calendar, footnotes = generate_calendar(
         year,
@@ -228,14 +252,19 @@
         first_day_of_month,
         num_days,
         holidays,
         indentation=indentation,
         color=color,
         unicode_p=unicode_p,
         true_color=true_color,
+        color_preset=color_preset,
+        weekend_color=weekend_color,
+        holiday_color=holiday_color,
+        footnote_color=footnote_color,
+        header_color=header_color,
     )
     line_indent = " "
     calendar = prefix_lines(calendar, prefix=line_indent)
     print(calendar)
 
     if footnotes_p:
         footnotes = prefix_lines(footnotes, prefix=f"{line_indent}  ")
@@ -244,17 +273,16 @@
         print(footnotes)
 
 
 def main(args=None) -> None:
     if args is None:
         args = sys.argv
 
-    default_holiday_data_json_path = (
-        os.getenv("JALALI_HOLIDAYS_JSON_PATH")
-        or str(pathlib.Path(__file__).parent / "holidays.json")
+    default_holiday_data_json_path = os.getenv("JALALI_HOLIDAYS_JSON_PATH") or str(
+        pathlib.Path(__file__).parent / "holidays.json"
     )
     # ic(default_holiday_data_json_path)
 
     parser = argparse.ArgumentParser()
 
     ##
     # Get current Jalali date
@@ -316,31 +344,119 @@
     parser.add_argument(
         "--holidays-json-path",
         type=str,
         default=default_holiday_data_json_path,
         help="path to JSON file containing holiday data",
     )
 
+    parser.add_argument(
+        "--color-preset",
+        type=str,
+        default="light",
+        help="color preset for the calendar output (default: light)",
+    )
+
+    true_color_group = parser.add_argument_group("24-bit True Color Options")
+    true_color_group.add_argument(
+        "--weekend-true-color",
+        type=str,
+        default=None,
+        help="RGB values for weekend color in 24-bit True Color",
+    )
+    true_color_group.add_argument(
+        "--holiday-true-color",
+        type=str,
+        default=None,
+        help="RGB values for holiday color in 24-bit True Color",
+    )
+    true_color_group.add_argument(
+        "--footnote-true-color",
+        type=str,
+        default=None,
+        # help="RGB values for footnote color in 24-bit True Color",
+        help=argparse.SUPPRESS,
+    )
+    true_color_group.add_argument(
+        "--header-true-color",
+        type=str,
+        default=None,
+        help="RGB values for header color in 24-bit True Color",
+    )
+
+    colorama_color_group = parser.add_argument_group("Colorama 256 Color Options")
+    colorama_color_group.add_argument(
+        "--weekend-color",
+        type=str,
+        default=None,
+        help="Colorama color name for weekend color",
+    )
+    colorama_color_group.add_argument(
+        "--holiday-color",
+        type=str,
+        default=None,
+        help="Colorama color name for holiday color",
+    )
+    colorama_color_group.add_argument(
+        "--footnote-color",
+        type=str,
+        default=None,
+        # help="Colorama color name for footnote color",
+        help=argparse.SUPPRESS,
+    )
+    colorama_color_group.add_argument(
+        "--header-color",
+        type=str,
+        default=None,
+        help="Colorama color name for header color",
+    )
+
     args = parser.parse_args()
 
     color = args.color == "always" or (args.color == "auto" and sys.stdout.isatty())
 
+    colors = dict()
+    color_keys = ["weekend", "holiday", "footnote", "header"]
+    if args.true_color:
+        for color_key in color_keys:
+            color_arg = getattr(args, f"{color_key}_true_color", None)
+            if color_arg:
+                if color_key not in colors:
+                    colors[color_key] = dict()
+                colors[color_key]["true"] = tuple(map(int, color_arg.split(",")))
+    else:
+        for color_key in color_keys:
+            color_arg = getattr(args, f"{color_key}_color", None)
+            if color_arg:
+                if color_key not in colors:
+                    colors[color_key] = dict()
+                colors[color_key]["name"] = color_arg.upper()
+
+    weekend_color = colors.get("weekend", None)
+    holiday_color = colors.get("holiday", None)
+    footnote_color = colors.get("footnote", None)
+    header_color = colors.get("header", None)
+
     unicode_p = True
     # unicode_p = args.unicode
 
     with open(args.holidays_json_path) as f:
         holidays_data = json.load(f)
 
     jalali_calendar(
         args.year,
         args.month,
         color,
         unicode_p,
         args.indentation,
         args.true_color,
-        footnotes_p=args.footnotes,
         holidays_data=holidays_data,
+        footnotes_p=args.footnotes,
+        color_preset=args.color_preset,
+        weekend_color=weekend_color,
+        holiday_color=holiday_color,
+        footnote_color=footnote_color,
+        header_color=header_color,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jalali_calendar_cli-0.1.1/pyproject.toml` & `jalali_calendar_cli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jalali-calendar-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "Jalali (Shamsi) calendar in your terminal, with holidays"
 authors = ["NightMachinery <feraidoonmehri@gmail.com>"]
 readme = "readme.org"
 packages = [{include = "jalali_calendar_cli"}]
 
 
 [tool.poetry.scripts]
```

### Comparing `jalali_calendar_cli-0.1.1/setup.py` & `jalali_calendar_cli-0.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 entry_points = \
 {'console_scripts': ['jalali-calendar = '
                      'jalali_calendar_cli.jalali_calendar:main',
                      'jcal = jalali_calendar_cli.jalali_calendar:main']}
 
 setup_kwargs = {
     'name': 'jalali-calendar-cli',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Jalali (Shamsi) calendar in your terminal, with holidays',
-    'long_description': '#+TITLE: jalali-calendar-cli\n\n* Install\n#+begin_example bash\npip install -U jalali-calendar-cli\n#+end_example\n\n* Usage\n#+ATTR_HTML: :width 800\n[[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]\n\n#+begin_example bash\nusage: jcal [-h] [--color {auto,always,never}]\n            [--true-color | --no-true-color] [--footnotes | --no-footnotes]\n            [--indentation INDENTATION]\n            [--holidays-json-path HOLIDAYS_JSON_PATH]\n            [month] [year]\n\npositional arguments:\n  month                 month in Jalali calendar (default: current month)\n  year                  year in Jalali calendar (default: current year)\n\noptions:\n  -h, --help            show this help message and exit\n  --color {auto,always,never}\n                        colorize the output\n  --true-color, --no-true-color\n                        enable true color support for output (default: False)\n  --footnotes, --no-footnotes\n                        show footnotes in the output (default: True)\n  --indentation INDENTATION\n                        number of spaces for indentation (default: 5)\n  --holidays-json-path HOLIDAYS_JSON_PATH\n                        path to JSON file containing holiday data\n#+end_example\n\n#+begin_example bash\njcal 12\n#+end_example\n\n#+begin_example\n            1402 Esfand           \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n                  1    2    3    4\n   5    6    7    8    9   10   11\n  12   13   14   15   16   17   18\n  19   20   21   22   23   24   25\n  26   27   28   29\n\n Holidays:\n   6: Birthday of Imam Mahdi\n   29: Nationalization of the Oil Industry\n#+end_example\n\n* Holidays Data\nThe default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date, but you can always supply your own.\n\n',
+    'long_description': '#+TITLE: jalali-calendar-cli\n\nJalali (Shamsi) calendar in your terminal, with holidays\n\n* Install\n#+begin_example bash\npip install -U jalali-calendar-cli\n#+end_example\n\n* Usage\n#+ATTR_HTML: :width 884\n[[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_103928_zRAerD.png]]\n\n#+begin_example bash\nusage: jalali-calendar [-h] [--color {auto,always,never}]\n                       [--true-color | --no-true-color]\n                       [--footnotes | --no-footnotes]\n                       [--indentation INDENTATION]\n                       [--holidays-json-path HOLIDAYS_JSON_PATH]\n                       [--color-preset COLOR_PRESET]\n                       [--weekend-true-color WEEKEND_TRUE_COLOR]\n                       [--holiday-true-color HOLIDAY_TRUE_COLOR]\n                       [--header-true-color HEADER_TRUE_COLOR]\n                       [--weekend-color WEEKEND_COLOR]\n                       [--holiday-color HOLIDAY_COLOR]\n                       [--header-color HEADER_COLOR]\n                       [month] [year]\n\npositional arguments:\n  month                 month in Jalali calendar (default: current month)\n  year                  year in Jalali calendar (default: current year)\n\noptions:\n  -h, --help            show this help message and exit\n  --color {auto,always,never}\n                        colorize the output\n  --true-color, --no-true-color\n                        enable true color support for output (default: False)\n  --footnotes, --no-footnotes\n                        show footnotes in the output (default: True)\n  --indentation INDENTATION\n                        number of spaces for indentation (default: 5)\n  --holidays-json-path HOLIDAYS_JSON_PATH\n                        path to JSON file containing holiday data\n  --color-preset COLOR_PRESET\n                        color preset for the calendar output (default: light)\n\n24-bit True Color Options:\n  --weekend-true-color WEEKEND_TRUE_COLOR\n                        RGB values for weekend color in 24-bit True Color\n  --holiday-true-color HOLIDAY_TRUE_COLOR\n                        RGB values for holiday color in 24-bit True Color\n  --header-true-color HEADER_TRUE_COLOR\n                        RGB values for header color in 24-bit True Color\n\nColorama 256 Color Options:\n  --weekend-color WEEKEND_COLOR\n                        Colorama color name for weekend color\n  --holiday-color HOLIDAY_COLOR\n                        Colorama color name for holiday color\n  --header-color HEADER_COLOR\n                        Colorama color name for header color\n#+end_example\n\n#+begin_example bash\njcal 12\n#+end_example\n\n#+begin_example\n            1402 Esfand           \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n                  1    2    3    4\n   5    6    7    8    9   10   11\n  12   13   14   15   16   17   18\n  19   20   21   22   23   24   25\n  26   27   28   29\n\n Holidays:\n   6: Birthday of Imam Mahdi\n   29: Nationalization of the Oil Industry\n#+end_example\n\n* Holidays Data\nThe default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date, but you can always supply your own.\n\n',
     'author': 'NightMachinery',
     'author_email': 'feraidoonmehri@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jalali_calendar_cli-0.1.1/PKG-INFO` & `jalali_calendar_cli-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 Metadata-Version: 2.1
 Name: jalali-calendar-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jalali (Shamsi) calendar in your terminal, with holidays
 Author: NightMachinery
 Author-email: feraidoonmehri@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: jdatetime (>=4.1.1,<5.0.0)
 Description-Content-Type: text/plain
 
 #+TITLE: jalali-calendar-cli
 
+Jalali (Shamsi) calendar in your terminal, with holidays
+
 * Install
 #+begin_example bash
 pip install -U jalali-calendar-cli
 #+end_example
 
 * Usage
-#+ATTR_HTML: :width 800
+#+ATTR_HTML: :width 884
 [[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]
+#+ATTR_HTML: :width 968
+[[file:readme.org_imgs/20230606_103928_zRAerD.png]]
 
 #+begin_example bash
-usage: jcal [-h] [--color {auto,always,never}]
-            [--true-color | --no-true-color] [--footnotes | --no-footnotes]
-            [--indentation INDENTATION]
-            [--holidays-json-path HOLIDAYS_JSON_PATH]
-            [month] [year]
+usage: jalali-calendar [-h] [--color {auto,always,never}]
+                       [--true-color | --no-true-color]
+                       [--footnotes | --no-footnotes]
+                       [--indentation INDENTATION]
+                       [--holidays-json-path HOLIDAYS_JSON_PATH]
+                       [--color-preset COLOR_PRESET]
+                       [--weekend-true-color WEEKEND_TRUE_COLOR]
+                       [--holiday-true-color HOLIDAY_TRUE_COLOR]
+                       [--header-true-color HEADER_TRUE_COLOR]
+                       [--weekend-color WEEKEND_COLOR]
+                       [--holiday-color HOLIDAY_COLOR]
+                       [--header-color HEADER_COLOR]
+                       [month] [year]
 
 positional arguments:
   month                 month in Jalali calendar (default: current month)
   year                  year in Jalali calendar (default: current year)
 
 options:
   -h, --help            show this help message and exit
@@ -42,14 +54,32 @@
                         enable true color support for output (default: False)
   --footnotes, --no-footnotes
                         show footnotes in the output (default: True)
   --indentation INDENTATION
                         number of spaces for indentation (default: 5)
   --holidays-json-path HOLIDAYS_JSON_PATH
                         path to JSON file containing holiday data
+  --color-preset COLOR_PRESET
+                        color preset for the calendar output (default: light)
+
+24-bit True Color Options:
+  --weekend-true-color WEEKEND_TRUE_COLOR
+                        RGB values for weekend color in 24-bit True Color
+  --holiday-true-color HOLIDAY_TRUE_COLOR
+                        RGB values for holiday color in 24-bit True Color
+  --header-true-color HEADER_TRUE_COLOR
+                        RGB values for header color in 24-bit True Color
+
+Colorama 256 Color Options:
+  --weekend-color WEEKEND_COLOR
+                        Colorama color name for weekend color
+  --holiday-color HOLIDAY_COLOR
+                        Colorama color name for holiday color
+  --header-color HEADER_COLOR
+                        Colorama color name for header color
 #+end_example
 
 #+begin_example bash
 jcal 12
 #+end_example
 
 #+begin_example
```

