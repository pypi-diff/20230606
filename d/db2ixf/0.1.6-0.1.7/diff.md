# Comparing `tmp/db2ixf-0.1.6.tar.gz` & `tmp/db2ixf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2ixf-0.1.6.tar", last modified: Mon Jun  5 15:46:36 2023, max compression
+gzip compressed data, was "db2ixf-0.1.7.tar", last modified: Tue Jun  6 21:45:49 2023, max compression
```

## Comparing `db2ixf-0.1.6.tar` & `db2ixf-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:46:36.554874 db2ixf-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-05 15:45:25.000000 db2ixf-0.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-05 15:45:25.000000 db2ixf-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-06-05 15:46:36.554874 db2ixf-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-05 15:45:25.000000 db2ixf-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-05 15:45:25.000000 db2ixf-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:46:36.554874 db2ixf-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 15:45:25.000000 db2ixf-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:46:36.550874 db2ixf-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:46:36.550874 db2ixf-0.1.6/src/db2ixf/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/ixf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-05 15:45:25.000000 db2ixf-0.1.6/src/db2ixf/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:46:36.554874 db2ixf-0.1.6/src/db2ixf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:46:35.000000 db2ixf-0.1.6/src/db2ixf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 15:46:36.000000 db2ixf-0.1.6/src/db2ixf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.596060 db2ixf-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-06 21:44:32.000000 db2ixf-0.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-06-06 21:44:32.000000 db2ixf-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-06 21:45:49.596060 db2ixf-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-06 21:44:32.000000 db2ixf-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-06 21:44:32.000000 db2ixf-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:45:49.596060 db2ixf-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-06 21:44:32.000000 db2ixf-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.592059 db2ixf-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.592059 db2ixf-0.1.7/src/db2ixf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/ixf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-06 21:44:32.000000 db2ixf-0.1.7/src/db2ixf/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:45:49.596060 db2ixf-0.1.7/src/db2ixf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:45:48.000000 db2ixf-0.1.7/src/db2ixf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 21:45:49.000000 db2ixf-0.1.7/src/db2ixf.egg-info/top_level.txt
```

### Comparing `db2ixf-0.1.6/CHANGELOG.md` & `db2ixf-0.1.7/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,30 @@
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the
 changes for the upcoming release may be found
 in [here](https://github.com/ismailhammounou/db2ixf/tree/main/resources/changelog)
 .
 
 <!-- release notes start -->
+
+## [0.1.7](https://github.com/ismailhammounou/db2ixf/tree/0.1.7) - 2023-06-06
+
+
+### Added
+
+- Add support for CLOB data type [db2ixf-16](https://github.com/ismailhammounou/db2ixf/issues/16)
+- Add support for BLOB data type [db2ixf-17](https://github.com/ismailhammounou/db2ixf/issues/17)
+- Add support for binary data type [db2ixf-19](https://github.com/ismailhammounou/db2ixf/issues/19)
+
+
+### Changed
+
+- Improve documentation [db2ixf-18](https://github.com/ismailhammounou/db2ixf/issues/18)
+
+
 ## [0.1.6](https://github.com/ismailhammounou/db2ixf/tree/0.1.6) - 2023-06-05
 
 
 ### Fixed
 
 - Fix bug with parquet_version param default value and pass it to pyarrow parquet writer [db2ixf-15](https://github.com/ismailhammounou/db2ixf/issues/15)
```

### Comparing `db2ixf-0.1.6/LICENSE` & `db2ixf-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.6/PKG-INFO` & `db2ixf-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://pypi.org/project/db2ixf/
 Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
@@ -29,17 +29,17 @@
 # DB2IXF Parser
 
 <div align="center">
   <img src="https://github.com/ismailhammounou/db2ixf/blob/main/resources/images/db2ixf-logo.png?raw=true" alt="Logo" width="300" height="300">
 </div>
 
 DB2IXF parser is an open-source python package that simplifies the parsing and
-processing of IBM eXchange Format (IXF) files. IXF is a file format used by
-IBM's DB2 database system for data import and export operations. This package
-provides a streamlined solution for extracting data from IXF files and
+processing of IBM Integration eXchange Format (IXF) files. IXF is a file format
+used by IBM's DB2 database system for data import and export operations. This
+package provides a streamlined solution for extracting data from IXF files and
 converting it to various formats, including JSON, CSV, and Parquet.
 
 ## Features
 
 - **Parse IXF files**: The package allows you to parse IXF files and extract the
   rows of data stored within them.
 - **Convert to multiple formats**: The parsed data can be easily converted to
@@ -67,14 +67,48 @@
 pip install db2ixf
 ```
 
 ### Usage
 
 Here are some examples of how to use DB2 IXF Parser:
 
+#### CLI
+
+Start with this:
+
+```bash
+db2ixf --help
+```
+
+Result:
+
+```
+ Usage: db2ixf [OPTIONS] COMMAND [ARGS]...
+
+ A command-line tool (CLI) for parsing and converting IXF (IBM DB2 Import/Export 
+ Format) files to various formats such as JSON, CSV, and Parquet. Easily parse 
+ and convert IXF files to meet your data processing needs.
+
++- Options -------------------------------------------------------------------+
+| --version             -v        Show the version of the CLI.                |
+| --install-completion            Install completion for the current shell.   |
+| --show-completion               Show completion for the current shell, to   |
+|                                 copy it or customize the installation.      |
+| --help                          Show this message and exit.                 |
++-----------------------------------------------------------------------------+
++- Commands ------------------------------------------------------------------+
+| csv      Parse ixf FILE and convert it to a csv OUTPUT.                     |
+| json     Parse ixf FILE and convert it to a json OUTPUT.                    |
+| parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                 |
++-----------------------------------------------------------------------------+
+
+ Made with heart :D
+
+```
+
 #### Parsing an IXF file
 
 ```python
 # coding=utf-8
 from pathlib import Path
 from db2ixf import IXFParser
 
@@ -127,44 +161,14 @@
 with open(path, mode='rb') as f:
     parser = IXFParser(f)
     output_path = Path('path/to/output/file.parquet')
     with open(output_path, mode='wb') as output_file:
         parser.to_parquet(output_file)
 ```
 
-#### CLI
-
-Start with this:
-
-```bash
-db2ixf --help
-```
-
-Result:
-
-```
-Usage: db2ixf [OPTIONS] COMMAND [ARGS]...
-
- A command-line tool (CLI) for parsing and converting IXF (IBM DB2 Import/Export Format) files to various formats such as JSON, CSV, and Parquet. Easily parse and convert IXF files to meet your data processing needs.
-
-┌─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
-│ --version             -v        Show the version of the CLI.                                                                                                                                                                        │
-│ --install-completion            Install completion for the current shell.                                                                                                                                                           │
-│ --show-completion               Show completion for the current shell, to copy it or customize the installation.                                                                                                                    │
-│ --help                          Show this message and exit.                                                                                                                                                                         │
-└─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
-┌─ Commands ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
-│ csv      Parse ixf FILE and convert it to a csv OUTPUT.                                                                                                                                                                             │
-│ json     Parse ixf FILE and convert it to a json OUTPUT.                                                                                                                                                                            │
-│ parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                                                                                                                                                                         │
-└─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
-
- Made with heart :D
-```
-
 For a detailed story and usage, please refer to the
 [documentation](https://ismailhammounou.github.io/db2ixf/).
 
 ## Contributing
 
 IXF Parser is actively seeking contributions to enhance its features and
 reliability. Your participation is valuable in shaping the future of the
@@ -188,15 +192,15 @@
 - [x] Adding new collector for the floating point data type.
 - [ ] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [x] Add better ci-cd.
 - [x] Improve Makefile.
-- [x] ~~Support multiprocessing.~~ 
+- [x] ~~Support multiprocessing.~~
 - [x] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `db2ixf-0.1.6/README.md` & `db2ixf-0.1.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # DB2IXF Parser
 
 <div align="center">
   <img src="https://github.com/ismailhammounou/db2ixf/blob/main/resources/images/db2ixf-logo.png?raw=true" alt="Logo" width="300" height="300">
 </div>
 
 DB2IXF parser is an open-source python package that simplifies the parsing and
-processing of IBM eXchange Format (IXF) files. IXF is a file format used by
-IBM's DB2 database system for data import and export operations. This package
-provides a streamlined solution for extracting data from IXF files and
+processing of IBM Integration eXchange Format (IXF) files. IXF is a file format
+used by IBM's DB2 database system for data import and export operations. This
+package provides a streamlined solution for extracting data from IXF files and
 converting it to various formats, including JSON, CSV, and Parquet.
 
 ## Features
 
 - **Parse IXF files**: The package allows you to parse IXF files and extract the
   rows of data stored within them.
 - **Convert to multiple formats**: The parsed data can be easily converted to
@@ -43,14 +43,48 @@
 pip install db2ixf
 ```
 
 ### Usage
 
 Here are some examples of how to use DB2 IXF Parser:
 
+#### CLI
+
+Start with this:
+
+```bash
+db2ixf --help
+```
+
+Result:
+
+```
+ Usage: db2ixf [OPTIONS] COMMAND [ARGS]...
+
+ A command-line tool (CLI) for parsing and converting IXF (IBM DB2 Import/Export 
+ Format) files to various formats such as JSON, CSV, and Parquet. Easily parse 
+ and convert IXF files to meet your data processing needs.
+
++- Options -------------------------------------------------------------------+
+| --version             -v        Show the version of the CLI.                |
+| --install-completion            Install completion for the current shell.   |
+| --show-completion               Show completion for the current shell, to   |
+|                                 copy it or customize the installation.      |
+| --help                          Show this message and exit.                 |
++-----------------------------------------------------------------------------+
++- Commands ------------------------------------------------------------------+
+| csv      Parse ixf FILE and convert it to a csv OUTPUT.                     |
+| json     Parse ixf FILE and convert it to a json OUTPUT.                    |
+| parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                 |
++-----------------------------------------------------------------------------+
+
+ Made with heart :D
+
+```
+
 #### Parsing an IXF file
 
 ```python
 # coding=utf-8
 from pathlib import Path
 from db2ixf import IXFParser
 
@@ -103,44 +137,14 @@
 with open(path, mode='rb') as f:
     parser = IXFParser(f)
     output_path = Path('path/to/output/file.parquet')
     with open(output_path, mode='wb') as output_file:
         parser.to_parquet(output_file)
 ```
 
-#### CLI
-
-Start with this:
-
-```bash
-db2ixf --help
-```
-
-Result:
-
-```
-Usage: db2ixf [OPTIONS] COMMAND [ARGS]...
-
- A command-line tool (CLI) for parsing and converting IXF (IBM DB2 Import/Export Format) files to various formats such as JSON, CSV, and Parquet. Easily parse and convert IXF files to meet your data processing needs.
-
-┌─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
-│ --version             -v        Show the version of the CLI.                                                                                                                                                                        │
-│ --install-completion            Install completion for the current shell.                                                                                                                                                           │
-│ --show-completion               Show completion for the current shell, to copy it or customize the installation.                                                                                                                    │
-│ --help                          Show this message and exit.                                                                                                                                                                         │
-└─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
-┌─ Commands ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
-│ csv      Parse ixf FILE and convert it to a csv OUTPUT.                                                                                                                                                                             │
-│ json     Parse ixf FILE and convert it to a json OUTPUT.                                                                                                                                                                            │
-│ parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                                                                                                                                                                         │
-└─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
-
- Made with heart :D
-```
-
 For a detailed story and usage, please refer to the
 [documentation](https://ismailhammounou.github.io/db2ixf/).
 
 ## Contributing
 
 IXF Parser is actively seeking contributions to enhance its features and
 reliability. Your participation is valuable in shaping the future of the
@@ -164,15 +168,15 @@
 - [x] Adding new collector for the floating point data type.
 - [ ] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [x] Add better ci-cd.
 - [x] Improve Makefile.
-- [x] ~~Support multiprocessing.~~ 
+- [x] ~~Support multiprocessing.~~
 - [x] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `db2ixf-0.1.6/pyproject.toml` & `db2ixf-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -123,21 +123,21 @@
 sigterm = true
 
 [tool.coverage.report]
 skip_empty = true
 sort = 'Cover'
 
 [tool.coverage.html]
-directory = 'report/coverage/html'
+directory = 'target/report/coverage/html'
 
 [tool.coverage.xml]
-output = 'report/coverage/coverage.xml'
+output = 'target/report/coverage/coverage.xml'
 
 [tool.coverage.json]
-output = 'report/coverage/coverage.json'
+output = 'target/report/coverage/coverage.json'
 
 
 
 [tool.towncrier]
 directory = 'resources/changelog'
 filename = 'CHANGELOG.md'
 start_string = '<!-- release notes start -->'
```

### Comparing `db2ixf-0.1.6/src/db2ixf/__init__.py` & `db2ixf-0.1.7/src/db2ixf/__init__.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.6/src/db2ixf/cli.py` & `db2ixf-0.1.7/src/db2ixf/cli.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.6/src/db2ixf/collectors.py` & `db2ixf-0.1.7/src/db2ixf/collectors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,45 @@
 # coding=utf-8
-"""Collects data from fields extracted from data records."""
-from datetime import datetime
+"""Collects data from the fields extracted from the data records (D)."""
+from datetime import datetime, date, time
+from db2ixf.exceptions import LargeObjectLengthException, \
+    BinaryLengthException, ExceedingDefinedMaximumLengthException
 from struct import unpack
 from typing import Union
 
 
+def collect_binary(c, fields, pos, encoding) -> bytes:
+    """Collects BINARY data type from ixf as a bytes.
+
+    Parameters
+    ----------
+    c : dict
+        Column descriptor extracted from IXF.
+    fields : str
+        Binary string containing data of the row.
+    pos : int
+        Position of the column in the `fields`.
+    encoding : str
+        Encoding of the ixf file.
+
+    Returns
+    -------
+    bytes:
+        a binary string data.
+    """
+    length = int(c['IXFCLENG'])
+    if length > 254:
+        msg = 'Length of a binary data types should not exceed 254 bytes.'
+        raise BinaryLengthException(msg)
+
+    field = fields[pos:pos + length]
+
+    return field
+
+
 def collect_smallint(c, fields, pos, encoding) -> int:
     """Collects SMALLINT data type from ixf as an integer.
 
     Parameters
     ----------
     c : dict
         Column descriptor extracted from IXF.
@@ -246,10 +277,89 @@
     encoding : str
         Encoding of the ixf file.
 
     Returns
     -------
     timestamp:
         Timestamp of format yyyy-mm-dd-HH.MM.SS.UUUUUU
+
+    Raises
+    ------
+    LargeObjectLengthException
+        When the length of the large object exceeds the maximum length.
     """
     field = str(fields[pos:pos + 26], encoding=encoding)
     return datetime.strptime(field, '%Y-%m-%d-%H.%M.%S.%f')
+
+
+def collect_clob(c, fields, pos, encoding) -> str:
+    """Collects CLOB data type from ixf as a string object.
+
+    Parameters
+    ----------
+    c : dict
+        Column descriptor extracted from IXF.
+    fields : str
+        Binary string containing data of the row.
+    pos : int
+        Position of the column in the `fields`.
+    encoding : str
+        Encoding of the ixf file.
+
+    Returns
+    -------
+    str
+        String representing the CLOB (Character Large Object).
+    """
+    max_length = int(c['IXFCLENG'])
+    if max_length > 32767:
+        msg = 'For CLOB data type, max length must be less than 32767 Bytes.'
+        raise ExceedingDefinedMaximumLengthException(msg)
+
+    length = int(unpack('<h', fields[pos:pos + 4])[0])
+    if length > max_length:
+        msg = f'Length exceeds the maximum length {max_length}.'
+        raise LargeObjectLengthException(msg)
+
+    pos += 4
+    field = str(fields[pos:pos + length], encoding=encoding)
+    return field.strip()
+
+
+def collect_blob(c, fields, pos, encoding) -> bytes:
+    """Collects BLOB data type from ixf as a binary string large object.
+
+    Parameters
+    ----------
+    c : dict
+        Column descriptor extracted from IXF.
+    fields : str
+        Binary string containing data of the row.
+    pos : int
+        Position of the column in the `fields`.
+    encoding : str
+        Encoding of the ixf file.
+
+    Returns
+    -------
+    bytes
+        Binary string representing the BLOB (Blob Large Object).
+
+    Raises
+    ------
+    LargeObjectLengthException
+        When the length of the large object exceeds the maximum length.
+    """
+    max_length = int(c['IXFCLENG'])
+    if max_length > 32767:
+        msg = 'For BLOB data type, max length must be less than 32767 Bytes.'
+        raise ExceedingDefinedMaximumLengthException(msg)
+
+    length = int(unpack('<h', fields[pos:pos + 4])[0])
+    if length > max_length:
+        msg = f'Length exceeds the maximum length {max_length}.'
+        raise LargeObjectLengthException(msg)
+
+    pos += 4
+    field = fields[pos:pos + length]
+
+    return field
```

### Comparing `db2ixf-0.1.6/src/db2ixf/constants.py` & `db2ixf-0.1.7/src/db2ixf/constants.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.6/src/db2ixf/helpers.py` & `db2ixf-0.1.7/src/db2ixf/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,29 +21,36 @@
         Maps columns extracted from IXF file to their pyarrow data types.
     """
 
     mapper = {
         'DATE': pyarrow.date32(),
         'TIME': pyarrow.time64('ns'),
         'TIMESTAMP': pyarrow.timestamp('ns'),
+        'BLOB': pyarrow.large_binary(),
+        'CLOB': pyarrow.large_string(),
         'VARCHAR': pyarrow.string(),
         'CHAR': pyarrow.string(),
         'FLOATING POINT': pyarrow.float64(),
         'DECIMAL': pyarrow.decimal128(19),
         'BIGINT': pyarrow.int64(),
         'INTEGER': pyarrow.int32(),
         'SMALLINT': pyarrow.int16(),
+        'BINARY': pyarrow.binary(254),
     }
 
     schema = {}
     for c in cols:
         cname = c['IXFCNAME'].decode('utf-8').strip()
         ctype = int(c['IXFCTYPE'])
         dtype = mapper[IXF_DTYPES[ctype]]
 
+        if ctype == 912:
+            length = int(c['IXFCLENG'])
+            dtype = pyarrow.binary(length)
+
         if ctype == 480:
             length = int(c['IXFCLENG'])
             dtype = pyarrow.float32() if length == 4 else dtype
 
         if ctype == 484:
             precision = int(c['IXFCLENG'][0:3])
             scale = int(c['IXFCLENG'][3:5])
@@ -59,23 +66,24 @@
             elif 0 < fsp <= 3:
                 dtype = pyarrow.timestamp('ms')
             elif 3 < fsp <= 6:
                 dtype = pyarrow.timestamp('us')
             elif 6 < fsp <= 12:
                 dtype = pyarrow.timestamp('ns')
             else:
-                msg = f'Precision of the decimal column {cname} is not valid, it should be <= 12'
+                msg = f'Precision of the decimal column {cname} is not' \
+                      f' valid, it should be <= 12'
                 raise NotValidDataPrecisionException(msg)
 
         schema[cname] = dtype
 
     return schema
 
 
-def get_pandas_schema(cols: list[dict]):
+def get_pandas_schema(cols: list[dict]) -> dict[str, object]:
     """Creates a pandas schema of the columns extracted from IXF file.
 
     Parameters
     ----------
     cols : list[dict]
         List of column descriptors extracted from IXF file.
 
@@ -85,21 +93,24 @@
         Maps columns extracted from IXF file to their pandas data types.
     """
 
     mapper = {
         'DATE': 'datetime64[ns]',
         'TIME': 'datetime64[ns]',
         'TIMESTAMP': 'datetime64[ns]',
+        'BLOB': bytes,
+        'CLOB': object,
         'VARCHAR': object,
         'CHAR': object,
         'FLOATING POINT': 'float64',
         'DECIMAL': 'float32',
         'BIGINT': 'int64',
         'INTEGER': 'int64',
         'SMALLINT': 'int64',
+        'BINARY': bytes,
     }
 
     schema = {}
     for c in cols:
         cname = str(c['IXFCNAME'], encoding='utf-8').strip()
         ctype = int(c['IXFCTYPE'])
         dtype = mapper[IXF_DTYPES[ctype]]
@@ -119,16 +130,16 @@
         schema[cname] = dtype
 
     return schema
 
 
 def merge_dicts(dicts: list[dict]) -> dict[str, list]:
     """
-    Merge a list of dictionaries into a single dictionary where each key is mapped
-    to a list of its values.
+    Merge a list of dictionaries into a single dictionary where each key is
+    mapped to a list of its values.
 
     Parameters
     ----------
     dicts : list
         A list of dictionaries.
 
     Returns
@@ -151,29 +162,30 @@
 
     return result
 
 
 def get_batch(generator: Generator, size: int = 500) -> Dict[str, list]:
     """Batch generator. It yields a batch of rows in a single dictionary.
 
-    It gets a list of size '`size`' containing rows from the data source generator then merge all
-    rows in one dictionary which is the yielded one.
+    It gets a list of size '`size`' containing rows from the data source
+    generator then merge all rows in one dictionary which is the yielded one.
 
 
     Parameters
     ----------
     generator : Generator
         Python generator that yields individual rows from the source data.
     size : int, optional
         Size of each batch (number of rows per batch). Default is 500.
 
     Yields
     ------
     Generator[List, None, None]
-        A generator that yields batches of rows, where each batch is a list of rows.
+        A generator that yields batches of rows, where each batch is a
+        list of rows.
 
     Examples
     --------
     Get a batch generator from a data generator and process the batches:
 
     >>> data_generator = some_data_generator  # Assuming yields rows  # noqa
     >>> batch_generator = get_batch(data_generator, size=100)
```

### Comparing `db2ixf-0.1.6/src/db2ixf/ixf.py` & `db2ixf-0.1.7/src/db2ixf/ixf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
                                collect_date,
                                collect_decimal,
                                collect_integer,
                                collect_time,
                                collect_timestamp,
                                collect_varchar,
                                collect_smallint,
-                               collect_floating_point)
+                               collect_floating_point,
+                               collect_blob,
+                               collect_clob,
+                               collect_binary)
 from db2ixf.constants import (HEADER_RECORD_TYPE,
                               TABLE_RECORD_TYPE,
                               COL_DESCRIPTOR_RECORD_TYPE,
                               DATA_RECORD_TYPE)
 from db2ixf.encoders import CustomJSONEncoder
 from db2ixf.exceptions import (
     NotValidColumnDescriptorException,
@@ -254,21 +257,24 @@
                     pos += 2
 
             # Collect data
             switcher = {
                 384: collect_date,
                 388: collect_time,
                 392: collect_timestamp,
+                404: collect_blob,
+                408: collect_clob,
                 448: collect_varchar,
                 452: collect_char,
                 480: collect_floating_point,
                 484: collect_decimal,
                 492: collect_bigint,
                 496: collect_integer,
                 500: collect_smallint,
+                912: collect_binary,
             }
             func = switcher.get(col_type, None)
             try:
                 if func is None:
                     msg = f'The column {col_name} has unknown data ' \
                           f'type {col_type}'
                     raise UnknownDataTypeException(msg)
```

### Comparing `db2ixf-0.1.6/src/db2ixf/logger.py` & `db2ixf-0.1.7/src/db2ixf/logger.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.6/src/db2ixf.egg-info/PKG-INFO` & `db2ixf-0.1.7/src/db2ixf.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://pypi.org/project/db2ixf/
 Project-URL: documentation, https://ismailhammounou.github.io/db2ixf/
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
@@ -29,17 +29,17 @@
 # DB2IXF Parser
 
 <div align="center">
   <img src="https://github.com/ismailhammounou/db2ixf/blob/main/resources/images/db2ixf-logo.png?raw=true" alt="Logo" width="300" height="300">
 </div>
 
 DB2IXF parser is an open-source python package that simplifies the parsing and
-processing of IBM eXchange Format (IXF) files. IXF is a file format used by
-IBM's DB2 database system for data import and export operations. This package
-provides a streamlined solution for extracting data from IXF files and
+processing of IBM Integration eXchange Format (IXF) files. IXF is a file format
+used by IBM's DB2 database system for data import and export operations. This
+package provides a streamlined solution for extracting data from IXF files and
 converting it to various formats, including JSON, CSV, and Parquet.
 
 ## Features
 
 - **Parse IXF files**: The package allows you to parse IXF files and extract the
   rows of data stored within them.
 - **Convert to multiple formats**: The parsed data can be easily converted to
@@ -67,14 +67,48 @@
 pip install db2ixf
 ```
 
 ### Usage
 
 Here are some examples of how to use DB2 IXF Parser:
 
+#### CLI
+
+Start with this:
+
+```bash
+db2ixf --help
+```
+
+Result:
+
+```
+ Usage: db2ixf [OPTIONS] COMMAND [ARGS]...
+
+ A command-line tool (CLI) for parsing and converting IXF (IBM DB2 Import/Export 
+ Format) files to various formats such as JSON, CSV, and Parquet. Easily parse 
+ and convert IXF files to meet your data processing needs.
+
++- Options -------------------------------------------------------------------+
+| --version             -v        Show the version of the CLI.                |
+| --install-completion            Install completion for the current shell.   |
+| --show-completion               Show completion for the current shell, to   |
+|                                 copy it or customize the installation.      |
+| --help                          Show this message and exit.                 |
++-----------------------------------------------------------------------------+
++- Commands ------------------------------------------------------------------+
+| csv      Parse ixf FILE and convert it to a csv OUTPUT.                     |
+| json     Parse ixf FILE and convert it to a json OUTPUT.                    |
+| parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                 |
++-----------------------------------------------------------------------------+
+
+ Made with heart :D
+
+```
+
 #### Parsing an IXF file
 
 ```python
 # coding=utf-8
 from pathlib import Path
 from db2ixf import IXFParser
 
@@ -127,44 +161,14 @@
 with open(path, mode='rb') as f:
     parser = IXFParser(f)
     output_path = Path('path/to/output/file.parquet')
     with open(output_path, mode='wb') as output_file:
         parser.to_parquet(output_file)
 ```
 
-#### CLI
-
-Start with this:
-
-```bash
-db2ixf --help
-```
-
-Result:
-
-```
-Usage: db2ixf [OPTIONS] COMMAND [ARGS]...
-
- A command-line tool (CLI) for parsing and converting IXF (IBM DB2 Import/Export Format) files to various formats such as JSON, CSV, and Parquet. Easily parse and convert IXF files to meet your data processing needs.
-
-┌─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
-│ --version             -v        Show the version of the CLI.                                                                                                                                                                        │
-│ --install-completion            Install completion for the current shell.                                                                                                                                                           │
-│ --show-completion               Show completion for the current shell, to copy it or customize the installation.                                                                                                                    │
-│ --help                          Show this message and exit.                                                                                                                                                                         │
-└─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
-┌─ Commands ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
-│ csv      Parse ixf FILE and convert it to a csv OUTPUT.                                                                                                                                                                             │
-│ json     Parse ixf FILE and convert it to a json OUTPUT.                                                                                                                                                                            │
-│ parquet  Parse ixf FILE and convert it to a parquet OUTPUT.                                                                                                                                                                         │
-└─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
-
- Made with heart :D
-```
-
 For a detailed story and usage, please refer to the
 [documentation](https://ismailhammounou.github.io/db2ixf/).
 
 ## Contributing
 
 IXF Parser is actively seeking contributions to enhance its features and
 reliability. Your participation is valuable in shaping the future of the
@@ -188,15 +192,15 @@
 - [x] Adding new collector for the floating point data type.
 - [ ] Adding new collectors for other ixf data types: binary ...etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [x] Add better ci-cd.
 - [x] Improve Makefile.
-- [x] ~~Support multiprocessing.~~ 
+- [x] ~~Support multiprocessing.~~
 - [x] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `db2ixf-0.1.6/src/db2ixf.egg-info/SOURCES.txt` & `db2ixf-0.1.7/src/db2ixf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

