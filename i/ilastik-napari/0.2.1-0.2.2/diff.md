# Comparing `tmp/ilastik-napari-0.2.1.tar.gz` & `tmp/ilastik-napari-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilastik-napari-0.2.1.tar", last modified: Tue Feb 28 05:02:25 2023, max compression
+gzip compressed data, was "ilastik-napari-0.2.2.tar", last modified: Tue Jun  6 13:05:43 2023, max compression
```

## Comparing `ilastik-napari-0.2.1.tar` & `ilastik-napari-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.369947 ilastik-napari-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.365947 ilastik-napari-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.365947 ilastik-napari-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/.github/workflows/build-upload.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-02-28 05:02:25.369947 ilastik-napari-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.365947 ilastik-napari-0.2.1/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/conda-recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.365947 ilastik-napari-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/examples/simple_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 05:02:25.369947 ilastik-napari-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.365947 ilastik-napari-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.365947 ilastik-napari-0.2.1/src/ilastik/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.369947 ilastik-napari-0.2.1/src/ilastik/napari/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/src/ilastik/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/src/ilastik/napari/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/src/ilastik/napari/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/src/ilastik/napari/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/src/ilastik/napari/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-28 05:02:14.000000 ilastik-napari-0.2.1/src/ilastik/napari/plugin.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:02:25.369947 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-02-28 05:02:25.000000 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-28 05:02:25.000000 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 05:02:25.000000 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-28 05:02:25.000000 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 05:02:25.000000 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 05:02:25.000000 ilastik-napari-0.2.1/src/ilastik_napari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/.github/workflows/build-upload.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/conda-recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/examples/simple_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/src/ilastik/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/src/ilastik/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/plugin.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/top_level.txt
```

### Comparing `ilastik-napari-0.2.1/.github/workflows/build-upload.yaml` & `ilastik-napari-0.2.2/.github/workflows/build-upload.yaml`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/LICENSE` & `ilastik-napari-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/PKG-INFO` & `ilastik-napari-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilastik-napari
-Version: 0.2.1
+Version: 0.2.2
 Summary: ilastik plugin for napari
 Author-email: Emil Melnikov <emilmelnikov@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ilastik/ilastik-napari
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -28,40 +28,32 @@
 # ilastik-napari
 
 [Napari][napari] plugin for interactive pixel classification.
 Designed to be similar to the pixel classification workflow in [classic ilastik][ilastik].
 
 ## Installation
 
-Currently, this plugin requires you to use a conda environment.
-If you haven't used conda before, please read [conda user guide][conda-user-guide].
+This plugin requires you to use a _conda_ environment. The environment manager conda comes in a few different forms.
+If you haven't used conda before, you can find more information in the [conda user guide][conda-user-guide].
+You can use whichever variant you prefer, as the resulting environment should be the same, but we recommend the [_mambaforge_][mambaforge] variant as it is usually the fastest.
+When using mambaforge, the `mamba` command usually replaces the `conda` command one would otherwise use.
 
-Instad of the default [_miniconda_][miniconda] installation, we highly recommend to use [_mambaforge_][mambaforge].
-It has better default settings, and the `mamba` command, which is an (almost) drop-in replacement for `conda`.
-
-After installing _mambaforge_, create a new environment with this plugin installed:
-   ```shell
-   mamba create -y -c ilastik-forge -n my-napari-env napari-ilastik
-   ```
-
-Finally, launch napari in the new environment.
-   ```shell
-   conda activate my-napari-env
-   napari
-   ```
-
-### Napari Hub and pip
-
-You can also install this plugin via Napari Hub or _pip_. However, in this case you must do that inside a conda environment with the _fastfilters_ package installed:
+Once you have installed mambaforge, set up a conda environment with the _fastfilters_ package, and then use pip to install _ilastik-napari_:
 ```shell
-mamba create -y -c ilastik-forge -n my-napari-env fastfilters
-conda activate my-napari-env
+mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env fastfilters
+mamba activate my-napari-env
 pip install ilastik-napari
 ```
 
+Finally, run napari:
+```shell
+napari
+```
+You should be able to find the ilastik-napari plugin in the Plugins menu.
+
 ## Usage
 
 As a prerequisite, make sure you understand the [napari basics][napari-quickstart].
 
 1. Open your image, or use a sample in _File - Open Sample_.
 
    ![Use a sample image](https://ilastik.org/assets/ilastik-napari/image-sample.png "Use a sample image")
```

### Comparing `ilastik-napari-0.2.1/README.md` & `ilastik-napari-0.2.2/src/ilastik_napari.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,59 @@
+Metadata-Version: 2.1
+Name: ilastik-napari
+Version: 0.2.2
+Summary: ilastik plugin for napari
+Author-email: Emil Melnikov <emilmelnikov@gmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/ilastik/ilastik-napari
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Framework :: napari
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ilastik-napari
 
 [Napari][napari] plugin for interactive pixel classification.
 Designed to be similar to the pixel classification workflow in [classic ilastik][ilastik].
 
 ## Installation
 
-Currently, this plugin requires you to use a conda environment.
-If you haven't used conda before, please read [conda user guide][conda-user-guide].
-
-Instad of the default [_miniconda_][miniconda] installation, we highly recommend to use [_mambaforge_][mambaforge].
-It has better default settings, and the `mamba` command, which is an (almost) drop-in replacement for `conda`.
-
-After installing _mambaforge_, create a new environment with this plugin installed:
-   ```shell
-   mamba create -y -c ilastik-forge -n my-napari-env napari-ilastik
-   ```
-
-Finally, launch napari in the new environment.
-   ```shell
-   conda activate my-napari-env
-   napari
-   ```
-
-### Napari Hub and pip
+This plugin requires you to use a _conda_ environment. The environment manager conda comes in a few different forms.
+If you haven't used conda before, you can find more information in the [conda user guide][conda-user-guide].
+You can use whichever variant you prefer, as the resulting environment should be the same, but we recommend the [_mambaforge_][mambaforge] variant as it is usually the fastest.
+When using mambaforge, the `mamba` command usually replaces the `conda` command one would otherwise use.
 
-You can also install this plugin via Napari Hub or _pip_. However, in this case you must do that inside a conda environment with the _fastfilters_ package installed:
+Once you have installed mambaforge, set up a conda environment with the _fastfilters_ package, and then use pip to install _ilastik-napari_:
 ```shell
-mamba create -y -c ilastik-forge -n my-napari-env fastfilters
-conda activate my-napari-env
+mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env fastfilters
+mamba activate my-napari-env
 pip install ilastik-napari
 ```
 
+Finally, run napari:
+```shell
+napari
+```
+You should be able to find the ilastik-napari plugin in the Plugins menu.
+
 ## Usage
 
 As a prerequisite, make sure you understand the [napari basics][napari-quickstart].
 
 1. Open your image, or use a sample in _File - Open Sample_.
 
    ![Use a sample image](https://ilastik.org/assets/ilastik-napari/image-sample.png "Use a sample image")
```

### Comparing `ilastik-napari-0.2.1/conda-recipe/meta.yaml` & `ilastik-napari-0.2.2/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/examples/simple_labeling.py` & `ilastik-napari-0.2.2/examples/simple_labeling.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/pyproject.toml` & `ilastik-napari-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 dependencies = [
-    "napari[all]",
+    "napari",
     "numpy>=1.20",
     "qtpy",
     "scikit-learn",
     "sparse",
 ]
 dynamic = ["version"]
```

### Comparing `ilastik-napari-0.2.1/src/ilastik/napari/classifier.py` & `ilastik-napari-0.2.2/src/ilastik/napari/classifier.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/src/ilastik/napari/filters.py` & `ilastik-napari-0.2.2/src/ilastik/napari/filters.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/src/ilastik/napari/gui.py` & `ilastik-napari-0.2.2/src/ilastik/napari/gui.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/src/ilastik/napari/plugin.py` & `ilastik-napari-0.2.2/src/ilastik/napari/plugin.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.1/src/ilastik_napari.egg-info/SOURCES.txt` & `ilastik-napari-0.2.2/src/ilastik_napari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

