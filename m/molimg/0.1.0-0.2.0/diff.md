# Comparing `tmp/molimg-0.1.0.tar.gz` & `tmp/molimg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molimg-0.1.0.tar", max compression
+gzip compressed data, was "molimg-0.2.0.tar", max compression
```

## Comparing `molimg-0.1.0.tar` & `molimg-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1957 2023-02-14 19:57:54.639670 molimg-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-02-14 17:48:39.859951 molimg-0.1.0/molimg/__init__.py
--rw-r--r--   0        0        0     2427 2023-02-14 19:06:12.304783 molimg-0.1.0/molimg/draw.py
--rw-r--r--   0        0        0     2389 2023-02-14 19:06:12.308398 molimg-0.1.0/molimg/excel.py
--rw-r--r--   0        0        0      112 2023-02-14 19:06:12.284041 molimg-0.1.0/molimg/helpers.py
--rw-r--r--   0        0        0      479 2023-02-14 19:43:00.129371 molimg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 molimg-0.1.0/setup.py
--rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 molimg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-01 18:06:51.188603 molimg-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1957 2023-06-06 17:28:35.843792 molimg-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-14 17:48:39.859951 molimg-0.2.0/molimg/__init__.py
+-rw-r--r--   0        0        0     2478 2023-06-01 17:46:43.554413 molimg-0.2.0/molimg/draw.py
+-rw-r--r--   0        0        0     2878 2023-06-01 17:49:05.307781 molimg-0.2.0/molimg/excel.py
+-rw-r--r--   0        0        0      112 2023-02-14 19:06:12.284041 molimg-0.2.0/molimg/helpers.py
+-rw-r--r--   0        0        0      479 2023-06-06 17:28:38.332148 molimg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 molimg-0.2.0/PKG-INFO
```

### Comparing `molimg-0.1.0/README.md` & `molimg-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Molecular Imager
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/jdkern11/molimg/workflows/tests/badge.svg)](https://github.com/jdkern11/molimg/actions?workflow=tests)
 [![codecov](https://codecov.io/gh/jdkern11/molimg/branch/main/graph/badge.svg?token=4MU1H8MD94)](https://codecov.io/gh/jdkern11/molimg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![version](https://img.shields.io/badge/Release-0.1.0-blue)](https://github.com/jdkern11/molimg/releases)
+[![version](https://img.shields.io/badge/Release-0.2.0-blue)](https://github.com/jdkern11/molimg/releases)
 
 Do you ever wish you could easily embed the images of your smiles strings into 
 an excel sheet? Wish no more! molimg is here to do just that!
 
 Take the following data in a csv:
 
 ![image of example data](https://raw.githubusercontent.com/jdkern11/molimg/main/images/example_csv.png)
```

### Comparing `molimg-0.1.0/molimg/draw.py` & `molimg-0.2.0/molimg/draw.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     if column not in df.columns:
         raise KeyError(f"{column} not in the dataframe")
     save_folder = Path(remove_extensions(save_folder))
     save_folder.mkdir(exist_ok=True)
     for index, row in df.iterrows():
         try:
             if not pd.isna(row[column]):
-                smiles_to_png(row[column], f"{str(save_folder / row[column])}.png")
+                image_column = column + "_image"
+                smiles_to_png(row[column], f"{str(save_folder / row[image_column])}")
         # To get Boost.Python.ArgumentError. This is a C++ error and can only
         # be caught with Excpetion
         except Exception as e:
             logger.warning(f"For {row[column]}, {e}")
             continue
```

### Comparing `molimg-0.1.0/molimg/excel.py` & `molimg-0.2.0/molimg/excel.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,39 +30,53 @@
     """
     logger.debug(f"Converting smiles in {smiles_columns} to images")
     filename = remove_extensions(filename)
     folder_name = str(uuid.uuid4())
     # make sure folder doesn't already exist
     while Path(folder_name).exists():
         folder_name = str(uuid.uuid4())
+    
+    # record columns before more added
+    columns = df.columns
+    # add uuid for each smiles column so names are unique and not invalid
+    for col in smiles_columns:
+        data = set()
+        for index, row in df.iterrows():
+            name = uuid.uuid4()
+            while name in data:
+                name = uuid.uuid4()
+            data.add(str(name))
+        df[f"{col}_image"] = list(data)
 
     df_columns_of_smiles_to_pngs(df, smiles_columns, folder_name)
 
     workbook = xlsxwriter.Workbook(f"{filename}.xlsx")
     worksheet = workbook.add_worksheet()
 
     r, c = 0, 0
-    for column in df.columns:
+    # use previously recorded columns
+    for column in columns:
         worksheet.write(r, c, column)
         for index, row in df.iterrows():
             r += 1
             if pd.isna(row[column]):
                 worksheet.write_blank(r, c, None)
             else:
                 worksheet.write(r, c, row[column])
 
         # image column should come next if column is in smiles column
         if column in smiles_columns:
             r = 0
             c += 1
-            worksheet.write(r, c, f"{column}_image")
+            image_column = f"{column}_image"
+            worksheet.write(r, c, image_column)
             worksheet.set_column_pixels(c, c, 205)
             for index, row in df.iterrows():
                 r += 1
-                filepath = Path(folder_name) / column / f"{row[column]}.png"
+                filepath = Path(folder_name) / column / f"{row[image_column]}.png"
                 if filepath.exists():
                     worksheet.insert_image(
                         r, c, str(filepath), {"x_offset": 2.5, "y_offset": 2.5}
                     )
                     worksheet.set_row_pixels(r, 205)
         c += 1
         r = 0
```

### Comparing `molimg-0.1.0/setup.py` & `molimg-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,61 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: molimg
+Version: 0.2.0
+Summary: 
+Home-page: https://github.com/jdkern11/molimg.git
+Author: jdkern11
+Author-email: josephdanielkern@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: rdkit (>=2022.9.4,<2023.0.0)
+Requires-Dist: xlsxwriter (>=3.0.8,<4.0.0)
+Project-URL: Repository, https://github.com/jdkern11/molimg.git
+Description-Content-Type: text/markdown
+
+# Molecular Imager
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Tests](https://github.com/jdkern11/molimg/workflows/tests/badge.svg)](https://github.com/jdkern11/molimg/actions?workflow=tests)
+[![codecov](https://codecov.io/gh/jdkern11/molimg/branch/main/graph/badge.svg?token=4MU1H8MD94)](https://codecov.io/gh/jdkern11/molimg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![version](https://img.shields.io/badge/Release-0.2.0-blue)](https://github.com/jdkern11/molimg/releases)
+
+Do you ever wish you could easily embed the images of your smiles strings into 
+an excel sheet? Wish no more! molimg is here to do just that!
+
+Take the following data in a csv:
+
+![image of example data](https://raw.githubusercontent.com/jdkern11/molimg/main/images/example_csv.png)
+
+and molimg will convert it like so:
+
+![image of example data](https://raw.githubusercontent.com/jdkern11/molimg/main/images/example_csv_with_images.png)
+
+## Usage
+First, import the data into a pandas dataframe, then pass this dataframe, the 
+columns that you want to convert to images, and the save name of the file to the 
+package:
+
+```Python
+import pandas as pd
+from molimg import excel
+
+df = pd.read_csv('example_data.csv')
+smiles_columns = ['smiles1', 'smiles2']
+excel.write(
+    df=df, 
+    smiles_columns=smiles_columns, 
+    filename='example_data_with_images.xlsx'
+)
+```
+
+The order the columns appear in df.columns is how the columns will be saved in
+the new excel sheet. The new smiles columns with images will always appear to the right
+of the data they originate from with `{original_column}_image` as the new column name.
+
+Any error that occurs when trying to convert a smiles string to an image 
+will appear as a warning log message and the image will not be produced. The excel sheet
+will still be created with the smiles strings that work.
 
-packages = \
-['molimg']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pandas>=1.5.3,<2.0.0',
- 'rdkit>=2022.9.4,<2023.0.0',
- 'xlsxwriter>=3.0.8,<4.0.0']
-
-setup_kwargs = {
-    'name': 'molimg',
-    'version': '0.1.0',
-    'description': '',
-    'long_description': "# Molecular Imager\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Tests](https://github.com/jdkern11/molimg/workflows/tests/badge.svg)](https://github.com/jdkern11/molimg/actions?workflow=tests)\n[![codecov](https://codecov.io/gh/jdkern11/molimg/branch/main/graph/badge.svg?token=4MU1H8MD94)](https://codecov.io/gh/jdkern11/molimg)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![version](https://img.shields.io/badge/Release-0.1.0-blue)](https://github.com/jdkern11/molimg/releases)\n\nDo you ever wish you could easily embed the images of your smiles strings into \nan excel sheet? Wish no more! molimg is here to do just that!\n\nTake the following data in a csv:\n\n![image of example data](https://raw.githubusercontent.com/jdkern11/molimg/main/images/example_csv.png)\n\nand molimg will convert it like so:\n\n![image of example data](https://raw.githubusercontent.com/jdkern11/molimg/main/images/example_csv_with_images.png)\n\n## Usage\nFirst, import the data into a pandas dataframe, then pass this dataframe, the \ncolumns that you want to convert to images, and the save name of the file to the \npackage:\n\n```Python\nimport pandas as pd\nfrom molimg import excel\n\ndf = pd.read_csv('example_data.csv')\nsmiles_columns = ['smiles1', 'smiles2']\nexcel.write(\n    df=df, \n    smiles_columns=smiles_columns, \n    filename='example_data_with_images.xlsx'\n)\n```\n\nThe order the columns appear in df.columns is how the columns will be saved in\nthe new excel sheet. The new smiles columns with images will always appear to the right\nof the data they originate from with `{original_column}_image` as the new column name.\n\nAny error that occurs when trying to convert a smiles string to an image \nwill appear as a warning log message and the image will not be produced. The excel sheet\nwill still be created with the smiles strings that work.\n",
-    'author': 'jdkern11',
-    'author_email': 'josephdanielkern@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jdkern11/molimg.git',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

