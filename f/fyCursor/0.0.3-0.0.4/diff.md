# Comparing `tmp/fyCursor-0.0.3.tar.gz` & `tmp/fyCursor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.0.3.tar", last modified: Tue May 16 03:39:00 2023, max compression
+gzip compressed data, was "fyCursor-0.0.4.tar", last modified: Tue Jun  6 21:33:19 2023, max compression
```

## Comparing `fyCursor-0.0.3.tar` & `fyCursor-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 03:39:00.255984 fyCursor-0.0.3/
--rw-r--r--   0 danielkay   (503) staff       (20)     1062 2023-05-14 02:45:31.000000 fyCursor-0.0.3/LICENSE
--rw-r--r--   0 danielkay   (503) staff       (20)      508 2023-05-16 03:39:00.255839 fyCursor-0.0.3/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      272 2023-05-16 03:37:49.000000 fyCursor-0.0.3/README.md
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 03:39:00.251340 fyCursor-0.0.3/fyCursor/
--rw-r--r--   0 danielkay   (503) staff       (20)      590 2023-05-16 03:38:55.000000 fyCursor-0.0.3/fyCursor/__init__.py
--rw-r--r--   0 danielkay   (503) staff       (20)     4015 2023-05-16 03:19:09.000000 fyCursor-0.0.3/fyCursor/core.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-05-16 03:39:00.255598 fyCursor-0.0.3/fyCursor.egg-info/
--rw-r--r--   0 danielkay   (503) staff       (20)      508 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      192 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-05-16 03:39:00.000000 fyCursor-0.0.3/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-05-16 03:39:00.256032 fyCursor-0.0.3/setup.cfg
--rw-r--r--   0 danielkay   (503) staff       (20)      698 2023-05-16 01:51:46.000000 fyCursor-0.0.3/setup.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.786867 fyCursor-0.0.4/
+-rw-r--r--   0 danielkay   (503) staff       (20)     1067 2023-05-18 03:38:19.000000 fyCursor-0.0.4/LICENSE
+-rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:33:19.786677 fyCursor-0.0.4/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      569 2023-06-06 20:46:34.000000 fyCursor-0.0.4/README.md
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.782289 fyCursor-0.0.4/fyCursor/
+-rw-r--r--   0 danielkay   (503) staff       (20)     1374 2023-06-06 21:31:15.000000 fyCursor-0.0.4/fyCursor/__init__.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.786255 fyCursor-0.0.4/fyCursor/core/
+-rw-r--r--   0 danielkay   (503) staff       (20)      148 2023-06-06 20:42:16.000000 fyCursor-0.0.4/fyCursor/core/__init__.py
+-rw-r--r--   0 danielkay   (503) staff       (20)     4342 2023-06-06 21:01:22.000000 fyCursor-0.0.4/fyCursor/core/cursor.py
+-rw-r--r--   0 danielkay   (503) staff       (20)      708 2023-05-30 01:08:38.000000 fyCursor-0.0.4/fyCursor/core/fields.py
+-rw-r--r--   0 danielkay   (503) staff       (20)     2208 2023-06-06 21:04:39.000000 fyCursor-0.0.4/fyCursor/core/table.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.784646 fyCursor-0.0.4/fyCursor.egg-info/
+-rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      272 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-06-06 21:33:19.786928 fyCursor-0.0.4/setup.cfg
+-rw-r--r--   0 danielkay   (503) staff       (20)      645 2023-06-06 21:32:53.000000 fyCursor-0.0.4/setup.py
```

### Comparing `fyCursor-0.0.3/LICENSE` & `fyCursor-0.0.4/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 felix
+Copyright (c) 2023 Baffu Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fyCursor-0.0.3/fyCursor/core.py` & `fyCursor-0.0.4/fyCursor/core/cursor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,153 @@
-import logging
 import sqlite3
+import logging
 
-from typing import Union, Any, Type, Optional
+from typing import Union, Any, Optional
+from .table import Table
 
-def connect(
-    database: str, 
-) -> 'fyCursor':
-
-    connection = sqlite3.connect(
-        database=database, 
-    )
-    return connection.cursor(fyCursor) #type: ignore
-    
 
 class fyCursor(sqlite3.Cursor):
     """
     Custom `sqlite3.Cursor` that can be used without string query. \n
     I just hate query because it does not have any highlighting in IDE, yeah.
 
     https://github.com/felixyeahh/fyCursor
     """
     def __init__(
-        self, 
-        __cursor: sqlite3.Connection, 
-        logger = None
+        self,
+        __cursor: sqlite3.Connection,
+        logger: Any = None
     ) -> None:
         """
         Initialise a cursor.
 
         :param __cursor - sqlite3 connection
-        :param logger - custom logger (Optional) 
+        :param logger - custom logger (Optional)
         """
         super().__init__(__cursor)
-        self._logger = logging.getLogger("fyCursor") if logger is None else logger
-        
+        self._logger = logging.getLogger(
+            "fyCursor"
+        ) if logger is None else logger
 
-    def update(self, table) -> 'fyCursor':
+    def update(self, table: str) -> 'fyCursor':
         """
         Use this as SQL `UPDATE {table}` method
-        
+
         :param table: - table to be updated
         :returns: - self
         """
         self._query = f"UPDATE {table}"
         return self
 
-
-    def add(self, **kwargs) -> 'fyCursor':
+    def add(self, **kwargs: Any) -> 'fyCursor':
         """
         Use this as SQL `SET {kwargs.keys}={kwargs.keys}+{kwargs.values}`
-        
+
         **kwargs
 
         :returns: - self
 
-        :raises: - `sqlite3.ProgrammingError` if you didn't use `fyCursor.update()` 
-        or something similar before this statement
+        :raises: - `sqlite3.ProgrammingError` if you didn't use
+        `fyCursor.update()` or something similar before this statement
         """
         if not self._query:
-            raise sqlite3.ProgrammingError("You should use something before `add`")
+            raise sqlite3.ProgrammingError(
+                "You should use something before `add`"
+            )
         column = list(kwargs.keys())[0]
         value = list(kwargs.values())[0]
         self._query += f" SET {column} = {column} + {value}"
         return self
-        
 
-    def set(self, **kwargs) -> 'fyCursor':
+    def set(self, **kwargs: Any) -> 'fyCursor':
         """
-        Use this as SQL `SET {kwargs.keys}={kwargs.values}`
+        Use this as SQL`SET {kwargs.keys} = {kwargs.values}`
 
         :returns: - self
 
-        :raises: - `sqlite3.ProgrammingError` if you didn't use `fyCursor.update()` 
-        or something similar before this statement
+        :raises: - `sqlite3.ProgrammingError` if you didn't use
+        `fyCursor.update()` or something similar before this statement
         """
         if not self._query:
-            raise sqlite3.ProgrammingError("You should use something before `set`")
+            raise sqlite3.ProgrammingError(
+                "You should use something before `set`"
+            )
 
         column = list(kwargs.keys())[0]
         value = str(list(kwargs.values())[0])
+        column = column or "NULL"
         self._query += f" SET {column} = {value}"
         return self
-        
 
-    def select(self, value, from_ = None) -> 'fyCursor':
+    def select(self, value, from_: Optional[str] = None) -> 'fyCursor':
         """
         Use this as SQL `SELECT {value} FROM {from_}`
 
         :param value: - value to be selected
         :param from_: - table from which value will be selected
 
         :returns: - self
         """
         self._query = f"SELECT {value}"
         if from_ is not None:
             self._from(from_)
         return self
 
-
     def _from(self, table) -> 'fyCursor':
         self._query += f" FROM {table}"
         return self
 
-
     def where(self, **kwargs) -> 'fyCursor':
         if not self._query:
-            raise sqlite3.ProgrammingError("You should use something before `where`")
-        self._query += f" WHERE {list(kwargs.keys())[0]} = \"{list(kwargs.values())[0]}\""
+            raise sqlite3.ProgrammingError(
+                "You should use something before `where`"
+            )
+        self._query += (
+            f" WHERE {list(kwargs.keys())[0]} "
+            f"= \"{list(kwargs.values())[0]}\""
+        )
         return self
 
-
-    def fetch(self, one: bool = False) -> Union[list, tuple[Any], None]:
+    def fetch(
+        self, one: bool = False
+    ) -> Optional[Union[tuple[Any], list[Any]]]:
         """
         fetch values from cursor query
-        
-        :param one - if `True` provided, the `cursor.fetchone()` function will be used
+
+        :param one - if `True` provided, the `cursor.fetchone()`
+        function will be used
         """
         if not self._query:
             raise sqlite3.ProgrammingError("Nothing to fetch")
         super().execute(self._query)
         super().connection.commit()
-        return super().fetchone() if one else super().fetchall()        
-
+        return super().fetchone() if one else super().fetchall()
 
     def one(self) -> Any:
         """
         returns exact one result of fetching, not tuple
         """
         fetching = self.fetch(True)
 
         if fetching is None:
             return None
-        elif type(fetching) in [list, tuple]:
+        elif isinstance(fetching, (list, tuple)):
             return fetching[0]
         return fetching
 
-
     def commit(self) -> 'fyCursor':
         if self._query:
             super().execute(self._query)
         super().connection.commit()
-        return self
+        return self
+
+    def create_table(
+        self,
+        table: Table,
+        if_not_exist: bool = False
+    ) -> "Table":
+        exist = "IF NOT EXISTS" if if_not_exist else ""
+        super().execute(f"""
+            CREATE TABLE {exist} {table.name}({table._sql[:-1]})
+        """)
+
+        return table
```

### Comparing `fyCursor-0.0.3/setup.py` & `fyCursor-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# usage: python3 setup.py sdist bdist_wheel
+
+# ! usage: python3 setup.py sdist bdist_wheel
 from setuptools import setup, find_packages
+
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
-from fyCursor import Info
-self = Info()
-
 # Setting up
 setup(
-    name=self.__title__,
-    version=self.__version__,
-    description=self.__version__,
-    author=self.__author__,
-    author_email=self.__author_email__,
-    license=self.__license__,
+    name="fyCursor",
+    version="0.0.4",
+    description='Simple sqlite3 cursor',
+    author="felixyeahh",
+    author_email="<felixyeah@outlook.com>",
+    license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     keywords=['python', 'sqlite3', 'database'],
 )
```

