# Comparing `tmp/docrobot-1.0.4.tar.gz` & `tmp/docrobot-1.0.5.tar.gz`

## Comparing `docrobot-1.0.4.tar` & `docrobot-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.4/convert.ps1
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 docrobot-1.0.4/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/form.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/form.ui
--rw-r--r--   0        0        0    19111 2020-02-02 00:00:00.000000 docrobot-1.0.4/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 docrobot-1.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.4/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.4/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.5/convert.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.5/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/form.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/form.ui
+-rw-r--r--   0        0        0    19125 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.5/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.5/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.5/PKG-INFO
```

### Comparing `docrobot-1.0.4/.github/workflows/python-publish.yml` & `docrobot-1.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.4/src/docrobot/form.py` & `docrobot-1.0.5/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.4/src/docrobot/form.ui` & `docrobot-1.0.5/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.4/src/docrobot/guimain.pyw` & `docrobot-1.0.5/src/docrobot/guimain.pyw`

 * *Files 2% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         if doc.tables[0].rows[3].cells[0].paragraphs[0].text == '项目周期：':
             doc.tables[0].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_start + '至' + prj.p_end
             self.clear_runs(doc.tables[0].rows[3].cells[1].paragraphs[0].runs)
             match = match + 1
         return match
 
     def start_time(self, doc, prj):
-        match = self.check_replace(doc.paragraphs, '申请立项时间：\d{4}[-/]\d{1,2}[-/]\d{1,2}',
+        match = self.check_replace(doc.paragraphs, '申请立项时间：\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
                                    '申请立项时间：' + prj.p_start)
         return match
 
     def second_table(self, doc, prj):
         match = 0
         if doc.tables[1].rows[0].cells[0].paragraphs[0].text == '项目立项名称':
             doc.tables[1].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
@@ -361,28 +361,28 @@
             match = match + 1
 
         match = match + self.check_replace(doc.tables[1].rows[1].cells[1].paragraphs
                                            , '项目团队由(.*)人组成，项目实施周期为(.*)个月。'
                                            ,
                                            '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
         match = match + self.check_replace(doc.tables[1].rows[6].cells[1].paragraphs
-                                           , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}',
+                                           , '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
                                            prj.p_start + '至' + prj.p_end)
         match = match + self.check_replace(doc.tables[1].rows[7].cells[1].paragraphs
                                            , '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
 
         match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs
                                            , '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
         if prj.p_owner != 'None':
             match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
                                                '项目负责人：' + prj.p_owner)
         if prj.p_rnd != 'None':
             match = match + self.check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*',
                                                '研发成员：' + prj.p_rnd)
-        match = match + self.check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{4}[-/]\d{1,2}[-/]\d{1,2}',
+        match = match + self.check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
                                            prj.p_start)
 
         return match
 
     def check_replace(self, paras, regex, dst):
         match = 0
         for i, para in enumerate(paras):
@@ -397,20 +397,20 @@
                 break  # 只替换一次就够用
         return match
 
     def third_table(self, doc, prj):
         match = 0
         if doc.tables[2].rows[0].cells[0].paragraphs[0].text == '项目名称':
             doc.tables[2].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
-            self.clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
+            self.clear_runs(doc.tables[2].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
         match = match + self.check_replace(doc.tables[2].rows[1].cells[1].paragraphs
-                                           , '\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
+                                           , '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
         match = match + self.check_replace(doc.tables[2].rows[2].cells[1].paragraphs
-                                           , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}',
+                                           , '\d{2,4}[-/]\d{1,2}[-/]\d{1,2}至\d{2,4}[-/]\d{1,2}[-/]\d{1,2}',
                                            prj.p_start + '至' + prj.p_end)
 
         if prj.p_owner != 'None':
             doc.tables[2].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_owner
             self.clear_runs(doc.tables[2].rows[3].cells[1].paragraphs[0].runs)
             match = match + 1
         return match
```

### Comparing `docrobot-1.0.4/LICENSE` & `docrobot-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.4/pyproject.toml` & `docrobot-1.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.4/PKG-INFO` & `docrobot-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

