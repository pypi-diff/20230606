# Comparing `tmp/yzy-0.1.1.tar.gz` & `tmp/yzy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzy-0.1.1.tar", last modified: Tue Jun  6 15:22:51 2023, max compression
+gzip compressed data, was "yzy-0.1.2.tar", last modified: Tue Jun  6 16:43:56 2023, max compression
```

## Comparing `yzy-0.1.1.tar` & `yzy-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.742728 yzy-0.1.1/
--rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.1.1/LICENSE
--rw-r--r--   0 yzy        (501) staff       (20)      767 2023-06-06 15:22:51.742606 yzy-0.1.1/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.1.1/README.md
--rw-r--r--   0 yzy        (501) staff       (20)      607 2023-06-06 15:22:34.000000 yzy-0.1.1/pyproject.toml
--rw-r--r--   0 yzy        (501) staff       (20)       38 2023-06-06 15:22:51.742773 yzy-0.1.1/setup.cfg
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.740395 yzy-0.1.1/src/
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.741748 yzy-0.1.1/src/yzy/
--rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.1.1/src/yzy/__init__.py
--rwx------   0 yzy        (501) staff       (20)     5782 2023-06-06 15:19:01.000000 yzy-0.1.1/src/yzy/arxiv.py
--rwx------   0 yzy        (501) staff       (20)      180 2023-06-06 13:43:30.000000 yzy-0.1.1/src/yzy/conf_list.txt
--rwx------   0 yzy        (501) staff       (20)     2596 2023-06-06 15:19:14.000000 yzy-0.1.1/src/yzy/file2md.py
--rwx------   0 yzy        (501) staff       (20)     2139 2023-06-06 15:20:03.000000 yzy-0.1.1/src/yzy/id2md.py
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 15:22:51.742422 yzy-0.1.1/src/yzy.egg-info/
--rwx------   0 yzy        (501) staff       (20)      767 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/PKG-INFO
--rwx------   0 yzy        (501) staff       (20)      281 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/SOURCES.txt
--rwx------   0 yzy        (501) staff       (20)        1 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/dependency_links.txt
--rwx------   0 yzy        (501) staff       (20)       17 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/requires.txt
--rwx------   0 yzy        (501) staff       (20)        4 2023-06-06 15:22:51.000000 yzy-0.1.1/src/yzy.egg-info/top_level.txt
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 16:43:56.520513 yzy-0.1.2/
+-rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.1.2/LICENSE
+-rw-r--r--   0 yzy        (501) staff       (20)      794 2023-06-06 16:43:56.520372 yzy-0.1.2/PKG-INFO
+-rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.1.2/README.md
+-rw-r--r--   0 yzy        (501) staff       (20)      634 2023-06-06 16:43:40.000000 yzy-0.1.2/pyproject.toml
+-rw-r--r--   0 yzy        (501) staff       (20)       38 2023-06-06 16:43:56.520583 yzy-0.1.2/setup.cfg
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 16:43:56.516959 yzy-0.1.2/src/
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 16:43:56.519119 yzy-0.1.2/src/yzy/
+-rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.1.2/src/yzy/__init__.py
+-rwx------   0 yzy        (501) staff       (20)     5858 2023-06-06 16:42:41.000000 yzy-0.1.2/src/yzy/arxiv.py
+-rwx------   0 yzy        (501) staff       (20)      180 2023-06-06 16:42:48.000000 yzy-0.1.2/src/yzy/conf_list.txt
+-rwx------   0 yzy        (501) staff       (20)     2672 2023-06-06 16:42:36.000000 yzy-0.1.2/src/yzy/file2md.py
+-rwx------   0 yzy        (501) staff       (20)     2180 2023-06-06 16:42:26.000000 yzy-0.1.2/src/yzy/id2md.py
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-06-06 16:43:56.520162 yzy-0.1.2/src/yzy.egg-info/
+-rwx------   0 yzy        (501) staff       (20)      794 2023-06-06 16:43:56.000000 yzy-0.1.2/src/yzy.egg-info/PKG-INFO
+-rwx------   0 yzy        (501) staff       (20)      281 2023-06-06 16:43:56.000000 yzy-0.1.2/src/yzy.egg-info/SOURCES.txt
+-rwx------   0 yzy        (501) staff       (20)        1 2023-06-06 16:43:56.000000 yzy-0.1.2/src/yzy.egg-info/dependency_links.txt
+-rwx------   0 yzy        (501) staff       (20)       17 2023-06-06 16:43:56.000000 yzy-0.1.2/src/yzy.egg-info/requires.txt
+-rwx------   0 yzy        (501) staff       (20)        4 2023-06-06 16:43:56.000000 yzy-0.1.2/src/yzy.egg-info/top_level.txt
```

### Comparing `yzy-0.1.1/LICENSE` & `yzy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yzy-0.1.1/PKG-INFO` & `yzy-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code/tree/master/Python%2BarXiv
 Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `yzy-0.1.1/pyproject.toml` & `yzy-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yzy"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Zhiyuan Yang", email="im.crazyang@gmail.com" },
 ]
 description = "Utils"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies =["feedparser",
@@ -17,9 +17,9 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/yzy1996/Python-Code"
+"Homepage" = "https://github.com/yzy1996/Python-Code/tree/master/Python%2BarXiv"
 "Bug Tracker" = "https://github.com/yzy1996/Python-Code/issues"
```

### Comparing `yzy-0.1.1/src/yzy/arxiv.py` & `yzy-0.1.2/src/yzy/arxiv.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,18 +33,19 @@
         self.abs_url_version = feed.entries[0].id
         self.abs_url = self.abs_url_version[:-2]
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
         self.id_version = self.abs_url_version[-12:]
         self.year = feed.entries[0].published[:4]
         self.summary = feed.entries[0].summary
 
-        try:
+        try: # try for no attribute 'arxiv_comment'
             self.comment = feed.entries[0].arxiv_comment
-            publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            self.publish = re.sub(r'\W?(\d{4})', r' \1', publish[0][0]) if publish else f'arXiv {self.year}'
+            self.conf = re.findall(rf'({CONF})', self.comment)[0]
+            self.conf_year = re.findall(r'(\d{4})', self.comment)[0]
+            self.publish = f'{self.conf} {self.conf_year}' if self.conf else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
 
         # self.project_urls = URLExtract().find_urls(self.summary) if self.comment else None
 
     # deprecated
     def _get_arxiv_info_regex(self):
```

### Comparing `yzy-0.1.1/src/yzy/file2md.py` & `yzy-0.1.2/src/yzy/file2md.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,19 @@
         self.abs_url_version = feed.entries[0].id
         self.abs_url = self.abs_url_version[:-2]
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
         self.id_version = self.abs_url_version[-12:]
         self.year = feed.entries[0].published[:4]
         self.summary = feed.entries[0].summary
 
-        try:
+        try: # try for no attribute 'arxiv_comment'
             self.comment = feed.entries[0].arxiv_comment
-            publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            self.publish = re.sub(r'\W?(\d{4})', r' \1', publish[0][0]) if publish else f'arXiv {self.year}'
+            self.conf = re.findall(rf'({CONF})', self.comment)[0]
+            self.conf_year = re.findall(r'(\d{4})', self.comment)[0]
+            self.publish = f'{self.conf} {self.conf_year}' if self.conf else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
 
     def write_notes(self):
 
         title_url = f'[{self.title}]({self.abs_url})  '
         publish = f'**[`{self.publish}`]**'
```

### Comparing `yzy-0.1.1/src/yzy/id2md.py` & `yzy-0.1.2/src/yzy/id2md.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         self.abs_url_version = feed.entries[0].id
         self.abs_url = self.abs_url_version[:-2]
         self.pdf_url = self.abs_url.replace('abs', 'pdf')
         self.id_version = self.abs_url_version[-12:]
         self.year = feed.entries[0].published[:4]
         self.summary = feed.entries[0].summary
 
-        try:
+        try: # try for no attribute 'arxiv_comment'
             self.comment = feed.entries[0].arxiv_comment
-            publish = re.findall(rf'[\s\S]*(({CONF}).*?\d{{4}})[\s\S]*', self.comment)
-            print(publish[0][0])
-            self.publish = re.sub(r'\W?(\d{4})', r' \1', publish[0][0]) if publish else f'arXiv {self.year}'
+            self.conf = re.findall(rf'({CONF})', self.comment)[0]
+            self.conf_year = re.findall(r'(\d{4})', self.comment)[0]
+            self.publish = f'{self.conf} {self.conf_year}' if self.conf else f'arXiv {self.year}'
         except:
             self.publish = f'arXiv {self.year}'
 
     def write_notes(self):
         '''
         define the markdown format and write notes
         '''
@@ -53,15 +53,15 @@
 
 if __name__ == "__main__":
 
     while True:
         id = input("type id: ")
 
         # 2011.13126 2210.08823
-        if re.findall(r'\d{4}\.\d{5}', id):
+        if re.match(r'\d{4}\.\d{5}', id):
 
             information = Information(id)
             information.write_notes()
         
         # >>>
         # - [Lifting 2D StyleGAN for 3D-Aware Face Generation](http://arxiv.org/abs/2011.13126v2)  
         #   **[`CVPR 2021`]** *Yichun Shi, Divyansh Aggarwal, Anil K. Jain*
```

### Comparing `yzy-0.1.1/src/yzy.egg-info/PKG-INFO` & `yzy-0.1.2/src/yzy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code/tree/master/Python%2BarXiv
 Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

