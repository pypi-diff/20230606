# Comparing `tmp/pdtr-0.1.2.tar.gz` & `tmp/pdtr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdtr-0.1.2.tar", last modified: Thu May 18 16:22:12 2023, max compression
+gzip compressed data, was "pdtr-0.1.3.tar", last modified: Tue Jun  6 13:34:29 2023, max compression
```

## Comparing `pdtr-0.1.2.tar` & `pdtr-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-18 16:22:12.868715 pdtr-0.1.2/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-12 08:26:44.000000 pdtr-0.1.2/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)    10914 2023-05-18 16:22:12.868394 pdtr-0.1.2/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)    10188 2023-05-18 16:21:18.000000 pdtr-0.1.2/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-18 16:22:12.866539 pdtr-0.1.2/pdtr/
--rw-r--r--   0 lubberit   (501) staff       (20)      265 2023-05-18 16:21:51.000000 pdtr-0.1.2/pdtr/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21376 2023-05-17 15:26:47.000000 pdtr-0.1.2/pdtr/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)    30113 2023-05-18 16:05:17.000000 pdtr-0.1.2/pdtr/transforme.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-18 16:22:12.868034 pdtr-0.1.2/pdtr.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)    10914 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      222 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      204 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        5 2023-05-18 16:22:12.000000 pdtr-0.1.2/pdtr.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-18 16:22:12.868799 pdtr-0.1.2/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1632 2023-05-17 16:04:40.000000 pdtr-0.1.2/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-06-06 13:34:29.105387 pdtr-0.1.3/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-12 08:26:44.000000 pdtr-0.1.3/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)       31 2023-06-06 13:34:17.000000 pdtr-0.1.3/MANIFEST.in
+-rw-r--r--   0 lubberit   (501) staff       (20)    11284 2023-06-06 13:34:29.105060 pdtr-0.1.3/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    10558 2023-05-29 08:56:25.000000 pdtr-0.1.3/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-06-06 13:34:29.102482 pdtr-0.1.3/pdtr/
+-rw-r--r--   0 lubberit   (501) staff       (20)      265 2023-06-06 13:34:04.000000 pdtr-0.1.3/pdtr/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21537 2023-05-21 02:25:24.000000 pdtr-0.1.3/pdtr/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)  4168588 2023-05-17 15:54:03.000000 pdtr-0.1.3/pdtr/matplot_chinese.ttf
+-rw-r--r--   0 lubberit   (501) staff       (20)     8418 2023-04-10 09:37:07.000000 pdtr-0.1.3/pdtr/template.xlsx
+-rw-r--r--   0 lubberit   (501) staff       (20)    30113 2023-05-18 16:05:17.000000 pdtr-0.1.3/pdtr/transforme.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-06-06 13:34:29.104548 pdtr-0.1.3/pdtr.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    11284 2023-06-06 13:34:28.000000 pdtr-0.1.3/pdtr.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      278 2023-06-06 13:34:28.000000 pdtr-0.1.3/pdtr.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-06-06 13:34:28.000000 pdtr-0.1.3/pdtr.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      204 2023-06-06 13:34:28.000000 pdtr-0.1.3/pdtr.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        5 2023-06-06 13:34:28.000000 pdtr-0.1.3/pdtr.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-06-06 13:34:29.105492 pdtr-0.1.3/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1632 2023-05-17 16:04:40.000000 pdtr-0.1.3/setup.py
```

### Comparing `pdtr-0.1.2/LICENSE` & `pdtr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdtr-0.1.2/PKG-INFO` & `pdtr-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtr
-Version: 0.1.2
+Version: 0.1.3
 Summary: 自动决策树规则挖掘工具包
 Home-page: https://github.com/itlubber/pdtr
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -27,14 +27,22 @@
 > 
 > 博文地址：https://itlubber.art/archives/auto-strategy-mining
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/8s785MfmVznNgQyy38YnWw
 > 
 > pipy包：https://pypi.org/project/pdtr/
 
+## 交流
+
+|  微信 |  微信公众号 |
+| :---: | :----: |
+| <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/> | <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/> |
+|  itlubber  | itlubber_art |
+
+
 ## 背景简介
 
 金融场景风险大致可以概括为三种：系统性风险、欺诈风险（无还款意愿）、信用风险（无还款能力），而作为一名风控搬砖工，日常工作中有大量的数据挖掘工作，如何从高维数据集中挖掘出行之有效的规则、策略及模型来防范欺诈风险和信用风险每个搬砖工的基操。本仓库由笔者基于网上开源的一系列相关知识，结合实际工作中遇到的实际需求，整理得到。旨在为诸位仁兄提供一个便捷、高效、赏心悦目的决策树组合策略挖掘报告，及一系列能够实际运用到风险控制上的策略。
 
 ## 项目结构
 
 ```bash
@@ -192,14 +200,18 @@
 
 仅包含决策树策略挖掘相关工具
 
 + `0.1.1`
 
 除版本 `0.1.0` 中的决策树挖掘相关工具以外，新增了基于 `toad` 和 `optbinning` 的单变量策略挖掘相关方法
 
++ `0.1.2`
+
+在 `0.1.1` 的基础上增加了部分方法的文档注释
+
 
 ### 运行样例
 
 + 导入相关依赖
 
 ```python
 import os
```

### Comparing `pdtr-0.1.2/README.md` & `pdtr-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 > 
 > 博文地址：https://itlubber.art/archives/auto-strategy-mining
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/8s785MfmVznNgQyy38YnWw
 > 
 > pipy包：https://pypi.org/project/pdtr/
 
+## 交流
+
+|  微信 |  微信公众号 |
+| :---: | :----: |
+| <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/> | <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/> |
+|  itlubber  | itlubber_art |
+
+
 ## 背景简介
 
 金融场景风险大致可以概括为三种：系统性风险、欺诈风险（无还款意愿）、信用风险（无还款能力），而作为一名风控搬砖工，日常工作中有大量的数据挖掘工作，如何从高维数据集中挖掘出行之有效的规则、策略及模型来防范欺诈风险和信用风险每个搬砖工的基操。本仓库由笔者基于网上开源的一系列相关知识，结合实际工作中遇到的实际需求，整理得到。旨在为诸位仁兄提供一个便捷、高效、赏心悦目的决策树组合策略挖掘报告，及一系列能够实际运用到风险控制上的策略。
 
 ## 项目结构
 
 ```bash
@@ -171,14 +179,18 @@
 
 仅包含决策树策略挖掘相关工具
 
 + `0.1.1`
 
 除版本 `0.1.0` 中的决策树挖掘相关工具以外，新增了基于 `toad` 和 `optbinning` 的单变量策略挖掘相关方法
 
++ `0.1.2`
+
+在 `0.1.1` 的基础上增加了部分方法的文档注释
+
 
 ### 运行样例
 
 + 导入相关依赖
 
 ```python
 import os
```

### Comparing `pdtr-0.1.2/pdtr/excel_writer.py` & `pdtr-0.1.3/pdtr/excel_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,23 +358,28 @@
             header_style, header_left_style, header_middle_style, header_right_style,
             last_style, last_left_style, last_middle_style, last_right_style,
             content_style, left_style, middle_style, right_style,
             merge_style, merge_left_style, merge_middle_style, merge_right_style,
             first_style, first_left_style, first_middle_style, first_right_style
         ])
 
-    def save(self, filename):
+    def save(self, filename, close=True):
         """
         保存excel文件
 
         :param filename: 需要保存 excel 文件的路径
+        :param close: 是否需要释放 writer
         """
-        self.workbook.remove(self.style_sheet)
+        if self.style_sheet in self.workbook.sheetnames:
+            self.workbook.remove(self.style_sheet)
+        
         self.workbook.save(filename)
-        self.workbook.close()
+        
+        if close:
+            self.workbook.close()
 
 
 if __name__ == '__main__':
     writer = ExcelWriter()
     worksheet = writer.get_sheet_by_name("模型报告")
     writer.insert_value2sheet(worksheet, "B2", value="模型报告", style="header")
     writer.insert_value2sheet(worksheet, "B3", value="当前模型主要为评分卡模型", style="content", auto_width=True)
```

### Comparing `pdtr-0.1.2/pdtr/transforme.py` & `pdtr-0.1.3/pdtr/transforme.py`

 * *Files identical despite different names*

### Comparing `pdtr-0.1.2/pdtr.egg-info/PKG-INFO` & `pdtr-0.1.3/pdtr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtr
-Version: 0.1.2
+Version: 0.1.3
 Summary: 自动决策树规则挖掘工具包
 Home-page: https://github.com/itlubber/pdtr
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -27,14 +27,22 @@
 > 
 > 博文地址：https://itlubber.art/archives/auto-strategy-mining
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/8s785MfmVznNgQyy38YnWw
 > 
 > pipy包：https://pypi.org/project/pdtr/
 
+## 交流
+
+|  微信 |  微信公众号 |
+| :---: | :----: |
+| <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/> | <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/> |
+|  itlubber  | itlubber_art |
+
+
 ## 背景简介
 
 金融场景风险大致可以概括为三种：系统性风险、欺诈风险（无还款意愿）、信用风险（无还款能力），而作为一名风控搬砖工，日常工作中有大量的数据挖掘工作，如何从高维数据集中挖掘出行之有效的规则、策略及模型来防范欺诈风险和信用风险每个搬砖工的基操。本仓库由笔者基于网上开源的一系列相关知识，结合实际工作中遇到的实际需求，整理得到。旨在为诸位仁兄提供一个便捷、高效、赏心悦目的决策树组合策略挖掘报告，及一系列能够实际运用到风险控制上的策略。
 
 ## 项目结构
 
 ```bash
@@ -192,14 +200,18 @@
 
 仅包含决策树策略挖掘相关工具
 
 + `0.1.1`
 
 除版本 `0.1.0` 中的决策树挖掘相关工具以外，新增了基于 `toad` 和 `optbinning` 的单变量策略挖掘相关方法
 
++ `0.1.2`
+
+在 `0.1.1` 的基础上增加了部分方法的文档注释
+
 
 ### 运行样例
 
 + 导入相关依赖
 
 ```python
 import os
```

### Comparing `pdtr-0.1.2/setup.py` & `pdtr-0.1.3/setup.py`

 * *Files identical despite different names*

