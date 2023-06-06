# Comparing `tmp/utilki-0.3.3.tar.gz` & `tmp/utilki-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.3.3.tar", max compression
+gzip compressed data, was "utilki-0.3.4.tar", max compression
```

## Comparing `utilki-0.3.3.tar` & `utilki-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.3/README.md
--rw-r--r--   0        0        0      525 2023-05-25 19:22:26.189250 utilki-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.3.3/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.3/utilki/cli.py
--rw-r--r--   0        0        0     6503 2023-05-25 19:16:01.896303 utilki-0.3.3/utilki/task_mixin.py
--rw-r--r--   0        0        0     1846 2023-05-25 19:22:33.847695 utilki-0.3.3/setup.py
--rw-r--r--   0        0        0     1608 2023-05-25 19:22:33.847862 utilki-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.4/README.md
+-rw-r--r--   0        0        0      525 2023-06-06 14:38:46.779862 utilki-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.3.4/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.4/utilki/cli.py
+-rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.4/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-06-06 14:38:52.952075 utilki-0.3.4/setup.py
+-rw-r--r--   0        0        0     1608 2023-06-06 14:38:52.952366 utilki-0.3.4/PKG-INFO
```

### Comparing `utilki-0.3.3/README.md` & `utilki-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.3.3/pyproject.toml` & `utilki-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.3.3"
+version = "0.3.4"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.3.3/utilki/cli.py` & `utilki-0.3.4/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.3/utilki/task_mixin.py` & `utilki-0.3.4/utilki/task_mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,20 @@
 lists = [List[int], List[float], List[str], List[bool]]
 options = [
     Union[int, None],
     Union[float, None],
     Union[str, None],
     Union[bool, None],
 ]
-types_we_support = singles + lists + options
+
+dicts = [Dict[str, Any], Dict[str, str], Dict[str, int], Dict[str, float]] + [
+    Dict[str, Dict[str, Any]]
+]
+
+types_we_support = singles + lists + options + dicts
 
 IsDefault = bool
 
 
 def dbg(msg):
     if False:
         print(msg)
@@ -96,15 +101,17 @@
         if is_default:
             if type_ not in types_we_support:
                 raise TypeError("Invalid type")
             if type_ != type(value) and type_ in singles:
                 raise TypeError("Invalid type")
             if type_ in lists and not isinstance(value, list):
                 raise TypeError("Invalid type")
-            return value
+            else:
+                print("in else")
+                return value
         dbg(f"parsing '{name_}' with type {type_} and value {value}")
         if isinstance(value, str):
             res = parse_variations(type_, value, name_)
             dbg(f"res: {res}, type: {type_}, actual type {type(res)}")
             return res
         elif isinstance(value, list):
             if type_ in [List[int], List[str], List[float], List[bool]]:
@@ -174,14 +181,24 @@
         return parse_options(value, int)
     elif type_ == Union[str, None]:
         return parse_options(value, str)
     elif type_ == Union[float, None]:
         return parse_options(value, float)
     elif type_ == Union[bool, None]:
         return parse_options(value, parse_bool)
+    elif type_ == Dict[int, Any]:
+        return json.loads(value)
+    elif type_ == Dict[str, Any]:
+        return json.loads(value)
+    elif type_ == Dict[float, Any]:
+        return json.loads(value)
+    elif type_ == Dict[bool, Any]:
+        return json.loads(value)
+    elif type_ == Dict[str, Dict[str, Any]]:
+        return json.loads(value)
     elif type_ == bool:
         return parse_bool(value)
     elif type_ == int:
         return int(value)
     elif type_ == float:
         return float(value)
     elif type_ == str:
```

### Comparing `utilki-0.3.3/setup.py` & `utilki-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.3.3/PKG-INFO` & `utilki-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.3.3
+Version: 0.3.4
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

