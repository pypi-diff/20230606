# Comparing `tmp/catencfamily-0.0.64.tar.gz` & `tmp/catencfamily-0.0.65.tar.gz`

## Comparing `catencfamily-0.0.64.tar` & `catencfamily-0.0.65.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.64/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.64/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    21665 2020-02-02 00:00:00.000000 catencfamily-0.0.64/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.64/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.64/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.64/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.64/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.65/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.65/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    26450 2020-02-02 00:00:00.000000 catencfamily-0.0.65/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.65/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.65/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.65/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.65/PKG-INFO
```

### Comparing `catencfamily-0.0.64/src/catencfamily/encoders.py` & `catencfamily-0.0.65/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.64/src/catencfamily/utils.py` & `catencfamily-0.0.65/src/catencfamily/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# 5th June, 2023
+# 6th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import make_classification
+from sklearn.feature_selection import  mutual_info_classif
 import pickle
 import pathlib
 import string
 import matplotlib.pyplot as plt
+import seaborn as sns
 
 
 
 def xgImptFeatures(model, df_columns, filename = None, master=None):
     """
     Given an xgboost classifier model & data col
     names, the function returns two lists of cols,
@@ -32,14 +34,15 @@
                 is important: df_columns = list(df.columns)
     master: Folder where impt feature sequence is saved
             File name: fe_1.txt          
     Returns
     -------
     fe_1 : List of columns having features imp > 0 in descending order
     fe_0 : List of columns having features imp of 0.0
+    fe   : Pandas Series with indicies as col names against imp scores 
     """
     # Sorted index are in descending order of impt
     sorted_idx = model.feature_importances_.argsort()[::-1]
     fe = pd.DataFrame(
                        model.feature_importances_[sorted_idx],
                        index = df_columns[sorted_idx],
                        columns =['imp']
@@ -52,20 +55,39 @@
     print("Order of feature importance is by 'gain'")
     # Save to file
     if filename is not None:
         # Also save these features
         filename = pathlib.Path(master) / filename
         with open(filename,'w') as tfile:
             tfile.write('\n'.join(fe_1))
-    return fe_1, fe_0
+    return fe_1, fe_0, fe
    
 
 # Ref: https://www.kaggle.com/code/tetsutani/ps3e16-eda-ensemble-ml-pipeline
 # For multiple models
 def visualize_importance(models, feature_cols, title, top=9):
+    """
+    Not tested
+    
+    Parameters
+    ----------
+    models : TYPE
+        DESCRIPTION.
+    feature_cols : TYPE
+        DESCRIPTION.
+    title : TYPE
+        DESCRIPTION.
+    top : TYPE, optional
+        DESCRIPTION. The default is 9.
+
+    Returns
+    -------
+    None.
+
+    """
     importances = []
     feature_importance = pd.DataFrame()
     for i, model in enumerate(models):
         _df = pd.DataFrame()
         _df["importance"] = model.feature_importances_
         _df["feature"] = pd.Series(feature_cols)
         _df["fold"] = i
@@ -626,11 +648,160 @@
     print("Concatenating test data")
     cc_te = pd.concat(obj_te, axis = 1)
     print("Done......")
     return cc_tr,cc_te,  vt ,ve, 
 
 
 
+# Ref: https://www.kaggle.com/code/ryanholbrook/mutual-information
+def calMIScores(X, y):
+    """
+    Desc
+    ---- 
+    Calculates mutual information scores when target
+    is discrete.
+
+    Parameters
+    ----------
+    X : Pandas DataFrame 
+    y : An array or Series; target
+
+    Returns
+    -------
+    mi_scores : Pandas Series (sorted)
+
+    """
+    
+    # Get sores
+    mi_scores = mutual_info_classif(X, y)
+    # Transform mi_scores to a Series:
+    mi_scores = pd.Series(mi_scores, name="MI Scores", index=X.columns)
+    # Sort Series in Descending order:
+    mi_scores = mi_scores.sort_values(ascending=False)
+    return mi_scores
+
+
+
+def plotSeries(scores, title= ""):
+    """
+    Desc
+    ----
+    Plots MI scores or feature impt by centrality 
+    calculated by calMIScores() or by featureImptByCentrality()
+    Use it as:
+        plt.figure(dpi=100, figsize=(8, 5))
+        plotSeries(calMIScores(X, y), someTitle)
+        OR, as
+        plotSeries(featureImptByCentrality, someTitle)
+        
+    Parameters
+    ----------
+    scores: Pandas Series
+    title: Graph title; default: Empty str
+    
+    """
+    # Scores sorted in ascending order:
+    scores = scores.sort_values(ascending=True)
+    # Map parameters:
+    width = np.arange(len(scores))
+    # Write ticks as per scores index:
+    ticks = list(scores.index)
+    # Plot width:
+    plt.barh(width, scores)
+    # Plot yticks
+    plt.yticks(width, ticks)
+    plt.title(title)
+    
+    
+
+def featureImptByCentFeatCounts(colList, normalize = False):
+    """
+    Desc
+    ----
+    In the colList, how many columns pertain to
+    degree centrality, eigenvector centrality,
+    page-rank and clustering coeff. Plot
+    by using plotSeries().
+
+    Parameters
+    ----------
+    colList : A list of columns
+    normalize: Boolean
+
+    Returns
+    -------
+    d : A sorted pandas Series
+
+    """
+    d = {'degree' : 0, 'pagerank' : 0, 'eigenvector' : 0, 'clusteringcoeff' : 0,
+         "betweenness" : 0, 'avgembeddedness' : 0, 'leidencomsdensity' : 0}
+    deg = [i for i in colList if 'deg_' in i ]
+    d['degree'] = len(deg)
+    pr =  [i for i in colList if 'pr_' in i ]
+    d['pagerank'] = len(pr)       
+    eig = [i for i in colList if 'eig_' in i ] 
+    d['eigenvector'] = len(eig)      
+    clu = [i for i in colList if 'clu_' in i ]
+    d['clusteringcoeff'] = len(clu)
+    bet = [i for i in colList if 'bet_' in i ]
+    d['betweenness'] = len(bet)
+    ae = [i for i in colList if 'ae_' in i ]
+    d['avgembeddedness'] = len(ae)
+    den = [i for i in colList if 'den_' in i ]
+    d['leidencomsdensity'] = len(den)
+    # Transform d to pandas Series:
+    d = pd.Series(d).sort_values(ascending = False)
+    if (normalize):
+        d = d/sum(d)
+    return d
+
+
+
+def featureImptByScore(score, colList, normalize = False):
+    """
+    Desc
+    ----
+    In the colList, total score of columns
+    that pertain to degree centrality, to eigenvector
+    centrality, to page-rank and clustering coeff and 
+    others. Plot by using plotSeries().
+
+    Parameters
+    ----------
+    score: Pandas Series giving column wise impt score
+    colList : A list of dataframe columns
+    normalize: Boolean
+
+    Returns
+    -------
+    d : A sorted pandas Series
+
+    """
+    d = {'degree' : 0, 'pagerank' : 0, 'eigenvector' : 0, 'clusteringcoeff' : 0,
+         "betweenness" : 0, 'avgembeddedness' : 0, 'leidencomsdensity' : 0}
+    deg = [i for i in colList if 'deg_' in i ]
+    d['degree'] = score[deg].sum()
+    pr =  [i for i in colList if 'pr_' in i ]
+    d['pagerank'] = score[pr].sum()      
+    eig = [i for i in colList if 'eig_' in i ] 
+    d['eigenvector'] = score[eig].sum()    
+    clu = [i for i in colList if 'clu_' in i ]
+    d['clusteringcoeff'] = score[clu].sum()
+    bet = [i for i in colList if 'bet_' in i ]
+    d['betweenness'] = score[bet].sum()
+    ae = [i for i in colList if 'ae_' in i ]
+    d['avgembeddedness'] = score[ae].sum()
+    den = [i for i in colList if 'den_' in i ]
+    d['leidencomsdensity'] = score[den].sum()
+    # Transform d to pandas Series:
+    d = pd.Series(d).sort_values(ascending = False)
+    if (normalize):
+        d = d/sum(d)
+    return d
+       
+           
+
+    
 ############################ BEGIN ###################
```

### Comparing `catencfamily-0.0.64/LICENSE` & `catencfamily-0.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.64/README.md` & `catencfamily-0.0.65/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.64/pyproject.toml` & `catencfamily-0.0.65/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.64"
+version = "0.0.65"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.64/PKG-INFO` & `catencfamily-0.0.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.64
+Version: 0.0.65
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

