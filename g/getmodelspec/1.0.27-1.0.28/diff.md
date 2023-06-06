# Comparing `tmp/getmodelspec-1.0.27.tar.gz` & `tmp/getmodelspec-1.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.27.tar", last modified: Tue Jun  6 16:17:42 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.28.tar", last modified: Tue Jun  6 16:26:42 2023, max compression
```

## Comparing `getmodelspec-1.0.27.tar` & `getmodelspec-1.0.28.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/
--rw-rw-rw-   0        0        0      126 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.27/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.27/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.27/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    10504 2023-06-06 16:16:27.000000 getmodelspec-1.0.27/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.27/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.27/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.27/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:17:42.000000 getmodelspec-1.0.27/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-06 16:17:32.000000 getmodelspec-1.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/
+-rw-rw-rw-   0        0        0      126 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.28/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.28/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.28/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    10658 2023-06-06 16:26:14.000000 getmodelspec-1.0.28/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.28/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.28/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.28/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-06 16:26:30.000000 getmodelspec-1.0.28/setup.py
```

### Comparing `getmodelspec-1.0.27/getmodelspec/src/sony.py` & `getmodelspec-1.0.28/getmodelspec/src/sony.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,13 +237,14 @@
 
 
 
 def closeModalCookie(webdriver):
         # 모달 창 요소를 식별하여 클릭
         try:
             close_button = webdriver.find_element(By.CLASS_NAME, '//*[@id="onetrust-close-btn-container"]/button')
-            webdriver = WebDriver.move_element_to_center(webdriver, close_button)
+            # webdriver = WebDriver.move_element_to_center(webdriver, close_button)
             close_button.click()
-
+            wait = WebDriverWait(webdriver, 10)
+            wait.until(EC.invisibility_of_element_located((By.XPATH,'//*[@id="onetrust-banner-sdk"]')))
         except:
             pass
         return webdriver
```

### Comparing `getmodelspec-1.0.27/getmodelspec/tools/functions.py` & `getmodelspec-1.0.28/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.27/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.28/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

