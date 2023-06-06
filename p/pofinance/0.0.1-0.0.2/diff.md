# Comparing `tmp/pofinance-0.0.1.tar.gz` & `tmp/pofinance-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pofinance-0.0.1.tar", last modified: Fri Jun  2 15:41:57 2023, max compression
+gzip compressed data, was "pofinance-0.0.2.tar", last modified: Tue Jun  6 12:46:22 2023, max compression
```

## Comparing `pofinance-0.0.1.tar` & `pofinance-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:57.024754 pofinance-0.0.1/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofinance-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5336 2023-06-02 15:41:57.024754 pofinance-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4791 2023-06-02 15:35:27.000000 pofinance-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:56.966902 pofinance-0.0.1/pofinance/
--rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 pofinance-0.0.1/pofinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:57.000031 pofinance-0.0.1/pofinance/api/
--rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 pofinance-0.0.1/pofinance/api/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-06-02 15:41:48.000000 pofinance-0.0.1/pofinance/api/shares.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:57.009553 pofinance-0.0.1/pofinance/core/
--rw-rw-rw-   0        0        0     8970 2023-06-02 15:33:35.000000 pofinance-0.0.1/pofinance/core/PDFType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.1/pofinance/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:57.011552 pofinance-0.0.1/pofinance/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.1/pofinance/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:57.016746 pofinance-0.0.1/pofinance/lib/pdf/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofinance-0.0.1/pofinance/lib/pdf/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 pofinance-0.0.1/pofinance/lib/pdf/add_watermark_service.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:56.992517 pofinance-0.0.1/pofinance.egg-info/
--rw-rw-rw-   0        0        0     5336 2023-06-02 15:41:56.000000 pofinance-0.0.1/pofinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-06-02 15:41:56.000000 pofinance-0.0.1/pofinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 15:41:56.000000 pofinance-0.0.1/pofinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 15:37:07.000000 pofinance-0.0.1/pofinance.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-02 15:41:56.000000 pofinance-0.0.1/pofinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      708 2023-06-02 15:41:57.033856 pofinance-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofinance-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:41:57.022758 pofinance-0.0.1/tests/
--rw-rw-rw-   0        0        0      185 2023-06-02 15:33:35.000000 pofinance-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2104 2023-06-02 15:36:41.000000 pofinance-0.0.1/tests/test_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.289601 pofinance-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofinance-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4115 2023-06-06 12:46:22.289601 pofinance-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3570 2023-06-04 03:26:57.000000 pofinance-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.262300 pofinance-0.0.2/pofinance/
+-rw-rw-rw-   0        0        0       36 2023-06-02 15:40:09.000000 pofinance-0.0.2/pofinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.276075 pofinance-0.0.2/pofinance/api/
+-rw-rw-rw-   0        0        0        0 2023-06-02 15:40:09.000000 pofinance-0.0.2/pofinance/api/__init__.py
+-rw-rw-rw-   0        0        0     4598 2023-06-05 15:28:12.000000 pofinance-0.0.2/pofinance/api/shares.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.281084 pofinance-0.0.2/pofinance/core/
+-rw-rw-rw-   0        0        0     8970 2023-06-02 15:33:35.000000 pofinance-0.0.2/pofinance/core/PDFType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.2/pofinance/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.283085 pofinance-0.0.2/pofinance/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofinance-0.0.2/pofinance/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.286687 pofinance-0.0.2/pofinance/lib/pdf/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofinance-0.0.2/pofinance/lib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-24 15:13:04.000000 pofinance-0.0.2/pofinance/lib/pdf/add_watermark_service.py
+drwxrwxrwx   0        0        0        0 2023-06-06 12:46:22.271565 pofinance-0.0.2/pofinance.egg-info/
+-rw-rw-rw-   0        0        0     4115 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 15:37:07.000000 pofinance-0.0.2/pofinance.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-06 12:46:22.000000 pofinance-0.0.2/pofinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2023-06-06 12:46:22.291606 pofinance-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofinance-0.0.2/setup.py
```

### Comparing `pofinance-0.0.1/LICENSE` & `pofinance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.1/README.md` & `pofinance-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pofinance
+Version: 0.0.2
+Summary: pip install pofinance
+Home-page: https://www.python-office.com/
+Author: CoderWanFeng
+Author-email: 1957875073@qq.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofinance/issues
+Project-URL: Documentation, https://github.com/CoderWanFeng/pofinance/blob/master/README.md
+Project-URL: Source Code, https://github.com/CoderWanFeng/pofinance
+Platform: any
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 <p align="center">
 	👉 <a target="_blank" href="https://www.python-office.com/">项目官网：https://www.python-office.com/</a> 👈
 </p>
 <p align="center">
 	👉 <a target="_blank" href="https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office.jpg">本开源项目的交流群</a> 👈
 </p>
@@ -10,15 +26,15 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📚简介
 
 
-pofinance是python自动化办公的PDF的代码合集。
+pofinance是python + 炒股的功能合集，1行代码就能使用。
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
@@ -29,44 +45,40 @@
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
 [📘官网：https://www.python-office.com/](https://www.python-office.com/)
 
-| 序号 | 功能名称       | 代码地址 |
-| ---- | -------------- | -------- |
-| 1    | [合同和财务系统](https://mp.weixin.qq.com/s/7Cx9f1Re9tbJVajtNVmsVA) | [源码](https://github.com/CoderWanFeng/awesome-python-framework/tree/project/1%E3%80%81%E5%90%88%E5%90%8C%E7%B3%BB%E7%BB%9F)     |
-| 2    | [人脸门禁系统](https://mp.weixin.qq.com/s/98X3nl-elyi7MYsU_uCeqA) | [源码](https://github.com/CoderWanFeng/awesome-python-framework/tree/project/2%E3%80%81Python%2BDjango%E5%AE%9E%E7%8E%B0%E5%9F%BA%E4%BA%8E%E4%BA%BA%E8%84%B8%E8%AF%86%E5%88%AB%E7%9A%84%E9%97%A8%E7%A6%81%E7%AE%A1%E7%90%86%E7%B3%BB%E7%BB%9F%E3%80%90%E6%BA%90%E7%A0%81%E3%80%91)     |
-| 3    | [商场管理系统](https://mp.weixin.qq.com/s/0FR4o2ddPe-9C2ijlnTuAg) | [源码](https://github.com/CoderWanFeng/awesome-python-framework/tree/project/3、用Python实现一个商场管理系统(附源码))     |
-| 4    | [报表自动化 + 邮件自动发送](https://mp.weixin.qq.com/s/RfG502Hez7UttfHMndc4eA) | [源码](https://github.com/CoderWanFeng/awesome-python-framework/tree/project/4%E3%80%81Python%E8%87%AA%E5%8A%A8%E5%8C%96%E5%8A%9E%E5%85%AC%E5%B0%8F%E7%A8%8B%E5%BA%8F%EF%BC%9A%E5%AE%9E%E7%8E%B0%E6%8A%A5%E8%A1%A8%E8%87%AA%E5%8A%A8%E5%8C%96%E5%92%8C%E8%87%AA%E5%8A%A8%E5%8F%91%E9%80%81%E5%88%B0%E7%9B%AE%E7%9A%84%E9%82%AE%E7%AE%B1)     |
-| 5    | 爬取招聘网站 | [源码](https://github.com/CoderWanFeng/awesome-python-framework/tree/project/5、Python招聘岗位信息聚合系统（拥有爬虫爬取、数据分析、可视化、互动等功能）)     |
+| 序号 | 功能名称                                                            | 代码地址 |
+| ---- |-----------------------------------------------------------------| -------- |
+| 1    | [做T](https://mp.weixin.qq.com/s/6keTzBI8CWnUbuXCaYhkMQ)             | [源码](https://cloud.tencent.com/developer/article/2293964)     |
 
 
 
 
 ## 🏗️添砖加瓦
 
 
 ### 📐PR的建议
 
-python-office欢迎任何人来添砖加瓦，贡献代码，建议提交的pr（pull request）符合一些规范，规范如下：
+pofinance 欢迎任何人来添砖加瓦，贡献代码，建议提交的pr（pull request）符合一些规范，规范如下：
 
 参与项目建设的步骤：
-- 例如：你需要给python-office添加一个add方法。
+- 例如：你需要给 pofinance 添加一个add方法。
    1. 你的Github账户名为：demo
    2. 于是你在./contributors新建了文件夹./demo
    3. 新建了add.py文件，编辑你的代码
    4. 编辑完成，提交pr到master分支（gitee或者GitHub，都可以）。可以注明你对自己功能的取名建议
    5. 晚枫收到后，会对各位的代码进行测试后，合并后打包上传到python官方库
 
 ### 📐代码规范
 
 1. 注释完备，尤其每个新增的方法应按照Google Python文档规范标明方法说明、参数说明、返回值说明等信息，必要时请添加单元测试，如果愿意，也可以加上你的大名。
-2. python-office的文档，需要进行格式化。注意：只能格式化你自己的代码
+2. pofinance 的文档，需要进行格式化。注意：只能格式化你自己的代码
 3. 请直接pull request到`master`分支。`master`是主分支，表示已经发布pypi库的版本。**未来参与人数增多，会开辟新的分支，请留意本文档的更新。**
 4. 我们如果关闭了你的issue或pr，请不要诧异，这是我们保持问题处理整洁的一种方式，你依旧可以继续讨论，当有讨论结果时我们会重新打开。
 
 
 ### 🧬贡献代码的步骤
 
 1. 在Gitee或者Github上fork项目到自己的repo
@@ -89,8 +101,8 @@
 ## 📌联系作者
 
 
 ![CoderWanFeng](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
 
 
 ## 📕参考资料
-- https://pypi.org/project/pyfinance/
+- https://pypi.org/project/pyfinance/
```

### Comparing `pofinance-0.0.1/pofinance/core/PDFType.py` & `pofinance-0.0.2/pofinance/core/PDFType.py`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.1/pofinance/lib/pdf/add_watermark_service.py` & `pofinance-0.0.2/pofinance/lib/pdf/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `pofinance-0.0.1/setup.cfg` & `pofinance-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f66 696e 616e 6365 0d0a 7665   = pofinance..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 310d 0a64  rsion = 0.0.1..d
+00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a64  rsion = 0.0.2..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2070 6970  escription = pip
 00000040: 2069 6e73 7461 6c6c 2070 6f66 696e 616e   install pofinan
 00000050: 6365 0d0a 6c6f 6e67 5f64 6573 6372 6970  ce..long_descrip
 00000060: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000070: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000080: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 00000090: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
```

