# Comparing `tmp/nn_tilde-1.5.2.tar.gz` & `tmp/nn_tilde-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_tilde-1.5.2.tar", last modified: Fri Jun  2 15:55:06 2023, max compression
+gzip compressed data, was "nn_tilde-1.5.3.tar", last modified: Tue Jun  6 13:42:08 2023, max compression
```

## Comparing `nn_tilde-1.5.2.tar` & `nn_tilde-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:55:06.826599 nn_tilde-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-02 15:55:06.826599 nn_tilde-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:55:06.822599 nn_tilde-1.5.2/nn_tilde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:55:06.822599 nn_tilde-1.5.2/python_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/python_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:55:06.826599 nn_tilde-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/nn_tilde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/python_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/python_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/setup.py
```

### Comparing `nn_tilde-1.5.2/LICENSE` & `nn_tilde-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.2/PKG-INFO` & `nn_tilde-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn_tilde
-Version: 1.5.2
+Version: 1.5.3
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.2 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.3 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
```

### Comparing `nn_tilde-1.5.2/README.md` & `nn_tilde-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.2/nn_tilde.egg-info/PKG-INFO` & `nn_tilde-1.5.3/nn_tilde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-tilde
-Version: 1.5.2
+Version: 1.5.3
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.2 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.3 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
```

### Comparing `nn_tilde-1.5.2/python_tools/__init__.py` & `nn_tilde-1.5.3/python_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.2/setup.py` & `nn_tilde-1.5.3/setup.py`

 * *Files identical despite different names*

