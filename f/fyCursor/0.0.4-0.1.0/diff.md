# Comparing `tmp/fyCursor-0.0.4.tar.gz` & `tmp/fyCursor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.0.4.tar", last modified: Tue Jun  6 21:33:19 2023, max compression
+gzip compressed data, was "fyCursor-0.1.0.tar", last modified: Tue Jun  6 21:46:49 2023, max compression
```

## Comparing `fyCursor-0.0.4.tar` & `fyCursor-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.786867 fyCursor-0.0.4/
--rw-r--r--   0 danielkay   (503) staff       (20)     1067 2023-05-18 03:38:19.000000 fyCursor-0.0.4/LICENSE
--rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:33:19.786677 fyCursor-0.0.4/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      569 2023-06-06 20:46:34.000000 fyCursor-0.0.4/README.md
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.782289 fyCursor-0.0.4/fyCursor/
--rw-r--r--   0 danielkay   (503) staff       (20)     1374 2023-06-06 21:31:15.000000 fyCursor-0.0.4/fyCursor/__init__.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.786255 fyCursor-0.0.4/fyCursor/core/
--rw-r--r--   0 danielkay   (503) staff       (20)      148 2023-06-06 20:42:16.000000 fyCursor-0.0.4/fyCursor/core/__init__.py
--rw-r--r--   0 danielkay   (503) staff       (20)     4342 2023-06-06 21:01:22.000000 fyCursor-0.0.4/fyCursor/core/cursor.py
--rw-r--r--   0 danielkay   (503) staff       (20)      708 2023-05-30 01:08:38.000000 fyCursor-0.0.4/fyCursor/core/fields.py
--rw-r--r--   0 danielkay   (503) staff       (20)     2208 2023-06-06 21:04:39.000000 fyCursor-0.0.4/fyCursor/core/table.py
-drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:33:19.784646 fyCursor-0.0.4/fyCursor.egg-info/
--rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 danielkay   (503) staff       (20)      272 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-06-06 21:33:19.000000 fyCursor-0.0.4/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-06-06 21:33:19.786928 fyCursor-0.0.4/setup.cfg
--rw-r--r--   0 danielkay   (503) staff       (20)      645 2023-06-06 21:32:53.000000 fyCursor-0.0.4/setup.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.078052 fyCursor-0.1.0/
+-rw-r--r--   0 danielkay   (503) staff       (20)     1067 2023-05-18 03:38:19.000000 fyCursor-0.1.0/LICENSE
+-rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:46:49.077894 fyCursor-0.1.0/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      569 2023-06-06 21:46:19.000000 fyCursor-0.1.0/README.md
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.059445 fyCursor-0.1.0/fyCursor/
+-rw-r--r--   0 danielkay   (503) staff       (20)     1374 2023-06-06 21:46:36.000000 fyCursor-0.1.0/fyCursor/__init__.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.077500 fyCursor-0.1.0/fyCursor/core/
+-rw-r--r--   0 danielkay   (503) staff       (20)      148 2023-06-06 20:42:16.000000 fyCursor-0.1.0/fyCursor/core/__init__.py
+-rw-r--r--   0 danielkay   (503) staff       (20)     4342 2023-06-06 21:01:22.000000 fyCursor-0.1.0/fyCursor/core/cursor.py
+-rw-r--r--   0 danielkay   (503) staff       (20)      708 2023-05-30 01:08:38.000000 fyCursor-0.1.0/fyCursor/core/fields.py
+-rw-r--r--   0 danielkay   (503) staff       (20)     2269 2023-06-06 21:44:41.000000 fyCursor-0.1.0/fyCursor/core/table.py
+drwxr-xr-x   0 danielkay   (503) staff       (20)        0 2023-06-06 21:46:49.062302 fyCursor-0.1.0/fyCursor.egg-info/
+-rw-r--r--   0 danielkay   (503) staff       (20)      821 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 danielkay   (503) staff       (20)      272 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        1 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)        9 2023-06-06 21:46:49.000000 fyCursor-0.1.0/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 danielkay   (503) staff       (20)       38 2023-06-06 21:46:49.078104 fyCursor-0.1.0/setup.cfg
+-rw-r--r--   0 danielkay   (503) staff       (20)      645 2023-06-06 21:46:27.000000 fyCursor-0.1.0/setup.py
```

### Comparing `fyCursor-0.0.4/LICENSE` & `fyCursor-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.0.4/PKG-INFO` & `fyCursor-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.0.4
+Version: 0.1.0
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,15 @@
 A simple cursor for managing sqlite3 databases
 
 ## Installation 
 You can simply use pip: &nbsp;
 \$`pip3 install fyCursor`
 
 # Changelog 📄
-### 📀 v0.0.4
+### 📀 v0.1.0
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
```

### Comparing `fyCursor-0.0.4/README.md` & `fyCursor-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A simple cursor for managing sqlite3 databases
 
 ## Installation 
 You can simply use pip: &nbsp;
 \$`pip3 install fyCursor`
 
 # Changelog 📄
-### 📀 v0.0.4
+### 📀 v0.1.0
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
```

### Comparing `fyCursor-0.0.4/fyCursor/__init__.py` & `fyCursor-0.1.0/fyCursor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
```

### Comparing `fyCursor-0.0.4/fyCursor/core/cursor.py` & `fyCursor-0.1.0/fyCursor/core/cursor.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.0.4/fyCursor/core/fields.py` & `fyCursor-0.1.0/fyCursor/core/fields.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.0.4/fyCursor/core/table.py` & `fyCursor-0.1.0/fyCursor/core/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,29 @@
     def __init__(
         self,
         name: str,
         cursor,
         args_fields: Optional[list[Field]] = None,
         kwargs_fields: Optional[dict[str, Field]] = None
     ) -> None:
-        assert kwargs_fields and args_fields, (
+        assert kwargs_fields or args_fields, (
             "you should provide either args_fields or kwargs_fields"
         )
         self._table = []
         self._sql = ""
         self.name = name
         self.cursor: fyCursor = cursor
-        self._table.extend(
-            f"{value} {value_._generate_field()},"
-            for value, value_ in kwargs_fields.items()
-        )
+        if kwargs_fields is not None:
+            self._table.extend(
+                f"{value} {value_._generate_field()},"
+                for value, value_ in kwargs_fields.items()
+            )
 
-        for value, value_ in kwargs_fields.items():
-            self._sql += f"{value} {value_._generate_field()},"
+            for value, value_ in kwargs_fields.items():
+                self._sql += f"{value} {value_._generate_field()},"
         if args_fields is not None:
             self._fields = {
                 str(arg.name): arg for arg in args_fields
             }
         else:
             return
         for value in args_fields:
```

### Comparing `fyCursor-0.0.4/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.0/fyCursor.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.0.4
+Version: 0.1.0
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,15 @@
 A simple cursor for managing sqlite3 databases
 
 ## Installation 
 You can simply use pip: &nbsp;
 \$`pip3 install fyCursor`
 
 # Changelog 📄
-### 📀 v0.0.4
+### 📀 v0.1.0
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
```

### Comparing `fyCursor-0.0.4/setup.py` & `fyCursor-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.0.4",
+    version="0.1.0",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

