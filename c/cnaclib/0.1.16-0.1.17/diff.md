# Comparing `tmp/cnaclib-0.1.16.tar.gz` & `tmp/cnaclib-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnaclib-0.1.16.tar", last modified: Wed May 31 08:07:16 2023, max compression
+gzip compressed data, was "cnaclib-0.1.17.tar", last modified: Tue Jun  6 13:18:43 2023, max compression
```

## Comparing `cnaclib-0.1.16.tar` & `cnaclib-0.1.17.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 08:07:16.588306 cnaclib-0.1.16/
--rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.16/LICENSE.txt
--rw-rw-rw-   0        0        0     2879 2023-05-31 08:07:16.584306 cnaclib-0.1.16/PKG-INFO
--rw-rw-rw-   0        0        0     1956 2023-05-30 11:25:19.000000 cnaclib-0.1.16/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 08:07:16.547302 cnaclib-0.1.16/cnaclib/
--rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.16/cnaclib/__init__.py
--rw-rw-rw-   0        0        0     7931 2023-05-22 15:45:17.000000 cnaclib-0.1.16/cnaclib/lSix.py
--rw-rw-rw-   0        0        0    23585 2023-05-31 07:35:47.000000 cnaclib-0.1.16/cnaclib/rac.py
--rw-rw-rw-   0        0        0       36 2023-05-22 15:54:04.000000 cnaclib-0.1.16/cnaclib/test.py
--rw-rw-rw-   0        0        0    21531 2023-05-31 07:37:31.000000 cnaclib-0.1.16/cnaclib/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-31 08:07:16.576305 cnaclib-0.1.16/cnaclib.egg-info/
--rw-rw-rw-   0        0        0     2879 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-31 08:07:15.000000 cnaclib-0.1.16/cnaclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 08:07:16.590306 cnaclib-0.1.16/setup.cfg
--rw-rw-rw-   0        0        0     1192 2023-05-31 07:31:23.000000 cnaclib-0.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:18:43.713052 cnaclib-0.1.17/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.17/LICENSE.txt
+-rw-rw-rw-   0        0        0     2879 2023-06-06 13:18:43.712051 cnaclib-0.1.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1956 2023-05-30 11:25:19.000000 cnaclib-0.1.17/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 13:18:43.669047 cnaclib-0.1.17/cnaclib/
+-rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.17/cnaclib/__init__.py
+-rw-rw-rw-   0        0        0     7931 2023-05-22 15:45:17.000000 cnaclib-0.1.17/cnaclib/lSix.py
+-rw-rw-rw-   0        0        0    23706 2023-06-06 13:17:30.000000 cnaclib-0.1.17/cnaclib/rac.py
+-rw-rw-rw-   0        0        0       36 2023-05-22 15:54:04.000000 cnaclib-0.1.17/cnaclib/test.py
+-rw-rw-rw-   0        0        0    21531 2023-05-31 07:37:31.000000 cnaclib-0.1.17/cnaclib/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-06 13:18:43.705051 cnaclib-0.1.17/cnaclib.egg-info/
+-rw-rw-rw-   0        0        0     2879 2023-06-06 13:18:41.000000 cnaclib-0.1.17/cnaclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-06 13:18:42.000000 cnaclib-0.1.17/cnaclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 13:18:41.000000 cnaclib-0.1.17/cnaclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-06-06 13:18:41.000000 cnaclib-0.1.17/cnaclib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 13:18:41.000000 cnaclib-0.1.17/cnaclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 13:18:43.715052 cnaclib-0.1.17/setup.cfg
+-rw-rw-rw-   0        0        0     1192 2023-06-06 13:18:27.000000 cnaclib-0.1.17/setup.py
```

### Comparing `cnaclib-0.1.16/LICENSE.txt` & `cnaclib-0.1.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.16/PKG-INFO` & `cnaclib-0.1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.16
+Version: 0.1.17
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
 Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC.
```

### Comparing `cnaclib-0.1.16/README.md` & `cnaclib-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.16/cnaclib/lSix.py` & `cnaclib-0.1.17/cnaclib/lSix.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.16/cnaclib/rac.py` & `cnaclib-0.1.17/cnaclib/rac.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,30 +192,34 @@
         CODMensuel : COD mensuelle.
         CODTotale : COD Totale à payer par l'employeur.
         '''
         
         if self.annee < 3 :
             CODMensuel = 0.0
             CODTotale = 0.0
-                
-        elif  self.annee >= 3 :
+            
+        elif  self.annee >= 3 and self.annee <21:
             CODMensuel =  0.8 * self.SMM
             CODTotale = (self.annee - 3) * CODMensuel
             if self.mois == 0 and self.jours == 0:
                 CODTotale += 0
             elif self.mois == 0 and self.jours > 0:
                 CODTotale +=  0.4 * self.SMM
             elif self.mois == 6 and self.jours == 0:
                 CODTotale += 0.4 * self.SMM
             elif self.mois == 6 and self.jours > 0:
                 CODTotale += 0.8 * self.SMM
             elif self.mois > 6:
                 CODTotale +=  0.8 * self.SMM
             elif self.mois < 6:
-                CODTotale += 0.4 * self.SMM            
+                CODTotale += 0.4 * self.SMM   
+        elif self.annee >=21:
+            CODMensuel =  0.8 * self.SMM
+            CODTotale = 18 * CODMensuel
+
         return CODMensuel, CODTotale
 
     def Cal_NumPeriode(self, dpc):
         '''
         Renvoi un dictionnaire qui comporte le numero de la période de prise en charge (de 1 a 4) ainsi que les numéros des mois (de 1 a dpc)
         qui appartienne a chaque periode.
```

### Comparing `cnaclib-0.1.16/cnaclib/tools.py` & `cnaclib-0.1.17/cnaclib/tools.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.16/cnaclib.egg-info/PKG-INFO` & `cnaclib-0.1.17/cnaclib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.16
+Version: 0.1.17
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
 Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC.
```

### Comparing `cnaclib-0.1.16/setup.py` & `cnaclib-0.1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 chemin = Path(__file__).parent
 long_description = (chemin / "README.md").read_text()
 
 
 setuptools.setup(
     name = 'cnaclib',
-    version = '0.1.16',
+    version = '0.1.17',
     author= 'BENHAMADA Nadir',
     author_email='aistatendz@gmail.com',
     description='Simulateur RAC',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=["certifi >=2023.5.7",
```

