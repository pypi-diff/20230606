# Comparing `tmp/getmodelspec-1.0.19.tar.gz` & `tmp/getmodelspec-1.0.191.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.19.tar", last modified: Tue Jun  6 00:29:01 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.191.tar", last modified: Tue Jun  6 00:33:16 2023, max compression
```

## Comparing `getmodelspec-1.0.19.tar` & `getmodelspec-1.0.191.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/
--rw-rw-rw-   0        0        0      126 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.19/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.19/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.19/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     9981 2023-06-06 00:28:39.000000 getmodelspec-1.0.19/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.19/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0      906 2023-06-05 14:59:18.000000 getmodelspec-1.0.19/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 00:29:01.000000 getmodelspec-1.0.19/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-06 00:28:48.000000 getmodelspec-1.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/
+-rw-rw-rw-   0        0        0      127 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.191/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.191/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.191/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     9986 2023-06-06 00:32:37.000000 getmodelspec-1.0.191/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.191/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-06-05 14:59:18.000000 getmodelspec-1.0.191/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      127 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 00:33:16.000000 getmodelspec-1.0.191/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-06-06 00:33:03.000000 getmodelspec-1.0.191/setup.py
```

### Comparing `getmodelspec-1.0.19/getmodelspec/src/sony.py` & `getmodelspec-1.0.191/getmodelspec/src/sony.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         dictSeries = {}
 
         wd = WebDriver.get_crome()
         wd.get(url=url)
         self.waitingPage(5)
 
         wait = WebDriverWait(wd, self.watingTime)
-        elements = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'custom-variant-selector__item')))  ## 시리즈의 모든 인치 모델 가져 옴
+        elements = wait.until(EC.presence_of_all_elements_located((By.CLASS_NAME, 'custom-variant-selector__item')))  ## 시리즈의 모든 인치 모델 가져 옴
 
         for element in elements:
             try:
                 element_url = element.get_attribute('href')
                 label = self.getNamefromURL(element_url)
                 dictSeries[label]=element_url # url 만 저장 함
             except Exception as e:
```

### Comparing `getmodelspec-1.0.19/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.191/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

