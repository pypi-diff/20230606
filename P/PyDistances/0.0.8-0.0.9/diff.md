# Comparing `tmp/PyDistances-0.0.8.tar.gz` & `tmp/PyDistances-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDistances-0.0.8.tar", last modified: Sat May 20 14:12:11 2023, max compression
+gzip compressed data, was "PyDistances-0.0.9.tar", last modified: Sat May 20 14:33:16 2023, max compression
```

## Comparing `PyDistances-0.0.8.tar` & `PyDistances-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:11.896569 PyDistances-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1069 2023-05-20 14:12:11.895574 PyDistances-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:11.884371 PyDistances-0.0.8/PyDistances/
--rw-rw-rw-   0        0        0      536 2023-05-20 14:08:13.000000 PyDistances-0.0.8/PyDistances/__init__.py
--rw-rw-rw-   0        0        0    52586 2023-05-20 14:04:02.000000 PyDistances-0.0.8/PyDistances/distances.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:11.893577 PyDistances-0.0.8/PyDistances.egg-info/
--rw-rw-rw-   0        0        0     1069 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      340 2023-05-20 11:51:44.000000 PyDistances-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 14:12:11.897567 PyDistances-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1045 2023-05-20 14:12:07.000000 PyDistances-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:33:16.048705 PyDistances-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1069 2023-05-20 14:33:16.047708 PyDistances-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 14:33:16.033746 PyDistances-0.0.9/PyDistances/
+-rw-rw-rw-   0        0        0      536 2023-05-20 14:08:13.000000 PyDistances-0.0.9/PyDistances/__init__.py
+-rw-rw-rw-   0        0        0    52576 2023-05-20 14:32:16.000000 PyDistances-0.0.9/PyDistances/distances.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:33:16.045713 PyDistances-0.0.9/PyDistances.egg-info/
+-rw-rw-rw-   0        0        0     1069 2023-05-20 14:33:15.000000 PyDistances-0.0.9/PyDistances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-20 14:33:15.000000 PyDistances-0.0.9/PyDistances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:33:15.000000 PyDistances-0.0.9/PyDistances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 14:33:15.000000 PyDistances-0.0.9/PyDistances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 14:33:15.000000 PyDistances-0.0.9/PyDistances.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      340 2023-05-20 11:51:44.000000 PyDistances-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:33:16.048705 PyDistances-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2023-05-20 14:32:48.000000 PyDistances-0.0.9/setup.py
```

### Comparing `PyDistances-0.0.8/LICENSE` & `PyDistances-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.8/PKG-INFO` & `PyDistances-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.8/PyDistances/__init__.py` & `PyDistances-0.0.9/PyDistances/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.8/PyDistances/distances.py` & `PyDistances-0.0.9/PyDistances/distances.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     else:
         pass
     n = len(Data)
     M =  np.zeros((n , n))
     S_inv=np.linalg.inv( np.cov(Data , rowvar=False) )
     for i in range(0, n):
          for r in range(i+1, n):
-            M[i,r] = Mahalanobis_Dist(x = np.array([Data[i,:] - Data[r,:]]) , S_inv=S_inv ) 
+            M[i,r] = Mahalanobis_Dist(x_i=Data[i,:], x_r=Data[r,:], S_inv=S_inv ) 
     M = M + M.T
     return M 
 
 def a_b_c_d_Matrix(Data):
     """
     Calcula las matrices con los parametros a,b,c y d usados en las distancias de Jaccard, Sokal y Gower.
```

### Comparing `PyDistances-0.0.8/PyDistances.egg-info/PKG-INFO` & `PyDistances-0.0.9/PyDistances.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.8/setup.py` & `PyDistances-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDistances",
-    version="0.0.8",
+    version="0.0.9",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/Distances_Package",  # add your project URL here
     packages=find_packages(),
```

