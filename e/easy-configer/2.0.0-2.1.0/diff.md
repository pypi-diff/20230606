# Comparing `tmp/easy_configer-2.0.0.tar.gz` & `tmp/easy_configer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_configer-2.0.0.tar", last modified: Fri Apr 21 06:56:32 2023, max compression
+gzip compressed data, was "easy_configer-2.1.0.tar", last modified: Tue Jun  6 09:32:55 2023, max compression
```

## Comparing `easy_configer-2.0.0.tar` & `easy_configer-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.187587 easy_configer-2.0.0/
--rw-rw-rw-   0        0        0    17635 2023-04-21 06:56:32.186614 easy_configer-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13903 2023-04-21 05:47:34.000000 easy_configer-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.112543 easy_configer-2.0.0/easy_configer/
--rw-rw-rw-   0        0        0     1456 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/Argparser.py
--rw-rw-rw-   0        0        0     9359 2023-04-12 14:02:36.000000 easy_configer-2.0.0/easy_configer/Configer.py
--rw-rw-rw-   0        0        0     2023 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/IO_Converter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.154513 easy_configer-2.0.0/easy_configer/utils/
--rw-rw-rw-   0        0        0      807 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/utils/Flag.py
--rw-rw-rw-   0        0        0     3160 2023-04-21 05:47:25.000000 easy_configer-2.0.0/easy_configer/utils/Type_Convertor.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.137911 easy_configer-2.0.0/easy_configer.egg-info/
--rw-rw-rw-   0        0        0    17635 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-21 06:56:31.000000 easy_configer-2.0.0/easy_configer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 06:56:32.188588 easy_configer-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-04-21 05:53:21.000000 easy_configer-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 06:56:32.176076 easy_configer-2.0.0/test/
--rw-rw-rw-   0        0        0     3033 2023-04-21 05:47:25.000000 easy_configer-2.0.0/test/test_Configer.py
--rw-rw-rw-   0        0        0     1294 2023-04-21 05:47:25.000000 easy_configer-2.0.0/test/test_IO_Converter.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.953714 easy_configer-2.1.0/
+-rw-rw-rw-   0        0        0    17635 2023-06-06 09:32:55.953714 easy_configer-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13903 2023-04-21 05:47:34.000000 easy_configer-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.941154 easy_configer-2.1.0/easy_configer/
+-rw-rw-rw-   0        0        0     1456 2023-04-21 05:47:25.000000 easy_configer-2.1.0/easy_configer/Argparser.py
+-rw-rw-rw-   0        0        0     9359 2023-06-06 09:06:37.000000 easy_configer-2.1.0/easy_configer/Configer.py
+-rw-rw-rw-   0        0        0     2023 2023-06-01 10:10:43.000000 easy_configer-2.1.0/easy_configer/IO_Converter.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.949722 easy_configer-2.1.0/easy_configer/utils/
+-rw-rw-rw-   0        0        0      807 2023-04-21 05:47:25.000000 easy_configer-2.1.0/easy_configer/utils/Flag.py
+-rw-rw-rw-   0        0        0     4189 2023-06-06 09:28:09.000000 easy_configer-2.1.0/easy_configer/utils/Type_Convertor.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.947165 easy_configer-2.1.0/easy_configer.egg-info/
+-rw-rw-rw-   0        0        0    17635 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:32:55.954713 easy_configer-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-06-06 09:32:08.000000 easy_configer-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.951721 easy_configer-2.1.0/test/
+-rw-rw-rw-   0        0        0     3033 2023-04-21 05:47:25.000000 easy_configer-2.1.0/test/test_Configer.py
+-rw-rw-rw-   0        0        0     1294 2023-04-21 05:47:25.000000 easy_configer-2.1.0/test/test_IO_Converter.py
```

### Comparing `easy_configer-2.0.0/PKG-INFO` & `easy_configer-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_configer
-Version: 2.0.0
+Version: 2.1.0
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Description: # Project description
         #### easy_configer version : 2.0.1
```

### Comparing `easy_configer-2.0.0/README.md` & `easy_configer-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easy_configer-2.0.0/easy_configer/Argparser.py` & `easy_configer-2.1.0/easy_configer/Argparser.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.0.0/easy_configer/Configer.py` & `easy_configer-2.1.0/easy_configer/Configer.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.0.0/easy_configer/IO_Converter.py` & `easy_configer-2.1.0/easy_configer/IO_Converter.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.0.0/easy_configer/utils/Flag.py` & `easy_configer-2.1.0/easy_configer/utils/Flag.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.0.0/easy_configer.egg-info/PKG-INFO` & `easy_configer-2.1.0/easy_configer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-configer
-Version: 2.0.0
+Version: 2.1.0
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Description: # Project description
         #### easy_configer version : 2.0.1
```

### Comparing `easy_configer-2.0.0/setup.py` & `easy_configer-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # read the contents of your README file
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easy_configer',
-    version='2.0.0',
+    version='2.1.0',
     description='An easy way for configurating python program by the given config file or config str',
     author='JosefHuang',
     author_email='a3285556aa@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/HuangChiEn/easy_config',
```

### Comparing `easy_configer-2.0.0/test/test_Configer.py` & `easy_configer-2.1.0/test/test_Configer.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.0.0/test/test_IO_Converter.py` & `easy_configer-2.1.0/test/test_IO_Converter.py`

 * *Files identical despite different names*

