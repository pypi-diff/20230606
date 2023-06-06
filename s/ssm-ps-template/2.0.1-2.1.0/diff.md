# Comparing `tmp/ssm-ps-template-2.0.1.tar.gz` & `tmp/ssm-ps-template-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-2.0.1.tar", last modified: Thu Jun  1 21:28:27 2023, max compression
+gzip compressed data, was "ssm-ps-template-2.1.0.tar", last modified: Tue Jun  6 16:53:39 2023, max compression
```

## Comparing `ssm-ps-template-2.0.1.tar` & `ssm-ps-template-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.425444 ssm-ps-template-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    11045 2023-06-01 21:28:27.425444 ssm-ps-template-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8409 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 21:28:27.425444 ssm-ps-template-2.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.421444 ssm-ps-template-2.0.1/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/discovery.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.421444 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11045 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 21:28:27.000000 ssm-ps-template-2.0.1/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:28:27.421444 ssm-ps-template-2.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_discovery.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_render.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-01 21:28:14.000000 ssm-ps-template-2.0.1/tests/test_ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    11887 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9251 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11887 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-06 16:53:39.000000 ssm-ps-template-2.1.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:53:39.977205 ssm-ps-template-2.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-06 16:53:27.000000 ssm-ps-template-2.1.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-2.0.1/LICENSE.txt` & `ssm-ps-template-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/PKG-INFO` & `ssm-ps-template-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.0.1
+Version: 2.1.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -47,14 +47,16 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # SSM Parameter Store Template
 
 Command line application to render templates with data from SSM Parameter Store
 
+[![codecov](https://codecov.io/gh/gmr/ssm-ps-template/branch/main/graph/badge.svg?token=KGneS7mP9t)](https://codecov.io/gh/gmr/ssm-ps-template)
+
 ## Installation
 
 The `ssm-ps-template` application is available via the [Python Package Index](https://pypi.org/project/ssm-ps-template/) and can be installed with pip:
 
 ```bash
 pip install ssm-ps-template
 ```
@@ -162,17 +164,18 @@
 | `get_parameters_by_path` | Get a dictionary value from SSM Parameter Store                                                                                                     |
 | `urlparse`               | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
 | `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
-| Filter   | Description                         |
-|----------|-------------------------------------|
-| `toyaml` | Converts a dictionary value to YAML |
+| Filter                  | Description                                                                                                  |
+|-------------------------|--------------------------------------------------------------------------------------------------------------|
+| `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
 | `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
 
@@ -194,29 +197,32 @@
 region: us-east-1
 verbose: false
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--endpoint-url ENDPOINT_URL] [--prefix PREFIX] [--replace-underscores]
+                       [--verbose] [--version]
+                       config
 
-Templating for SSM Parameter Store
+Command line application to render templates with data from SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
-                        AWS Profile
+                        AWS Profile (default: None)
   --aws-region AWS_REGION
-                        AWS Region
-  --endpoint-url SSM_ENDPOINT_URL
-                        Specify an endpoint URL to use when contacting SSM Parameter Store.
-  --prefix PREFIX       Default SSM Key Prefix
+                        AWS Region (default: None)
+  --endpoint-url ENDPOINT_URL
+                        Specify an endpoint URL to use when contacting SSM Parameter Store. (default: None)
+  --prefix PREFIX       Default SSM Key Prefix (default: /)
   --replace-underscores
-                        Replace underscores in variable names to dashes when looking for values in SSM
+                        Replace underscores in variable names to dashes when looking for values in SSM (default: False)
   --verbose
+  --version             show program's version number and exit
 ```
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
 the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-2.0.1/README.md` & `ssm-ps-template-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SSM Parameter Store Template
 
 Command line application to render templates with data from SSM Parameter Store
 
+[![codecov](https://codecov.io/gh/gmr/ssm-ps-template/branch/main/graph/badge.svg?token=KGneS7mP9t)](https://codecov.io/gh/gmr/ssm-ps-template)
+
 ## Installation
 
 The `ssm-ps-template` application is available via the [Python Package Index](https://pypi.org/project/ssm-ps-template/) and can be installed with pip:
 
 ```bash
 pip install ssm-ps-template
 ```
@@ -113,17 +115,18 @@
 | `get_parameters_by_path` | Get a dictionary value from SSM Parameter Store                                                                                                     |
 | `urlparse`               | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
 | `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
-| Filter   | Description                         |
-|----------|-------------------------------------|
-| `toyaml` | Converts a dictionary value to YAML |
+| Filter                  | Description                                                                                                  |
+|-------------------------|--------------------------------------------------------------------------------------------------------------|
+| `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
 | `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
 
@@ -145,29 +148,32 @@
 region: us-east-1
 verbose: false
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--endpoint-url ENDPOINT_URL] [--prefix PREFIX] [--replace-underscores]
+                       [--verbose] [--version]
+                       config
 
-Templating for SSM Parameter Store
+Command line application to render templates with data from SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
-                        AWS Profile
+                        AWS Profile (default: None)
   --aws-region AWS_REGION
-                        AWS Region
-  --endpoint-url SSM_ENDPOINT_URL
-                        Specify an endpoint URL to use when contacting SSM Parameter Store.
-  --prefix PREFIX       Default SSM Key Prefix
+                        AWS Region (default: None)
+  --endpoint-url ENDPOINT_URL
+                        Specify an endpoint URL to use when contacting SSM Parameter Store. (default: None)
+  --prefix PREFIX       Default SSM Key Prefix (default: /)
   --replace-underscores
-                        Replace underscores in variable names to dashes when looking for values in SSM
+                        Replace underscores in variable names to dashes when looking for values in SSM (default: False)
   --verbose
+  --version             show program's version number and exit
 ```
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
 the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-2.0.1/pyproject.toml` & `ssm-ps-template-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "2.0.1"
+version = "2.1.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template/__main__.py` & `ssm-ps-template-2.1.0/ssm_ps_template/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,45 @@
 import time
 import typing
 from importlib import metadata
 
 from ssm_ps_template import config, discovery, render, ssm
 
 LOGGER = logging.getLogger(__name__)
+LOGGING_FORMAT = '%(message)s'
 
 
 def parse_cli_arguments(args: typing.Optional[typing.List[str]] = None) \
         -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        description='Templating for SSM Parameter Store')
-    parser.add_argument('--aws-profile', action='store', help='AWS Profile',
-                        default=os.environ.get('AWS_PROFILE'))
-    parser.add_argument('--aws-region', action='store', help='AWS Region',
-                        default=os.environ.get('AWS_REGION'))
-    parser.add_argument('--endpoint-url', action='store',
-                        help=('Specify an endpoint URL to use when contacting '
-                              'SSM Parameter Store.'),
-                        default=os.environ.get('SSM_ENDPOINT_URL'))
-    parser.add_argument('--prefix', action='store',
-                        help='Default SSM Key Prefix',
-                        default=os.environ.get('PARAMS_PREFIX', '/'))
-    parser.add_argument('--replace-underscores', action='store_true',
-                        help=('Replace underscores in variable names to dashes'
-                              ' when looking for values in SSM'))
+        description='Command line application to render templates with data '
+                    'from SSM Parameter Store',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument(
+        '--aws-profile', action='store', help='AWS Profile',
+        default=os.environ.get('AWS_PROFILE'))
+    parser.add_argument(
+        '--aws-region', action='store', help='AWS Region',
+        default=os.environ.get('AWS_REGION'))
+    parser.add_argument(
+        '--endpoint-url', action='store',
+        help=('Specify an endpoint URL to use when contacting '
+              'SSM Parameter Store.'),
+        default=os.environ.get('SSM_ENDPOINT_URL'))
+    parser.add_argument(
+        '--prefix', action='store', help='Default SSM Key Prefix',
+        default=os.environ.get('PARAMS_PREFIX', '/'))
+    parser.add_argument(
+        '--replace-underscores', action='store_true',
+        help='Replace underscores in variable names to dashes when looking '
+             'for values in SSM')
     parser.add_argument('--verbose', action='store_true')
+    parser.add_argument(
+        '--version', action='version',
+        version=f'%(prog)s {metadata.version("ssm-ps-template")}')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
     return parser.parse_args(args)
 
 
 def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
         profile=args.aws_profile or args.config[0].profile,
@@ -61,13 +71,15 @@
         LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
                     time.time() - start_time)
 
 
 def main():  # pragma: no cover
     args = parse_cli_arguments()
     verbose = args.config[0].verbose or args.verbose
-    logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
+    logging.basicConfig(
+        format=LOGGING_FORMAT,
+        level=logging.DEBUG if verbose else logging.INFO)
     for logger in ['boto3', 'botocore', 'urllib3']:
         logging.getLogger(logger).setLevel(logging.INFO)
 
     LOGGER.info('ssm-ps-template v%s', metadata.version('ssm-ps-template'))
     render_templates(args)
```

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template/config.py` & `ssm-ps-template-2.1.0/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template/discovery.py` & `ssm-ps-template-2.1.0/ssm_ps_template/discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template/render.py` & `ssm-ps-template-2.1.0/ssm_ps_template/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,54 @@
 from jinja2 import sandbox
 
 from ssm_ps_template import ssm
 
 LOGGER = logging.getLogger(__name__)
 
 
+def replace_dashes_with_underscores(value_in: typing.Union[dict, list]) \
+        -> typing.Union[dict, list]:
+    if isinstance(value_in, dict):
+        output = {}
+        for key, value in value_in.items():
+            new_key = key.replace('-', '_')
+            if isinstance(value, (dict, list)):
+                output[new_key] = replace_dashes_with_underscores(value)
+            else:
+                output[new_key] = value
+        return output
+    elif isinstance(value_in, list):
+        output = []
+        for value in value_in:
+            if isinstance(value, (dict, list)):
+                output.append(replace_dashes_with_underscores(value))
+            else:
+                output.append(value)
+        return output
+    else:
+        raise TypeError('Method invoked with incorrect data type')
+
+
 class Renderer:
 
     def __init__(self, source: pathlib.Path):
         with source.open('r') as handle:
             self._source = handle.read()
         self._values: typing.Optional[ssm.Values] = None
 
     def render(self, values: ssm.Values) -> str:
         """Render the template to the internal buffer"""
         self._values = values
         environment = sandbox.ImmutableSandboxedEnvironment()
+        environment.filters['dashes_to_underscores'] = \
+            replace_dashes_with_underscores
+        environment.filters['toyaml'] = lambda v: yaml.safe_dump(v)
         environment.globals['get_parameter'] = self._get_parameter
         environment.globals['get_parameters_by_path'] = \
             self._get_parameters_by_path
-        environment.filters['toyaml'] = lambda v: yaml.safe_dump(v)
         environment.globals['parse_qs'] = parse.parse_qs
         environment.globals['unquote'] = parse.unquote
         environment.globals['urlparse'] = parse.urlparse
         return environment.from_string(self._source).render(
             **{'environ': os.environ})
 
     def _get_parameter(self,
```

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template/ssm.py` & `ssm-ps-template-2.1.0/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-2.1.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 2.0.1
+Version: 2.1.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -47,14 +47,16 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # SSM Parameter Store Template
 
 Command line application to render templates with data from SSM Parameter Store
 
+[![codecov](https://codecov.io/gh/gmr/ssm-ps-template/branch/main/graph/badge.svg?token=KGneS7mP9t)](https://codecov.io/gh/gmr/ssm-ps-template)
+
 ## Installation
 
 The `ssm-ps-template` application is available via the [Python Package Index](https://pypi.org/project/ssm-ps-template/) and can be installed with pip:
 
 ```bash
 pip install ssm-ps-template
 ```
@@ -162,17 +164,18 @@
 | `get_parameters_by_path` | Get a dictionary value from SSM Parameter Store                                                                                                     |
 | `urlparse`               | The [`urllib.parse.urlparse`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse) function from the Python standard library. |
 | `parse_qs`               | The [`urllib.parse.parse_qs`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.parse_qs) function from the Python standard library. |
 | `unquote`                | The [`urllib.parse.unquote`](https://docs.python.org/3/library/urllib.parse.html#urllib.parse.unquote) function from the Python standard library.   |
 
 The following filters are added:
 
-| Filter   | Description                         |
-|----------|-------------------------------------|
-| `toyaml` | Converts a dictionary value to YAML |
+| Filter                  | Description                                                                                                  |
+|-------------------------|--------------------------------------------------------------------------------------------------------------|
+| `dashes_to_underscores` | Recursively replaces dashes with underscores in keys in data structures returned by `get_parameters_by_path` |
+| `toyaml`                | Converts a dictionary value to YAML                                                                          |
 
 The following variables are exposed:
 
 | Variable  | Definition                                                                                                              |
 |-----------|-------------------------------------------------------------------------------------------------------------------------|
 | `environ` | The [`os.environ`](https://docs.python.org/3/library/os.html#os.environ) dictionary for accessing environment variables |
 
@@ -194,29 +197,32 @@
 region: us-east-1
 verbose: false
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--endpoint-url ENDPOINT_URL] [--prefix PREFIX] [--replace-underscores]
+                       [--verbose] [--version]
+                       config
 
-Templating for SSM Parameter Store
+Command line application to render templates with data from SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
-                        AWS Profile
+                        AWS Profile (default: None)
   --aws-region AWS_REGION
-                        AWS Region
-  --endpoint-url SSM_ENDPOINT_URL
-                        Specify an endpoint URL to use when contacting SSM Parameter Store.
-  --prefix PREFIX       Default SSM Key Prefix
+                        AWS Region (default: None)
+  --endpoint-url ENDPOINT_URL
+                        Specify an endpoint URL to use when contacting SSM Parameter Store. (default: None)
+  --prefix PREFIX       Default SSM Key Prefix (default: /)
   --replace-underscores
-                        Replace underscores in variable names to dashes when looking for values in SSM
+                        Replace underscores in variable names to dashes when looking for values in SSM (default: False)
   --verbose
+  --version             show program's version number and exit
 ```
 Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
 the endpoint URL setting cn be set with the `SSM_ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-2.0.1/ssm_ps_template.egg-info/SOURCES.txt` & `ssm-ps-template-2.1.0/ssm_ps_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/tests/test_config.py` & `ssm-ps-template-2.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/tests/test_discovery.py` & `ssm-ps-template-2.1.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/tests/test_main.py` & `ssm-ps-template-2.1.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-2.0.1/tests/test_ssm.py` & `ssm-ps-template-2.1.0/tests/test_ssm.py`

 * *Files identical despite different names*

