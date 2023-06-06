# Comparing `tmp/YMS-0.99.tar.gz` & `tmp/YMS-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.99.tar", last modified: Thu May 25 12:33:19 2023, max compression
+gzip compressed data, was "YMS-1.0.0.tar", last modified: Tue Jun  6 09:17:56 2023, max compression
```

## Comparing `YMS-0.99.tar` & `YMS-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-25 12:33:19.842944 YMS-0.99/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-25 12:33:19.842944 YMS-0.99/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.99/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-25 12:33:19.842944 YMS-0.99/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-25 12:33:19.000000 YMS-0.99/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-25 12:33:19.000000 YMS-0.99/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-25 12:33:19.000000 YMS-0.99/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-25 12:33:19.000000 YMS-0.99/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-25 12:33:19.000000 YMS-0.99/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-25 12:33:19.000000 YMS-0.99/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-25 12:33:19.842944 YMS-0.99/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-25 12:32:42.000000 YMS-0.99/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-25 12:33:19.842944 YMS-0.99/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.99/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.99/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11707 2023-05-25 11:51:37.000000 YMS-0.99/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.99/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.99/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.99/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-06-06 09:17:56.349099 YMS-1.0.0/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2759 2023-06-06 09:17:56.349099 YMS-1.0.0/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2561 2023-06-06 08:58:43.000000 YMS-1.0.0/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-06-06 09:17:56.349099 YMS-1.0.0/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2759 2023-06-06 09:17:56.000000 YMS-1.0.0/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-06-06 09:17:56.000000 YMS-1.0.0/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-06-06 09:17:56.000000 YMS-1.0.0/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-06-06 09:17:56.000000 YMS-1.0.0/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-06-06 09:17:56.000000 YMS-1.0.0/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-06-06 09:17:56.000000 YMS-1.0.0/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-06-06 09:17:56.349099 YMS-1.0.0/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      693 2023-06-06 09:17:44.000000 YMS-1.0.0/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-06-06 09:17:56.349099 YMS-1.0.0/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-1.0.0/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-1.0.0/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11707 2023-05-25 11:51:37.000000 YMS-1.0.0/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-1.0.0/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-1.0.0/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-1.0.0/yamas/utilities.py
```

### Comparing `YMS-0.99/README.md` & `YMS-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 # YaMAS (YOLO Microbiome Analysis System)
 
 YaMAS is a package designed to easily download DNA datasets from the NCBI SRA website. It is developed by the [YOLO lab team](https://yolo.math.biu.ac.il), and is designed to be simple, efficient, and easy to use for non-programmers.
 
+## Dependencies
+Before proceeding with the installation and execution of YaMAS, please ensure that you have a clean environment set up on your system, with all dependencies installed. To create one, follow the steps below:
+1. Create a new [qiime2](https://docs.qiime2.org/2023.2/install/native/) environment using [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html). Make sure you name it 'qiime2'.
+2. Download the [SRA-toolkit](https://github.com/ncbi/sra-tools/wiki/02.-Installing-SRA-Toolkit) and [Entrez](http://bioconda.github.io/recipes/entrez-direct/README.html) packages to the environment.
+3. Download the [metaphlan](https://github.com/biobakery/biobakery/wiki/metaphlan4) package. Make sure the database works properly before proceeding.
+4. Exporting a 16S project requires a downloaded [classifier file](https://data.qiime2.org/2022.8/common/gg-13-8-99-nb-classifier.qza). 
+
+You are now ready to run and install YaMAS in the newly created and activated qiime2 environment.
 ## Installation
 
 To install YaMAS, you can use pip:
 
 ```
 pip install yamas
 ```
 
-## Dependencies
-Before proceeding with the installation and execution of YaMAS, please ensure that you have a clean environment set up on your system, with all dependencies installed. To create one, follow the steps below:
-1. create a new [qiime2](https://docs.qiime2.org/2023.2/install/native/) environment using [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html). Make sure you name it 'qiime2'.
-2. download the [SRA-toolkit](https://github.com/ncbi/sra-tools/wiki/02.-Installing-SRA-Toolkit) and [Entrez](http://bioconda.github.io/recipes/entrez-direct/README.html) packages to the environment.
-3. Exporting a project requires a downloaded [classifier file](https://data.qiime2.org/2022.8/common/gg-13-8-99-nb-classifier.qza).
-
-You are now ready to run and install YaMAS in the newly created and activated qiime2 environment.
 ## Getting Started
 
 YaMAS provides an easy-to-use interface in the terminal.
-
-To download a project, use the following command:
+To download a project, use the one of the following templates:
+### 16S dataset
 ```
-yamas --download PRJEB01234
+yamas --download PRJEB01234 --type 16S 
 ```
-Listing more than one project will download them one by one into different folders.
-
 To export an OTU (Operational Taxonomic Unit), taxonomy, and phylogeny tree for a single project, use the following command:
 ```
 yamas --export <project_path> <trim> <trunc> <classifier_file> <threads>
 ```
 Arguments:
 - project_path: path to the project directory (created by YaMAS in the previous step).
 - classifier_file: path to the trained classifier file. 
 - trim & trunc: choose graph edges. 
 - threads: specifies the number of threads to use for parallel processing, which can speed up the export process (default is 12).
 
+### Shotgun dataset
+```
+    yamas --download PRJEB01234 --type Shotgun 
+```
+
+### Other arguments and configurations
+1. config: You can add a configuration file in order to save the data in a different folder, and change other configurations. 
+2. verbose: To get more information about a downloading process, use the verbose option (this is highly recommended).
+3. Listing more than one project will download them one by one into different folders.
```

### Comparing `YMS-0.99/yamas/__init__.py` & `YMS-1.0.0/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.99/yamas/create_visualization.py` & `YMS-1.0.0/yamas/create_visualization.py`

 * *Files identical despite different names*

### Comparing `YMS-0.99/yamas/dataset_downloading.py` & `YMS-1.0.0/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.99/yamas/export_data.py` & `YMS-1.0.0/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.99/yamas/utilities.py` & `YMS-1.0.0/yamas/utilities.py`

 * *Files identical despite different names*

