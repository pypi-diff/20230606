# Comparing `tmp/absplit-0.1.5.tar.gz` & `tmp/absplit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-0.1.5.tar` & `absplit-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4958 2023-05-20 17:44:37.211000 absplit-0.1.5/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-02-18 09:50:13.578000 absplit-0.1.5/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      193 2023-02-18 09:50:13.614000 absplit-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-0.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-0.1.5/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0     6030 2023-05-20 17:38:11.538000 absplit-0.1.5/README.md
--rw-r--r--   0        0        0       62 2023-05-20 17:44:37.289000 absplit-0.1.5/absplit/__init__.py
--rw-r--r--   0        0        0     8213 2023-05-20 17:32:17.963000 absplit-0.1.5/absplit/data.py
--rw-r--r--   0        0        0    19949 2023-05-20 16:53:44.320000 absplit-0.1.5/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-0.1.5/absplit/param.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-0.1.5/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-05-20 17:47:05.965000 absplit-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-20 08:12:29.431000 absplit-0.1.5/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-0.1.5/tests/test_data.py
--rw-r--r--   0        0        0     2105 2023-02-18 09:46:26.249000 absplit-0.1.5/tests/test_ga.py
--rw-r--r--   0        0        0     7095 1970-01-01 00:00:00.000000 absplit-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-05-20 17:44:37.211000 absplit-1.0.0/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-02-18 09:50:13.578000 absplit-1.0.0/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-05 22:39:03.152000 absplit-1.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.0.0/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     6872 2023-06-05 23:18:41.806000 absplit-1.0.0/README.md
+-rw-r--r--   0        0        0       62 2023-06-05 22:46:15.889000 absplit-1.0.0/absplit/__init__.py
+-rw-r--r--   0        0        0     8775 2023-06-05 15:37:08.054000 absplit-1.0.0/absplit/data.py
+-rw-r--r--   0        0        0    21148 2023-06-05 23:13:31.496000 absplit-1.0.0/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.0.0/absplit/param.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.0.0/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-06-05 22:35:18.918000 absplit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-20 08:12:29.431000 absplit-1.0.0/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.0.0/tests/test_data.py
+-rw-r--r--   0        0        0     2078 2023-06-05 22:46:15.926000 absplit-1.0.0/tests/test_ga.py
+-rw-r--r--   0        0        0     7923 1970-01-01 00:00:00.000000 absplit-1.0.0/PKG-INFO
```

### Comparing `absplit-0.1.5/.gitignore` & `absplit-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-0.1.5/LICENSE` & `absplit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-0.1.5/README.md` & `absplit-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 <a name="readme-top"></a>
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
-Split your data into matching A/B groups
+Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-0.1.5-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
-    <li><a href="#tutorial">Tutorial</a></li>
+    <li><a href="#tutorial">Tutorials</a></li>
     <ul>
         <li><a href="#do-it-yourself">Do it yourself</a></li>
     </ul>
     <li><a href="#usage">Usage</a></li>
     <li><a href="#api-reference">API Reference</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
   </ol>
 </details>
 
 ## About the project
-ABSplit is a python package that uses a genetic algorithm to generate as equal as possible A/B test splits.
+ABSplit is a python package that uses a genetic algorithm to generate as equal as possible A/B, A/B/C, or A/B/n test splits.
 
-The project aims to provide a convenient solution for efficiently splitting population data into two distinct 
-groups (ABSplit) and finding matching samples that closely resemble a given original sample (Match). Whether you have static 
-population data or time series data, this Python package simplifies the process and allows you to 
-analyze and manipulate your data effectively.
+The project aims to provide a convenient and efficient way for splitting population data into distinct 
+groups (ABSplit), as well as and finding matching samples that closely resemble a given original sample (Match).
+
+
+Whether you have static population data or time series data, this Python package simplifies the process and allows you to 
+analyze and manipulate your population data.
 
 This covers the following use cases:
-1. Splitting an entire population into 2 groups
-2. Finding a matching set in the population for a given sample
+1. **ABSplit class**: Splitting an entire population into n groups by given proportions
+2. **Match class**: Finding a matching group in a population for a given sample
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Getting Started
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install ABSplit and it's prerequisites
-### Prerequisites
-```bash
-pip install pygad==3.0.1 numpy sklearn pandas seaborn
-```
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install ABSplit and it's prerequisites.
+
+ABSplit requires `pygad==3.0.1`
+
 ### Installation
 
 ```bash
 pip install absplit
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Tutorials
 Please see [this colab](https://colab.research.google.com/drive/1gL7dxDJrtVoO5m1mSUWutdr7yas7sZwI?usp=sharing) for 
 a range of examples on how to use ABSplit and Match
 
 ### Do it yourself
-Learn how ABSplit works under the hood, and how to build your own group splitting tool using [PyGAD](https://pypi.org/project/pygad/),
-check out [this colab](https://colab.research.google.com/drive/1SlCNnOtN4WCDTSJHsFrZtI7gKcXEl8-C?usp=sharing)
+See [this colab](https://colab.research.google.com/drive/1SlCNnOtN4WCDTSJHsFrZtI7gKcXEl8-C?usp=sharing) to learn how 
+ABSplit works under the hood, and how to build your own group splitting tool using 
+[PyGAD](https://pypi.org/project/pygad/),
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Usage
 
 ```python
 from absplit import ABSplit
@@ -99,14 +101,15 @@
     'date_col': 'date',
     'splitting': 'city'
 }
 
 # Initialise
 ab = ABSplit(
     df=df,
+    split=[.5, .5],  # Split into 2 groups of equal size
     **kwargs,
 )
 
 # Generate split
 ab.run()
 
 # Visualise generation fitness
@@ -118,46 +121,57 @@
 # Extract results
 df = ab.results
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
-`ABSplit(df, ga_params={}, metric_weights={}, **kwargs)`
+`ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5])`
 
 Splits population into 2 groups. Mutually exclusive, completely exhaustive
 
 Arguments:
 * `df` (pd.DataFrame): Dataframe to be split
 * `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
-* `splitting` (str): Name of column that represents individual in the population that is getting split
-* `date_col` (str, optional): Name of column that represents time periods, if applicable.
-* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters (default: {})
-* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on one metrics more than the other, you can prioritise this here (default: {})
+* `splitting` (str): Name of column that represents individuals in the population that is getting split
+* `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
+perform a static split, i.e. not across timeseries, (default `None`)
+* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
+[here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
+(default: `{}`)
+* `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
+2 groups of equal size)
+* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
+one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
-`Match(population, sample, ga_params={}, metric_weights={}, **kwargs)`
+`Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
 
 Takes DataFrame `sample` and finds a comparable group in `population`.
 
 Arguments:
-* `population` (pd.DataFrame): Population to search  for comparable group. Must exclude sample data.
+* `population` (pd.DataFrame): Population to search  for comparable group (**Must exclude sample data**)
 * `sample` (pd.DataFrame): Sample we are looking to find a match for.
 * `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
-* `splitting` (str): Name of column that represents individual in the population that is getting split
-* `date_col` (str, optional): Name of column that represents time periods, if applicable.
-* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters (default: {})
-* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on one metrics more than the other, you can prioritise this here (default: {})
-
+* `splitting` (str): Name of column that represents individuals in the population that is getting split
+* `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
+perform a static split, i.e. not across timeseries, (default `None`)
+* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
+[here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
+(default: `{}`)
+* `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
+2 groups of equal size)
+* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
+one metrics more than the other, you can prioritise this here (default: `{}`)
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Contributing
 
-I welcome contributions to absplit! For major changes, please open an issue first
+I welcome contributions to ABSplit! For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## License
```

#### html2text {}

```diff
@@ -1,82 +1,92 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
-  Split your data into matching A/B groups ![license](https://img.shields.io/
+ Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 0.1.5-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.0.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
-          o Prerequisites
           o Installation
-   3. Tutorial
+   3. Tutorials
           o Do_it_yourself
    4. Usage
    5. API_Reference
    6. Contributing
    7. License
    8. Contact
  ## About the project ABSplit is a python package that uses a genetic algorithm
-to generate as equal as possible A/B test splits. The project aims to provide a
-convenient solution for efficiently splitting population data into two distinct
-groups (ABSplit) and finding matching samples that closely resemble a given
-original sample (Match). Whether you have static population data or time series
-data, this Python package simplifies the process and allows you to analyze and
-manipulate your data effectively. This covers the following use cases: 1.
-Splitting an entire population into 2 groups 2. Finding a matching set in the
+to generate as equal as possible A/B, A/B/C, or A/B/n test splits. The project
+aims to provide a convenient and efficient way for splitting population data
+into distinct groups (ABSplit), as well as and finding matching samples that
+closely resemble a given original sample (Match). Whether you have static
+population data or time series data, this Python package simplifies the process
+and allows you to analyze and manipulate your population data. This covers the
+following use cases: 1. **ABSplit class**: Splitting an entire population into
+n groups by given proportions 2. **Match class**: Finding a matching group in a
 population for a given sample
                                                                   (back_to_top)
 ## Getting Started Use the package manager [pip](https://pip.pypa.io/en/stable/
-) to install ABSplit and it's prerequisites ### Prerequisites ```bash pip
-install pygad==3.0.1 numpy sklearn pandas seaborn ``` ### Installation ```bash
-pip install absplit ```
+) to install ABSplit and it's prerequisites. ABSplit requires `pygad==3.0.1`
+### Installation ```bash pip install absplit ```
                                                                   (back_to_top)
 ## Tutorials Please see [this colab](https://colab.research.google.com/drive/
 1gL7dxDJrtVoO5m1mSUWutdr7yas7sZwI?usp=sharing) for a range of examples on how
-to use ABSplit and Match ### Do it yourself Learn how ABSplit works under the
-hood, and how to build your own group splitting tool using [PyGAD](https://
-pypi.org/project/pygad/), check out [this colab](https://
+to use ABSplit and Match ### Do it yourself See [this colab](https://
 colab.research.google.com/drive/1SlCNnOtN4WCDTSJHsFrZtI7gKcXEl8-C?usp=sharing)
+to learn how ABSplit works under the hood, and how to build your own group
+splitting tool using [PyGAD](https://pypi.org/project/pygad/),
                                                                   (back_to_top)
 ## Usage ```python from absplit import ABSplit import pandas as pd import
 datetime import numpy as np # Synthetic data data_dct = { 'date':
 [datetime.date(2030,4,1) + datetime.timedelta(days=x) for x in range(3)]*5,
 'country': ['UK'] * 15, 'region': [item for sublist in [[x]*6 for x in ['z',
 'y']] for item in sublist] + ['x']*3, 'city': [item for sublist in [[x]*3 for x
 in ['a', 'b', 'c', 'd', 'e']] for item in sublist], 'metric1': np.arange(0, 15,
 1), 'metric2': np.arange(0, 150, 10) } df = pd.DataFrame(data_dct) # Identify
 which columns are metrics, which is the time period, and what to split on
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
-'city' } # Initialise ab = ABSplit( df=df, **kwargs, ) # Generate split ab.run
-() # Visualise generation fitness ab.fitness() # Visualise data ab.visualise()
-# Extract results df = ab.results ```
-                                                                  (back_to_top)
-## API Reference ### Absplit `ABSplit(df, ga_params={}, metric_weights={},
-**kwargs)` Splits population into 2 groups. Mutually exclusive, completely
-exhaustive Arguments: * `df` (pd.DataFrame): Dataframe to be split * `metrics`
-(str, list): Name of, or list of names of, metric columns in DataFrame *
-`splitting` (str): Name of column that represents individual in the population
-that is getting split * `date_col` (str, optional): Name of column that
-represents time periods, if applicable. * `ga_params` (dict, optional):
-Parameters for the genetic algorithm `pygad.GA` module parameters (default: {})
-* `metric_weights` (dict, optional): Weights for each metric in the data. If
-you want the splitting to focus on one metrics more than the other, you can
-prioritise this here (default: {}) ### Match `Match(population, sample,
-ga_params={}, metric_weights={}, **kwargs)` Takes DataFrame `sample` and finds
-a comparable group in `population`. Arguments: * `population` (pd.DataFrame):
-Population to search for comparable group. Must exclude sample data. * `sample`
-(pd.DataFrame): Sample we are looking to find a match for. * `metrics` (str,
-list): Name of, or list of names of, metric columns in DataFrame * `splitting`
-(str): Name of column that represents individual in the population that is
-getting split * `date_col` (str, optional): Name of column that represents time
-periods, if applicable. * `ga_params` (dict, optional): Parameters for the
-genetic algorithm `pygad.GA` module parameters (default: {}) * `metric_weights`
-(dict, optional): Weights for each metric in the data. If you want the
-splitting to focus on one metrics more than the other, you can prioritise this
-here (default: {})
+'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
+groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
+generation fitness ab.fitness() # Visualise data ab.visualise() # Extract
+results df = ab.results ```
+                                                                  (back_to_top)
+## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
+ga_params={}, metric_weights={}, splits=[0.5, 0.5])` Splits population into 2
+groups. Mutually exclusive, completely exhaustive Arguments: * `df`
+(pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of, or list
+of names of, metric columns in DataFrame * `splitting` (str): Name of column
+that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
+pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
+for arguments you can pass (default: `{}`) * `splits` (list, optional): How
+many groups to split into, and relative size of the groups (default: `[0.5,
+0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
+each metric in the data. If you want the splitting to focus on one metrics more
+than the other, you can prioritise this here (default: `{}`) ### Match `Match
+(population, sample, metrics, splitting, date_col=None, ga_params={},
+metric_weights={})` Takes DataFrame `sample` and finds a comparable group in
+`population`. Arguments: * `population` (pd.DataFrame): Population to search
+for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
+Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
+list of names of, metric columns in DataFrame * `splitting` (str): Name of
+column that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
+pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
+for arguments you can pass (default: `{}`) * `splits` (list, optional): How
+many groups to split into, and relative size of the groups (default: `[0.5,
+0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
+each metric in the data. If you want the splitting to focus on one metrics more
+than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
-## Contributing I welcome contributions to absplit! For major changes, please
+## Contributing I welcome contributions to ABSplit! For major changes, please
 open an issue first to discuss what you would like to change. Please make sure
 to update tests as appropriate.
                                                                   (back_to_top)
 ## License [MIT](https://choosealicense.com/licenses/mit/)
                                                                   (back_to_top)
```

### Comparing `absplit-0.1.5/absplit/data.py` & `absplit-1.0.0/absplit/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,32 @@
         for col in self.remainder_cols:
             dtype = self._df_stacked[col].dtype
             if not dtype == 'object':
                 print(f'Column \'{col}\' will be treated as a variable to split on. Normally additional splitting'
                       f'columns are of type object, this is type {dtype}, this could cause problems in splitting. '
                       'Please check your kwargs are correct and remove any metrics you dont intend on splitting on.')
 
+    # groups = np.array([(solution == i).astype(int) for i in range(3)])
+    # # print(groups.shape)
+    #
+    # w = np.array([1, 0.5, 1])
+    # costs = (groups @ all_metrics_global)
+    # # print(costs.shape)
+    # costs *= w.reshape(1, -1, 1)
+    # # print(costs.shape)
+    #
+    # # print(costs.shape)
+    # # return
+    # diffs = np.roll(costs, -1, axis=0) - costs
+    # mse = ((diffs ** 2).mean(axis=1)).sum()
+    #
+    # # Fitness
+    # fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
+    # return fitness
+
     def _extract_metadata(self):
         """Extracts metadata used for 3D transformation from unstacked dataframe, builds transformation tuple
 
         Returns:
             None
         """
```

### Comparing `absplit-0.1.5/absplit/ga.py` & `absplit-1.0.0/absplit/ga.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,38 +62,40 @@
 
     Attributes:
         _default_ga_params (dict): Default parameters for genetic algorithm
         params (dict): PyGAD GA module parameters to be implemented
 
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, splits, **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             **kwargs: Genetic algorithm parameters
         """
         global fitness_func_absplit
+        self._splits = splits
+        self._splits_num = len(self._splits)
 
         # Default parameters
         self._default_ga_params = dict(
             # -- General Genetic Algorithm params --
             num_generations=200,
             sol_per_pop=100,
             num_parents_mating=5,
             mutation_type='scramble',
             mutation_probability=0.1,
             fitness_func=fitness_func_absplit,
             keep_elitism=1,
 
             # -- Binary Genetic Algorithm specific parameters --
             init_range_low=0,
-            init_range_high=2,
+            init_range_high=self._splits_num,
             random_mutation_min_val=0,
-            random_mutation_max_val=2,
+            random_mutation_max_val=self._splits_num,
             gene_type=int,
         )
 
         self._dont_touch = [
             'init_range_low',
             'init_range_high',
             'random_mutation_min_val',
@@ -113,17 +115,18 @@
         """
 
         # Update if args passed
         if kwargs:
             for key, value in kwargs.items():
                 if key in self._dont_touch:
                     print(f'Parameter \'{key}\' is essential to running the genetic algorithm as a'\
-                          f'binary genetic algorith, and so you\'re not allowed to modify this')
+                          f'discrete genetic algorith, and so you\'re not allowed to modify this')
                     continue
-                print(f'[Updating] {key} to {value}')
+                if not callable(value):
+                    print(f'[Updating] {key} to {value}')
                 self.params[key] = value
 
 
 class SplitBase(ParamMixin):
     """Base class for genetic algorithm orchestration.
 
     Manages applying different weights to costs, using multiple runs, extracting and visualising results.
@@ -147,28 +150,30 @@
     Methods:
         _cost_weighting(): Modifies cost weighting array
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
-    def __init__(self, ga_params={}, metric_weights={}, runs=1, **kwargs):
+    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             ga_params (dict, optional): Genetic algorithm parameters to add/modify
             metric_weights (dict, optional): Cost weightings to apply to metrics
             runs (int, optional): How many runs to try
             **kwargs: Additional keyword arguments
         """
         super().__init__(**kwargs)
         if ga_params:
             assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
         self._runs = runs
-        self._ga_params = GAParams(**ga_params)
+        self._splits = splits
+        self._splits_num = len(self._splits)
+        self._ga_params = GAParams(splits=splits, **ga_params)
         self._best_score = -1
         self._metric_weights = metric_weights
         self._df = None
         self._population = None
         self._df_result = None  # Final results dataframe
         self._ga = None  # genetic algorithm instance
         self._df_vis = None  # Visualisation dataframe
@@ -202,14 +207,17 @@
         """Runs genetic algorithm and returns bin splits into _df_result
 
         Returns:
             None
         """
 
         global all_metrics_global
+        global splits_global
+        splits_global = np.array(self._splits).sum() / np.array(self._splits)
+
         logger.debug('Splitting..')
         all_metrics_global = self._population.matrix
 
         # Run multiple times, save the best solution
         for i in range(self._runs):
             if self._runs > 1:
                 print(f'[Run {i+1}]')
@@ -294,15 +302,17 @@
             ax = [ax]
 
         # Plot each metric
         for i, metric in enumerate(vis_metrics):
 
             # If over time, plot line graph, else bar
             if self.date_col:
-                sns.lineplot(data=df, x=self.date_col, y=metric, hue='bin', ax=ax[i])
+                palette = ["C0", "C1", "k"][:self._splits_num]
+
+                sns.lineplot(data=df, x=self.date_col, y=metric, hue='bin', ax=ax[i], palette='Dark2')
             else:
                 df['metric'] = metric
                 sns.barplot(data=df, x='metric', y=metric, hue='bin', ax=ax[i])
 
             ax[i].set_title(f'{metric.title()}')
             ax[i].tick_params(axis='x', labelrotation=45)
 
@@ -460,15 +470,16 @@
         """
 
         # Specify fitness function
         global fitness_func_match
         ga_params['fitness_func'] = fitness_func_match
         ga_params['mutation_type'] = 'scramble'
         super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
-
+        self._splits = [0.5, 0.5]
+        self._splits_num = 2
         self._df_pop = population
         self._df_samp = sample
 
         # Ensure consistent dates between sample and population
         if self.date_col:
             mdp = MatchDataProc(df_pop=self._df_pop, df_samp=self._df_samp, **kwargs)
             self._df_pop = mdp.population.reset_index()
@@ -535,19 +546,32 @@
 
 
 def fitness_func_absplit(ga_instance, solution, solution_idx):
     """Fitness function for ABSplit
     """
     global all_metrics_global
     global metric_weights_global
+    global splits_global
 
-    cost1 = solution @ all_metrics_global
-    cost2 = (1 - solution) @ all_metrics_global
-    # Average over time axis, sum over metric axis
-    mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
+    # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
+    groups = np.array([(solution == i).astype(int) for i in range(len(splits_global))])
+
+    # Size penalty
+    # Calculate all_metrics mean * number of days * number of metrics
+    mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
+    # Get size cost for each group
+    mean_group = (groups * mean).sum(1) * splits_global
+    # Calculate group differences, sum
+    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum())
+
+    # Metric cost
+    costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1))
+    diffs = np.roll(costs, -1, axis=1) - costs
+    mse = ((diffs ** 2).mean(axis=1)).sum()
+    mse = mse + size_cost
 
     # Fitness
     fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
     return fitness
 
 
 def fitness_func_match(ga_instance, solution, solution_idx):
@@ -561,7 +585,10 @@
     cost2 = solution @ all_metrics_global
     # Average over time axis, sum over metric axis
     mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
 
     # Fitness
     fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
     return fitness
+
+
+fitness_func_match.__name__ = 'fitness_function_match'
```

### Comparing `absplit-0.1.5/absplit/param.py` & `absplit-1.0.0/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-0.1.5/images/logo.jpeg` & `absplit-1.0.0/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-0.1.5/pyproject.toml` & `absplit-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "0.1.5"
+version = "1.0.0"
 description = "Generates A/B test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-0.1.5/tests/test_data.py` & `absplit-1.0.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-0.1.5/tests/test_ga.py` & `absplit-1.0.0/tests/test_ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 }
 df = pd.DataFrame(data_dct)
 
 # Column kwargs
 kwargs = {
     'metrics': ['metric1', 'metric2'],
     'date_col': 'date',
-    'split_by': 'region',
     'splitting': 'city'
 }
 
 # Initialise and run
 ab = ABSplit(
     df=df,
     **kwargs,
```

### Comparing `absplit-0.1.5/PKG-INFO` & `absplit-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 0.1.5
+Version: 1.0.0
 Summary: Generates A/B test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,82 +28,84 @@
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 
 <a name="readme-top"></a>
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
-Split your data into matching A/B groups
+Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-0.1.5-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
     <li>
       <a href="#about-the-project">About The Project</a>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
         <li><a href="#installation">Installation</a></li>
       </ul>
     </li>
-    <li><a href="#tutorial">Tutorial</a></li>
+    <li><a href="#tutorial">Tutorials</a></li>
     <ul>
         <li><a href="#do-it-yourself">Do it yourself</a></li>
     </ul>
     <li><a href="#usage">Usage</a></li>
     <li><a href="#api-reference">API Reference</a></li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
   </ol>
 </details>
 
 ## About the project
-ABSplit is a python package that uses a genetic algorithm to generate as equal as possible A/B test splits.
+ABSplit is a python package that uses a genetic algorithm to generate as equal as possible A/B, A/B/C, or A/B/n test splits.
 
-The project aims to provide a convenient solution for efficiently splitting population data into two distinct 
-groups (ABSplit) and finding matching samples that closely resemble a given original sample (Match). Whether you have static 
-population data or time series data, this Python package simplifies the process and allows you to 
-analyze and manipulate your data effectively.
+The project aims to provide a convenient and efficient way for splitting population data into distinct 
+groups (ABSplit), as well as and finding matching samples that closely resemble a given original sample (Match).
+
+
+Whether you have static population data or time series data, this Python package simplifies the process and allows you to 
+analyze and manipulate your population data.
 
 This covers the following use cases:
-1. Splitting an entire population into 2 groups
-2. Finding a matching set in the population for a given sample
+1. **ABSplit class**: Splitting an entire population into n groups by given proportions
+2. **Match class**: Finding a matching group in a population for a given sample
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Getting Started
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install ABSplit and it's prerequisites
-### Prerequisites
-```bash
-pip install pygad==3.0.1 numpy sklearn pandas seaborn
-```
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install ABSplit and it's prerequisites.
+
+ABSplit requires `pygad==3.0.1`
+
 ### Installation
 
 ```bash
 pip install absplit
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Tutorials
 Please see [this colab](https://colab.research.google.com/drive/1gL7dxDJrtVoO5m1mSUWutdr7yas7sZwI?usp=sharing) for 
 a range of examples on how to use ABSplit and Match
 
 ### Do it yourself
-Learn how ABSplit works under the hood, and how to build your own group splitting tool using [PyGAD](https://pypi.org/project/pygad/),
-check out [this colab](https://colab.research.google.com/drive/1SlCNnOtN4WCDTSJHsFrZtI7gKcXEl8-C?usp=sharing)
+See [this colab](https://colab.research.google.com/drive/1SlCNnOtN4WCDTSJHsFrZtI7gKcXEl8-C?usp=sharing) to learn how 
+ABSplit works under the hood, and how to build your own group splitting tool using 
+[PyGAD](https://pypi.org/project/pygad/),
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Usage
 
 ```python
 from absplit import ABSplit
@@ -128,14 +130,15 @@
     'date_col': 'date',
     'splitting': 'city'
 }
 
 # Initialise
 ab = ABSplit(
     df=df,
+    split=[.5, .5],  # Split into 2 groups of equal size
     **kwargs,
 )
 
 # Generate split
 ab.run()
 
 # Visualise generation fitness
@@ -147,46 +150,57 @@
 # Extract results
 df = ab.results
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
-`ABSplit(df, ga_params={}, metric_weights={}, **kwargs)`
+`ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5])`
 
 Splits population into 2 groups. Mutually exclusive, completely exhaustive
 
 Arguments:
 * `df` (pd.DataFrame): Dataframe to be split
 * `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
-* `splitting` (str): Name of column that represents individual in the population that is getting split
-* `date_col` (str, optional): Name of column that represents time periods, if applicable.
-* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters (default: {})
-* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on one metrics more than the other, you can prioritise this here (default: {})
+* `splitting` (str): Name of column that represents individuals in the population that is getting split
+* `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
+perform a static split, i.e. not across timeseries, (default `None`)
+* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
+[here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
+(default: `{}`)
+* `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
+2 groups of equal size)
+* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
+one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
-`Match(population, sample, ga_params={}, metric_weights={}, **kwargs)`
+`Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
 
 Takes DataFrame `sample` and finds a comparable group in `population`.
 
 Arguments:
-* `population` (pd.DataFrame): Population to search  for comparable group. Must exclude sample data.
+* `population` (pd.DataFrame): Population to search  for comparable group (**Must exclude sample data**)
 * `sample` (pd.DataFrame): Sample we are looking to find a match for.
 * `metrics` (str, list): Name of, or list of names of, metric columns in DataFrame
-* `splitting` (str): Name of column that represents individual in the population that is getting split
-* `date_col` (str, optional): Name of column that represents time periods, if applicable.
-* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters (default: {})
-* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on one metrics more than the other, you can prioritise this here (default: {})
-
+* `splitting` (str): Name of column that represents individuals in the population that is getting split
+* `date_col` (str, optional): Name of column that represents time periods, if applicable. If left empty, it will
+perform a static split, i.e. not across timeseries, (default `None`)
+* `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
+[here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
+(default: `{}`)
+* `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
+2 groups of equal size)
+* `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
+one metrics more than the other, you can prioritise this here (default: `{}`)
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Contributing
 
-I welcome contributions to absplit! For major changes, please open an issue first
+I welcome contributions to ABSplit! For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 0.1.5 Summary: Generates A/B test
+Metadata-Version: 2.1 Name: absplit Version: 1.0.0 Summary: Generates A/B test
 groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
 formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -13,87 +13,97 @@
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Scientific/
 Engineering :: Visualization Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
-  Split your data into matching A/B groups ![license](https://img.shields.io/
+ Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 0.1.5-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.0.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
-          o Prerequisites
           o Installation
-   3. Tutorial
+   3. Tutorials
           o Do_it_yourself
    4. Usage
    5. API_Reference
    6. Contributing
    7. License
    8. Contact
  ## About the project ABSplit is a python package that uses a genetic algorithm
-to generate as equal as possible A/B test splits. The project aims to provide a
-convenient solution for efficiently splitting population data into two distinct
-groups (ABSplit) and finding matching samples that closely resemble a given
-original sample (Match). Whether you have static population data or time series
-data, this Python package simplifies the process and allows you to analyze and
-manipulate your data effectively. This covers the following use cases: 1.
-Splitting an entire population into 2 groups 2. Finding a matching set in the
+to generate as equal as possible A/B, A/B/C, or A/B/n test splits. The project
+aims to provide a convenient and efficient way for splitting population data
+into distinct groups (ABSplit), as well as and finding matching samples that
+closely resemble a given original sample (Match). Whether you have static
+population data or time series data, this Python package simplifies the process
+and allows you to analyze and manipulate your population data. This covers the
+following use cases: 1. **ABSplit class**: Splitting an entire population into
+n groups by given proportions 2. **Match class**: Finding a matching group in a
 population for a given sample
                                                                   (back_to_top)
 ## Getting Started Use the package manager [pip](https://pip.pypa.io/en/stable/
-) to install ABSplit and it's prerequisites ### Prerequisites ```bash pip
-install pygad==3.0.1 numpy sklearn pandas seaborn ``` ### Installation ```bash
-pip install absplit ```
+) to install ABSplit and it's prerequisites. ABSplit requires `pygad==3.0.1`
+### Installation ```bash pip install absplit ```
                                                                   (back_to_top)
 ## Tutorials Please see [this colab](https://colab.research.google.com/drive/
 1gL7dxDJrtVoO5m1mSUWutdr7yas7sZwI?usp=sharing) for a range of examples on how
-to use ABSplit and Match ### Do it yourself Learn how ABSplit works under the
-hood, and how to build your own group splitting tool using [PyGAD](https://
-pypi.org/project/pygad/), check out [this colab](https://
+to use ABSplit and Match ### Do it yourself See [this colab](https://
 colab.research.google.com/drive/1SlCNnOtN4WCDTSJHsFrZtI7gKcXEl8-C?usp=sharing)
+to learn how ABSplit works under the hood, and how to build your own group
+splitting tool using [PyGAD](https://pypi.org/project/pygad/),
                                                                   (back_to_top)
 ## Usage ```python from absplit import ABSplit import pandas as pd import
 datetime import numpy as np # Synthetic data data_dct = { 'date':
 [datetime.date(2030,4,1) + datetime.timedelta(days=x) for x in range(3)]*5,
 'country': ['UK'] * 15, 'region': [item for sublist in [[x]*6 for x in ['z',
 'y']] for item in sublist] + ['x']*3, 'city': [item for sublist in [[x]*3 for x
 in ['a', 'b', 'c', 'd', 'e']] for item in sublist], 'metric1': np.arange(0, 15,
 1), 'metric2': np.arange(0, 150, 10) } df = pd.DataFrame(data_dct) # Identify
 which columns are metrics, which is the time period, and what to split on
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
-'city' } # Initialise ab = ABSplit( df=df, **kwargs, ) # Generate split ab.run
-() # Visualise generation fitness ab.fitness() # Visualise data ab.visualise()
-# Extract results df = ab.results ```
-                                                                  (back_to_top)
-## API Reference ### Absplit `ABSplit(df, ga_params={}, metric_weights={},
-**kwargs)` Splits population into 2 groups. Mutually exclusive, completely
-exhaustive Arguments: * `df` (pd.DataFrame): Dataframe to be split * `metrics`
-(str, list): Name of, or list of names of, metric columns in DataFrame *
-`splitting` (str): Name of column that represents individual in the population
-that is getting split * `date_col` (str, optional): Name of column that
-represents time periods, if applicable. * `ga_params` (dict, optional):
-Parameters for the genetic algorithm `pygad.GA` module parameters (default: {})
-* `metric_weights` (dict, optional): Weights for each metric in the data. If
-you want the splitting to focus on one metrics more than the other, you can
-prioritise this here (default: {}) ### Match `Match(population, sample,
-ga_params={}, metric_weights={}, **kwargs)` Takes DataFrame `sample` and finds
-a comparable group in `population`. Arguments: * `population` (pd.DataFrame):
-Population to search for comparable group. Must exclude sample data. * `sample`
-(pd.DataFrame): Sample we are looking to find a match for. * `metrics` (str,
-list): Name of, or list of names of, metric columns in DataFrame * `splitting`
-(str): Name of column that represents individual in the population that is
-getting split * `date_col` (str, optional): Name of column that represents time
-periods, if applicable. * `ga_params` (dict, optional): Parameters for the
-genetic algorithm `pygad.GA` module parameters (default: {}) * `metric_weights`
-(dict, optional): Weights for each metric in the data. If you want the
-splitting to focus on one metrics more than the other, you can prioritise this
-here (default: {})
+'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
+groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
+generation fitness ab.fitness() # Visualise data ab.visualise() # Extract
+results df = ab.results ```
+                                                                  (back_to_top)
+## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
+ga_params={}, metric_weights={}, splits=[0.5, 0.5])` Splits population into 2
+groups. Mutually exclusive, completely exhaustive Arguments: * `df`
+(pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of, or list
+of names of, metric columns in DataFrame * `splitting` (str): Name of column
+that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
+pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
+for arguments you can pass (default: `{}`) * `splits` (list, optional): How
+many groups to split into, and relative size of the groups (default: `[0.5,
+0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
+each metric in the data. If you want the splitting to focus on one metrics more
+than the other, you can prioritise this here (default: `{}`) ### Match `Match
+(population, sample, metrics, splitting, date_col=None, ga_params={},
+metric_weights={})` Takes DataFrame `sample` and finds a comparable group in
+`population`. Arguments: * `population` (pd.DataFrame): Population to search
+for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
+Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
+list of names of, metric columns in DataFrame * `splitting` (str): Name of
+column that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
+pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
+for arguments you can pass (default: `{}`) * `splits` (list, optional): How
+many groups to split into, and relative size of the groups (default: `[0.5,
+0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
+each metric in the data. If you want the splitting to focus on one metrics more
+than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
-## Contributing I welcome contributions to absplit! For major changes, please
+## Contributing I welcome contributions to ABSplit! For major changes, please
 open an issue first to discuss what you would like to change. Please make sure
 to update tests as appropriate.
                                                                   (back_to_top)
 ## License [MIT](https://choosealicense.com/licenses/mit/)
                                                                   (back_to_top)
```

