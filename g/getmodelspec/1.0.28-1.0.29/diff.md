# Comparing `tmp/getmodelspec-1.0.28.tar.gz` & `tmp/getmodelspec-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.28.tar", last modified: Tue Jun  6 16:26:42 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.29.tar", last modified: Tue Jun  6 16:29:01 2023, max compression
```

## Comparing `getmodelspec-1.0.28.tar` & `getmodelspec-1.0.29.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/
--rw-rw-rw-   0        0        0      126 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.28/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.28/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.28/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    10658 2023-06-06 16:26:14.000000 getmodelspec-1.0.28/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.28/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.28/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.28/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:26:42.000000 getmodelspec-1.0.28/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-06 16:26:30.000000 getmodelspec-1.0.28/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/
+-rw-rw-rw-   0        0        0      126 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.29/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.29/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.29/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0    10658 2023-06-06 16:28:44.000000 getmodelspec-1.0.29/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.29/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-06-06 13:53:01.000000 getmodelspec-1.0.29/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     2598 2023-06-06 13:53:01.000000 getmodelspec-1.0.29/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-06-06 16:29:00.000000 getmodelspec-1.0.29/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-06-06 16:29:00.000000 getmodelspec-1.0.29/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:29:00.000000 getmodelspec-1.0.29/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-06 16:29:00.000000 getmodelspec-1.0.29/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 16:29:00.000000 getmodelspec-1.0.29/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 16:29:00.000000 getmodelspec-1.0.29/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:29:01.000000 getmodelspec-1.0.29/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-06 16:28:52.000000 getmodelspec-1.0.29/setup.py
```

### Comparing `getmodelspec-1.0.28/getmodelspec/src/sony.py` & `getmodelspec-1.0.29/getmodelspec/src/sony.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
                 #이미지 정보 및 url 저장
                 dictSpec["src_url"] = url
                 dictSpec["Img_url"] = wd.find_element(By.XPATH, '//app-custom-cx-media//img').get_attribute('src')
 
 
                 if self.envr == "colab":
                     wd.quit()
-                    print(f"{model}\n", dictModel)
                     dictModel = {model: dictSpec}
+                    print(f"{model}\n", dictModel)
                     return dictModel
 
 
                 elementSpec = wd.find_element(By.ID,"PDPSpecificationsLink")
                 wd = WebDriver.move_element_to_center(wd,elementSpec)
                 wd.save_screenshot(f"./{dir_model}/{getNamefromURL(url)}_1_move_to_spec_{get_today()}.png")  # 스크린 샷
```

### Comparing `getmodelspec-1.0.28/getmodelspec/tools/functions.py` & `getmodelspec-1.0.29/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.28/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.29/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

