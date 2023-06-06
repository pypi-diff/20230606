# Comparing `tmp/vertica-sqlalchemy-dialect-0.0.3.tar.gz` & `tmp/vertica-sqlalchemy-dialect-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.3.tar", last modified: Mon Jun  5 10:28:58 2023, max compression
+gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.4.tar", last modified: Tue Jun  6 17:05:22 2023, max compression
```

## Comparing `vertica-sqlalchemy-dialect-0.0.3.tar` & `vertica-sqlalchemy-dialect-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.139608 vertica-sqlalchemy-dialect-0.0.3/
--rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5742 2023-06-05 10:28:58.141609 vertica-sqlalchemy-dialect-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5395 2023-06-05 10:26:49.000000 vertica-sqlalchemy-dialect-0.0.3/README.rst
--rw-rw-rw-   0        0        0      211 2023-06-05 10:28:58.145603 vertica-sqlalchemy-dialect-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1916 2023-06-05 10:28:52.000000 vertica-sqlalchemy-dialect-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.054604 vertica-sqlalchemy-dialect-0.0.3/test/
--rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/test/test_core.py
--rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/test/test_integration.py
--rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/test/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.092608 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/
--rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/__init__.py
--rw-rw-rw-   0        0        0    68805 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/base.py
--rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_pyodbc.py
--rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_vertica_python.py
--rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/requirements.py
-drwxrwxrwx   0        0        0        0 2023-06-05 10:28:58.134602 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/
--rw-rw-rw-   0        0        0     5742 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-05 10:28:57.000000 vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.978170 vertica-sqlalchemy-dialect-0.0.4/
+-rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5749 2023-06-06 17:05:22.980141 vertica-sqlalchemy-dialect-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2023-06-06 16:57:33.000000 vertica-sqlalchemy-dialect-0.0.4/README.rst
+-rw-rw-rw-   0        0        0      211 2023-06-06 17:05:22.984145 vertica-sqlalchemy-dialect-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2023-06-06 16:58:01.000000 vertica-sqlalchemy-dialect-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.884139 vertica-sqlalchemy-dialect-0.0.4/test/
+-rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/test/test_core.py
+-rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/test/test_integration.py
+-rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.929143 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/
+-rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/__init__.py
+-rw-rw-rw-   0        0        0    68805 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/base.py
+-rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_pyodbc.py
+-rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_vertica_python.py
+-rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/requirements.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:22.973138 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/
+-rw-rw-rw-   0        0        0     5749 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-06 17:05:22.000000 vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/top_level.txt
```

### Comparing `vertica-sqlalchemy-dialect-0.0.3/LICENSE` & `vertica-sqlalchemy-dialect-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.3
+Version: 0.0.4
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
@@ -24,15 +24,15 @@
 Prerequisites
 -------------
 
 You will need the following softwares to run, build and test the dialect. Everything apart from Python and pip can be installed via pip itself.
 
 1. Python 3.x or higher
 2. pip 22 or higher
-3. SQLAlchemy 1.4.48
+3. sqlalchemy>=1.3.24,<=1.4
 4. vertica-python 1.1.1 or higher
 
 #####################################
 Vertica-Python
 #####################################
 
 `vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.3/README.rst` & `vertica-sqlalchemy-dialect-0.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,299 +40,299 @@
 00000270: 6869 6e67 2061 7061 7274 2066 726f 6d20  hing apart from 
 00000280: 5079 7468 6f6e 2061 6e64 2070 6970 2063  Python and pip c
 00000290: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
 000002a0: 7669 6120 7069 7020 6974 7365 6c66 2e0d  via pip itself..
 000002b0: 0a0d 0a31 2e20 5079 7468 6f6e 2033 2e78  ...1. Python 3.x
 000002c0: 206f 7220 6869 6768 6572 0d0a 322e 2070   or higher..2. p
 000002d0: 6970 2032 3220 6f72 2068 6967 6865 720d  ip 22 or higher.
-000002e0: 0a33 2e20 5351 4c41 6c63 6865 6d79 2031  .3. SQLAlchemy 1
-000002f0: 2e34 2e34 380d 0a34 2e20 7665 7274 6963  .4.48..4. vertic
-00000300: 612d 7079 7468 6f6e 2031 2e31 2e31 206f  a-python 1.1.1 o
-00000310: 7220 6869 6768 6572 0d0a 0d0a 2323 2323  r higher....####
-00000320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000002e0: 0a33 2e20 7371 6c61 6c63 6865 6d79 3e3d  .3. sqlalchemy>=
+000002f0: 312e 332e 3234 2c3c 3d31 2e34 0d0a 342e  1.3.24,<=1.4..4.
+00000300: 2076 6572 7469 6361 2d70 7974 686f 6e20   vertica-python 
+00000310: 312e 312e 3120 6f72 2068 6967 6865 720d  1.1.1 or higher.
+00000320: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
 00000330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000340: 230d 0a56 6572 7469 6361 2d50 7974 686f  #..Vertica-Pytho
-00000350: 6e0d 0a23 2323 2323 2323 2323 2323 2323  n..#############
+00000340: 2323 2323 2323 2323 0d0a 5665 7274 6963  ########..Vertic
+00000350: 612d 5079 7468 6f6e 0d0a 2323 2323 2323  a-Python..######
 00000360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000370: 2323 2323 2323 2323 0d0a 0d0a 6076 6572  ########....`ver
-00000380: 7469 6361 2d70 7974 686f 6e20 0d0a 3c68  tica-python ..<h
-00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003a0: 6d2f 7665 7274 6963 612f 7665 7274 6963  m/vertica/vertic
-000003b0: 612d 7079 7468 6f6e 3e60 5f20 6973 206e  a-python>`_ is n
-000003c0: 6565 6465 6420 746f 2075 7365 2074 6865  eeded to use the
-000003d0: 2056 6572 7469 6361 2d53 514c 416c 6368   Vertica-SQLAlch
-000003e0: 656d 792d 4469 616c 6563 742e 2054 6865  emy-Dialect. The
-000003f0: 2063 6f6e 6e65 6374 6f72 2064 6f65 7320   connector does 
-00000400: 6e6f 7420 6e65 6564 2074 6f20 6265 2069  not need to be i
-00000410: 6e73 7461 6c6c 6564 2061 7320 7468 6520  nstalled as the 
-00000420: 6469 616c 6563 7420 696e 7374 616c 6c61  dialect installa
-00000430: 7469 6f6e 2074 616b 6573 2063 6172 6520  tion takes care 
-00000440: 6f66 2069 742e 0d0a 0d0a 4e6f 7465 3a20  of it.....Note: 
-00000450: 5765 2072 6563 6f6d 6d65 6e64 2075 7369  We recommend usi
-00000460: 6e67 2074 6865 2076 6572 7469 6361 2d70  ng the vertica-p
-00000470: 7974 686f 6e20 636f 6e6e 6563 746f 722e  ython connector.
-00000480: 2048 6f77 6576 6572 2c20 7468 6520 6469   However, the di
-00000490: 616c 6563 7420 616c 736f 2061 6c6c 6f77  alect also allow
-000004a0: 7320 636f 6e6e 6563 7469 6e67 2075 7369  s connecting usi
-000004b0: 6e67 2060 7079 6f64 6263 203c 6874 7470  ng `pyodbc <http
-000004c0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000004d0: 6a65 6374 2f70 796f 6462 632f 3e60 5f2e  ject/pyodbc/>`_.
-000004e0: 204d 6f72 6520 696e 7374 7275 6374 696f   More instructio
-000004f0: 6e73 2061 7265 2061 7420 7468 6520 656e  ns are at the en
-00000500: 6420 6f66 2074 6869 7320 5245 4144 4d45  d of this README
-00000510: 2e0d 0a0d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .....-----------
+00000370: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+00000380: 0a0d 0a60 7665 7274 6963 612d 7079 7468  ...`vertica-pyth
+00000390: 6f6e 200d 0a3c 6874 7470 733a 2f2f 6769  on ..<https://gi
+000003a0: 7468 7562 2e63 6f6d 2f76 6572 7469 6361  thub.com/vertica
+000003b0: 2f76 6572 7469 6361 2d70 7974 686f 6e3e  /vertica-python>
+000003c0: 605f 2069 7320 6e65 6564 6564 2074 6f20  `_ is needed to 
+000003d0: 7573 6520 7468 6520 5665 7274 6963 612d  use the Vertica-
+000003e0: 5351 4c41 6c63 6865 6d79 2d44 6961 6c65  SQLAlchemy-Diale
+000003f0: 6374 2e20 5468 6520 636f 6e6e 6563 746f  ct. The connecto
+00000400: 7220 646f 6573 206e 6f74 206e 6565 6420  r does not need 
+00000410: 746f 2062 6520 696e 7374 616c 6c65 6420  to be installed 
+00000420: 6173 2074 6865 2064 6961 6c65 6374 2069  as the dialect i
+00000430: 6e73 7461 6c6c 6174 696f 6e20 7461 6b65  nstallation take
+00000440: 7320 6361 7265 206f 6620 6974 2e0d 0a0d  s care of it....
+00000450: 0a4e 6f74 653a 2057 6520 7265 636f 6d6d  .Note: We recomm
+00000460: 656e 6420 7573 696e 6720 7468 6520 7665  end using the ve
+00000470: 7274 6963 612d 7079 7468 6f6e 2063 6f6e  rtica-python con
+00000480: 6e65 6374 6f72 2e20 486f 7765 7665 722c  nector. However,
+00000490: 2074 6865 2064 6961 6c65 6374 2061 6c73   the dialect als
+000004a0: 6f20 616c 6c6f 7773 2063 6f6e 6e65 6374  o allows connect
+000004b0: 696e 6720 7573 696e 6720 6070 796f 6462  ing using `pyodb
+000004c0: 6320 3c68 7474 7073 3a2f 2f70 7970 692e  c <https://pypi.
+000004d0: 6f72 672f 7072 6f6a 6563 742f 7079 6f64  org/project/pyod
+000004e0: 6263 2f3e 605f 2e20 4d6f 7265 2069 6e73  bc/>`_. More ins
+000004f0: 7472 7563 7469 6f6e 7320 6172 6520 6174  tructions are at
+00000500: 2074 6865 2065 6e64 206f 6620 7468 6973   the end of this
+00000510: 2052 4541 444d 452e 0d0a 0d0a 2d2d 2d2d   README.....----
 00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 496e 7374  ----------..Inst
-00000540: 616c 6c69 6e67 2056 6572 7469 6361 2053  alling Vertica S
-00000550: 514c 416c 6368 656d 7920 4469 616c 6563  QLAlchemy Dialec
-00000560: 740d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  t..-------------
+00000530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000540: 2d0d 0a49 6e73 7461 6c6c 696e 6720 5665  -..Installing Ve
+00000550: 7274 6963 6120 5351 4c41 6c63 6865 6d79  rtica SQLAlchemy
+00000560: 2044 6961 6c65 6374 0d0a 2d2d 2d2d 2d2d   Dialect..------
 00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000580: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 5468 6520  --------....The 
-00000590: 5665 7274 6963 6120 5351 4c41 6c63 6865  Vertica SQLAlche
-000005a0: 6d79 2070 6163 6b61 6765 2063 616e 2062  my package can b
-000005b0: 6520 696e 7374 616c 6c65 6420 6672 6f6d  e installed from
-000005c0: 2074 6865 2070 7562 6c69 6320 5079 5049   the public PyPI
-000005d0: 2072 6570 6f73 6974 6f72 7920 7573 696e   repository usin
-000005e0: 6720 6070 6970 603a 200d 0a3a 3a0d 0a0d  g `pip`: ..::...
-000005f0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
-00000600: 202d 2d75 7067 7261 6465 2076 6572 7469   --upgrade verti
-00000610: 6361 2d73 716c 616c 6368 656d 792d 6469  ca-sqlalchemy-di
-00000620: 616c 6563 740d 0a0d 0a0d 0a60 7069 7060  alect......`pip`
-00000630: 2061 7574 6f6d 6174 6963 616c 6c79 2069   automatically i
-00000640: 6e73 7461 6c6c 7320 616c 6c20 7265 7175  nstalls all requ
-00000650: 6972 6564 206d 6f64 756c 6573 2c20 696e  ired modules, in
-00000660: 636c 7564 696e 6720 7665 7274 6963 612d  cluding vertica-
-00000670: 7079 7468 6f6e 2e0d 0a0d 0a46 6f72 206d  python.....For m
-00000680: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
-00000690: 6f6e 2069 6e73 7461 6c6c 6174 696f 6e20  on installation 
-000006a0: 616e 6420 7661 6c69 6461 7469 6f6e 2063  and validation c
-000006b0: 6865 636b 206f 7572 2067 6974 6875 6220  heck our github 
-000006c0: 7061 6765 2e0d 0a0d 0a2d 2d2d 2d2d 2d2d  page.....-------
+00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d  ---------------.
+00000590: 0a0d 0a54 6865 2056 6572 7469 6361 2053  ...The Vertica S
+000005a0: 514c 416c 6368 656d 7920 7061 636b 6167  QLAlchemy packag
+000005b0: 6520 6361 6e20 6265 2069 6e73 7461 6c6c  e can be install
+000005c0: 6564 2066 726f 6d20 7468 6520 7075 626c  ed from the publ
+000005d0: 6963 2050 7950 4920 7265 706f 7369 746f  ic PyPI reposito
+000005e0: 7279 2075 7369 6e67 2060 7069 7060 3a20  ry using `pip`: 
+000005f0: 0d0a 3a3a 0d0a 0d0a 2020 2020 7069 7020  ..::....    pip 
+00000600: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
+00000610: 6520 7665 7274 6963 612d 7371 6c61 6c63  e vertica-sqlalc
+00000620: 6865 6d79 2d64 6961 6c65 6374 0d0a 0d0a  hemy-dialect....
+00000630: 0d0a 6070 6970 6020 6175 746f 6d61 7469  ..`pip` automati
+00000640: 6361 6c6c 7920 696e 7374 616c 6c73 2061  cally installs a
+00000650: 6c6c 2072 6571 7569 7265 6420 6d6f 6475  ll required modu
+00000660: 6c65 732c 2069 6e63 6c75 6469 6e67 2076  les, including v
+00000670: 6572 7469 6361 2d70 7974 686f 6e2e 0d0a  ertica-python...
+00000680: 0d0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
+00000690: 6d61 7469 6f6e 206f 6e20 696e 7374 616c  mation on instal
+000006a0: 6c61 7469 6f6e 2061 6e64 2076 616c 6964  lation and valid
+000006b0: 6174 696f 6e20 6368 6563 6b20 6f75 7220  ation check our 
+000006c0: 6769 7468 7562 2070 6167 652e 0d0a 0d0a  github page.....
 000006d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000006e0: 0d0a 5061 7261 6d65 7465 7273 2061 6e64  ..Parameters and
-000006f0: 2042 6568 6176 696f 720d 0a2d 2d2d 2d2d   Behavior..-----
-00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000710: 2d2d 0d0a 0d0a 4173 206d 7563 6820 6173  --....As much as
-00000720: 2070 6f73 7369 626c 652c 2056 6572 7469   possible, Verti
-00000730: 6361 2053 514c 416c 6368 656d 7920 7072  ca SQLAlchemy pr
-00000740: 6f76 6964 6573 2063 6f6d 7061 7469 626c  ovides compatibl
-00000750: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
-00000760: 666f 7220 5351 4c41 6c63 6865 6d79 2061  for SQLAlchemy a
-00000770: 7070 6c69 6361 7469 6f6e 732e 200d 0a46  pplications. ..F
-00000780: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-00000790: 6e20 7573 696e 6720 5351 4c41 6c63 6865  n using SQLAlche
-000007a0: 6d79 2c20 7365 6520 7468 6520 6053 514c  my, see the `SQL
-000007b0: 416c 6368 656d 7920 646f 6375 6d65 6e74  Alchemy document
-000007c0: 6174 696f 6e0d 0a3c 6874 7470 3a2f 2f64  ation..<http://d
-000007d0: 6f63 732e 7371 6c61 6c63 6865 6d79 2e6f  ocs.sqlalchemy.o
-000007e0: 7267 2f65 6e2f 6c61 7465 7374 2f3e 605f  rg/en/latest/>`_
-000007f0: 2e0d 0a0d 0a4e 6f74 653a 2043 7572 7265  .....Note: Curre
-00000800: 6e74 2073 7461 7465 206f 6620 7468 6520  nt state of the 
-00000810: 6469 616c 6563 7420 6f6e 6c79 2073 7570  dialect only sup
-00000820: 706f 7274 7320 6d65 7461 6461 7461 2066  ports metadata f
-00000830: 756e 6374 696f 6e73 2e20 4974 2069 7320  unctions. It is 
-00000840: 7374 696c 6c20 756e 6465 7220 6465 7665  still under deve
-00000850: 6c6f 706d 656e 742e 200d 0a0d 0a48 6f77  lopment. ....How
-00000860: 6576 6572 2c20 5665 7274 6963 6120 5351  ever, Vertica SQ
-00000870: 4c41 6c63 6865 6d79 2061 6c73 6f20 7072  LAlchemy also pr
-00000880: 6f76 6964 6573 2073 7065 6369 6669 6320  ovides specific 
-00000890: 7061 7261 6d65 7465 7273 2061 6e64 2062  parameters and b
-000008a0: 6568 6176 696f 722c 2077 6869 6368 2061  ehavior, which a
-000008b0: 7265 2064 6573 6372 6962 6564 2069 6e20  re described in 
-000008c0: 7468 6520 666f 6c6c 6f77 696e 6720 7365  the following se
-000008d0: 6374 696f 6e73 2e0d 0a0d 0a23 2323 2323  ctions.....#####
-000008e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000008f0: 0d0a 436f 6e6e 6563 7469 6f6e 2050 6172  ..Connection Par
-00000900: 616d 6574 6572 730d 0a23 2323 2323 2323  ameters..#######
-00000910: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-00000920: 0d0a 5665 7274 6963 6120 5351 4c41 6c63  ..Vertica SQLAlc
-00000930: 6865 6d79 2044 6961 6c65 6374 2075 7365  hemy Dialect use
-00000940: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
-00000950: 7379 6e74 6178 2066 6f72 2074 6865 2063  syntax for the c
-00000960: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
-00000970: 2075 7365 6420 746f 2063 6f6e 6e65 6374   used to connect
-00000980: 2074 6f20 5665 7274 6963 6120 616e 6420   to Vertica and 
-00000990: 696e 6974 6961 7465 2061 2073 6573 7369  initiate a sessi
-000009a0: 6f6e 3a0d 0a3a 3a0d 0a0d 0a20 2020 2027  on:..::....    '
-000009b0: 7665 7274 6963 612b 7665 7274 6963 615f  vertica+vertica_
-000009c0: 7079 7468 6f6e 3a2f 2f3c 7573 6572 3e3a  python://<user>:
-000009d0: 3c70 6173 7377 6f72 643e 403c 686f 7374  <password>@<host
-000009e0: 5f6e 616d 653e 2f3c 6461 7461 6261 7365  _name>/<database
-000009f0: 5f6e 616d 653e 270d 0a0d 0a0d 0a57 6865  _name>'......Whe
-00000a00: 7265 3a0d 0a0d 0a2d 2060 3c75 7365 723e  re:....- `<user>
-00000a10: 6020 6973 2074 6865 206c 6f67 696e 206e  ` is the login n
-00000a20: 616d 6520 666f 7220 796f 7572 2056 6572  ame for your Ver
-00000a30: 7469 6361 2075 7365 722e 0d0a 2d20 603c  tica user...- `<
-00000a40: 7061 7373 776f 7264 3e60 2069 7320 7468  password>` is th
-00000a50: 6520 7061 7373 776f 7264 2066 6f72 2079  e password for y
-00000a60: 6f75 7220 5665 7274 6963 6120 7573 6572  our Vertica user
-00000a70: 2e0d 0a2d 2060 3c68 6f73 745f 6e61 6d65  ...- `<host_name
-00000a80: 3e60 2069 7320 7468 6520 4950 2f46 5144  >` is the IP/FQD
-00000a90: 4e20 6f66 2079 6f75 7220 5665 7274 6963  N of your Vertic
-00000aa0: 6120 486f 7374 2e0d 0a2d 2060 3c64 6174  a Host...- `<dat
-00000ab0: 6162 6173 655f 6e61 6d65 3e60 2069 7320  abase_name>` is 
-00000ac0: 7468 6520 6e61 6d65 206f 6620 796f 7572  the name of your
-00000ad0: 2056 6572 7469 6361 2044 6174 6162 6173   Vertica Databas
-00000ae0: 652e 0d0a 0d0a 0d0a 596f 7520 6361 6e20  e.......You can 
-00000af0: 6f70 7469 6f6e 616c 6c79 2073 7065 6369  optionally speci
-00000b00: 6679 2074 6865 2069 6e69 7469 616c 2064  fy the initial d
-00000b10: 6174 6162 6173 6520 616e 6420 7363 6865  atabase and sche
-00000b20: 6d61 2066 6f72 2074 6865 2056 6572 7469  ma for the Verti
-00000b30: 6361 2073 6573 7369 6f6e 2062 7920 696e  ca session by in
-00000b40: 636c 7564 696e 6720 7468 656d 2061 7420  cluding them at 
-00000b50: 7468 6520 656e 6420 6f66 2074 6865 2063  the end of the c
-00000b60: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
-00000b70: 2c20 7365 7061 7261 7465 6420 6279 2060  , separated by `
-00000b80: 2f60 2e20 596f 7520 6361 6e20 616c 736f  /`. You can also
-00000b90: 2073 7065 6369 6679 206f 7468 6572 2073   specify other s
-00000ba0: 7570 706f 7274 6564 2070 6172 616d 6574  upported paramet
-00000bb0: 6572 7320 6279 2076 6572 7469 6361 2d70  ers by vertica-p
-00000bc0: 7974 686f 6e20 6174 2074 6865 2065 6e64  ython at the end
-00000bd0: 206f 6620 7468 6520 636f 6e6e 6563 7469   of the connecti
-00000be0: 6f6e 2073 7472 696e 673a 0d0a 3a3a 0d0a  on string:..::..
-00000bf0: 0d0a 2020 2020 2776 6572 7469 6361 2b76  ..    'vertica+v
-00000c00: 6572 7469 6361 5f70 7974 686f 6e3a 2f2f  ertica_python://
-00000c10: 3c75 7365 723e 3a3c 7061 7373 776f 7264  <user>:<password
-00000c20: 3e40 3c68 6f73 745f 6e61 6d65 3e2f 3c64  >@<host_name>/<d
-00000c30: 6174 6162 6173 655f 6e61 6d65 3e3f 7365  atabase_name>?se
-00000c40: 7373 696f 6e5f 6c61 6265 6c3d 7371 6c61  ssion_label=sqla
-00000c50: 6c63 6865 6d79 2663 6f6e 6e65 6374 696f  lchemy&connectio
-00000c60: 6e5f 6c6f 6164 5f62 616c 616e 6365 3d31  n_load_balance=1
-00000c70: 270d 0a0d 0a46 6f72 206d 6f72 6520 696e  '....For more in
-00000c80: 666f 726d 6174 696f 6e2c 2063 6865 636b  formation, check
-00000c90: 206f 7574 2074 6865 2063 6f6e 6e65 6374   out the connect
-00000ca0: 696f 6e20 606f 7074 696f 6e73 203c 6874  ion `options <ht
-00000cb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000cc0: 2f76 6572 7469 6361 2f76 6572 7469 6361  /vertica/vertica
-00000cd0: 2d70 7974 686f 6e23 7365 742d 7072 6f70  -python#set-prop
-00000ce0: 6572 7469 6573 2d77 6974 682d 636f 6e6e  erties-with-conn
-00000cf0: 6563 7469 6f6e 2d73 7472 696e 673e 605f  ection-string>`_
-00000d00: 206f 6620 7665 7274 6963 612d 7079 7468   of vertica-pyth
-00000d10: 6f6e 2e0d 0a0d 0a23 2323 2323 2323 2323  on.....#########
+000006e0: 2d2d 2d2d 2d2d 2d0d 0a50 6172 616d 6574  -------..Paramet
+000006f0: 6572 7320 616e 6420 4265 6861 7669 6f72  ers and Behavior
+00000700: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
+00000710: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a41 7320  ---------....As 
+00000720: 6d75 6368 2061 7320 706f 7373 6962 6c65  much as possible
+00000730: 2c20 5665 7274 6963 6120 5351 4c41 6c63  , Vertica SQLAlc
+00000740: 6865 6d79 2070 726f 7669 6465 7320 636f  hemy provides co
+00000750: 6d70 6174 6962 6c65 2066 756e 6374 696f  mpatible functio
+00000760: 6e61 6c69 7479 2066 6f72 2053 514c 416c  nality for SQLAl
+00000770: 6368 656d 7920 6170 706c 6963 6174 696f  chemy applicatio
+00000780: 6e73 2e20 0d0a 466f 7220 696e 666f 726d  ns. ..For inform
+00000790: 6174 696f 6e20 6f6e 2075 7369 6e67 2053  ation on using S
+000007a0: 514c 416c 6368 656d 792c 2073 6565 2074  QLAlchemy, see t
+000007b0: 6865 2060 5351 4c41 6c63 6865 6d79 2064  he `SQLAlchemy d
+000007c0: 6f63 756d 656e 7461 7469 6f6e 0d0a 3c68  ocumentation..<h
+000007d0: 7474 703a 2f2f 646f 6373 2e73 716c 616c  ttp://docs.sqlal
+000007e0: 6368 656d 792e 6f72 672f 656e 2f6c 6174  chemy.org/en/lat
+000007f0: 6573 742f 3e60 5f2e 0d0a 0d0a 4e6f 7465  est/>`_.....Note
+00000800: 3a20 4375 7272 656e 7420 7374 6174 6520  : Current state 
+00000810: 6f66 2074 6865 2064 6961 6c65 6374 206f  of the dialect o
+00000820: 6e6c 7920 7375 7070 6f72 7473 206d 6574  nly supports met
+00000830: 6164 6174 6120 6675 6e63 7469 6f6e 732e  adata functions.
+00000840: 2049 7420 6973 2073 7469 6c6c 2075 6e64   It is still und
+00000850: 6572 2064 6576 656c 6f70 6d65 6e74 2e20  er development. 
+00000860: 0d0a 0d0a 486f 7765 7665 722c 2056 6572  ....However, Ver
+00000870: 7469 6361 2053 514c 416c 6368 656d 7920  tica SQLAlchemy 
+00000880: 616c 736f 2070 726f 7669 6465 7320 7370  also provides sp
+00000890: 6563 6966 6963 2070 6172 616d 6574 6572  ecific parameter
+000008a0: 7320 616e 6420 6265 6861 7669 6f72 2c20  s and behavior, 
+000008b0: 7768 6963 6820 6172 6520 6465 7363 7269  which are descri
+000008c0: 6265 6420 696e 2074 6865 2066 6f6c 6c6f  bed in the follo
+000008d0: 7769 6e67 2073 6563 7469 6f6e 732e 0d0a  wing sections...
+000008e0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+000008f0: 2323 2323 2323 230d 0a43 6f6e 6e65 6374  #######..Connect
+00000900: 696f 6e20 5061 7261 6d65 7465 7273 0d0a  ion Parameters..
+00000910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000920: 2323 2323 230d 0a0d 0a56 6572 7469 6361  #####....Vertica
+00000930: 2053 514c 416c 6368 656d 7920 4469 616c   SQLAlchemy Dial
+00000940: 6563 7420 7573 6573 2074 6865 2066 6f6c  ect uses the fol
+00000950: 6c6f 7769 6e67 2073 796e 7461 7820 666f  lowing syntax fo
+00000960: 7220 7468 6520 636f 6e6e 6563 7469 6f6e  r the connection
+00000970: 2073 7472 696e 6720 7573 6564 2074 6f20   string used to 
+00000980: 636f 6e6e 6563 7420 746f 2056 6572 7469  connect to Verti
+00000990: 6361 2061 6e64 2069 6e69 7469 6174 6520  ca and initiate 
+000009a0: 6120 7365 7373 696f 6e3a 0d0a 3a3a 0d0a  a session:..::..
+000009b0: 0d0a 2020 2020 2776 6572 7469 6361 2b76  ..    'vertica+v
+000009c0: 6572 7469 6361 5f70 7974 686f 6e3a 2f2f  ertica_python://
+000009d0: 3c75 7365 723e 3a3c 7061 7373 776f 7264  <user>:<password
+000009e0: 3e40 3c68 6f73 745f 6e61 6d65 3e2f 3c64  >@<host_name>/<d
+000009f0: 6174 6162 6173 655f 6e61 6d65 3e27 0d0a  atabase_name>'..
+00000a00: 0d0a 0d0a 5768 6572 653a 0d0a 0d0a 2d20  ....Where:....- 
+00000a10: 603c 7573 6572 3e60 2069 7320 7468 6520  `<user>` is the 
+00000a20: 6c6f 6769 6e20 6e61 6d65 2066 6f72 2079  login name for y
+00000a30: 6f75 7220 5665 7274 6963 6120 7573 6572  our Vertica user
+00000a40: 2e0d 0a2d 2060 3c70 6173 7377 6f72 643e  ...- `<password>
+00000a50: 6020 6973 2074 6865 2070 6173 7377 6f72  ` is the passwor
+00000a60: 6420 666f 7220 796f 7572 2056 6572 7469  d for your Verti
+00000a70: 6361 2075 7365 722e 0d0a 2d20 603c 686f  ca user...- `<ho
+00000a80: 7374 5f6e 616d 653e 6020 6973 2074 6865  st_name>` is the
+00000a90: 2049 502f 4651 444e 206f 6620 796f 7572   IP/FQDN of your
+00000aa0: 2056 6572 7469 6361 2048 6f73 742e 0d0a   Vertica Host...
+00000ab0: 2d20 603c 6461 7461 6261 7365 5f6e 616d  - `<database_nam
+00000ac0: 653e 6020 6973 2074 6865 206e 616d 6520  e>` is the name 
+00000ad0: 6f66 2079 6f75 7220 5665 7274 6963 6120  of your Vertica 
+00000ae0: 4461 7461 6261 7365 2e0d 0a0d 0a0d 0a59  Database.......Y
+00000af0: 6f75 2063 616e 206f 7074 696f 6e61 6c6c  ou can optionall
+00000b00: 7920 7370 6563 6966 7920 7468 6520 696e  y specify the in
+00000b10: 6974 6961 6c20 6461 7461 6261 7365 2061  itial database a
+00000b20: 6e64 2073 6368 656d 6120 666f 7220 7468  nd schema for th
+00000b30: 6520 5665 7274 6963 6120 7365 7373 696f  e Vertica sessio
+00000b40: 6e20 6279 2069 6e63 6c75 6469 6e67 2074  n by including t
+00000b50: 6865 6d20 6174 2074 6865 2065 6e64 206f  hem at the end o
+00000b60: 6620 7468 6520 636f 6e6e 6563 7469 6f6e  f the connection
+00000b70: 2073 7472 696e 672c 2073 6570 6172 6174   string, separat
+00000b80: 6564 2062 7920 602f 602e 2059 6f75 2063  ed by `/`. You c
+00000b90: 616e 2061 6c73 6f20 7370 6563 6966 7920  an also specify 
+00000ba0: 6f74 6865 7220 7375 7070 6f72 7465 6420  other supported 
+00000bb0: 7061 7261 6d65 7465 7273 2062 7920 7665  parameters by ve
+00000bc0: 7274 6963 612d 7079 7468 6f6e 2061 7420  rtica-python at 
+00000bd0: 7468 6520 656e 6420 6f66 2074 6865 2063  the end of the c
+00000be0: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
+00000bf0: 3a0d 0a3a 3a0d 0a0d 0a20 2020 2027 7665  :..::....    've
+00000c00: 7274 6963 612b 7665 7274 6963 615f 7079  rtica+vertica_py
+00000c10: 7468 6f6e 3a2f 2f3c 7573 6572 3e3a 3c70  thon://<user>:<p
+00000c20: 6173 7377 6f72 643e 403c 686f 7374 5f6e  assword>@<host_n
+00000c30: 616d 653e 2f3c 6461 7461 6261 7365 5f6e  ame>/<database_n
+00000c40: 616d 653e 3f73 6573 7369 6f6e 5f6c 6162  ame>?session_lab
+00000c50: 656c 3d73 716c 616c 6368 656d 7926 636f  el=sqlalchemy&co
+00000c60: 6e6e 6563 7469 6f6e 5f6c 6f61 645f 6261  nnection_load_ba
+00000c70: 6c61 6e63 653d 3127 0d0a 0d0a 466f 7220  lance=1'....For 
+00000c80: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00000c90: 2c20 6368 6563 6b20 6f75 7420 7468 6520  , check out the 
+00000ca0: 636f 6e6e 6563 7469 6f6e 2060 6f70 7469  connection `opti
+00000cb0: 6f6e 7320 3c68 7474 7073 3a2f 2f67 6974  ons <https://git
+00000cc0: 6875 622e 636f 6d2f 7665 7274 6963 612f  hub.com/vertica/
+00000cd0: 7665 7274 6963 612d 7079 7468 6f6e 2373  vertica-python#s
+00000ce0: 6574 2d70 726f 7065 7274 6965 732d 7769  et-properties-wi
+00000cf0: 7468 2d63 6f6e 6e65 6374 696f 6e2d 7374  th-connection-st
+00000d00: 7269 6e67 3e60 5f20 6f66 2076 6572 7469  ring>`_ of verti
+00000d10: 6361 2d70 7974 686f 6e2e 0d0a 0d0a 2323  ca-python.....##
 00000d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d30: 2323 2323 230d 0a4f 7065 6e69 6e67 2061  #####..Opening a
-00000d40: 6e64 2043 6c6f 7369 6e67 2043 6f6e 6e65  nd Closing Conne
-00000d50: 6374 696f 6e0d 0a23 2323 2323 2323 2323  ction..#########
+00000d30: 2323 2323 2323 2323 2323 2323 0d0a 4f70  ############..Op
+00000d40: 656e 696e 6720 616e 6420 436c 6f73 696e  ening and Closin
+00000d50: 6720 436f 6e6e 6563 7469 6f6e 0d0a 2323  g Connection..##
 00000d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d70: 2323 2323 230d 0a0d 0a4f 7065 6e20 6120  #####....Open a 
-00000d80: 636f 6e6e 6563 7469 6f6e 2062 7920 6578  connection by ex
-00000d90: 6563 7574 696e 6720 6065 6e67 696e 652e  ecuting `engine.
-00000da0: 636f 6e6e 6563 7428 2960 3b20 6176 6f69  connect()`; avoi
-00000db0: 6420 7573 696e 6720 6065 6e67 696e 652e  d using `engine.
-00000dc0: 6578 6563 7574 6528 2960 2e20 4d61 6b65  execute()`. Make
-00000dd0: 2063 6572 7461 696e 2074 6f20 636c 6f73   certain to clos
-00000de0: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
-00000df0: 2062 7920 6578 6563 7574 696e 6720 6063   by executing `c
-00000e00: 6f6e 6e65 6374 696f 6e2e 636c 6f73 6528  onnection.close(
-00000e10: 2960 2062 6566 6f72 650d 0a60 656e 6769  )` before..`engi
-00000e20: 6e65 2e64 6973 706f 7365 2829 603b 206f  ne.dispose()`; o
-00000e30: 7468 6572 7769 7365 2c20 7468 6520 5079  therwise, the Py
-00000e40: 7468 6f6e 2047 6172 6261 6765 2063 6f6c  thon Garbage col
-00000e50: 6c65 6374 6f72 2072 656d 6f76 6573 2074  lector removes t
-00000e60: 6865 2072 6573 6f75 7263 6573 2072 6571  he resources req
-00000e70: 7569 7265 6420 746f 2063 6f6d 6d75 6e69  uired to communi
-00000e80: 6361 7465 2077 6974 6820 5665 7274 6963  cate with Vertic
-00000e90: 612c 2070 7265 7665 6e74 696e 6720 7468  a, preventing th
-00000ea0: 6520 5079 7468 6f6e 2063 6f6e 6e65 6374  e Python connect
-00000eb0: 6f72 2066 726f 6d20 636c 6f73 696e 6720  or from closing 
-00000ec0: 7468 6520 7365 7373 696f 6e20 7072 6f70  the session prop
-00000ed0: 6572 6c79 2e0d 0a0d 0a3a 3a0d 0a0d 0a20  erly.....::.... 
-00000ee0: 2020 2065 6e67 696e 6520 3d20 6372 6561     engine = crea
-00000ef0: 7465 5f65 6e67 696e 6528 2e2e 2e29 0d0a  te_engine(...)..
-00000f00: 2020 2020 636f 6e6e 6563 7469 6f6e 203d      connection =
-00000f10: 2065 6e67 696e 652e 636f 6e6e 6563 7428   engine.connect(
-00000f20: 290d 0a20 2020 2074 7279 3a0d 0a20 2020  )..    try:..   
-00000f30: 2020 2020 2063 6f6e 6e65 6374 696f 6e2e       connection.
-00000f40: 6578 6563 7574 6528 3c53 514c 3e29 0d0a  execute(<SQL>)..
-00000f50: 2020 2020 6669 6e61 6c6c 793a 0d0a 2020      finally:..  
-00000f60: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
-00000f70: 2e63 6c6f 7365 2829 0d0a 2020 2020 2020  .close()..      
-00000f80: 2020 656e 6769 6e65 2e64 6973 706f 7365    engine.dispose
-00000f90: 2829 0d0a 0d0a 0d0a 2a2a 5573 696e 6720  ()......**Using 
-00000fa0: 7079 6f64 6263 2069 6e73 7465 6164 206f  pyodbc instead o
-00000fb0: 6620 7665 7274 6963 612d 7079 7468 6f6e  f vertica-python
-00000fc0: 2a2a 0d0a 0d0a 596f 7520 6d61 7920 7573  **....You may us
-00000fd0: 6520 7079 6f64 6263 2069 6e73 7465 6164  e pyodbc instead
-00000fe0: 206f 6620 7665 7274 6963 612d 7079 7468   of vertica-pyth
-00000ff0: 6f6e 2066 6f72 2074 6865 2063 6f6e 6e65  on for the conne
-00001000: 6374 696f 6e2e 0d0a 0d0a 2a43 7265 6174  ction.....*Creat
-00001010: 6520 6120 5665 7274 6963 6120 4453 4e2a  e a Vertica DSN*
-00001020: 200d 0a0d 0a0d 0a59 6f75 2077 696c 6c20   ......You will 
-00001030: 6e65 6564 2074 6f20 6861 7665 2061 2056  need to have a V
-00001040: 6572 7469 6361 204f 4442 4320 6472 6976  ertica ODBC driv
-00001050: 6572 2069 6e73 7461 6c6c 6564 2066 726f  er installed fro
-00001060: 6d20 6056 6572 7469 6361 2d43 6c69 656e  m `Vertica-Clien
-00001070: 742d 4472 6976 6572 7320 3c68 7474 7073  t-Drivers <https
-00001080: 3a2f 2f77 7777 2e76 6572 7469 6361 2e63  ://www.vertica.c
-00001090: 6f6d 2f64 6f77 6e6c 6f61 642f 7665 7274  om/download/vert
-000010a0: 6963 612f 636c 6965 6e74 2d64 7269 7665  ica/client-drive
-000010b0: 7273 2f3e 605f 2e20 466f 7220 7374 6570  rs/>`_. For step
-000010c0: 7320 746f 2069 6e73 7461 6c6c 204f 4442  s to install ODB
-000010d0: 4320 666f 7220 5665 7274 6963 612c 2066  C for Vertica, f
-000010e0: 6f6c 6c6f 7720 6f66 6669 6369 616c 2060  ollow official `
-000010f0: 5665 7274 6963 6120 446f 6373 203c 6874  Vertica Docs <ht
-00001100: 7470 733a 2f2f 7777 772e 7665 7274 6963  tps://www.vertic
-00001110: 612e 636f 6d2f 646f 6373 2f31 322e 302e  a.com/docs/12.0.
-00001120: 782f 4854 4d4c 2f43 6f6e 7465 6e74 2f41  x/HTML/Content/A
-00001130: 7574 686f 7269 6e67 2f43 6f6e 6e65 6374  uthoring/Connect
-00001140: 696e 6754 6f56 6572 7469 6361 2f43 6c69  ingToVertica/Cli
-00001150: 656e 744f 4442 432f 496e 7374 616c 6c69  entODBC/Installi
-00001160: 6e67 4f44 4243 2e68 746d 3e60 5f2e 0d0a  ngODBC.htm>`_...
-00001170: 0d0a 466f 7220 6578 616d 706c 652c 2079  ..For example, y
-00001180: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
-00001190: 636f 6e66 6967 7572 6520 7468 6573 6520  configure these 
-000011a0: 6669 6c65 7320 7769 7468 2079 6f75 7220  files with your 
-000011b0: 6372 6564 656e 7469 616c 733a 0d0a 0d0a  credentials:....
-000011c0: 602f 6574 632f 7665 7274 6963 612e 696e  `/etc/vertica.in
-000011d0: 6960 0d0a 3a3a 0d0a 0d0a 2020 2020 5b44  i`..::....    [D
-000011e0: 7269 7665 725d 0d0a 2020 2020 4572 726f  river]..    Erro
-000011f0: 724d 6573 7361 6765 7350 6174 6820 3d20  rMessagesPath = 
-00001200: 2f6f 7074 2f76 6572 7469 6361 2f6c 6962  /opt/vertica/lib
-00001210: 3634 2f0d 0a20 2020 204f 4442 4349 6e73  64/..    ODBCIns
-00001220: 744c 6962 203d 202f 7573 722f 6c69 622f  tLib = /usr/lib/
-00001230: 7838 365f 3634 2d6c 696e 7578 2d67 6e75  x86_64-linux-gnu
-00001240: 2f6c 6962 6f64 6263 696e 7374 2e73 6f0d  /libodbcinst.so.
-00001250: 0a20 2020 2044 7269 7665 724d 616e 6167  .    DriverManag
-00001260: 6572 456e 636f 6469 6e67 3d55 5446 2d31  erEncoding=UTF-1
-00001270: 360d 0a0d 0a0d 0a60 7e2f 2e6f 6462 632e  6......`~/.odbc.
-00001280: 696e 6960 0d0a 3a3a 0d0a 0d0a 2020 2020  ini`..::....    
-00001290: 5b4f 4442 4320 4461 7461 2053 6f75 7263  [ODBC Data Sourc
-000012a0: 6573 5d0d 0a20 2020 2076 6572 7469 6361  es]..    vertica
-000012b0: 203d 2022 4d79 2044 6174 6162 6173 6522   = "My Database"
-000012c0: 0d0a 0d0a 2020 2020 5b76 6572 7469 6361  ....    [vertica
-000012d0: 6473 6e5d 0d0a 2020 2020 4465 7363 7269  dsn]..    Descri
-000012e0: 7074 696f 6e20 3d20 4d79 2044 6174 6162  ption = My Datab
-000012f0: 6173 650d 0a20 2020 2044 7269 7665 7220  ase..    Driver 
-00001300: 3d20 2f6f 7074 2f76 6572 7469 6361 2f6c  = /opt/vertica/l
-00001310: 6962 3634 2f6c 6962 7665 7274 6963 616f  ib64/libverticao
-00001320: 6462 632e 736f 0d0a 2020 2020 4461 7461  dbc.so..    Data
-00001330: 6261 7365 203d 2064 6f63 6b65 720d 0a20  base = docker.. 
-00001340: 2020 2053 6572 7665 726e 616d 6520 3d20     Servername = 
-00001350: 3132 372e 302e 302e 310d 0a20 2020 2055  127.0.0.1..    U
-00001360: 4944 203d 2064 6261 646d 696e 0d0a 2020  ID = dbadmin..  
-00001370: 2020 5057 4420 3d0d 0a0d 0a0d 0a0d 0a54    PWD =........T
-00001380: 6865 6e20 7573 6520 7468 6520 5665 7274  hen use the Vert
-00001390: 6963 6120 4453 4e20 696e 2061 2066 696c  ica DSN in a fil
-000013a0: 6520 6c69 6b65 2073 6f3a 0d0a 3a3a 0d0a  e like so:..::..
-000013b0: 0d0a 2020 2020 6672 6f6d 2073 716c 616c  ..    from sqlal
-000013c0: 6368 656d 7920 696d 706f 7274 2063 7265  chemy import cre
-000013d0: 6174 655f 656e 6769 6e65 0d0a 0d0a 2020  ate_engine....  
-000013e0: 2020 656e 6769 6e65 203d 2073 612e 6372    engine = sa.cr
-000013f0: 6561 7465 5f65 6e67 696e 6528 2776 6572  eate_engine('ver
-00001400: 7469 6361 2b70 796f 6462 633a 2f2f 4076  tica+pyodbc://@v
-00001410: 6572 7469 6361 6473 6e27 290d 0a20 2020  erticadsn')..   
-00001420: 2074 7279 3a0d 0a20 2020 2020 2020 2072   try:..        r
-00001430: 6573 203d 2065 6e67 696e 652e 636f 6e6e  es = engine.conn
-00001440: 6563 7428 292e 7363 616c 6172 2827 7365  ect().scalar('se
-00001450: 6c65 6374 2076 6572 7369 6f6e 2829 3b27  lect version();'
-00001460: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00001470: 2872 6573 290d 0a20 2020 2066 696e 616c  (res)..    final
-00001480: 6c79 3a0d 0a20 2020 2020 2020 2063 6f6e  ly:..        con
-00001490: 6e65 6374 696f 6e2e 636c 6f73 6528 290d  nection.close().
-000014a0: 0a20 2020 2020 2020 2065 6e67 696e 652e  .        engine.
-000014b0: 6469 7370 6f73 6528 290d 0a0d 0a54 6869  dispose()....Thi
-000014c0: 7320 7368 6f75 6c64 2064 6973 706c 6179  s should display
-000014d0: 2074 6865 2056 6572 7469 6361 2076 6572   the Vertica ver
-000014e0: 7369 6f6e 2069 6e66 6f3a 2022 5665 7274  sion info: "Vert
-000014f0: 6963 6120 416e 616c 7974 6963 2044 6174  ica Analytic Dat
-00001500: 6162 6173 6520 7631 322e 302e 302d 3022  abase v12.0.0-0"
-00001510: 2e0d 0a                                  ...
+00000d70: 2323 2323 2323 2323 2323 2323 0d0a 0d0a  ############....
+00000d80: 4f70 656e 2061 2063 6f6e 6e65 6374 696f  Open a connectio
+00000d90: 6e20 6279 2065 7865 6375 7469 6e67 2060  n by executing `
+00000da0: 656e 6769 6e65 2e63 6f6e 6e65 6374 2829  engine.connect()
+00000db0: 603b 2061 766f 6964 2075 7369 6e67 2060  `; avoid using `
+00000dc0: 656e 6769 6e65 2e65 7865 6375 7465 2829  engine.execute()
+00000dd0: 602e 204d 616b 6520 6365 7274 6169 6e20  `. Make certain 
+00000de0: 746f 2063 6c6f 7365 2074 6865 2063 6f6e  to close the con
+00000df0: 6e65 6374 696f 6e20 6279 2065 7865 6375  nection by execu
+00000e00: 7469 6e67 2060 636f 6e6e 6563 7469 6f6e  ting `connection
+00000e10: 2e63 6c6f 7365 2829 6020 6265 666f 7265  .close()` before
+00000e20: 0d0a 6065 6e67 696e 652e 6469 7370 6f73  ..`engine.dispos
+00000e30: 6528 2960 3b20 6f74 6865 7277 6973 652c  e()`; otherwise,
+00000e40: 2074 6865 2050 7974 686f 6e20 4761 7262   the Python Garb
+00000e50: 6167 6520 636f 6c6c 6563 746f 7220 7265  age collector re
+00000e60: 6d6f 7665 7320 7468 6520 7265 736f 7572  moves the resour
+00000e70: 6365 7320 7265 7175 6972 6564 2074 6f20  ces required to 
+00000e80: 636f 6d6d 756e 6963 6174 6520 7769 7468  communicate with
+00000e90: 2056 6572 7469 6361 2c20 7072 6576 656e   Vertica, preven
+00000ea0: 7469 6e67 2074 6865 2050 7974 686f 6e20  ting the Python 
+00000eb0: 636f 6e6e 6563 746f 7220 6672 6f6d 2063  connector from c
+00000ec0: 6c6f 7369 6e67 2074 6865 2073 6573 7369  losing the sessi
+00000ed0: 6f6e 2070 726f 7065 726c 792e 0d0a 0d0a  on properly.....
+00000ee0: 3a3a 0d0a 0d0a 2020 2020 656e 6769 6e65  ::....    engine
+00000ef0: 203d 2063 7265 6174 655f 656e 6769 6e65   = create_engine
+00000f00: 282e 2e2e 290d 0a20 2020 2063 6f6e 6e65  (...)..    conne
+00000f10: 6374 696f 6e20 3d20 656e 6769 6e65 2e63  ction = engine.c
+00000f20: 6f6e 6e65 6374 2829 0d0a 2020 2020 7472  onnect()..    tr
+00000f30: 793a 0d0a 2020 2020 2020 2020 636f 6e6e  y:..        conn
+00000f40: 6563 7469 6f6e 2e65 7865 6375 7465 283c  ection.execute(<
+00000f50: 5351 4c3e 290d 0a20 2020 2066 696e 616c  SQL>)..    final
+00000f60: 6c79 3a0d 0a20 2020 2020 2020 2063 6f6e  ly:..        con
+00000f70: 6e65 6374 696f 6e2e 636c 6f73 6528 290d  nection.close().
+00000f80: 0a20 2020 2020 2020 2065 6e67 696e 652e  .        engine.
+00000f90: 6469 7370 6f73 6528 290d 0a0d 0a0d 0a2a  dispose()......*
+00000fa0: 2a55 7369 6e67 2070 796f 6462 6320 696e  *Using pyodbc in
+00000fb0: 7374 6561 6420 6f66 2076 6572 7469 6361  stead of vertica
+00000fc0: 2d70 7974 686f 6e2a 2a0d 0a0d 0a59 6f75  -python**....You
+00000fd0: 206d 6179 2075 7365 2070 796f 6462 6320   may use pyodbc 
+00000fe0: 696e 7374 6561 6420 6f66 2076 6572 7469  instead of verti
+00000ff0: 6361 2d70 7974 686f 6e20 666f 7220 7468  ca-python for th
+00001000: 6520 636f 6e6e 6563 7469 6f6e 2e0d 0a0d  e connection....
+00001010: 0a2a 4372 6561 7465 2061 2056 6572 7469  .*Create a Verti
+00001020: 6361 2044 534e 2a20 0d0a 0d0a 0d0a 596f  ca DSN* ......Yo
+00001030: 7520 7769 6c6c 206e 6565 6420 746f 2068  u will need to h
+00001040: 6176 6520 6120 5665 7274 6963 6120 4f44  ave a Vertica OD
+00001050: 4243 2064 7269 7665 7220 696e 7374 616c  BC driver instal
+00001060: 6c65 6420 6672 6f6d 2060 5665 7274 6963  led from `Vertic
+00001070: 612d 436c 6965 6e74 2d44 7269 7665 7273  a-Client-Drivers
+00001080: 203c 6874 7470 733a 2f2f 7777 772e 7665   <https://www.ve
+00001090: 7274 6963 612e 636f 6d2f 646f 776e 6c6f  rtica.com/downlo
+000010a0: 6164 2f76 6572 7469 6361 2f63 6c69 656e  ad/vertica/clien
+000010b0: 742d 6472 6976 6572 732f 3e60 5f2e 2046  t-drivers/>`_. F
+000010c0: 6f72 2073 7465 7073 2074 6f20 696e 7374  or steps to inst
+000010d0: 616c 6c20 4f44 4243 2066 6f72 2056 6572  all ODBC for Ver
+000010e0: 7469 6361 2c20 666f 6c6c 6f77 206f 6666  tica, follow off
+000010f0: 6963 6961 6c20 6056 6572 7469 6361 2044  icial `Vertica D
+00001100: 6f63 7320 3c68 7474 7073 3a2f 2f77 7777  ocs <https://www
+00001110: 2e76 6572 7469 6361 2e63 6f6d 2f64 6f63  .vertica.com/doc
+00001120: 732f 3132 2e30 2e78 2f48 544d 4c2f 436f  s/12.0.x/HTML/Co
+00001130: 6e74 656e 742f 4175 7468 6f72 696e 672f  ntent/Authoring/
+00001140: 436f 6e6e 6563 7469 6e67 546f 5665 7274  ConnectingToVert
+00001150: 6963 612f 436c 6965 6e74 4f44 4243 2f49  ica/ClientODBC/I
+00001160: 6e73 7461 6c6c 696e 674f 4442 432e 6874  nstallingODBC.ht
+00001170: 6d3e 605f 2e0d 0a0d 0a46 6f72 2065 7861  m>`_.....For exa
+00001180: 6d70 6c65 2c20 796f 7520 7769 6c6c 206e  mple, you will n
+00001190: 6565 6420 746f 2063 6f6e 6669 6775 7265  eed to configure
+000011a0: 2074 6865 7365 2066 696c 6573 2077 6974   these files wit
+000011b0: 6820 796f 7572 2063 7265 6465 6e74 6961  h your credentia
+000011c0: 6c73 3a0d 0a0d 0a60 2f65 7463 2f76 6572  ls:....`/etc/ver
+000011d0: 7469 6361 2e69 6e69 600d 0a3a 3a0d 0a0d  tica.ini`..::...
+000011e0: 0a20 2020 205b 4472 6976 6572 5d0d 0a20  .    [Driver].. 
+000011f0: 2020 2045 7272 6f72 4d65 7373 6167 6573     ErrorMessages
+00001200: 5061 7468 203d 202f 6f70 742f 7665 7274  Path = /opt/vert
+00001210: 6963 612f 6c69 6236 342f 0d0a 2020 2020  ica/lib64/..    
+00001220: 4f44 4243 496e 7374 4c69 6220 3d20 2f75  ODBCInstLib = /u
+00001230: 7372 2f6c 6962 2f78 3836 5f36 342d 6c69  sr/lib/x86_64-li
+00001240: 6e75 782d 676e 752f 6c69 626f 6462 6369  nux-gnu/libodbci
+00001250: 6e73 742e 736f 0d0a 2020 2020 4472 6976  nst.so..    Driv
+00001260: 6572 4d61 6e61 6765 7245 6e63 6f64 696e  erManagerEncodin
+00001270: 673d 5554 462d 3136 0d0a 0d0a 0d0a 607e  g=UTF-16......`~
+00001280: 2f2e 6f64 6263 2e69 6e69 600d 0a3a 3a0d  /.odbc.ini`..::.
+00001290: 0a0d 0a20 2020 205b 4f44 4243 2044 6174  ...    [ODBC Dat
+000012a0: 6120 536f 7572 6365 735d 0d0a 2020 2020  a Sources]..    
+000012b0: 7665 7274 6963 6120 3d20 224d 7920 4461  vertica = "My Da
+000012c0: 7461 6261 7365 220d 0a0d 0a20 2020 205b  tabase"....    [
+000012d0: 7665 7274 6963 6164 736e 5d0d 0a20 2020  verticadsn]..   
+000012e0: 2044 6573 6372 6970 7469 6f6e 203d 204d   Description = M
+000012f0: 7920 4461 7461 6261 7365 0d0a 2020 2020  y Database..    
+00001300: 4472 6976 6572 203d 202f 6f70 742f 7665  Driver = /opt/ve
+00001310: 7274 6963 612f 6c69 6236 342f 6c69 6276  rtica/lib64/libv
+00001320: 6572 7469 6361 6f64 6263 2e73 6f0d 0a20  erticaodbc.so.. 
+00001330: 2020 2044 6174 6162 6173 6520 3d20 646f     Database = do
+00001340: 636b 6572 0d0a 2020 2020 5365 7276 6572  cker..    Server
+00001350: 6e61 6d65 203d 2031 3237 2e30 2e30 2e31  name = 127.0.0.1
+00001360: 0d0a 2020 2020 5549 4420 3d20 6462 6164  ..    UID = dbad
+00001370: 6d69 6e0d 0a20 2020 2050 5744 203d 0d0a  min..    PWD =..
+00001380: 0d0a 0d0a 0d0a 5468 656e 2075 7365 2074  ......Then use t
+00001390: 6865 2056 6572 7469 6361 2044 534e 2069  he Vertica DSN i
+000013a0: 6e20 6120 6669 6c65 206c 696b 6520 736f  n a file like so
+000013b0: 3a0d 0a3a 3a0d 0a0d 0a20 2020 2066 726f  :..::....    fro
+000013c0: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
+000013d0: 6f72 7420 6372 6561 7465 5f65 6e67 696e  ort create_engin
+000013e0: 650d 0a0d 0a20 2020 2065 6e67 696e 6520  e....    engine 
+000013f0: 3d20 7361 2e63 7265 6174 655f 656e 6769  = sa.create_engi
+00001400: 6e65 2827 7665 7274 6963 612b 7079 6f64  ne('vertica+pyod
+00001410: 6263 3a2f 2f40 7665 7274 6963 6164 736e  bc://@verticadsn
+00001420: 2729 0d0a 2020 2020 7472 793a 0d0a 2020  ')..    try:..  
+00001430: 2020 2020 2020 7265 7320 3d20 656e 6769        res = engi
+00001440: 6e65 2e63 6f6e 6e65 6374 2829 2e73 6361  ne.connect().sca
+00001450: 6c61 7228 2773 656c 6563 7420 7665 7273  lar('select vers
+00001460: 696f 6e28 293b 2729 0d0a 2020 2020 2020  ion();')..      
+00001470: 2020 7072 696e 7428 7265 7329 0d0a 2020    print(res)..  
+00001480: 2020 6669 6e61 6c6c 793a 0d0a 2020 2020    finally:..    
+00001490: 2020 2020 636f 6e6e 6563 7469 6f6e 2e63      connection.c
+000014a0: 6c6f 7365 2829 0d0a 2020 2020 2020 2020  lose()..        
+000014b0: 656e 6769 6e65 2e64 6973 706f 7365 2829  engine.dispose()
+000014c0: 0d0a 0d0a 5468 6973 2073 686f 756c 6420  ....This should 
+000014d0: 6469 7370 6c61 7920 7468 6520 5665 7274  display the Vert
+000014e0: 6963 6120 7665 7273 696f 6e20 696e 666f  ica version info
+000014f0: 3a20 2256 6572 7469 6361 2041 6e61 6c79  : "Vertica Analy
+00001500: 7469 6320 4461 7461 6261 7365 2076 3132  tic Database v12
+00001510: 2e30 2e30 2d30 222e 0d0a                 .0.0-0"...
```

### Comparing `vertica-sqlalchemy-dialect-0.0.3/setup.py` & `vertica-sqlalchemy-dialect-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from setuptools import setup
 
 with open("README.rst", "r") as f:
     description = f.read()
 
 
-version_info = (0, 0, 3)
+version_info = (0, 0, 4)
 
 version = '.'.join(map(str, version_info))
 
 setup(
     name='vertica-sqlalchemy-dialect',
     version=version,
     description='Official Vertica dialect for SQLalchemy',
@@ -35,15 +35,15 @@
     url='https://github.com/vertica/vertica-sqlalchemy-dialect',
     author='Narendra Prabhu',
     packages=(
         'vertica_sqlalchemy_dialect',
     ),
     install_requires=(
         'six >= 1.10.0',
-        'sqlalchemy==1.4.48',
+        'sqlalchemy>=1.3.24,<=1.4',
         'vertica-python>=1.1.1'
     ),
     extras_require={
         'pyodbc': [
             'pyodbc>=4.0.16',
         ],
         'vertica-python': [
```

### Comparing `vertica-sqlalchemy-dialect-0.0.3/test/test_core.py` & `vertica-sqlalchemy-dialect-0.0.4/test/test_core.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/test/test_integration.py` & `vertica-sqlalchemy-dialect-0.0.4/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/test/test_suite.py` & `vertica-sqlalchemy-dialect-0.0.4/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/base.py` & `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/base.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_pyodbc.py` & `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_pyodbc.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/dialect_vertica_python.py` & `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/dialect_vertica_python.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect/requirements.py` & `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect/requirements.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.3
+Version: 0.0.4
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
@@ -24,15 +24,15 @@
 Prerequisites
 -------------
 
 You will need the following softwares to run, build and test the dialect. Everything apart from Python and pip can be installed via pip itself.
 
 1. Python 3.x or higher
 2. pip 22 or higher
-3. SQLAlchemy 1.4.48
+3. sqlalchemy>=1.3.24,<=1.4
 4. vertica-python 1.1.1 or higher
 
 #####################################
 Vertica-Python
 #####################################
 
 `vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.3/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt` & `vertica-sqlalchemy-dialect-0.0.4/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

