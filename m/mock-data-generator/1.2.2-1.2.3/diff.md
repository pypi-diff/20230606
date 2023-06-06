# Comparing `tmp/mock_data_generator-1.2.2.tar.gz` & `tmp/mock_data_generator-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.2.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.3.tar", max compression
```

## Comparing `mock_data_generator-1.2.2.tar` & `mock_data_generator-1.2.3.tar`

### file list

```diff
@@ -1,5 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.2/LICENSE
--rw-r--r--   0        0        0     2414 2023-06-05 13:18:09.875340 mock_data_generator-1.2.2/README.md
--rw-r--r--   0        0        0     1411 2023-06-05 12:29:43.508935 mock_data_generator-1.2.2/mock_data_generator/driver.py
--rw-r--r--   0        0        0      922 2023-06-05 13:37:14.890403 mock_data_generator-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 mock_data_generator-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-06 03:18:43.414782 mock_data_generator-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2414 2023-06-06 03:18:43.415217 mock_data_generator-1.2.3/README.md
+-rw-r--r--   0        0        0     1451 2023-06-06 04:11:00.162686 mock_data_generator-1.2.3/mock_data_generator/driver.py
+-rw-r--r--   0        0        0     2519 2023-06-06 03:18:43.415652 mock_data_generator-1.2.3/mock_data_generator/generator/generate.py
+-rw-r--r--   0        0        0       81 2023-06-06 03:18:43.417351 mock_data_generator-1.2.3/mock_data_generator/resources/config.ini
+-rw-r--r--   0        0        0      348 2023-06-06 03:18:43.417642 mock_data_generator-1.2.3/mock_data_generator/resources/schema.json
+-rw-r--r--   0        0        0     1085 2023-06-06 04:10:02.967992 mock_data_generator-1.2.3/mock_data_generator/schema_handler/schema_validator.py
+-rw-r--r--   0        0        0      626 2023-06-06 04:06:31.813648 mock_data_generator-1.2.3/mock_data_generator/tests/fileutils_test.py
+-rw-r--r--   0        0        0      735 2023-06-06 04:04:13.106286 mock_data_generator-1.2.3/mock_data_generator/tests/schema_validator_test.py
+-rw-r--r--   0        0        0      133 2023-06-06 03:18:43.419384 mock_data_generator-1.2.3/mock_data_generator/tests/test.json
+-rw-r--r--   0        0        0      152 2023-06-06 03:18:43.419675 mock_data_generator-1.2.3/mock_data_generator/utils/constants.py
+-rw-r--r--   0        0        0     2088 2023-06-06 04:11:30.163451 mock_data_generator-1.2.3/mock_data_generator/utils/fileutils.py
+-rw-r--r--   0        0        0      947 2023-06-06 04:19:55.261251 mock_data_generator-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 mock_data_generator-1.2.3/PKG-INFO
```

### Comparing `mock_data_generator-1.2.2/LICENSE` & `mock_data_generator-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.2/README.md` & `mock_data_generator-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.2/mock_data_generator/driver.py` & `mock_data_generator-1.2.3/mock_data_generator/driver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
-from utils.constants import FILE_FORMATS
-from utils.fileutils import proceed
+from mock_data_generator.utils.constants import FILE_FORMATS
+from mock_data_generator.utils.fileutils import proceed
 
 
 def validate_file_format(value):
     if value.upper() not in FILE_FORMATS:
         raise argparse.ArgumentTypeError(
             f"Unsupported output file format {value} detected. Supported file formats are {FILE_FORMATS}"
         )
```

### Comparing `mock_data_generator-1.2.2/pyproject.toml` & `mock_data_generator-1.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.2"
+version = "1.2.3"
 description = "Generate mock data using json schema supplied."
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
 
 [tool.poetry.dependencies]
-python = "~3.11.3"
+python = "^3.10"
 faker = "^18.9.0"
 jsonschema = "^4.17.3"
 lxml = "^4.9.2"
 openpyxl = "^3.1.2"
 pandas = "^2.0.2"
 tqdm = "^4.65.0"
 pyarrow = "^12.0.0"
@@ -23,21 +23,22 @@
 [tool.poetry.dev-dependencies]
 bumpver = "^2022.1119"
 coverage = "^6.5.0"
 pytest = "^7.3.1"
 
 [tool.pytest.ini_options]
 pythonpath = [
-  "."
+  ".",
+  "./mock_data_generator"
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "1.2.2"
+current_version = "1.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.2.2/PKG-INFO` & `mock_data_generator-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.2
+Version: 1.2.3
 Summary: Generate mock data using json schema supplied.
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
-Requires-Python: >=3.11.3,<3.12.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=18.9.0,<19.0.0)
 Requires-Dist: fastparquet (>=2023.4.0,<2024.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
```

