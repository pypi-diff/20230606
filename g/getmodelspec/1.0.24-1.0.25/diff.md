# Comparing `tmp/getmodelspec-1.0.24.tar.gz` & `tmp/getmodelspec-1.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.24.tar", last modified: Tue Jun  6 15:46:00 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.25.tar", last modified: Tue Jun  6 15:58:12 2023, max compression
```

## Comparing `getmodelspec-1.0.24.tar` & `getmodelspec-1.0.25.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/
--rw-rw-rw-   0        0        0      126 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.24/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.24/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.24/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     9856 2023-06-06 15:45:08.000000 getmodelspec-1.0.24/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.24/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.24/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.24/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:46:00.000000 getmodelspec-1.0.24/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-06 15:45:58.000000 getmodelspec-1.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/
+-rw-rw-rw-   0        0        0      126 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.25/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.25/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.25/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    10334 2023-06-06 15:58:04.000000 getmodelspec-1.0.25/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.25/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.25/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.25/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:58:12.000000 getmodelspec-1.0.25/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-06 15:58:04.000000 getmodelspec-1.0.25/setup.py
```

### Comparing `getmodelspec-1.0.24/getmodelspec/src/sony.py` & `getmodelspec-1.0.25/getmodelspec/src/sony.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,37 +69,43 @@
         scrolling_cnt: int = 10
 
         wd =  WebDriver.get_crome()
         wd.get(url=url)
         wait = WebDriverWait(wd, 10)
 
         for cnt in range(scrolling_cnt):
+
+            waitingPage(1)
+            closeModalCookie(wd) #쿠키 모달창 닫기
+
             elements = wait.until(EC.visibility_of_all_elements_located((By.CLASS_NAME, 'custom-product-grid-item__product-name')))  ## 모든 인치 모델 가져 옴
             for element in elements:
                 try: set_mainSeries.add(element.get_attribute('href')) #URL만 저장 함
                 except Exception as e:
                     print(f"getPage1st error ({e})")
                     pass
             wd.find_element(By.TAG_NAME,'body').send_keys(Keys.PAGE_DOWN)
             wd.save_screenshot(f"./{self.dir_1st}/Main_Series_{cnt}_{get_today()}.png")  # 스크린 샷
-            waitingPage(1)
         wd.quit()
         print("Number of SONY Main Series:", len(set_mainSeries))
         return set_mainSeries
 
     ###=====================get info Sub page====================================##
     def getPage2nd(self, url:str) -> dict:
 
         for cntTry in range(5):
             try:
                 dictSeries = {}
                 wd = WebDriver.get_crome()
                 wd.get(url=url)
                 print("connect to",url)
 
+                waitingPage(1)
+                closeModalCookie(wd)  # 쿠키 모달창 닫기
+
                 wd.execute_script("window.scrollTo(0, 200);")
                 wait = WebDriverWait(wd, 10)
                 elements = wait.until(EC.visibility_of_all_elements_located((By.CLASS_NAME, 'custom-variant-selector__item')))  ## 시리즈의 모든 인치 모델 가져 옴
                 for element in elements:
                     try:
                         element_url = element.get_attribute('href')
                         label = getNamefromURL(element_url)
@@ -129,14 +135,16 @@
         for cntTry in range(cntTryTotal):
             try:
                 dictSpec = {}
                 wd = WebDriver.get_crome()
                 wd.get(url=url)
                 waitingPage(5)
 
+                closeModalCookie(wd)  # 쿠키 모달창 닫기
+
                 #모델 정보 확인
                 wd.execute_script("window.scrollTo(0, 200);")
                 elementModel = wd.find_element(By.CLASS_NAME, 'product-intro__code')
                 model = elementModel.text.replace("Model: ", "")
 
                 dictSpec["Descr"] = wd.find_element(By.CLASS_NAME, 'product-intro__title').text.strip()
 
@@ -192,15 +200,15 @@
                 waitingPage(2)  # 페이지 로딩 대기 -
                 wd.find_element(By.ID, "ngb-nav-0-panel").click()
                 #스펙 팝업 창의 스펙 가져오기
                 for cnt in range(15):
                     elements = wd.find_elements(By.CLASS_NAME, "full-specifications__specifications-single-card__sub-list")
                     for element in elements:
                         soup = BeautifulSoup(element.get_attribute("innerHTML"), 'html.parser')
-                        dictSpec.update(SoupToDict(soup))
+                        dictSpec.update(soupToDict(soup))
                     ActionChains(wd).key_down(Keys.PAGE_DOWN).perform()
                 wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_4_end_{get_today()}.png")  # 스크린 샷
 
                 wd.quit()
                 dictModel = {model: dictSpec}
                 print(f"{model}\n", dictModel)
                 return dictModel
@@ -212,17 +220,25 @@
 
 
 
 
 # ===============================
 
 
-def SoupToDict(soup):
+def soupToDict(soup):
     try:
         h4_tag = soup.find('h4').text.strip()
         p_tag = soup.find('p').text.strip()
     except Exception as e:
         print("parser err", e)
         h4_tag = soup.find('h4').text.strip()
         p_tag =  ""
         pass
     return {h4_tag: p_tag}
+
+
+
+def closeModalCookie(webdriver):
+        # 모달 창 요소를 식별하여 클릭
+        close_button = webdriver.find_element(By.XPATH, "//button[@class='onetrust-close-btn-handler']")
+        close_button.click()
+        return None
```

### Comparing `getmodelspec-1.0.24/getmodelspec/tools/functions.py` & `getmodelspec-1.0.25/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.24/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.25/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

