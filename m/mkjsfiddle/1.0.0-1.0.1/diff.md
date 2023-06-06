# Comparing `tmp/mkjsfiddle-1.0.0.tar.gz` & `tmp/mkjsfiddle-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkjsfiddle-1.0.0.tar", last modified: Tue Jun  6 14:31:00 2023, max compression
+gzip compressed data, was "mkjsfiddle-1.0.1.tar", last modified: Tue Jun  6 14:36:20 2023, max compression
```

## Comparing `mkjsfiddle-1.0.0.tar` & `mkjsfiddle-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.863286 mkjsfiddle-1.0.0/mkjsfiddle/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/mkjsfiddle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/mkjsfiddle/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/mkjsfiddle/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:20.121896 mkjsfiddle-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-06 14:36:20.121896 mkjsfiddle-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:20.121896 mkjsfiddle-1.0.1/mkjsfiddle/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/mkjsfiddle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/mkjsfiddle/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/mkjsfiddle/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:20.121896 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-06 14:36:20.000000 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-06 14:36:20.000000 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:36:20.000000 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 14:36:20.000000 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 14:36:20.000000 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 14:36:20.000000 mkjsfiddle-1.0.1/mkjsfiddle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:36:20.121896 mkjsfiddle-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:36:20.121896 mkjsfiddle-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-06 14:36:09.000000 mkjsfiddle-1.0.1/tests/test_parser.py
```

### Comparing `mkjsfiddle-1.0.0/LICENSE.txt` & `mkjsfiddle-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkjsfiddle-1.0.0/PKG-INFO` & `mkjsfiddle-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mkjsfiddle
-Version: 1.0.0
+Version: 1.0.1
 Summary: An MkDocs plugin that lets you edit code fences in JSFiddle.
 Home-page: https://github.com/stadiamaps/mkjsfiddle
 Author: Stadia Maps
 Author-email: info@stadiamaps.com
 License: MIT
 Keywords: mkdocs jsfiddle plugin
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1 Name: mkjsfiddle Version: 1.0.0 Summary: An MkDocs plugin
+Metadata-Version: 2.1 Name: mkjsfiddle Version: 1.0.1 Summary: An MkDocs plugin
 that lets you edit code fences in JSFiddle. Home-page: https://github.com/
 stadiamaps/mkjsfiddle Author: Stadia Maps Author-email: info@stadiamaps.com
 License: MIT Keywords: mkdocs jsfiddle plugin Classifier: Development Status ::
-4 - Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
-Documentation Classifier: Topic :: Software Development :: Documentation
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <4 Description-Content-Type: text/markdown Provides-
-Extra: test License-File: LICENSE.txt # MkDocs JSFiddle Plugin A plugin for
-[MkDocs](https://www.mkdocs.org/) that lets you augment your code fences with
-an "Try it in JSFiddle" button. ## Installation This package can be installed
-via pip. ``` pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins`
-section of your `mkdocs.yml` file. ```yaml plugins: - jsfiddle ``` ## Usage
-Code fences will be left alone by default, as many code blocks may not form a
-coherent block for a user to edit. To opt in for a given code fence, add
-`jsfiddle-` to your fence language declaration, like so. ~~~markdown
-```jsfiddle-html
+5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Topic :: Documentation Classifier: Topic :: Software Development ::
+Documentation Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.8, <4 Description-Content-Type: text/markdown Provides-Extra: test
+License-File: LICENSE.txt # MkDocs JSFiddle Plugin A plugin for [MkDocs](https:
+//www.mkdocs.org/) that lets you augment your code fences with an "Try it in
+JSFiddle" button. ## Installation This package can be installed via pip. ```
+pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins` section of
+your `mkdocs.yml` file. ```yaml plugins: - jsfiddle ``` ## Usage Code fences
+will be left alone by default, as many code blocks may not form a coherent
+block for a user to edit. To opt in for a given code fence, add `jsfiddle-` to
+your fence language declaration, like so. ~~~markdown ```jsfiddle-html
   ``` ~~~ The `html` above will be preserved for syntax highlighting, and the
 `jsfiddle-` will be dropped. Other languages are theoretically supported, but
 will have no impact besides code highlighting. The default behavior is for a
 simple HTML parser to extract the inline JS and CSS elements and put their
 contents in the appropriate JSFiddle panels. More specifically, if you have a
 `script` tag with the attribute `type=text/javascript` AND not having the `src`
 attribute, or if you have a `style` tag with the attribute `type=text/css`, it
```

### Comparing `mkjsfiddle-1.0.0/README.md` & `mkjsfiddle-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mkjsfiddle-1.0.0/mkjsfiddle/parser.py` & `mkjsfiddle-1.0.1/mkjsfiddle/parser.py`

 * *Files identical despite different names*

### Comparing `mkjsfiddle-1.0.0/mkjsfiddle/plugin.py` & `mkjsfiddle-1.0.1/mkjsfiddle/plugin.py`

 * *Files identical despite different names*

### Comparing `mkjsfiddle-1.0.0/mkjsfiddle.egg-info/PKG-INFO` & `mkjsfiddle-1.0.1/mkjsfiddle.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mkjsfiddle
-Version: 1.0.0
+Version: 1.0.1
 Summary: An MkDocs plugin that lets you edit code fences in JSFiddle.
 Home-page: https://github.com/stadiamaps/mkjsfiddle
 Author: Stadia Maps
 Author-email: info@stadiamaps.com
 License: MIT
 Keywords: mkdocs jsfiddle plugin
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1 Name: mkjsfiddle Version: 1.0.0 Summary: An MkDocs plugin
+Metadata-Version: 2.1 Name: mkjsfiddle Version: 1.0.1 Summary: An MkDocs plugin
 that lets you edit code fences in JSFiddle. Home-page: https://github.com/
 stadiamaps/mkjsfiddle Author: Stadia Maps Author-email: info@stadiamaps.com
 License: MIT Keywords: mkdocs jsfiddle plugin Classifier: Development Status ::
-4 - Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
-Documentation Classifier: Topic :: Software Development :: Documentation
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <4 Description-Content-Type: text/markdown Provides-
-Extra: test License-File: LICENSE.txt # MkDocs JSFiddle Plugin A plugin for
-[MkDocs](https://www.mkdocs.org/) that lets you augment your code fences with
-an "Try it in JSFiddle" button. ## Installation This package can be installed
-via pip. ``` pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins`
-section of your `mkdocs.yml` file. ```yaml plugins: - jsfiddle ``` ## Usage
-Code fences will be left alone by default, as many code blocks may not form a
-coherent block for a user to edit. To opt in for a given code fence, add
-`jsfiddle-` to your fence language declaration, like so. ~~~markdown
-```jsfiddle-html
+5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Topic :: Documentation Classifier: Topic :: Software Development ::
+Documentation Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.8, <4 Description-Content-Type: text/markdown Provides-Extra: test
+License-File: LICENSE.txt # MkDocs JSFiddle Plugin A plugin for [MkDocs](https:
+//www.mkdocs.org/) that lets you augment your code fences with an "Try it in
+JSFiddle" button. ## Installation This package can be installed via pip. ```
+pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins` section of
+your `mkdocs.yml` file. ```yaml plugins: - jsfiddle ``` ## Usage Code fences
+will be left alone by default, as many code blocks may not form a coherent
+block for a user to edit. To opt in for a given code fence, add `jsfiddle-` to
+your fence language declaration, like so. ~~~markdown ```jsfiddle-html
   ``` ~~~ The `html` above will be preserved for syntax highlighting, and the
 `jsfiddle-` will be dropped. Other languages are theoretically supported, but
 will have no impact besides code highlighting. The default behavior is for a
 simple HTML parser to extract the inline JS and CSS elements and put their
 contents in the appropriate JSFiddle panels. More specifically, if you have a
 `script` tag with the attribute `type=text/javascript` AND not having the `src`
 attribute, or if you have a `style` tag with the attribute `type=text/css`, it
```

### Comparing `mkjsfiddle-1.0.0/setup.py` & `mkjsfiddle-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as fp:
     long_description = fp.read()
 
 setup(
     name="mkjsfiddle",
-    version="1.0.0",
+    version="1.0.1",
     description="An MkDocs plugin that lets you edit code fences in JSFiddle.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stadiamaps/mkjsfiddle",
     author="Stadia Maps",
     author_email="info@stadiamaps.com",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Documentation",
         "Topic :: Software Development :: Documentation",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="mkdocs jsfiddle plugin",
     license="MIT",
     packages=["mkjsfiddle"],
```

### Comparing `mkjsfiddle-1.0.0/tests/test_parser.py` & `mkjsfiddle-1.0.1/tests/test_parser.py`

 * *Files identical despite different names*

