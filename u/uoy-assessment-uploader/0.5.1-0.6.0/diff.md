# Comparing `tmp/uoy_assessment_uploader-0.5.1.tar.gz` & `tmp/uoy_assessment_uploader-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy_assessment_uploader-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "uoy_assessment_uploader-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `uoy_assessment_uploader-0.5.1.tar` & `uoy_assessment_uploader-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    32422 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/LICENSE
--rw-r--r--   0        0        0     1399 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/README.md
--rw-r--r--   0        0        0      857 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/pyproject.toml
--rwxr-xr-x   0        0        0     7233 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     2535 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/argument_parser.py
--rw-r--r--   0        0        0     2320 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/credentials.py
--rw-r--r--   0        0        0     6032 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem
--rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 uoy_assessment_uploader-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-06-06 01:47:25.682649 uoy_assessment_uploader-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1630 2023-06-06 01:47:25.682649 uoy_assessment_uploader-0.6.0/README.md
+-rw-r--r--   0        0        0      946 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/pyproject.toml
+-rwxr-xr-x   0        0        0     5372 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     3369 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/argparse.py
+-rw-r--r--   0        0        0      587 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/constants.py
+-rw-r--r--   0        0        0     5149 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/credentials.py
+-rw-r--r--   0        0        0    11239 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/requests.py
+-rw-r--r--   0        0        0     6032 2023-06-06 01:47:25.686649 uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem
+-rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 uoy_assessment_uploader-0.6.0/PKG-INFO
```

### Comparing `uoy_assessment_uploader-0.5.1/LICENSE` & `uoy_assessment_uploader-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy_assessment_uploader-0.5.1/README.md` & `uoy_assessment_uploader-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 **If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
 
 ## Install
 1. When you have Python and Pip ready, it's as easy as:
    ```shell
    python -m pip install "uoy-assessment-uploader"
    ```
-   - or, directly from the repo:
-      ```shell
-      python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
-      ```
 2. As shrimple as that
 
+### Alternative install
+- You can also install it directly from the repo with pip:
+    ```shell
+    python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader.git"
+    ```
+
+- Or on an alpm (Arch) Linux system you can get it from the AUR at https://aur.archlinux.org/packages/uoy-assessment-uploader.
+    ```shell
+    paru uoy-assessment-uploader
+    ```
+
 ## Use
 Like this:
 - ```shell
   python -m uoy_assessment_uploader --help
   ```
   or
 - ```shell
```

### Comparing `uoy_assessment_uploader-0.5.1/pyproject.toml` & `uoy_assessment_uploader-0.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,13 @@
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/joelsgp/uoy-assessment-uploader"
 
 [project.scripts]
 uoy-assessment-uploader = "uoy_assessment_uploader:main"
+
+[tool.isort]
+profile = "black"
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules"
```

### Comparing `uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem` & `uoy_assessment_uploader-0.6.0/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem`

 * *Files identical despite different names*

### Comparing `uoy_assessment_uploader-0.5.1/PKG-INFO` & `uoy_assessment_uploader-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.5.1
+Version: 0.6.0
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -24,20 +24,27 @@
 **If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
 
 ## Install
 1. When you have Python and Pip ready, it's as easy as:
    ```shell
    python -m pip install "uoy-assessment-uploader"
    ```
-   - or, directly from the repo:
-      ```shell
-      python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
-      ```
 2. As shrimple as that
 
+### Alternative install
+- You can also install it directly from the repo with pip:
+    ```shell
+    python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader.git"
+    ```
+
+- Or on an alpm (Arch) Linux system you can get it from the AUR at https://aur.archlinux.org/packages/uoy-assessment-uploader.
+    ```shell
+    paru uoy-assessment-uploader
+    ```
+
 ## Use
 Like this:
 - ```shell
   python -m uoy_assessment_uploader --help
   ```
   or
 - ```shell
```

