# Comparing `tmp/validar_modelos-0.0.5.tar.gz` & `tmp/validar_modelos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validar_modelos-0.0.5.tar", last modified: Tue Jun  6 05:18:59 2023, max compression
+gzip compressed data, was "validar_modelos-0.0.6.tar", last modified: Tue Jun  6 05:32:56 2023, max compression
```

## Comparing `validar_modelos-0.0.5.tar` & `validar_modelos-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 05:18:59.056039 validar_modelos-0.0.5/
--rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      480 2023-06-06 05:18:59.056039 validar_modelos-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2023-06-06 04:46:41.000000 validar_modelos-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 05:18:59.057039 validar_modelos-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-06-06 05:17:56.000000 validar_modelos-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:18:59.048040 validar_modelos-0.0.5/validar_modelos/
--rw-rw-rw-   0        0        0       93 2023-06-06 03:55:00.000000 validar_modelos-0.0.5/validar_modelos/__init__.py
--rw-rw-rw-   0        0        0    43461 2023-06-06 05:18:46.000000 validar_modelos-0.0.5/validar_modelos/validar_modelos.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:18:59.055039 validar_modelos-0.0.5/validar_modelos.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-06 05:18:58.000000 validar_modelos-0.0.5/validar_modelos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-06 05:18:58.000000 validar_modelos-0.0.5/validar_modelos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 05:18:58.000000 validar_modelos-0.0.5/validar_modelos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-06 05:18:58.000000 validar_modelos-0.0.5/validar_modelos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 05:18:58.000000 validar_modelos-0.0.5/validar_modelos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 05:32:56.672176 validar_modelos-0.0.6/
+-rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      480 2023-06-06 05:32:56.672176 validar_modelos-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2333 2023-06-06 04:46:41.000000 validar_modelos-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:32:56.673176 validar_modelos-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-06-06 05:32:41.000000 validar_modelos-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:32:56.661785 validar_modelos-0.0.6/validar_modelos/
+-rw-rw-rw-   0        0        0       93 2023-06-06 05:30:58.000000 validar_modelos-0.0.6/validar_modelos/__init__.py
+-rw-rw-rw-   0        0        0    43457 2023-06-06 05:32:46.000000 validar_modelos-0.0.6/validar_modelos/validar_modelos.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:32:56.671166 validar_modelos-0.0.6/validar_modelos.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/top_level.txt
```

### Comparing `validar_modelos-0.0.5/LICENSE.txt` & `validar_modelos-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.5/README.md` & `validar_modelos-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.5/setup.py` & `validar_modelos-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="validar_modelos",
-    version="0.0.5",
+    version="0.0.6",
     description="Ferramentas e Instruções para Validação de Modelos Clássicos",
     url="http://github.com/Alexandre-Papandrea/validar_modelos",
     author="Alexandre Papandrea",
     author_email="alexandre@dadosinteligentes.com",
     packages=find_packages(),
     install_requires=[
         "ipywidgets",
```

### Comparing `validar_modelos-0.0.5/validar_modelos/validar_modelos.py` & `validar_modelos-0.0.6/validar_modelos/validar_modelos.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
             result_train = permutation_importance(model, X_train, y_train_pred, scoring=scorer, n_repeats=10, random_state=42)
             result_test = permutation_importance(model, X_test, y_test, scoring=scorer, n_repeats=10, random_state=42)
             
             importance_df_train = pandas.DataFrame({'Variável': X_train.columns,
                                            'Importância Treino': result_train.importances_mean,
                                            'Importância Desvio Padrão Treino': result_train.importances_std})
             
-            importance_df_test = numpy.arrayDataFrame({'Variável': X_test.columns,
+            importance_df_test = pandas.DataFrame({'Variável': X_test.columns,
                                            'Importância Teste': result_test.importances_mean,
                                            'Importância Desvio Padrão Teste': result_test.importances_std})
                                            
             importance_df_train.sort_values(by='Importância Treino', ascending=False, inplace=True)
             importance_df_test.sort_values(by='Importância Teste', ascending=False, inplace=True)
             
             results_train[metric_name] = importance_df_train
```

