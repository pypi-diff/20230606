# Comparing `tmp/crillab-autograph-0.1.0rc8.tar.gz` & `tmp/crillab-autograph-0.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crillab-autograph-0.1.0rc8.tar", last modified: Tue May  4 14:42:24 2021, max compression
+gzip compressed data, was "dist/crillab-autograph-0.1.0rc9.tar", last modified: Tue May  4 14:51:23 2021, max compression
```

## Comparing `crillab-autograph-0.1.0rc8.tar` & `crillab-autograph-0.1.0rc9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1372 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      611 2021-04-19 09:35:40.000000 crillab-autograph-0.1.0rc8/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/autograph/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2899 2021-05-04 14:41:41.000000 crillab-autograph-0.1.0rc8/autograph/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/autograph/core/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1953 2021-04-19 06:20:07.000000 crillab-autograph-0.1.0rc8/autograph/core/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3605 2021-04-19 06:20:07.000000 crillab-autograph-0.1.0rc8/autograph/core/enumstyle.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8067 2021-05-04 12:34:24.000000 crillab-autograph-0.1.0rc8/autograph/core/plot.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6290 2021-05-04 12:45:00.000000 crillab-autograph-0.1.0rc8/autograph/core/style.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/autograph/wrapper/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1954 2021-04-19 06:20:07.000000 crillab-autograph-0.1.0rc8/autograph/wrapper/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     9474 2021-05-04 12:34:24.000000 crillab-autograph-0.1.0rc8/autograph/wrapper/mpl.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     9461 2021-05-04 12:34:24.000000 crillab-autograph-0.1.0rc8/autograph/wrapper/plotly.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1372 2021-05-04 14:42:23.000000 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      469 2021-05-04 14:42:24.000000 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2021-05-04 14:42:23.000000 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2021-05-04 14:42:23.000000 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/not-zip-safe
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      205 2021-05-04 14:42:23.000000 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       10 2021-05-04 14:42:23.000000 crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2021-05-04 14:42:24.021772 crillab-autograph-0.1.0rc8/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3765 2021-05-04 12:51:46.000000 crillab-autograph-0.1.0rc8/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1372 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      611 2021-04-19 09:35:40.000000 crillab-autograph-0.1.0rc9/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/autograph/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2896 2021-05-04 14:50:56.000000 crillab-autograph-0.1.0rc9/autograph/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/autograph/core/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1953 2021-04-19 06:20:07.000000 crillab-autograph-0.1.0rc9/autograph/core/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3605 2021-04-19 06:20:07.000000 crillab-autograph-0.1.0rc9/autograph/core/enumstyle.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     8067 2021-05-04 12:34:24.000000 crillab-autograph-0.1.0rc9/autograph/core/plot.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6290 2021-05-04 12:45:00.000000 crillab-autograph-0.1.0rc9/autograph/core/style.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/autograph/wrapper/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1954 2021-04-19 06:20:07.000000 crillab-autograph-0.1.0rc9/autograph/wrapper/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     9474 2021-05-04 12:34:24.000000 crillab-autograph-0.1.0rc9/autograph/wrapper/mpl.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     9461 2021-05-04 12:34:24.000000 crillab-autograph-0.1.0rc9/autograph/wrapper/plotly.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1372 2021-05-04 14:51:23.000000 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      469 2021-05-04 14:51:23.000000 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2021-05-04 14:51:23.000000 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2021-05-04 14:51:23.000000 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/not-zip-safe
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      205 2021-05-04 14:51:23.000000 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       10 2021-05-04 14:51:23.000000 crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2021-05-04 14:51:23.841775 crillab-autograph-0.1.0rc9/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3765 2021-05-04 12:51:46.000000 crillab-autograph-0.1.0rc9/setup.py
```

### Comparing `crillab-autograph-0.1.0rc8/PKG-INFO` & `crillab-autograph-0.1.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crillab-autograph
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: AUtogRAPH - A Unified libRary for drAwing Plots in pytHon
 Home-page: https://github.com/crillab/autograph
 Author: Thibault Falque, Romain Wallon, Hugues Wattez
 Author-email: thibault.falque@exakis-nelite.com, wallon@lix.polytechnique.fr, wattez@cril.fr
 License: MIT
 Description: # AUtogRAPH - A Unified libRary for drAwing Plots in pytHon
```

### Comparing `crillab-autograph-0.1.0rc8/README.md` & `crillab-autograph-0.1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/__init__.py` & `crillab-autograph-0.1.0rc9/autograph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 #  NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT                 #
 #  HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,                #
 #  WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING                #
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR               #
 #  OTHER DEALINGS IN THE SOFTWARE.                                             #
 # ##############################################################################
 
+from autograph.core.plot import Plot
+
 
 def create_plot(name: str):
-    from autograph.core.plot import Plot
     from autograph.wrapper.mpl import MPL
     from autograph.wrapper.plotly import Plotly
 
     for elt in Plot.__subclasses__():
         if elt.name == name.lower():
             return globals()[elt.__name__]()
     raise ValueError(f'{name} is not a valid class')
@@ -46,13 +47,13 @@
     '__copyright__',
 ]
 
 __title__ = 'autograph'
 __summary__ = 'AUtogRAPH - A Unified libRary for drAwing Plots in pytHon'
 __keywords__ = 'visualization plots'
 __uri__ = 'https://github.com/crillab/autograph'
-__version__ = '0.1.0-rc8'
+__version__ = '0.1.0-rc9'
 __author__ = 'Thibault Falque, Romain Wallon, Hugues Wattez'
 __email__ = 'thibault.falque@exakis-nelite.com, wallon@lix.polytechnique.fr, wattez@cril.fr'
 
 __license__ = 'MIT'
 __copyright__ = '2021-2022 - Univ Artois & CNRS, Exakis Nelite'
```

### Comparing `crillab-autograph-0.1.0rc8/autograph/core/__init__.py` & `crillab-autograph-0.1.0rc9/autograph/core/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/core/enumstyle.py` & `crillab-autograph-0.1.0rc9/autograph/core/enumstyle.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/core/plot.py` & `crillab-autograph-0.1.0rc9/autograph/core/plot.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/core/style.py` & `crillab-autograph-0.1.0rc9/autograph/core/style.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/wrapper/__init__.py` & `crillab-autograph-0.1.0rc9/autograph/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/wrapper/mpl.py` & `crillab-autograph-0.1.0rc9/autograph/wrapper/mpl.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/autograph/wrapper/plotly.py` & `crillab-autograph-0.1.0rc9/autograph/wrapper/plotly.py`

 * *Files identical despite different names*

### Comparing `crillab-autograph-0.1.0rc8/crillab_autograph.egg-info/PKG-INFO` & `crillab-autograph-0.1.0rc9/crillab_autograph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crillab-autograph
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: AUtogRAPH - A Unified libRary for drAwing Plots in pytHon
 Home-page: https://github.com/crillab/autograph
 Author: Thibault Falque, Romain Wallon, Hugues Wattez
 Author-email: thibault.falque@exakis-nelite.com, wallon@lix.polytechnique.fr, wattez@cril.fr
 License: MIT
 Description: # AUtogRAPH - A Unified libRary for drAwing Plots in pytHon
```

### Comparing `crillab-autograph-0.1.0rc8/setup.py` & `crillab-autograph-0.1.0rc9/setup.py`

 * *Files identical despite different names*

