# Comparing `tmp/bcirisktools-0.3.3.tar.gz` & `tmp/bcirisktools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.3.3.tar", last modified: Tue Jun  6 19:22:38 2023, max compression
+gzip compressed data, was "bcirisktools-0.3.4.tar", last modified: Tue Jun  6 19:27:45 2023, max compression
```

## Comparing `bcirisktools-0.3.3.tar` & `bcirisktools-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:22:38.307000 bcirisktools-0.3.3/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.3.3/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-06-06 19:22:38.300000 bcirisktools-0.3.3/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.3.3/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:22:38.158000 bcirisktools-0.3.3/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.3.3/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5614 2023-06-06 19:20:34.000000 bcirisktools-0.3.3/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.3.3/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.3.3/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-23 00:01:50.000000 bcirisktools-0.3.3/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5783 2023-05-09 16:19:37.000000 bcirisktools-0.3.3/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.3.3/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:22:38.266000 bcirisktools-0.3.3/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-06-06 19:22:37.000000 bcirisktools-0.3.3/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-06-06 19:22:37.000000 bcirisktools-0.3.3/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-06-06 19:22:37.000000 bcirisktools-0.3.3/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-06-06 19:22:37.000000 bcirisktools-0.3.3/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-06-06 19:22:37.000000 bcirisktools-0.3.3/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.3.3/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-06-06 19:22:38.312000 bcirisktools-0.3.3/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-06-06 19:22:23.000000 bcirisktools-0.3.3/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:27:45.338000 bcirisktools-0.3.4/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.3.4/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-06-06 19:27:45.333000 bcirisktools-0.3.4/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.3.4/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:27:45.207000 bcirisktools-0.3.4/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5638 2023-06-06 19:27:22.000000 bcirisktools-0.3.4/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-23 00:01:50.000000 bcirisktools-0.3.4/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5783 2023-05-09 16:19:37.000000 bcirisktools-0.3.4/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.3.4/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:27:45.311000 bcirisktools-0.3.4/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-06-06 19:27:45.342000 bcirisktools-0.3.4/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-06-06 19:27:40.000000 bcirisktools-0.3.4/setup.py
```

### Comparing `bcirisktools-0.3.3/LICENCE` & `bcirisktools-0.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/PKG-INFO` & `bcirisktools-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.3.3
+Version: 0.3.4
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.3.3/README.md` & `bcirisktools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/bcirisktools/input_filters.py` & `bcirisktools-0.3.4/bcirisktools/input_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,23 +72,14 @@
                 data[col] = data[col].fillna(cat_value, inplace=True)
 
         return data
     
     @staticmethod
     def select_k_percentile(df_input, label_name, vars_no_considerar=None, fill_nan = -9999):
     
-        def train_and_evaluate(
-            pipe, print_=True, X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test
-        ):
-            """function to train and evaluate the selection pipeline using the f1-score"""
-
-            pipe.fit(X_train, y_train)
-            y_pred = pipe.predict(X_test)
-            return f1_score(y_test, y_pred, average="macro")
-
         # Select targets and features from the input data
         labels = df_input.loc[:, label_name]
         if (np.array(vars_no_considerar) != None).any():
             features = df_input.drop(columns=vars_no_considerar)
         else:
             features = df_input.drop(label_name)
 
@@ -98,14 +89,23 @@
             labels,
             test_size=0.2,
             random_state=42,
             shuffle=True,
             stratify=labels,
         )
 
+        def train_and_evaluate(
+            pipe, print_=True, X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test
+        ):
+            """function to train and evaluate the selection pipeline using the f1-score"""
+
+            pipe.fit(X_train, y_train)
+            y_pred = pipe.predict(X_test)
+            return f1_score(y_test, y_pred, average="macro")
+
         # Pipeline creation
         selection_pipeline = Pipeline(
             steps=[
                 ("Preprocessing", SimpleImputer(missing_values=np.nan, strategy='constant', fill_value=fill_nan)),
                 ("Selection", SelectPercentile(mutual_info_classif, percentile=20)),
                 ("Tree", DecisionTreeClassifier(random_state=42)),
             ]
@@ -125,14 +125,15 @@
         # Final Plot
         fig = px.line(
             x=f1[:, 0],
             y=f1[:, 1],
             title="F1 según cantidad de Features Conservadas",
         )
 
+        # Update figure
         fig.update_layout(xaxis_title="Cantidad de variables", yaxis_title="F1 Score")
 
         # Return features list
         return features_dict
 
     @staticmethod
     def _flatten(list_):
```

### Comparing `bcirisktools-0.3.3/bcirisktools/metrics_bci.py` & `bcirisktools-0.3.4/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/bcirisktools/modeling.py` & `bcirisktools-0.3.4/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/bcirisktools/shapley_report.py` & `bcirisktools-0.3.4/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/bcirisktools/stability.py` & `bcirisktools-0.3.4/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/bcirisktools/tree_crt.py` & `bcirisktools-0.3.4/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.3/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.3.4/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.3.3
+Version: 0.3.4
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.3.3/setup.py` & `bcirisktools-0.3.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.3.3"
+VERSION = "0.3.4"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

