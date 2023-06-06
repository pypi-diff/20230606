# Comparing `tmp/getmodelspec-1.0.23.tar.gz` & `tmp/getmodelspec-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.23.tar", last modified: Tue Jun  6 15:24:34 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.24.tar", last modified: Tue Jun  6 15:46:00 2023, max compression
```

## Comparing `getmodelspec-1.0.23.tar` & `getmodelspec-1.0.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/
--rw-rw-rw-   0        0        0      126 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.23/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.23/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.23/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     9748 2023-06-06 15:23:19.000000 getmodelspec-1.0.23/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.23/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.23/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.23/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:24:34.000000 getmodelspec-1.0.23/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-06 15:23:27.000000 getmodelspec-1.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/
+-rw-rw-rw-   0        0        0      126 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.24/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.24/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.24/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     9856 2023-06-06 15:45:08.000000 getmodelspec-1.0.24/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.24/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.24/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.24/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-06 15:45:58.000000 getmodelspec-1.0.24/setup.py
```

### Comparing `getmodelspec-1.0.23/getmodelspec/src/sony.py` & `getmodelspec-1.0.24/getmodelspec/src/sony.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         backUp(dictAllSeries, "dictAllSeries")
         # with open(f"dictAllSeries.pickle", "rb") as file:
         #     dictAllSeries = pickle.load(file)
         # ==========================================================================
 
         # 모든 모델 리스트를 추출
         dictModels = {}
-        for model_url in dictAllSeries.values():
-            print(model_url)
+        for cnt, model_url in enumerate(dictAllSeries.values()):
+            print(f"{cnt+1}/{len(dictAllSeries)} | {model_url}")
             try:
                 dictModels.update(self.getPage3rd(model_url))
             except:
                 print(f"fail to get info from {model_url}")
 
                 dictModels.update({getNamefromURL(url): dict()})
                 pass
@@ -121,15 +121,15 @@
                 wd.quit()
                 waitingPage(1)
                 print(f"stage 2nd try: {cntTry}/5")
 
     ###======================final stage===============================##
     def getPage3rd(self, url:str) -> dict:
 
-        cntTryTotal = 10
+        cntTryTotal = 20
         for cntTry in range(cntTryTotal):
             try:
                 dictSpec = {}
                 wd = WebDriver.get_crome()
                 wd.get(url=url)
                 waitingPage(5)
 
@@ -151,16 +151,19 @@
                     print("price error")
                     dictSpec["price"] = ""
 
 
                 #이미지 정보 및 url 저장
                 dictSpec["src_url"] = url
                 dictSpec["Img_url"] = wd.find_element(By.XPATH, '//app-custom-cx-media//img').get_attribute('src')
+
+
                 if self.envr == "colab":
                     wd.quit()
+                    print(f"{model}\n", dictModel)
                     dictModel = {model: dictSpec}
                     return dictModel
 
 
                 elementSpec = wd.find_element(By.ID,"PDPSpecificationsLink")
                 wd = WebDriver.move_element_to_center(wd,elementSpec)
                 wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_1_move_to_spec_{get_today()}.png")  # 스크린 샷
```

### Comparing `getmodelspec-1.0.23/getmodelspec/tools/functions.py` & `getmodelspec-1.0.24/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.23/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.24/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

