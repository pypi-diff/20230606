# Comparing `tmp/py-csv-xls-0.0.4.tar.gz` & `tmp/py-csv-xls-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-csv-xls-0.0.4.tar", last modified: Mon Nov 28 10:37:37 2022, max compression
+gzip compressed data, was "py-csv-xls-0.0.6.tar", last modified: Tue Jun  6 07:49:50 2023, max compression
```

## Comparing `py-csv-xls-0.0.4.tar` & `py-csv-xls-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 gmp       (1000) gmp       (1000)        0 2022-11-28 10:37:37.859376 py-csv-xls-0.0.4/
--rw-rw-r--   0 gmp       (1000) gmp       (1000)     1917 2022-11-28 10:37:37.859376 py-csv-xls-0.0.4/PKG-INFO
--rw-rw-r--   0 gmp       (1000) gmp       (1000)      824 2022-11-28 09:50:06.000000 py-csv-xls-0.0.4/README.md
-drwxrwxr-x   0 gmp       (1000) gmp       (1000)        0 2022-11-28 10:37:37.859376 py-csv-xls-0.0.4/py_csv_xls/
--rw-rw-r--   0 gmp       (1000) gmp       (1000)      178 2022-11-28 10:37:33.000000 py-csv-xls-0.0.4/py_csv_xls/__init__.py
--rw-rw-r--   0 gmp       (1000) gmp       (1000)     2848 2022-11-28 10:37:01.000000 py-csv-xls-0.0.4/py_csv_xls/csvsniffer.py
--rw-rw-r--   0 gmp       (1000) gmp       (1000)     2763 2022-11-28 10:36:24.000000 py-csv-xls-0.0.4/py_csv_xls/excelworker.py
--rw-rw-r--   0 gmp       (1000) gmp       (1000)      289 2022-11-27 17:59:52.000000 py-csv-xls-0.0.4/py_csv_xls/exception.py
-drwxrwxr-x   0 gmp       (1000) gmp       (1000)        0 2022-11-28 10:37:37.859376 py-csv-xls-0.0.4/py_csv_xls.egg-info/
--rw-rw-r--   0 gmp       (1000) gmp       (1000)     1917 2022-11-28 10:37:37.000000 py-csv-xls-0.0.4/py_csv_xls.egg-info/PKG-INFO
--rw-rw-r--   0 gmp       (1000) gmp       (1000)      285 2022-11-28 10:37:37.000000 py-csv-xls-0.0.4/py_csv_xls.egg-info/SOURCES.txt
--rw-rw-r--   0 gmp       (1000) gmp       (1000)        1 2022-11-28 10:37:37.000000 py-csv-xls-0.0.4/py_csv_xls.egg-info/dependency_links.txt
--rw-rw-r--   0 gmp       (1000) gmp       (1000)       17 2022-11-28 10:37:37.000000 py-csv-xls-0.0.4/py_csv_xls.egg-info/requires.txt
--rw-rw-r--   0 gmp       (1000) gmp       (1000)       11 2022-11-28 10:37:37.000000 py-csv-xls-0.0.4/py_csv_xls.egg-info/top_level.txt
--rw-rw-r--   0 gmp       (1000) gmp       (1000)       38 2022-11-28 10:37:37.859376 py-csv-xls-0.0.4/setup.cfg
--rw-rw-r--   0 gmp       (1000) gmp       (1000)     1327 2022-11-27 18:12:23.000000 py-csv-xls-0.0.4/setup.py
+drwxrwxr-x   0 pog7x     (1000) pog7x     (1000)        0 2023-06-06 07:49:50.229091 py-csv-xls-0.0.6/
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)     1062 2023-06-06 06:48:02.000000 py-csv-xls-0.0.6/LICENSE
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)     1536 2023-06-06 07:49:50.229091 py-csv-xls-0.0.6/PKG-INFO
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)      675 2023-06-06 06:48:02.000000 py-csv-xls-0.0.6/README.md
+drwxrwxr-x   0 pog7x     (1000) pog7x     (1000)        0 2023-06-06 07:49:50.225091 py-csv-xls-0.0.6/py_csv_xls/
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)      177 2023-06-06 07:49:43.000000 py-csv-xls-0.0.6/py_csv_xls/__init__.py
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)     2786 2023-06-06 07:39:22.000000 py-csv-xls-0.0.6/py_csv_xls/csvsniffer.py
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)     2767 2023-06-06 07:38:21.000000 py-csv-xls-0.0.6/py_csv_xls/excelworker.py
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)      289 2023-06-06 06:48:02.000000 py-csv-xls-0.0.6/py_csv_xls/exception.py
+drwxrwxr-x   0 pog7x     (1000) pog7x     (1000)        0 2023-06-06 07:49:50.225091 py-csv-xls-0.0.6/py_csv_xls.egg-info/
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)     1536 2023-06-06 07:49:50.000000 py-csv-xls-0.0.6/py_csv_xls.egg-info/PKG-INFO
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)      293 2023-06-06 07:49:50.000000 py-csv-xls-0.0.6/py_csv_xls.egg-info/SOURCES.txt
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)        1 2023-06-06 07:49:50.000000 py-csv-xls-0.0.6/py_csv_xls.egg-info/dependency_links.txt
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)       17 2023-06-06 07:49:50.000000 py-csv-xls-0.0.6/py_csv_xls.egg-info/requires.txt
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)       11 2023-06-06 07:49:50.000000 py-csv-xls-0.0.6/py_csv_xls.egg-info/top_level.txt
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)       38 2023-06-06 07:49:50.229091 py-csv-xls-0.0.6/setup.cfg
+-rw-rw-r--   0 pog7x     (1000) pog7x     (1000)     1327 2023-06-06 06:48:02.000000 py-csv-xls-0.0.6/setup.py
```

### Comparing `py-csv-xls-0.0.4/py_csv_xls/csvsniffer.py` & `py-csv-xls-0.0.6/py_csv_xls/csvsniffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,56 +23,53 @@
         )
         self.__fields: typing.List = fields
         self.__start_row_flag: bool = not self.__fields
 
     def get_dir_files_with_lines(self) -> typing.List:
         try:
             return list(self.__main_dir_sniffer())
-        except Exception as e:
-            raise PyCsvXlsException(msg=f"{self.__class__.__name__} error", exc=e)
+        except Exception as err:
+            raise PyCsvXlsException(msg=f"{self.__class__.__name__} error", exc=err)
 
     @property
     def is_file(self) -> bool:
         return self.__is_file
 
     @property
     def is_csv_file(self) -> bool:
         return self.__is_csv_file(file_name=self.__main_path, only_ext=True)
 
     def __main_dir_sniffer(self) -> typing.Generator:
-        if not os.path.exists(self.__main_dir_path) or (
-            not os.path.isdir(self.__main_dir_path) and not self.__is_file
+        if not os.path.exists(self.__main_dir_path) or not (
+            os.path.isdir(self.__main_dir_path) or self.__is_file
         ):
             raise FileNotFoundError
         if self.__is_csv_file(file_name=self.__main_path, only_ext=True):
-            yield {
-                self.__main_path.split("/")[-1].rstrip(".csv"): list(
-                    self.__csv_file_parser(self.__main_path)
-                )
-            }
+            file_name = os.path.basename(self.__main_path)
+            lines = self.__csv_file_parser(self.__main_path)
+            yield {file_name: list(lines)}
         else:
             for dir_path, _, files_list in os.walk(self.__main_dir_path):
                 yield from self.__files_sniffer_by_pattern(dir_path, files_list)
 
     def __is_csv_file(self, file_name: str, only_ext: bool = False) -> bool:
+        ends_with = str(file_name).endswith(".csv")
         if only_ext:
-            return str(file_name).endswith(".csv")
-        return str(file_name).startswith(self.__file_startswith) and file_name.endswith(
-            ".csv"
-        )
+            return ends_with
+        starts_with = str(file_name).startswith(self.__file_startswith)
+        return starts_with and ends_with
 
     def __files_sniffer_by_pattern(
         self, curr_dir_path: str, files_list: typing.List[str]
     ) -> typing.Generator:
         for file_name in files_list:
             if self.__is_csv_file(file_name=file_name):
-                self.__start_row_flag = not self.__fields
                 lines = self.__csv_file_parser(os.path.join(curr_dir_path, file_name))
                 yield {file_name: list(lines)}
 
     def __csv_file_parser(self, abs_file_path: str) -> typing.Generator:
         with open(abs_file_path, "r", encoding="utf-8") as csv_file:
             for csv_line in csv.reader(csv_file):
                 if not self.__start_row_flag and csv_line == self.__fields:
                     self.__start_row_flag = True
-                if self.__start_row_flag is True:
+                if self.__start_row_flag:
                     yield csv_line
```

### Comparing `py-csv-xls-0.0.4/py_csv_xls/excelworker.py` & `py-csv-xls-0.0.6/py_csv_xls/excelworker.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
     def fill_workbook(self, all_data: typing.List[typing.Dict[str, typing.List]]):
         try:
             for ad in all_data:
                 for k, v in ad.items():
                     self.__create_and_fill_ws(sheet_name=k, data_to_fill=v)
                 self.__save_and_close_wb()
-        except Exception as e:
-            raise PyCsvXlsException(msg=f"{self.__class__.__name__} error", exc=e)
+        except Exception as err:
+            raise PyCsvXlsException(msg=f"{self.__class__.__name__} error", exc=err)
 
     @property
     def full_workbook_name(self) -> str:
         return self.__full_workbook_name
 
     def __load_or_create_wb(self):
         if self.__want_cleared:
```

### Comparing `py-csv-xls-0.0.4/setup.py` & `py-csv-xls-0.0.6/setup.py`

 * *Files identical despite different names*

