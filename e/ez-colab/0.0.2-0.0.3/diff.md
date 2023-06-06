# Comparing `tmp/ez-colab-0.0.2.tar.gz` & `tmp/ez-colab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-colab-0.0.2.tar", last modified: Wed May 31 03:44:08 2023, max compression
+gzip compressed data, was "ez-colab-0.0.3.tar", last modified: Tue Jun  6 19:19:36 2023, max compression
```

## Comparing `ez-colab-0.0.2.tar` & `ez-colab-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 03:44:08.925681 ez-colab-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-31 02:33:01.000000 ez-colab-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2128 2023-05-31 03:44:08.925681 ez-colab-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1326 2023-05-31 03:42:56.000000 ez-colab-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 03:44:08.925681 ez-colab-0.0.2/ez_colab.egg-info/
--rw-rw-rw-   0        0        0     2128 2023-05-31 03:44:08.000000 ez-colab-0.0.2/ez_colab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-31 03:44:08.000000 ez-colab-0.0.2/ez_colab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:44:08.000000 ez-colab-0.0.2/ez_colab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:44:08.000000 ez-colab-0.0.2/ez_colab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 03:44:08.929627 ez-colab-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-05-31 03:43:57.000000 ez-colab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:19:36.328701 ez-colab-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-31 02:33:01.000000 ez-colab-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2130 2023-06-06 19:19:36.328701 ez-colab-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1328 2023-05-31 03:45:29.000000 ez-colab-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 19:19:36.328701 ez-colab-0.0.3/ez_colab.egg-info/
+-rw-rw-rw-   0        0        0     2130 2023-06-06 19:19:36.000000 ez-colab-0.0.3/ez_colab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-06-06 19:19:36.000000 ez-colab-0.0.3/ez_colab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:19:36.000000 ez-colab-0.0.3/ez_colab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:19:36.000000 ez-colab-0.0.3/ez_colab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:19:36.328701 ez-colab-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-06-06 19:12:53.000000 ez-colab-0.0.3/setup.py
```

### Comparing `ez-colab-0.0.2/LICENSE.txt` & `ez-colab-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-colab-0.0.2/PKG-INFO` & `ez-colab-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-colab
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package that helps you manage files in Google Colab notebooks.
 Home-page: https://github.com/pratik-tan10/ez-colab
 Author: Pratik Dhungana
 Author-email: pdhungana@crimson.ua.edu
 Keywords: python,ez-colab,colab
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 - `finish_work(output_zip_file_name)`: This function zips all the files in the current working directory and downloads the zip file with the given name.
 - `clear_directory()`: This function deletes all the files and folders in the current working directory, effectively resetting the working directory.
 
 ## Installation
 
 You can install ez-colab using pip:
 
-!pip install ez-colab
+`!pip install ez-colab`
 
 
 ## Usage
 
 To use ez-colab, you need to import it in your notebook:
 
 `import easy_colab as ec`
```

### Comparing `ez-colab-0.0.2/README.md` & `ez-colab-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - `finish_work(output_zip_file_name)`: This function zips all the files in the current working directory and downloads the zip file with the given name.
 - `clear_directory()`: This function deletes all the files and folders in the current working directory, effectively resetting the working directory.
 
 ## Installation
 
 You can install ez-colab using pip:
 
-!pip install ez-colab
+`!pip install ez-colab`
 
 
 ## Usage
 
 To use ez-colab, you need to import it in your notebook:
 
 `import easy_colab as ec`
```

### Comparing `ez-colab-0.0.2/ez_colab.egg-info/PKG-INFO` & `ez-colab-0.0.3/ez_colab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-colab
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package that helps you manage files in Google Colab notebooks.
 Home-page: https://github.com/pratik-tan10/ez-colab
 Author: Pratik Dhungana
 Author-email: pdhungana@crimson.ua.edu
 Keywords: python,ez-colab,colab
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 - `finish_work(output_zip_file_name)`: This function zips all the files in the current working directory and downloads the zip file with the given name.
 - `clear_directory()`: This function deletes all the files and folders in the current working directory, effectively resetting the working directory.
 
 ## Installation
 
 You can install ez-colab using pip:
 
-!pip install ez-colab
+`!pip install ez-colab`
 
 
 ## Usage
 
 To use ez-colab, you need to import it in your notebook:
 
 `import easy_colab as ec`
```

### Comparing `ez-colab-0.0.2/setup.py` & `ez-colab-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as rd:
   long_description = rd.read()
 
 setup(
  name='ez-colab',
- version='0.0.2',
+ version='0.0.3',
  description='A python package that helps you manage files in Google Colab notebooks.',
  url='https://github.com/pratik-tan10/ez-colab', 
  author='Pratik Dhungana',
  author_email='pdhungana@crimson.ua.edu',
  classifiers=[
    'Development Status :: 4 - Beta',
    'Intended Audience :: Developers',
```

