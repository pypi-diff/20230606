# Comparing `tmp/novem-0.4.6.tar.gz` & `tmp/novem-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novem-0.4.6.tar", max compression
+gzip compressed data, was "novem-0.4.7.tar", max compression
```

## Comparing `novem-0.4.6.tar` & `novem-0.4.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1194 2022-04-03 20:39:39.813737 novem-0.4.6/LICENSE
--rw-r--r--   0        0        0     3976 2022-04-03 20:39:39.814271 novem-0.4.6/README.md
--rw-r--r--   0        0        0      130 2023-04-20 13:43:13.511872 novem-0.4.6/novem/__init__.py
--rw-r--r--   0        0        0      152 2023-04-20 13:43:13.512282 novem-0.4.6/novem/__main__.py
--rw-r--r--   0        0        0     5520 2023-04-20 13:43:13.515626 novem-0.4.6/novem/api_ref.py
--rw-r--r--   0        0        0      252 2023-04-20 13:43:13.516040 novem-0.4.6/novem/applicator.py
--rw-r--r--   0        0        0    12405 2023-04-20 13:43:13.524293 novem-0.4.6/novem/cli/__init__.py
--rw-r--r--   0        0        0     3269 2023-04-20 13:43:13.516704 novem-0.4.6/novem/cli/config.py
--rw-r--r--   0        0        0     2661 2023-04-20 13:43:13.516400 novem-0.4.6/novem/cli/editor.py
--rw-r--r--   0        0        0     8148 2023-04-20 13:43:13.522685 novem-0.4.6/novem/cli/group.py
--rw-r--r--   0        0        0     3213 2023-04-20 13:43:13.523043 novem-0.4.6/novem/cli/invite.py
--rw-r--r--   0        0        0     5812 2023-04-20 13:43:13.517287 novem-0.4.6/novem/cli/mail.py
--rw-r--r--   0        0        0     5556 2023-04-20 13:43:13.517832 novem-0.4.6/novem/cli/plot.py
--rw-r--r--   0        0        0    11982 2023-04-20 13:43:13.523470 novem-0.4.6/novem/cli/setup.py
--rw-r--r--   0        0        0     5309 2023-04-20 13:43:13.523855 novem-0.4.6/novem/cli/vis.py
--rw-r--r--   0        0        0      109 2023-04-20 13:43:13.524723 novem-0.4.6/novem/colors/__init__.py
--rw-r--r--   0        0        0     2033 2023-04-20 13:43:13.525078 novem-0.4.6/novem/colors/colors.py
--rw-r--r--   0        0        0      133 2023-04-20 13:43:13.527691 novem-0.4.6/novem/exceptions/__init__.py
--rw-r--r--   0        0        0      382 2023-04-20 13:43:13.530285 novem-0.4.6/novem/mail.py
--rw-r--r--   0        0        0       66 2023-04-20 13:43:13.530715 novem-0.4.6/novem/table/__init__.py
--rw-r--r--   0        0        0     6022 2023-04-20 13:43:13.532077 novem-0.4.6/novem/table/selector.py
--rw-r--r--   0        0        0     8940 2023-04-20 13:43:13.532517 novem-0.4.6/novem/utils.py
--rw-r--r--   0        0        0       22 2023-04-20 13:43:13.532866 novem-0.4.6/novem/version.py
--rw-r--r--   0        0        0    13852 2023-04-20 13:43:13.538362 novem-0.4.6/novem/vis/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-20 13:43:13.533703 novem-0.4.6/novem/vis/cell.py
--rw-r--r--   0        0        0     1406 2023-04-20 13:43:13.534013 novem-0.4.6/novem/vis/colors.py
--rw-r--r--   0        0        0      915 2023-04-20 13:43:13.535107 novem-0.4.6/novem/vis/files.py
--rw-r--r--   0        0        0     9117 2023-04-20 13:43:13.538660 novem-0.4.6/novem/vis/mail.py
--rw-r--r--   0        0        0    16106 2023-04-20 13:43:13.534300 novem-0.4.6/novem/vis/mail_sections.py
--rw-r--r--   0        0        0     7237 2023-04-20 13:43:13.539041 novem-0.4.6/novem/vis/plot.py
--rw-r--r--   0        0        0     1487 2023-04-20 13:43:13.534589 novem-0.4.6/novem/vis/plot_config.py
--rw-r--r--   0        0        0     1468 2023-04-20 13:43:13.534847 novem-0.4.6/novem/vis/shared.py
--rw-r--r--   0        0        0     1507 2023-04-20 13:43:05.274390 novem-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     5065 2023-04-20 13:44:22.708201 novem-0.4.6/setup.py
--rw-r--r--   0        0        0     4773 2023-04-20 13:44:22.709103 novem-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1194 2022-04-03 20:39:39.813737 novem-0.4.7/LICENSE
+-rw-r--r--   0        0        0     3976 2022-04-03 20:39:39.814271 novem-0.4.7/README.md
+-rw-r--r--   0        0        0      130 2023-06-06 19:59:28.430024 novem-0.4.7/novem/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-06 19:59:28.430722 novem-0.4.7/novem/__main__.py
+-rw-r--r--   0        0        0     5520 2023-06-06 19:59:28.438765 novem-0.4.7/novem/api_ref.py
+-rw-r--r--   0        0        0      252 2023-06-06 19:59:28.439358 novem-0.4.7/novem/applicator.py
+-rw-r--r--   0        0        0    12405 2023-06-06 19:59:28.451533 novem-0.4.7/novem/cli/__init__.py
+-rw-r--r--   0        0        0     3269 2023-06-06 19:59:28.440431 novem-0.4.7/novem/cli/config.py
+-rw-r--r--   0        0        0     2661 2023-06-06 19:59:28.439887 novem-0.4.7/novem/cli/editor.py
+-rw-r--r--   0        0        0     8148 2023-06-06 19:59:28.448531 novem-0.4.7/novem/cli/group.py
+-rw-r--r--   0        0        0     3213 2023-06-06 19:59:28.449052 novem-0.4.7/novem/cli/invite.py
+-rw-r--r--   0        0        0     5812 2023-06-06 19:59:28.441322 novem-0.4.7/novem/cli/mail.py
+-rw-r--r--   0        0        0     5556 2023-06-06 19:59:28.441947 novem-0.4.7/novem/cli/plot.py
+-rw-r--r--   0        0        0    11982 2023-06-06 19:59:28.450198 novem-0.4.7/novem/cli/setup.py
+-rw-r--r--   0        0        0     5309 2023-06-06 19:59:28.450814 novem-0.4.7/novem/cli/vis.py
+-rw-r--r--   0        0        0      109 2023-06-06 19:59:28.452160 novem-0.4.7/novem/colors/__init__.py
+-rw-r--r--   0        0        0     2033 2023-06-06 19:59:28.452749 novem-0.4.7/novem/colors/colors.py
+-rw-r--r--   0        0        0      133 2023-06-06 19:59:28.454650 novem-0.4.7/novem/exceptions/__init__.py
+-rw-r--r--   0        0        0      382 2023-06-06 19:59:28.455966 novem-0.4.7/novem/mail.py
+-rw-r--r--   0        0        0       66 2023-06-06 19:59:28.456575 novem-0.4.7/novem/table/__init__.py
+-rw-r--r--   0        0        0     7075 2023-06-06 19:59:28.458135 novem-0.4.7/novem/table/selector.py
+-rw-r--r--   0        0        0     8940 2023-06-06 19:59:28.458760 novem-0.4.7/novem/utils.py
+-rw-r--r--   0        0        0       22 2023-06-06 19:59:28.459020 novem-0.4.7/novem/version.py
+-rw-r--r--   0        0        0    13852 2023-06-06 19:59:28.468238 novem-0.4.7/novem/vis/__init__.py
+-rw-r--r--   0        0        0     3398 2023-06-06 19:59:28.459885 novem-0.4.7/novem/vis/cell.py
+-rw-r--r--   0        0        0     1406 2023-06-06 19:59:28.460399 novem-0.4.7/novem/vis/colors.py
+-rw-r--r--   0        0        0      915 2023-06-06 19:59:28.462529 novem-0.4.7/novem/vis/files.py
+-rw-r--r--   0        0        0     9117 2023-06-06 19:59:28.468830 novem-0.4.7/novem/vis/mail.py
+-rw-r--r--   0        0        0    16106 2023-06-06 19:59:28.460991 novem-0.4.7/novem/vis/mail_sections.py
+-rw-r--r--   0        0        0     7237 2023-06-06 19:59:28.469373 novem-0.4.7/novem/vis/plot.py
+-rw-r--r--   0        0        0     1487 2023-06-06 19:59:28.461554 novem-0.4.7/novem/vis/plot_config.py
+-rw-r--r--   0        0        0     1468 2023-06-06 19:59:28.462068 novem-0.4.7/novem/vis/shared.py
+-rw-r--r--   0        0        0     1507 2023-06-06 19:59:37.804128 novem-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     5065 2023-06-06 20:04:17.716713 novem-0.4.7/setup.py
+-rw-r--r--   0        0        0     4773 2023-06-06 20:04:17.717252 novem-0.4.7/PKG-INFO
```

### Comparing `novem-0.4.6/LICENSE` & `novem-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/README.md` & `novem-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/api_ref.py` & `novem-0.4.7/novem/api_ref.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/__init__.py` & `novem-0.4.7/novem/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/config.py` & `novem-0.4.7/novem/cli/config.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/editor.py` & `novem-0.4.7/novem/cli/editor.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/group.py` & `novem-0.4.7/novem/cli/group.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/invite.py` & `novem-0.4.7/novem/cli/invite.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/mail.py` & `novem-0.4.7/novem/cli/mail.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/plot.py` & `novem-0.4.7/novem/cli/plot.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/setup.py` & `novem-0.4.7/novem/cli/setup.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/cli/vis.py` & `novem-0.4.7/novem/cli/vis.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/colors/colors.py` & `novem-0.4.7/novem/colors/colors.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/table/selector.py` & `novem-0.4.7/novem/table/selector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 import numpy as np
 import pandas as pd
 
 from novem.exceptions import NovemException
 
 
@@ -10,14 +10,27 @@
     def __init__(self, message: str):
 
         message = f"Invalid selector format {message}."
 
         super().__init__(message)
 
 
+def enhance_positions(positions: List[int], ior: int) -> List[int]:
+    if not positions or not isinstance(ior, int):
+        return positions
+    if ior == 0:
+        return positions
+    elif ior < 0:
+        return list(range(min(positions) + ior, min(positions))) + positions
+    else:  # ior > 0
+        return positions + list(
+            range(max(positions) + 1, max(positions) + 1 + ior)
+        )
+
+
 class Selector(object):
     """
     The novem Selector is a convenience function for carving out parts of a
     dataframe for styling
 
     The purpose of a novem selector is to supply it with a sliced dataframe
     along with the original and the selector will figure out the correct novem
@@ -50,26 +63,30 @@
         selector: Any,
         applicator: Any,
         r: Any = None,
         c: Optional[str] = None,
         i: Optional[str] = None,
         co: Optional[int] = None,
         io: Optional[int] = None,
+        cor: Optional[int] = None,
+        ior: Optional[int] = None,
     ) -> None:
         """ """
 
         # TODO: verify that it's a valid novem selector before
         # storing it and throw an error if not
         self.selector = selector
         self.applicator = applicator
         self.ref = r
         self.c = c
         self.i = i
         self.co = co
         self.io = io
+        self.cor = cor
+        self.ior = ior
 
     def _pd_ix_lookup(self) -> str:
 
         filter = self.selector
         frame = self.ref
 
         if frame is None:
@@ -91,14 +108,21 @@
         co = 0
         io = 0
         if self.co:
             co = self.co
         if self.io:
             io = self.io
 
+        cor = 0
+        ior = 0
+        if self.cor:
+            cor = self.cor
+        if self.ior:
+            ior = self.ior
+
         # Check if the filter is a DataFrame or a Series
         if isinstance(filter, pd.DataFrame):
             row_indices = filter.index
             col_indices = filter.columns
             cl = filter.columns.nlevels
         else:
             row_indices = filter.index
@@ -109,14 +133,18 @@
             # on our original frame to be sure, this is not perfect
             # as if all the values are in both the columns and index we
             # have to just guess
             if all(value in frame.columns for value in row_indices):
                 row_indices = pd.Index([filter.name])
                 col_indices = filter.index
 
+        # TODO: We need to check against values in the frame for our
+        # filtered dataset, else we are still failing to account for
+        # duplicate values outside of filter
+
         # Find the row and column positions in the original dataframe
         row_positions = []
         used_positions = set()
         for row_label in row_indices:
             position = frame.index.get_loc(row_label)
             if isinstance(position, np.ndarray):
                 position = np.flatnonzero(position)
@@ -144,18 +172,24 @@
             else:
                 if position not in used_col_positions:
                     used_col_positions.add(position)
                     col_positions.append(position)
 
         # convert to novem 0 based index and drop negative offset results
         row_positions = [x + rl + io for x in row_positions if x < len(frame)]
-        row_positions = [x for x in row_positions if x >= 0]
+        row_positions = enhance_positions(row_positions, ior)
+        row_positions = [
+            x for x in row_positions if x >= 0 and x <= len(frame)
+        ]
 
         col_positions = [x + cl + co for x in col_positions if x < len(frame)]
-        col_positions = [x for x in col_positions if x >= 0]
+        col_positions = enhance_positions(col_positions, cor)
+        col_positions = [
+            x for x in col_positions if x >= 0 and x <= len(frame)
+        ]
 
         # Create a comma-separated list of row and column positions
         row_str = ",".join(map(str, row_positions))
         col_str = ",".join(map(str, col_positions))
 
         if self.i:
             row_str = self.i
```

### Comparing `novem-0.4.6/novem/utils.py` & `novem-0.4.7/novem/utils.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/__init__.py` & `novem-0.4.7/novem/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/cell.py` & `novem-0.4.7/novem/vis/cell.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/colors.py` & `novem-0.4.7/novem/vis/colors.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/files.py` & `novem-0.4.7/novem/vis/files.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/mail.py` & `novem-0.4.7/novem/vis/mail.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/mail_sections.py` & `novem-0.4.7/novem/vis/mail_sections.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/plot.py` & `novem-0.4.7/novem/vis/plot.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/plot_config.py` & `novem-0.4.7/novem/vis/plot_config.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/novem/vis/shared.py` & `novem-0.4.7/novem/vis/shared.py`

 * *Files identical despite different names*

### Comparing `novem-0.4.6/pyproject.toml` & `novem-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "novem"
-version = "0.4.6"
+version = "0.4.7"
 description = "python library for the novem.no data visualisation platform"
 authors = ["Sondov Engen <sondov@novem.no>"]
 homepage = "https://novem.no"
 repository = "https://github.com/novem-no/novem"
 readme = "README.md"
 license = "MIT"
```

### Comparing `novem-0.4.6/setup.py` & `novem-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'urllib3>=1.26.15,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['novem = novem.cli:run_cli']}
 
 setup_kwargs = {
     'name': 'novem',
-    'version': '0.4.6',
+    'version': '0.4.7',
     'description': 'python library for the novem.no data visualisation platform',
     'long_description': '\n# novem - data visualisation for coders\n\nA wrapper library for the novem.no data visualisation platform. Create charts,\ndocuments e-mails and dashboards through one simple api.\n\n**NB:** novem is currently in closed alpha, if you want to try it out please\nreach out to hello@novem.no\n\n\n## Exampels\n\nCreate a linechart from a dataframe using pandas data reader\n\n```python\nfrom pandas_datareader import data\nfrom novem import Plot\n\nline = Plot("aapl_price_hist", type="line", name="Apple price history")\n\n# Only get the adjusted close.\naapl = data.DataReader("AAPL",\n                       start="2015-1-1",\n                       end="2021-12-31",\n                       data_source="yahoo")["Adj Close"]\n\n# send data to the plot\naapl.pipe(line)\n\n# url to view plot\nprint(line.url)\n```\n\n\n## Getting started\nTo get started with novem you\'ll have to register an account, currently this\ncan be done by reaching out to the novem developers on hello@novem.no.\n\nOnce you have a username and password you can setup your environment using:\n```bash\n  python -m novem --init\n```\n\nIn additon to invoking the novem module as shown above, the novem package also\nincludes an extensive command-line interface (cli). Check out CLI.md in this\nrepostiory or [novem.no](https://novem.no) for more details.\n\n\n\n## Creating a plot\nNovem represents plots as a Plot class that can be imported from the main novem\npackage `from novem import Plot`.\n\nThe plot class takes a single mandatory positional argument, the name of the\nplot.\n * If the plot name is new, the instantiation of the class will create the plot.\n * If the plot name already exist, then the new object will operate on the\n   existing plot.\n\nIn addition to the name, there are two broad categories of options for a\nplot, data and config:\n * The **data** contains the actual information to visualise (usually in the form\n   of numeric csv)\n * **Config**, which contains information about the visual such as:\n   * Type (bar, line, donut, map etc)\n   * Titles/captions/names/colors/legends/axis etc\n\n\nThere are two ways to interact with the plots, one can either supply all\nthe neccessary options as named arguments when creating the plot, or use the\nproperty accessors to modfity them one by one (this is more helpful when working\nwith the plot in an interactive way). Below is an example of the two\napproaches.\n\n```python\nfrom novem import Plot\n\n# everything in the constructor\nbarchart = Plot(<name>, \\\n  type="bar", \\\n  title="barchart title", \\\n  caption = "caption"\n)\n\n# property approach\nbarchart = Plot("plot_name")\nbarchart.type = "bar"\nbarchart.title = "barchart title"\nbarchart.caption = "caption"\n```\n\nIn addition to setting individual properties, the plot object is also callable.\nThis means that the resulting plot can be used as a function, either by being\nprovided data as an argument, or used as part of a pipe chain.\n\n```python\nfrom novem import Plot\nimport pandas as pd\nimport numpy as np\n\n# construct some random sample data\ndf = pd.DataFrame(np.random.randn(100, 4), columns=list("ABCD")).cumsum()\n\nline = Plot("new_line", type="line")\n\n# alternative one, setting data explicitly to a csv string\nline.data = df.to_csv()\n\n# or let the plot invoke the to_csv\nline.data = df\n\n# alternative two, calling Plot with a csv string\nline(df.to_csv())\n\n# alternative three calling the Plot with an object that has a to_csv function\nline(df)\n\n# or\ndf.pipe(line)\n\n```\n\n\n**NB:** All novem plot operations are live.\nThis means that as soon as you write to or modify any aspects of the plot\nobject, those changes are reflected on the novem server and anyone watching\nthe plot in real time.\n\n\n\n## Contribution and development\nThe novem python library and platform is under active development, contributions\nor issues are most welcome.\n\nFor guidelines on how to contribute, please check out the CONTRIBUTING.md file\nin this repository.\n\n\n## LICENSE\nThis python library is licensed under the MIT license, see the LICENSE file for\ndetails\n',
     'author': 'Sondov Engen',
     'author_email': 'sondov@novem.no',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://novem.no',
```

### Comparing `novem-0.4.6/PKG-INFO` & `novem-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novem
-Version: 0.4.6
+Version: 0.4.7
 Summary: python library for the novem.no data visualisation platform
 Home-page: https://novem.no
 License: MIT
 Author: Sondov Engen
 Author-email: sondov@novem.no
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

