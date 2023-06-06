# Comparing `tmp/hb_account_statement_banque_postale_csv-0.3.0.tar.gz` & `tmp/hb_account_statement_banque_postale_csv-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb_account_statement_banque_postale_csv-0.3.0.tar", last modified: Tue Jun  6 13:22:15 2023, max compression
+gzip compressed data, was "hb_account_statement_banque_postale_csv-0.3.1.tar", last modified: Tue Jun  6 13:30:27 2023, max compression
```

## Comparing `hb_account_statement_banque_postale_csv-0.3.0.tar` & `hb_account_statement_banque_postale_csv-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      633 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/COPYRIGHT
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    35147 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/LICENSE
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       81 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/MANIFEST.in
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2865 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/PKG-INFO
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1533 2023-06-06 13:19:56.000000 hb_account_statement_banque_postale_csv-0.3.0/README.rst
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.872521 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      562 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3148 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/account.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1307 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/configuration.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      490 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/configuration.xml
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      142 2022-06-20 10:29:22.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/tryton.cfg
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/view/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      472 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/view/configuration_form.xml
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2865 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      979 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/dependency_links.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      100 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/entry_points.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2022-06-20 10:34:43.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/not-zip-safe
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       47 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/requires.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       46 2023-06-06 13:22:15.000000 hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/top_level.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       70 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/setup.cfg
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2592 2023-06-06 13:20:23.000000 hb_account_statement_banque_postale_csv-0.3.0/setup.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:22:15.876521 hb_account_statement_banque_postale_csv-0.3.0/tests/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1861 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/01.csv
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      257 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3608 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/scenario_account_statement_banque_postale_csv.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      873 2023-06-06 13:18:21.000000 hb_account_statement_banque_postale_csv-0.3.0/tests/test_hb_account_statement_banque_postale_csv.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:30:27.622032 hb_account_statement_banque_postale_csv-0.3.1/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      633 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/COPYRIGHT
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    35147 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/LICENSE
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       81 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/MANIFEST.in
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2865 2023-06-06 13:30:27.622032 hb_account_statement_banque_postale_csv-0.3.1/PKG-INFO
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1533 2023-06-06 13:28:27.000000 hb_account_statement_banque_postale_csv-0.3.1/README.rst
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:30:27.622032 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      562 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4545 2023-06-06 13:28:06.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/account.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1307 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/configuration.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      490 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/configuration.xml
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      142 2022-06-20 10:29:22.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/tryton.cfg
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:30:27.622032 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/view/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      472 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/view/configuration_form.xml
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:30:27.622032 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2865 2023-06-06 13:30:27.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1056 2023-06-06 13:30:27.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2023-06-06 13:30:27.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      100 2023-06-06 13:30:27.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/entry_points.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2022-06-20 10:34:43.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/not-zip-safe
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       47 2023-06-06 13:30:27.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/requires.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       46 2023-06-06 13:30:27.000000 hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/top_level.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       70 2023-06-06 13:30:27.626032 hb_account_statement_banque_postale_csv-0.3.1/setup.cfg
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2534 2023-06-06 13:28:39.000000 hb_account_statement_banque_postale_csv-0.3.1/setup.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:30:27.622032 hb_account_statement_banque_postale_csv-0.3.1/tests/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1861 2022-06-20 10:25:47.000000 hb_account_statement_banque_postale_csv-0.3.1/tests/01.csv
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1794 2023-06-06 13:28:06.000000 hb_account_statement_banque_postale_csv-0.3.1/tests/02.csv
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-06-06 13:28:06.000000 hb_account_statement_banque_postale_csv-0.3.1/tests/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3301 2023-06-06 13:28:06.000000 hb_account_statement_banque_postale_csv-0.3.1/tests/scenario_account_statement_banque_postale_csv_new.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3608 2023-06-06 13:28:06.000000 hb_account_statement_banque_postale_csv-0.3.1/tests/scenario_account_statement_banque_postale_csv_old.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      405 2023-06-06 13:28:06.000000 hb_account_statement_banque_postale_csv-0.3.1/tests/test_hb_account_statement_banque_postale_csv.py
```

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/COPYRIGHT` & `hb_account_statement_banque_postale_csv-0.3.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/LICENSE` & `hb_account_statement_banque_postale_csv-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/PKG-INFO` & `hb_account_statement_banque_postale_csv-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb_account_statement_banque_postale_csv
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://hashbang.fr/
 Author: Hashbang
 Author-email: contact@hashbang.fr
 License: GPL-3
 Project-URL: Bug Tracker, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/-/issues
 Project-URL: Source Code, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/
 Keywords: tryton,banque postale
@@ -77,15 +77,15 @@
     If the the module **hb_bank_statement_machine_learning** is installed then 
     the party and account will be predict form the number on the line
 
 *********
 CHANGELOG
 *********
 
-0.3.0 (2022-06-06)
+0.3.1 (2022-06-06)
 ------------------
 
 * Format change, the script is modified to import old and new format, the old format will be removed in the next release
 
 0.2.0 (2022-06-20)
 ------------------
```

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/README.rst` & `hb_account_statement_banque_postale_csv-0.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     If the the module **hb_bank_statement_machine_learning** is installed then 
     the party and account will be predict form the number on the line
 
 *********
 CHANGELOG
 *********
 
-0.3.0 (2022-06-06)
+0.3.1 (2022-06-06)
 ------------------
 
 * Format change, the script is modified to import old and new format, the old format will be removed in the next release
 
 0.2.0 (2022-06-20)
 ------------------
```

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/__init__.py` & `hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv/configuration.py` & `hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv/configuration.py`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO` & `hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-account-statement-banque-postale-csv
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://hashbang.fr/
 Author: Hashbang
 Author-email: contact@hashbang.fr
 License: GPL-3
 Project-URL: Bug Tracker, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/-/issues
 Project-URL: Source Code, https://gitlab.com/hashbangfr/tryton-modules/hb_account_statement_banque_postale_csv/
 Keywords: tryton,banque postale
@@ -77,15 +77,15 @@
     If the the module **hb_bank_statement_machine_learning** is installed then 
     the party and account will be predict form the number on the line
 
 *********
 CHANGELOG
 *********
 
-0.3.0 (2022-06-06)
+0.3.1 (2022-06-06)
 ------------------
 
 * Format change, the script is modified to import old and new format, the old format will be removed in the next release
 
 0.2.0 (2022-06-20)
 ------------------
```

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt` & `hb_account_statement_banque_postale_csv-0.3.1/hb_account_statement_banque_postale_csv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,12 @@
 hb_account_statement_banque_postale_csv.egg-info/dependency_links.txt
 hb_account_statement_banque_postale_csv.egg-info/entry_points.txt
 hb_account_statement_banque_postale_csv.egg-info/not-zip-safe
 hb_account_statement_banque_postale_csv.egg-info/requires.txt
 hb_account_statement_banque_postale_csv.egg-info/top_level.txt
 hb_account_statement_banque_postale_csv/view/configuration_form.xml
 tests/01.csv
+tests/02.csv
 tests/__init__.py
-tests/scenario_account_statement_banque_postale_csv.rst
+tests/scenario_account_statement_banque_postale_csv_new.rst
+tests/scenario_account_statement_banque_postale_csv_old.rst
 tests/test_hb_account_statement_banque_postale_csv.py
```

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/setup.py` & `hb_account_statement_banque_postale_csv-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 requires = [
     'wheel',
     'tryton',
     'trytond',
     'trytond_account_statement',
 ]
 
-tests_require = ['proteus']
+tests_require = ['psycopg2', 'proteus']
 
 setup(
     name=name,
-    version='0.3.0',
+    version='0.3.1',
     description='',
     long_description=read('README.rst'),
     author='Hashbang',
     author_email='contact@hashbang.fr',
     url='https://hashbang.fr/',
     project_urls={
         "Bug Tracker": (
@@ -83,11 +83,9 @@
     install_requires=requires,
     zip_safe=False,
     entry_points={
         'trytond.modules': [
             f'{name}={name}',
         ],
     },
-    test_suite='tests',
-    test_loader='trytond.test_loader:Loader',
     tests_require=tests_require,
 )
```

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/tests/01.csv` & `hb_account_statement_banque_postale_csv-0.3.1/tests/01.csv`

 * *Files identical despite different names*

### Comparing `hb_account_statement_banque_postale_csv-0.3.0/tests/scenario_account_statement_banque_postale_csv.rst` & `hb_account_statement_banque_postale_csv-0.3.1/tests/scenario_account_statement_banque_postale_csv_old.rst`

 * *Files identical despite different names*

