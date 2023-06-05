# Comparing `tmp/nxs_analysis_tools-0.0.8.tar.gz` & `tmp/nxs_analysis_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxs_analysis_tools-0.0.8.tar", last modified: Tue May 23 04:29:39 2023, max compression
+gzip compressed data, was "nxs_analysis_tools-0.0.9.tar", last modified: Tue May 23 04:39:01 2023, max compression
```

## Comparing `nxs_analysis_tools-0.0.8.tar` & `nxs_analysis_tools-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 04:29:39.413015 nxs_analysis_tools-0.0.8/
--rw-rw-rw-   0        0        0     1102 2023-05-23 02:22:35.000000 nxs_analysis_tools-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1455 2023-05-23 04:29:39.413015 nxs_analysis_tools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-05-23 02:58:41.000000 nxs_analysis_tools-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 04:29:39.390926 nxs_analysis_tools-0.0.8/nxs_analysis_tools/
--rw-rw-rw-   0        0        0        2 2023-05-23 01:58:04.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools/__init__.py
--rw-rw-rw-   0        0        0     7956 2023-05-10 11:45:08.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools/plot_slice.py
--rw-rw-rw-   0        0        0     2922 2023-05-10 11:44:00.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools/symmetrize_2d.py
-drwxrwxrwx   0        0        0        0 2023-05-23 04:29:39.413015 nxs_analysis_tools-0.0.8/nxs_analysis_tools.egg-info/
--rw-rw-rw-   0        0        0     1455 2023-05-23 04:29:39.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-23 04:29:39.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 04:29:39.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-23 04:29:39.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-23 04:29:39.000000 nxs_analysis_tools-0.0.8/nxs_analysis_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 04:29:39.413015 nxs_analysis_tools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1429 2023-05-23 04:29:17.000000 nxs_analysis_tools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:39:01.325528 nxs_analysis_tools-0.0.9/
+-rw-rw-rw-   0        0        0     1102 2023-05-23 02:22:35.000000 nxs_analysis_tools-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1253 2023-05-23 04:39:01.325528 nxs_analysis_tools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-05-23 02:58:41.000000 nxs_analysis_tools-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 04:39:01.314405 nxs_analysis_tools-0.0.9/nxs_analysis_tools/
+-rw-rw-rw-   0        0        0        2 2023-05-23 01:58:04.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools/__init__.py
+-rw-rw-rw-   0        0        0     7956 2023-05-10 11:45:08.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools/plot_slice.py
+-rw-rw-rw-   0        0        0     2922 2023-05-10 11:44:00.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools/symmetrize_2d.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:39:01.325528 nxs_analysis_tools-0.0.9/nxs_analysis_tools.egg-info/
+-rw-rw-rw-   0        0        0     1253 2023-05-23 04:39:01.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-23 04:39:01.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 04:39:01.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-23 04:39:01.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-23 04:39:01.000000 nxs_analysis_tools-0.0.9/nxs_analysis_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 04:39:01.325528 nxs_analysis_tools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1213 2023-05-23 04:37:50.000000 nxs_analysis_tools-0.0.9/setup.py
```

### Comparing `nxs_analysis_tools-0.0.8/LICENSE.txt` & `nxs_analysis_tools-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nxs_analysis_tools-0.0.8/README.md` & `nxs_analysis_tools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nxs_analysis_tools-0.0.8/nxs_analysis_tools/plot_slice.py` & `nxs_analysis_tools-0.0.9/nxs_analysis_tools/plot_slice.py`

 * *Files identical despite different names*

### Comparing `nxs_analysis_tools-0.0.8/nxs_analysis_tools/symmetrize_2d.py` & `nxs_analysis_tools-0.0.9/nxs_analysis_tools/symmetrize_2d.py`

 * *Files identical despite different names*

### Comparing `nxs_analysis_tools-0.0.8/setup.py` & `nxs_analysis_tools-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,34 +5,29 @@
     long_description = file.read()
 
 
 # specify requirements of your package here
 REQUIREMENTS = ['matplotlib>=3.0.0',
                 'numpy>=1.0.0',
                 'ipython>=1.0.0',
-                'python>=3.7.0',
                 ]
 
 # some more details
 CLASSIFIERS = [
     'Development Status :: 1 - Planning',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Image Processing',
     'Topic :: Scientific/Engineering :: Physics',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.3',
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
     ]
 
 # calling the setup function 
 setup(name='nxs_analysis_tools',
-      version='0.0.8',
+      version='0.0.9',
       description='Tools for analyzing scattering data in .nxs format.',
       long_description=long_description,
       url='https://github.com/stevenjgomez/nxs_analysis_tools',
       author='Steven J. Gomez Alvarado',
       author_email='stevenjgomez@ucsb.edu',
       license='MIT',
       packages=['nxs_analysis_tools'],
```

