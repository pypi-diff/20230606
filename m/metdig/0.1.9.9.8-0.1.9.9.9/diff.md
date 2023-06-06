# Comparing `tmp/metdig-0.1.9.9.8-py3-none-any.whl.zip` & `tmp/metdig-0.1.9.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8828157 bytes, number of entries: 722
--rw-rw-rw-  2.0 fat     1654 b- defN 22-Sep-22 06:37 metdig/__init__.py
+Zip file size: 8828165 bytes, number of entries: 722
+-rw-rw-rw-  2.0 fat     1654 b- defN 22-Sep-27 03:55 metdig/__init__.py
 -rw-rw-rw-  2.0 fat      779 b- defN 21-Jun-17 10:06 metdig/package_tools.py
 -rw-rw-rw-  2.0 fat     1883 b- defN 22-Sep-22 06:45 metdig/__pycache__/__init__.cpython-38.pyc
 -rw-rw-rw-  2.0 fat      849 b- defN 21-Jun-18 06:15 metdig/__pycache__/package_tools.cpython-38.pyc
 -rw-rw-rw-  2.0 fat      233 b- defN 21-Dec-29 08:34 metdig/cal/__init__.py
 -rw-rw-rw-  2.0 fat     5370 b- defN 21-Aug-11 08:14 metdig/cal/cross_sections_module.py
 -rw-rw-rw-  2.0 fat    11039 b- defN 22-May-31 07:56 metdig/cal/dynamic.py
 -rw-rw-rw-  2.0 fat       43 b- defN 21-Apr-25 02:23 metdig/cal/elements.py
@@ -712,13 +712,13 @@
 -rw-rw-rw-  2.0 fat    19166 b- defN 22-Jun-14 01:38 metdig/utl/utl_stda_station.py
 -rw-rw-rw-  2.0 fat     3723 b- defN 21-Aug-11 08:14 metdig/utl/utl_units.py
 -rw-rw-rw-  2.0 fat      274 b- defN 21-Apr-25 03:05 metdig/utl/__pycache__/__init__.cpython-38.pyc
 -rw-rw-rw-  2.0 fat     2189 b- defN 21-Aug-09 09:09 metdig/utl/__pycache__/utl_stda_attrs.cpython-38.pyc
 -rw-rw-rw-  2.0 fat    21929 b- defN 22-Jun-23 14:27 metdig/utl/__pycache__/utl_stda_grid.cpython-38.pyc
 -rw-rw-rw-  2.0 fat    16451 b- defN 22-Jun-14 01:38 metdig/utl/__pycache__/utl_stda_station.cpython-38.pyc
 -rw-rw-rw-  2.0 fat     1256 b- defN 21-Aug-11 08:16 metdig/utl/__pycache__/utl_units.cpython-38.pyc
--rw-rw-rw-  2.0 fat    35821 b- defN 22-Sep-22 06:49 metdig-0.1.9.9.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 22-Sep-22 06:49 metdig-0.1.9.9.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 22-Sep-22 06:49 metdig-0.1.9.9.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 22-Sep-22 06:49 metdig-0.1.9.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    76322 b- defN 22-Sep-22 06:49 metdig-0.1.9.9.8.dist-info/RECORD
-722 files, 19873566 bytes uncompressed, 8702553 bytes compressed:  56.2%
+-rw-rw-rw-  2.0 fat    35821 b- defN 22-Sep-27 03:59 metdig-0.1.9.9.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      534 b- defN 22-Sep-27 03:59 metdig-0.1.9.9.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 22-Sep-27 03:59 metdig-0.1.9.9.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 22-Sep-27 03:58 metdig-0.1.9.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    76322 b- defN 22-Sep-27 03:59 metdig-0.1.9.9.9.dist-info/RECORD
+722 files, 19873618 bytes uncompressed, 8702561 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -2145,23 +2145,23 @@
 
 Filename: metdig/utl/__pycache__/utl_stda_station.cpython-38.pyc
 Comment: 
 
 Filename: metdig/utl/__pycache__/utl_units.cpython-38.pyc
 Comment: 
 
-Filename: metdig-0.1.9.9.8.dist-info/LICENSE
+Filename: metdig-0.1.9.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: metdig-0.1.9.9.8.dist-info/METADATA
+Filename: metdig-0.1.9.9.9.dist-info/METADATA
 Comment: 
 
-Filename: metdig-0.1.9.9.8.dist-info/WHEEL
+Filename: metdig-0.1.9.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: metdig-0.1.9.9.8.dist-info/top_level.txt
+Filename: metdig-0.1.9.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: metdig-0.1.9.9.8.dist-info/RECORD
+Filename: metdig-0.1.9.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metdig/__init__.py

```diff
@@ -1,9 +1,9 @@
 __author__ = "The R & D Center for Weather Forecasting Technology in NMC, CMA"
-__version__ = '0.1.9.9.8'
+__version__ = '0.1.9.9.9'
 
 from . import cal
 from . import graphics
 from . import hub
 from . import io
 from . import onestep
 from . import products
```

## Comparing `metdig-0.1.9.9.8.dist-info/LICENSE` & `metdig-0.1.9.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `metdig-0.1.9.9.8.dist-info/RECORD` & `metdig-0.1.9.9.9.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-metdig/__init__.py,sha256=4wsKmgi22uJIsiTqC6cCK3Q1fNwIhsg341_b7ADln18,1654
+metdig/__init__.py,sha256=uqn8DFCNPQCMi5aBxrD1FCoSZO3HI_aGStzRNZs_FuU,1654
 metdig/package_tools.py,sha256=MCLXoEL7ujmrjngmpAhVCTLFs7pXtKcPNZkp1rS24fU,779
 metdig/__pycache__/__init__.cpython-38.pyc,sha256=tc1wpoAro6Jq1mauWj5NTxwosngYh1-v0R5LErpoz-E,1883
 metdig/__pycache__/package_tools.cpython-38.pyc,sha256=zgf5pi59vYkRBl4LPaR1UNmTt4EuQH2xgRmqSSgEK5E,849
 metdig/cal/__init__.py,sha256=3fCYgBqusM5DRlFBBg8439IjBoZjXbELG9aQm_DZ-SU,233
 metdig/cal/cross_sections_module.py,sha256=7inx5Gssv8poI3CyCYfkMWmRuoiRDfzAqAIlNw_1Yv4,5370
 metdig/cal/dynamic.py,sha256=qk4_w_oLmdxgPLmJCRiGmS8-UJbHG1cvg52qowBjOcU,11039
 metdig/cal/elements.py,sha256=pMKpelA7wuC4UfyJCB-0sg5E5UZY6LruXXMfdppn3nY,43
@@ -711,12 +711,12 @@
 metdig/utl/utl_stda_station.py,sha256=tJwlzMJ--7-N155GATek1XdaJDOYje00sfO-DQt_7Pk,19166
 metdig/utl/utl_units.py,sha256=9sgEcNNByVvVcRSL5bZ1o8cv2wLSvUQTFyPdthZ7J-A,3723
 metdig/utl/__pycache__/__init__.cpython-38.pyc,sha256=0qzsQJQLIhcwV_Ft74OzLohmJhuLGMick-Yqz7fKgyo,274
 metdig/utl/__pycache__/utl_stda_attrs.cpython-38.pyc,sha256=QqsLj2Byxwo0ECACu7UQlP06_kgGw4VA7fY8hl152zA,2189
 metdig/utl/__pycache__/utl_stda_grid.cpython-38.pyc,sha256=0pCUOunXAkAGWTgLyMIJO_j0b5e7eVWHUu1MYhrGwpQ,21929
 metdig/utl/__pycache__/utl_stda_station.cpython-38.pyc,sha256=44XxhvFq0zCgDV09iIaA-eqaxLYT1pzk2QQs53_tcvA,16451
 metdig/utl/__pycache__/utl_units.cpython-38.pyc,sha256=TLiu906HPGH-DEopWT1VxftS7i5mss2cSQwFh4mcsIk,1256
-metdig-0.1.9.9.8.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-metdig-0.1.9.9.8.dist-info/METADATA,sha256=_p_zfpNQkyjNEqTdFAwZaYp5CV4Ftzln5U3SPrLj_lI,482
-metdig-0.1.9.9.8.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-metdig-0.1.9.9.8.dist-info/top_level.txt,sha256=yGvlgmMUUGilkJMIfC2kgNUC6gj0fktK8D8cZUziu3E,7
-metdig-0.1.9.9.8.dist-info/RECORD,,
+metdig-0.1.9.9.9.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+metdig-0.1.9.9.9.dist-info/METADATA,sha256=luevjFS-3NmPEaTVE_JjVUZkwWEzAju3mrgDBYWGFhY,534
+metdig-0.1.9.9.9.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+metdig-0.1.9.9.9.dist-info/top_level.txt,sha256=yGvlgmMUUGilkJMIfC2kgNUC6gj0fktK8D8cZUziu3E,7
+metdig-0.1.9.9.9.dist-info/RECORD,,
```

