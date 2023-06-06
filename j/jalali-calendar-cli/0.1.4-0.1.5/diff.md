# Comparing `tmp/jalali_calendar_cli-0.1.4.tar.gz` & `tmp/jalali_calendar_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jalali_calendar_cli-0.1.4.tar", max compression
+gzip compressed data, was "jalali_calendar_cli-0.1.5.tar", max compression
```

## Comparing `jalali_calendar_cli-0.1.4.tar` & `jalali_calendar_cli-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.4/jalali_calendar_cli/__init__.py
--rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.4/jalali_calendar_cli/holidays.json
--rwxr-xr-x   0        0        0    13776 2023-06-06 09:33:07.404687 jalali_calendar_cli-0.1.4/jalali_calendar_cli/jalali_calendar.py
--rw-r--r--   0        0        0      567 2023-06-06 09:34:01.168009 jalali_calendar_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4363 2023-06-06 09:33:49.122724 jalali_calendar_cli-0.1.4/readme.org
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.4/setup.py
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-23 20:42:38.619220 jalali_calendar_cli-0.1.5/jalali_calendar_cli/__init__.py
+-rw-r--r--   0        0        0     3653 2023-05-23 20:16:16.981447 jalali_calendar_cli-0.1.5/jalali_calendar_cli/holidays.json
+-rwxr-xr-x   0        0        0    13794 2023-06-06 09:51:22.047303 jalali_calendar_cli-0.1.5/jalali_calendar_cli/jalali_calendar.py
+-rw-r--r--   0        0        0      567 2023-06-06 09:52:10.604481 jalali_calendar_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4632 2023-06-06 09:51:51.076976 jalali_calendar_cli-0.1.5/readme.org
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.5/setup.py
+-rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 jalali_calendar_cli-0.1.5/PKG-INFO
```

### Comparing `jalali_calendar_cli-0.1.4/jalali_calendar_cli/holidays.json` & `jalali_calendar_cli-0.1.5/jalali_calendar_cli/holidays.json`

 * *Files identical despite different names*

### Comparing `jalali_calendar_cli-0.1.4/jalali_calendar_cli/jalali_calendar.py` & `jalali_calendar_cli-0.1.5/jalali_calendar_cli/jalali_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         type=str,
         default=default_holiday_data_json_path,
         help="path to JSON file containing holiday data",
     )
 
     parser.add_argument(
         "--color-preset",
-        type=str,
+        choices=["light", "dark",],
         default="light",
         help="color preset for the calendar output (default: light)",
     )
 
     true_color_group = parser.add_argument_group("24-bit true color options")
     true_color_group.add_argument(
         "--weekend-true-color",
```

### Comparing `jalali_calendar_cli-0.1.4/pyproject.toml` & `jalali_calendar_cli-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jalali-calendar-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "Jalali (Shamsi) calendar in your terminal, with holidays"
 authors = ["NightMachinery <feraidoonmehri@gmail.com>"]
 readme = "readme.org"
 packages = [{include = "jalali_calendar_cli"}]
 
 
 [tool.poetry.scripts]
```

### Comparing `jalali_calendar_cli-0.1.4/readme.org` & `jalali_calendar_cli-0.1.5/readme.org`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 #+begin_example bash
 usage: jalali-calendar [-h] [--color {auto,always,never}]
                        [--true-color | --no-true-color]
                        [--footnotes | --no-footnotes]
                        [--indentation INDENTATION]
                        [--holidays-json-path HOLIDAYS_JSON_PATH]
-                       [--color-preset COLOR_PRESET]
+                       [--color-preset {light,dark}]
                        [--weekend-true-color WEEKEND_TRUE_COLOR]
                        [--holiday-true-color HOLIDAY_TRUE_COLOR]
                        [--header-true-color HEADER_TRUE_COLOR]
                        [--weekend-color WEEKEND_COLOR]
                        [--holiday-color HOLIDAY_COLOR]
                        [--header-color HEADER_COLOR]
                        [month] [year]
@@ -46,15 +46,15 @@
                         enable true color support for output (default: False)
   --footnotes, --no-footnotes
                         show footnotes in the output (default: True)
   --indentation INDENTATION
                         number of spaces for indentation (default: 5)
   --holidays-json-path HOLIDAYS_JSON_PATH
                         path to JSON file containing holiday data
-  --color-preset COLOR_PRESET
+  --color-preset {light,dark}
                         color preset for the calendar output (default: light)
 
 24-bit true color options:
   --weekend-true-color WEEKEND_TRUE_COLOR
                         RGB values for weekend color in 24-bit true color
   --holiday-true-color HOLIDAY_TRUE_COLOR
                         RGB values for holiday color in 24-bit true color
@@ -109,14 +109,23 @@
 
 #+ATTR_HTML: :width 968
 [[file:readme.org_imgs/20230606_125617_sazNzJ.png]]
 
 #+ATTR_HTML: :width 968
 [[file:readme.org_imgs/20230606_103928_zRAerD.png]]
 
+*** Shell Aliases in Bash
+You can add aliases to =~/.bashrc= and =~/.bash_profile= to persist your settings:
+
+#+begin_example bash
+alias jcal='command jcal --color-preset dark'
+#+end_example
+
+Aliases work the same way in Zsh, you just need to add them to =~/.zshenv=.
+
 ** =colorama= Colors
 These colors are defined by your terminal theme. Use true (24-bit) colors if you want to specify colors in RGB.
 
 #+begin_example
 BLACK
 BLUE
 CYAN
```

### Comparing `jalali_calendar_cli-0.1.4/setup.py` & `jalali_calendar_cli-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 entry_points = \
 {'console_scripts': ['jalali-calendar = '
                      'jalali_calendar_cli.jalali_calendar:main',
                      'jcal = jalali_calendar_cli.jalali_calendar:main']}
 
 setup_kwargs = {
     'name': 'jalali-calendar-cli',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Jalali (Shamsi) calendar in your terminal, with holidays',
-    'long_description': '#+TITLE: jalali-calendar-cli\n\nJalali (Shamsi) calendar in your terminal, with holidays\n\n* Install\n#+begin_example bash\npip install -U jalali-calendar-cli\n#+end_example\n\nThis requires Python ≥3.10.\n\n* Usage\n# #+ATTR_HTML: :width 884\n# [[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]\n#+ATTR_HTML: :width 914\n[[file:readme.org_imgs/20230606_125421_Bh79HZ.png]]\n\n#+ATTR_HTML: :width 900\n[[file:readme.org_imgs/20230606_125356_jLt2Jh.png]]\n\n\n#+begin_example bash\nusage: jalali-calendar [-h] [--color {auto,always,never}]\n                       [--true-color | --no-true-color]\n                       [--footnotes | --no-footnotes]\n                       [--indentation INDENTATION]\n                       [--holidays-json-path HOLIDAYS_JSON_PATH]\n                       [--color-preset COLOR_PRESET]\n                       [--weekend-true-color WEEKEND_TRUE_COLOR]\n                       [--holiday-true-color HOLIDAY_TRUE_COLOR]\n                       [--header-true-color HEADER_TRUE_COLOR]\n                       [--weekend-color WEEKEND_COLOR]\n                       [--holiday-color HOLIDAY_COLOR]\n                       [--header-color HEADER_COLOR]\n                       [month] [year]\n\npositional arguments:\n  month                 month in Jalali calendar (default: current month)\n  year                  year in Jalali calendar (default: current year)\n\noptions:\n  -h, --help            show this help message and exit\n  --color {auto,always,never}\n                        colorize the output\n  --true-color, --no-true-color\n                        enable true color support for output (default: False)\n  --footnotes, --no-footnotes\n                        show footnotes in the output (default: True)\n  --indentation INDENTATION\n                        number of spaces for indentation (default: 5)\n  --holidays-json-path HOLIDAYS_JSON_PATH\n                        path to JSON file containing holiday data\n  --color-preset COLOR_PRESET\n                        color preset for the calendar output (default: light)\n\n24-bit true color options:\n  --weekend-true-color WEEKEND_TRUE_COLOR\n                        RGB values for weekend color in 24-bit true color\n  --holiday-true-color HOLIDAY_TRUE_COLOR\n                        RGB values for holiday color in 24-bit true color\n  --header-true-color HEADER_TRUE_COLOR\n                        RGB values for header color in 24-bit true color\n\ncolorama 256 color options:\n  --weekend-color WEEKEND_COLOR\n                        colorama color name for weekend color\n  --holiday-color HOLIDAY_COLOR\n                        colorama color name for holiday color\n  --header-color HEADER_COLOR\n                        colorama color name for header color\n#+end_example\n\n** Examples\n#+begin_example bash\njcal 12\n#+end_example\n\n#+begin_example\n            1402 Esfand           \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n                  1    2    3    4\n   5    6    7    8    9   10   11\n  12   13   14   15   16   17   18\n  19   20   21   22   23   24   25\n  26   27   28   29\n\n Holidays:\n    6: Birthday of Imam Mahdi\n   29: Nationalization of the Oil Industry\n#+end_example\n\n#+begin_example bash\njcal 7 1402\n#+end_example\n\n#+begin_example\n             1402 Mehr            \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n   1    2    3    4    5    6    7\n   8    9   10   11   12   13   14\n  15   16   17   18   19   20   21\n  22   23   24   25   26   27   28\n  29   30\n\n Holidays:\n    2: Martyrdom of Imam Hassan Askari and Start of Imamate of Imam Mahdi\n   11: Birthday of Prophet Muhammad and Imam Sadiq\n#+end_example\n\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_125617_sazNzJ.png]]\n\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_103928_zRAerD.png]]\n\n** =colorama= Colors\nThese colors are defined by your terminal theme. Use true (24-bit) colors if you want to specify colors in RGB.\n\n#+begin_example\nBLACK\nBLUE\nCYAN\nGREEN\nLIGHTBLACK_EX\nLIGHTBLUE_EX\nLIGHTCYAN_EX\nLIGHTGREEN_EX\nLIGHTMAGENTA_EX\nLIGHTRED_EX\nLIGHTWHITE_EX\nLIGHTYELLOW_EX\nMAGENTA\nRED\nRESET\nWHITE\nYELLOW\n#+end_example\n\n* Holiday Data\nThe default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date for the upcoming years, but you can always supply your own.\n\nThe holiday data of previous years (≤1401) has not been added.\n\n',
+    'long_description': "#+TITLE: jalali-calendar-cli\n\nJalali (Shamsi) calendar in your terminal, with holidays\n\n* Install\n#+begin_example bash\npip install -U jalali-calendar-cli\n#+end_example\n\nThis requires Python ≥3.10.\n\n* Usage\n# #+ATTR_HTML: :width 884\n# [[file:readme.org_imgs/20230524_003016_h5V1Xf.png]]\n#+ATTR_HTML: :width 914\n[[file:readme.org_imgs/20230606_125421_Bh79HZ.png]]\n\n#+ATTR_HTML: :width 900\n[[file:readme.org_imgs/20230606_125356_jLt2Jh.png]]\n\n\n#+begin_example bash\nusage: jalali-calendar [-h] [--color {auto,always,never}]\n                       [--true-color | --no-true-color]\n                       [--footnotes | --no-footnotes]\n                       [--indentation INDENTATION]\n                       [--holidays-json-path HOLIDAYS_JSON_PATH]\n                       [--color-preset {light,dark}]\n                       [--weekend-true-color WEEKEND_TRUE_COLOR]\n                       [--holiday-true-color HOLIDAY_TRUE_COLOR]\n                       [--header-true-color HEADER_TRUE_COLOR]\n                       [--weekend-color WEEKEND_COLOR]\n                       [--holiday-color HOLIDAY_COLOR]\n                       [--header-color HEADER_COLOR]\n                       [month] [year]\n\npositional arguments:\n  month                 month in Jalali calendar (default: current month)\n  year                  year in Jalali calendar (default: current year)\n\noptions:\n  -h, --help            show this help message and exit\n  --color {auto,always,never}\n                        colorize the output\n  --true-color, --no-true-color\n                        enable true color support for output (default: False)\n  --footnotes, --no-footnotes\n                        show footnotes in the output (default: True)\n  --indentation INDENTATION\n                        number of spaces for indentation (default: 5)\n  --holidays-json-path HOLIDAYS_JSON_PATH\n                        path to JSON file containing holiday data\n  --color-preset {light,dark}\n                        color preset for the calendar output (default: light)\n\n24-bit true color options:\n  --weekend-true-color WEEKEND_TRUE_COLOR\n                        RGB values for weekend color in 24-bit true color\n  --holiday-true-color HOLIDAY_TRUE_COLOR\n                        RGB values for holiday color in 24-bit true color\n  --header-true-color HEADER_TRUE_COLOR\n                        RGB values for header color in 24-bit true color\n\ncolorama 256 color options:\n  --weekend-color WEEKEND_COLOR\n                        colorama color name for weekend color\n  --holiday-color HOLIDAY_COLOR\n                        colorama color name for holiday color\n  --header-color HEADER_COLOR\n                        colorama color name for header color\n#+end_example\n\n** Examples\n#+begin_example bash\njcal 12\n#+end_example\n\n#+begin_example\n            1402 Esfand           \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n                  1    2    3    4\n   5    6    7    8    9   10   11\n  12   13   14   15   16   17   18\n  19   20   21   22   23   24   25\n  26   27   28   29\n\n Holidays:\n    6: Birthday of Imam Mahdi\n   29: Nationalization of the Oil Industry\n#+end_example\n\n#+begin_example bash\njcal 7 1402\n#+end_example\n\n#+begin_example\n             1402 Mehr            \n Sat  Sun  Mon  Tue  Wed  Thu  Fri\n   1    2    3    4    5    6    7\n   8    9   10   11   12   13   14\n  15   16   17   18   19   20   21\n  22   23   24   25   26   27   28\n  29   30\n\n Holidays:\n    2: Martyrdom of Imam Hassan Askari and Start of Imamate of Imam Mahdi\n   11: Birthday of Prophet Muhammad and Imam Sadiq\n#+end_example\n\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_125617_sazNzJ.png]]\n\n#+ATTR_HTML: :width 968\n[[file:readme.org_imgs/20230606_103928_zRAerD.png]]\n\n*** Shell Aliases in Bash\nYou can add aliases to =~/.bashrc= and =~/.bash_profile= to persist your settings:\n\n#+begin_example bash\nalias jcal='command jcal --color-preset dark'\n#+end_example\n\nAliases work the same way in Zsh, you just need to add them to =~/.zshenv=.\n\n** =colorama= Colors\nThese colors are defined by your terminal theme. Use true (24-bit) colors if you want to specify colors in RGB.\n\n#+begin_example\nBLACK\nBLUE\nCYAN\nGREEN\nLIGHTBLACK_EX\nLIGHTBLUE_EX\nLIGHTCYAN_EX\nLIGHTGREEN_EX\nLIGHTMAGENTA_EX\nLIGHTRED_EX\nLIGHTWHITE_EX\nLIGHTYELLOW_EX\nMAGENTA\nRED\nRESET\nWHITE\nYELLOW\n#+end_example\n\n* Holiday Data\nThe default data dictionary is [[https://github.com/NightMachinery/jalali-calendar-cli/blob/master/jalali_calendar_cli/holidays.json][here]]. I plan to keep the data up-to-date for the upcoming years, but you can always supply your own.\n\nThe holiday data of previous years (≤1401) has not been added.\n\n",
     'author': 'NightMachinery',
     'author_email': 'feraidoonmehri@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jalali_calendar_cli-0.1.4/PKG-INFO` & `jalali_calendar_cli-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jalali-calendar-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Jalali (Shamsi) calendar in your terminal, with holidays
 Author: NightMachinery
 Author-email: feraidoonmehri@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,15 +35,15 @@
 
 #+begin_example bash
 usage: jalali-calendar [-h] [--color {auto,always,never}]
                        [--true-color | --no-true-color]
                        [--footnotes | --no-footnotes]
                        [--indentation INDENTATION]
                        [--holidays-json-path HOLIDAYS_JSON_PATH]
-                       [--color-preset COLOR_PRESET]
+                       [--color-preset {light,dark}]
                        [--weekend-true-color WEEKEND_TRUE_COLOR]
                        [--holiday-true-color HOLIDAY_TRUE_COLOR]
                        [--header-true-color HEADER_TRUE_COLOR]
                        [--weekend-color WEEKEND_COLOR]
                        [--holiday-color HOLIDAY_COLOR]
                        [--header-color HEADER_COLOR]
                        [month] [year]
@@ -60,15 +60,15 @@
                         enable true color support for output (default: False)
   --footnotes, --no-footnotes
                         show footnotes in the output (default: True)
   --indentation INDENTATION
                         number of spaces for indentation (default: 5)
   --holidays-json-path HOLIDAYS_JSON_PATH
                         path to JSON file containing holiday data
-  --color-preset COLOR_PRESET
+  --color-preset {light,dark}
                         color preset for the calendar output (default: light)
 
 24-bit true color options:
   --weekend-true-color WEEKEND_TRUE_COLOR
                         RGB values for weekend color in 24-bit true color
   --holiday-true-color HOLIDAY_TRUE_COLOR
                         RGB values for holiday color in 24-bit true color
@@ -123,14 +123,23 @@
 
 #+ATTR_HTML: :width 968
 [[file:readme.org_imgs/20230606_125617_sazNzJ.png]]
 
 #+ATTR_HTML: :width 968
 [[file:readme.org_imgs/20230606_103928_zRAerD.png]]
 
+*** Shell Aliases in Bash
+You can add aliases to =~/.bashrc= and =~/.bash_profile= to persist your settings:
+
+#+begin_example bash
+alias jcal='command jcal --color-preset dark'
+#+end_example
+
+Aliases work the same way in Zsh, you just need to add them to =~/.zshenv=.
+
 ** =colorama= Colors
 These colors are defined by your terminal theme. Use true (24-bit) colors if you want to specify colors in RGB.
 
 #+begin_example
 BLACK
 BLUE
 CYAN
```

