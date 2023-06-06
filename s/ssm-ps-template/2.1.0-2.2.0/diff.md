# Comparing `tmp/ssm-ps-template-2.1.0.tar.gz` & `tmp/ssm-ps-template-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.1.0.tar", last modified: Tue Jun  6 16:53:39 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.2.0.tar", last modified: Tue Jun  6 18:35:06 2023, max compression
```

## Comparing `ssm-ps-template-2.1.0.tar` & `ssm-ps-template-2.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    11887 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9251 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11887 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    12040 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9404 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12040 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 18:35:06.000000 ssm-ps-template-2.2.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 18:35:06.668367 ssm-ps-template-2.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-06 18:34:57.000000 ssm-ps-template-2.2.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.1.0/LICENSE.txt` & `ssm-ps-template-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/PKG-INFO` & `ssm-ps-template-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.1.0
+Version: 2.2.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -94,17 +94,17 @@
 The following example will iterate over the results:
 ```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
-Or you can use a Jinja filter to convert them to YAML:
+Or you can use Jinja filters to convert them to YAML:
 ```yaml
-{{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
+{{ get_parameters_by_path('settings/') | path_to_dict | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
 |-------------------------------|----------------------------------|
 | `/my-application/connections` | `amqp://server1, amqp://server2` |
@@ -167,14 +167,15 @@
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
 | `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
```

### Comparing `ssm-ps-template-2.1.0/README.md` & `ssm-ps-template-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 The following example will iterate over the results:
 ```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
-Or you can use a Jinja filter to convert them to YAML:
+Or you can use Jinja filters to convert them to YAML:
 ```yaml
-{{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
+{{ get_parameters_by_path('settings/') | path_to_dict | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
 |-------------------------------|----------------------------------|
 | `/my-application/connections` | `amqp://server1, amqp://server2` |
@@ -118,14 +118,15 @@
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
 | `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
```

### Comparing `ssm-ps-template-2.1.0/pyproject.toml` & `ssm-ps-template-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.1.0"
+version = "2.2.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template/__main__.py` & `ssm-ps-template-2.2.0/ssm_ps_template/__main__.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template/config.py` & `ssm-ps-template-2.2.0/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template/discovery.py` & `ssm-ps-template-2.2.0/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template/render.py` & `ssm-ps-template-2.2.0/ssm_ps_template/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import logging
 import os
 import pathlib
 import typing
 from urllib import parse
 
+import flatdict
 import yaml
 from jinja2 import sandbox
 
 from ssm_ps_template import ssm
 
 LOGGER = logging.getLogger(__name__)
 
 
+def path_to_dict(value: dict) -> dict:
+    flat = flatdict.FlatDict(value, delimiter='/')
+    return flat.as_dict()
+
+
 def replace_dashes_with_underscores(value_in: typing.Union[dict, list]) \
         -> typing.Union[dict, list]:
     if isinstance(value_in, dict):
         output = {}
         for key, value in value_in.items():
             new_key = key.replace('-', '_')
             if isinstance(value, (dict, list)):
@@ -44,14 +50,15 @@
 
     def render(self, values: ssm.Values) -> str:
         """Render the template to the internal buffer"""
         self._values = values
         environment = sandbox.ImmutableSandboxedEnvironment()
         environment.filters['dashes_to_underscores'] = \
             replace_dashes_with_underscores
+        environment.filters['path_to_dict'] = path_to_dict
         environment.filters['toyaml'] = lambda v: yaml.safe_dump(v)
         environment.globals['get_parameter'] = self._get_parameter
         environment.globals['get_parameters_by_path'] = \
             self._get_parameters_by_path
         environment.globals['parse_qs'] = parse.parse_qs
         environment.globals['unquote'] = parse.unquote
         environment.globals['urlparse'] = parse.urlparse
```

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template/ssm.py` & `ssm-ps-template-2.2.0/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.2.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.1.0
+Version: 2.2.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -94,17 +94,17 @@
 The following example will iterate over the results:
 ```yaml
 {% for key, value in get_parameters_by_path('settings/', {}).items() %}
   {{ key }}: {{ value }}
 {% endfor %}
 ```
 
-Or you can use a Jinja filter to convert them to YAML:
+Or you can use Jinja filters to convert them to YAML:
 ```yaml
-{{ get_parameters_by_path('settings/') | toyaml | indent(2, first=True) }}
+{{ get_parameters_by_path('settings/') | path_to_dict | toyaml | indent(2, first=True) }}
 ```
 
 For values in ParameterStore that are stored as `StringList`, they are automatically transformed as a list of strings. Given the following value:
 
 | Key                           | Value                            |
 |-------------------------------|----------------------------------|
 | `/my-application/connections` | `amqp://server1, amqp://server2` |
@@ -167,14 +167,15 @@
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
 | Filter                  | Description                                                                                                  |
 |-------------------------|--------------------------------------------------------------------------------------------------------------|
 | `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `path_to_dict`          | Converts a dict with forward-slash delimited keys (`/`) to a nested dict using the `/` as the key delimiter  |
 | `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
 | `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
```

### Comparing `ssm-ps-template-2.1.0/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.2.0/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/tests/test_config.py` & `ssm-ps-template-2.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/tests/test_discovery.py` & `ssm-ps-template-2.2.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/tests/test_main.py` & `ssm-ps-template-2.2.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.1.0/tests/test_render.py` & `ssm-ps-template-2.2.0/tests/test_render.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
         renderer = render.Renderer(
             utils.TEST_DATA_PATH / 'render/template.yaml.j2')
         result = renderer.render(values)
 
         path = utils.TEST_DATA_PATH / 'render/expectation.yaml'
         expectation = path.read_text('utf-8')
-
         self.assertEqual(result.strip(), expectation.strip())
 
 
 class DashesToUnderscoresTestCase(unittest.TestCase):
 
     def test_replace_dashes_with_underscores(self):
         value = {
@@ -57,7 +56,25 @@
         }
         self.assertDictEqual(
             render.replace_dashes_with_underscores(value), expectation)
 
     def test_raises_on_bad_data_type(self):
         with self.assertRaises(TypeError):
             render.replace_dashes_with_underscores('foo')
+
+
+class PathToDictTestCase(unittest.TestCase):
+
+    def test_path_to_dict(self):
+        value = {
+            'foo/bar/baz': 'qux',
+            'foo/bar/qux': 'quux'
+        }
+        expectation = {
+            'foo': {
+                'bar': {
+                    'baz': 'qux',
+                    'qux': 'quux'
+                }
+            }
+        }
+        self.assertDictEqual(render.path_to_dict(value), expectation)
```

### Comparing `ssm-ps-template-2.1.0/tests/test_ssm.py` & `ssm-ps-template-2.2.0/tests/test_ssm.py`

 * *Files identical despite different names*

