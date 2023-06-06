# Comparing `tmp/validar_modelos-0.0.6.tar.gz` & `tmp/validar_modelos-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validar_modelos-0.0.6.tar", last modified: Tue Jun  6 05:32:56 2023, max compression
+gzip compressed data, was "validar_modelos-0.0.7.tar", last modified: Tue Jun  6 05:47:56 2023, max compression
```

## Comparing `validar_modelos-0.0.6.tar` & `validar_modelos-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 05:32:56.672176 validar_modelos-0.0.6/
--rw-rw-rw-   0        0        0     1076 2023-06-06 04:00:25.000000 validar_modelos-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      480 2023-06-06 05:32:56.672176 validar_modelos-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2023-06-06 04:46:41.000000 validar_modelos-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 05:32:56.673176 validar_modelos-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-06-06 05:32:41.000000 validar_modelos-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:32:56.661785 validar_modelos-0.0.6/validar_modelos/
--rw-rw-rw-   0        0        0       93 2023-06-06 05:30:58.000000 validar_modelos-0.0.6/validar_modelos/__init__.py
--rw-rw-rw-   0        0        0    43457 2023-06-06 05:32:46.000000 validar_modelos-0.0.6/validar_modelos/validar_modelos.py
-drwxrwxrwx   0        0        0        0 2023-06-06 05:32:56.671166 validar_modelos-0.0.6/validar_modelos.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 05:32:56.000000 validar_modelos-0.0.6/validar_modelos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:56.663534 validar_modelos-0.0.7/
+-rw-rw-rw-   0        0        0     1076 2023-06-06 05:45:52.000000 validar_modelos-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      480 2023-06-06 05:47:56.663534 validar_modelos-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2333 2023-06-06 05:45:50.000000 validar_modelos-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 05:47:56.663534 validar_modelos-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-06-06 05:47:37.000000 validar_modelos-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:56.654534 validar_modelos-0.0.7/validar_modelos/
+-rw-rw-rw-   0        0        0       93 2023-06-06 05:45:58.000000 validar_modelos-0.0.7/validar_modelos/__init__.py
+-rw-rw-rw-   0        0        0    43443 2023-06-06 05:47:41.000000 validar_modelos-0.0.7/validar_modelos/validar_modelos.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:47:56.662534 validar_modelos-0.0.7/validar_modelos.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-06 05:47:56.000000 validar_modelos-0.0.7/validar_modelos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-06 05:47:56.000000 validar_modelos-0.0.7/validar_modelos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:47:56.000000 validar_modelos-0.0.7/validar_modelos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-06 05:47:56.000000 validar_modelos-0.0.7/validar_modelos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 05:47:56.000000 validar_modelos-0.0.7/validar_modelos.egg-info/top_level.txt
```

### Comparing `validar_modelos-0.0.6/LICENSE.txt` & `validar_modelos-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.6/README.md` & `validar_modelos-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `validar_modelos-0.0.6/setup.py` & `validar_modelos-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="validar_modelos",
-    version="0.0.6",
+    version="0.0.7",
     description="Ferramentas e Instruções para Validação de Modelos Clássicos",
     url="http://github.com/Alexandre-Papandrea/validar_modelos",
     author="Alexandre Papandrea",
     author_email="alexandre@dadosinteligentes.com",
     packages=find_packages(),
     install_requires=[
         "ipywidgets",
```

### Comparing `validar_modelos-0.0.6/validar_modelos/validar_modelos.py` & `validar_modelos-0.0.7/validar_modelos/validar_modelos.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,26 +489,26 @@
 
         cm_train = confusion_matrix(y_train, y_train_pred)
         acc_train = accuracy_score(y_train, y_train_pred)
         b_acc_train = balanced_accuracy_score(y_train, y_train_pred)
         prec_train = precision_score(y_train, y_train_pred)
         rec_train = recall_score(y_train, y_train_pred)
 
-        plotly.seaborn.heatmap(cm_train, annot=True, fmt="d", ax=ax[0], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
+        seaborn.heatmap(cm_train, annot=True, fmt="d", ax=ax[0], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
         ax[0].set_title(f'Treino\nAcurácia: {acc_train:.2f}\nAcurácia Balanceada: {b_acc_train:.2f}\nPrecisão: {prec_train:.2f}\nRecall: {rec_train:.2f}')
         ax[0].set_xlabel('Predito')
         ax[0].set_ylabel('Real')
 
         cm_test = confusion_matrix(y_test, y_pred)
         acc_test = accuracy_score(y_test, y_pred)
         b_acc_test = balanced_accuracy_score(y_test, y_pred)
         prec_test = precision_score(y_test, y_pred)
         rec_test = recall_score(y_test, y_pred)
 
-        plotly.seaborn.heatmap(cm_test, annot=True, fmt="d", ax=ax[1], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
+        seaborn.heatmap(cm_test, annot=True, fmt="d", ax=ax[1], cmap='Blues', cbar=False, xticklabels=[0, 1], yticklabels=[0, 1])
         ax[1].set_title(f'Teste\nAcurácia: {acc_test:.2f}\nAcurácia Balanceada: {b_acc_test:.2f}\nPrecisão: {prec_test:.2f}\nRecall: {rec_test:.2f}')
         ax[1].set_xlabel('Predito')
         ax[1].set_ylabel('Real')
 
         matplotlib.pyplot.show()
 
     def roc_auc_curve():
```

