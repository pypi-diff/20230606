# Comparing `tmp/yzy-0.0.4.tar.gz` & `tmp/yzy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzy-0.0.4.tar", last modified: Sun Apr  9 04:25:13 2023, max compression
+gzip compressed data, was "yzy-0.0.5.tar", last modified: Tue Jun  6 10:21:50 2023, max compression
```

## Comparing `yzy-0.0.4.tar` & `yzy-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.170597 yzy-0.0.4/
--rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.0.4/LICENSE
--rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 04:25:13.170457 yzy-0.0.4/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.0.4/README.md
--rw-r--r--   0 yzy        (501) staff       (20)      552 2023-04-09 04:24:53.000000 yzy-0.0.4/pyproject.toml
--rw-r--r--   0 yzy        (501) staff       (20)       38 2023-04-09 04:25:13.170647 yzy-0.0.4/setup.cfg
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.168104 yzy-0.0.4/src/
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.169647 yzy-0.0.4/src/yzy/
--rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.0.4/src/yzy/__init__.py
--rwx------   0 yzy        (501) staff       (20)     5820 2023-04-09 04:22:19.000000 yzy-0.0.4/src/yzy/arxiv.py
--rwx------   0 yzy        (501) staff       (20)     2497 2023-04-09 04:22:05.000000 yzy-0.0.4/src/yzy/file2md.py
--rwx------   0 yzy        (501) staff       (20)     1767 2023-04-09 04:22:25.000000 yzy-0.0.4/src/yzy/id2md.py
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 04:25:13.170273 yzy-0.0.4/src/yzy.egg-info/
--rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      229 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/SOURCES.txt
--rw-r--r--   0 yzy        (501) staff       (20)        1 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/dependency_links.txt
--rw-r--r--   0 yzy        (501) staff       (20)        4 2023-04-09 04:25:13.000000 yzy-0.0.4/src/yzy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.797742 yzy-0.0.5/
+-rw-rw-rw-   0        0        0     1073 2023-04-02 11:39:35.000000 yzy-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-06 10:21:50.797742 yzy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-09 03:08:26.000000 yzy-0.0.5/README.md
+-rw-rw-rw-   0        0        0      608 2023-06-06 10:20:52.000000 yzy-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:21:50.797742 yzy-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.777740 yzy-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.788740 yzy-0.0.5/src/yzy/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:41:50.000000 yzy-0.0.5/src/yzy/__init__.py
+-rw-rw-rw-   0        0        0     5660 2023-06-06 09:19:07.000000 yzy-0.0.5/src/yzy/arxiv.py
+-rw-rw-rw-   0        0        0     2500 2023-06-06 09:17:59.000000 yzy-0.0.5/src/yzy/file2md.py
+-rw-rw-rw-   0        0        0     1973 2023-06-06 09:18:22.000000 yzy-0.0.5/src/yzy/id2md.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.796740 yzy-0.0.5/src/yzy.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/top_level.txt
```

### Comparing `yzy-0.0.4/LICENSE` & `yzy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yzy-0.0.4/PKG-INFO` & `yzy-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: yzy
-Version: 0.0.4
-Summary: Utils
-Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/yzy1996/Python-Code
-Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# yzy
-
-各种工具
-
-
-
-## Support
-
-- **arxiv.py**: combined
-- **id2md.py**: input arxiv id and then get the markdown format output.
-- **file2md.py**: input foldername containing papers and then get the markdown format output.
-
-```
-python -m yzy.id2md
-
-python yzy.arxiv.id2md()
-```
-
-
-
-
-
-
-
+Metadata-Version: 2.1
+Name: yzy
+Version: 0.0.5
+Summary: Utils
+Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# yzy
+
+各种工具
+
+
+
+## Support
+
+- **arxiv.py**: combined
+- **id2md.py**: input arxiv id and then get the markdown format output.
+- **file2md.py**: input foldername containing papers and then get the markdown format output.
+
+```
+python -m yzy.id2md
+
+python yzy.arxiv.id2md()
+```
+
+
+
+
+
+
+
```

### Comparing `yzy-0.0.4/pyproject.toml` & `yzy-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yzy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Zhiyuan Yang", email="im.crazyang@gmail.com" },
 ]
 description = "Utils"
 readme = "README.md"
 requires-python = ">=3.9"
+dependencies =["feedparser",
+               "PyPDF2",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `yzy-0.0.4/src/yzy/arxiv.py` & `yzy-0.0.5/src/yzy/arxiv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 from urllib import request
 from pathlib import Path
 import feedparser
-# from urlextract import URLExtract
 
-CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI|WACV|ICASSP|ICRA'
+with open('conf_list.txt', 'r') as f:
+    data = f.read()
+CONF = data.split('\n')
+CONF = '|'.join(CONF)
 
 
 class Information():
     '''
     extract information from arxiv api
     '''
 
@@ -33,15 +35,14 @@
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
             self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
-            pass
 
         # self.project_urls = URLExtract().find_urls(self.summary) if self.comment else None
 
     # deprecated
     def _get_arxiv_info_regex(self):
 
         Id = r'<id>http://arxiv.org/abs/(.*)</id>'
@@ -69,18 +70,14 @@
         self.year = year
         self.publish = ''
         self.affiliation = ''
 
         self.abs_url = f'https://arxiv.org/abs/{self.id}'
         self.pdf_url = f'https://arxiv.org/pdf/{self.id}'
 
-        # with open(r'conf_list.txt') as f:
-        #     lines = [line.strip() for line in f]
-        # reg = '|'.join(lines)
-
         publish = re.findall(Publish, self.export_arxiv)
 
         if publish != []:
             self.publish = publish[0][0]
             self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2',
                                   self.publish)  # CVPR2020 -> CVPR 2020
```

### Comparing `yzy-0.0.4/src/yzy/file2md.py` & `yzy-0.0.5/src/yzy/file2md.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from urllib import request
 import re
 from pathlib import Path
 from PyPDF2 import PdfReader
 import feedparser
 
-CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI|WACV|ICASSP|ICRA'
-
+with open('conf_list.txt', 'r') as f:
+    data = f.read()
+CONF = data.split('\n')
+CONF = '|'.join(CONF)
 
 class Information():
     def __init__(self, query_title) -> None:
 
         query_id = read_pdf(query_title)
 
         if re.findall(r'\d{4}.\d{5}', query_id):
@@ -32,15 +34,14 @@
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
             self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
-            pass
 
     def write_notes(self):
 
         title_url = f'[{self.title}]({self.abs_url})  '
         publish = f'**[`{self.publish}`]**'
         authors = ', '.join(self.authors)
         authors = f'*{authors}*'
```

### Comparing `yzy-0.0.4/src/yzy/id2md.py` & `yzy-0.0.5/src/yzy/id2md.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from urllib import request
 import re
 import feedparser
 
-CONF = 'ICML|NIPS|NeurIPS|ICLR|CVPR|ICCV|ECCV|AAAI|IJCAI|3DV|UAI|WACV|ICASSP|ICRA'
-
+with open('conf_list.txt', 'r') as f:
+    data = f.read()
+CONF = data.split('\n')
+CONF = '|'.join(CONF)
 
 class Information():
     '''
     extract information from arxiv api
     '''    
+    
     def __init__(self, query_id) -> None:
 
         query_url = f'http://export.arxiv.org/api/query?id_list={query_id}'
         export_arxiv = request.urlopen(query_url).read().decode('utf-8')
         feed = feedparser.parse(export_arxiv)
 
         self.title = re.sub(r'[^\w\s-]', '', feed.entries[0].title)
@@ -25,15 +28,14 @@
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
             self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
-            pass
 
     def write_notes(self):
         '''
         define the markdown format and write notes
         '''
 
         title_url = f'[{self.title}]({self.abs_url})  '
@@ -50,7 +52,11 @@
         id = input("type id: ")
 
         # 2011.13126
         if re.findall(r'\d{4}\.\d{5}', id):
 
             information = Information(id)
             information.write_notes()
+        
+        # >>>
+        # - [Lifting 2D StyleGAN for 3D-Aware Face Generation](http://arxiv.org/abs/2011.13126v2)  
+        #   **[`CVPR 2021`]** *Yichun Shi, Divyansh Aggarwal, Anil K. Jain*
```

### Comparing `yzy-0.0.4/src/yzy.egg-info/PKG-INFO` & `yzy-0.0.5/src/yzy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: yzy
-Version: 0.0.4
-Summary: Utils
-Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/yzy1996/Python-Code
-Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# yzy
-
-各种工具
-
-
-
-## Support
-
-- **arxiv.py**: combined
-- **id2md.py**: input arxiv id and then get the markdown format output.
-- **file2md.py**: input foldername containing papers and then get the markdown format output.
-
-```
-python -m yzy.id2md
-
-python yzy.arxiv.id2md()
-```
-
-
-
-
-
-
-
+Metadata-Version: 2.1
+Name: yzy
+Version: 0.0.5
+Summary: Utils
+Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# yzy
+
+各种工具
+
+
+
+## Support
+
+- **arxiv.py**: combined
+- **id2md.py**: input arxiv id and then get the markdown format output.
+- **file2md.py**: input foldername containing papers and then get the markdown format output.
+
+```
+python -m yzy.id2md
+
+python yzy.arxiv.id2md()
+```
+
+
+
+
+
+
+
```

