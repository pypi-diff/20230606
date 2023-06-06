# Comparing `tmp/sphinx_revealjs_slides-0.2.4.tar.gz` & `tmp/sphinx_revealjs_slides-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_revealjs_slides-0.2.4.tar", max compression
+gzip compressed data, was "sphinx_revealjs_slides-0.2.5.tar", max compression
```

## Comparing `sphinx_revealjs_slides-0.2.4.tar` & `sphinx_revealjs_slides-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,78 @@
--rw-r--r--   0        0        0       25 2023-06-06 00:14:16.589409 sphinx_revealjs_slides-0.2.4/README.md
--rw-r--r--   0        0        0      697 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2271 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/__init__.py
--rw-r--r--   0        0        0      323 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/builder.py
--rw-r--r--   0        0        0       89 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/__init__.py
--rw-r--r--   0        0        0     1082 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/_base_slide.py
--rw-r--r--   0        0        0     4082 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/incremental.py
--rw-r--r--   0        0        0     1716 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/newslide.py
--rw-r--r--   0        0        0     1257 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/speakernote.py
--rw-r--r--   0        0        0     3030 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/overridenodes.py
--rw-r--r--   0        0        0      780 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/themes/revealjs/layout.html
--rw-r--r--   0        0        0      127 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/themes/revealjs/theme.conf
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 sphinx_revealjs_slides-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-06-05 23:23:50.200187 sphinx_revealjs_slides-0.2.5/README.md
+-rw-r--r--   0        0        0      697 2023-06-06 00:29:14.675345 sphinx_revealjs_slides-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2271 2023-06-05 23:54:32.472221 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/__init__.py
+-rw-r--r--   0        0        0      323 2023-06-05 23:54:43.516358 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/builder.py
+-rw-r--r--   0        0        0       89 2023-06-05 23:54:53.625121 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/__init__.py
+-rw-r--r--   0        0        0     1082 2023-03-20 21:25:23.466424 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/_base_slide.py
+-rw-r--r--   0        0        0     4082 2023-03-20 21:30:13.522912 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/incremental.py
+-rw-r--r--   0        0        0     1716 2023-03-20 21:35:10.734100 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/newslide.py
+-rw-r--r--   0        0        0     1257 2023-03-20 21:08:06.121295 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/speakernote.py
+-rw-r--r--   0        0        0     3030 2023-05-25 23:10:58.649071 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/overridenodes.py
+-rw-r--r--   0        0        0      871 2023-06-06 00:11:14.884520 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/reset.css
+-rw-r--r--   0        0        0    46578 2023-06-06 00:11:14.884966 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/reveal.css
+-rw-r--r--   0        0        0    92046 2023-06-06 00:11:14.885865 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/reveal.esm.js
+-rw-r--r--   0        0        0   362276 2023-06-06 00:11:14.889894 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/reveal.esm.js.map
+-rw-r--r--   0        0        0    92268 2023-06-06 00:11:14.890920 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/reveal.js
+-rw-r--r--   0        0        0   362268 2023-06-06 00:11:14.893918 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/reveal.js.map
+-rw-r--r--   0        0        0     7874 2023-06-06 00:11:14.895059 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/beige.css
+-rw-r--r--   0        0        0     7223 2023-06-06 00:11:14.895310 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/black-contrast.css
+-rw-r--r--   0        0        0     7054 2023-06-06 00:11:14.895520 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/black.css
+-rw-r--r--   0        0        0     7941 2023-06-06 00:11:14.895749 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/blood.css
+-rw-r--r--   0        0        0     8081 2023-06-06 00:11:14.896013 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/dracula.css
+-rw-r--r--   0        0        0       92 2023-06-06 00:11:14.896410 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/league-gothic/LICENSE
+-rw-r--r--   0        0        0      317 2023-06-06 00:11:14.896699 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.css
+-rwxr-xr-x   0        0        0    25696 2023-06-06 00:11:14.897516 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.eot
+-rwxr-xr-x   0        0        0    64256 2023-06-06 00:11:14.899429 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.ttf
+-rwxr-xr-x   0        0        0    30764 2023-06-06 00:11:14.899868 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.woff
+-rw-r--r--   0        0        0     4632 2023-06-06 00:11:14.900233 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/LICENSE
+-rwxr-xr-x   0        0        0    75720 2023-06-06 00:11:14.900735 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-italic.eot
+-rwxr-xr-x   0        0        0   238084 2023-06-06 00:11:14.903016 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-italic.ttf
+-rwxr-xr-x   0        0        0    98556 2023-06-06 00:11:14.904071 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-italic.woff
+-rwxr-xr-x   0        0        0    88070 2023-06-06 00:11:14.904623 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-regular.eot
+-rwxr-xr-x   0        0        0   288008 2023-06-06 00:11:14.906980 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-regular.ttf
+-rwxr-xr-x   0        0        0   114324 2023-06-06 00:11:14.908635 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-regular.woff
+-rwxr-xr-x   0        0        0    89897 2023-06-06 00:11:14.909138 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibold.eot
+-rwxr-xr-x   0        0        0   284640 2023-06-06 00:11:14.911259 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibold.ttf
+-rwxr-xr-x   0        0        0   115648 2023-06-06 00:11:14.912307 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibold.woff
+-rwxr-xr-x   0        0        0    75706 2023-06-06 00:11:14.912891 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibolditalic.eot
+-rwxr-xr-x   0        0        0   240944 2023-06-06 00:11:14.914967 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibolditalic.ttf
+-rwxr-xr-x   0        0        0    98816 2023-06-06 00:11:14.915625 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibolditalic.woff
+-rw-r--r--   0        0        0     1457 2023-06-06 00:11:14.915896 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro.css
+-rw-r--r--   0        0        0     7949 2023-06-06 00:11:14.916202 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/league.css
+-rw-r--r--   0        0        0     7164 2023-06-06 00:11:14.916482 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/moon.css
+-rw-r--r--   0        0        0     7089 2023-06-06 00:11:14.916683 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/night.css
+-rw-r--r--   0        0        0     7152 2023-06-06 00:11:14.917087 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/serif.css
+-rw-r--r--   0        0        0     7289 2023-06-06 00:11:14.917401 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/simple.css
+-rw-r--r--   0        0        0     7690 2023-06-06 00:11:14.917595 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/sky.css
+-rw-r--r--   0        0        0     6918 2023-06-06 00:11:14.917772 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/solarized.css
+-rw-r--r--   0        0        0     7210 2023-06-06 00:11:14.917996 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/white-contrast.css
+-rw-r--r--   0        0        0     7024 2023-06-06 00:11:14.918211 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/white.css
+-rw-r--r--   0        0        0     7205 2023-06-06 00:11:14.918477 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/dist/theme/white_contrast_compact_verbatim_headers.css
+-rw-r--r--   0        0        0   922447 2023-06-06 00:11:14.947090 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/highlight/highlight.esm.js
+-rw-r--r--   0        0        0   922686 2023-06-06 00:11:14.948820 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/highlight/highlight.js
+-rw-r--r--   0        0        0      940 2023-06-06 00:11:14.956336 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/highlight/monokai.css
+-rw-r--r--   0        0        0    16331 2023-06-06 00:11:14.956622 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/highlight/plugin.js
+-rw-r--r--   0        0        0      947 2023-06-06 00:11:14.956818 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/highlight/zenburn.css
+-rw-r--r--   0        0        0    41059 2023-06-06 00:11:14.957439 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/markdown/markdown.esm.js
+-rw-r--r--   0        0        0    41301 2023-06-06 00:11:14.957700 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/markdown/markdown.js
+-rwxr-xr-x   0        0        0    14577 2023-06-06 00:11:14.957991 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/markdown/plugin.js
+-rwxr-xr-x   0        0        0     2574 2023-06-06 00:11:14.958284 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/math/katex.js
+-rw-r--r--   0        0        0     3038 2023-06-06 00:11:14.958575 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/math/math.esm.js
+-rw-r--r--   0        0        0     3163 2023-06-06 00:11:14.958779 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/math/math.js
+-rw-r--r--   0        0        0     2094 2023-06-06 00:11:14.958961 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/math/mathjax2.js
+-rw-r--r--   0        0        0     2216 2023-06-06 00:11:14.959157 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/math/mathjax3.js
+-rw-r--r--   0        0        0      334 2023-06-06 00:11:14.959419 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/math/plugin.js
+-rw-r--r--   0        0        0    66372 2023-06-06 00:11:14.960110 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/notes/notes.esm.js
+-rw-r--r--   0        0        0    66603 2023-06-06 00:11:14.960432 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/notes/notes.js
+-rw-r--r--   0        0        0     6656 2023-06-06 00:11:14.960696 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/notes/plugin.js
+-rw-r--r--   0        0        0    23506 2023-06-06 00:11:14.961055 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/notes/speaker-view.html
+-rw-r--r--   0        0        0     6490 2023-06-06 00:11:14.961458 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/search/plugin.js
+-rw-r--r--   0        0        0     2890 2023-06-06 00:11:14.961669 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/search/search.esm.js
+-rw-r--r--   0        0        0     3127 2023-06-06 00:11:14.961865 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/search/search.js
+-rw-r--r--   0        0        0     6779 2023-06-06 00:11:14.962242 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/zoom/plugin.js
+-rw-r--r--   0        0        0     2870 2023-06-06 00:11:14.962443 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/zoom/zoom.esm.js
+-rw-r--r--   0        0        0     3108 2023-06-06 00:11:14.962636 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin/zoom/zoom.js
+-rw-r--r--   0        0        0      780 2023-05-25 22:46:16.483520 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/revealjs/layout.html
+-rw-r--r--   0        0        0      127 2023-05-25 22:45:31.603928 sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/revealjs/theme.conf
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 sphinx_revealjs_slides-0.2.5/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 sphinx_revealjs_slides-0.2.5/PKG-INFO
```

### Comparing `sphinx_revealjs_slides-0.2.4/pyproject.toml` & `sphinx_revealjs_slides-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-revealjs-slides"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Ashley Trinh <ashley@hackbrightacademy.com>"]
 readme = "README.md"
 packages = [{ include = "sphinx_revealjs_slides", from = "src" }]
 exclude = ["src/sphinx_revealjs_slides/themes/lib/reveal.js/*"]
 include = [
   "src/sphinx_revealjs_slides/themes/lib/reveal.js/dist",
```

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/__init__.py` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/_base_slide.py` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/_base_slide.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/incremental.py` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/incremental.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/newslide.py` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/newslide.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/speakernote.py` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/directives/speakernote.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/overridenodes.py` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/overridenodes.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/themes/revealjs/layout.html` & `sphinx_revealjs_slides-0.2.5/src/sphinx_revealjs_slides/themes/revealjs/layout.html`

 * *Files identical despite different names*

