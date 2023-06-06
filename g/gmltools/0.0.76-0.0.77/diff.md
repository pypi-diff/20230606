# Comparing `tmp/gmltools-0.0.76.tar.gz` & `tmp/gmltools-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.76.tar", last modified: Fri Jun  2 10:17:30 2023, max compression
+gzip compressed data, was "gmltools-0.0.77.tar", last modified: Tue Jun  6 10:55:44 2023, max compression
```

## Comparing `gmltools-0.0.76.tar` & `gmltools-0.0.77.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.328075 gmltools-0.0.76/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.76/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.76/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-06-02 10:17:30.328075 gmltools-0.0.76/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.76/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.138412 gmltools-0.0.76/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.76/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.76/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.76/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-06-02 10:15:53.000000 gmltools-0.0.76/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 10:17:30.329156 gmltools-0.0.76/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-02 10:15:42.000000 gmltools-0.0.76/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.035285 gmltools-0.0.76/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.160144 gmltools-0.0.76/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.76/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.76/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.207078 gmltools-0.0.76/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.76/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.76/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.273550 gmltools-0.0.76/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.76/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.76/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.76/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.76/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   127158 2023-06-02 10:16:23.000000 gmltools-0.0.76/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.76/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.76/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.295963 gmltools-0.0.76/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.76/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.76/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.76/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.327043 gmltools-0.0.76/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.76/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.76/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.76/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.76/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.194339 gmltools-0.0.76/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.243115 gmltools-0.0.77/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.77/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.77/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-06-06 10:55:44.243115 gmltools-0.0.77/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.77/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.035778 gmltools-0.0.77/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.77/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.77/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.77/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-06-06 10:53:29.000000 gmltools-0.0.77/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:55:44.243115 gmltools-0.0.77/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-06-06 10:54:46.000000 gmltools-0.0.77/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.005729 gmltools-0.0.77/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.046738 gmltools-0.0.77/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.77/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.77/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.090375 gmltools-0.0.77/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.77/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.77/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.176765 gmltools-0.0.77/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.77/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.77/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.77/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.77/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   160690 2023-06-06 10:49:51.000000 gmltools-0.0.77/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7037 2023-06-06 10:47:14.000000 gmltools-0.0.77/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.77/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.204694 gmltools-0.0.77/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.77/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.77/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.77/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.242176 gmltools-0.0.77/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.77/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.77/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.77/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.77/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.079414 gmltools-0.0.77/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.76/LICENSE` & `gmltools-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/Models.ipynb` & `gmltools-0.0.77/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/PKG-INFO` & `gmltools-0.0.77/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.76
+Version: 0.0.77
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.76/README.md` & `gmltools-0.0.77/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.77/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/gmltools.yml` & `gmltools-0.0.77/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/mltools.yml` & `gmltools-0.0.77/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/pyproject.toml` & `gmltools-0.0.77/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.76"
+version = "0.0.77"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.21.6"
 pandas = "^1.5.0"
 matplotlib = "^3.6.3"
 xgboost = "^1.5.0"
+linear-tree = "^0.3.5"
+lightgbm = "^3.3.5"
+scikit-learn = "^1.2.1"
+
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.15.2"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gmltools-0.0.76/setup.py` & `gmltools-0.0.77/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['gmltools','gmltools.preprocess','gmltools.eda','gmltools.models','gmltools.models_analysis']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
+['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.76',
+    'version': '0.0.77',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.76/src/gmltools/To_Do.txt` & `gmltools-0.0.77/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/eda/eda.py` & `gmltools-0.0.77/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/models/bayes.py` & `gmltools-0.0.77/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.77/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/models/dummy_model.py` & `gmltools-0.0.77/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/models/model.py` & `gmltools-0.0.77/src/gmltools/models/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #REGRESSION
 from sklearn.ensemble import RandomForestRegressor
 from xgboost import XGBRegressor
 from sklearn.linear_model import LinearRegression
 from sklearn.neighbors import KNeighborsRegressor
 from sklearn.neural_network import MLPRegressor
 from sklearn.tree import DecisionTreeRegressor
+from lineartree import LinearForestRegressor, LinearBoostRegressor
+from  lightgbm import LGBMRegressor
 from sklearn.svm import SVR
 
 
 
 #PREPROCESSING
 from sklearn.pipeline import Pipeline
 from sklearn.compose import ColumnTransformer
@@ -39,15 +41,17 @@
     lr_default_params_reg,
     mlp_default_params_clf,
     mlp_default_params_reg,
     knn_default_params_clf,
     knn_default_params_reg,
     dt_default_params_clf,
     dt_default_params_reg,
-    svr_default_params_reg
+    svr_default_params_reg,
+    lgbm_default_params_reg,
+    lb_default_params_reg
 )
 #import compute_sample_weight
 from sklearn.utils.class_weight import compute_sample_weight
 import joblib
 import os
 from openpyxl import load_workbook
 import time
@@ -238,14 +242,20 @@
                 self._model.fit(self.X_train, self.y_train, LR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'MLP':
                 self._model.fit(self.X_train, self.y_train, MLP__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'DT':
                 self._model.fit(self.X_train, self.y_train, DT__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'SVR':
                 self._model.fit(self.X_train, self.y_train, SVR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+
+            elif self.pipe.steps[-1][0] == 'LF':
+                self._model.fit(self.X_train, self.y_train, SVR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+
+            elif self.pipe.steps[-1][0] == 'LB':
+                self._model.fit(self.X_train, self.y_train, SVR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
         else:
             self._model.fit(X=self.X_train, y=self.y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
         return self._model
 
 
     
@@ -1217,14 +1227,32 @@
                 Number of iterations for bayesian optimization. The default is 30.
             
             random_state : int, optional
                 Random state. The default is None.
             
             n_jobs : int, optional
                 Number of jobs. The default is -1.
+
+            columns_lags : list, optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list, optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+               Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
             
             Returns
             -------
             model_ : sklearn model
                 Trained model.
             
             """
@@ -1320,14 +1348,34 @@
                 Number of iterations for bayesian optimization. The default is 30.
             
             random_state : int, optional
                 Random state. The default is None.
             
             n_jobs : int, optional
                 Number of jobs. The default is -1.
+
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional   
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+
             
             Returns
             -------
             model_ : sklearn model
                 Trained model.
             
             """
@@ -1421,15 +1469,35 @@
                 Number of iterations for bayesian optimization. The default is 30.
             
             random_state : int, optional
                 Random state. The default is None.
             
             n_jobs : int, optional
                 Number of jobs. The default is -1.
-            
+
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+
             Returns
             -------
             model_ : sklearn model
                 Trained model.
             
             """
 
@@ -1521,18 +1589,36 @@
                 Number of iterations for bayesian optimization. The default is 30.
             
             random_state : int, optional
                 Random state. The default is None.
             
             n_jobs : int, optional
                 Number of jobs. The default is -1.
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
             
             Returns
             -------
-            model_ : sklearn model
+            self.model : sklearn model
                 Trained model.
             
             """
 
             print(" INFO: Agurments params must start as 'KNN__param'" + '\n' "INFO: Default params in Documentation for KNN Regressor are: ", knn_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
@@ -1623,18 +1709,36 @@
                 Number of iterations for bayesian optimization. The default is 30.
             
             random_state : int, optional
                 Random state. The default is None.
             
             n_jobs : int, optional
                 Number of jobs. The default is -1.
-            
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+
             Returns
             -------
-            model_ : sklearn model
+            self.model : sklearn model
                 Trained model.
             
             """
 
             print(" INFO: Agurments params must start as 'DT__param'" + '\n' "INFO: Default params in Documentation for Decision Tree Regressor are: ", dt_default_params_reg)
             print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
             f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
@@ -1728,14 +1832,33 @@
 
             random_state : int, optional
                 Random state. The default is None.
 
             n_jobs : int, optional
                 Number of jobs. The default is -1.
 
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+        
             Returns
             -------
             None.
 
             """
             
 
@@ -1798,14 +1921,17 @@
                 Training set.
     
             y_train : pandas dataframe
                 Training set labels.
     
             ordinal_cat_cols : list, optional
                 List of ordinal categorical variables. The default is None.
+            
+            categories : list[str], optional
+                Categories for OneHotEncoder Interpretation. The default is 'auto'.
     
             scoring : str, optional
                 Evaluation metric. The default is 'neg_mean_squared_error'.
     
             grid_params : dict, optional
                 Dictionary of parameters for grid search. The default is
 
@@ -1829,14 +1955,33 @@
                 Number of iterations for bayesian optimization. The default is 30.
             
             random_state : int, optional
                 Random state. The default is None.
             
             n_jobs : int, optional
                 Number of jobs. The default is -1.
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+            
             
             Returns
             -------
             model_ : sklearn model
                 Trained model.
             
             """
@@ -1874,15 +2019,393 @@
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
-    
+
+
+    def LinearForest_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error', criterion='mse',
+                            grid_params={'LF__n_estimators': [100,200,300,400,500],
+                                'LF__max_depth': [None,2,3,4,5],
+                                'LF__min_samples_split': [2,3,4,],
+                                'LF__max_features': ['auto', 'sqrt', 'log2'],
+                                'LF__min_impurity_decrease': [0.0,0.1,0.2]},
+                            random_params=None, random_n_iter=10, bayes_pbounds=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
+                            columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
+        
+            """
+            This method performs a Decision Tree Regressor model with grid search or bayesian optimization.
+
+            Parameters
+            ----------
+            X_train : pandas
+                Training set.
+            
+            y_train : pandas 
+                Training set labels.
+
+            categories : list[str], optional
+                Categories for OneHotEncoder Interpretation. The default is 'auto'.
+            
+            ordinal_cat_cols : list, optional
+                List of ordinal categorical variables. The default is None.
+
+            scoring : str, optional
+                Evaluation metric. The default is 'neg_mean_squared_error'.
+            
+            grid_params : dict, optional
+                Dictionary of parameters for grid search. The default is
+
+            cv : int, optional
+                Number of folds for cross validation. The default is 10.
+                For time series data, cv must be a TimeSeriesSplit object.
+
+            random_params : dict, optional
+                Dictionary of parameters for random search. The default is None.
+
+            random_n_iter : int, optional
+                Number of iterations for random search. The default is 10.
+            
+            bayes_pbounds : dict, optional
+                Dictionary of parameters for bayesian optimization. The default is None.
+
+            bayes_int_params : list, optional
+                List of parameters for bayesian optimization that are integers. The default is None.
+
+            bayes_n_iter : int, optional
+                Number of iterations for bayesian optimization. The default is 30.
+
+            random_state : int, optional
+                Random state. The default is None.
+
+            n_jobs : int, optional
+                Number of jobs. The default is -1.
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+
+            Returns
+            -------
+            model_ : sklearn model
+                Trained model.
+
+            """
+
+            print(" INFO: Agurments params must start as 'LF__param'" + '\n' "INFO: Default params in Documentation for Linear Forest Regressor are: ", rf_default_params_reg)
+            print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
+            f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
+            f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
+            assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
+            assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
+            assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
+            assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
+            assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
+            assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
+            # DT__ is the prefix for every hyperparameter in the Decision Tree Regressor
+            if grid_params is not None and random_params is None and bayes_pbounds is None:
+                assert all('LF__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'LF__'"
+            elif random_params is not None:
+                assert all('LF__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'LF__'"
+            elif bayes_pbounds is not None:
+                assert all('LF__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LF__'"
+                assert all('LF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LF__'"
+            
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
+            pipe = Pipeline(steps=[('Prep', preprocessor),
+                                ('LF', LinearForestRegressor(base_estimator=LinearRegression(), criterion=criterion, random_state=random_state, n_jobs=n_jobs))]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
+
+
+
+    def LinearBoost_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error', criterion='mse',
+                            grid_params={'LB__n_estimators': [10,100,200,300,400,500],
+                                'LB__loss':["linear", "square", "absolute", "exponential"],
+                                'LB__max_depth': [None,2,3,4,5],
+                                'LB__min_samples_split': [2,3,4],
+                                'LB__max_features': ['auto', 'sqrt', 'log2'],
+                                'LB__min_impurity_decrease': [0.0,0.1,0.2]},
+                            random_params=None, random_n_iter=10, bayes_pbounds=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
+                            columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
+        
+            """
+            This method performs Linear Boosting Regressor from the following Library
+            https://github.com/cerlymarco/linear-tree/blob/main/lineartree/lineartree.py
+
+            Parameters
+            ----------
+            X_train : pandas
+                Training set.
+            
+            y_train : pandas 
+                Training set labels.
+
+            categories : list[str], optional
+                Categories for OneHotEncoder Interpretation. The default is 'auto'.
+            
+            ordinal_cat_cols : list, optional
+                List of ordinal categorical variables. The default is None.
+
+            scoring : str, optional
+                Evaluation metric. The default is 'neg_mean_squared_error'.
+            
+            grid_params : dict, optional
+                Dictionary of parameters for grid search. The default is
+
+            cv : int, optional
+                Number of folds for cross validation. The default is 10.
+                For time series data, cv must be a TimeSeriesSplit object.
+
+            random_params : dict, optional
+                Dictionary of parameters for random search. The default is None.
+            
+            random_n_iter : int, optional
+                Number of iterations for random search. The default is 10.
+
+            bayes_pbounds : dict, optional
+                Dictionary of parameters for bayesian optimization. The default is None.
+
+            bayes_int_params : list, optional   
+                List of parameters for bayesian optimization that are integers. The default is None.
+            
+            bayes_n_iter : int, optional
+                Number of iterations for bayesian optimization. The default is 30.
+
+            random_state : int, optional
+                Random state. The default is None.
+
+            n_jobs : int, optional
+                Number of jobs. The default is -1.
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+            
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+
+            
+            Returns
+            -------
+            model_ : sklearn model
+                Trained model.
+
+            """
+
+            print(" INFO: Agurments params must start as 'LB__param'" + '\n' "INFO: Default params in Documentation for Linear Boosting Regressor are: ", lb_default_params_reg)
+            print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
+            f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
+            f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
+            assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
+            assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
+            assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
+            assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
+            assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
+            assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
+            # DT__ is the prefix for every hyperparameter in the Decision Tree Regressor
+            if grid_params is not None and random_params is None and bayes_pbounds is None:
+                assert all('LB__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'LF__'"
+            elif random_params is not None:
+                assert all('LB__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'LF__'"
+            elif bayes_pbounds is not None:
+                assert all('LB__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LF__'"
+                assert all('LB__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LF__'"
+            
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
+            pipe = Pipeline(steps=[('Prep', preprocessor),
+                                ('LB', LinearBoostRegressor(base_estimator=LinearRegression(), criterion=criterion, random_state=random_state))]) # Model always the last step
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
+
+
+    def LightGBM_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
+                            grid_params={'LGBM__n_estimators': [100,200,300,400,500],
+                                    'LGBM__boosting_type': ['gbdt', 'dart', 'goss', 'rf'],
+                                    'LGBM__objective': [None],
+                                    'LGBM__num_leaves': [31, 127, 255],
+                                    'LGBM__max_depth': [-1,2,3,4,5],
+                                    'LGBM__learning_rate': [0.1,0.001],
+                                    'LGBM__subsample_for_bin': [200000, 500000],
+                                    'LGBM__min_split_gain':[0.0],
+                                    'LGBM__min_child_weight': [0.001],
+                                    'LGBM__min_child_samples':[20],
+                                    'LGBM__subsample':[1.0],
+                                    'LGBM__subsample_freq':[0], 
+                                    'LGBM__colsample_bytree':[1.0]},
+                            random_params=None, random_n_iter=10, bayes_pbounds=None,
+                            bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
+                            columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
+        
+            """
+            This method performs a LightGBM Regressor model with grid search random search or  bayesian optimization.
+            Bayesian optimization for forescating recusrive lgas option is not available yet.
+            https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMRegressor.html
+
+            Parameters
+            ----------
+            X_train : pandas
+                Training set.
+
+            y_train : pandas
+                Training set labels.
+
+            ordinal_cat_cols : list, optional
+                List of ordinal categorical variables. The default is None.
+
+            categories : list[str], optional
+                Categories for OneHotEncoder Interpretation. The default is 'auto'.
+
+            scoring : str, optional
+                Evaluation metric. The default is 'neg_mean_squared_error'.
+
+            grid_params : dict, optional
+                Dictionary of parameters for grid search. The default is
+            
+            cv : int, optional
+                Number of folds for cross validation. The default is 10.
+                For time series data, cv must be a TimeSeriesSplit object.
+
+            random_params : dict, optional
+                Dictionary of parameters for random search. The default is None.
+            
+            random_n_iter : int, optional
+                Number of iterations for random search. The default is 10.
+
+            bayes_pbounds : dict, optional
+                Dictionary of parameters for bayesian optimization. The default is None.
+
+            bayes_int_params : list, optional
+                List of parameters for bayesian optimization that are integers. The default is None.    
+            
+            bayes_n_iter : int, optional
+                Number of iterations for bayesian optimization. The default is 30.
+
+            random_state : int, optional
+                Random state. The default is None.
+
+            n_jobs : int, optional
+                Number of jobs. The default is -1.
+
+            columns_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recursive. The default is None.
+
+            column_rolled_lags : list[int], optional
+                List of columns iloc position to apply lags for Forecasting Recusrive Rolling. The default is None.
+
+            lags : list[int], optional
+                Value Number of lags to apply for Forecasting Recursive. The default is None.
+
+            rolled_lags : list[int], optional
+                Value  Number of lags to apply for Forecasting Recursive Rolling. The default is None.
+
+            rolled_metrics : list, optional 
+                List of metrics to apply for Forecasting Recursive Rolling. The default is None.
+            
+            column_rolled_lags_initial : int, optional
+                Int where from prevoiuosly register rolled lags starts computing. The default is None. Ususally use 1.
+
+            Returns
+            -------
+            model_ : sklearn model
+                Trained model.
+
+            """
+
+
+            print(" INFO: Agurments params must start as 'LGBM__param'" + '\n' "INFO: Default params in Documentation for LightGBM Regressor are: ", lgbm_default_params_reg)
+            print("\n"+ "INFO: Default params RUN for this model are: ", f'grid_params = {grid_params}',f'scoring = {scoring}',
+            f'bayes_n_iter = {bayes_n_iter}', f'bayes_pbounds = {bayes_pbounds}',
+            f'bayes_int_params = {bayes_int_params}', f'ordinal_cat_cols = {ordinal_cat_cols}', f'random_state = {random_state}', f'n_jobs = {n_jobs}')
+            assert self.X_train is not None and self.y_train is not None, "X_train and y_train must be provided, when initializing the class"
+            assert ordinal_cat_cols is None or isinstance(ordinal_cat_cols, list), "In case of ordinal categorical variables, ordinal_cat_cols must be a list of column names"
+            assert grid_params is None or isinstance(grid_params, dict), "In case of grid search, grid_param_grid must be a dictionary of parameter bounds"
+            assert bayes_pbounds is None or isinstance(bayes_pbounds, dict), "In case of bayesian optimization, bayes_pbounds must be a dictionary of parameter bounds"
+            assert random_params is None or isinstance(random_params, dict), "In case of random search, random_params must be a dictionary of parameter bounds"
+            assert bayes_int_params is None or isinstance(bayes_int_params, list), "In case of bayesian optimization, bayes_int_params must be a list of parameter names"
+            assert isinstance(bayes_n_iter,int), "In case of bayesian optimization, bayes_n_iter must be an integer"
+            # DT__ is the prefix for every hyperparameter in the Decision Tree Regressor
+            if grid_params is not None and random_params is None and bayes_pbounds is None:
+                assert all('LGBM__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'LGBM__'"
+            elif random_params is not None:
+                assert all('LGBM__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'LGBM__'"
+            elif bayes_pbounds is not None:
+                assert all('LGBM__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LGBM__'"
+                assert all('LGBM__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LGBM__'"
+            
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
+            pipe = Pipeline(steps=[('Prep', preprocessor),
+                                ('LGBM', LGBMRegressor(random_state=random_state))])
+            #Select Grid Search, Random Search or Bayesian Optimization
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
+            select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+
+            #generate a dictionary with all the parameters used in the model
+            self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
+            self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
+
+            self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
+                                        'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+            print(self.model.best_params_)
+            
 
     def save(self,return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
         ----------
```

### Comparing `gmltools-0.0.76/src/gmltools/models/models_info.py` & `gmltools-0.0.77/src/gmltools/models/models_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,12 +277,45 @@
     'shrinking': True,
     'cache_size': 200,
     'verbose': False,
     'max_iter': -1
 }
 
 
+lb_default_params_reg = {
+    "n_estimators": 10,
+    "criterion": ["linear", "square", "absolute", "exponential"],
+    "max_depth": 3,
+    "min_samples_split": 2,
+    "min_samples_leaf": 1,
+    "min_weight_fraction_leaf": 0.0,
+    "max_features": None,
+    "max_leaf_nodes": None,
+    "min_impurity_decrease": 0.0,
+    "random_state": None,
+    "ccp_alpha": 0.0,
+}
+
+
+lgb_default_params_reg = {
+    'n_estimators': [100,200,300,400,500],
+    'boosting_type': ['gbdt', 'dart', 'goss', 'rf'],
+    'objective': [None],
+    'num_leaves': [31, 127, 255],
+    'max_depth': [-1,2,3,4,5],
+    'learning_rate': [0.1,0.001],
+    'subsample_for_bin': [200000, 500000],
+    'min_split_gain':[0.0],
+    'min_child_weight': [0.001],
+    'min_child_samples':[20],
+    'subsample':[1.0],
+    'subsample_freq':[0], 
+    'colsample_bytree':[1.0],
+}
+
+
+
```

### Comparing `gmltools-0.0.76/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.77/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.77/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.77/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.77/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.77/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.77/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.76/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.77/src/gmltools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.76
+Version: 0.0.77
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.76/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.77/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

