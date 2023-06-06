# Comparing `tmp/ppocrlabel-japan-0.0.1.tar.gz` & `tmp/ppocrlabel-japan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppocrlabel-japan-0.0.1.tar", last modified: Tue Jun  6 04:45:03 2023, max compression
+gzip compressed data, was "ppocrlabel-japan-0.0.2.tar", last modified: Tue Jun  6 05:08:04 2023, max compression
```

## Comparing `ppocrlabel-japan-0.0.1.tar` & `ppocrlabel-japan-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 04:45:03.475401 ppocrlabel-japan-0.0.1/
--rw-rw-rw-   0        0        0    20484 2023-06-06 04:45:03.476400 ppocrlabel-japan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0   120562 2023-06-06 04:21:28.000000 ppocrlabel-japan-0.0.1/PPOCRLabel.py
-drwxrwxrwx   0        0        0        0 2023-06-06 04:45:03.472403 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/
--rw-rw-rw-   0        0        0    20484 2023-06-06 04:45:03.000000 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2023-06-06 04:45:03.000000 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 04:45:03.000000 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-06 04:45:03.000000 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-06 04:45:03.000000 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 04:45:03.000000 ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16874 2023-06-06 03:37:01.000000 ppocrlabel-japan-0.0.1/README.md
--rw-rw-rw-   0        0        0        0 2023-06-06 03:37:01.000000 ppocrlabel-japan-0.0.1/__init__.py
--rw-rw-rw-   0        0        0     6137 2023-06-06 03:37:01.000000 ppocrlabel-japan-0.0.1/gen_ocr_train_val_test.py
--rw-rw-rw-   0        0        0      149 2023-06-06 04:45:03.482402 ppocrlabel-japan-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2321 2023-06-06 04:44:54.000000 ppocrlabel-japan-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:08:04.355722 ppocrlabel-japan-0.0.2/
+-rw-rw-rw-   0        0        0    20484 2023-06-06 05:08:04.356692 ppocrlabel-japan-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0   120555 2023-06-06 05:06:11.000000 ppocrlabel-japan-0.0.2/PPOCRLabel.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:08:04.353717 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/
+-rw-rw-rw-   0        0        0    20484 2023-06-06 05:08:04.000000 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-06-06 05:08:04.000000 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:08:04.000000 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-06 05:08:04.000000 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-06 05:08:04.000000 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 05:08:04.000000 ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16874 2023-06-06 03:37:01.000000 ppocrlabel-japan-0.0.2/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-06 03:37:01.000000 ppocrlabel-japan-0.0.2/__init__.py
+-rw-rw-rw-   0        0        0     6137 2023-06-06 03:37:01.000000 ppocrlabel-japan-0.0.2/gen_ocr_train_val_test.py
+-rw-rw-rw-   0        0        0      149 2023-06-06 05:08:04.362698 ppocrlabel-japan-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2321 2023-06-06 05:04:49.000000 ppocrlabel-japan-0.0.2/setup.py
```

### Comparing `ppocrlabel-japan-0.0.1/PKG-INFO` & `ppocrlabel-japan-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppocrlabel-japan
-Version: 0.0.1
+Version: 0.0.2
 Summary: PPOCRLabelv2 is a semi-automatic graphic annotation tool suitable for OCR field, with built-in PP-OCR model to automatically detect and re-recognize data. It is written in Python3 and PyQT5, supporting rectangular box, table, irregular text and key information annotation modes. Annotations can be directly used for the training of PP-OCR detection and recognition models.
 Home-page: https://github.com/PaddlePaddle/PaddleOCR
 License: Apache License 2.0
 Download-URL: https://github.com/PaddlePaddle/PaddleOCR.git
 Description: English | [简体中文](README_ch.md)
         
         # PPOCRLabelv2
```

### Comparing `ppocrlabel-japan-0.0.1/PPOCRLabel.py` & `ppocrlabel-japan-0.0.2/PPOCRLabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 LABEL_COLORMAP = label_colormap()
 
 
 class MainWindow(QMainWindow):
     FIT_WINDOW, FIT_WIDTH, MANUAL_ZOOM = list(range(3))
 
     def __init__(self,
-                 lang="japan",
+                 lang="ch",
                  gpu=False,
-                 kie_mode=False,
+                 kie_mode=True,
                  default_filename=None,
                  default_predefined_class_file=None,
                  default_save_dir=None):
         super(MainWindow, self).__init__()
         self.setWindowTitle(__appname__)
         self.setWindowState(Qt.WindowMaximized)  # set window max
         self.activateWindow()  # PPOCRLabel goes to the front when activate
@@ -99,15 +99,15 @@
                              det=True,
                              cls=True,
                              use_gpu=gpu,
                              lang='japan',
                              show_log=False)
         self.table_ocr = PPStructure(use_pdserving=False,
                                      use_gpu=gpu,
-                                     lang='japan',
+                                     lang=lang,
                                      layout=False,
                                      show_log=False)
 
         if os.path.exists('./data/paddle.png'):
             result = self.ocr.ocr('./data/paddle.png', cls=True, det=True)
             result = self.table_ocr('./data/paddle.png', return_ocr_result_in_table=True)
```

### Comparing `ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/PKG-INFO` & `ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppocrlabel-japan
-Version: 0.0.1
+Version: 0.0.2
 Summary: PPOCRLabelv2 is a semi-automatic graphic annotation tool suitable for OCR field, with built-in PP-OCR model to automatically detect and re-recognize data. It is written in Python3 and PyQT5, supporting rectangular box, table, irregular text and key information annotation modes. Annotations can be directly used for the training of PP-OCR detection and recognition models.
 Home-page: https://github.com/PaddlePaddle/PaddleOCR
 License: Apache License 2.0
 Download-URL: https://github.com/PaddlePaddle/PaddleOCR.git
 Description: English | [简体中文](README_ch.md)
         
         # PPOCRLabelv2
```

### Comparing `ppocrlabel-japan-0.0.1/PPOCRLabel_Japan.egg-info/SOURCES.txt` & `ppocrlabel-japan-0.0.2/PPOCRLabel_Japan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppocrlabel-japan-0.0.1/README.md` & `ppocrlabel-japan-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ppocrlabel-japan-0.0.1/gen_ocr_train_val_test.py` & `ppocrlabel-japan-0.0.2/gen_ocr_train_val_test.py`

 * *Files identical despite different names*

### Comparing `ppocrlabel-japan-0.0.1/setup.py` & `ppocrlabel-japan-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 setup(
     name='ppocrlabel-japan',
     packages=['PPOCRLabel'],
     package_data = {'PPOCRLabel': ['libs/*','resources/strings/*','resources/icons/*']},
     package_dir={'PPOCRLabel': ''},
     include_package_data=True,
     entry_points={"console_scripts": ["PPOCRLabel= PPOCRLabel.PPOCRLabel:main"]},
-    version='0.0.1',
+    version='0.0.2',
     install_requires=requirements,
     license='Apache License 2.0',
     description='PPOCRLabelv2 is a semi-automatic graphic annotation tool suitable for OCR field, with built-in PP-OCR model to automatically detect and re-recognize data. It is written in Python3 and PyQT5, supporting rectangular box, table, irregular text and key information annotation modes. Annotations can be directly used for the training of PP-OCR detection and recognition models.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PaddlePaddle/PaddleOCR',
     download_url='https://github.com/PaddlePaddle/PaddleOCR.git',
```

