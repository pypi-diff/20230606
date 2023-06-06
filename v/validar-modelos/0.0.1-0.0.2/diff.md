# Comparing `tmp/validar_modelos-0.0.1.tar.gz` & `tmp/validar_modelos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validar_modelos-0.0.1.tar", last modified: Tue Jun  6 04:13:28 2023, max compression
+gzip compressed data, was "validar_modelos-0.0.2.tar", last modified: Tue Jun  6 04:48:04 2023, max compression
```

## Comparing `validar_modelos-0.0.1.tar` & `validar_modelos-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:13:28.406370 validar_modelos-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      480 2023-06-06 04:13:28.406370 validar_modelos-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2023-06-06 04:10:45.000000 validar_modelos-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 04:13:28.407370 validar_modelos-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-06-06 03:58:25.000000 validar_modelos-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 04:13:28.391370 validar_modelos-0.0.1/validar_modelos/
--rw-rw-rw-   0        0        0       93 2023-06-06 03:55:00.000000 validar_modelos-0.0.1/validar_modelos/__init__.py
--rw-rw-rw-   0        0        0    40696 2023-06-06 03:52:04.000000 validar_modelos-0.0.1/validar_modelos/validar_modelos.py
-drwxrwxrwx   0        0        0        0 2023-06-06 04:13:28.405372 validar_modelos-0.0.1/validar_modelos.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-06 04:13:28.000000 validar_modelos-0.0.1/validar_modelos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-06 04:13:28.000000 validar_modelos-0.0.1/validar_modelos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:13:28.000000 validar_modelos-0.0.1/validar_modelos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-06 04:13:28.000000 validar_modelos-0.0.1/validar_modelos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 04:13:28.000000 validar_modelos-0.0.1/validar_modelos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 04:48:04.335835 validar_modelos-0.0.2/
+-rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      480 2023-06-06 04:48:04.335835 validar_modelos-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2333 2023-06-06 04:46:41.000000 validar_modelos-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 04:48:04.335835 validar_modelos-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-06-06 04:46:26.000000 validar_modelos-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 04:48:04.324835 validar_modelos-0.0.2/validar_modelos/
+-rw-rw-rw-   0        0        0       93 2023-06-06 03:55:00.000000 validar_modelos-0.0.2/validar_modelos/__init__.py
+-rw-rw-rw-   0        0        0    41460 2023-06-06 04:46:11.000000 validar_modelos-0.0.2/validar_modelos/validar_modelos.py
+drwxrwxrwx   0        0        0        0 2023-06-06 04:48:04.334837 validar_modelos-0.0.2/validar_modelos.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 04:48:04.000000 validar_modelos-0.0.2/validar_modelos.egg-info/top_level.txt
```

### Comparing `validar_modelos-0.0.1/LICENSE.txt` & `validar_modelos-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.1/README.md` & `validar_modelos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.1/setup.py` & `validar_modelos-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="validar_modelos",
-    version="0.0.1",
+    version="0.0.2",
     description="Ferramentas e Instruções para Validação de Modelos Clássicos",
     url="http://github.com/Alexandre-Papandrea/validar_modelos",
     author="Alexandre Papandrea",
     author_email="alexandre@dadosinteligentes.com",
     packages=find_packages(),
     install_requires=[
         "ipywidgets",
```

### Comparing `validar_modelos-0.0.1/validar_modelos/validar_modelos.py` & `validar_modelos-0.0.2/validar_modelos/validar_modelos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ## Manipulação de Dados
 
 
-import pandas as pd
+import pandas
 
 
 
 # Statisticas
 
 
-import statsmodels.api as sm
+import statsmodels.api
 from scipy.stats import probplot
 
 # Machine Learning
 
 
 from sklearn.exceptions import NotFittedError
 from sklearn.inspection import permutation_importance
@@ -24,20 +24,20 @@
                              average_precision_score, confusion_matrix, auc, 
                              precision_recall_curve)
 from sklearn.calibration import calibration_curve
 
 # Visualização
 
 
-import matplotlib.pyplot as plt
-import plotly.express as px
-import plotly.graph_objects as go
-import seaborn as sns
+import matplotlib.pyplot
+import plotly.express
+import plotly.graph_objects
+import seaborn
 from IPython.display import display, Markdown
-import ipywidgets as widgets
+import ipywidgets
 
 
 ############### INPUTS ########################################
 
 
 def inputs_validacao():
     
@@ -51,29 +51,29 @@
         'nbinbs': 'O número de bins no histograma dos dados. Este valor pode afetar a interpretação dos resultados, ao determinar o nível de detalhamento na visualização dos dados.',
         'n_repeats': 'Este é o número de vezes que repetimos a avaliação da importância dos recursos, por permutação. Mais repetições podem dar uma visão mais precisa de quais recursos são mais relevantes para as previsões do modelo.'
     }
 
     def exibir_descricao(input):
         display(Markdown(f"<div style='background: #ffffff; color: #000000; padding: 0.5em; margin: 0.5em 0; font-family: Arial, sans-serif;'><h2 style='background: #c0c0c0; display: inline-block; padding: 0.2em 0.5em;'>{input}</h2><p>{descricoes[input]}</p></div>"))
 
-    dropdown = widgets.Dropdown(options=list(descricoes.keys()))
-    widgets.interact(exibir_descricao, input=dropdown)
+    dropdown = ipywidgets.Dropdown(options=list(descricoes.keys()))
+    ipywidgets.interact(exibir_descricao, input=dropdown)
 
 #################### VALIDAR REGRESSÃO ##################################    
     
     
 def validar_regressao(model, X_train, y_train, X_test, y_test, cv, nbins, n_repeats):
 
-### Transformando y_test e y_train em np.array caso não estejam nesse formato ainda.
+### Transformando y_test e y_train em numpy.array caso não estejam nesse formato ainda.
 
-    if not isinstance(y_test, np.ndarray):
-         y_test = np.array(y_test)
+    if not isinstance(y_test, numpy.ndarray):
+         y_test = numpy.array(y_test)
 
-    if not isinstance(y_train, np.ndarray):
-         y_train = np.array(y_train)
+    if not isinstance(y_train, numpy.ndarray):
+         y_train = numpy.array(y_train)
 
     
 ### Testando se o modelo já está treinado, caso contrário o modelo ou pipeline é treinada com os parâmetros padrões 
 
     try:
         
         
@@ -94,27 +94,27 @@
 ### Definição de Métricas e função para avaliar as métricas 
     
     
     def mean_absolute_percentage_error(y_true, y_pred): 
         
         
         
-        return np.mean(np.abs((y_true - y_pred) / y_true)) * 100   
+        return numpy.mean(numpy.abs((y_true - y_pred) / y_true)) * 100   
     
     ###### Veio olhar o código né?? :D     
     def evaluation_metrics():
 
         y_train_pred = model.predict(X_train)
         y_pred = model.predict(X_test)
 
         r2_train = r2_score(y_train, y_train_pred)
         r2_test = r2_score(y_test, y_pred)
 
-        rmse_train = np.sqrt(mean_squared_error(y_train, y_train_pred))
-        rmse_test = np.sqrt(mean_squared_error(y_test, y_pred))
+        rmse_train = numpy.sqrt(mean_squared_error(y_train, y_train_pred))
+        rmse_test = numpy.sqrt(mean_squared_error(y_test, y_pred))
 
         mae_train = mean_absolute_error(y_train, y_train_pred)
         mae_test = mean_absolute_error(y_test, y_pred)
 
         mape_train = mean_absolute_percentage_error(y_train, y_train_pred) * 100
         mape_test = mean_absolute_percentage_error(y_test, y_pred) * 100
 
@@ -126,129 +126,129 @@
         }
         ##### BRAZILIAN BEAST &&&&&&&&&&&&&&&&& UNTOUCHABLE PRESENTS 
         cv_scores = {}
         for metric_name, scorer in scoring_dict.items():
             cv_score = cross_val_score(model, X_train, y_train, cv=cv, scoring=scorer)
             cv_scores[metric_name] = cv_score.mean()
 
-        metrics = pd.DataFrame({
+        metrics = pandas.DataFrame({
             'Metric': ['R2', 'RMSE', 'MAE', 'MAPE'],
             'Train Value': [r2_train, rmse_train, mae_train, mape_train],
             'Test Value': [r2_test, rmse_test, mae_test, mape_test],
             'CV Score': [cv_scores['r2'], -cv_scores['rmse'], -cv_scores['mae'], -cv_scores['mape']]
         })
 
-        fig = go.Figure(data=[go.Table(header=dict(values=['Metrica', 'Valor Dados Treino', 'Valor Dados Teste', 'Score Validação Cruzada']),
+        fig = plotly.graph_objects.Figure(data=[plotly.graph_objects.Table(header=dict(values=['Metrica', 'Valor Dados Treino', 'Valor Dados Teste', 'Score Validação Cruzada']),
                                        cells=dict(values=[metrics['Metric'], metrics['Train Value'], metrics['Test Value'], metrics['CV Score']]))])
         fig.show()  
 
     ### Função para Valor Real Versus Previsto 
 
-    import plotly.graph_objs as go
+
     from plotly.subplots import make_subplots
 
     def grafico_previsto_vs_real():
         fig = make_subplots(rows=1, cols=2, subplot_titles=("Previsto vs Real - Treino", "Previsto vs Real - Teste"))
 
         fig.add_trace(
-            go.Scatter(x=y_train, y=y_train_pred, mode='markers'),
+            plotly.graph_objects.Scatter(x=y_train, y=y_train_pred, mode='markers'),
             row=1, col=1
         )
 
         fig.add_trace(
-            go.Scatter(x=[y_train.min(), y_train.max()], y=[y_train.min(), y_train.max()], mode='lines'),
+            plotly.graph_objects.Scatter(x=[y_train.min(), y_train.max()], y=[y_train.min(), y_train.max()], mode='lines'),
             row=1, col=1
         )
 
         fig.add_trace(
-            go.Scatter(x=y_test, y=y_pred, mode='markers'),
+            plotly.graph_objects.Scatter(x=y_test, y=y_pred, mode='markers'),
             row=1, col=2
         )
 
         fig.add_trace(
-            go.Scatter(x=[y_test.min(), y_test.max()], y=[y_test.min(), y_test.max()], mode='lines'),
+            plotly.graph_objects.Scatter(x=[y_test.min(), y_test.max()], y=[y_test.min(), y_test.max()], mode='lines'),
             row=1, col=2
         )
 
         fig.update_layout(height=600, width=1200, title_text="Previsto vs Real")
         fig.show()
 
     def grafico_residuos():
         fig = make_subplots(rows=1, cols=2, subplot_titles=("Gráfico Resíduos - Treino", "Gráfico Resíduos - Teste"))
 
         residuos_treino = y_train - y_train_pred
         fig.add_trace(
-            go.Scatter(x=y_train_pred, y=residuos_treino, mode='markers'),
+            plotly.graph_objects.Scatter(x=y_train_pred, y=residuos_treino, mode='markers'),
             row=1, col=1
         )
 
         fig.add_trace(
-            go.Scatter(x=[y_train_pred.min(), y_train_pred.max()], y=[0, 0], mode='lines'),
+            plotly.graph_objects.Scatter(x=[y_train_pred.min(), y_train_pred.max()], y=[0, 0], mode='lines'),
             row=1, col=1
         )
 
         residuos_teste = y_test - y_pred
         fig.add_trace(
-            go.Scatter(x=y_pred, y=residuos_teste, mode='markers'),
+            plotly.graph_objects.Scatter(x=y_pred, y=residuos_teste, mode='markers'),
             row=1, col=2
         )
 
         fig.add_trace(
-            go.Scatter(x=[y_pred.min(), y_pred.max()], y=[0, 0], mode='lines'),
+            plotly.graph_objects.Scatter(x=[y_pred.min(), y_pred.max()], y=[0, 0], mode='lines'),
             row=1, col=2
         )
 
         fig.update_layout(height=600, width=1200, title_text="Gráfico de Resíduos")
         fig.show()
 
 
     def histograma_residuos():
         fig = make_subplots(rows=1, cols=2, subplot_titles=("Histograma Resíduos - Treino", "Histograma Resíduos - Teste"))
 
         residuos_treino = y_train - y_train_pred
         fig.add_trace(
-            go.Histogram(x=residuos_treino, nbinsx=nbins),
+            plotly.graph_objects.Histogram(x=residuos_treino, nbinsx=nbins),
             row=1, col=1
         )
 
         residuos_teste = y_test - y_pred
         fig.add_trace(
-            go.Histogram(x=residuos_teste, nbinsx=nbins),
+            plotly.graph_objects.Histogram(x=residuos_teste, nbinsx=nbins),
             row=1, col=2
         )
 
         fig.update_layout(height=600, width=1200, title_text="Histograma de Resíduos")
         fig.show()
 
     def qq_plot():
-        fig, ax = plt.subplots(1, 2, figsize=(15, 5))
+        fig, ax = matplotlib.pyplot.subplots(1, 2, figsize=(15, 5))
 
         residuos_treino = y_train - y_train_pred
-        sm.qqplot(residuos_treino, line ='45', ax=ax[0])
+        statsmodels.api.qqplot(residuos_treino, line ='45', ax=ax[0])
         ax[0].set_title('QQ Plot Resíduos - Treino')
 
         residuos_teste = y_test - y_pred
-        sm.qqplot(residuos_teste, line ='45', ax=ax[1])
+        statsmodels.api.qqplot(residuos_teste, line ='45', ax=ax[1])
         ax[1].set_title('QQ Plot Resíduos - Teste')
 
-        plt.show()
+        matplotlib.pyplot.show()
             
 
     def qq_plot():
-        fig, ax = plt.subplots(1, 2, figsize=(15, 5))
+        fig, ax = matplotlib.pyplot.subplots(1, 2, figsize=(15, 5))
 
         residuos_treino = y_train - y_train_pred
-        sm.qqplot(residuos_treino, line ='45', ax=ax[0])
+        statsmodels.api.qqplot(residuos_treino, line ='45', ax=ax[0])
         ax[0].set_title('QQ Plot Resíduos - Treino')
 
         residuos_teste = y_test - y_pred
-        sm.qqplot(residuos_teste, line ='45', ax=ax[1])
+        statsmodels.api.qqplot(residuos_teste, line ='45', ax=ax[1])
         ax[1].set_title('QQ Plot Resíduos - Teste')
 
-        plt.show()
+        matplotlib.pyplot.show()
             
             
         
     def permutation_feature_importance():
         
         scoring_dict = {
             'r2': 'r2',
@@ -259,46 +259,46 @@
 
         results_train = {}
         results_test = {}
         for metric_name, scorer in scoring_dict.items():
             result_train = permutation_importance(model, X_train, y_train_pred, scoring=scorer, n_repeats=10, random_state=42)
             result_test = permutation_importance(model, X_test, y_test, scoring=scorer, n_repeats=10, random_state=42)
             
-            importance_df_train = pd.DataFrame({'Variável': X_train.columns,
+            importance_df_train = pandas.DataFrame({'Variável': X_train.columns,
                                            'Importância Treino': result_train.importances_mean,
                                            'Importância Desvio Padrão Treino': result_train.importances_std})
             
-            importance_df_test = pd.DataFrame({'Variável': X_test.columns,
+            importance_df_test = numpy.arrayDataFrame({'Variável': X_test.columns,
                                            'Importância Teste': result_test.importances_mean,
                                            'Importância Desvio Padrão Teste': result_test.importances_std})
                                            
             importance_df_train.sort_values(by='Importância Treino', ascending=False, inplace=True)
             importance_df_test.sort_values(by='Importância Teste', ascending=False, inplace=True)
             
             results_train[metric_name] = importance_df_train
             results_test[metric_name] = importance_df_test
             
-            importance_difference = pd.merge(importance_df_train, importance_df_test, on="Variável", suffixes=('_train', '_test'))
+            importance_difference = pandas.merge(importance_df_train, importance_df_test, on="Variável", suffixes=('_train', '_test'))
             importance_difference["Diferença"] = abs(importance_difference['Importância Treino'] - importance_difference['Importância Teste'])
 
-            fig = go.Figure()
-            fig.add_trace(go.Bar(name='Treino', 
+            fig = plotly.graph_objects.Figure()
+            fig.add_trace(plotly.graph_objects.Bar(name='Treino', 
                                  x=importance_df_train['Variável'], 
                                  y=importance_df_train['Importância Treino'], 
                                  error_y=dict(array=importance_df_train['Importância Desvio Padrão Treino'])))
 
-            fig.add_trace(go.Bar(name='Teste', 
+            fig.add_trace(plotly.graph_objects.Bar(name='Teste', 
                                  x=importance_df_test['Variável'], 
                                  y=importance_df_test['Importância Teste'], 
                                  error_y=dict(array=importance_df_test['Importância Desvio Padrão Teste'])))
             fig.update_layout(barmode='group', title=f'Permutation Feature Importance ({metric_name.upper()})')
             fig.show()
 
 
-            fig_diff = go.Figure(data=[go.Table(header=dict(values=['Variável', 'Diferença']),
+            fig_diff = plotly.graph_objects.Figure(data=[plotly.graph_objects.Table(header=dict(values=['Variável', 'Diferença']),
                                                 cells=dict(values=[importance_difference['Variável'], importance_difference['Diferença']]))])
             fig_diff.show()
         
     
     
 
     def plot_explanation(plot_type):
@@ -343,17 +343,17 @@
 
             'Importancia das Features Permutadas':
             '''
             Imagine que queremos saber qual é a "matéria" (ou feature) que mais "pesa" na nota final do nosso modelo. E ainda queremos saber se o modelo está "colando" (overfitting) dessa matéria. Para isso, permutamos as features e vemos como isso afeta o resultado. Se uma matéria tem um peso muito grande na nota final e o modelo vai mal quando essa matéria é alterada, pode ser que o modelo esteja "colando" dessa matéria. É como se estivéssemos tentando entender melhor o "processo de aprendizagem" do nosso modelo, para garantir que ele será capaz de responder bem a novas perguntas.
             '''
         }
     
-        text_widget = widgets.Textarea(
+        text_widget = ipywidgets.Textarea(
             value=explanations[plot_type],
-            layout=widgets.Layout(width="100%", height="200px")
+            layout=ipywidgets.Layout(width="100%", height="200px")
         )
 
         display(text_widget)
 
         plot_selected(plot_type)
         
     def plot_selected(plot_type):
@@ -367,27 +367,27 @@
         elif plot_type ==  'Histograma Residuos':
             histograma_residuos()
         elif plot_type ==  'Q-Q Plot':
             qq_plot()
         elif plot_type ==  'Importancia das Features Permutadas':
             permutation_feature_importance()
         
-    dropdown = widgets.Dropdown(options=['Métricas de Avaliação','Plot do Valor Real vs Previsto', 'Plot Residuos', 'Histograma Residuos', 'Q-Q Plot','Importancia das Features Permutadas'])
+    dropdown = ipywidgets.Dropdown(options=['Métricas de Avaliação','Plot do Valor Real vs Previsto', 'Plot Residuos', 'Histograma Residuos', 'Q-Q Plot','Importancia das Features Permutadas'])
     interact(plot_explanation, plot_type=dropdown)
     
     
     
 def validar_classificacao_binaria(model, X_train, y_train, X_test, y_test, cv, nbins, n_repeats):
 
 
-    if not isinstance(y_test, np.ndarray):
-         y_test = np.array(y_test)
+    if not isinstance(y_test, numpy.ndarray):
+         y_test = numpy.array(y_test)
 
-    if not isinstance(y_train, np.ndarray):
-         y_train = np.array(y_train)
+    if not isinstance(y_train, numpy.ndarray):
+         y_train = numpy.array(y_train)
 
     
     
     try:
         
         
         y_pred = model.predict(X_test)
@@ -445,54 +445,54 @@
         }
 
         cv_scores = {}
         for metric_name, scorer in scoring_dict.items():
             cv_score = cross_val_score(model, X_train, y_train, cv=cv, scoring=scorer,n_jobs=-1)
             cv_scores[metric_name] = cv_score.mean()
 
-        metrics = pd.DataFrame({
+        metrics = pandas.DataFrame({
             'Métrica': ['Acurácia','Acurácia Balanceada','Precisão','Recall', 'F1-Score', 'AUC-ROC', 'PR AUC Score'],
             'Valor Treino': [acc_train, b_acc_train,prec_train, rec_train, f1_train, auc_train, pr_auc_train],
             'Valor Teste': [acc_test, b_acc_test,prec_test, rec_test, f1_test, auc_test, pr_auc_test],
             'Score Validação Cruzada': [cv_scores['Acurácia'],cv_scores['Acurácia Balanceada'],cv_scores['Precisão'], cv_scores['Recall'], cv_scores['F1-Score'], cv_scores['AUC-ROC'], cv_scores['PR AUC Score']]
         })
 
-        fig = go.Figure(data=[go.Table(header=dict(values=['Métrica', 'Valor Treino', 'Valor Teste', 'Score Validação Cruzada']),
+        fig = plotly.graph_objects.Figure(data=[plotly.graph_objects.Table(header=dict(values=['Métrica', 'Valor Treino', 'Valor Teste', 'Score Validação Cruzada']),
                                        cells=dict(values=[metrics['Métrica'], metrics['Valor Treino'], metrics['Valor Teste'], metrics['Score Validação Cruzada']]))])
         fig.show() 
 
     def matriz_confusao():
-        fig, ax = plt.subplots(1, 2, figsize=(15, 5))
+        fig, ax = matplotlib.pyplot.subplots(1, 2, figsize=(15, 5))
 
         cm_train = confusion_matrix(y_train, y_train_pred)
         acc_train = accuracy_score(y_train, y_train_pred)
         b_acc_train = balanced_accuracy_score(y_train, y_train_pred)
         prec_train = precision_score(y_train, y_train_pred)
         rec_train = recall_score(y_train, y_train_pred)
 
-        sns.heatmap(cm_train, annot=True, fmt="d", ax=ax[0], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
+        plotly.seaborn.heatmap(cm_train, annot=True, fmt="d", ax=ax[0], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
         ax[0].set_title(f'Treino\nAcurácia: {acc_train:.2f}\nAcurácia Balanceada: {b_acc_train:.2f}\nPrecisão: {prec_train:.2f}\nRecall: {rec_train:.2f}')
         ax[0].set_xlabel('Predito')
         ax[0].set_ylabel('Real')
 
         cm_test = confusion_matrix(y_test, y_pred)
         acc_test = accuracy_score(y_test, y_pred)
         b_acc_test = balanced_accuracy_score(y_test, y_pred)
         prec_test = precision_score(y_test, y_pred)
         rec_test = recall_score(y_test, y_pred)
 
-        sns.heatmap(cm_test, annot=True, fmt="d", ax=ax[1], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
+        plotly.seaborn.heatmap(cm_test, annot=True, fmt="d", ax=ax[1], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
         ax[1].set_title(f'Teste\nAcurácia: {acc_test:.2f}\nAcurácia Balanceada: {b_acc_test:.2f}\nPrecisão: {prec_test:.2f}\nRecall: {rec_test:.2f}')
         ax[1].set_xlabel('Predito')
         ax[1].set_ylabel('Real')
 
-        plt.show()
+        matplotlib.pyplot.show()
 
     def roc_auc_curve():
-        fig, ax = plt.subplots(1, 2, figsize=(15, 5))
+        fig, ax = matplotlib.pyplot.subplots(1, 2, figsize=(15, 5))
 
         fpr_train, tpr_train, _ = roc_curve(y_train, y_train_prob)
         roc_auc_train = auc(fpr_train, tpr_train)
 
         ax[0].plot(fpr_train, tpr_train, color='darkorange', lw=2, label=f'ROC curve (area = {roc_auc_train:.2f})')
         ax[0].plot([0, 1], [0, 1], color='navy', lw=2, linestyle='--')
         ax[0].set_xlim([0.0, 1.0])
@@ -511,20 +511,20 @@
         ax[1].set_xlim([0.0, 1.0])
         ax[1].set_ylim([0.0, 1.05])
         ax[1].set_xlabel('Taxa de Falso Positivo')
         ax[1].set_ylabel('Taxa de Verdadeiro Positivo')
         ax[1].set_title('Curva ROC - Teste')
         ax[1].legend(loc="lower right")
 
-        plt.show()
+        matplotlib.pyplot.show()
         
         
         
     def precision_recall():
-        fig, ax = plt.subplots(1, 2, figsize=(15, 5))
+        fig, ax = matplotlib.pyplot.subplots(1, 2, figsize=(15, 5))
 
         precision_train, recall_train, _ = precision_recall_curve(y_train, y_train_prob)
         average_precision_train = average_precision_score(y_train, y_train_prob)
 
         ax[0].step(recall_train, precision_train, color='b', alpha=0.2, where='post')
         ax[0].fill_between(recall_train, precision_train, step='post', alpha=0.2, color='b')
         ax[0].set_xlabel('Recall')
@@ -544,50 +544,50 @@
         ax[1].fill_between(recall_test, precision_test, step='post', alpha=0.2, color='b')
         ax[1].set_xlabel('Recall')
         ax[1].set_ylabel('Precision')
         ax[1].set_ylim([0.0, 1.05])
         ax[1].set_xlim([0.0, 1.0])
         ax[1].set_title('Curva de Precisão-Recall: AP={0:0.2f}'.format(average_precision_test))
 
-        plt.show()
+        matplotlib.pyplot.show()
         
     def histograma_probabilidade():
-        df_treino = pd.DataFrame({'Probabilidade Prevista': y_train_prob, 'Rótulo Verdadeiro': y_train, 'Dados': 'Treino'})
-        df_teste = pd.DataFrame({'Probabilidade Prevista': y_test_prob, 'Rótulo Verdadeiro': y_test, 'Dados': 'Teste'})
+        df_treino = pandas.DataFrame({'Probabilidade Prevista': y_train_prob, 'Rótulo Verdadeiro': y_train, 'Dados': 'Treino'})
+        df_teste = pandas.DataFrame({'Probabilidade Prevista': y_test_prob, 'Rótulo Verdadeiro': y_test, 'Dados': 'Teste'})
 
-        df = pd.concat([df_treino, df_teste])
+        df = pandas.concat([df_treino, df_teste])
 
-        fig = px.histogram(df, x='Probabilidade Prevista', color='Rótulo Verdadeiro', facet_col='Dados', nbins=50, opacity=0.7,
+        fig = plotly.express.histogram(df, x='Probabilidade Prevista', color='Rótulo Verdadeiro', facet_col='Dados', nbins=50, opacity=0.7,
                            labels={'Probabilidade Prevista': 'Probabilidade Prevista', 'Rótulo Verdadeiro': 'Rótulo Verdadeiro'},
                            title='Histograma de Probabilidade Prevista')
         fig.show()
 
     def plot_densidade_probabilidade():
-        df_treino = pd.DataFrame({'Probabilidade Prevista': y_train_prob, 'Rótulo Verdadeiro': y_train, 'Dados': 'Treino'})
-        df_teste = pd.DataFrame({'Probabilidade Prevista': y_test_prob, 'Rótulo Verdadeiro': y_test, 'Dados': 'Teste'})
+        df_treino = pandas.DataFrame({'Probabilidade Prevista': y_train_prob, 'Rótulo Verdadeiro': y_train, 'Dados': 'Treino'})
+        df_teste = pandas.DataFrame({'Probabilidade Prevista': y_test_prob, 'Rótulo Verdadeiro': y_test, 'Dados': 'Teste'})
 
-        df = pd.concat([df_treino, df_teste])
+        df = pandas.concat([df_treino, df_teste])
 
-        fig = px.histogram(df, x='Probabilidade Prevista', color='Rótulo Verdadeiro', facet_col='Dados', nbins=50, opacity=0.7,
+        fig = plotly.express.histogram(df, x='Probabilidade Prevista', color='Rótulo Verdadeiro', facet_col='Dados', nbins=50, opacity=0.7,
                            marginal='box', histnorm='density', barmode='overlay',
                            labels={'Probabilidade Prevista': 'Probabilidade Prevista', 'Rótulo Verdadeiro': 'Rótulo Verdadeiro'},
                            title='Densidade de Probabilidade Prevista')
         fig.show()
 
         
 ##### Esse aqui é perigoso, cuidado , só grave.        
         
     def plot_calibracao_probabilidade():
         prob_verdadeira_treino, prob_prevista_treino = calibration_curve(y_train, y_train_prob, n_bins=10)
         prob_verdadeira_teste, prob_prevista_teste = calibration_curve(y_test, y_test_prob, n_bins=10)
 
-        fig = go.Figure()
+        fig = plotly.graph_objects.Figure()
 
-        fig.add_trace(go.Scatter(x=prob_prevista_treino, y=prob_verdadeira_treino, mode='lines+markers', name='Treino'))
-        fig.add_trace(go.Scatter(x=prob_prevista_teste, y=prob_verdadeira_teste, mode='lines+markers', name='Teste'))
+        fig.add_trace(plotly.graph_objects.Scatter(x=prob_prevista_treino, y=prob_verdadeira_treino, mode='lines+markers', name='Treino'))
+        fig.add_trace(plotly.graph_objects.Scatter(x=prob_prevista_teste, y=prob_verdadeira_teste, mode='lines+markers', name='Teste'))
         fig.add_shape(type='line', x0=0, x1=1, y0=0, y1=1, yref='y', xref='x', line=dict(color='Black', dash='dash'))
 
         fig.update_layout(title='Plot de Calibração de Probabilidade', xaxis_title='Probabilidade Prevista', yaxis_title='Probabilidade Verdadeira')
 
         fig.show()
         
         
@@ -604,46 +604,46 @@
 
         results_train = {}
         results_test = {}
         for metric_name, scorer in scoring_dict.items():
             result_train = permutation_importance(model, X_train, y_train, scoring=scorer, n_repeats=10, random_state=42)
             result_test = permutation_importance(model, X_test, y_test, scoring=scorer, n_repeats=10, random_state=42)
 
-            importance_df_train = pd.DataFrame({'Variável': X_train.columns,
+            importance_df_train = pandas.DataFrame({'Variável': X_train.columns,
                                                'Importância Treino': result_train.importances_mean,
                                                'Importância Desvio Padrão Treino': result_train.importances_std})
 
-            importance_df_test = pd.DataFrame({'Variável': X_test.columns,
+            importance_df_test = pandas.DataFrame({'Variável': X_test.columns,
                                                'Importância Teste': result_test.importances_mean,
                                                'Importância Desvio Padrão Teste': result_test.importances_std})
 
             importance_df_train.sort_values(by='Importância Treino', ascending=False, inplace=True)
             importance_df_test.sort_values(by='Importância Teste', ascending=False, inplace=True)
 
             results_train[metric_name] = importance_df_train
             results_test[metric_name] = importance_df_test
 
-            importance_difference = pd.merge(importance_df_train, importance_df_test, on="Variável", suffixes=('_train', '_test'))
+            importance_difference = pandas.merge(importance_df_train, importance_df_test, on="Variável", suffixes=('_train', '_test'))
             importance_difference["Diferença"] = abs(importance_difference['Importância Treino'] - importance_difference['Importância Teste'])
 
-            fig = go.Figure()
-            fig.add_trace(go.Bar(name='Treino', 
+            fig = plotly.graph_objects.Figure()
+            fig.add_trace(plotly.graph_objects.Bar(name='Treino', 
                                  x=importance_df_train['Variável'], 
                                  y=importance_df_train['Importância Treino'], 
                                  error_y=dict(array=importance_df_train['Importância Desvio Padrão Treino'])))
 
-            fig.add_trace(go.Bar(name='Teste', 
+            fig.add_trace(plotly.graph_objects.Bar(name='Teste', 
                                  x=importance_df_test['Variável'], 
                                  y=importance_df_test['Importância Teste'], 
                                  error_y=dict(array=importance_df_test['Importância Desvio Padrão Teste'])))
             fig.update_layout(barmode='group', title=f'Permutation Feature Importance ({metric_name.upper()})')
             fig.show()
 
 
-            fig_diff = go.Figure(data=[go.Table(header=dict(values=['Variável', 'Diferença']),
+            fig_diff = plotly.graph_objects.Figure(data=[plotly.graph_objects.Table(header=dict(values=['Variável', 'Diferença']),
                                                 cells=dict(values=[importance_difference['Variável'], importance_difference['Diferença']]))])
             fig_diff.show()
 
     
     
 
     def plot_explanation(plot_type):
@@ -718,17 +718,17 @@
             '''            
             
         }
 
 
     
 
-        text_widget = widgets.Textarea(
+        text_widget = ipywidgets.Textarea(
             value=explanations[plot_type],
-            layout=widgets.Layout(width="100%", height="200px")
+            layout=ipywidgets.Layout(width="100%", height="200px")
         )
         display(text_widget)
 
         plot_selected(plot_type)
         
     def plot_selected(plot_type):
 
@@ -760,10 +760,10 @@
 
             plot_calibracao_probabilidade()
 
         elif plot_type == 'Importância das Features Permutadas':
 
             permutation_feature_importance()
 
-    dropdown = widgets.Dropdown(options=['Métricas de Avaliação', 'Matriz de Confusão', 'Curva AUC-ROC', 'Curva de Precisão-Recall', 'Histograma de Probabilidade', 'Plot de Densidade de Probabilidade', 'Plot de Calibração de Probabilidade', 'Importância das Features Permutadas'])
+    dropdown = ipywidgets.Dropdown(options=['Métricas de Avaliação', 'Matriz de Confusão', 'Curva AUC-ROC', 'Curva de Precisão-Recall', 'Histograma de Probabilidade', 'Plot de Densidade de Probabilidade', 'Plot de Calibração de Probabilidade', 'Importância das Features Permutadas'])
 
     interact(plot_explanation, plot_type=dropdown)
```

