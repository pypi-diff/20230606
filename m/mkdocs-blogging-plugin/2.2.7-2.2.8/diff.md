# Comparing `tmp/mkdocs-blogging-plugin-2.2.7.tar.gz` & `tmp/mkdocs-blogging-plugin-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-blogging-plugin-2.2.7.tar", last modified: Tue Jun  6 03:21:32 2023, max compression
+gzip compressed data, was "mkdocs-blogging-plugin-2.2.8.tar", last modified: Tue Jun  6 13:09:50 2023, max compression
```

## Comparing `mkdocs-blogging-plugin-2.2.7.tar` & `mkdocs-blogging-plugin-2.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:32.170082 mkdocs-blogging-plugin-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 03:21:32.170082 mkdocs-blogging-plugin-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:32.162082 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:32.170082 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-button-theme.html
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-card-theme.html
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-tags-index.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-tags-render.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-tags.html
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog.html
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:32.166082 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 03:21:32.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 03:21:32.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 03:21:32.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 03:21:32.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 03:21:32.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 03:21:32.000000 mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 03:21:32.170082 mkdocs-blogging-plugin-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:32.170082 mkdocs-blogging-plugin-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-06 03:21:08.000000 mkdocs-blogging-plugin-2.2.7/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.400224 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-button-theme.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-card-theme.html
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-render.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/test_template.py
```

### Comparing `mkdocs-blogging-plugin-2.2.7/LICENSE` & `mkdocs-blogging-plugin-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/PKG-INFO` & `mkdocs-blogging-plugin-2.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-blogging-plugin
-Version: 2.2.7
+Version: 2.2.8
 Summary: Mkdocs plugin that generates a blog index page sorted by creation date.
 Author: Liang Yesheang
 Author-email: liang2kl@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/liang2kl/mkdocs-blogging-plugin
 Keywords: mkdocs blog plugin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-blogging-plugin-2.2.7/README.md` & `mkdocs-blogging-plugin-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/config.py` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/plugin.py` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-button-theme.html` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-button-theme.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-card-theme.html` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-card-theme.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-tags-index.html` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-index.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog-tags-render.html` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-render.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/blog.html` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/templates/pagination.js` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/pagination.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -10,48 +10,50 @@
 
 function scrollToTop() {
     setTimeout(function() {
         window.scrollTo(0, 0);
     }, 100);
 }
 
+const onButtonClick = (ele) => {
+    var current = pagination.getElementsByClassName("active");
+    if (current.length) {
+        current[0].className = current[0].className.replace(
+            " active", ""
+        );
+    }
+    ele.className += " active";
+
+    // Togglg visibility of pages
+    const destPage = parseInt(ele.textContent)
+    var pages = document.getElementsByClassName("page")
+    if (destPage && pages.length) {
+        for (var j = 0; j < pages.length; j++) {
+            const pageId = parseInt(pages[j].id.replace("page", ""))
+            if (pageId != destPage) {
+                // This is not the destination page
+                if (!pages[j].className.includes("blog-hidden")) {
+                    pages[j].className += " blog-hidden"
+                }
+            } else {
+                // This is the destination page
+                pages[j].className = pages[j].className.replace(" blog-hidden", "")
+            }
+        }
+        scrollToTop();
+    }
+};
+
 var pagination = document.getElementById("blog-pagination");
 if (pagination) {
     var links = pagination.getElementsByClassName("page-number");
     if (links.length) {
         for (var i = 0; i < links.length; i++) {
             // Toggle pagination highlight
             links[i].addEventListener("click", function() {
-                var current = pagination.getElementsByClassName("active");
-                if (current.length) {
-                    current[0].className = current[0].className.replace(
-                        " active", ""
-                    );
-                }
-                this.className += " active";
-
-                // Togglg visibility of pages
-                const destPage = parseInt(this.textContent)
-                var pages = document.getElementsByClassName("page")
-                if (destPage && pages.length) {
-                    for (var j = 0; j < pages.length; j++) {
-                        const pageId = parseInt(pages[j].id.replace("page", ""))
-                        if (pageId != destPage) {
-                            // This is not the destination page
-                            if (!pages[j].className.includes("blog-hidden")) {
-                                pages[j].className += " blog-hidden"
-                            }
-                        } else {
-                            // This is the destination page
-                            pages[j].className = pages[j].className.replace(" blog-hidden", "")
-                        }
-                    }
-                    scrollToTop();
-                }
+                onButtonClick(this);
             });
         }
         links[currentPage].className += " active"
-        if (currentPage > 0) {
-            links[currentPage].click();
-        }
+        onButtonClick(links[currentPage]);
     }
 }
```

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin/util.py` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/PKG-INFO` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-blogging-plugin
-Version: 2.2.7
+Version: 2.2.8
 Summary: Mkdocs plugin that generates a blog index page sorted by creation date.
 Author: Liang Yesheang
 Author-email: liang2kl@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/liang2kl/mkdocs-blogging-plugin
 Keywords: mkdocs blog plugin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-blogging-plugin-2.2.7/mkdocs_blogging_plugin.egg-info/SOURCES.txt` & `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/setup.py` & `mkdocs-blogging-plugin-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     LONG_DESCRIPTION = file.read()
 
 with open("requirements.txt", "r") as file:
     DEPENDENCIES = file.readlines()
 
 setup(
     name="mkdocs-blogging-plugin",
-    version="2.2.7",
+    version="2.2.8",
     description="Mkdocs plugin that generates a blog index page sorted by creation date.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="mkdocs blog plugin",
     project_urls={
         "Source": "https://github.com/liang2kl/mkdocs-blogging-plugin"
     },
```

### Comparing `mkdocs-blogging-plugin-2.2.7/tests/test_config.py` & `mkdocs-blogging-plugin-2.2.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/tests/test_format.py` & `mkdocs-blogging-plugin-2.2.8/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.7/tests/test_template.py` & `mkdocs-blogging-plugin-2.2.8/tests/test_template.py`

 * *Files identical despite different names*

