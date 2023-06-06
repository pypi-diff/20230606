# Comparing `tmp/absplit-1.0.0.tar.gz` & `tmp/absplit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.0.0.tar` & `absplit-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4958 2023-05-20 17:44:37.211000 absplit-1.0.0/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.0.0/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-02-18 09:50:13.578000 absplit-1.0.0/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-05 22:39:03.152000 absplit-1.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.0.0/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0     6872 2023-06-05 23:18:41.806000 absplit-1.0.0/README.md
--rw-r--r--   0        0        0       62 2023-06-05 22:46:15.889000 absplit-1.0.0/absplit/__init__.py
--rw-r--r--   0        0        0     8775 2023-06-05 15:37:08.054000 absplit-1.0.0/absplit/data.py
--rw-r--r--   0        0        0    21148 2023-06-05 23:13:31.496000 absplit-1.0.0/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.0.0/absplit/param.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.0.0/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-06-05 22:35:18.918000 absplit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-20 08:12:29.431000 absplit-1.0.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.0.0/tests/test_data.py
--rw-r--r--   0        0        0     2078 2023-06-05 22:46:15.926000 absplit-1.0.0/tests/test_ga.py
--rw-r--r--   0        0        0     7923 1970-01-01 00:00:00.000000 absplit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.0.1/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-05 23:23:06.142000 absplit-1.0.1/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-05 23:23:06.158000 absplit-1.0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.0.1/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     7015 2023-06-06 00:11:28.620000 absplit-1.0.1/README.md
+-rw-r--r--   0        0        0       62 2023-06-06 00:11:28.566000 absplit-1.0.1/absplit/__init__.py
+-rw-r--r--   0        0        0     8775 2023-06-05 23:23:06.210000 absplit-1.0.1/absplit/data.py
+-rw-r--r--   0        0        0    21344 2023-06-05 23:49:01.136000 absplit-1.0.1/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.0.1/absplit/param.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.0.1/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-06-06 00:11:28.664000 absplit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.0.1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.0.1/tests/test_data.py
+-rw-r--r--   0        0        0     2099 2023-06-05 23:50:53.798000 absplit-1.0.1/tests/test_ga.py
+-rw-r--r--   0        0        0     8064 1970-01-01 00:00:00.000000 absplit-1.0.1/PKG-INFO
```

### Comparing `absplit-1.0.0/.gitignore` & `absplit-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.0.0/LICENSE` & `absplit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.0.0/README.md` & `absplit-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.0.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.1-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -121,29 +121,31 @@
 # Extract results
 df = ab.results
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
-`ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5])`
+`ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
 Splits population into 2 groups. Mutually exclusive, completely exhaustive
 
 Arguments:
 * `df` (pd.DataFrame): Dataframe to be split
 * `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
 * `splitting` (str): Name of column that represents individuals in the population that is getting split
 * `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
 perform a static split, i.e. not across timeseries, (default `None`)
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
+* `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
+(default: `0`)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.0.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.0.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -47,46 +47,48 @@
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
 'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
 groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
 generation fitness ab.fitness() # Visualise data ab.visualise() # Extract
 results df = ab.results ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
-ga_params={}, metric_weights={}, splits=[0.5, 0.5])` Splits population into 2
-groups. Mutually exclusive, completely exhaustive Arguments: * `df`
-(pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of, or list
-of names of, metric columns in DataFrame * `splitting` (str): Name of column
-that represents individuals in the population that is getting split *
-`date_col` (str, optional): Name of column that represents time periods, if
-applicable. If left empty, it will perform a static split, i.e. not across
-timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
-genetic algorithm `pygad.GA` module parameters, see [here](https://
-pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
-for arguments you can pass (default: `{}`) * `splits` (list, optional): How
-many groups to split into, and relative size of the groups (default: `[0.5,
-0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
-each metric in the data. If you want the splitting to focus on one metrics more
-than the other, you can prioritise this here (default: `{}`) ### Match `Match
-(population, sample, metrics, splitting, date_col=None, ga_params={},
-metric_weights={})` Takes DataFrame `sample` and finds a comparable group in
-`population`. Arguments: * `population` (pd.DataFrame): Population to search
-for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
-Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
-list of names of, metric columns in DataFrame * `splitting` (str): Name of
+ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
+population into 2 groups. Mutually exclusive, completely exhaustive Arguments:
+* `df` (pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of,
+or list of names of, metric columns in DataFrame * `splitting` (str): Name of
 column that represents individuals in the population that is getting split *
 `date_col` (str, optional): Name of column that represents time periods, if
 applicable. If left empty, it will perform a static split, i.e. not across
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
-0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
-each metric in the data. If you want the splitting to focus on one metrics more
-than the other, you can prioritise this here (default: `{}`)
+0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
+weighting for differences in the population count between groups (default: `0`)
+* `metric_weights` (dict, optional): Weights for each metric in the data. If
+you want the splitting to focus on one metrics more than the other, you can
+prioritise this here (default: `{}`) ### Match `Match(population, sample,
+metrics, splitting, date_col=None, ga_params={}, metric_weights={})` Takes
+DataFrame `sample` and finds a comparable group in `population`. Arguments: *
+`population` (pd.DataFrame): Population to search for comparable group (**Must
+exclude sample data**) * `sample` (pd.DataFrame): Sample we are looking to find
+a match for. * `metrics` (str, list): Name of, or list of names of, metric
+columns in DataFrame * `splitting` (str): Name of column that represents
+individuals in the population that is getting split * `date_col` (str,
+optional): Name of column that represents time periods, if applicable. If left
+empty, it will perform a static split, i.e. not across timeseries, (default
+`None`) * `ga_params` (dict, optional): Parameters for the genetic algorithm
+`pygad.GA` module parameters, see [here](https://pygad.readthedocs.io/en/
+latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
+(default: `{}`) * `splits` (list, optional): How many groups to split into, and
+relative size of the groups (default: `[0.5, 0.5]`, 2 groups of equal size) *
+`metric_weights` (dict, optional): Weights for each metric in the data. If you
+want the splitting to focus on one metrics more than the other, you can
+prioritise this here (default: `{}`)
                                                                   (back_to_top)
 ## Contributing I welcome contributions to ABSplit! For major changes, please
 open an issue first to discuss what you would like to change. Please make sure
 to update tests as appropriate.
                                                                   (back_to_top)
 ## License [MIT](https://choosealicense.com/licenses/mit/)
                                                                   (back_to_top)
```

### Comparing `absplit-1.0.0/absplit/data.py` & `absplit-1.0.1/absplit/data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.0.0/absplit/ga.py` & `absplit-1.0.1/absplit/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,24 +150,27 @@
     Methods:
         _cost_weighting(): Modifies cost weighting array
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
-    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], **kwargs):
+    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], size_penalty=1, **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             ga_params (dict, optional): Genetic algorithm parameters to add/modify
             metric_weights (dict, optional): Cost weightings to apply to metrics
             runs (int, optional): How many runs to try
             **kwargs: Additional keyword arguments
         """
         super().__init__(**kwargs)
+        global size_penalty_global
+        size_penalty_global = size_penalty
+
         if ga_params:
             assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
         self._runs = runs
         self._splits = splits
         self._splits_num = len(self._splits)
         self._ga_params = GAParams(splits=splits, **ga_params)
         self._best_score = -1
@@ -176,14 +179,15 @@
         self._population = None
         self._df_result = None  # Final results dataframe
         self._ga = None  # genetic algorithm instance
         self._df_vis = None  # Visualisation dataframe
         self._best_ga = None
         self._solution = None
 
+
         self._cost_weighting()
 
     def _cost_weighting(self):
         """Set relative cost weights for each metric. Defaults to 1 unless specified.
 
         Used if you want the genetic algorithm to penalise the MSE cost of some metrics
         over others. Particularly useful if one metric is quite volatile, as the MSE cost can
@@ -547,28 +551,29 @@
 
 def fitness_func_absplit(ga_instance, solution, solution_idx):
     """Fitness function for ABSplit
     """
     global all_metrics_global
     global metric_weights_global
     global splits_global
+    global size_penalty_global
 
     # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
     groups = np.array([(solution == i).astype(int) for i in range(len(splits_global))])
 
     # Size penalty
     # Calculate all_metrics mean * number of days * number of metrics
     mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
     # Get size cost for each group
     mean_group = (groups * mean).sum(1) * splits_global
     # Calculate group differences, sum
-    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum())
+    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum()) * size_penalty_global
 
     # Metric cost
-    costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1))
+    costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1)) * metric_weights_global.reshape(-1, 1, 1)
     diffs = np.roll(costs, -1, axis=1) - costs
     mse = ((diffs ** 2).mean(axis=1)).sum()
     mse = mse + size_cost
 
     # Fitness
     fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
     return fitness
```

### Comparing `absplit-1.0.0/absplit/param.py` & `absplit-1.0.1/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.0.0/images/logo.jpeg` & `absplit-1.0.1/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.0.0/pyproject.toml` & `absplit-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.0.0"
+version = "1.0.1"
 description = "Generates A/B test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.0.0/tests/test_data.py` & `absplit-1.0.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.0.0/tests/test_ga.py` & `absplit-1.0.1/tests/test_ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     'date_col': 'date',
     'splitting': 'city'
 }
 
 # Initialise and run
 ab = ABSplit(
     df=df,
+    size_penalty=0,
     **kwargs,
 )
 ab.run()
 
 # Results
 data_dct1 = {
     'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
```

### Comparing `absplit-1.0.0/PKG-INFO` & `absplit-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generates A/B test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.0.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.1-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -150,29 +150,31 @@
 # Extract results
 df = ab.results
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
-`ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5])`
+`ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
 Splits population into 2 groups. Mutually exclusive, completely exhaustive
 
 Arguments:
 * `df` (pd.DataFrame): Dataframe to be split
 * `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
 * `splitting` (str): Name of column that represents individuals in the population that is getting split
 * `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
 perform a static split, i.e. not across timeseries, (default `None`)
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
+* `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
+(default: `0`)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.0.0 Summary: Generates A/B test
+Metadata-Version: 2.1 Name: absplit Version: 1.0.1 Summary: Generates A/B test
 groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
 formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.0.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.0.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -64,46 +64,48 @@
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
 'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
 groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
 generation fitness ab.fitness() # Visualise data ab.visualise() # Extract
 results df = ab.results ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
-ga_params={}, metric_weights={}, splits=[0.5, 0.5])` Splits population into 2
-groups. Mutually exclusive, completely exhaustive Arguments: * `df`
-(pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of, or list
-of names of, metric columns in DataFrame * `splitting` (str): Name of column
-that represents individuals in the population that is getting split *
-`date_col` (str, optional): Name of column that represents time periods, if
-applicable. If left empty, it will perform a static split, i.e. not across
-timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
-genetic algorithm `pygad.GA` module parameters, see [here](https://
-pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
-for arguments you can pass (default: `{}`) * `splits` (list, optional): How
-many groups to split into, and relative size of the groups (default: `[0.5,
-0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
-each metric in the data. If you want the splitting to focus on one metrics more
-than the other, you can prioritise this here (default: `{}`) ### Match `Match
-(population, sample, metrics, splitting, date_col=None, ga_params={},
-metric_weights={})` Takes DataFrame `sample` and finds a comparable group in
-`population`. Arguments: * `population` (pd.DataFrame): Population to search
-for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
-Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
-list of names of, metric columns in DataFrame * `splitting` (str): Name of
+ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
+population into 2 groups. Mutually exclusive, completely exhaustive Arguments:
+* `df` (pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of,
+or list of names of, metric columns in DataFrame * `splitting` (str): Name of
 column that represents individuals in the population that is getting split *
 `date_col` (str, optional): Name of column that represents time periods, if
 applicable. If left empty, it will perform a static split, i.e. not across
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
-0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
-each metric in the data. If you want the splitting to focus on one metrics more
-than the other, you can prioritise this here (default: `{}`)
+0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
+weighting for differences in the population count between groups (default: `0`)
+* `metric_weights` (dict, optional): Weights for each metric in the data. If
+you want the splitting to focus on one metrics more than the other, you can
+prioritise this here (default: `{}`) ### Match `Match(population, sample,
+metrics, splitting, date_col=None, ga_params={}, metric_weights={})` Takes
+DataFrame `sample` and finds a comparable group in `population`. Arguments: *
+`population` (pd.DataFrame): Population to search for comparable group (**Must
+exclude sample data**) * `sample` (pd.DataFrame): Sample we are looking to find
+a match for. * `metrics` (str, list): Name of, or list of names of, metric
+columns in DataFrame * `splitting` (str): Name of column that represents
+individuals in the population that is getting split * `date_col` (str,
+optional): Name of column that represents time periods, if applicable. If left
+empty, it will perform a static split, i.e. not across timeseries, (default
+`None`) * `ga_params` (dict, optional): Parameters for the genetic algorithm
+`pygad.GA` module parameters, see [here](https://pygad.readthedocs.io/en/
+latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
+(default: `{}`) * `splits` (list, optional): How many groups to split into, and
+relative size of the groups (default: `[0.5, 0.5]`, 2 groups of equal size) *
+`metric_weights` (dict, optional): Weights for each metric in the data. If you
+want the splitting to focus on one metrics more than the other, you can
+prioritise this here (default: `{}`)
                                                                   (back_to_top)
 ## Contributing I welcome contributions to ABSplit! For major changes, please
 open an issue first to discuss what you would like to change. Please make sure
 to update tests as appropriate.
                                                                   (back_to_top)
 ## License [MIT](https://choosealicense.com/licenses/mit/)
                                                                   (back_to_top)
```

