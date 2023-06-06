# Comparing `tmp/mkdocs-charts-plugin-0.0.8.tar.gz` & `tmp/mkdocs-charts-plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-charts-plugin-0.0.8.tar", last modified: Sun Feb 20 10:02:07 2022, max compression
+gzip compressed data, was "mkdocs-charts-plugin-0.0.9.tar", last modified: Tue Jun  6 11:27:36 2023, max compression
```

## Comparing `mkdocs-charts-plugin-0.0.8.tar` & `mkdocs-charts-plugin-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 10:02:07.078856 mkdocs-charts-plugin-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-02-20 10:02:07.078856 mkdocs-charts-plugin-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 10:02:07.078856 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/fences.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 10:02:07.078856 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/js/mkdocs-charts-plugin.js
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-20 10:02:07.078856 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-02-20 10:02:06.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-02-20 10:02:06.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-20 10:02:06.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-02-20 10:02:06.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-20 10:02:06.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-20 10:02:06.000000 mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-20 10:02:07.078856 mkdocs-charts-plugin-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-02-20 10:01:49.000000 mkdocs-charts-plugin-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:27:36.725497 mkdocs-charts-plugin-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-06 11:27:36.725497 mkdocs-charts-plugin-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:27:36.725497 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/fences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:27:36.725497 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/js/mkdocs-charts-plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:27:36.725497 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-06 11:27:36.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-06 11:27:36.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:27:36.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 11:27:36.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 11:27:36.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 11:27:36.000000 mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:27:36.725497 mkdocs-charts-plugin-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-06 11:27:16.000000 mkdocs-charts-plugin-0.0.9/setup.py
```

### Comparing `mkdocs-charts-plugin-0.0.8/LICENSE` & `mkdocs-charts-plugin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-charts-plugin-0.0.8/PKG-INFO` & `mkdocs-charts-plugin-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-charts-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: MkDocs plugin to add charts from data
 Home-page: https://github.com/timvink/mkdocs-charts-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,14 +29,16 @@
 
 [MkDocs](https://www.mkdocs.org/) plugin to create plots from data using the declarative [vegalite](https://vega.github.io/vega-lite/) syntax. This makes it easier to [build reproducible reports with MkDocs](https://timvink.nl/reproducible-reports-with-mkdocs/).
 
 👉 See it in action on the [demo page](https://timvink.github.io/mkdocs-charts-plugin/demo/)
 
 Includes supports for [mkdocs-material](https://github.com/squidfunk/mkdocs-material) theme features like [instant loading](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/?h=reload#instant-loading) and [dark color themes](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-palette-toggle).
 
+Do checkout the other [charting plugins for mkdocs](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins#images-tables-charts--graphs) that might suit your specific use-case better.
+
 ## Installation
 
 Install the plugin using `pip3`:
 
 ```shell
 pip3 install mkdocs-charts-plugin
 ```
@@ -91,9 +92,7 @@
 
 See the [vegalite editor](https://vega.github.io/editor/#/) for a range of examples you could copy-paste into your mkdocs site
 
 ## Documentation
 
 See the documentation [timvink.github.io/mkdocs-charts-plugin](https://timvink.github.io/mkdocs-charts-plugin/) for examples, use cases and options.
 
-
-
```

### Comparing `mkdocs-charts-plugin-0.0.8/README.md` & `mkdocs-charts-plugin-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 [MkDocs](https://www.mkdocs.org/) plugin to create plots from data using the declarative [vegalite](https://vega.github.io/vega-lite/) syntax. This makes it easier to [build reproducible reports with MkDocs](https://timvink.nl/reproducible-reports-with-mkdocs/).
 
 👉 See it in action on the [demo page](https://timvink.github.io/mkdocs-charts-plugin/demo/)
 
 Includes supports for [mkdocs-material](https://github.com/squidfunk/mkdocs-material) theme features like [instant loading](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/?h=reload#instant-loading) and [dark color themes](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-palette-toggle).
 
+Do checkout the other [charting plugins for mkdocs](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins#images-tables-charts--graphs) that might suit your specific use-case better.
+
 ## Installation
 
 Install the plugin using `pip3`:
 
 ```shell
 pip3 install mkdocs-charts-plugin
 ```
```

### Comparing `mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/fences.py` & `mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/fences.py`

 * *Files identical despite different names*

### Comparing `mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/js/mkdocs-charts-plugin.js` & `mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/js/mkdocs-charts-plugin.js`

 * *Files identical despite different names*

### Comparing `mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin/plugin.py` & `mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
-from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from mkdocs.exceptions import PluginError
+from mkdocs.plugins import BasePlugin
 from mkdocs.utils import copy_file
 
 from mkdocs_charts_plugin.fences import fence_vegalite
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
@@ -19,15 +19,14 @@
             return True
     raise PluginError(
         f"[mkdocs_charts_plugin]: Missing 'extra_javascript' dependency for {dependency}. Please see setup instructions."
     )
 
 
 class ChartsPlugin(BasePlugin):
-
     config_scheme = (
         ("data_path", config_options.Type(str, default="")),
         ("use_data_path", config_options.Type(bool, default=True)),
         ("vega_theme", config_options.Type(str, default="default")),
         ("vega_theme_dark", config_options.Type(str, default="dark")),
         ("vega_renderer", config_options.Type(str, default="svg")),
         ("vega_width", config_options.Type(str, default="container")),
@@ -37,42 +36,29 @@
     def on_config(self, config, **kwargs):
         """
         Event trigger on config.
         See https://www.mkdocs.org/user-guide/plugins/#on_config.
         """
         # Add pointer to mkdocs-charts-plugin.js
         # which is added to the output directory during on_post_build() event
-        config["extra_javascript"] = ["js/mkdocs-charts-plugin.js"] + config[
-            "extra_javascript"
-        ]
+        config["extra_javascript"] = ["js/mkdocs-charts-plugin.js"] + config["extra_javascript"]
 
         # Make sure custom fences are configured.
-        custom_fences = (
-            config.get("mdx_configs", {})
-            .get("pymdownx.superfences", {})
-            .get("custom_fences", {})
-        )
+        custom_fences = config.get("mdx_configs", {}).get("pymdownx.superfences", {}).get("custom_fences", {})
         if not custom_fences:
             raise PluginError(
                 "[mkdocs_charts_plugin]: You have not configured any custom fences, please see the setup instructions."
             )
 
         # Make sure javascript is configured
         libnames = config.get("extra_javascript", [])
         check_library(libnames, "vega")
         check_library(libnames, "vega-lite")
         check_library(libnames, "vega-embed")
 
-    def on_page_content(self, html, page, config, files, **kwargs):
-        """
-        Store reference to homepage
-        """
-        if page.is_homepage:
-            self.homepage = page.file
-
     def on_post_page(self, output, page, config, **kwargs):
         """
         Insert plugin config as javascript variables into the page.
         """
         # Early return if not necessary
         if "vegalite" not in output:
             return output
@@ -97,17 +83,19 @@
         """
         Each page might be in a different location.
 
         Determine path to root and add to html of page as a JS variable.
         """
         plugin_config = self.config.copy()
 
-        # Find path to homepage
-        path_to_homepage = self.homepage.url_relative_to(page.file)
-        path_to_homepage = os.path.dirname(path_to_homepage)
+        # Find the path to the homepage
+        docs_directory = config["docs_dir"]
+        page_path = os.path.join(docs_directory, page.file.src_uri)
+        path_to_homepage = os.path.relpath(docs_directory, os.path.dirname(page_path))
+
         if config.get("use_directory_urls"):
             path_to_homepage = os.path.join("..", path_to_homepage)
         plugin_config["path_to_homepage"] = path_to_homepage
 
         # ensure plugin config is string
         plugin_config["use_data_path"] = str(plugin_config["use_data_path"])
```

### Comparing `mkdocs-charts-plugin-0.0.8/mkdocs_charts_plugin.egg-info/PKG-INFO` & `mkdocs-charts-plugin-0.0.9/mkdocs_charts_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-charts-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: MkDocs plugin to add charts from data
 Home-page: https://github.com/timvink/mkdocs-charts-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,14 +29,16 @@
 
 [MkDocs](https://www.mkdocs.org/) plugin to create plots from data using the declarative [vegalite](https://vega.github.io/vega-lite/) syntax. This makes it easier to [build reproducible reports with MkDocs](https://timvink.nl/reproducible-reports-with-mkdocs/).
 
 👉 See it in action on the [demo page](https://timvink.github.io/mkdocs-charts-plugin/demo/)
 
 Includes supports for [mkdocs-material](https://github.com/squidfunk/mkdocs-material) theme features like [instant loading](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/?h=reload#instant-loading) and [dark color themes](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-palette-toggle).
 
+Do checkout the other [charting plugins for mkdocs](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins#images-tables-charts--graphs) that might suit your specific use-case better.
+
 ## Installation
 
 Install the plugin using `pip3`:
 
 ```shell
 pip3 install mkdocs-charts-plugin
 ```
@@ -91,9 +92,7 @@
 
 See the [vegalite editor](https://vega.github.io/editor/#/) for a range of examples you could copy-paste into your mkdocs site
 
 ## Documentation
 
 See the documentation [timvink.github.io/mkdocs-charts-plugin](https://timvink.github.io/mkdocs-charts-plugin/) for examples, use cases and options.
 
-
-
```

### Comparing `mkdocs-charts-plugin-0.0.8/setup.py` & `mkdocs-charts-plugin-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-charts-plugin",
-    version="0.0.8",
+    version="0.0.9",
     description="MkDocs plugin to add charts from data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin",
     url="https://github.com/timvink/mkdocs-charts-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

