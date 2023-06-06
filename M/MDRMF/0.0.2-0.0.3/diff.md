# Comparing `tmp/MDRMF-0.0.2.tar.gz` & `tmp/MDRMF-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDRMF-0.0.2.tar", last modified: Tue May 23 11:39:05 2023, max compression
+gzip compressed data, was "MDRMF-0.0.3.tar", last modified: Tue Jun  6 17:41:25 2023, max compression
```

## Comparing `MDRMF-0.0.2.tar` & `MDRMF-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.872810 MDRMF-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.816806 MDRMF-0.0.2/MDRMF/
--rw-rw-rw-   0        0        0      153 2023-05-23 10:29:57.000000 MDRMF-0.0.2/MDRMF/__init__.py
--rw-rw-rw-   0        0        0     2702 2023-05-23 10:04:01.000000 MDRMF-0.0.2/MDRMF/dataset.py
--rw-rw-rw-   0        0        0     3808 2023-05-15 19:01:09.000000 MDRMF-0.0.2/MDRMF/featurizer.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.866810 MDRMF-0.0.2/MDRMF/models/
--rw-rw-rw-   0        0        0       86 2023-05-23 10:56:06.000000 MDRMF-0.0.2/MDRMF/models/__init__.py
--rw-rw-rw-   0        0        0     1736 2023-05-23 11:07:29.000000 MDRMF-0.0.2/MDRMF/models/modeller.py
--rw-rw-rw-   0        0        0     1847 2023-05-23 11:12:03.000000 MDRMF-0.0.2/MDRMF/models/rfmodeller.py
--rw-rw-rw-   0        0        0     2634 2023-05-15 18:57:32.000000 MDRMF-0.0.2/MDRMF/moleculeloader.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:39:05.860949 MDRMF-0.0.2/MDRMF.egg-info/
--rw-rw-rw-   0        0        0      436 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-23 11:39:05.000000 MDRMF-0.0.2/MDRMF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      436 2023-05-23 11:39:05.871812 MDRMF-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 11:39:05.873810 MDRMF-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-23 11:37:14.000000 MDRMF-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.994315 MDRMF-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.946315 MDRMF-0.0.3/MDRMF/
+-rw-rw-rw-   0        0        0      284 2023-06-06 17:40:38.000000 MDRMF-0.0.3/MDRMF/__init__.py
+-rw-rw-rw-   0        0        0     3839 2023-06-06 07:35:43.000000 MDRMF-0.0.3/MDRMF/dataset.py
+-rw-rw-rw-   0        0        0     2002 2023-06-02 06:30:06.000000 MDRMF-0.0.3/MDRMF/evaluator.py
+-rw-rw-rw-   0        0        0     6928 2023-06-06 17:32:00.000000 MDRMF-0.0.3/MDRMF/experimenter.py
+-rw-rw-rw-   0        0        0     3808 2023-06-02 13:46:50.000000 MDRMF-0.0.3/MDRMF/featurizer.py
+-rw-rw-rw-   0        0        0     1727 2023-06-06 08:00:32.000000 MDRMF-0.0.3/MDRMF/model.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.989311 MDRMF-0.0.3/MDRMF/models/
+-rw-rw-rw-   0        0        0       86 2023-05-23 10:56:06.000000 MDRMF-0.0.3/MDRMF/models/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-06-06 07:36:51.000000 MDRMF-0.0.3/MDRMF/models/modeller.py
+-rw-rw-rw-   0        0        0     3634 2023-06-06 17:37:35.000000 MDRMF-0.0.3/MDRMF/models/rfmodeller.py
+-rw-rw-rw-   0        0        0     2643 2023-06-02 14:00:31.000000 MDRMF-0.0.3/MDRMF/moleculeloader.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:41:25.974316 MDRMF-0.0.3/MDRMF.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 17:41:25.000000 MDRMF-0.0.3/MDRMF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      436 2023-06-06 17:41:25.993317 MDRMF-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-11 07:27:32.000000 MDRMF-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:41:25.995314 MDRMF-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-06-05 18:45:57.000000 MDRMF-0.0.3/setup.py
```

### Comparing `MDRMF-0.0.2/MDRMF/featurizer.py` & `MDRMF-0.0.3/MDRMF/featurizer.py`

 * *Files identical despite different names*

### Comparing `MDRMF-0.0.2/MDRMF/moleculeloader.py` & `MDRMF-0.0.3/MDRMF/moleculeloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     def _process_data(self):
         """
         Processes the loaded DataFrame.
         """
         if 'molecules' not in self._df.columns:
             self._df['molecules'] = self._df[self.smi_col].apply(Chem.MolFromSmiles)
 
-        self._df.rename(columns={self.scores_col: "scores"}, inplace=True)
-        self._df.rename(columns={self.smi_col: "SMILES"}, inplace=True)
+        #self._df.rename(columns={self.scores_col: "scores"}, inplace=True)
+        #self._df.rename(columns={self.smi_col: "SMILES"}, inplace=True)
 
-        self._df.sort_values(by="scores")
+        self._df.sort_values(by=self.scores_col)
 
     @property
     def df(self):
         """
         Provides access to the loaded and processed DataFrame.
 
         If the data has not been loaded yet, it is loaded automatically
```

