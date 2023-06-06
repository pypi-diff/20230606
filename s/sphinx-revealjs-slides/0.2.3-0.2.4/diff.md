# Comparing `tmp/sphinx_revealjs_slides-0.2.3.tar.gz` & `tmp/sphinx_revealjs_slides-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_revealjs_slides-0.2.3.tar", max compression
+gzip compressed data, was "sphinx_revealjs_slides-0.2.4.tar", max compression
```

## Comparing `sphinx_revealjs_slides-0.2.3.tar` & `sphinx_revealjs_slides-0.2.4.tar`

### file list

```diff
@@ -1,78 +1,13 @@
--rw-r--r--   0        0        0       17 2023-05-24 17:21:32.490960 sphinx_revealjs_slides-0.2.3/README.md
--rw-r--r--   0        0        0      669 2023-06-05 23:22:32.090105 sphinx_revealjs_slides-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2264 2023-05-30 20:18:00.440100 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/__init__.py
--rw-r--r--   0        0        0      316 2023-05-30 20:15:36.390643 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/builder.py
--rw-r--r--   0        0        0       82 2023-05-24 17:17:43.845387 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/__init__.py
--rw-r--r--   0        0        0     1082 2023-03-20 21:25:23.466424 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/_base_slide.py
--rw-r--r--   0        0        0     4082 2023-03-20 21:30:13.522912 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/incremental.py
--rw-r--r--   0        0        0     1716 2023-03-20 21:35:10.734100 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/newslide.py
--rw-r--r--   0        0        0     1257 2023-03-20 21:08:06.121295 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/speakernote.py
--rw-r--r--   0        0        0     3030 2023-05-25 23:10:58.649071 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/overridenodes.py
--rw-r--r--   0        0        0      871 2023-05-30 20:16:18.060732 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/reset.css
--rw-r--r--   0        0        0    46578 2023-05-30 20:16:18.061571 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/reveal.css
--rw-r--r--   0        0        0    92046 2023-05-30 20:16:18.063030 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/reveal.esm.js
--rw-r--r--   0        0        0   362276 2023-05-30 20:16:18.065700 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/reveal.esm.js.map
--rw-r--r--   0        0        0    92268 2023-05-30 20:16:18.066463 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/reveal.js
--rw-r--r--   0        0        0   362268 2023-05-30 20:16:18.068691 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/reveal.js.map
--rw-r--r--   0        0        0     7874 2023-05-30 20:16:18.069066 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/beige.css
--rw-r--r--   0        0        0     7223 2023-05-30 20:16:18.069242 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/black-contrast.css
--rw-r--r--   0        0        0     7054 2023-05-30 20:16:18.069400 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/black.css
--rw-r--r--   0        0        0     7941 2023-05-30 20:16:18.069543 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/blood.css
--rw-r--r--   0        0        0     8081 2023-05-30 20:16:18.069688 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/dracula.css
--rw-r--r--   0        0        0       92 2023-05-30 20:16:18.070004 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/league-gothic/LICENSE
--rw-r--r--   0        0        0      317 2023-05-30 20:16:18.070174 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.css
--rwxr-xr-x   0        0        0    25696 2023-05-30 20:16:18.070729 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.eot
--rwxr-xr-x   0        0        0    64256 2023-05-30 20:16:18.071597 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.ttf
--rwxr-xr-x   0        0        0    30764 2023-05-30 20:16:18.072254 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/league-gothic/league-gothic.woff
--rw-r--r--   0        0        0     4632 2023-05-30 20:16:18.072565 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/LICENSE
--rwxr-xr-x   0        0        0    75720 2023-05-30 20:16:18.073519 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-italic.eot
--rwxr-xr-x   0        0        0   238084 2023-05-30 20:16:18.075317 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-italic.ttf
--rwxr-xr-x   0        0        0    98556 2023-05-30 20:16:18.076384 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-italic.woff
--rwxr-xr-x   0        0        0    88070 2023-05-30 20:16:18.076758 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-regular.eot
--rwxr-xr-x   0        0        0   288008 2023-05-30 20:16:18.078651 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-regular.ttf
--rwxr-xr-x   0        0        0   114324 2023-05-30 20:16:18.080884 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-regular.woff
--rwxr-xr-x   0        0        0    89897 2023-05-30 20:16:18.081903 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibold.eot
--rwxr-xr-x   0        0        0   284640 2023-05-30 20:16:18.084351 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibold.ttf
--rwxr-xr-x   0        0        0   115648 2023-05-30 20:16:18.085020 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibold.woff
--rwxr-xr-x   0        0        0    75706 2023-05-30 20:16:18.086139 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibolditalic.eot
--rwxr-xr-x   0        0        0   240944 2023-05-30 20:16:18.088431 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibolditalic.ttf
--rwxr-xr-x   0        0        0    98816 2023-05-30 20:16:18.089060 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro-semibolditalic.woff
--rw-r--r--   0        0        0     1457 2023-05-30 20:16:18.089326 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/fonts/source-sans-pro/source-sans-pro.css
--rw-r--r--   0        0        0     7949 2023-05-30 20:16:18.089454 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/league.css
--rw-r--r--   0        0        0     7164 2023-05-30 20:16:18.089621 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/moon.css
--rw-r--r--   0        0        0     7089 2023-05-30 20:16:18.089742 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/night.css
--rw-r--r--   0        0        0     7152 2023-05-30 20:16:18.089877 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/serif.css
--rw-r--r--   0        0        0     7289 2023-05-30 20:16:18.091469 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/simple.css
--rw-r--r--   0        0        0     7690 2023-05-30 20:16:18.091629 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/sky.css
--rw-r--r--   0        0        0     6918 2023-05-30 20:16:18.092532 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/solarized.css
--rw-r--r--   0        0        0     7210 2023-05-30 20:16:18.092811 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/white-contrast.css
--rw-r--r--   0        0        0     7024 2023-05-30 20:16:18.092989 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/white.css
--rw-r--r--   0        0        0     7205 2023-05-30 20:16:18.093701 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/dist/theme/white_contrast_compact_verbatim_headers.css
--rw-r--r--   0        0        0   922447 2023-05-30 20:16:18.115506 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/highlight/highlight.esm.js
--rw-r--r--   0        0        0   922686 2023-05-30 20:16:18.117187 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/highlight/highlight.js
--rw-r--r--   0        0        0      940 2023-05-30 20:16:18.118321 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/highlight/monokai.css
--rw-r--r--   0        0        0    16331 2023-05-30 20:16:18.118603 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/highlight/plugin.js
--rw-r--r--   0        0        0      947 2023-05-30 20:16:18.118799 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/highlight/zenburn.css
--rw-r--r--   0        0        0    41059 2023-05-30 20:16:18.119497 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/markdown/markdown.esm.js
--rw-r--r--   0        0        0    41301 2023-05-30 20:16:18.119779 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/markdown/markdown.js
--rwxr-xr-x   0        0        0    14577 2023-05-30 20:16:18.120066 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/markdown/plugin.js
--rwxr-xr-x   0        0        0     2574 2023-05-30 20:16:18.120437 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/math/katex.js
--rw-r--r--   0        0        0     3038 2023-05-30 20:16:18.120664 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/math/math.esm.js
--rw-r--r--   0        0        0     3163 2023-05-30 20:16:18.120880 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/math/math.js
--rw-r--r--   0        0        0     2094 2023-05-30 20:16:18.121063 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/math/mathjax2.js
--rw-r--r--   0        0        0     2216 2023-05-30 20:16:18.121249 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/math/mathjax3.js
--rw-r--r--   0        0        0      334 2023-05-30 20:16:18.121435 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/math/plugin.js
--rw-r--r--   0        0        0    66372 2023-05-30 20:16:18.122294 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/notes/notes.esm.js
--rw-r--r--   0        0        0    66603 2023-05-30 20:16:18.122642 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/notes/notes.js
--rw-r--r--   0        0        0     6656 2023-05-30 20:16:18.123014 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/notes/plugin.js
--rw-r--r--   0        0        0    23506 2023-05-30 20:16:18.123315 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/notes/speaker-view.html
--rw-r--r--   0        0        0     6490 2023-05-30 20:16:18.123673 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/search/plugin.js
--rw-r--r--   0        0        0     2890 2023-05-30 20:16:18.123885 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/search/search.esm.js
--rw-r--r--   0        0        0     3127 2023-05-30 20:16:18.124073 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/search/search.js
--rw-r--r--   0        0        0     6779 2023-05-30 20:16:18.124380 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/zoom/plugin.js
--rw-r--r--   0        0        0     2870 2023-05-30 20:16:18.124594 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/zoom/zoom.esm.js
--rw-r--r--   0        0        0     3108 2023-05-30 20:16:18.124781 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/lib/reveal.js/plugin/zoom/zoom.js
--rw-r--r--   0        0        0      780 2023-05-25 22:46:16.483520 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/revealjs/layout.html
--rw-r--r--   0        0        0      127 2023-05-25 22:45:31.603928 sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/revealjs/theme.conf
--rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 sphinx_revealjs_slides-0.2.3/setup.py
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 sphinx_revealjs_slides-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-06-06 00:14:16.589409 sphinx_revealjs_slides-0.2.4/README.md
+-rw-r--r--   0        0        0      697 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2271 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/__init__.py
+-rw-r--r--   0        0        0      323 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/builder.py
+-rw-r--r--   0        0        0       89 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/__init__.py
+-rw-r--r--   0        0        0     1082 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/_base_slide.py
+-rw-r--r--   0        0        0     4082 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/incremental.py
+-rw-r--r--   0        0        0     1716 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/newslide.py
+-rw-r--r--   0        0        0     1257 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/speakernote.py
+-rw-r--r--   0        0        0     3030 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/overridenodes.py
+-rw-r--r--   0        0        0      780 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/themes/revealjs/layout.html
+-rw-r--r--   0        0        0      127 2023-06-06 00:14:16.593410 sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/themes/revealjs/theme.conf
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 sphinx_revealjs_slides-0.2.4/PKG-INFO
```

### Comparing `sphinx_revealjs_slides-0.2.3/pyproject.toml` & `sphinx_revealjs_slides-0.2.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "sphinx-revealjs-slides"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Ashley Trinh <ashley@hackbrightacademy.com>"]
 readme = "README.md"
-packages = [{ include = "sphinx_revealjs", from = "src" }]
-exclude = ["src/sphinx_revealjs/themes/lib/reveal.js/*"]
+packages = [{ include = "sphinx_revealjs_slides", from = "src" }]
+exclude = ["src/sphinx_revealjs_slides/themes/lib/reveal.js/*"]
 include = [
-  "src/sphinx_revealjs/themes/lib/reveal.js/dist",
-  "src/sphinx_revealjs/themes/lib/reveal.js/plugin"
+  "src/sphinx_revealjs_slides/themes/lib/reveal.js/dist",
+  "src/sphinx_revealjs_slides/themes/lib/reveal.js/plugin"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sphinx = "^6.1.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/__init__.py` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from . import builder, directives, overridenodes
 
 if TYPE_CHECKING:
     from sphinx.application import Sphinx
     from sphinx.config import Config
 
-__name__ = "sphinx_revealjs"
+__name__ = "sphinx_revealjs_slides"
 __version__ = importlib.metadata.version(__name__)
 
 package_dir = Path(__file__).parent.resolve()
 themes_dir = package_dir / "themes"
 revealjs_dir = themes_dir / "lib" / "reveal.js"
```

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/_base_slide.py` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/_base_slide.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/incremental.py` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/incremental.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/newslide.py` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/newslide.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/directives/speakernote.py` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/directives/speakernote.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/overridenodes.py` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/overridenodes.py`

 * *Files identical despite different names*

### Comparing `sphinx_revealjs_slides-0.2.3/src/sphinx_revealjs/themes/revealjs/layout.html` & `sphinx_revealjs_slides-0.2.4/src/sphinx_revealjs_slides/themes/revealjs/layout.html`

 * *Files identical despite different names*

