# Comparing `tmp/hb_account_statement_banque_postale_csv-0.2.0.tar.gz` & `tmp/hb_account_statement_banque_postale_csv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb_account_statement_banque_postale_csv-0.2.0.tar", last modified: Mon Jun 20 10:34:45 2022, max compression
+gzip compressed data, was "hb_account_statement_banque_postale_csv-0.3.0.tar", last modified: Tue Jun  6 13:22:15 2023, max compression
```

## Comparing `hb_account_statement_banque_postale_csv-0.2.0.tar` & `hb_account_statement_banque_postale_csv-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2022-06-20 10:34:45.608720 hb_account_statement_banque_postale_csv-0.2.0/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      633 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/COPYRIGHT
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    35147 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/LICENSE
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       81 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/MANIFEST.in
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2704 2022-06-20 10:34:45.608720 hb_account_statement_banque_postale_csv-0.2.0/PKG-INFO
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1372 2022-06-20 10:28:44.000000 hb_account_statement_banque_postale_csv-0.2.0/README.rst
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2022-06-20 10:34:45.604720 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      562 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3148 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/account.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1307 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/configuration.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      490 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/configuration.xml
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      142 2022-06-20 10:29:22.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/tryton.cfg
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2022-06-20 10:34:45.604720 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/view/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      472 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/view/configuration_form.xml
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2022-06-20 10:34:45.604720 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2704 2022-06-20 10:34:45.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      979 2022-06-20 10:34:45.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2022-06-20 10:34:45.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/dependency_links.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      100 2022-06-20 10:34:45.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/entry_points.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2022-06-20 10:34:43.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/not-zip-safe
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       47 2022-06-20 10:34:45.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/requires.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       46 2022-06-20 10:34:45.000000 hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/top_level.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       70 2022-06-20 10:34:45.608720 hb_account_statement_banque_postale_csv-0.2.0/setup.cfg
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2592 2022-06-20 10:28:55.000000 hb_account_statement_banque_postale_csv-0.2.0/setup.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2022-06-20 10:34:45.608720 hb_account_statement_banque_postale_csv-0.2.0/tests/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1861 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/tests/01.csv
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      257 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/tests/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3608 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/tests/scenario_account_statement_banque_postale_csv.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      873 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.2.0/tests/test_hb_account_statement_banque_postale_csv.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      633 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/COPYRIGHT
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    35147 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/LICENSE
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       81 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/MANIFEST.in
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2865 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/PKG-INFO
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1533 2023-06-06 13:19:56.000000 hb_account_statement_banque_postale_csv-0.3.0/README.rst
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.872521 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      562 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3148 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/account.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1307 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/configuration.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      490 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/configuration.xml
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      142 2022-06-20 10:29:22.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/tryton.cfg
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/view/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      472 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/view/configuration_form.xml
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2865 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      979 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      100 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/entry_points.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2022-06-20 10:34:43.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/not-zip-safe
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       47 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/requires.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       46 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/top_level.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       70 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/setup.cfg
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2592 2023-06-06 13:20:23.000000 hb_account_statement_banque_postale_csv-0.3.0/setup.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/tests/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1861 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/01.csv
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      257 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3608 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/scenario_account_statement_banque_postale_csv.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      873 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/test_hb_account_statement_banque_postale_csv.py
```

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/COPYRIGHT` & `hb_account_statement_banque_postale_csv-0.3.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/LICENSE` & `hb_account_statement_banque_postale_csv-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/PKG-INFO` & `hb_account_statement_banque_postale_csv-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb_account_statement_banque_postale_csv
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://hashbang.fr/
 Author: Hashbang
 Author-email: contact@hashbang.fr
 License: GPL-3
 Project-URL: Bug Tracker, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/-/issues
 Project-URL: Source Code, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/
 Keywords: tryton,banque postale
@@ -77,14 +77,19 @@
     If the the module **hb_bank_statement_machine_learning** is installed then 
     the party and account will be predict form the number on the line
 
 *********
 CHANGELOG
 *********
 
+0.3.0 (2022-06-06)
+------------------
+
+* Format change, the script is modified to import old and new format, the old format will be removed in the next release
+
 0.2.0 (2022-06-20)
 ------------------
 
 * Fixed date during import
 * Fixed default account, if no account is defined use the account of the journal
```

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/README.rst` & `hb_account_statement_banque_postale_csv-0.3.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,19 @@
     If the the module **hb_bank_statement_machine_learning** is installed then 
     the party and account will be predict form the number on the line
 
 *********
 CHANGELOG
 *********
 
+0.3.0 (2022-06-06)
+------------------
+
+* Format change, the script is modified to import old and new format, the old format will be removed in the next release
+
 0.2.0 (2022-06-20)
 ------------------
 
 * Fixed date during import
 * Fixed default account, if no account is defined use the account of the journal
```

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/__init__.py` & `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/account.py` & `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/account.py`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv/configuration.py` & `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/configuration.py`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO` & `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-account-statement-banque-postale-csv
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://hashbang.fr/
 Author: Hashbang
 Author-email: contact@hashbang.fr
 License: GPL-3
 Project-URL: Bug Tracker, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/-/issues
 Project-URL: Source Code, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/
 Keywords: tryton,banque postale
@@ -77,14 +77,19 @@
     If the the module **hb_bank_statement_machine_learning** is installed then 
     the party and account will be predict form the number on the line
 
 *********
 CHANGELOG
 *********
 
+0.3.0 (2022-06-06)
+------------------
+
+* Format change, the script is modified to import old and new format, the old format will be removed in the next release
+
 0.2.0 (2022-06-20)
 ------------------
 
 * Fixed date during import
 * Fixed default account, if no account is defined use the account of the journal
```

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt` & `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/setup.py` & `hb_account_statement_banque_postale_csv-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     'trytond_account_statement',
 ]
 
 tests_require = ['proteus']
 
 setup(
     name=name,
-    version='0.2.0',
+    version='0.3.0',
     description='',
     long_description=read('README.rst'),
     author='Hashbang',
     author_email='contact@hashbang.fr',
     url='https://hashbang.fr/',
     project_urls={
         "Bug Tracker": (
```

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/tests/01.csv` & `hb_account_statement_banque_postale_csv-0.3.0/tests/01.csv`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/tests/scenario_account_statement_banque_postale_csv.rst` & `hb_account_statement_banque_postale_csv-0.3.0/tests/scenario_account_statement_banque_postale_csv.rst`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.2.0/tests/test_hb_account_statement_banque_postale_csv.py` & `hb_account_statement_banque_postale_csv-0.3.0/tests/test_hb_account_statement_banque_postale_csv.py`

 * *Files identical despite different names*

