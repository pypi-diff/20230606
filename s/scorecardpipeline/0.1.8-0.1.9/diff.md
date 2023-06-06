# Comparing `tmp/scorecardpipeline-0.1.8.tar.gz` & `tmp/scorecardpipeline-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecardpipeline-0.1.8.tar", last modified: Wed May 24 14:47:25 2023, max compression
+gzip compressed data, was "scorecardpipeline-0.1.9.tar", last modified: Tue Jun  6 13:30:18 2023, max compression
```

## Comparing `scorecardpipeline-0.1.8.tar` & `scorecardpipeline-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 14:47:25.596210 scorecardpipeline-0.1.8/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.8/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)    34236 2023-05-24 14:47:25.595893 scorecardpipeline-0.1.8/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)    33354 2023-05-24 14:46:24.000000 scorecardpipeline-0.1.8/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 14:47:25.593841 scorecardpipeline-0.1.8/scorecardpipeline/
--rw-r--r--   0 lubberit   (501) staff       (20)     1093 2023-05-24 14:47:15.000000 scorecardpipeline-0.1.8/scorecardpipeline/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    20449 2023-05-24 14:31:49.000000 scorecardpipeline-0.1.8/scorecardpipeline/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)     1502 2023-05-23 14:15:12.000000 scorecardpipeline-0.1.8/scorecardpipeline/logger.py
--rw-r--r--   0 lubberit   (501) staff       (20)    19807 2023-05-24 13:37:13.000000 scorecardpipeline-0.1.8/scorecardpipeline/model.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21542 2023-05-23 15:37:48.000000 scorecardpipeline-0.1.8/scorecardpipeline/processing.py
--rw-r--r--   0 lubberit   (501) staff       (20)    29990 2023-05-24 09:30:40.000000 scorecardpipeline-0.1.8/scorecardpipeline/utils.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 14:47:25.595409 scorecardpipeline-0.1.8/scorecardpipeline.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)    34236 2023-05-24 14:47:25.000000 scorecardpipeline-0.1.8/scorecardpipeline.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      408 2023-05-24 14:47:25.000000 scorecardpipeline-0.1.8/scorecardpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-24 14:47:25.000000 scorecardpipeline-0.1.8/scorecardpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-05-24 14:47:25.000000 scorecardpipeline-0.1.8/scorecardpipeline.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-24 14:47:25.000000 scorecardpipeline-0.1.8/scorecardpipeline.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-24 14:47:25.596298 scorecardpipeline-0.1.8/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.8/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-06-06 13:30:18.994588 scorecardpipeline-0.1.9/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.9/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)       81 2023-06-06 13:29:05.000000 scorecardpipeline-0.1.9/MANIFEST.in
+-rw-r--r--   0 lubberit   (501) staff       (20)    34236 2023-06-06 13:30:18.994241 scorecardpipeline-0.1.9/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    33354 2023-05-24 14:46:24.000000 scorecardpipeline-0.1.9/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-06-06 13:30:18.992049 scorecardpipeline-0.1.9/scorecardpipeline/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1248 2023-06-06 13:24:34.000000 scorecardpipeline-0.1.9/scorecardpipeline/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    20449 2023-05-24 14:31:49.000000 scorecardpipeline-0.1.9/scorecardpipeline/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)   268042 2023-05-23 14:17:23.000000 scorecardpipeline-0.1.9/scorecardpipeline/germancredit.csv
+-rw-r--r--   0 lubberit   (501) staff       (20)     1502 2023-05-23 14:15:12.000000 scorecardpipeline-0.1.9/scorecardpipeline/logger.py
+-rw-r--r--   0 lubberit   (501) staff       (20)  4168588 2023-05-17 15:54:03.000000 scorecardpipeline-0.1.9/scorecardpipeline/matplot_chinese.ttf
+-rw-r--r--   0 lubberit   (501) staff       (20)    19807 2023-05-25 08:00:46.000000 scorecardpipeline-0.1.9/scorecardpipeline/model.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21542 2023-05-23 15:37:48.000000 scorecardpipeline-0.1.9/scorecardpipeline/processing.py
+-rw-r--r--   0 lubberit   (501) staff       (20)     8418 2023-04-10 09:37:07.000000 scorecardpipeline-0.1.9/scorecardpipeline/template.xlsx
+-rw-r--r--   0 lubberit   (501) staff       (20)    30060 2023-05-25 08:00:24.000000 scorecardpipeline-0.1.9/scorecardpipeline/utils.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-06-06 13:30:18.993746 scorecardpipeline-0.1.9/scorecardpipeline.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    34236 2023-06-06 13:30:18.000000 scorecardpipeline-0.1.9/scorecardpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      525 2023-06-06 13:30:18.000000 scorecardpipeline-0.1.9/scorecardpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-06-06 13:30:18.000000 scorecardpipeline-0.1.9/scorecardpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-06-06 13:30:18.000000 scorecardpipeline-0.1.9/scorecardpipeline.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-06-06 13:30:18.000000 scorecardpipeline-0.1.9/scorecardpipeline.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-06-06 13:30:18.994677 scorecardpipeline-0.1.9/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.9/setup.py
```

### Comparing `scorecardpipeline-0.1.8/LICENSE` & `scorecardpipeline-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.8/PKG-INFO` & `scorecardpipeline-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.8
+Version: 0.1.9
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scorecardpipeline-0.1.8/README.md` & `scorecardpipeline-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.8/scorecardpipeline/excel_writer.py` & `scorecardpipeline-0.1.9/scorecardpipeline/excel_writer.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.8/scorecardpipeline/logger.py` & `scorecardpipeline-0.1.9/scorecardpipeline/logger.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.8/scorecardpipeline/model.py` & `scorecardpipeline-0.1.9/scorecardpipeline/model.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.8/scorecardpipeline/processing.py` & `scorecardpipeline-0.1.9/scorecardpipeline/processing.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.8/scorecardpipeline/utils.py` & `scorecardpipeline-0.1.9/scorecardpipeline/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,35 +405,36 @@
                 os.makedirs(os.path.dirname(save), exist_ok=True)
                 
             plt.savefig(save, dpi=240, format="png", bbox_inches="tight")
 
         return fig
 
 
-def hist_plot(score, y_true, figsize=(15, 10), bins=30, save=None, labels=["坏样本", "好样本"], anchor=1.1, fontsize=14, **kwargs):
+def hist_plot(score, y_true=None, figsize=(15, 10), bins=30, save=None, labels=["坏样本", "好样本"], anchor=1.1, fontsize=14, **kwargs):
     fig, ax = plt.subplots(1, 1, figsize = figsize)
     palette = sns.diverging_palette(340, 267, n=2, s=100, l=40)
 
     sns.histplot(
-                x=score, hue=y_true.replace({i: v for i, v in enumerate(labels)}), element="step", stat="probability", bins=bins, common_bins=True, common_norm=True, palette=palette, ax=ax, **kwargs
+                x=score, hue=y_true.replace({i: v for i, v in enumerate(labels)}) if y_true is not None else y_true, element="step", stat="probability", bins=bins, common_bins=True, common_norm=True, palette=palette, ax=ax, **kwargs
             )
 
     sns.despine()
     
     ax.spines['top'].set_color("#2639E9")
     ax.spines['bottom'].set_color("#2639E9")
     ax.spines['right'].set_color("#2639E9")
     ax.spines['left'].set_color("#2639E9")
 
     ax.set_xlabel("评分分布", fontsize=fontsize)
     ax.set_ylabel("样本占比", fontsize=fontsize)
     
     ax.yaxis.set_major_formatter(PercentFormatter(1))
     
-    ax.legend(labels[:y_true.nunique()], loc='upper center', ncol=y_true.nunique(), bbox_to_anchor=(0.5, anchor), frameon=False, fontsize=fontsize)
+    if y_true is not None:
+        ax.legend(labels[:y_true.nunique()], loc='upper center', ncol=y_true.nunique(), bbox_to_anchor=(0.5, anchor), frameon=False, fontsize=fontsize)
     
     fig.tight_layout()
 
     if save:
         if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
             os.makedirs(os.path.dirname(save), exist_ok=True)
         
@@ -449,15 +450,15 @@
     df_psi[f"{labels[1]}% - {labels[0]}%"] = df_psi[f"{labels[1]}样本占比"] - df_psi[f"{labels[0]}样本占比"]
     df_psi[f"ln({labels[1]}% / {labels[0]}%)"] = np.log(df_psi[f"{labels[1]}样本占比"] / df_psi[f"{labels[0]}样本占比"])
     df_psi["分档PSI值"] = (df_psi[f"{labels[1]}% - {labels[0]}%"] * df_psi[f"ln({labels[1]}% / {labels[0]}%)"])
     df_psi = df_psi.fillna(0).replace(np.inf, 0).replace(-np.inf, 0)
     df_psi["总体PSI值"] = df_psi["分档PSI值"].sum()
     
     if plot:
-        x = df_psi['分箱'].apply(lambda l: l if max_len is None else str(l)[:max_len] + "...")
+        x = df_psi['分箱'].apply(lambda l: l if max_len is None else f"{str(l)[:max_len]}...")
         x_indexes = np.arange(len(x))
         fig, ax1 = plt.subplots(figsize=figsize)
 
         ax1.bar(x_indexes - width / 2, df_psi[f'{labels[0]}样本占比'], width, label=f'{labels[0]}样本占比', color=colors[0], hatch="/")
         ax1.bar(x_indexes + width / 2, df_psi[f'{labels[1]}样本占比'], width, label=f'{labels[1]}样本占比', color=colors[1], hatch="\\")
 
         ax1.set_ylabel('样本占比: 分箱内样本数 / 样本总数')
@@ -499,15 +500,15 @@
     df_csi[f"{labels[1]}% - {labels[0]}%"] = df_csi[f"{labels[1]}样本占比"] - df_csi[f"{labels[0]}样本占比"]
     df_csi = df_csi.merge(pd.DataFrame({"分箱": feature_bins(score_bins["bins"]).values(), "对应分数": score_bins["scores"]}), on="分箱", how="left").replace(np.nan, 0)
     df_csi["分档CSI值"] = (df_csi[f"{labels[1]}% - {labels[0]}%"] * df_csi["对应分数"])
     df_csi = df_csi.fillna(0).replace(np.inf, 0).replace(-np.inf, 0)
     df_csi["总体CSI值"] = df_csi["分档CSI值"].sum()
     
     if plot:
-        x = df_csi['分箱'].apply(lambda l: l if max_len is None else str(l)[:max_len] + "...")
+        x = df_csi['分箱'].apply(lambda l: l if max_len is None else f"{str(l)[:max_len]}...")
         x_indexes = np.arange(len(x))
         fig, ax1 = plt.subplots(figsize=figsize)
 
         ax1.bar(x_indexes - width / 2, df_csi[f'{labels[0]}样本占比'], width, label=f'{labels[0]}样本占比', color=colors[0], hatch="/")
         ax1.bar(x_indexes + width / 2, df_csi[f'{labels[1]}样本占比'], width, label=f'{labels[1]}样本占比', color=colors[1], hatch="\\")
 
         ax1.set_ylabel('样本占比: 分箱内样本数 / 样本总数')
```

### Comparing `scorecardpipeline-0.1.8/scorecardpipeline.egg-info/PKG-INFO` & `scorecardpipeline-0.1.9/scorecardpipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.8
+Version: 0.1.9
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `scorecardpipeline-0.1.8/setup.py` & `scorecardpipeline-0.1.9/setup.py`

 * *Files identical despite different names*

