# Comparing `tmp/mkjsfiddle-0.2.0.tar.gz` & `tmp/mkjsfiddle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkjsfiddle-0.2.0.tar", last modified: Wed Oct  5 07:43:03 2022, max compression
+gzip compressed data, was "mkjsfiddle-1.0.0.tar", last modified: Tue Jun  6 14:31:00 2023, max compression
```

## Comparing `mkjsfiddle-0.2.0.tar` & `mkjsfiddle-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 ianthetechie   (501) staff       (20)        0 2022-10-05 07:43:03.750431 mkjsfiddle-0.2.0/
--rw-r--r--   0 ianthetechie   (501) staff       (20)     1051 2020-02-02 01:16:18.000000 mkjsfiddle-0.2.0/LICENSE.txt
--rw-r--r--   0 ianthetechie   (501) staff       (20)     2806 2022-10-05 07:43:03.750303 mkjsfiddle-0.2.0/PKG-INFO
--rw-r--r--   0 ianthetechie   (501) staff       (20)     1932 2022-10-05 07:23:44.000000 mkjsfiddle-0.2.0/README.md
-drwxr-xr-x   0 ianthetechie   (501) staff       (20)        0 2022-10-05 07:43:03.749471 mkjsfiddle-0.2.0/mkjsfiddle/
--rw-r--r--   0 ianthetechie   (501) staff       (20)       85 2020-02-02 03:17:34.000000 mkjsfiddle-0.2.0/mkjsfiddle/__init__.py
--rw-r--r--   0 ianthetechie   (501) staff       (20)     2874 2020-02-02 02:38:55.000000 mkjsfiddle-0.2.0/mkjsfiddle/parser.py
--rw-r--r--   0 ianthetechie   (501) staff       (20)     2891 2022-10-05 07:19:06.000000 mkjsfiddle-0.2.0/mkjsfiddle/plugin.py
-drwxr-xr-x   0 ianthetechie   (501) staff       (20)        0 2022-10-05 07:43:03.750146 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/
--rw-r--r--   0 ianthetechie   (501) staff       (20)     2806 2022-10-05 07:43:03.000000 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/PKG-INFO
--rw-r--r--   0 ianthetechie   (501) staff       (20)      316 2022-10-05 07:43:03.000000 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/SOURCES.txt
--rw-r--r--   0 ianthetechie   (501) staff       (20)        1 2022-10-05 07:43:03.000000 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/dependency_links.txt
--rw-r--r--   0 ianthetechie   (501) staff       (20)       61 2022-10-05 07:43:03.000000 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/entry_points.txt
--rw-r--r--   0 ianthetechie   (501) staff       (20)       22 2022-10-05 07:43:03.000000 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/requires.txt
--rw-r--r--   0 ianthetechie   (501) staff       (20)       11 2022-10-05 07:43:03.000000 mkjsfiddle-0.2.0/mkjsfiddle.egg-info/top_level.txt
--rw-r--r--   0 ianthetechie   (501) staff       (20)      279 2020-02-02 01:26:53.000000 mkjsfiddle-0.2.0/pyproject.toml
--rw-r--r--   0 ianthetechie   (501) staff       (20)       38 2022-10-05 07:43:03.750474 mkjsfiddle-0.2.0/setup.cfg
--rw-r--r--   0 ianthetechie   (501) staff       (20)     1346 2022-10-05 07:32:54.000000 mkjsfiddle-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.863286 mkjsfiddle-1.0.0/mkjsfiddle/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/mkjsfiddle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/mkjsfiddle/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/mkjsfiddle/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 14:31:00.000000 mkjsfiddle-1.0.0/mkjsfiddle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:31:00.867286 mkjsfiddle-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-06 14:30:48.000000 mkjsfiddle-1.0.0/tests/test_parser.py
```

### Comparing `mkjsfiddle-0.2.0/LICENSE.txt` & `mkjsfiddle-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkjsfiddle-0.2.0/PKG-INFO` & `mkjsfiddle-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkjsfiddle
-Version: 0.2.0
+Version: 1.0.0
 Summary: An MkDocs plugin that lets you edit code fences in JSFiddle.
 Home-page: https://github.com/stadiamaps/mkjsfiddle
 Author: Stadia Maps
 Author-email: info@stadiamaps.com
 License: MIT
 Keywords: mkdocs jsfiddle plugin
 Classifier: Development Status :: 4 - Beta
@@ -13,23 +13,23 @@
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # MkDocs JSFiddle Plugin
 
 A plugin for [MkDocs](https://www.mkdocs.org/) that lets you
-augment your code fences with an "edit in JSFiddle" button.
+augment your code fences with an "Try it in JSFiddle" button.
 
 ## Installation
 
 This package can be installed via pip.
 
 ```
 pip install mkjsfiddle
@@ -72,10 +72,10 @@
 the HTML box, you can add `-htmlonly` to the language string (for a full string that
 looks something like `jsfiddle-html-htmlonly`).
 
 ## Known limitations
 
 We attempt to keep formatting as-is, but make no guarantees in the default mode. The
 `-htmlonly` option however should preserve formatting (if it does not, please submit
-a bug report). This has been developed and tested with the `readthedocs` style, and
-has not been tested extensively with additional styles. Pull requests to improve styling
+a bug report). This has been developed and tested with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material),
+and has not been tested extensively with additional styles. Pull requests to improve styling
 are welcome.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: mkjsfiddle Version: 0.2.0 Summary: An MkDocs plugin
+Metadata-Version: 2.1 Name: mkjsfiddle Version: 1.0.0 Summary: An MkDocs plugin
 that lets you edit code fences in JSFiddle. Home-page: https://github.com/
 stadiamaps/mkjsfiddle Author: Stadia Maps Author-email: info@stadiamaps.com
 License: MIT Keywords: mkdocs jsfiddle plugin Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
 Documentation Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown Provides-
+Requires-Python: >=3.8, <4 Description-Content-Type: text/markdown Provides-
 Extra: test License-File: LICENSE.txt # MkDocs JSFiddle Plugin A plugin for
 [MkDocs](https://www.mkdocs.org/) that lets you augment your code fences with
-an "edit in JSFiddle" button. ## Installation This package can be installed via
-pip. ``` pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins`
+an "Try it in JSFiddle" button. ## Installation This package can be installed
+via pip. ``` pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins`
 section of your `mkdocs.yml` file. ```yaml plugins: - jsfiddle ``` ## Usage
 Code fences will be left alone by default, as many code blocks may not form a
 coherent block for a user to edit. To opt in for a given code fence, add
 `jsfiddle-` to your fence language declaration, like so. ~~~markdown
 ```jsfiddle-html
   ``` ~~~ The `html` above will be preserved for syntax highlighting, and the
 `jsfiddle-` will be dropped. Other languages are theoretically supported, but
@@ -28,10 +28,11 @@
 will be extracted to the appropriate panel. If you have multiple of these, they
 will all be extracted and concatenated with some newlines thrown in as breaks.
 If you prefer to opt out of this behavior and just dump everything as-is into
 the HTML box, you can add `-htmlonly` to the language string (for a full string
 that looks something like `jsfiddle-html-htmlonly`). ## Known limitations We
 attempt to keep formatting as-is, but make no guarantees in the default mode.
 The `-htmlonly` option however should preserve formatting (if it does not,
-please submit a bug report). This has been developed and tested with the
-`readthedocs` style, and has not been tested extensively with additional
-styles. Pull requests to improve styling are welcome.
+please submit a bug report). This has been developed and tested with [Material
+for MkDocs](https://github.com/squidfunk/mkdocs-material), and has not been
+tested extensively with additional styles. Pull requests to improve styling are
+welcome.
```

### Comparing `mkjsfiddle-0.2.0/README.md` & `mkjsfiddle-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MkDocs JSFiddle Plugin
 
 A plugin for [MkDocs](https://www.mkdocs.org/) that lets you
-augment your code fences with an "edit in JSFiddle" button.
+augment your code fences with an "Try it in JSFiddle" button.
 
 ## Installation
 
 This package can be installed via pip.
 
 ```
 pip install mkjsfiddle
@@ -48,10 +48,10 @@
 the HTML box, you can add `-htmlonly` to the language string (for a full string that
 looks something like `jsfiddle-html-htmlonly`).
 
 ## Known limitations
 
 We attempt to keep formatting as-is, but make no guarantees in the default mode. The
 `-htmlonly` option however should preserve formatting (if it does not, please submit
-a bug report). This has been developed and tested with the `readthedocs` style, and
-has not been tested extensively with additional styles. Pull requests to improve styling
+a bug report). This has been developed and tested with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material),
+and has not been tested extensively with additional styles. Pull requests to improve styling
 are welcome.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # MkDocs JSFiddle Plugin A plugin for [MkDocs](https://www.mkdocs.org/) that
-lets you augment your code fences with an "edit in JSFiddle" button. ##
+lets you augment your code fences with an "Try it in JSFiddle" button. ##
 Installation This package can be installed via pip. ``` pip install mkjsfiddle
 ``` Then, add `jsfiddle` to the `plugins` section of your `mkdocs.yml` file.
 ```yaml plugins: - jsfiddle ``` ## Usage Code fences will be left alone by
 default, as many code blocks may not form a coherent block for a user to edit.
 To opt in for a given code fence, add `jsfiddle-` to your fence language
 declaration, like so. ~~~markdown ```jsfiddle-html
   ``` ~~~ The `html` above will be preserved for syntax highlighting, and the
@@ -16,10 +16,11 @@
 will be extracted to the appropriate panel. If you have multiple of these, they
 will all be extracted and concatenated with some newlines thrown in as breaks.
 If you prefer to opt out of this behavior and just dump everything as-is into
 the HTML box, you can add `-htmlonly` to the language string (for a full string
 that looks something like `jsfiddle-html-htmlonly`). ## Known limitations We
 attempt to keep formatting as-is, but make no guarantees in the default mode.
 The `-htmlonly` option however should preserve formatting (if it does not,
-please submit a bug report). This has been developed and tested with the
-`readthedocs` style, and has not been tested extensively with additional
-styles. Pull requests to improve styling are welcome.
+please submit a bug report). This has been developed and tested with [Material
+for MkDocs](https://github.com/squidfunk/mkdocs-material), and has not been
+tested extensively with additional styles. Pull requests to improve styling are
+welcome.
```

### Comparing `mkjsfiddle-0.2.0/mkjsfiddle/parser.py` & `mkjsfiddle-1.0.0/mkjsfiddle/parser.py`

 * *Files identical despite different names*

### Comparing `mkjsfiddle-0.2.0/mkjsfiddle/plugin.py` & `mkjsfiddle-1.0.0/mkjsfiddle/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       <svg width="48" height="40" stroke="#2E71FF" style="vertical-align: middle;">
         <g stroke-width="1.5" fill="none" fill-rule="evenodd">
         <path d="M23.4888889,20.543316 C21.4404656,18.4187374 19.0750303,15.6666667 16.4832014,15.6666667 C13.8721947,15.6666667 11.7555556,17.6366138 11.7555556,20.0666667 C11.7555556,22.4967196 13.8721947,24.4666667 16.4832014,24.4666667 C18.8347252,24.4666667 19.9845474,23.0125628 20.6429148,22.312473" stroke-linecap="round"></path>
         <path d="M22.5111111,19.5900174 C24.5595344,21.7145959 26.9249697,24.4666667 29.5167986,24.4666667 C32.1278053,24.4666667 34.2444444,22.4967196 34.2444444,20.0666667 C34.2444444,17.6366138 32.1278053,15.6666667 29.5167986,15.6666667 C27.1652748,15.6666667 26.0154526,17.1207706 25.3570852,17.8208603" stroke-linecap="round"></path>
         <path d="M45,22.7331459 C45,19.1499462 42.7950446,16.079593 39.6628004,14.7835315 C39.6774469,14.5246474 39.7003932,14.2674038 39.7003932,14.0035978 C39.7003932,6.82243304 33.8412885,1 26.611593,1 C21.3985635,1 16.9102123,4.03409627 14.8051788,8.41527616 C13.7828502,7.62878013 12.503719,7.15547161 11.1134367,7.15547161 C7.77825654,7.15547161 5.07450503,9.84159999 5.07450503,13.1544315 C5.07450503,13.7760488 5.16938207,14.3779791 5.3477444,14.9418479 C2.74863428,16.4787471 1,19.2867709 1,22.5105187 C1,27.3287502 4.89630545,31.2367856 9.72803666,31.31094 L36.3341301,31.3109406 C41.1201312,31.3406346 45,27.4870665 45,22.7331459 L45,22.7331459 Z" stroke-linejoin="round" />
       </g>
       </svg>
-      Edit in JSFiddle
+      Try it in JSFiddle
     </a>
     {data_fields}
 </form>
 
 ```{lang}
 {code}
 ```"""
```

### Comparing `mkjsfiddle-0.2.0/mkjsfiddle.egg-info/PKG-INFO` & `mkjsfiddle-1.0.0/mkjsfiddle.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkjsfiddle
-Version: 0.2.0
+Version: 1.0.0
 Summary: An MkDocs plugin that lets you edit code fences in JSFiddle.
 Home-page: https://github.com/stadiamaps/mkjsfiddle
 Author: Stadia Maps
 Author-email: info@stadiamaps.com
 License: MIT
 Keywords: mkdocs jsfiddle plugin
 Classifier: Development Status :: 4 - Beta
@@ -13,23 +13,23 @@
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # MkDocs JSFiddle Plugin
 
 A plugin for [MkDocs](https://www.mkdocs.org/) that lets you
-augment your code fences with an "edit in JSFiddle" button.
+augment your code fences with an "Try it in JSFiddle" button.
 
 ## Installation
 
 This package can be installed via pip.
 
 ```
 pip install mkjsfiddle
@@ -72,10 +72,10 @@
 the HTML box, you can add `-htmlonly` to the language string (for a full string that
 looks something like `jsfiddle-html-htmlonly`).
 
 ## Known limitations
 
 We attempt to keep formatting as-is, but make no guarantees in the default mode. The
 `-htmlonly` option however should preserve formatting (if it does not, please submit
-a bug report). This has been developed and tested with the `readthedocs` style, and
-has not been tested extensively with additional styles. Pull requests to improve styling
+a bug report). This has been developed and tested with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material),
+and has not been tested extensively with additional styles. Pull requests to improve styling
 are welcome.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: mkjsfiddle Version: 0.2.0 Summary: An MkDocs plugin
+Metadata-Version: 2.1 Name: mkjsfiddle Version: 1.0.0 Summary: An MkDocs plugin
 that lets you edit code fences in JSFiddle. Home-page: https://github.com/
 stadiamaps/mkjsfiddle Author: Stadia Maps Author-email: info@stadiamaps.com
 License: MIT Keywords: mkdocs jsfiddle plugin Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
 Documentation Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown Provides-
+Requires-Python: >=3.8, <4 Description-Content-Type: text/markdown Provides-
 Extra: test License-File: LICENSE.txt # MkDocs JSFiddle Plugin A plugin for
 [MkDocs](https://www.mkdocs.org/) that lets you augment your code fences with
-an "edit in JSFiddle" button. ## Installation This package can be installed via
-pip. ``` pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins`
+an "Try it in JSFiddle" button. ## Installation This package can be installed
+via pip. ``` pip install mkjsfiddle ``` Then, add `jsfiddle` to the `plugins`
 section of your `mkdocs.yml` file. ```yaml plugins: - jsfiddle ``` ## Usage
 Code fences will be left alone by default, as many code blocks may not form a
 coherent block for a user to edit. To opt in for a given code fence, add
 `jsfiddle-` to your fence language declaration, like so. ~~~markdown
 ```jsfiddle-html
   ``` ~~~ The `html` above will be preserved for syntax highlighting, and the
 `jsfiddle-` will be dropped. Other languages are theoretically supported, but
@@ -28,10 +28,11 @@
 will be extracted to the appropriate panel. If you have multiple of these, they
 will all be extracted and concatenated with some newlines thrown in as breaks.
 If you prefer to opt out of this behavior and just dump everything as-is into
 the HTML box, you can add `-htmlonly` to the language string (for a full string
 that looks something like `jsfiddle-html-htmlonly`). ## Known limitations We
 attempt to keep formatting as-is, but make no guarantees in the default mode.
 The `-htmlonly` option however should preserve formatting (if it does not,
-please submit a bug report). This has been developed and tested with the
-`readthedocs` style, and has not been tested extensively with additional
-styles. Pull requests to improve styling are welcome.
+please submit a bug report). This has been developed and tested with [Material
+for MkDocs](https://github.com/squidfunk/mkdocs-material), and has not been
+tested extensively with additional styles. Pull requests to improve styling are
+welcome.
```

### Comparing `mkjsfiddle-0.2.0/setup.py` & `mkjsfiddle-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as fp:
     long_description = fp.read()
 
 setup(
     name="mkjsfiddle",
-    version="0.2.0",
+    version="1.0.0",
     description="An MkDocs plugin that lets you edit code fences in JSFiddle.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stadiamaps/mkjsfiddle",
     author="Stadia Maps",
     author_email="info@stadiamaps.com",
     classifiers=[
@@ -27,12 +27,12 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="mkdocs jsfiddle plugin",
     license="MIT",
     packages=["mkjsfiddle"],
-    python_requires=">=3.6, <4",
+    python_requires=">=3.8, <4",
     install_requires=["mkdocs"],
     extras_require={"test": ["pytest"],},
     entry_points={"mkdocs.plugins": ["jsfiddle = mkjsfiddle.plugin:JSFiddlePlugin",],},
 )
```

