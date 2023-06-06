# Comparing `tmp/yzy-0.1.0.tar.gz` & `tmp/yzy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzy-0.1.0.tar", last modified: Tue Jun  6 11:49:34 2023, max compression
+gzip compressed data, was "yzy-0.1.1.tar", last modified: Tue Jun  6 15:22:51 2023, max compression
```

## Comparing `yzy-0.1.0.tar` & `yzy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:34.003075 yzy-0.1.0/
--rw-rw-rw-   0        0        0     1073 2023-04-02 11:39:35.000000 yzy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-06 11:49:34.003075 yzy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-09 03:08:26.000000 yzy-0.1.0/README.md
--rw-rw-rw-   0        0        0      607 2023-06-06 11:47:40.000000 yzy-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 11:49:34.003075 yzy-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:33.990076 yzy-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:33.994075 yzy-0.1.0/src/yzy/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:41:50.000000 yzy-0.1.0/src/yzy/__init__.py
--rw-rw-rw-   0        0        0     5660 2023-06-06 09:19:07.000000 yzy-0.1.0/src/yzy/arxiv.py
--rw-rw-rw-   0        0        0     2500 2023-06-06 09:17:59.000000 yzy-0.1.0/src/yzy/file2md.py
--rw-rw-rw-   0        0        0     1973 2023-06-06 09:18:22.000000 yzy-0.1.0/src/yzy/id2md.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:34.002074 yzy-0.1.0/src/yzy.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/top_level.txt
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.742728 yzy-0.1.1/
+-rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.1.1/LICENSE
+-rw-r--r--   0 yzy        (501) staff       (20)      767 2023-06-06 15:22:51.742606 yzy-0.1.1/PKG-INFO
+-rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.1.1/README.md
+-rw-r--r--   0 yzy        (501) staff       (20)      607 2023-06-06 15:22:34.000000 yzy-0.1.1/pyproject.toml
+-rw-r--r--   0 yzy        (501) staff       (20)       38 2023-06-06 15:22:51.742773 yzy-0.1.1/setup.cfg
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.740395 yzy-0.1.1/src/
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.741748 yzy-0.1.1/src/yzy/
+-rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.1.1/src/yzy/__init__.py
+-rwx------   0 yzy        (501) staff       (20)     5782 2023-06-06 15:19:01.000000 yzy-0.1.1/src/yzy/arxiv.py
+-rwx------   0 yzy        (501) staff       (20)      180 2023-06-06 13:43:30.000000 yzy-0.1.1/src/yzy/conf_list.txt
+-rwx------   0 yzy        (501) staff       (20)     2596 2023-06-06 15:19:14.000000 yzy-0.1.1/src/yzy/file2md.py
+-rwx------   0 yzy        (501) staff       (20)     2139 2023-06-06 15:20:03.000000 yzy-0.1.1/src/yzy/id2md.py
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.742422 yzy-0.1.1/src/yzy.egg-info/
+-rwx------   0 yzy        (501) staff       (20)      767 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/PKG-INFO
+-rwx------   0 yzy        (501) staff       (20)      281 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/SOURCES.txt
+-rwx------   0 yzy        (501) staff       (20)        1 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/dependency_links.txt
+-rwx------   0 yzy        (501) staff       (20)       17 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/requires.txt
+-rwx------   0 yzy        (501) staff       (20)        4 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/top_level.txt
```

### Comparing `yzy-0.1.0/LICENSE` & `yzy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yzy-0.1.0/PKG-INFO` & `yzy-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: yzy
-Version: 0.1.0
-Summary: Utils
-Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/yzy1996/Python-Code
-Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
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
+Version: 0.1.1
+Summary: Utils
+Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
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

### Comparing `yzy-0.1.0/pyproject.toml` & `yzy-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yzy"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Zhiyuan Yang", email="im.crazyang@gmail.com" },
 ]
 description = "Utils"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies =["feedparser",
```

### Comparing `yzy-0.1.0/src/yzy/arxiv.py` & `yzy-0.1.1/src/yzy/arxiv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import re
 from urllib import request
 from pathlib import Path
 import feedparser
+from pathlib import Path
+
+p = Path(__file__)
 
-with open('conf_list.txt', 'r') as f:
+with open(p.parents[0] / 'conf_list.txt', 'r') as f:
     data = f.read()
 CONF = data.split('\n')
 CONF = '|'.join(CONF)
 
 
 class Information():
     '''
@@ -23,24 +26,25 @@
             query_url = f'https://export.arxiv.org/api/query?search_query=ti:{query_title1}&max_results=1'
 
         export_arxiv = request.urlopen(query_url).read().decode('utf-8')
         feed = feedparser.parse(export_arxiv)
 
         self.title = re.sub(r'[^\w\s-]', '', feed.entries[0].title)
         self.authors = [author.name for author in feed.entries[0].authors]
-        self.abs_url = feed.entries[0].id
+        self.abs_url_version = feed.entries[0].id
+        self.abs_url = self.abs_url_version[:-2]
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
-        self.id_version = self.abs_url[-12:]
+        self.id_version = self.abs_url_version[-12:]
         self.year = feed.entries[0].published[:4]
         self.summary = feed.entries[0].summary
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
+            self.publish = re.sub(r'\W?(\d{4})', r' \1', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
 
         # self.project_urls = URLExtract().find_urls(self.summary) if self.comment else None
 
     # deprecated
     def _get_arxiv_info_regex(self):
```

### Comparing `yzy-0.1.0/src/yzy/file2md.py` & `yzy-0.1.1/src/yzy/file2md.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from urllib import request
 import re
 from pathlib import Path
-from PyPDF2 import PdfReader
+from pypdf import PdfReader
 import feedparser
 
-with open('conf_list.txt', 'r') as f:
+p = Path(__file__)
+
+with open(p.parents[0] / 'conf_list.txt', 'r') as f:
     data = f.read()
 CONF = data.split('\n')
 CONF = '|'.join(CONF)
 
 class Information():
     def __init__(self, query_title) -> None:
 
@@ -22,24 +24,25 @@
             self.query_url = f'https://export.arxiv.org/api/query?search_query=ti:{query_title1}&max_results=1'
 
         export_arxiv = request.urlopen(query_url).read().decode('utf-8')
         feed = feedparser.parse(export_arxiv)
 
         self.title = re.sub(r'[^\w\s-]', '', feed.entries[0].title)
         self.authors = [author.name for author in feed.entries[0].authors]
-        self.abs_url = feed.entries[0].id
+        self.abs_url_version = feed.entries[0].id
+        self.abs_url = self.abs_url_version[:-2]
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
-        self.id_version = self.abs_url[-12:]
+        self.id_version = self.abs_url_version[-12:]
         self.year = feed.entries[0].published[:4]
         self.summary = feed.entries[0].summary
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
+            self.publish = re.sub(r'\W?(\d{4})', r' \1', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
 
     def write_notes(self):
 
         title_url = f'[{self.title}]({self.abs_url})  '
         publish = f'**[`{self.publish}`]**'
```

### Comparing `yzy-0.1.0/src/yzy/id2md.py` & `yzy-0.1.1/src/yzy/id2md.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from urllib import request
 import re
 import feedparser
+from pathlib import Path
 
-with open('conf_list.txt', 'r') as f:
+p = Path(__file__)
+
+with open(p.parents[0] / 'conf_list.txt', 'r') as f:
     data = f.read()
 CONF = data.split('\n')
 CONF = '|'.join(CONF)
 
 class Information():
     '''
     extract information from arxiv api
@@ -16,24 +19,26 @@
 
         query_url = f'http://export.arxiv.org/api/query?id_list={query_id}'
         export_arxiv = request.urlopen(query_url).read().decode('utf-8')
         feed = feedparser.parse(export_arxiv)
 
         self.title = re.sub(r'[^\w\s-]', '', feed.entries[0].title)
         self.authors = [author.name for author in feed.entries[0].authors]
-        self.abs_url = feed.entries[0].id
+        self.abs_url_version = feed.entries[0].id
+        self.abs_url = self.abs_url_version[:-2]
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
-        self.id_version = self.abs_url[-12:]
+        self.id_version = self.abs_url_version[-12:]
         self.year = feed.entries[0].published[:4]
         self.summary = feed.entries[0].summary
 
         try:
             self.comment = feed.entries[0].arxiv_comment
             publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            self.publish = re.sub(r'(\w)(\d{4})', r'\1 \2', publish[0][0]) if publish else f'arXiv {self.year}'
+            print(publish[0][0])
+            self.publish = re.sub(r'\W?(\d{4})', r' \1', publish[0][0]) if publish else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
 
     def write_notes(self):
         '''
         define the markdown format and write notes
         '''
@@ -47,15 +52,15 @@
         print(' ', publish, authors)
 
 if __name__ == "__main__":
 
     while True:
         id = input("type id: ")
 
-        # 2011.13126
+        # 2011.13126 2210.08823
         if re.findall(r'\d{4}\.\d{5}', id):
 
             information = Information(id)
             information.write_notes()
         
         # >>>
         # - [Lifting 2D StyleGAN for 3D-Aware Face Generation](http://arxiv.org/abs/2011.13126v2)
```

### Comparing `yzy-0.1.0/src/yzy.egg-info/PKG-INFO` & `yzy-0.1.1/src/yzy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: yzy
-Version: 0.1.0
-Summary: Utils
-Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/yzy1996/Python-Code
-Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
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
+Version: 0.1.1
+Summary: Utils
+Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
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

