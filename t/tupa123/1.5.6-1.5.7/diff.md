# Comparing `tmp/tupa123-1.5.6.tar.gz` & `tmp/tupa123-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.5.6.tar", last modified: Mon Jun  5 19:09:13 2023, max compression
+gzip compressed data, was "tupa123-1.5.7.tar", last modified: Tue Jun  6 20:06:17 2023, max compression
```

## Comparing `tupa123-1.5.6.tar` & `tupa123-1.5.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.115947 tupa123-1.5.6/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-06-05 19:09:13.115947 tupa123-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 19:09:13.116937 tupa123-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-05 19:07:46.000000 tupa123-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.096828 tupa123-1.5.6/tupa12/
--rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.6/tupa12/__init__.py
--rw-rw-rw-   0        0        0    54180 2023-06-05 16:54:03.000000 tupa123-1.5.6/tupa12/tupa12.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.105082 tupa123-1.5.6/tupa123/
--rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.6/tupa123/__init__.py
--rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.6/tupa123/machine1.txt
--rw-rw-rw-   0        0        0    94064 2023-06-05 18:09:11.000000 tupa123-1.5.6/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.113922 tupa123-1.5.6/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-05 19:09:13.000000 tupa123-1.5.6/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.865681 tupa123-1.5.7/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-06-06 20:06:17.865681 tupa123-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 20:06:17.865681 tupa123-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-06 20:05:09.000000 tupa123-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.765444 tupa123-1.5.7/tupa12/
+-rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.7/tupa12/__init__.py
+-rw-rw-rw-   0        0        0    54180 2023-06-05 16:54:03.000000 tupa123-1.5.7/tupa12/tupa12.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.843757 tupa123-1.5.7/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.7/tupa123/__init__.py
+-rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.7/tupa123/machine1.txt
+-rw-rw-rw-   0        0        0    94178 2023-06-06 19:56:11.000000 tupa123-1.5.7/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.865681 tupa123-1.5.7/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.5.6/LICENSE.txt` & `tupa123-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.6/PKG-INFO` & `tupa123-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.6
+Version: 1.5.7
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.5.6/README.md` & `tupa123-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.6/setup.py` & `tupa123-1.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.5.6',
+    version='1.5.7',
     license = 'MIT',
     license_files=('LICENSE.txt',),
     packages=['tupa123', 'tupa12'],
     package_data={'tupa123': ['machine1.txt'],},    
     install_requires=['numpy','matplotlib','pandas','opencv-python'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
```

### Comparing `tupa123-1.5.6/tupa12/tupa12.py` & `tupa123-1.5.7/tupa12/tupa12.py`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.6/tupa123/machine1.txt` & `tupa123-1.5.7/tupa123/machine1.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.6/tupa123/tupa123.py` & `tupa123-1.5.7/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,34 +669,36 @@
     denormalized = data * (vetormax2 - vetormin2) + vetormin2
     return denormalized
 
 
 
 
 #compressão logaritmica, dado um vetor de 0 a n por variável
-def Compress(data, vetorlog):
+def Compress(data, vetorlog, expo=1):
     a,b = data.shape
     for i in range(0, a):
         for j in range(0, b):
             comando = vetorlog[j]
             if (comando > 0):
                 for k in range(comando):
                     data[i][j] = np.log10(data[i][j])
+                data[i][j] = data[i][j]**expo
     return data
 
 
 
 
 #descompressão logaritmica, dado um vetor de 0 a n por variável
-def Decompress(data, vetorlog):
+def Decompress(data, vetorlog, expo=1):
     a,b = data.shape
     for i in range(0, a):
         for j in range(0, b):
             comando = vetorlog[j]
             if (comando > 0):
+                data[i][j] = data[i][j]**(1/expo)
                 for k in range(comando):
                     data[i][j] =10**(data[i][j])
     return data
```

### Comparing `tupa123-1.5.6/tupa123.egg-info/PKG-INFO` & `tupa123-1.5.7/tupa123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.6
+Version: 1.5.7
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

