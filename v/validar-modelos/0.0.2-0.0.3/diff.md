# Comparing `tmp/validar_modelos-0.0.2.tar.gz` & `tmp/validar_modelos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validar_modelos-0.0.2.tar", last modified: Tue Jun  6 04:48:04 2023, max compression
+gzip compressed data, was "validar_modelos-0.0.3.tar", last modified: Tue Jun  6 05:00:41 2023, max compression
```

## Comparing `validar_modelos-0.0.2.tar` & `validar_modelos-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:48:04.335835 validar_modelos-0.0.2/
--rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      480 2023-06-06 04:48:04.335835 validar_modelos-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2023-06-06 04:46:41.000000 validar_modelos-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 04:48:04.335835 validar_modelos-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-06-06 04:46:26.000000 validar_modelos-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 04:48:04.324835 validar_modelos-0.0.2/validar_modelos/
--rw-rw-rw-   0        0        0       93 2023-06-06 03:55:00.000000 validar_modelos-0.0.2/validar_modelos/__init__.py
--rw-rw-rw-   0        0        0    41460 2023-06-06 04:46:11.000000 validar_modelos-0.0.2/validar_modelos/validar_modelos.py
-drwxrwxrwx   0        0        0        0 2023-06-06 04:48:04.334837 validar_modelos-0.0.2/validar_modelos.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 05:00:41.857073 validar_modelos-0.0.3/
+-rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      480 2023-06-06 05:00:41.857073 validar_modelos-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2333 2023-06-06 04:46:41.000000 validar_modelos-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:00:41.857073 validar_modelos-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-06-06 05:00:33.000000 validar_modelos-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:00:41.848617 validar_modelos-0.0.3/validar_modelos/
+-rw-rw-rw-   0        0        0       93 2023-06-06 03:55:00.000000 validar_modelos-0.0.3/validar_modelos/__init__.py
+-rw-rw-rw-   0        0        0    43391 2023-06-06 04:59:35.000000 validar_modelos-0.0.3/validar_modelos/validar_modelos.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:00:41.856063 validar_modelos-0.0.3/validar_modelos.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-06 05:00:41.000000 validar_modelos-0.0.3/validar_modelos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-06 05:00:41.000000 validar_modelos-0.0.3/validar_modelos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:00:41.000000 validar_modelos-0.0.3/validar_modelos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-06 05:00:41.000000 validar_modelos-0.0.3/validar_modelos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 05:00:41.000000 validar_modelos-0.0.3/validar_modelos.egg-info/top_level.txt
```

### Comparing `validar_modelos-0.0.2/LICENSE.txt` & `validar_modelos-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.2/README.md` & `validar_modelos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.2/setup.py` & `validar_modelos-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="validar_modelos",
-    version="0.0.2",
+    version="0.0.3",
     description="Ferramentas e Instruções para Validação de Modelos Clássicos",
     url="http://github.com/Alexandre-Papandrea/validar_modelos",
     author="Alexandre Papandrea",
     author_email="alexandre@dadosinteligentes.com",
     packages=find_packages(),
     install_requires=[
         "ipywidgets",
```

### Comparing `validar_modelos-0.0.2/validar_modelos/validar_modelos.py` & `validar_modelos-0.0.3/validar_modelos/validar_modelos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,29 @@
-## Manipulação de Dados
-
-
-import pandas
-
-
-
-# Statisticas
-
-
-import statsmodels.api
-from scipy.stats import probplot
-
-# Machine Learning
-
-
-from sklearn.exceptions import NotFittedError
-from sklearn.inspection import permutation_importance
-from sklearn.model_selection import cross_val_score, cross_val_predict
-from sklearn.metrics import (r2_score, mean_squared_error, mean_absolute_error, 
-                             mean_absolute_percentage_error, mean_squared_log_error, 
-                             make_scorer, roc_curve, accuracy_score, balanced_accuracy_score, 
-                             precision_score, recall_score, f1_score, roc_auc_score, 
-                             average_precision_score, confusion_matrix, auc, 
-                             precision_recall_curve)
-from sklearn.calibration import calibration_curve
-
-# Visualização
-
-
-import matplotlib.pyplot
-import plotly.express
-import plotly.graph_objects
-import seaborn
-from IPython.display import display, Markdown
-import ipywidgets
-
-
-############### INPUTS ########################################
 
 
 def inputs_validacao():
+    import pandas
+    import statsmodels.api
+    from scipy.stats import probplot
+    from sklearn.exceptions import NotFittedError
+    from sklearn.inspection import permutation_importance
+    from sklearn.model_selection import cross_val_score, cross_val_predict
+    from sklearn.metrics import (r2_score, mean_squared_error, mean_absolute_error, 
+                                 mean_absolute_percentage_error, mean_squared_log_error, 
+                                 make_scorer, roc_curve, accuracy_score, balanced_accuracy_score, 
+                                 precision_score, recall_score, f1_score, roc_auc_score, 
+                                 average_precision_score, confusion_matrix, auc, 
+                                 precision_recall_curve)
+    from sklearn.calibration import calibration_curve
+    import matplotlib.pyplot
+    import plotly.express
+    import plotly.graph_objects
+    import seaborn
+    from IPython.display import display, Markdown
+    import ipywidgets
     
     descricoes = {
         'model': 'Este é o modelo já treinado, compatível com o framework do Scikit-Learn. Pode ser uma pipeline do Scikit-Learn com um modelo como último passo. Este modelo já aprendeu os padrões dos dados e está pronto para fazer previsões. Para problemas de regressão, é necessário que o modelo tenha o método .predict. Em problemas de classificação, além do .predict, também é necessário o método .predict_proba.',
         'X_train': 'Estes são os dados usados para treinar o modelo. São informações estruturadas em observações e variáveis que o modelo usou para aprender.',
         'y_train': 'Estes são os rótulos ou valores-alvo associados aos dados de treinamento. Serviram como resposta para o modelo durante a fase de treinamento.',
         'X_test': 'Estes são novos dados, que o modelo ainda não viu. Serão utilizados para avaliar o desempenho do modelo, simulando uma situação real.',
         'y_test': 'Estes são os rótulos ou valores-alvo dos dados de teste. Servirão como referência para comparar as previsões do modelo e avaliar seu desempenho.',
@@ -58,14 +38,33 @@
     dropdown = ipywidgets.Dropdown(options=list(descricoes.keys()))
     ipywidgets.interact(exibir_descricao, input=dropdown)
 
 #################### VALIDAR REGRESSÃO ##################################    
     
     
 def validar_regressao(model, X_train, y_train, X_test, y_test, cv, nbins, n_repeats):
+    import pandas
+    import statsmodels.api
+    from scipy.stats import probplot
+    from sklearn.exceptions import NotFittedError
+    from sklearn.inspection import permutation_importance
+    from sklearn.model_selection import cross_val_score, cross_val_predict
+    from sklearn.metrics import (r2_score, mean_squared_error, mean_absolute_error, 
+                                 mean_absolute_percentage_error, mean_squared_log_error, 
+                                 make_scorer, roc_curve, accuracy_score, balanced_accuracy_score, 
+                                 precision_score, recall_score, f1_score, roc_auc_score, 
+                                 average_precision_score, confusion_matrix, auc, 
+                                 precision_recall_curve)
+    from sklearn.calibration import calibration_curve
+    import matplotlib.pyplot
+    import plotly.express
+    import plotly.graph_objects
+    import seaborn
+    from IPython.display import display, Markdown
+    import ipywidgets
 
 ### Transformando y_test e y_train em numpy.array caso não estejam nesse formato ainda.
 
     if not isinstance(y_test, numpy.ndarray):
          y_test = numpy.array(y_test)
 
     if not isinstance(y_train, numpy.ndarray):
@@ -373,14 +372,35 @@
         
     dropdown = ipywidgets.Dropdown(options=['Métricas de Avaliação','Plot do Valor Real vs Previsto', 'Plot Residuos', 'Histograma Residuos', 'Q-Q Plot','Importancia das Features Permutadas'])
     interact(plot_explanation, plot_type=dropdown)
     
     
     
 def validar_classificacao_binaria(model, X_train, y_train, X_test, y_test, cv, nbins, n_repeats):
+    
+    
+    import pandas
+    import statsmodels.api
+    from scipy.stats import probplot
+    from sklearn.exceptions import NotFittedError
+    from sklearn.inspection import permutation_importance
+    from sklearn.model_selection import cross_val_score, cross_val_predict
+    from sklearn.metrics import (r2_score, mean_squared_error, mean_absolute_error, 
+                                 mean_absolute_percentage_error, mean_squared_log_error, 
+                                 make_scorer, roc_curve, accuracy_score, balanced_accuracy_score, 
+                                 precision_score, recall_score, f1_score, roc_auc_score, 
+                                 average_precision_score, confusion_matrix, auc, 
+                                 precision_recall_curve)
+    from sklearn.calibration import calibration_curve
+    import matplotlib.pyplot
+    import plotly.express
+    import plotly.graph_objects
+    import seaborn
+    from IPython.display import display, Markdown
+    import ipywidgets
 
 
     if not isinstance(y_test, numpy.ndarray):
          y_test = numpy.array(y_test)
 
     if not isinstance(y_train, numpy.ndarray):
          y_train = numpy.array(y_train)
```

