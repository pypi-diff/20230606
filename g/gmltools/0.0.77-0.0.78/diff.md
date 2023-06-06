# Comparing `tmp/gmltools-0.0.77.tar.gz` & `tmp/gmltools-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.77.tar", last modified: Tue Jun  6 10:55:44 2023, max compression
+gzip compressed data, was "gmltools-0.0.78.tar", last modified: Tue Jun  6 11:26:33 2023, max compression
```

## Comparing `gmltools-0.0.77.tar` & `gmltools-0.0.78.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.243115 gmltools-0.0.77/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.77/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.77/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-06-06 10:55:44.243115 gmltools-0.0.77/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.77/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.035778 gmltools-0.0.77/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.77/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.77/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.77/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-06-06 10:53:29.000000 gmltools-0.0.77/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 10:55:44.243115 gmltools-0.0.77/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-06-06 10:54:46.000000 gmltools-0.0.77/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.005729 gmltools-0.0.77/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.046738 gmltools-0.0.77/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.77/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.77/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.090375 gmltools-0.0.77/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.77/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.77/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.176765 gmltools-0.0.77/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.77/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.77/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.77/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.77/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   160690 2023-06-06 10:49:51.000000 gmltools-0.0.77/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7037 2023-06-06 10:47:14.000000 gmltools-0.0.77/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.77/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.204694 gmltools-0.0.77/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.77/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.77/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.77/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.242176 gmltools-0.0.77/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.77/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.77/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.77/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.77/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:55:44.079414 gmltools-0.0.77/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 10:55:43.000000 gmltools-0.0.77/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.828389 gmltools-0.0.78/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.78/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.78/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-06-06 11:26:33.828389 gmltools-0.0.78/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.78/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.783541 gmltools-0.0.78/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.78/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.78/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.78/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-06-06 11:25:29.000000 gmltools-0.0.78/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:26:33.828389 gmltools-0.0.78/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-06-06 11:25:20.000000 gmltools-0.0.78/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.771578 gmltools-0.0.78/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.785532 gmltools-0.0.78/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.78/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.78/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.810487 gmltools-0.0.78/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.78/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.78/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.819419 gmltools-0.0.78/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.78/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.78/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.78/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.78/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   160690 2023-06-06 10:49:51.000000 gmltools-0.0.78/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.78/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.78/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.822408 gmltools-0.0.78/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.78/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.78/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.78/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.827392 gmltools-0.0.78/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.78/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.78/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.78/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.78/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:26:33.808488 gmltools-0.0.78/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-06-06 11:26:33.000000 gmltools-0.0.78/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-06-06 11:26:33.000000 gmltools-0.0.78/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:26:33.000000 gmltools-0.0.78/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-06 11:26:33.000000 gmltools-0.0.78/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 11:26:33.000000 gmltools-0.0.78/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.77/LICENSE` & `gmltools-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/Models.ipynb` & `gmltools-0.0.78/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/PKG-INFO` & `gmltools-0.0.78/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.77
+Version: 0.0.78
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.77/README.md` & `gmltools-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.78/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/gmltools.yml` & `gmltools-0.0.78/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/mltools.yml` & `gmltools-0.0.78/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/pyproject.toml` & `gmltools-0.0.78/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.77"
+version = "0.0.78"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.77/setup.py` & `gmltools-0.0.78/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.77',
+    'version': '0.0.78',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.77/src/gmltools/To_Do.txt` & `gmltools-0.0.78/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/eda/eda.py` & `gmltools-0.0.78/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models/bayes.py` & `gmltools-0.0.78/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.78/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models/dummy_model.py` & `gmltools-0.0.78/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models/model.py` & `gmltools-0.0.78/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models/models_info.py` & `gmltools-0.0.78/src/gmltools/models/models_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     "max_leaf_nodes": None,
     "min_impurity_decrease": 0.0,
     "random_state": None,
     "ccp_alpha": 0.0,
 }
 
 
-lgb_default_params_reg = {
+lgbm_default_params_reg = {
     'n_estimators': [100,200,300,400,500],
     'boosting_type': ['gbdt', 'dart', 'goss', 'rf'],
     'objective': [None],
     'num_leaves': [31, 127, 255],
     'max_depth': [-1,2,3,4,5],
     'learning_rate': [0.1,0.001],
     'subsample_for_bin': [200000, 500000],
```

### Comparing `gmltools-0.0.77/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.78/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.78/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.78/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.78/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.78/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.78/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.77/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.78/src/gmltools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.77
+Version: 0.0.78
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.77/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.78/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

