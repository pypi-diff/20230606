# Comparing `tmp/torchqtm-0.0.2.tar.gz` & `tmp/torchqtm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchqtm-0.0.2.tar", last modified: Tue Jun  6 06:21:17 2023, max compression
+gzip compressed data, was "torchqtm-0.0.3.tar", last modified: Tue Jun  6 06:25:12 2023, max compression
```

## Comparing `torchqtm-0.0.2.tar` & `torchqtm-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,61 @@
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:21:17.832912 torchqtm-0.0.2/
--rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-05-21 08:16:14.000000 torchqtm-0.0.2/LICENSE
--rw-r--r--   0 nymath     (501) staff       (20)     1679 2023-06-06 06:21:17.832708 torchqtm-0.0.2/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     1291 2023-06-03 06:24:39.000000 torchqtm-0.0.2/README.md
--rw-r--r--   0 nymath     (501) staff       (20)       38 2023-06-06 06:21:17.832967 torchqtm-0.0.2/setup.cfg
--rw-r--r--   0 nymath     (501) staff       (20)      949 2023-06-06 01:04:18.000000 torchqtm-0.0.2/setup.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:21:17.829548 torchqtm-0.0.2/test/
--rw-r--r--   0 nymath     (501) staff       (20)        2 2023-05-20 16:39:21.000000 torchqtm-0.0.2/test/test_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-06 01:01:34.000000 torchqtm-0.0.2/test/testfunc_.py
--rw-r--r--   0 nymath     (501) staff       (20)     1994 2023-06-06 01:01:34.000000 torchqtm-0.0.2/test/testgplearn.py
--rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-06 01:01:34.000000 torchqtm-0.0.2/test/testop.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:21:17.830239 torchqtm-0.0.2/torchqtm/
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:21:17.832158 torchqtm-0.0.2/torchqtm/_C/
--rw-r--r--   0 nymath     (501) staff       (20)   108922 2023-06-06 01:03:03.000000 torchqtm-0.0.2/torchqtm/_C/__init__.c
--rw-r--r--   0 nymath     (501) staff       (20)   289042 2023-06-06 01:03:03.000000 torchqtm-0.0.2/torchqtm/_C/_functional.c
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 06:09:18.000000 torchqtm-0.0.2/torchqtm/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      119 2023-05-21 02:33:17.000000 torchqtm-0.0.2/torchqtm/config.py
--rw-r--r--   0 nymath     (501) staff       (20)      629 2023-06-06 03:21:03.000000 torchqtm-0.0.2/torchqtm/utils.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:21:17.831138 torchqtm-0.0.2/torchqtm.egg-info/
--rw-r--r--   0 nymath     (501) staff       (20)     1679 2023-06-06 06:21:17.000000 torchqtm-0.0.2/torchqtm.egg-info/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)      336 2023-06-06 06:21:17.000000 torchqtm-0.0.2/torchqtm.egg-info/SOURCES.txt
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-06 06:21:17.000000 torchqtm-0.0.2/torchqtm.egg-info/dependency_links.txt
--rw-r--r--   0 nymath     (501) staff       (20)        9 2023-06-06 06:21:17.000000 torchqtm-0.0.2/torchqtm.egg-info/top_level.txt
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.032804 torchqtm-0.0.3/
+-rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-05-21 08:16:14.000000 torchqtm-0.0.3/LICENSE
+-rw-r--r--   0 nymath     (501) staff       (20)     1679 2023-06-06 06:25:12.032622 torchqtm-0.0.3/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     1291 2023-06-03 06:24:39.000000 torchqtm-0.0.3/README.md
+-rw-r--r--   0 nymath     (501) staff       (20)       38 2023-06-06 06:25:12.032863 torchqtm-0.0.3/setup.cfg
+-rw-r--r--   0 nymath     (501) staff       (20)      952 2023-06-06 06:24:57.000000 torchqtm-0.0.3/setup.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.022024 torchqtm-0.0.3/test/
+-rw-r--r--   0 nymath     (501) staff       (20)        2 2023-05-20 16:39:21.000000 torchqtm-0.0.3/test/test_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-06 01:01:34.000000 torchqtm-0.0.3/test/testfunc_.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1994 2023-06-06 01:01:34.000000 torchqtm-0.0.3/test/testgplearn.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-06 01:01:34.000000 torchqtm-0.0.3/test/testop.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.023114 torchqtm-0.0.3/torchqtm/
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025032 torchqtm-0.0.3/torchqtm/_C/
+-rw-r--r--   0 nymath     (501) staff       (20)   108922 2023-06-06 01:03:03.000000 torchqtm-0.0.3/torchqtm/_C/__init__.c
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/_C/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   289042 2023-06-06 01:03:03.000000 torchqtm-0.0.3/torchqtm/_C/_functional.c
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 06:09:18.000000 torchqtm-0.0.3/torchqtm/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025508 torchqtm-0.0.3/torchqtm/autoalpha/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:33:58.000000 torchqtm-0.0.3/torchqtm/autoalpha/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025618 torchqtm-0.0.3/torchqtm/autoalpha/boost/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-21 03:29:04.000000 torchqtm-0.0.3/torchqtm/autoalpha/boost/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.025730 torchqtm-0.0.3/torchqtm/autoalpha/cnn/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:35:23.000000 torchqtm-0.0.3/torchqtm/autoalpha/cnn/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.027849 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/
+-rw-r--r--   0 nymath     (501) staff       (20)      218 2023-02-04 05:13:39.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/_program.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6595 2023-05-20 06:10:27.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/fitness.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7239 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/functions.py
+-rw-r--r--   0 nymath     (501) staff       (20)    66949 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/genetic.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-02-04 05:13:39.000000 torchqtm-0.0.3/torchqtm/autoalpha/gplearn/utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)      119 2023-05-21 02:33:17.000000 torchqtm-0.0.3/torchqtm/config.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.028080 torchqtm-0.0.3/torchqtm/edbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-21 09:03:13.000000 torchqtm-0.0.3/torchqtm/edbt/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.029070 torchqtm-0.0.3/torchqtm/op/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-17 06:33:06.000000 torchqtm-0.0.3/torchqtm/op/CrossSectionalOperators.py
+-rw-r--r--   0 nymath     (501) staff       (20)       20 2023-05-25 13:48:11.000000 torchqtm-0.0.3/torchqtm/op/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)       68 2023-05-26 11:03:24.000000 torchqtm-0.0.3/torchqtm/op/algos.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2136 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/op/base.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9803 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/op/functional.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.030247 torchqtm-0.0.3/torchqtm/option/
+-rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/option/Option.py
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/option/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1640 2023-06-06 00:48:35.000000 torchqtm-0.0.3/torchqtm/option/functional.py
+-rw-r--r--   0 nymath     (501) staff       (20)      586 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/option/main.py
+-rw-r--r--   0 nymath     (501) staff       (20)      629 2023-06-06 03:21:03.000000 torchqtm-0.0.3/torchqtm/utils.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.031851 torchqtm-0.0.3/torchqtm/vbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:36:01.000000 torchqtm-0.0.3/torchqtm/vbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7983 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/vbt/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/vbt/benchmark.py
+-rw-r--r--   0 nymath     (501) staff       (20)      278 2023-05-25 11:20:21.000000 torchqtm-0.0.3/torchqtm/vbt/dataset.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2142 2023-05-25 14:46:07.000000 torchqtm-0.0.3/torchqtm/vbt/rebalance.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-06 05:11:02.000000 torchqtm-0.0.3/torchqtm/vbt/stats.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1452 2023-06-06 01:01:34.000000 torchqtm-0.0.3/torchqtm/vbt/universe.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.032236 torchqtm-0.0.3/torchqtm/visualization/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-05-20 16:36:40.000000 torchqtm-0.0.3/torchqtm/visualization/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1803 2023-05-18 06:40:49.000000 torchqtm-0.0.3/torchqtm/visualization/visualization.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-06-06 06:25:12.023776 torchqtm-0.0.3/torchqtm.egg-info/
+-rw-r--r--   0 nymath     (501) staff       (20)     1679 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     1205 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/SOURCES.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/dependency_links.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        9 2023-06-06 06:25:11.000000 torchqtm-0.0.3/torchqtm.egg-info/top_level.txt
```

### Comparing `torchqtm-0.0.2/LICENSE` & `torchqtm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.2/PKG-INFO` & `torchqtm-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: torchqtm
-Version: 0.0.2
-Summary: None
-Home-page: https://github.com/nymath/torchquantum/tree/main
-Author: ny
-Author-email: nymath@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img src="https://github.com/nymath/torchquantum/blob/main/src/fig/logo.png" align="right" width="196" />
 
 # torchquantum
 
 TorchQuantum is a backtesting framework that integrates
 the structure of PyTorch and WorldQuant's Operator for
 efficient quantitative financial analysis.
```

### Comparing `torchqtm-0.0.2/README.md` & `torchqtm-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: torchqtm
+Version: 0.0.3
+Summary: None
+Home-page: https://github.com/nymath/torchquantum/tree/main
+Author: ny
+Author-email: nymath@163.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src="https://github.com/nymath/torchquantum/blob/main/src/fig/logo.png" align="right" width="196" />
 
 # torchquantum
 
 TorchQuantum is a backtesting framework that integrates
 the structure of PyTorch and WorldQuant's Operator for
 efficient quantitative financial analysis.
```

### Comparing `torchqtm-0.0.2/setup.py` & `torchqtm-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 extensions = glob.glob("torchqtm/_C/*.pyx")
 
 setup(
     ext_modules=cythonize(extensions),
     include_dirs=[numpy.get_include()],
     name="torchqtm",
-    version="0.0.2",
+    version="0.0.3",
     author="ny",
     author_email="nymath@163.com",
     description="None",
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nymath/torchquantum/tree/main",
-    packages=['torchqtm'],
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `torchqtm-0.0.2/test/testgplearn.py` & `torchqtm-0.0.3/test/testgplearn.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.2/test/testop.py` & `torchqtm-0.0.3/test/testop.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.2/torchqtm/_C/__init__.c` & `torchqtm-0.0.3/torchqtm/_C/__init__.c`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.2/torchqtm/_C/_functional.c` & `torchqtm-0.0.3/torchqtm/_C/_functional.c`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.2/torchqtm/utils.py` & `torchqtm-0.0.3/torchqtm/utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.0.2/torchqtm.egg-info/PKG-INFO` & `torchqtm-0.0.3/torchqtm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.0.2
+Version: 0.0.3
 Summary: None
 Home-page: https://github.com/nymath/torchquantum/tree/main
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

