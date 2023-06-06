# Comparing `tmp/giefstat-0.0.5.tar.gz` & `tmp/giefstat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.5.tar", last modified: Mon Jun  5 15:34:18 2023, max compression
+gzip compressed data, was "giefstat-0.0.6.tar", last modified: Tue Jun  6 07:13:43 2023, max compression
```

## Comparing `giefstat-0.0.5.tar` & `giefstat-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.843501 giefstat-0.0.5/
--rw-rw-rw-   0        0        0     3561 2023-06-05 15:34:18.842503 giefstat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3170 2023-06-05 14:19:49.000000 giefstat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.739779 giefstat-0.0.5/giefstat/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:49:40.000000 giefstat-0.0.5/giefstat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.755737 giefstat-0.0.5/giefstat/estimate/
--rw-rw-rw-   0        0        0     3953 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/__init__.py
--rw-rw-rw-   0        0        0     5258 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/_univar_encoding.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.757731 giefstat-0.0.5/giefstat/estimate/gief/
--rw-rw-rw-   0        0        0      414 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.763714 giefstat-0.0.5/giefstat/estimate/gief/entropy/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/entropy/__init__.py
--rw-rw-rw-   0        0        0      915 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/entropy/cond_entropy.py
--rw-rw-rw-   0        0        0     2602 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/entropy/marg_entropy.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.773688 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/__init__.py
--rw-rw-rw-   0        0        0    11405 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/_kraskov.py
--rw-rw-rw-   0        0        0     2767 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/_ross.py
--rw-rw-rw-   0        0        0     2651 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/cmi.py
--rw-rw-rw-   0        0        0     1931 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/gief/mutual_info/mi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.777678 giefstat-0.0.5/giefstat/estimate/kde/
--rw-rw-rw-   0        0        0       89 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/kde/__init__.py
--rw-rw-rw-   0        0        0     3015 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/kde/kde.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.781666 giefstat-0.0.5/giefstat/estimate/mic/
--rw-rw-rw-   0        0        0      194 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/mic/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/mic/_mic_rmic.py
--rw-rw-rw-   0        0        0     2802 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/mic/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.785657 giefstat-0.0.5/giefstat/estimate/model_based/
--rw-rw-rw-   0        0        0      260 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/model_based/__init__.py
--rw-rw-rw-   0        0        0     4099 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/model_based/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.797623 giefstat-0.0.5/giefstat/estimate/other/
--rw-rw-rw-   0        0        0      289 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/other/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/other/coefficient.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.811586 giefstat-0.0.5/giefstat/estimate/quant_based/
--rw-rw-rw-   0        0        0      281 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/__init__.py
--rw-rw-rw-   0        0        0     7282 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/_quant_darbellay.py
--rw-rw-rw-   0        0        0     2111 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/mi_classic.py
--rw-rw-rw-   0        0        0     1700 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/quant_based/mi_darbellay.py
--rw-rw-rw-   0        0        0       90 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/setting.py
--rw-rw-rw-   0        0        0     3447 2023-04-27 12:50:49.000000 giefstat-0.0.5/giefstat/estimate/util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.840510 giefstat-0.0.5/giefstat/statistical_tools/
--rw-rw-rw-   0        0        0      498 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/__init__.py
--rw-rw-rw-   0        0        0     3142 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/surrog_indep_test.py
--rw-rw-rw-   0        0        0     2692 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/time_delayed_association.py
--rw-rw-rw-   0        0        0     1068 2023-06-05 14:19:01.000000 giefstat-0.0.5/giefstat/statistical_tools/util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 15:34:18.747757 giefstat-0.0.5/giefstat.egg-info/
--rw-rw-rw-   0        0        0     3561 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1394 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 15:34:18.000000 giefstat-0.0.5/giefstat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 15:34:18.843501 giefstat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-06-05 15:34:12.000000 giefstat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.907204 giefstat-0.0.6/
+-rw-rw-rw-   0        0        0     4384 2023-06-06 07:13:43.906207 giefstat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-06 07:11:47.000000 giefstat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.832405 giefstat-0.0.6/giefstat/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.6/giefstat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.844373 giefstat-0.0.6/giefstat/estimate/
+-rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.6/giefstat/estimate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.850356 giefstat-0.0.6/giefstat/estimate/correlation_coeff/
+-rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.6/giefstat/estimate/correlation_coeff/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.6/giefstat/estimate/correlation_coeff/coefficient.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.852350 giefstat-0.0.6/giefstat/estimate/gief/
+-rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.6/giefstat/estimate/gief/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.857337 giefstat-0.0.6/giefstat/estimate/gief/entropy/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/gief/entropy/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/gief/entropy/cond_entropy.py
+-rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.6/giefstat/estimate/gief/entropy/marg_entropy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.868309 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_kraskov.py
+-rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_ross.py
+-rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/cmi.py
+-rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/mi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.872297 giefstat-0.0.6/giefstat/estimate/kde/
+-rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/kde/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.6/giefstat/estimate/kde/kde.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.879279 giefstat-0.0.6/giefstat/estimate/mic/
+-rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.6/giefstat/estimate/mic/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/mic/_mic_rmic.py
+-rw-rw-rw-   0        0        0     2550 2023-06-06 06:52:23.000000 giefstat-0.0.6/giefstat/estimate/mic/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.885263 giefstat-0.0.6/giefstat/estimate/model_based/
+-rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.6/giefstat/estimate/model_based/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.6/giefstat/estimate/model_based/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.895237 giefstat-0.0.6/giefstat/estimate/quant_based/
+-rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.6/giefstat/estimate/quant_based/__init__.py
+-rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.6/giefstat/estimate/quant_based/_quant_darbellay.py
+-rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.6/giefstat/estimate/quant_based/mi_classic.py
+-rw-rw-rw-   0        0        0     1569 2023-06-06 06:59:21.000000 giefstat-0.0.6/giefstat/estimate/quant_based/mi_darbellay.py
+-rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.6/giefstat/setting.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.903216 giefstat-0.0.6/giefstat/statistical_tools/
+-rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.6/giefstat/statistical_tools/__init__.py
+-rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/statistical_tools/surrog_indep_test.py
+-rw-rw-rw-   0        0        0     2693 2023-06-06 07:05:47.000000 giefstat-0.0.6/giefstat/statistical_tools/time_delayed_association.py
+-rw-rw-rw-   0        0        0     9737 2023-06-06 07:08:36.000000 giefstat-0.0.6/giefstat/util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.842378 giefstat-0.0.6/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     4384 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1327 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:13:43.907204 giefstat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      886 2023-06-06 07:12:16.000000 giefstat-0.0.6/setup.py
```

### Comparing `giefstat-0.0.5/PKG-INFO` & `giefstat-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,8 @@
-Metadata-Version: 2.1
-Name: giefstat
-Version: 0.0.5
-Summary: Package for information estimation, independence test, etc.
-Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
-Author: Dreisteine
-Author-email: dreisteine@163.com
-License: MIT
-Keywords: python,information estimation
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-
-### general-information-estimation-framework
-
-### TODOs
-
-1. ~~script/独立性检验/statistical_power_test.py~~
-2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
-3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+### general-information-estimation-framework (GIEF)
 
 ### Project Purpose
 
 This project aims for:
 1. computing higher-order information interactions between different types (discrete & continuous) of variables
 2. uncovering complex associations and causal relationships in high-dimensional data
 
@@ -97,7 +79,13 @@
 
 1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
 2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
 3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
 4. https://github.com/dizcza/entropy-estimators
 5. https://github.com/danielhomola/mifs
 
+### TODOs
+
+1. ~~script/独立性检验/statistical_power_test.py~~
+2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
+3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+4. 继续estimate中mic及剩下的部分的封装测试
```

### Comparing `giefstat-0.0.5/README.md` & `giefstat-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,104 @@
-### general-information-estimation-framework
-
-### TODOs
-
-1. ~~script/独立性检验/statistical_power_test.py~~
-2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
-3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
-
-### Project Purpose
-
-This project aims for:
-1. computing higher-order information interactions between different types (discrete & continuous) of variables
-2. uncovering complex associations and causal relationships in high-dimensional data
-
-### Project Structure
-
-```
-|-- general-information-estimation-framework
-    |-- estimate            # information estimation base on KNN, KDE, etc.
-        |-- __init__.py     
-        |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
-        |-- util.py
-        |-- _univar_encoding.py     # encoding one-dimensional variable data
-        |-- gief            # general information estimation
-            __init__.py
-            |-- entropy     # marginal and conditional entropies
-                |-- __init__.py
-                |-- cond_entropy.py
-                |-- marg_entropy.py
-            |-- mutual_info
-                |-- __init__.py
-                |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
-                |-- _ross.py    # proposed by Ross
-                |-- mi.py       # mutual information estimation
-                |-- cmi.py      # conditional mutual information estimation
-
-    |-- statistical_tools
-        |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
-        |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
-        |-- time_delayed_association.py         # time delayed association detection
-
-    |-- script
-        |-- 独立性检验
-            |-- indep_test.py               # independence test
-            |-- statistical_power_test.py   # statistical power test
-        |-- 条件独立性检验
-            |-- cond_indep_test.py          # conditional independence test
-        |-- 时延关联检测
-
-```
-
-file dependency plot：
-
-```mermaid
-flowchart LR
-
-subgraph estimate
-    subgraph gief
-        H-G & MI-G & CMI-G
-    end
-
-    subgraph kde
-        MI-KDE
-    end
-
-    subgraph other
-        coefficient --> PearsonCorr & SpearmanCorr & DistCorr
-    end
-
-    subgraph quant_based
-        MI-Classic --> MI-cut & MI-qcut
-        MI-Darbellay
-    end
-end
-
-subgraph statistical_tools
-    cal_general_assoc --> surrog_indep_test
-    surrog_indep_test --> time_delayed_assocication
-end
-
-estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
-```
-
-### References
-
-1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
-2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
-3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
-4. https://github.com/dizcza/entropy-estimators
-5. https://github.com/danielhomola/mifs
-
+Metadata-Version: 2.1
+Name: giefstat
+Version: 0.0.6
+Summary: Package for information estimation, independence test, etc.
+Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
+Author: Dreisteine
+Author-email: dreisteine@163.com
+License: MIT
+Description: ### general-information-estimation-framework (GIEF)
+        
+        ### Project Purpose
+        
+        This project aims for:
+        1. computing higher-order information interactions between different types (discrete & continuous) of variables
+        2. uncovering complex associations and causal relationships in high-dimensional data
+        
+        ### Project Structure
+        
+        ```
+        |-- general-information-estimation-framework
+            |-- estimate            # information estimation base on KNN, KDE, etc.
+                |-- __init__.py     
+                |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
+                |-- util.py
+                |-- _univar_encoding.py     # encoding one-dimensional variable data
+                |-- gief            # general information estimation
+                    __init__.py
+                    |-- entropy     # marginal and conditional entropies
+                        |-- __init__.py
+                        |-- cond_entropy.py
+                        |-- marg_entropy.py
+                    |-- mutual_info
+                        |-- __init__.py
+                        |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
+                        |-- _ross.py    # proposed by Ross
+                        |-- mi.py       # mutual information estimation
+                        |-- cmi.py      # conditional mutual information estimation
+        
+            |-- statistical_tools
+                |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
+                |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
+                |-- time_delayed_association.py         # time delayed association detection
+        
+            |-- script
+                |-- 独立性检验
+                    |-- indep_test.py               # independence test
+                    |-- statistical_power_test.py   # statistical power test
+                |-- 条件独立性检验
+                    |-- cond_indep_test.py          # conditional independence test
+                |-- 时延关联检测
+        
+        ```
+        
+        file dependency plot：
+        
+        ```mermaid
+        flowchart LR
+        
+        subgraph estimate
+            subgraph gief
+                H-G & MI-G & CMI-G
+            end
+        
+            subgraph kde
+                MI-KDE
+            end
+        
+            subgraph other
+                coefficient --> PearsonCorr & SpearmanCorr & DistCorr
+            end
+        
+            subgraph quant_based
+                MI-Classic --> MI-cut & MI-qcut
+                MI-Darbellay
+            end
+        end
+        
+        subgraph statistical_tools
+            cal_general_assoc --> surrog_indep_test
+            surrog_indep_test --> time_delayed_assocication
+        end
+        
+        estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
+        ```
+        
+        ### References
+        
+        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+        4. https://github.com/dizcza/entropy-estimators
+        5. https://github.com/danielhomola/mifs
+        
+        ### TODOs
+        
+        1. ~~script/独立性检验/statistical_power_test.py~~
+        2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
+        3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+        4. 继续estimate中mic及剩下的部分的封装测试
+        
+Keywords: python,information estimation
+Platform: UNKNOWN
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
```

### Comparing `giefstat-0.0.5/giefstat/estimate/__init__.py` & `giefstat-0.0.6/giefstat/estimate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 1))
-sys.path.insert(0, BASE_DIR)
+from ..setting import DTYPES
 
-from gief import MutualInfoGIEF, CondMutualInfoGIEF, MargEntropy, CondEntropy
-from kde import MutualInfoKDE
-from mic import MIC, CMIC
-from model_based import MutualInfoModel, CondMutualInfoModel
-from quant_based import MutualInfoClassic, MutualInfoDarbellay
-from other import cal_dist_corr, cal_pearson_corr, cal_spearman_corr
+from .gief import MutualInfoGIEF, CondMutualInfoGIEF, MargEntropy, CondEntropy
+from .kde import MutualInfoKDE
+from .mic import MIC, CMIC
+from .model_based import MutualInfoModel, CondMutualInfoModel
+from .quant_based import MutualInfoClassic, MutualInfoDarbellay
+from .correlation_coeff import cal_dist_corr, cal_pearson_corr, cal_spearman_corr
 
-DTYPES = ["d", "c"]
 ASSOC_METHODS = [
     "PearsonCorr", "SpearmanCorr", "DistCorr",
     "MI-GIEF", "MI-model", "MI-cut", "MI-qcut", "MI-Darbellay", "MI-KDE",
     "MIC", "RMIC"
 ]
 COND_ASSOC_METHODS = [
     "CMI-GIEF", "CMI-model", "CMI-cut", "CMI-qcut",
```

### Comparing `giefstat-0.0.5/giefstat/estimate/gief/entropy/cond_entropy.py` & `giefstat-0.0.6/giefstat/estimate/gief/entropy/cond_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.5/giefstat/estimate/gief/entropy/marg_entropy.py` & `giefstat-0.0.6/giefstat/estimate/gief/entropy/marg_entropy.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,40 +28,34 @@
     3. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator, 2015.
     4. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets, 2014.
 """
 
 from scipy.special import psi
 from numpy import log
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 4))
-sys.path.insert(0, BASE_DIR)
-
-from estimate.setting import DTYPES, BASE
-from estimate.util import stdize_values, build_tree, query_neighbors_dist, get_unit_ball_volume
+from ....util import stdize_values, build_tree, query_neighbors_dist, get_unit_ball_volume
+from ....setting import DTYPES, BASE
 
 
 def _cal_discrete_entropy(x):
     _, counts = np.unique(x, return_counts=True, axis=0)
     proba = counts.astype(float) / len(x)
     proba = proba[proba > 0.0]
     return np.sum(proba * np.log(1. / proba))
 
 
 def _cal_kl_entropy(x, k, metric="chebyshev"):
     assert k <= len(x) - 1
     N, D = x.shape
     
-    # 构建距离树.
+    # 构建距离树
     tree = build_tree(x, "chebyshev")
 
-    # 计算结果.
-    # 参见Kraskov, et al. Estimating Mutual Information, 2004. Eq. (20).
+    # 计算结果
     nn_distc = query_neighbors_dist(tree, x, k)  # 获得了各样本第k近邻的距离
     v = get_unit_ball_volume(D, metric)
     return (-psi(k) + psi(N) + np.log(v) + D * np.log(nn_distc).mean())
     
 
 class MargEntropy(object):
     """计算任意连续和离散变量的信息熵"""
```

### Comparing `giefstat-0.0.5/giefstat/estimate/gief/mutual_info/_kraskov.py` & `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_kraskov.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 @Author: luolei
 
 @Email: dreisteine262@163.com
 
 @Describe: 使用Kraskov方法计算互信息
 """
 
-import warnings
-
-import numpy as np
+from sklearn.neighbors import BallTree, KDTree
+from scipy.special import digamma
 import numpy.linalg as la
 from numpy import log
-from scipy.special import digamma
-from sklearn.neighbors import BallTree, KDTree
+import numpy as np
+import warnings
 
 __doc__ = """
     （补充文献）
 """
 
 
 def entropy(x, k=3, base=2):
```

### Comparing `giefstat-0.0.5/giefstat/estimate/gief/mutual_info/_ross.py` & `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_ross.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from scipy.special import psi
-import numpy as np
 from numpy import log
-import sys
-import os
-
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 3))
-sys.path.insert(0, BASE_DIR)
+import numpy as np
 
-# from mod.data_process.numpy import compress_z_data
-from util import build_tree, query_neighbors_dist
+from ....util import build_tree, query_neighbors_dist
 
 
 # ---- 高维数据压缩, 计算互信息时要用. ----------------------------------------------------------------
 
 def _reorder_z_series(z_compress: np.ndarray):
     z_compress = z_compress.copy()
     map_ = dict(zip(set(z_compress), list(range(len(set(z_compress))))))
```

### Comparing `giefstat-0.0.5/giefstat/estimate/gief/mutual_info/cmi.py` & `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/cmi.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,21 @@
 
 @Email: dreisteine262@163.com
 
 @Describe: 条件互信息
 """
 
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 3))
-sys.path.insert(0, BASE_DIR)
-
-from estimate.setting import DTYPES, BASE
-from estimate.util import stdize_values
-from ._kraskov import kraskov_mi as cal_kraskov_cmi
-from .mi import MutualInfoGIEF
+from ....util import stdize_values
+from ....setting import DTYPES, BASE
 from ..entropy.cond_entropy import CondEntropy
 from ..entropy.marg_entropy import MargEntropy
+from ._kraskov import kraskov_mi as cal_kraskov_cmi
+from .mi import MutualInfoGIEF
 
 
 class CondMutualInfoGIEF(object):
     """条件互信息"""
     
     def __init__(self, x: np.ndarray, xtype: str, y: np.ndarray, ytype: str, z: np.ndarray, ztype: str):
         assert xtype in DTYPES
```

### Comparing `giefstat-0.0.5/giefstat/estimate/gief/mutual_info/mi.py` & `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/mi.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,20 @@
 @Email: dreisteine262@163.com
 
 @Describe: 互信息
 """
 
 from numpy import log
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 4))
-sys.path.insert(0, BASE_DIR)
-
-from estimate.setting import DTYPES, BASE
-from estimate.util import stdize_values
+from ....util import stdize_values
+from ....setting import DTYPES, BASE
+from ..entropy.marg_entropy import MargEntropy
 from ._kraskov import kraskov_mi as cal_kraskov_mi
 from ._ross import cal_ross_mi
-from ..entropy.marg_entropy import MargEntropy
 
 
 def _cal_mi_cc(x, y, k):
     return cal_kraskov_mi(x, y, k=k, base=BASE, alpha=0)
     
     
 def _cal_mi_cd(x, y, k, metric="chebyshev", base=BASE):
```

### Comparing `giefstat-0.0.5/giefstat/estimate/mic/_mic_rmic.py` & `giefstat-0.0.6/giefstat/estimate/mic/_mic_rmic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.5/giefstat/estimate/mic/mi_cmi.py` & `giefstat-0.0.6/giefstat/estimate/mic/mi_cmi.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,17 @@
 
 @Email: dreisteine262@163.com
 
 @Describe: MIC和RMIC
 """
 
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 2))
-sys.path.insert(0, BASE_DIR)
-
-from _mic_rmic import MaximalInfoCoeff, RefinedMaximalInfoCoeff
-from _univar_encoding import SuperCategorEncoding
-from util import discretize_arr
+from ...util import SuperCategorEncoding, discretize_arr
+from ._mic_rmic import MaximalInfoCoeff, RefinedMaximalInfoCoeff
 
 
 # ---- 数据压缩编码 ---------------------------------------------------------------------------------
 
 def _transf_labels2char(s: np.ndarray):
     """哎, numpy直接匹配函数没找到, 只能暂时转成字符串来处理了"""
     return "".join(f"-{int(p)}" for p in s)
@@ -56,26 +50,20 @@
         self.x = x.copy().reshape(len(x), -1)
         self.y = y.copy().reshape(len(y), -1)
     
     def __call__(self, method="rmic", encode=True):
         # 多维数组逐列离散化, 并合并编码压缩为一维数组
         # todo 优化此处离散化编码处理, 能否确定y顺序?
         y = _reencode(self.y) if self.y.shape[1] > 1 else self.y.copy()
-        
-        if self.x.shape[1] > 1:
-            x = _reencode(self.x)
-        else:
-            x = self.x.copy()
-            
-        if method == "rmic":
-            if encode:
-                x = SuperCategorEncoding(x, y).encode(method="mhg") # 进行有监督编码, NOTE x值需为int
-            return RefinedMaximalInfoCoeff(x, y).cal_assoc()
-        else:
+        x = _reencode(self.x) if self.x.shape[1] > 1 else self.x.copy()
+        if method != "rmic":
             return MaximalInfoCoeff(x, y).cal_assoc()
+        if encode:
+            x = SuperCategorEncoding(x, y).encode(method="mhg") # 进行有监督编码, NOTE x值需为int
+        return RefinedMaximalInfoCoeff(x, y).cal_assoc()
             
             
 class CMIC(object):
     """条件最大信息系数"""
     
     def __init__(self, x, y, z):
         self.x = x
```

### Comparing `giefstat-0.0.5/giefstat/estimate/model_based/mi_cmi.py` & `giefstat-0.0.6/giefstat/estimate/model_based/mi_cmi.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,17 @@
     I(x;Y) = Accu(y, model.predict(x))
     I(x;Y|Z) = I(Y; xZ) - I(Y; Z)
              = Accu(y, model.predict(xz)) - Accu(y, model.predict(z))
 """
 
 from sklearn.metrics import f1_score as cal_f1, r2_score as cal_r2
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 3))
-sys.path.insert(0, BASE_DIR)
-
-from estimate.setting import DTYPES
-from estimate.util import stdize_values
+from ...setting import DTYPES
+from ...util import stdize_values
 
 
 def _cal_metric(y_true, y_pred, ytype):
     if ytype == "d":
         return cal_f1(y_true, y_pred, average="micro")  # note 使用微平均
     else:
         return cal_r2(y_true, y_pred)
@@ -92,47 +87,47 @@
         self.ztype = ztype
         
     def __call__(self, model, test_ratio=0.3):
         return _exec_model_test(
             self.x_norm, self.y_norm.flatten(), self.ytype, model, test_ratio, self.z_norm)
         
 
-if __name__ == "__main__":
-    def test_mi():
-        x = np.random.normal(0, 1, 10000)
-        y = np.random.randint(0, 5, 10000)
-        
-        self = MutualInfoModel(x, "c", y, "d")
-    
-        from lightgbm import LGBMClassifier as LightGBM
-        model = LightGBM(
-            n_estimators=100,
-            max_depth=3,
-            boosting_type="goss",
-            learning_rate=0.1,
-            importance_type="split",
-            n_jobs=3,
-        )
-    
-        print(f"mi = {self(model)}")
-    
-    def test_cmi():
-        x = np.random.normal(0, 1, 10000)
-        y = np.random.normal(0, 1, 10000)
-        z = np.random.normal(0, 1, 10000)
-        
-        self = CondMutualInfoModel(x, "c", y, "c", z, "c")
-
-        from lightgbm import LGBMRegressor as LightGBM
-        model = LightGBM(
-            n_estimators=100,
-            max_depth=3,
-            boosting_type="goss",
-            learning_rate=0.1,
-            importance_type="split",
-            n_jobs=3,
-        )
+# if __name__ == "__main__":
+#     def test_mi():
+#         x = np.random.normal(0, 1, 10000)
+#         y = np.random.randint(0, 5, 10000)
+        
+#         self = MutualInfoModel(x, "c", y, "d")
+    
+#         from lightgbm import LGBMClassifier as LightGBM
+#         model = LightGBM(
+#             n_estimators=100,
+#             max_depth=3,
+#             boosting_type="goss",
+#             learning_rate=0.1,
+#             importance_type="split",
+#             n_jobs=3,
+#         )
+    
+#         print(f"mi = {self(model)}")
+    
+#     def test_cmi():
+#         x = np.random.normal(0, 1, 10000)
+#         y = np.random.normal(0, 1, 10000)
+#         z = np.random.normal(0, 1, 10000)
+        
+#         self = CondMutualInfoModel(x, "c", y, "c", z, "c")
+
+#         from lightgbm import LGBMRegressor as LightGBM
+#         model = LightGBM(
+#             n_estimators=100,
+#             max_depth=3,
+#             boosting_type="goss",
+#             learning_rate=0.1,
+#             importance_type="split",
+#             n_jobs=3,
+#         )
 
-        print(f"cmi = {self(model)}")
+#         print(f"cmi = {self(model)}")
         
-    test_mi()  # todo 分类问题算得关联值下限不为0
-    test_cmi()
+#     test_mi()  # todo 分类问题算得关联值下限不为0
+#     test_cmi()
```

### Comparing `giefstat-0.0.5/giefstat/estimate/quant_based/_quant_darbellay.py` & `giefstat-0.0.6/giefstat/estimate/quant_based/_quant_darbellay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-# import matplotlib.pyplot as plt
 from typing import List
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 2))
-sys.path.insert(0, BASE_DIR)
+from ...util import stdize_values
 
 if "plt" not in dir():
     import matplotlib.pyplot as plt
     
-from util import stdize_values
 
 
 def cal_area(bounds: List[tuple], D) -> float:
     """计算面积"""
     area = 1.0
     for i in range(D):
         bd = bounds[i]
@@ -110,21 +105,20 @@
         x_thres, y_thres = self.part_thres
         cell_ul.def_cell_bounds_cal_area([(xl, x_thres), (y_thres, yu)])
         cell_ur.def_cell_bounds_cal_area([(x_thres, xu), (y_thres, yu)])
         cell_ll.def_cell_bounds_cal_area([(xl, x_thres), (yl, y_thres)])
         cell_lr.def_cell_bounds_cal_area([(x_thres, xu), (yl, y_thres)])
         return cell_ul, cell_ur, cell_ll, cell_lr
     
-    def show(self, N_total: int, pdf_ub: float=1e4, linewidth: float = 0.5):
+    def show(self, linewidth: float = 0.5):
         (xl, xu), (yl, yu) = self.bounds
-        # plt.fill_between([xl, xu], [yl, yl], [yu, yu], alpha=self.cal_proba_dens(N_total) / pdf_ub, facecolor="grey")
-        plt.plot([xl, xu], [yl, yl], '-', c='k', linewidth=linewidth)
-        plt.plot([xu, xu], [yl, yu], '-', c='k', linewidth=linewidth)
-        plt.plot([xu, xl], [yu, yu], '-', c='k', linewidth=linewidth)
-        plt.plot([xl, xl], [yu, yl], '-', c='k', linewidth=linewidth)
+        plt.plot([xl, xu], [yl, yl], "-", c="k", linewidth=linewidth)
+        plt.plot([xu, xu], [yl, yu], "-", c="k", linewidth=linewidth)
+        plt.plot([xu, xl], [yu, yu], "-", c="k", linewidth=linewidth)
+        plt.plot([xl, xl], [yu, yl], "-", c="k", linewidth=linewidth)
         
 
 # 递归离散化.
 def _try_partition(cell: Cell, p_eps: float, N_total: int):
     """尝试对Cell进行一次分裂, 若样本数少于规定阈值或概率密度收敛, 则返回为四个空cell, 否则正常分裂"""
     # 尝试分裂一下, 并检查分裂效果.
     proba_dens = cell.cal_proba_dens(N_total)
```

### Comparing `giefstat-0.0.5/giefstat/estimate/quant_based/mi_classic.py` & `giefstat-0.0.6/giefstat/estimate/quant_based/mi_classic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from pyitlib import discrete_random_variable as drv
 import pandas as pd
 import numpy as np
-import sys
-import os
 
-BASE_DIR = os.path.abspath(os.path.join(os.path.abspath(__file__), "../" * 2))
-sys.path.insert(0, BASE_DIR)
-
-from util import stdize_values
+from ...util import stdize_values
 
 
 def discretize_series(x: np.ndarray, n: int = None, method="qcut"):
     """对数据序列采用等频分箱"""
     n = len(x) // 15 if n is None else n
     q = int(len(x) // n)
 
@@ -40,22 +35,22 @@
             return float(mi)
         
         z_enc = discretize_series(self.z_norm, method=method).astype(int)
         cmi = drv.information_mutual_conditional(x_enc, y_enc, z_enc)
         return float(cmi)  # NOTE: drv.infor_mutual_cond居然返回array格式
     
 
-if __name__ == "__main__":
+# if __name__ == "__main__":
     
-    def test_cc():
-        x = np.random.normal(0, 1, 100000)
-        y = np.random.normal(0, 1, 100000)
-        print(f"mi = {MutualInfoClassic(x, y)()}")
+#     def test_cc():
+#         x = np.random.normal(0, 1, 100000)
+#         y = np.random.normal(0, 1, 100000)
+#         print(f"mi = {MutualInfoClassic(x, y)()}")
         
-    def test_ccc():
-        x = np.random.normal(0, 1, 100000)
-        y = np.random.normal(0, 1, 100000)
-        z = np.random.normal(0, 1, 100000)
-        print(f"cmi = {MutualInfoClassic(x, y, z)()}")
+#     def test_ccc():
+#         x = np.random.normal(0, 1, 100000)
+#         y = np.random.normal(0, 1, 100000)
+#         z = np.random.normal(0, 1, 100000)
+#         print(f"cmi = {MutualInfoClassic(x, y, z)()}")
         
-    test_cc()
-    test_ccc()
+#     test_cc()
+#     test_ccc()
```

### Comparing `giefstat-0.0.5/giefstat/statistical_tools/surrog_indep_test.py` & `giefstat-0.0.6/giefstat/statistical_tools/surrog_indep_test.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.5/giefstat/statistical_tools/time_delayed_association.py` & `giefstat-0.0.6/giefstat/statistical_tools/time_delayed_association.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @Describe: 时延关联检测
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 import logging
 
-from .util import build_td_series
+from ..util import build_td_series
 from .surrog_indep_test import exec_surrog_indep_test
 
 
 def detect_time_delayed_assoc(x, y, taus, xtype="c", ytype="c", max_size_bt=1000, method="MI-GIEF", 
                               show=False, **kwargs):
     """双变量间的时延关联检测
```

### Comparing `giefstat-0.0.5/giefstat.egg-info/PKG-INFO` & `giefstat-0.0.6/giefstat.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
+Description: ### general-information-estimation-framework (GIEF)
+        
+        ### Project Purpose
+        
+        This project aims for:
+        1. computing higher-order information interactions between different types (discrete & continuous) of variables
+        2. uncovering complex associations and causal relationships in high-dimensional data
+        
+        ### Project Structure
+        
+        ```
+        |-- general-information-estimation-framework
+            |-- estimate            # information estimation base on KNN, KDE, etc.
+                |-- __init__.py     
+                |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
+                |-- util.py
+                |-- _univar_encoding.py     # encoding one-dimensional variable data
+                |-- gief            # general information estimation
+                    __init__.py
+                    |-- entropy     # marginal and conditional entropies
+                        |-- __init__.py
+                        |-- cond_entropy.py
+                        |-- marg_entropy.py
+                    |-- mutual_info
+                        |-- __init__.py
+                        |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
+                        |-- _ross.py    # proposed by Ross
+                        |-- mi.py       # mutual information estimation
+                        |-- cmi.py      # conditional mutual information estimation
+        
+            |-- statistical_tools
+                |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
+                |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
+                |-- time_delayed_association.py         # time delayed association detection
+        
+            |-- script
+                |-- 独立性检验
+                    |-- indep_test.py               # independence test
+                    |-- statistical_power_test.py   # statistical power test
+                |-- 条件独立性检验
+                    |-- cond_indep_test.py          # conditional independence test
+                |-- 时延关联检测
+        
+        ```
+        
+        file dependency plot：
+        
+        ```mermaid
+        flowchart LR
+        
+        subgraph estimate
+            subgraph gief
+                H-G & MI-G & CMI-G
+            end
+        
+            subgraph kde
+                MI-KDE
+            end
+        
+            subgraph other
+                coefficient --> PearsonCorr & SpearmanCorr & DistCorr
+            end
+        
+            subgraph quant_based
+                MI-Classic --> MI-cut & MI-qcut
+                MI-Darbellay
+            end
+        end
+        
+        subgraph statistical_tools
+            cal_general_assoc --> surrog_indep_test
+            surrog_indep_test --> time_delayed_assocication
+        end
+        
+        estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
+        ```
+        
+        ### References
+        
+        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+        4. https://github.com/dizcza/entropy-estimators
+        5. https://github.com/danielhomola/mifs
+        
+        ### TODOs
+        
+        1. ~~script/独立性检验/statistical_power_test.py~~
+        2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
+        3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+        4. 继续estimate中mic及剩下的部分的封装测试
+        
 Keywords: python,information estimation
+Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-
-### general-information-estimation-framework
-
-### TODOs
-
-1. ~~script/独立性检验/statistical_power_test.py~~
-2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
-3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
-
-### Project Purpose
-
-This project aims for:
-1. computing higher-order information interactions between different types (discrete & continuous) of variables
-2. uncovering complex associations and causal relationships in high-dimensional data
-
-### Project Structure
-
-```
-|-- general-information-estimation-framework
-    |-- estimate            # information estimation base on KNN, KDE, etc.
-        |-- __init__.py     
-        |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
-        |-- util.py
-        |-- _univar_encoding.py     # encoding one-dimensional variable data
-        |-- gief            # general information estimation
-            __init__.py
-            |-- entropy     # marginal and conditional entropies
-                |-- __init__.py
-                |-- cond_entropy.py
-                |-- marg_entropy.py
-            |-- mutual_info
-                |-- __init__.py
-                |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
-                |-- _ross.py    # proposed by Ross
-                |-- mi.py       # mutual information estimation
-                |-- cmi.py      # conditional mutual information estimation
-
-    |-- statistical_tools
-        |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
-        |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
-        |-- time_delayed_association.py         # time delayed association detection
-
-    |-- script
-        |-- 独立性检验
-            |-- indep_test.py               # independence test
-            |-- statistical_power_test.py   # statistical power test
-        |-- 条件独立性检验
-            |-- cond_indep_test.py          # conditional independence test
-        |-- 时延关联检测
-
-```
-
-file dependency plot：
-
-```mermaid
-flowchart LR
-
-subgraph estimate
-    subgraph gief
-        H-G & MI-G & CMI-G
-    end
-
-    subgraph kde
-        MI-KDE
-    end
-
-    subgraph other
-        coefficient --> PearsonCorr & SpearmanCorr & DistCorr
-    end
-
-    subgraph quant_based
-        MI-Classic --> MI-cut & MI-qcut
-        MI-Darbellay
-    end
-end
-
-subgraph statistical_tools
-    cal_general_assoc --> surrog_indep_test
-    surrog_indep_test --> time_delayed_assocication
-end
-
-estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
-```
-
-### References
-
-1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
-2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
-3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
-4. https://github.com/dizcza/entropy-estimators
-5. https://github.com/danielhomola/mifs
-
```

### Comparing `giefstat-0.0.5/giefstat.egg-info/SOURCES.txt` & `giefstat-0.0.6/giefstat.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 README.md
 setup.py
 giefstat/__init__.py
+giefstat/setting.py
+giefstat/util.py
 giefstat.egg-info/PKG-INFO
 giefstat.egg-info/SOURCES.txt
 giefstat.egg-info/dependency_links.txt
 giefstat.egg-info/requires.txt
 giefstat.egg-info/top_level.txt
 giefstat/estimate/__init__.py
-giefstat/estimate/_univar_encoding.py
-giefstat/estimate/setting.py
-giefstat/estimate/util.py
+giefstat/estimate/correlation_coeff/__init__.py
+giefstat/estimate/correlation_coeff/coefficient.py
 giefstat/estimate/gief/__init__.py
 giefstat/estimate/gief/entropy/__init__.py
 giefstat/estimate/gief/entropy/cond_entropy.py
 giefstat/estimate/gief/entropy/marg_entropy.py
 giefstat/estimate/gief/mutual_info/__init__.py
 giefstat/estimate/gief/mutual_info/_kraskov.py
 giefstat/estimate/gief/mutual_info/_ross.py
@@ -22,17 +23,14 @@
 giefstat/estimate/kde/__init__.py
 giefstat/estimate/kde/kde.py
 giefstat/estimate/mic/__init__.py
 giefstat/estimate/mic/_mic_rmic.py
 giefstat/estimate/mic/mi_cmi.py
 giefstat/estimate/model_based/__init__.py
 giefstat/estimate/model_based/mi_cmi.py
-giefstat/estimate/other/__init__.py
-giefstat/estimate/other/coefficient.py
 giefstat/estimate/quant_based/__init__.py
 giefstat/estimate/quant_based/_quant_darbellay.py
 giefstat/estimate/quant_based/mi_classic.py
 giefstat/estimate/quant_based/mi_darbellay.py
 giefstat/statistical_tools/__init__.py
 giefstat/statistical_tools/surrog_indep_test.py
-giefstat/statistical_tools/time_delayed_association.py
-giefstat/statistical_tools/util.py
+giefstat/statistical_tools/time_delayed_association.py
```

### Comparing `giefstat-0.0.5/setup.py` & `giefstat-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 from pathlib import Path
-import os
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
     author="Dreisteine",
     author_email="dreisteine@163.com",
     description=DESCRIPTION,
-    packages=find_packages(include=["giefstat", "giefstat.*"]),
+    packages=find_packages(include=["giefstat", "giefstat.*"]),  # NOTE: 注意giefstat.*的写法
     install_requires=["scikit-learn==0.24.0", "minepy==1.2.6"],
     keywords=["python", "information estimation"],
     python_requires=">=3.8.0",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ulti-Dreisteine/general-information-estimation-framework",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

