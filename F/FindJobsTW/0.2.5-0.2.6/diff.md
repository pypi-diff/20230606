# Comparing `tmp/FindJobsTW-0.2.5.tar.gz` & `tmp/FindJobsTW-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-0.2.5.tar", last modified: Tue Jun  6 09:07:27 2023, max compression
+gzip compressed data, was "FindJobsTW-0.2.6.tar", last modified: Tue Jun  6 09:10:12 2023, max compression
```

## Comparing `FindJobsTW-0.2.5.tar` & `FindJobsTW-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:07:27.124568 FindJobsTW-0.2.5/
-drwxrwxrwx   0        0        0        0 2023-06-06 09:07:27.115565 FindJobsTW-0.2.5/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-06 09:07:26.000000 FindJobsTW-0.2.5/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-06 09:07:27.000000 FindJobsTW-0.2.5/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:07:26.000000 FindJobsTW-0.2.5/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-06 09:07:26.000000 FindJobsTW-0.2.5/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 09:07:26.000000 FindJobsTW-0.2.5/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      591 2023-06-06 09:07:27.123560 FindJobsTW-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 09:07:27.121558 FindJobsTW-0.2.5/findJobs/
--rw-rw-rw-   0        0        0    11162 2023-06-06 08:59:40.000000 FindJobsTW-0.2.5/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.2.5/findJobs/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 09:07:27.124568 FindJobsTW-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-06 09:01:06.000000 FindJobsTW-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:10:12.982374 FindJobsTW-0.2.6/
+drwxrwxrwx   0        0        0        0 2023-06-06 09:10:12.974366 FindJobsTW-0.2.6/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 09:10:12.000000 FindJobsTW-0.2.6/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      591 2023-06-06 09:10:12.981373 FindJobsTW-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 09:10:12.978363 FindJobsTW-0.2.6/findJobs/
+-rw-rw-rw-   0        0        0    11164 2023-06-06 09:09:34.000000 FindJobsTW-0.2.6/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 03:04:46.000000 FindJobsTW-0.2.6/findJobs/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:10:12.982374 FindJobsTW-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-06-06 09:10:06.000000 FindJobsTW-0.2.6/setup.py
```

### Comparing `FindJobsTW-0.2.5/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-0.2.6/FindJobsTW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.2.5/LICENSE` & `FindJobsTW-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-0.2.5/PKG-INFO` & `FindJobsTW-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-0.2.5/findJobs/FindJobs.py` & `FindJobsTW-0.2.6/findJobs/FindJobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
              "工作技能" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[2]/div[{index}]/div[2]/div//*/a/u",
              "具備證照" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[2]/div[{index}]/div[2]/div//*/p/a/u",
              "其他條件" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[3]/div/div[2]/div/div/p",
              "具備駕照" : f"/html/body/div[2]/div/div[2]/div/div[1]/div[2]/div[2]/div[{index}]/div[2]/div",
             }
         return match.get(col_name)
 
-    def search_jobs(self, max_pages = 3):
+    def search_links(self, max_pages = 3):
         page = 1
         data = []
         print(f"開始搜尋關鍵字: {self.keyword}")
         while True:
             url = f'https://www.104.com.tw/jobs/search/?ro=0&kwop=7&keyword={self.keyword}&expansionType=area%2Cspec%2Ccom%2Cjob%2Cwf%2Cwktm&order=15&asc=0&page={page}&mode=s&jobsource=2018indexpoc&langFlag=0&langStatus=0&recommendJob=1&hotJob=1'
             res = requests.get(url, timeout=10)
             soup = BeautifulSoup(res.text, features="lxml")
@@ -223,11 +223,11 @@
         path = self.keyword + r"-職位資料爬蟲.xlsx"
         self.jobs.to_excel(path, index = False)
         print(f"{path}資料已儲存")
            
 if __name__ == "__main__":
     keyword = "平面設計"
     jobs = Jobs(keyword)
-    jobs.search_jobs(max_pages = 3)
+    jobs.search_links(max_pages = 3)
     jobs.find_jobs()
     jobs.save_jobs()
```

### Comparing `FindJobsTW-0.2.5/setup.py` & `FindJobsTW-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='0.2.5',      
+    version='0.2.6',      
     packages=find_packages(),    
     install_requires=requirements,
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
```

