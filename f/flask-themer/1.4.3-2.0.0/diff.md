# Comparing `tmp/flask-themer-1.4.3.tar.gz` & `tmp/flask-themer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-themer-1.4.3.tar", last modified: Sat Sep 11 00:17:08 2021, max compression
+gzip compressed data, was "flask-themer-2.0.0.tar", last modified: Tue Jun  6 05:05:43 2023, max compression
```

## Comparing `flask-themer-1.4.3.tar` & `flask-themer-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 00:17:08.000000 flask-themer-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     6608 2021-09-11 00:17:08.000000 flask-themer-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2021-09-11 00:16:53.000000 flask-themer-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 00:17:08.000000 flask-themer-1.4.3/flask_themer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6608 2021-09-11 00:17:08.000000 flask-themer-1.4.3/flask_themer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-09-11 00:17:08.000000 flask-themer-1.4.3/flask_themer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-11 00:17:08.000000 flask-themer-1.4.3/flask_themer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-11 00:17:08.000000 flask-themer-1.4.3/flask_themer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-11 00:17:08.000000 flask-themer-1.4.3/flask_themer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7773 2021-09-11 00:16:53.000000 flask-themer-1.4.3/flask_themer.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-11 00:17:08.000000 flask-themer-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-09-11 00:16:53.000000 flask-themer-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:05:43.832616 flask-themer-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 05:05:30.000000 flask-themer-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-06 05:05:43.832616 flask-themer-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-06 05:05:30.000000 flask-themer-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:05:43.832616 flask-themer-2.0.0/flask_themer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-06 05:05:43.000000 flask-themer-2.0.0/flask_themer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-06 05:05:43.000000 flask-themer-2.0.0/flask_themer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:05:43.000000 flask-themer-2.0.0/flask_themer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 05:05:43.000000 flask-themer-2.0.0/flask_themer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 05:05:43.000000 flask-themer-2.0.0/flask_themer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-06 05:05:30.000000 flask-themer-2.0.0/flask_themer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 05:05:43.832616 flask-themer-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-06 05:05:30.000000 flask-themer-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flask-themer-1.4.3/PKG-INFO` & `flask-themer-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-themer
-Version: 1.4.3
+Version: 2.0.0
 Summary: Simple theme mechanism for Flask
 Home-page: https://github.com/tktech/flask-themer
 Author: Tyler Kennedy
 Author-email: tk@tkte.ch
 License: UNKNOWN
 Description: ![PyPI](https://img.shields.io/pypi/v/flask-themer?style=flat-square)
         ![PyPI - License](https://img.shields.io/pypi/l/flask-themer?style=flat-square)
@@ -12,45 +12,44 @@
         
         
         # Flask-Themer
         
         Simple theme support for flask apps.
         
         Flask-Themer is inspired by the (seemingly) abandoned [flask-themes][] project,
-        but has been written from scratch for py3.7+ (or 3.6 with the dataclasses
-        backport). However it is _not_ immediately compatible with flask-themes and
-        does not seek to be. Flask-Themer tries to have little opinion on how you
-        actually structure your project and its themes and does not require a
-        particular metadata format/file.
+        but has been written from scratch for Python 3.8+. However, it is _not_ immediately
+        compatible with flask-themes and does not seek to be. Flask-Themer tries to have
+        little opinion on how you actually structure your project and its themes and does
+        not require a particular metadata format/file.
         
         Flask-Themer releases follow [Semantic Versioning][semver].
         Flask-Themer has 100% test coverage and considers it an error to fall below
         100%.
         
         ## Installation
         
         Install the latest release from [PyPi][]:
         
         ```
         pip install flask-themer
         ```
         
-        or get the latest development version from github:
+        or get the latest development version from GitHub:
         
         ```
         git clone https://github.com/TkTech/flask-themer.git
         cd flask-themer
         python setup.py develop
         ```
         
         ## Quickstart
         
         
         Flask-Themer usage is usually very basic, and once setup you likely won't need
-        to touch it again. Lets do a quickstart. Notice how we import `render_template`
+        to touch it again. Let's do a quickstart. Notice how we import `render_template`
         from `flask_themer` instead of `flask`.
         
         
         Our `app.py` looks like this:
         
         ```python
         from flask import Flask
@@ -108,14 +107,21 @@
         
         {% block header %}
             {{ super() }}
             <link rel="stylesheet" href="{{ theme_static("bootstrap.css") }}">
         {% endblock %}
         ```
         
+        Themes can also extend other themes using the `theme` argument:
+        
+        ```jinja2
+        {% extends theme("base.html", theme="my_parent_theme") %}
+        ```
+        
+        
         ## Theme Loaders
         
         _Theme_ loaders are the mechanism by which Flask-Themer discovers what themes
         are available. You can create a custom loader to get themes from a ZIP file, or
         a database for example. Usually if you create a new `ThemeLoader` you'll also
         need to create a new Jinja [_template_ loader][loader] so Jinja knows how to
         read individual templates. Lets do a very minimal example that loads just a
@@ -175,9 +181,9 @@
         [loader]: https://jinja.palletsprojects.com/en/latest/api/#loaders
         
 Keywords: flask,themes,jinja2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `flask-themer-1.4.3/README.md` & `flask-themer-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,45 +4,44 @@
 
 
 # Flask-Themer
 
 Simple theme support for flask apps.
 
 Flask-Themer is inspired by the (seemingly) abandoned [flask-themes][] project,
-but has been written from scratch for py3.7+ (or 3.6 with the dataclasses
-backport). However it is _not_ immediately compatible with flask-themes and
-does not seek to be. Flask-Themer tries to have little opinion on how you
-actually structure your project and its themes and does not require a
-particular metadata format/file.
+but has been written from scratch for Python 3.8+. However, it is _not_ immediately
+compatible with flask-themes and does not seek to be. Flask-Themer tries to have
+little opinion on how you actually structure your project and its themes and does
+not require a particular metadata format/file.
 
 Flask-Themer releases follow [Semantic Versioning][semver].
 Flask-Themer has 100% test coverage and considers it an error to fall below
 100%.
 
 ## Installation
 
 Install the latest release from [PyPi][]:
 
 ```
 pip install flask-themer
 ```
 
-or get the latest development version from github:
+or get the latest development version from GitHub:
 
 ```
 git clone https://github.com/TkTech/flask-themer.git
 cd flask-themer
 python setup.py develop
 ```
 
 ## Quickstart
 
 
 Flask-Themer usage is usually very basic, and once setup you likely won't need
-to touch it again. Lets do a quickstart. Notice how we import `render_template`
+to touch it again. Let's do a quickstart. Notice how we import `render_template`
 from `flask_themer` instead of `flask`.
 
 
 Our `app.py` looks like this:
 
 ```python
 from flask import Flask
@@ -100,14 +99,21 @@
 
 {% block header %}
     {{ super() }}
     <link rel="stylesheet" href="{{ theme_static("bootstrap.css") }}">
 {% endblock %}
 ```
 
+Themes can also extend other themes using the `theme` argument:
+
+```jinja2
+{% extends theme("base.html", theme="my_parent_theme") %}
+```
+
+
 ## Theme Loaders
 
 _Theme_ loaders are the mechanism by which Flask-Themer discovers what themes
 are available. You can create a custom loader to get themes from a ZIP file, or
 a database for example. Usually if you create a new `ThemeLoader` you'll also
 need to create a new Jinja [_template_ loader][loader] so Jinja knows how to
 read individual templates. Lets do a very minimal example that loads just a
```

### Comparing `flask-themer-1.4.3/flask_themer.egg-info/PKG-INFO` & `flask-themer-2.0.0/flask_themer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-themer
-Version: 1.4.3
+Version: 2.0.0
 Summary: Simple theme mechanism for Flask
 Home-page: https://github.com/tktech/flask-themer
 Author: Tyler Kennedy
 Author-email: tk@tkte.ch
 License: UNKNOWN
 Description: ![PyPI](https://img.shields.io/pypi/v/flask-themer?style=flat-square)
         ![PyPI - License](https://img.shields.io/pypi/l/flask-themer?style=flat-square)
@@ -12,45 +12,44 @@
         
         
         # Flask-Themer
         
         Simple theme support for flask apps.
         
         Flask-Themer is inspired by the (seemingly) abandoned [flask-themes][] project,
-        but has been written from scratch for py3.7+ (or 3.6 with the dataclasses
-        backport). However it is _not_ immediately compatible with flask-themes and
-        does not seek to be. Flask-Themer tries to have little opinion on how you
-        actually structure your project and its themes and does not require a
-        particular metadata format/file.
+        but has been written from scratch for Python 3.8+. However, it is _not_ immediately
+        compatible with flask-themes and does not seek to be. Flask-Themer tries to have
+        little opinion on how you actually structure your project and its themes and does
+        not require a particular metadata format/file.
         
         Flask-Themer releases follow [Semantic Versioning][semver].
         Flask-Themer has 100% test coverage and considers it an error to fall below
         100%.
         
         ## Installation
         
         Install the latest release from [PyPi][]:
         
         ```
         pip install flask-themer
         ```
         
-        or get the latest development version from github:
+        or get the latest development version from GitHub:
         
         ```
         git clone https://github.com/TkTech/flask-themer.git
         cd flask-themer
         python setup.py develop
         ```
         
         ## Quickstart
         
         
         Flask-Themer usage is usually very basic, and once setup you likely won't need
-        to touch it again. Lets do a quickstart. Notice how we import `render_template`
+        to touch it again. Let's do a quickstart. Notice how we import `render_template`
         from `flask_themer` instead of `flask`.
         
         
         Our `app.py` looks like this:
         
         ```python
         from flask import Flask
@@ -108,14 +107,21 @@
         
         {% block header %}
             {{ super() }}
             <link rel="stylesheet" href="{{ theme_static("bootstrap.css") }}">
         {% endblock %}
         ```
         
+        Themes can also extend other themes using the `theme` argument:
+        
+        ```jinja2
+        {% extends theme("base.html", theme="my_parent_theme") %}
+        ```
+        
+        
         ## Theme Loaders
         
         _Theme_ loaders are the mechanism by which Flask-Themer discovers what themes
         are available. You can create a custom loader to get themes from a ZIP file, or
         a database for example. Usually if you create a new `ThemeLoader` you'll also
         need to create a new Jinja [_template_ loader][loader] so Jinja knows how to
         read individual templates. Lets do a very minimal example that loads just a
@@ -175,9 +181,9 @@
         [loader]: https://jinja.palletsprojects.com/en/latest/api/#loaders
         
 Keywords: flask,themes,jinja2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `flask-themer-1.4.3/flask_themer.py` & `flask-themer-2.0.0/flask_themer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 from dataclasses import dataclass, field
-from typing import Iterable, Callable, Union
+from typing import Iterable, Callable, Optional, Union
 from contextlib import contextmanager
 
 from flask import render_template as flask_render_template
 from flask import current_app, Blueprint, url_for, send_from_directory, abort
 from jinja2 import TemplateNotFound
 from jinja2.loaders import BaseLoader, FileSystemLoader
 
@@ -62,15 +62,15 @@
 
 
 class FileSystemThemeLoader(ThemeLoader):
     """A simple theme loader that assumes all sub-directories immediately under
     `path` are themes.
     """
     def __init__(self, path: Union[Path, str],
-                 filter: Callable[[Path], bool] = None):
+                 filter: Optional[Callable[[Path], bool]] = None):
         #: The path the loader is searching for themes.
         self.path = Path(path)
         self._filter = filter
 
     @property
     def themes(self):
         themes = {}
@@ -162,27 +162,29 @@
     """
     try:
         return flask_render_template(lookup_theme_path(path), *args, **kwargs)
     except TemplateNotFound:
         return flask_render_template(path, *args, **kwargs)
 
 
-def lookup_theme_path(path):
+def lookup_theme_path(path, theme=None):
     """Given the path to a template, lookup the "real" path after resolving the
     active theme.
     """
     themer = _current_themer()
-    return f'{MAGIC_PATH_PREFIX}/{themer.current_theme}/{path}'
+    theme = theme or themer.current_theme
+    return f'{MAGIC_PATH_PREFIX}/{theme}/{path}'
 
 
-def lookup_static_theme_path(path, **kwargs):
+def lookup_static_theme_path(path, theme=None, **kwargs):
     themer = _current_themer()
+    theme = theme or themer.current_theme
     return url_for(
         f'{MAGIC_PATH_PREFIX}.static',
-        theme=themer.current_theme,
+        theme=theme,
         filename=path,
         **kwargs
     )
 
 
 @contextmanager
 def use_theme(theme):
```

### Comparing `flask-themer-1.4.3/setup.py` & `flask-themer-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='flask-themer',
-    version='1.4.3',
+    version='2.0.0',
     description='Simple theme mechanism for Flask',
     author='Tyler Kennedy',
     author_email='tk@tkte.ch',
     url='https://github.com/tktech/flask-themer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=['flask_themer'],
@@ -21,14 +21,14 @@
         'pytest-cov'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     keywords=[
         'flask',
         'themes',
         'jinja2'
     ]
 )
```

