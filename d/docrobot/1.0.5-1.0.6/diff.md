# Comparing `tmp/docrobot-1.0.5.tar.gz` & `tmp/docrobot-1.0.6.tar.gz`

## Comparing `docrobot-1.0.5.tar` & `docrobot-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.5/convert.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.5/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/form.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/form.ui
--rw-r--r--   0        0        0    19125 2020-02-02 00:00:00.000000 docrobot-1.0.5/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.5/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.5/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.6/convert.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.6/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/form.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/form.ui
+-rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 docrobot-1.0.6/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.6/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.6/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.6/PKG-INFO
```

### Comparing `docrobot-1.0.5/.github/workflows/python-publish.yml` & `docrobot-1.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.5/src/docrobot/form.py` & `docrobot-1.0.6/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.5/src/docrobot/form.ui` & `docrobot-1.0.6/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.5/src/docrobot/guimain.pyw` & `docrobot-1.0.6/src/docrobot/guimain.pyw`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,22 @@
 
                 if modify:
                     document.save(doc_name)
             except PackageNotFoundError:
                 self.textEdit.append('Error打开文件错误：' + doc_name)
             except PermissionError:
                 self.textEdit.append('Error 保存文件错误，可能是文件已被打开：' + doc_name)
-            self.textEdit.append(project.p_order + ' 项目：处理完成。 <font color="green"><b>'
-                                 + str(match) + ' </b></font> 项条目匹配。')
+            # 基础17项替换和检查 + N项专利
+            needmatch = 17 + len(project.pat_list.splitlines())
+            if needmatch - match > 0:
+                self.textEdit.append(project.p_order + ' 项目检查完成。 <font color="red"><b>'
+                                     + str(needmatch - match) + ' </b></font> 项条目不匹配。')
+            else:
+                self.textEdit.append(project.p_order + ' 项目检查完成。 <font color="green"><b>'
+                                     + str(match) + ' </b></font> 项条目完全匹配。')
 
     def checkpatent(self, modify=False):
         if modify:
             self.textEdit.setText('')
             self.update_data()
 
         match = 0  # 已匹配条目数
@@ -334,15 +340,15 @@
             doc.tables[0].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
             self.clear_runs(doc.tables[0].rows[0].cells[1].paragraphs[0].runs)
             match = match + 1
         if doc.tables[0].rows[1].cells[0].paragraphs[0].text == '项目编号：':
             doc.tables[0].rows[1].cells[1].paragraphs[0].runs[0].text = prj.p_start[0:4] + 'RD' + prj.p_order
             self.clear_runs(doc.tables[0].rows[1].cells[1].paragraphs[0].runs)
             match = match + 1
-        if doc.tables[0].rows[2].cells[0].paragraphs[0].text == '项目负责人：' and prj.p_owner != 'None':
+        if doc.tables[0].rows[2].cells[0].paragraphs[0].text == '项目负责人：':
             doc.tables[0].rows[2].cells[1].paragraphs[0].runs[0].text = prj.p_owner
             self.clear_runs(doc.tables[0].rows[2].cells[1].paragraphs[0].runs)
             match = match + 1
         if doc.tables[0].rows[3].cells[0].paragraphs[0].text == '项目周期：':
             doc.tables[0].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_start + '至' + prj.p_end
             self.clear_runs(doc.tables[0].rows[3].cells[1].paragraphs[0].runs)
             match = match + 1
@@ -385,19 +391,20 @@
 
     def check_replace(self, paras, regex, dst):
         match = 0
         for i, para in enumerate(paras):
             result = re.search(regex, para.text)
             if result is not None:
                 if result.group() != dst:
-                    self.textEdit.append(result.group() + ' ===> ' + dst)
+                    self.textEdit.append(str(result.group()) + ' ===> ' + dst)
                     para.runs[0].text = re.sub(regex, dst,
                                                para.text)
                     self.clear_runs(para.runs)
-                match = match + 1
+                else:
+                    match = match + 1
                 break  # 只替换一次就够用
         return match
 
     def third_table(self, doc, prj):
         match = 0
         if doc.tables[2].rows[0].cells[0].paragraphs[0].text == '项目名称':
             doc.tables[2].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
```

### Comparing `docrobot-1.0.5/LICENSE` & `docrobot-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.5/pyproject.toml` & `docrobot-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.5/PKG-INFO` & `docrobot-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.5
+Version: 1.0.6
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

