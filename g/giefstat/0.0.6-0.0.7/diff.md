# Comparing `tmp/giefstat-0.0.6.tar.gz` & `tmp/giefstat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.6.tar", last modified: Tue Jun  6 07:13:43 2023, max compression
+gzip compressed data, was "giefstat-0.0.7.tar", last modified: Tue Jun  6 07:48:00 2023, max compression
```

## Comparing `giefstat-0.0.6.tar` & `giefstat-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.907204 giefstat-0.0.6/
--rw-rw-rw-   0        0        0     4384 2023-06-06 07:13:43.906207 giefstat-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-06 07:11:47.000000 giefstat-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.832405 giefstat-0.0.6/giefstat/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.6/giefstat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.844373 giefstat-0.0.6/giefstat/estimate/
--rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.6/giefstat/estimate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.850356 giefstat-0.0.6/giefstat/estimate/correlation_coeff/
--rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.6/giefstat/estimate/correlation_coeff/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.6/giefstat/estimate/correlation_coeff/coefficient.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.852350 giefstat-0.0.6/giefstat/estimate/gief/
--rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.6/giefstat/estimate/gief/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.857337 giefstat-0.0.6/giefstat/estimate/gief/entropy/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/gief/entropy/__init__.py
--rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/gief/entropy/cond_entropy.py
--rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.6/giefstat/estimate/gief/entropy/marg_entropy.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.868309 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_kraskov.py
--rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_ross.py
--rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/cmi.py
--rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.6/giefstat/estimate/gief/mutual_info/mi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.872297 giefstat-0.0.6/giefstat/estimate/kde/
--rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/kde/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.6/giefstat/estimate/kde/kde.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.879279 giefstat-0.0.6/giefstat/estimate/mic/
--rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.6/giefstat/estimate/mic/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/estimate/mic/_mic_rmic.py
--rw-rw-rw-   0        0        0     2550 2023-06-06 06:52:23.000000 giefstat-0.0.6/giefstat/estimate/mic/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.885263 giefstat-0.0.6/giefstat/estimate/model_based/
--rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.6/giefstat/estimate/model_based/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.6/giefstat/estimate/model_based/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.895237 giefstat-0.0.6/giefstat/estimate/quant_based/
--rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.6/giefstat/estimate/quant_based/__init__.py
--rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.6/giefstat/estimate/quant_based/_quant_darbellay.py
--rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.6/giefstat/estimate/quant_based/mi_classic.py
--rw-rw-rw-   0        0        0     1569 2023-06-06 06:59:21.000000 giefstat-0.0.6/giefstat/estimate/quant_based/mi_darbellay.py
--rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.6/giefstat/setting.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.903216 giefstat-0.0.6/giefstat/statistical_tools/
--rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.6/giefstat/statistical_tools/__init__.py
--rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.6/giefstat/statistical_tools/surrog_indep_test.py
--rw-rw-rw-   0        0        0     2693 2023-06-06 07:05:47.000000 giefstat-0.0.6/giefstat/statistical_tools/time_delayed_association.py
--rw-rw-rw-   0        0        0     9737 2023-06-06 07:08:36.000000 giefstat-0.0.6/giefstat/util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:13:43.842378 giefstat-0.0.6/giefstat.egg-info/
--rw-rw-rw-   0        0        0     4384 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1327 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 07:13:43.000000 giefstat-0.0.6/giefstat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 07:13:43.907204 giefstat-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-06-06 07:12:16.000000 giefstat-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.843257 giefstat-0.0.7/
+-rw-rw-rw-   0        0        0     5790 2023-06-06 07:48:00.841260 giefstat-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4391 2023-06-06 07:47:09.000000 giefstat-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.766462 giefstat-0.0.7/giefstat/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.7/giefstat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.780423 giefstat-0.0.7/giefstat/estimate/
+-rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.7/giefstat/estimate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.783415 giefstat-0.0.7/giefstat/estimate/correlation_coeff/
+-rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.7/giefstat/estimate/correlation_coeff/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.7/giefstat/estimate/correlation_coeff/coefficient.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.787406 giefstat-0.0.7/giefstat/estimate/gief/
+-rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.7/giefstat/estimate/gief/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.793389 giefstat-0.0.7/giefstat/estimate/gief/entropy/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/gief/entropy/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/gief/entropy/cond_entropy.py
+-rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.7/giefstat/estimate/gief/entropy/marg_entropy.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.802366 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_kraskov.py
+-rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_ross.py
+-rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/cmi.py
+-rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/mi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.809346 giefstat-0.0.7/giefstat/estimate/kde/
+-rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/kde/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.7/giefstat/estimate/kde/kde.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.819320 giefstat-0.0.7/giefstat/estimate/mic/
+-rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.7/giefstat/estimate/mic/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/mic/_mic_rmic.py
+-rw-rw-rw-   0        0        0     2550 2023-06-06 06:52:23.000000 giefstat-0.0.7/giefstat/estimate/mic/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.825304 giefstat-0.0.7/giefstat/estimate/model_based/
+-rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.7/giefstat/estimate/model_based/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.7/giefstat/estimate/model_based/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.832285 giefstat-0.0.7/giefstat/estimate/quant_based/
+-rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.7/giefstat/estimate/quant_based/__init__.py
+-rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.7/giefstat/estimate/quant_based/_quant_darbellay.py
+-rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.7/giefstat/estimate/quant_based/mi_classic.py
+-rw-rw-rw-   0        0        0     1569 2023-06-06 06:59:21.000000 giefstat-0.0.7/giefstat/estimate/quant_based/mi_darbellay.py
+-rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.7/giefstat/setting.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.839266 giefstat-0.0.7/giefstat/statistical_tools/
+-rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.7/giefstat/statistical_tools/__init__.py
+-rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/statistical_tools/surrog_indep_test.py
+-rw-rw-rw-   0        0        0     2693 2023-06-06 07:05:47.000000 giefstat-0.0.7/giefstat/statistical_tools/time_delayed_association.py
+-rw-rw-rw-   0        0        0     9737 2023-06-06 07:08:36.000000 giefstat-0.0.7/giefstat/util.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.778428 giefstat-0.0.7/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     5790 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1327 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:48:00.843257 giefstat-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      886 2023-06-06 07:47:31.000000 giefstat-0.0.7/setup.py
```

### Comparing `giefstat-0.0.6/PKG-INFO` & `giefstat-0.0.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,122 @@
-Metadata-Version: 2.1
-Name: giefstat
-Version: 0.0.6
-Summary: Package for information estimation, independence test, etc.
-Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
-Author: Dreisteine
-Author-email: dreisteine@163.com
-License: MIT
-Description: ### general-information-estimation-framework (GIEF)
-        
-        ### Project Purpose
-        
-        This project aims for:
-        1. computing higher-order information interactions between different types (discrete & continuous) of variables
-        2. uncovering complex associations and causal relationships in high-dimensional data
-        
-        ### Project Structure
-        
-        ```
-        |-- general-information-estimation-framework
-            |-- estimate            # information estimation base on KNN, KDE, etc.
-                |-- __init__.py     
-                |-- setting.py      # NOTE var types: "d" for discrete and "c" for continuous
-                |-- util.py
-                |-- _univar_encoding.py     # encoding one-dimensional variable data
-                |-- gief            # general information estimation
-                    __init__.py
-                    |-- entropy     # marginal and conditional entropies
-                        |-- __init__.py
-                        |-- cond_entropy.py
-                        |-- marg_entropy.py
-                    |-- mutual_info
-                        |-- __init__.py
-                        |-- _kraskov.py # KNN estimation proposed by Kraskov et al.
-                        |-- _ross.py    # proposed by Ross
-                        |-- mi.py       # mutual information estimation
-                        |-- cmi.py      # conditional mutual information estimation
-        
-            |-- statistical_tools
-                |-- (deprecated) bootstrap_coeff.py     # association measure based on bootstrap test
-                |-- surrog_indep_test.py                # association measure and independence test based on surrogate data
-                |-- time_delayed_association.py         # time delayed association detection
-        
-            |-- script
-                |-- 独立性检验
-                    |-- indep_test.py               # independence test
-                    |-- statistical_power_test.py   # statistical power test
-                |-- 条件独立性检验
-                    |-- cond_indep_test.py          # conditional independence test
-                |-- 时延关联检测
-        
-        ```
-        
-        file dependency plot：
-        
-        ```mermaid
-        flowchart LR
-        
-        subgraph estimate
-            subgraph gief
-                H-G & MI-G & CMI-G
-            end
-        
-            subgraph kde
-                MI-KDE
-            end
-        
-            subgraph other
-                coefficient --> PearsonCorr & SpearmanCorr & DistCorr
-            end
-        
-            subgraph quant_based
-                MI-Classic --> MI-cut & MI-qcut
-                MI-Darbellay
-            end
-        end
-        
-        subgraph statistical_tools
-            cal_general_assoc --> surrog_indep_test
-            surrog_indep_test --> time_delayed_assocication
-        end
-        
-        estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
-        ```
-        
-        ### References
-        
-        1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
-        2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
-        3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
-        4. https://github.com/dizcza/entropy-estimators
-        5. https://github.com/danielhomola/mifs
-        
-        ### TODOs
-        
-        1. ~~script/独立性检验/statistical_power_test.py~~
-        2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
-        3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
-        4. 继续estimate中mic及剩下的部分的封装测试
-        
-Keywords: python,information estimation
-Platform: UNKNOWN
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
+### general-information-estimation-framework (GIEF)
+
+### Project Purpose
+
+This project aims for:
+1. computing higher-order information interactions between different types (discrete & continuous) of variables
+2. uncovering complex associations and causal relationships in high-dimensional data
+
+### Project Structure
+
+```
+    |-- giefstat
+    |   |-- __init__.py
+    |   |-- setting.py          # 项目设置
+    |   |-- util.py             # 通用工具
+    |   |
+    |   |-- estimate            # 基于KNN和KDE等方法的数据信息计算和关联估计方法
+    |   |   |-- __init__.py
+    |   |   |
+    |   |   |-- correlation_coeff   # 常见相关系数
+    |   |   |   |-- __init__.py
+    |   |   |   |-- coefficient.py
+    |   |   |
+    |   |   |-- gief            # 通用信息估计
+    |   |   |   |-- __init__.py
+    |   |   |   |-- entropy     # 信息熵
+    |   |   |   |   |-- __init__.py
+    |   |   |   |   |-- cond_entropy.py  # 条件熵估计
+    |   |   |   |   |-- marg_entropy.py  # 边际熵估计
+    |   |   |   |-- mutual_info
+    |   |   |       |-- __init__.py
+    |   |   |       |-- _kraskov.py # 由Kraskov等提出的K近邻互信息估计
+    |   |   |       |-- _ross.py    # 由Ross等提出的互信息估计
+    |   |   |       |-- mi.py       # 互信息估计
+    |   |   |       |-- cmi.py      # 条件互信息估计
+    |   |   |
+    |   |   |-- kde
+    |   |   |   |-- __init__.py
+    |   |   |   |-- kde.py  # 基于KDE的边际熵和互信息估计
+    |   |   |
+    |   |   |-- mic
+    |   |   |   |-- __init__.py
+    |   |   |   |-- _mic_rmic.py    # MIC和RMIC计算
+    |   |   |   |-- mi_cmi.py       # 基于MIC和RMIC的互信息和条件互信息估计
+    |   |   |   |-- rgsr.pickle     # RMIC中用于修正MIC下界的回归模型
+    |   |   |
+    |   |   |-- model_based
+    |   |   |   |-- __init__.py
+    |   |   |   |-- mi_cmi.py       # 基于机器学习预测模型的关联和条件关联系数估计
+    |   |   |
+    |   |   |-- quant_based
+    |   |       |-- __init__.py
+    |   |       |-- _quant_darbellay.py # Darbellay数据离散化方法
+    |   |       |-- mi_classic.py   # 基于经典等距和等频离散化的互信息估计
+    |   |       |-- mi_darbellay.py # 基于Darbellay离散化的互信息估计
+    |   |   
+    |   |-- statistical_tools
+    |       |-- __init__.py
+    |       |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
+    |       |-- time_delayed_association.py         # 时延关联检测
+    |
+    |-- script
+        |-- 独立性检验
+        |   |-- indep_test.py               # 独立性检验测试
+        |   |-- statistical_power_test.py   # 统计效能测试
+        |
+        |-- 条件独立性检验
+        |   |-- cond_indep_test.py          # 条件独立性检验测试
+        |
+        |-- 时延关联检测
+            |-- td_assoc_test.py            # 时延关联检测测试
+
+```
+
+file dependency plot：
+
+```mermaid
+flowchart LR
+
+subgraph estimate
+    subgraph gief
+        H-G & MI-G & CMI-G
+    end
+
+    subgraph kde
+        MI-KDE
+    end
+
+    subgraph other
+        coefficient --> PearsonCorr & SpearmanCorr & DistCorr
+    end
+
+    subgraph quant_based
+        MI-Classic --> MI-cut & MI-qcut
+        MI-Darbellay
+    end
+end
+
+subgraph statistical_tools
+    cal_general_assoc --> surrog_indep_test
+    surrog_indep_test --> time_delayed_assocication
+end
+
+estimate --cal_assoc & cal_cond_assoc--> cal_general_assoc
+```
+
+### References
+
+1. A. Kraskov, H. Stoegbauer, P. Grassberger: Estimating Mutual Information. Physical Review E, 2003.
+2. D. Lombardi, S. Pant: A Non-Parametric K-Nearest Neighbor Entropy Estimator. Physical Review E, 2015.
+3. B. C. Ross: Mutual Information between Discrete and Continuous Data Sets. PLoS One, 2014.
+4. https://github.com/dizcza/entropy-estimators
+5. https://github.com/danielhomola/mifs
+
+### TODOs
+
+1. ~~script/独立性检验/statistical_power_test.py~~
+2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
+3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
+4. ~~继续estimate中mic及剩下的部分的封装测试~~
+5. 一致性测试
+6. 时效性测试
```

### Comparing `giefstat-0.0.6/giefstat/estimate/__init__.py` & `giefstat-0.0.7/giefstat/estimate/__init__.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/correlation_coeff/coefficient.py` & `giefstat-0.0.7/giefstat/estimate/correlation_coeff/coefficient.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/gief/entropy/cond_entropy.py` & `giefstat-0.0.7/giefstat/estimate/gief/entropy/cond_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/gief/entropy/marg_entropy.py` & `giefstat-0.0.7/giefstat/estimate/gief/entropy/marg_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_kraskov.py` & `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_kraskov.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/_ross.py` & `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_ross.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/cmi.py` & `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/gief/mutual_info/mi.py` & `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/mi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/kde/kde.py` & `giefstat-0.0.7/giefstat/estimate/kde/kde.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/mic/_mic_rmic.py` & `giefstat-0.0.7/giefstat/estimate/mic/_mic_rmic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/mic/mi_cmi.py` & `giefstat-0.0.7/giefstat/estimate/mic/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/model_based/mi_cmi.py` & `giefstat-0.0.7/giefstat/estimate/model_based/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/quant_based/_quant_darbellay.py` & `giefstat-0.0.7/giefstat/estimate/quant_based/_quant_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/quant_based/mi_classic.py` & `giefstat-0.0.7/giefstat/estimate/quant_based/mi_classic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/estimate/quant_based/mi_darbellay.py` & `giefstat-0.0.7/giefstat/estimate/quant_based/mi_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/statistical_tools/surrog_indep_test.py` & `giefstat-0.0.7/giefstat/statistical_tools/surrog_indep_test.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/statistical_tools/time_delayed_association.py` & `giefstat-0.0.7/giefstat/statistical_tools/time_delayed_association.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat/util.py` & `giefstat-0.0.7/giefstat/util.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/giefstat.egg-info/SOURCES.txt` & `giefstat-0.0.7/giefstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.6/setup.py` & `giefstat-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
```

