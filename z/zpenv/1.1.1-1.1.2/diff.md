# Comparing `tmp/zpenv-1.1.1.tar.gz` & `tmp/zpenv-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpenv-1.1.1.tar", last modified: Tue Jun  6 20:51:54 2023, max compression
+gzip compressed data, was "zpenv-1.1.2.tar", last modified: Tue Jun  6 21:02:08 2023, max compression
```

## Comparing `zpenv-1.1.1.tar` & `zpenv-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:51:54.384000 zpenv-1.1.1/
--rw-rw-rw-   0        0        0     5138 2023-06-06 20:51:54.380000 zpenv-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4917 2022-12-26 19:01:11.000000 zpenv-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 20:51:54.383000 zpenv-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 20:51:54.331000 zpenv-1.1.1/zpenv/
--rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.1.1/zpenv/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.1.1/zpenv/__main__.py
--rw-rw-rw-   0        0        0    31382 2023-06-06 20:40:58.000000 zpenv-1.1.1/zpenv/zpenv.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:51:54.374000 zpenv-1.1.1/zpenv.egg-info/
--rw-rw-rw-   0        0        0     5138 2023-06-06 20:51:53.000000 zpenv-1.1.1/zpenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-06 20:51:54.000000 zpenv-1.1.1/zpenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:51:53.000000 zpenv-1.1.1/zpenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-06 20:51:53.000000 zpenv-1.1.1/zpenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 20:51:54.000000 zpenv-1.1.1/zpenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 20:51:54.000000 zpenv-1.1.1/zpenv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 21:02:08.737000 zpenv-1.1.2/
+-rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5522 2023-06-06 21:02:08.733000 zpenv-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4917 2022-12-26 19:01:11.000000 zpenv-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 21:02:08.736000 zpenv-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 21:02:08.688000 zpenv-1.1.2/zpenv/
+-rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.1.2/zpenv/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.1.2/zpenv/__main__.py
+-rw-rw-rw-   0        0        0    31382 2023-06-06 20:40:58.000000 zpenv-1.1.2/zpenv/zpenv.py
+drwxrwxrwx   0        0        0        0 2023-06-06 21:02:08.727000 zpenv-1.1.2/zpenv.egg-info/
+-rw-rw-rw-   0        0        0     5522 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/top_level.txt
```

### Comparing `zpenv-1.1.1/PKG-INFO` & `zpenv-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-Metadata-Version: 2.1
-Name: zpenv
-Version: 1.1.1
-Summary: Gestionnaire d'environnement virtuel
-Author: 
-License: UNKNOWN
-Platform: ALL
-Description-Content-Type: text/markdown
-
 # zpenv
 # Langue/Language
 [English Version](#EN-Informations)
 # Informations
-Outil multi-plateforme de gestion d'environnement virtuel Python pour la crÃ©ation, l'Ã©dition, la suppression ou le travail avec un environnement virtuel.<br>
+Outil multi-plateforme de gestion d'environnement virtuel Python pour la création, l'édition, la suppression ou le travail avec un environnement virtuel.<br>
 Tout se passe directement en console.<br>
 Il est possible de migrer ces anciens environnements virtuels sur cette solution.
 ## Prerequis
 - Python 3
 <br>
 
 # Installation
@@ -31,35 +22,35 @@
 ```
 <br>
 
 ## Installation d'un environnement
 ```console
 [user@host ~]$ zpenv --install [NomEnvironnement]
 ```
->- --name = Donner un nom Ã  notre environnement
->- --tag = Ajouter des tags (sÃ©parÃ©s avec ,)
+>- --name = Donner un nom à notre environnement
+>- --tag = Ajouter des tags (séparés avec ,)
 >- --comment = Ajouter un commentaire
->- --projectfolder = SpÃ©cifier le dossier du projet (emplacement du code)
+>- --projectfolder = Spécifier le dossier du projet (emplacement du code)
 (D'autres options sont disponibles)
 <br>
 
 ## Suppression d'un environnement
 ```console
 [user@host ~]$ zpenv --remove [NomEnvironnement]
 ```
 > --nopurge = Ne pas supprimer le dossier de l'environnement
-Le dossier du projet ne sera jamais supprimÃ©
+Le dossier du projet ne sera jamais supprimé
 <br>
 
 ## Migration d'un environnement
-Permet de rÃ©cupÃ©rer la gestion d'un environnement crÃ©Ã© par venv ou virtualenv par exemple.
+Permet de récupérer la gestion d'un environnement créé par venv ou virtualenv par exemple.
 ```console
 [user@host ~]$ zpenv --migrate [CheminVersEnvironnement]
 ```
-Si aucun chemin n'est spÃ©cifiÃ©, l'app prendra le rÃ©pertoire courant.
+Si aucun chemin n'est spécifié, l'app prendra le répertoire courant.
 <br><br>
 
 ## Lister les environnements disponibles
 ```console
 [user@host ~]$ zpenv --list
 - Project1
 - Project2
@@ -74,15 +65,15 @@
 Environment version:     3.10.8
 Environment tag:         ProjectConsole,TabBar
 Project Folder:          C:\Users\zephyroff\Desktop\ENVCode
 ```
 <br>
 
 ## Ouverture d'un environnement
-Pour activer l'environnement virtuel et commencer Ã  travailler dessus, il faut l'ouvrir.
+Pour activer l'environnement virtuel et commencer à travailler dessus, il faut l'ouvrir.
 ```console
 [user@host ~]$ zpenv --open [NomDeLEnvironnement]
 ```
 > --shell = Pour entrer directement dans le shell Python
 <br>
 
 ## Gestion de package
@@ -96,15 +87,15 @@
 ```
 
 ### Supprimer un package
 ```console
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
-### Mettre Ã  jour un package
+### Mettre à jour un package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
 <br><br>
 
 # EN - Informations
 Cross-platform Python virtual environment management tool for creating, editing, deleting, or working with a virtual environment.<br>
@@ -195,9 +186,8 @@
 ```console
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
 ### Update a package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
-```
-
+```
```

### Comparing `zpenv-1.1.1/README.md` & `zpenv-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+Metadata-Version: 2.1
+Name: zpenv
+Version: 1.1.2
+Summary: Gestionnaire d'environnement virtuel
+Home-page: https://github.com/ZephyrOff/py-zpenv
+Author: 
+License: MIT License
+Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
+Keywords: venv virtualenv terminal zephyroff
+Platform: ALL
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # zpenv
 # Langue/Language
 [English Version](#EN-Informations)
 # Informations
-Outil multi-plateforme de gestion d'environnement virtuel Python pour la création, l'édition, la suppression ou le travail avec un environnement virtuel.<br>
+Outil multi-plateforme de gestion d'environnement virtuel Python pour la crÃ©ation, l'Ã©dition, la suppression ou le travail avec un environnement virtuel.<br>
 Tout se passe directement en console.<br>
 Il est possible de migrer ces anciens environnements virtuels sur cette solution.
 ## Prerequis
 - Python 3
 <br>
 
 # Installation
@@ -22,35 +39,35 @@
 ```
 <br>
 
 ## Installation d'un environnement
 ```console
 [user@host ~]$ zpenv --install [NomEnvironnement]
 ```
->- --name = Donner un nom à notre environnement
->- --tag = Ajouter des tags (séparés avec ,)
+>- --name = Donner un nom Ã  notre environnement
+>- --tag = Ajouter des tags (sÃ©parÃ©s avec ,)
 >- --comment = Ajouter un commentaire
->- --projectfolder = Spécifier le dossier du projet (emplacement du code)
+>- --projectfolder = SpÃ©cifier le dossier du projet (emplacement du code)
 (D'autres options sont disponibles)
 <br>
 
 ## Suppression d'un environnement
 ```console
 [user@host ~]$ zpenv --remove [NomEnvironnement]
 ```
 > --nopurge = Ne pas supprimer le dossier de l'environnement
-Le dossier du projet ne sera jamais supprimé
+Le dossier du projet ne sera jamais supprimÃ©
 <br>
 
 ## Migration d'un environnement
-Permet de récupérer la gestion d'un environnement créé par venv ou virtualenv par exemple.
+Permet de rÃ©cupÃ©rer la gestion d'un environnement crÃ©Ã© par venv ou virtualenv par exemple.
 ```console
 [user@host ~]$ zpenv --migrate [CheminVersEnvironnement]
 ```
-Si aucun chemin n'est spécifié, l'app prendra le répertoire courant.
+Si aucun chemin n'est spÃ©cifiÃ©, l'app prendra le rÃ©pertoire courant.
 <br><br>
 
 ## Lister les environnements disponibles
 ```console
 [user@host ~]$ zpenv --list
 - Project1
 - Project2
@@ -65,15 +82,15 @@
 Environment version:     3.10.8
 Environment tag:         ProjectConsole,TabBar
 Project Folder:          C:\Users\zephyroff\Desktop\ENVCode
 ```
 <br>
 
 ## Ouverture d'un environnement
-Pour activer l'environnement virtuel et commencer à travailler dessus, il faut l'ouvrir.
+Pour activer l'environnement virtuel et commencer Ã  travailler dessus, il faut l'ouvrir.
 ```console
 [user@host ~]$ zpenv --open [NomDeLEnvironnement]
 ```
 > --shell = Pour entrer directement dans le shell Python
 <br>
 
 ## Gestion de package
@@ -87,15 +104,15 @@
 ```
 
 ### Supprimer un package
 ```console
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
-### Mettre à jour un package
+### Mettre Ã  jour un package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
 ```
 <br><br>
 
 # EN - Informations
 Cross-platform Python virtual environment management tool for creating, editing, deleting, or working with a virtual environment.<br>
@@ -186,8 +203,9 @@
 ```console
 [user@host ~]$ zpenv --removemodule [package]
 ```
 
 ### Update a package
 ```console
 [user@host ~]$ zpenv --upgrademodule [package]
-```
+```
+
```

### Comparing `zpenv-1.1.1/zpenv/zpenv.py` & `zpenv-1.1.2/zpenv/zpenv.py`

 * *Files identical despite different names*

### Comparing `zpenv-1.1.1/zpenv.egg-info/PKG-INFO` & `zpenv-1.1.2/zpenv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.1.1
+Version: 1.1.2
 Summary: Gestionnaire d'environnement virtuel
+Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
-License: UNKNOWN
+License: MIT License
+Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
+Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # zpenv
 # Langue/Language
 [English Version](#EN-Informations)
 # Informations
 Outil multi-plateforme de gestion d'environnement virtuel Python pour la crÃ©ation, l'Ã©dition, la suppression ou le travail avec un environnement virtuel.<br>
 Tout se passe directement en console.<br>
```

