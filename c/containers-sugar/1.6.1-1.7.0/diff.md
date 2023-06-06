# Comparing `tmp/containers_sugar-1.6.1.tar.gz` & `tmp/containers_sugar-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "containers_sugar-1.6.1.tar", max compression
+gzip compressed data, was "containers_sugar-1.7.0.tar", max compression
```

## Comparing `containers_sugar-1.6.1.tar` & `containers_sugar-1.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      897 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.containers-sugar.yaml
--rw-r--r--   0        0        0       88 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      327 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1395 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1760 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1889 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1799 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.gitignore
--rw-r--r--   0        0        0     1106 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1887 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/.releaserc.json
--rw-r--r--   0        0        0     1514 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/LICENSE
--rw-r--r--   0        0        0     4340 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/Makefile
--rw-r--r--   0        0        0     3416 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/README.md
--rw-r--r--   0        0        0      197 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/conda/dev.yaml
--rw-r--r--   0        0        0      216 2023-06-05 22:22:33.691911 containers_sugar-1.6.1/containers_sugar/__init__.py
--rw-r--r--   0        0        0       75 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/__main__.py
--rw-r--r--   0        0        0     4254 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/cli.py
--rw-r--r--   0        0        0       23 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/errors.py
--rw-r--r--   0        0        0    13847 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/containers_sugar/sugar.py
--rw-r--r--   0        0        0     6707 2023-06-05 22:22:33.703911 containers_sugar-1.6.1/docs/changelog.md
--rw-r--r--   0        0        0     5038 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/contributing.md
--rw-r--r--   0        0        0      956 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-06-05 22:18:59.440073 containers_sugar-1.6.1/docs/images/logo.png
--rw-r--r--   0        0        0      352 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/docs/index.md
--rw-r--r--   0        0        0     1000 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/docs/installation.md
--rw-r--r--   0        0        0     3908 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/docs/mkdocs.yaml
--rw-r--r--   0        0        0   139563 2023-06-05 22:18:59.444073 containers_sugar-1.6.1/poetry.lock
--rw-r--r--   0        0        0     1555 2023-06-05 22:22:33.691911 containers_sugar-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 containers_sugar-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      965 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.containers-sugar.yaml
+-rw-r--r--   0        0        0       88 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      327 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1395 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1704 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1889 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1799 2023-06-06 19:04:05.821493 containers_sugar-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1106 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1887 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/.releaserc.json
+-rw-r--r--   0        0        0     1514 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/LICENSE
+-rw-r--r--   0        0        0     4393 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/Makefile
+-rw-r--r--   0        0        0     3474 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/README.md
+-rw-r--r--   0        0        0      197 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/conda/dev.yaml
+-rw-r--r--   0        0        0      216 2023-06-06 19:07:11.059737 containers_sugar-1.7.0/containers_sugar/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/containers_sugar/__main__.py
+-rw-r--r--   0        0        0     4254 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/containers_sugar/cli.py
+-rw-r--r--   0        0        0      751 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/containers_sugar/logs.py
+-rw-r--r--   0        0        0    16076 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/containers_sugar/sugar.py
+-rw-r--r--   0        0        0     7065 2023-06-06 19:07:11.071737 containers_sugar-1.7.0/docs/changelog.md
+-rw-r--r--   0        0        0     5038 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/contributing.md
+-rw-r--r--   0        0        0      956 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/images/logo.png
+-rw-r--r--   0        0        0      352 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/index.md
+-rw-r--r--   0        0        0     1000 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/installation.md
+-rw-r--r--   0        0        0     3908 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/docs/mkdocs.yaml
+-rw-r--r--   0        0        0   140069 2023-06-06 19:04:05.825493 containers_sugar-1.7.0/poetry.lock
+-rw-r--r--   0        0        0     1581 2023-06-06 19:07:11.059737 containers_sugar-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 containers_sugar-1.7.0/PKG-INFO
```

### Comparing `containers_sugar-1.6.1/.containers-sugar.yaml` & `containers_sugar-1.7.0/.containers-sugar.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-version: 1.0.0
+version: 1.0
 compose-app: docker-compose
+env-file: .env
+defaults:
+  group: {{ env.KXGR_GROUP }}
 service-groups:
   - name: group1
     project-name: project1  # optional
     compose-path: tests/containers/group1/compose.yaml
     env-file: .env
     services:
       default: service1-1,service1-3
-      list:
+      available:
         - name: service1-1
         - name: service1-2
         - name: service1-3
 
   - name: group2
     project-name: null  # optional
     compose-path: tests/containers/group2/compose.yaml
     env-file: .env
     services:
       default: null
-      list:
+      available:
         - name: service2-1
         - name: service2-2
 
   - name: group-mix
     project-name: null  # optional
     compose-path:
       - tests/containers/group1/compose.yaml
       - tests/containers/group2/compose.yaml
     env-file: .env
     services:
       default: null
-      list:
+      available:
         - name: service1-1
         - name: service1-2
         - name: service2-1
         - name: service2-2
```

### Comparing `containers_sugar-1.6.1/.github/PULL_REQUEST_TEMPLATE.md` & `containers_sugar-1.7.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/.github/workflows/main.yaml` & `containers_sugar-1.7.0/.github/workflows/main.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     - uses: actions/checkout@v3
 
     - name: Prepare conda environment
       run: |
         sed -i s/python\ 3\.8\.1/python\ ${{ matrix.python_version }}/ conda/dev.yaml
         cat conda/dev.yaml
 
-    - name: create a dotenv file
-      run: touch .env
-
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniconda-version: "latest"
         environment-file: conda/dev.yaml
         channels: conda-forge,nodefaults
         activate-environment: containers-sugar
         use-mamba: true
```

### Comparing `containers_sugar-1.6.1/.github/workflows/release.yaml` & `containers_sugar-1.7.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/.gitignore` & `containers_sugar-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/.pre-commit-config.yaml` & `containers_sugar-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/.releaserc.json` & `containers_sugar-1.7.0/.releaserc.json`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/LICENSE` & `containers_sugar-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/Makefile` & `containers_sugar-1.7.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 
 .ONESHELL:
 .PHONY: smoke-tests
 smoke-tests:
 	# note: don't change the order of the commands heres
 
 	set -ex
+
+	# test default group option
+	kxgr build --verbose
+
 	# group 1
 	kxgr --help
 	kxgr --version
 	kxgr build --verbose --group group1 --all
 	kxgr build --verbose --group group1
 	kxgr build --verbose --group group1 --services service1-1
 	kxgr pull --verbose --group group1 --all
```

### Comparing `containers_sugar-1.6.1/README.md` & `containers_sugar-1.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -68,41 +68,40 @@
 
 ## How to use it
 
 First you need to place the config file `.containers-sugar.yaml` in the root
 of your project. This is an example of a configuration file:
 
 ```yaml
-version: 1.0.0
+version: 1.0
 compose-app: docker-compose
+default:
+  group: {{ env.ENV }}
 service-groups:
   - name: group1
-    project-name: project1  # optional
+    project-name: project1
     compose-path: containers/tests/group1/compose.yaml
     env-file: .env
     services:
-      default: service1,service3
-      list:
+      default:
+        - service1
+        - service3
+      available:
         - name: service1
-          health-check: true
         - name: service2
-          health-check: false
         - name: service3
-          health-check: true
   - name: group2
-    project-name: null  # optional
+    project-name: null
     compose-path: containers/tests/group2/compose.yaml
     env-file: .env
     services:
-      default: null
-      list:
+      # default: null
+      available:
         - name: service1
-          health-check: true
         - name: service1
-          health-check: false
 ```
 
 **NOTE**: containers-sugar has an convenient alias `kxgr` that helps to
 keep the command line shorter, where **k** stands for *containers*,
 **x** stands for *su* (*shu* sound), and **gr** stands for *gar*.
 In another words, you can use `containers-sugar` or `kxgr` CLI.
 
@@ -121,7 +120,12 @@
   `kxgr ext start --group group1`
 
 * restart all services (ignore defaults) for group1:
   `kxgr ext restart --group group1 --all`
 
 * restart service1 and service2 for group1:
   `kxgr ext restart --group group1 --services service1,service2`
+
+
+**NOTE**: If you use: ```default: group: {{ env.ENV }}```, you don't need to
+give `--group <GROUP_NAME>`, except if you want a different group than the
+default one.
```

### Comparing `containers_sugar-1.6.1/containers_sugar/cli.py` & `containers_sugar-1.7.0/containers_sugar/cli.py`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/docs/changelog.md` & `containers_sugar-1.7.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Release Notes
 ---
 
+# [1.7.0](https://github.com/osl-incubator/containers-sugar/compare/1.6.1...1.7.0) (2023-06-06)
+
+
+### Features
+
+* Add support for default option configuration for group service ([#80](https://github.com/osl-incubator/containers-sugar/issues/80)) ([0045a4a](https://github.com/osl-incubator/containers-sugar/commit/0045a4aabcb6106f6ba145fa1edfd12e3fc5cb6a))
+
 ## [1.6.1](https://github.com/osl-incubator/containers-sugar/compare/1.6.0...1.6.1) (2023-06-05)
 
 
 ### Bug Fixes
 
 * **ext:** Fix restart and start ext commands ([#79](https://github.com/osl-incubator/containers-sugar/issues/79)) ([e9622c3](https://github.com/osl-incubator/containers-sugar/commit/e9622c3ac21e0e08de15263a82f77b3828aecaa9))
```

### Comparing `containers_sugar-1.6.1/docs/contributing.md` & `containers_sugar-1.7.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/docs/example.ipynb` & `containers_sugar-1.7.0/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/docs/images/favicon.ico` & `containers_sugar-1.7.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/docs/images/logo.png` & `containers_sugar-1.7.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/docs/installation.md` & `containers_sugar-1.7.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/docs/mkdocs.yaml` & `containers_sugar-1.7.0/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `containers_sugar-1.6.1/poetry.lock` & `containers_sugar-1.7.0/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 2320 5468 6973 2066 696c 6520 6973 2061  # This file is a
 00000010: 7574 6f6d 6174 6963 616c 6c79 2040 6765  utomatically @ge
 00000020: 6e65 7261 7465 6420 6279 2050 6f65 7472  nerated by Poetr
-00000030: 7920 312e 352e 3020 616e 6420 7368 6f75  y 1.5.0 and shou
+00000030: 7920 312e 352e 3120 616e 6420 7368 6f75  y 1.5.1 and shou
 00000040: 6c64 206e 6f74 2062 6520 6368 616e 6765  ld not be change
 00000050: 6420 6279 2068 616e 642e 0a0a 5b5b 7061  d by hand...[[pa
 00000060: 636b 6167 655d 5d0a 6e61 6d65 203d 2022  ckage]].name = "
 00000070: 6173 7079 2d79 616d 6c22 0a76 6572 7369  aspy-yaml".versi
 00000080: 6f6e 203d 2022 312e 332e 3022 0a64 6573  on = "1.3.0".des
 00000090: 6372 6970 7469 6f6e 203d 2022 4120 6665  cription = "A fe
 000000a0: 7720 6578 7465 6e73 696f 6e73 2074 6f20  w extensions to 
@@ -6369,2355 +6369,2387 @@
 00018e00: 3364 6333 3435 3365 6262 6335 3964 6264  3dc3453ebbc59dbd
 00018e10: 6561 3965 3465 3131 6335 3635 3135 3230  ea9e4e11c5651520
 00018e20: 6138 3736 6430 6634 6462 3136 3165 3836  a876d0f4db161e86
 00018e30: 3734 6161 6539 3335 6461 3922 7d2c 0a5d  74aae935da9"},.]
 00018e40: 0a0a 5b70 6163 6b61 6765 2e64 6570 656e  ..[package.depen
 00018e50: 6465 6e63 6965 735d 0a73 6978 203d 2022  dencies].six = "
 00018e60: 3e3d 312e 3522 0a0a 5b5b 7061 636b 6167  >=1.5"..[[packag
-00018e70: 655d 5d0a 6e61 6d65 203d 2022 7079 746b  e]].name = "pytk
-00018e80: 646f 6373 220a 7665 7273 696f 6e20 3d20  docs".version = 
-00018e90: 2230 2e31 362e 3122 0a64 6573 6372 6970  "0.16.1".descrip
-00018ea0: 7469 6f6e 203d 2022 4c6f 6164 2050 7974  tion = "Load Pyt
-00018eb0: 686f 6e20 6f62 6a65 6374 7320 646f 6375  hon objects docu
-00018ec0: 6d65 6e74 6174 696f 6e2e 220a 6f70 7469  mentation.".opti
-00018ed0: 6f6e 616c 203d 2066 616c 7365 0a70 7974  onal = false.pyt
-00018ee0: 686f 6e2d 7665 7273 696f 6e73 203d 2022  hon-versions = "
-00018ef0: 3e3d 332e 3722 0a66 696c 6573 203d 205b  >=3.7".files = [
-00018f00: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-00018f10: 746b 646f 6373 2d30 2e31 362e 312d 7079  tkdocs-0.16.1-py
-00018f20: 332d 6e6f 6e65 2d61 6e79 2e77 686c 222c  3-none-any.whl",
-00018f30: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-00018f40: 6138 6333 6634 3665 6365 6630 6239 3238  a8c3f46ecef0b928
-00018f50: 3634 6363 3539 3865 3931 3031 6539 6334  64cc598e9101e9c4
-00018f60: 6366 3833 3265 6262 6632 3238 6635 3063  cf832ebbf228f50c
-00018f70: 3834 6161 3564 6438 3530 6161 6333 3739  84aa5dd850aac379
-00018f80: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-00018f90: 2270 7974 6b64 6f63 732d 302e 3136 2e31  "pytkdocs-0.16.1
-00018fa0: 2e74 6172 2e67 7a22 2c20 6861 7368 203d  .tar.gz", hash =
-00018fb0: 2022 7368 6132 3536 3a65 3263 6366 3664   "sha256:e2ccf6d
-00018fc0: 6665 3964 6262 6365 6230 3938 3138 3637  fe9dbbceb0981867
-00018fd0: 3366 3034 3066 3161 3763 3332 6564 3062  3f040f1a7c32ed0b
-00018fe0: 6666 6232 6437 3039 6230 3662 6536 3435  ffb2d709b06be645
-00018ff0: 3363 3430 3236 3034 3522 7d2c 0a5d 0a0a  3c4026045"},.]..
-00019000: 5b70 6163 6b61 6765 2e64 6570 656e 6465  [package.depende
-00019010: 6e63 6965 735d 0a61 7374 756e 7061 7273  ncies].astunpars
-00019020: 6520 3d20 7b76 6572 7369 6f6e 203d 2022  e = {version = "
-00019030: 3e3d 312e 3622 2c20 6d61 726b 6572 7320  >=1.6", markers 
-00019040: 3d20 2270 7974 686f 6e5f 7665 7273 696f  = "python_versio
-00019050: 6e20 3c20 5c22 332e 395c 2222 7d0a 0a5b  n < \"3.9\""}..[
-00019060: 7061 636b 6167 652e 6578 7472 6173 5d0a  package.extras].
-00019070: 6e75 6d70 792d 7374 796c 6520 3d20 5b22  numpy-style = ["
-00019080: 646f 6373 7472 696e 675f 7061 7273 6572  docstring_parser
-00019090: 2028 3e3d 302e 3729 225d 0a0a 5b5b 7061   (>=0.7)"]..[[pa
-000190a0: 636b 6167 655d 5d0a 6e61 6d65 203d 2022  ckage]].name = "
-000190b0: 7079 7769 6e33 3222 0a76 6572 7369 6f6e  pywin32".version
-000190c0: 203d 2022 3330 3622 0a64 6573 6372 6970   = "306".descrip
-000190d0: 7469 6f6e 203d 2022 5079 7468 6f6e 2066  tion = "Python f
-000190e0: 6f72 2057 696e 646f 7720 4578 7465 6e73  or Window Extens
-000190f0: 696f 6e73 220a 6f70 7469 6f6e 616c 203d  ions".optional =
-00019100: 2066 616c 7365 0a70 7974 686f 6e2d 7665   false.python-ve
-00019110: 7273 696f 6e73 203d 2022 2a22 0a66 696c  rsions = "*".fil
-00019120: 6573 203d 205b 0a20 2020 207b 6669 6c65  es = [.    {file
-00019130: 203d 2022 7079 7769 6e33 322d 3330 362d   = "pywin32-306-
-00019140: 6370 3331 302d 6370 3331 302d 7769 6e33  cp310-cp310-win3
-00019150: 322e 7768 6c22 2c20 6861 7368 203d 2022  2.whl", hash = "
-00019160: 7368 6132 3536 3a30 3664 3334 3230 6135  sha256:06d3420a5
-00019170: 3135 3562 6136 3566 3062 3732 6632 3639  155ba65f0b72f269
-00019180: 3962 3562 6163 6633 3130 3966 3336 6163  9b5bacf3109f36ac
-00019190: 6265 3839 3233 3736 3563 3232 3933 3861  be8923765c22938a
-000191a0: 3639 6466 6338 6422 7d2c 0a20 2020 207b  69dfc8d"},.    {
-000191b0: 6669 6c65 203d 2022 7079 7769 6e33 322d  file = "pywin32-
-000191c0: 3330 362d 6370 3331 302d 6370 3331 302d  306-cp310-cp310-
-000191d0: 7769 6e5f 616d 6436 342e 7768 6c22 2c20  win_amd64.whl", 
-000191e0: 6861 7368 203d 2022 7368 6132 3536 3a38  hash = "sha256:8
-000191f0: 3466 3434 3731 6462 6361 3138 3837 6561  4f4471dbca1887ea
-00019200: 3338 3033 6438 3834 3861 3136 3136 3432  3803d8848a161642
-00019210: 3961 6339 3461 3461 3864 3035 6634 6263  9ac94a4a8d05f4bc
-00019220: 3963 3564 6366 6434 3263 6139 3963 3822  9c5dcfd42ca99c8"
-00019230: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-00019240: 7079 7769 6e33 322d 3330 362d 6370 3331  pywin32-306-cp31
-00019250: 312d 6370 3331 312d 7769 6e33 322e 7768  1-cp311-win32.wh
-00019260: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-00019270: 3536 3a65 3635 3032 3831 3333 6431 3562  56:e65028133d15b
-00019280: 3634 6432 6564 3866 3036 6464 3966 6263  64d2ed8f06dd9fbc
-00019290: 3236 3833 3532 3437 3864 3466 3932 3839  268352478d4f9289
-000192a0: 6536 3963 3139 3065 6364 3638 3138 6236  e69c190ecd6818b6
-000192b0: 3430 3722 7d2c 0a20 2020 207b 6669 6c65  407"},.    {file
-000192c0: 203d 2022 7079 7769 6e33 322d 3330 362d   = "pywin32-306-
-000192d0: 6370 3331 312d 6370 3331 312d 7769 6e5f  cp311-cp311-win_
-000192e0: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
-000192f0: 203d 2022 7368 6132 3536 3a61 3736 3339   = "sha256:a7639
-00019300: 6635 3163 3138 3463 3032 3732 6539 3366  f51c184c0272e93f
-00019310: 3234 3465 6232 3464 6166 6361 3962 3138  244eb24dafca9b18
-00019320: 3535 3730 3764 3934 6331 3932 6434 6130  55707d94c192d4a0
-00019330: 6234 6330 3165 3131 3030 6522 7d2c 0a20  b4c01e1100e"},. 
-00019340: 2020 207b 6669 6c65 203d 2022 7079 7769     {file = "pywi
-00019350: 6e33 322d 3330 362d 6370 3331 312d 6370  n32-306-cp311-cp
-00019360: 3331 312d 7769 6e5f 6172 6d36 342e 7768  311-win_arm64.wh
-00019370: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-00019380: 3536 3a37 3064 6261 3063 3931 3364 3139  56:70dba0c913d19
-00019390: 6639 3432 6132 6462 3235 3231 3764 3961  f942a2db25217d9a
-000193a0: 3162 3732 3663 3237 3866 3438 3361 3931  1b726c278f483a91
-000193b0: 3966 3161 6266 6564 3739 6339 6366 3634  9f1abfed79c9cf64
-000193c0: 6433 6122 7d2c 0a20 2020 207b 6669 6c65  d3a"},.    {file
-000193d0: 203d 2022 7079 7769 6e33 322d 3330 362d   = "pywin32-306-
-000193e0: 6370 3331 322d 6370 3331 322d 7769 6e33  cp312-cp312-win3
-000193f0: 322e 7768 6c22 2c20 6861 7368 203d 2022  2.whl", hash = "
-00019400: 7368 6132 3536 3a33 3833 3232 3964 3531  sha256:383229d51
-00019410: 3536 3537 6634 6533 6564 3133 3433 6461  5657f4e3ed1343da
-00019420: 3862 6531 3031 3030 3035 3632 6266 3531  8be101000562bf51
-00019430: 3435 3931 6666 3338 3361 6539 3430 6361  4591ff383ae940ca
-00019440: 6436 3534 3538 6222 7d2c 0a20 2020 207b  d65458b"},.    {
-00019450: 6669 6c65 203d 2022 7079 7769 6e33 322d  file = "pywin32-
-00019460: 3330 362d 6370 3331 322d 6370 3331 322d  306-cp312-cp312-
-00019470: 7769 6e5f 616d 6436 342e 7768 6c22 2c20  win_amd64.whl", 
-00019480: 6861 7368 203d 2022 7368 6132 3536 3a33  hash = "sha256:3
-00019490: 3732 3537 3739 3463 3161 6433 3965 6539  7257794c1ad39ee9
-000194a0: 6265 3635 3264 6130 3436 3264 6332 6533  be652da0462dc2e3
-000194b0: 3934 6338 3135 3964 6664 3931 3361 3861  94c8159dfd913a8a
-000194c0: 3465 3865 6236 6664 3334 3664 6130 6522  4e8eb6fd346da0e"
-000194d0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-000194e0: 7079 7769 6e33 322d 3330 362d 6370 3331  pywin32-306-cp31
-000194f0: 322d 6370 3331 322d 7769 6e5f 6172 6d36  2-cp312-win_arm6
-00019500: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-00019510: 7368 6132 3536 3a35 3832 3165 6335 3266  sha256:5821ec52f
-00019520: 3664 3332 3161 6135 3965 3264 6237 6530  6d321aa59e2db7e0
-00019530: 6133 3562 3939 3764 6536 3063 3230 3139  a35b997de60c2019
-00019540: 3433 3535 3764 3130 3861 6639 6434 6165  43557d108af9d4ae
-00019550: 3165 6337 3034 3022 7d2c 0a20 2020 207b  1ec7040"},.    {
-00019560: 6669 6c65 203d 2022 7079 7769 6e33 322d  file = "pywin32-
-00019570: 3330 362d 6370 3337 2d63 7033 376d 2d77  306-cp37-cp37m-w
-00019580: 696e 3332 2e77 686c 222c 2068 6173 6820  in32.whl", hash 
-00019590: 3d20 2273 6861 3235 363a 3163 3733 6561  = "sha256:1c73ea
-000195a0: 3961 3064 3232 3833 6438 3839 3030 3139  9a0d2283d8890019
-000195b0: 3938 3035 3966 3565 6161 6261 3362 3632  98059f5eaaba3b62
-000195c0: 3338 6637 3637 6339 6366 3238 3333 6231  38f767c9cf2833b1
-000195d0: 3365 3661 3638 3566 3635 227d 2c0a 2020  3e6a685f65"},.  
-000195e0: 2020 7b66 696c 6520 3d20 2270 7977 696e    {file = "pywin
-000195f0: 3332 2d33 3036 2d63 7033 372d 6370 3337  32-306-cp37-cp37
-00019600: 6d2d 7769 6e5f 616d 6436 342e 7768 6c22  m-win_amd64.whl"
-00019610: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00019620: 3a37 3263 3566 3632 3135 3432 6437 6264  :72c5f621542d7bd
-00019630: 6434 6664 6237 3136 3232 3762 6530 6464  d4fdb716227be0dd
-00019640: 3366 3835 3635 6331 3162 3238 3062 6536  3f8565c11b280be6
-00019650: 3331 3562 3036 6163 6533 3534 3837 6433  315b06ace35487d3
-00019660: 3622 7d2c 0a20 2020 207b 6669 6c65 203d  6"},.    {file =
-00019670: 2022 7079 7769 6e33 322d 3330 362d 6370   "pywin32-306-cp
-00019680: 3338 2d63 7033 382d 7769 6e33 322e 7768  38-cp38-win32.wh
-00019690: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-000196a0: 3536 3a65 3463 3039 3265 3235 3839 6235  56:e4c092e2589b5
-000196b0: 6366 3064 3336 3538 3439 6537 3365 3032  cf0d365849e73e02
-000196c0: 6333 3931 6331 3334 3939 3538 6335 6163  c391c1349958c5ac
-000196d0: 3365 3964 3563 6362 3961 3238 6530 3137  3e9d5ccb9a28e017
-000196e0: 6233 6122 7d2c 0a20 2020 207b 6669 6c65  b3a"},.    {file
-000196f0: 203d 2022 7079 7769 6e33 322d 3330 362d   = "pywin32-306-
-00019700: 6370 3338 2d63 7033 382d 7769 6e5f 616d  cp38-cp38-win_am
-00019710: 6436 342e 7768 6c22 2c20 6861 7368 203d  d64.whl", hash =
-00019720: 2022 7368 6132 3536 3a65 3861 6331 6165   "sha256:e8ac1ae
-00019730: 3336 3031 6265 6536 6361 3966 3763 6234  3601bee6ca9f7cb4
-00019740: 6235 3336 3362 6631 6330 6261 6462 3933  b5363bf1c0badb93
-00019750: 3565 6632 3433 6334 3733 3366 6639 6133  5ef243c4733ff9a3
-00019760: 3933 6231 3639 3063 3022 7d2c 0a20 2020  93b1690c0"},.   
-00019770: 207b 6669 6c65 203d 2022 7079 7769 6e33   {file = "pywin3
-00019780: 322d 3330 362d 6370 3339 2d63 7033 392d  2-306-cp39-cp39-
-00019790: 7769 6e33 322e 7768 6c22 2c20 6861 7368  win32.whl", hash
-000197a0: 203d 2022 7368 6132 3536 3a65 3235 6664   = "sha256:e25fd
-000197b0: 3562 3438 3562 3535 6163 3963 3035 3766  5b485b55ac9c057f
-000197c0: 3637 6439 3462 6332 3033 6633 6636 3539  67d94bc203f3f659
-000197d0: 3530 3738 6431 6662 3362 3435 3863 3963  5078d1fb3b458c9c
-000197e0: 3238 6237 3135 3361 3830 3222 7d2c 0a20  28b7153a802"},. 
-000197f0: 2020 207b 6669 6c65 203d 2022 7079 7769     {file = "pywi
-00019800: 6e33 322d 3330 362d 6370 3339 2d63 7033  n32-306-cp39-cp3
-00019810: 392d 7769 6e5f 616d 6436 342e 7768 6c22  9-win_amd64.whl"
-00019820: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00019830: 3a33 3962 3631 6331 3532 3732 3833 3362  :39b61c15272833b
-00019840: 3563 3332 3961 3239 3839 3939 3964 6361  5c329a2989999dca
-00019850: 6538 3336 6231 6565 6436 3530 3235 3261  e836b1eed650252a
-00019860: 6231 6237 6266 6265 3164 3539 6633 3066  b1b7bfbe1d59f30f
-00019870: 3422 7d2c 0a5d 0a0a 5b5b 7061 636b 6167  4"},.]..[[packag
-00019880: 655d 5d0a 6e61 6d65 203d 2022 7079 7961  e]].name = "pyya
-00019890: 6d6c 220a 7665 7273 696f 6e20 3d20 2236  ml".version = "6
-000198a0: 2e30 220a 6465 7363 7269 7074 696f 6e20  .0".description 
-000198b0: 3d20 2259 414d 4c20 7061 7273 6572 2061  = "YAML parser a
-000198c0: 6e64 2065 6d69 7474 6572 2066 6f72 2050  nd emitter for P
-000198d0: 7974 686f 6e22 0a6f 7074 696f 6e61 6c20  ython".optional 
-000198e0: 3d20 6661 6c73 650a 7079 7468 6f6e 2d76  = false.python-v
-000198f0: 6572 7369 6f6e 7320 3d20 223e 3d33 2e36  ersions = ">=3.6
-00019900: 220a 6669 6c65 7320 3d20 5b0a 2020 2020  ".files = [.    
-00019910: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
-00019920: 362e 302d 6370 3331 302d 6370 3331 302d  6.0-cp310-cp310-
-00019930: 6d61 636f 7378 5f31 305f 395f 7838 365f  macosx_10_9_x86_
-00019940: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-00019950: 2273 6861 3235 363a 6434 6462 3763 3761  "sha256:d4db7c7a
-00019960: 6566 3038 3538 3732 6566 3635 6138 6664  ef085872ef65a8fd
-00019970: 3764 3664 3039 6131 3461 6539 3166 3639  7d6d09a14ae91f69
-00019980: 3164 6563 3365 3837 6565 3565 6530 3533  1dec3e87ee5ee053
-00019990: 3964 3531 3666 3533 227d 2c0a 2020 2020  9d516f53"},.    
-000199a0: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
-000199b0: 362e 302d 6370 3331 302d 6370 3331 302d  6.0-cp310-cp310-
-000199c0: 6d61 636f 7378 5f31 315f 305f 6172 6d36  macosx_11_0_arm6
-000199d0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-000199e0: 7368 6132 3536 3a39 6466 3765 6433 6233  sha256:9df7ed3b3
-000199f0: 6432 6530 6563 6665 3039 6531 3437 3431  d2e0ecfe09e14741
-00019a00: 6238 3537 6466 3433 6164 6235 6133 6464  b857df43adb5a3dd
-00019a10: 6164 6339 3139 6132 6439 3466 6264 6637  adc919a2d94fbdf7
-00019a20: 3866 6561 3533 6322 7d2c 0a20 2020 207b  8fea53c"},.    {
-00019a30: 6669 6c65 203d 2022 5079 5941 4d4c 2d36  file = "PyYAML-6
-00019a40: 2e30 2d63 7033 3130 2d63 7033 3130 2d6d  .0-cp310-cp310-m
-00019a50: 616e 796c 696e 7578 5f32 5f31 375f 6161  anylinux_2_17_aa
-00019a60: 7263 6836 342e 6d61 6e79 6c69 6e75 7832  rch64.manylinux2
-00019a70: 3031 345f 6161 7263 6836 342e 7768 6c22  014_aarch64.whl"
-00019a80: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00019a90: 3a37 3766 3339 3665 3665 6634 6337 3366  :77f396e6ef4c73f
-00019aa0: 6463 3333 6139 3135 3734 3436 3436 3666  dc33a9157446466f
-00019ab0: 3163 6666 3535 3364 3937 3962 6430 3065  1cff553d979bd00e
-00019ac0: 6362 3634 3338 3537 3630 6336 6261 6264  cb64385760c6babd
-00019ad0: 6322 7d2c 0a20 2020 207b 6669 6c65 203d  c"},.    {file =
-00019ae0: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
-00019af0: 3130 2d63 7033 3130 2d6d 616e 796c 696e  10-cp310-manylin
-00019b00: 7578 5f32 5f31 375f 7333 3930 782e 6d61  ux_2_17_s390x.ma
-00019b10: 6e79 6c69 6e75 7832 3031 345f 7333 3930  nylinux2014_s390
-00019b20: 782e 7768 6c22 2c20 6861 7368 203d 2022  x.whl", hash = "
-00019b30: 7368 6132 3536 3a61 3830 6137 3830 3436  sha256:a80a78046
-00019b40: 6137 3233 3631 6465 3733 6638 6633 3935  a72361de73f8f395
-00019b50: 6631 6631 6534 3966 3935 3663 3662 6538  f1f1e49f956c6be8
-00019b60: 3832 6565 6435 3835 3035 6131 3566 3365  82eed58505a15f3e
-00019b70: 3433 3039 3632 6222 7d2c 0a20 2020 207b  430962b"},.    {
-00019b80: 6669 6c65 203d 2022 5079 5941 4d4c 2d36  file = "PyYAML-6
-00019b90: 2e30 2d63 7033 3130 2d63 7033 3130 2d6d  .0-cp310-cp310-m
-00019ba0: 616e 796c 696e 7578 5f32 5f35 5f78 3836  anylinux_2_5_x86
-00019bb0: 5f36 342e 6d61 6e79 6c69 6e75 7831 5f78  _64.manylinux1_x
-00019bc0: 3836 5f36 342e 6d61 6e79 6c69 6e75 785f  86_64.manylinux_
-00019bd0: 325f 3132 5f78 3836 5f36 342e 6d61 6e79  2_12_x86_64.many
-00019be0: 6c69 6e75 7832 3031 305f 7838 365f 3634  linux2010_x86_64
-00019bf0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
-00019c00: 6861 3235 363a 6638 3466 6263 3938 6230  ha256:f84fbc98b0
-00019c10: 3139 6665 6632 6565 3961 3163 6233 6365  19fef2ee9a1cb3ce
-00019c20: 3933 6533 3138 3761 3664 6630 6232 3533  93e3187a6df0b253
-00019c30: 3861 3635 3162 6662 3839 3032 3534 6261  8a651bfb890254ba
-00019c40: 3966 3930 6235 227d 2c0a 2020 2020 7b66  9f90b5"},.    {f
-00019c50: 696c 6520 3d20 2250 7959 414d 4c2d 362e  ile = "PyYAML-6.
-00019c60: 302d 6370 3331 302d 6370 3331 302d 7769  0-cp310-cp310-wi
-00019c70: 6e33 322e 7768 6c22 2c20 6861 7368 203d  n32.whl", hash =
-00019c80: 2022 7368 6132 3536 3a32 6364 3564 6633   "sha256:2cd5df3
-00019c90: 6465 3438 3835 3765 6430 3534 3462 3334  de48857ed0544b34
-00019ca0: 6532 6434 3065 3966 6163 3434 3539 3330  e2d40e9fac445930
-00019cb0: 3033 3966 3363 6665 3462 6363 3539 3261  039f3cfe4bcc592a
-00019cc0: 3166 3833 3664 3531 3322 7d2c 0a20 2020  1f836d513"},.   
-00019cd0: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
-00019ce0: 2d36 2e30 2d63 7033 3130 2d63 7033 3130  -6.0-cp310-cp310
-00019cf0: 2d77 696e 5f61 6d64 3634 2e77 686c 222c  -win_amd64.whl",
-00019d00: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-00019d10: 6461 6634 3936 6335 3861 3863 3532 3038  daf496c58a8c5208
-00019d20: 3364 6630 3962 3830 6338 3630 3030 3531  3df09b80c8600051
-00019d30: 3934 3031 3463 3336 3938 3639 3864 3161  94014c3698698d1a
-00019d40: 3537 6362 6366 6131 3832 3134 3261 3361  57cbcfa182142a3a
-00019d50: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-00019d60: 2250 7959 414d 4c2d 362e 302d 6370 3331  "PyYAML-6.0-cp31
-00019d70: 312d 6370 3331 312d 6d61 636f 7378 5f31  1-cp311-macosx_1
-00019d80: 305f 395f 7838 365f 3634 2e77 686c 222c  0_9_x86_64.whl",
-00019d90: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-00019da0: 6434 6230 6261 3935 3132 3531 3935 3232  d4b0ba9512519522
-00019db0: 6231 3138 3039 3032 3537 6265 3131 3362  b118090257be113b
-00019dc0: 3934 3638 6438 3034 6231 3964 3633 6337  9468d804b19d63c7
-00019dd0: 3164 6263 6634 6134 3866 6133 3233 3538  1dbcf4a48fa32358
-00019de0: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-00019df0: 2250 7959 414d 4c2d 362e 302d 6370 3331  "PyYAML-6.0-cp31
-00019e00: 312d 6370 3331 312d 6d61 636f 7378 5f31  1-cp311-macosx_1
-00019e10: 315f 305f 6172 6d36 342e 7768 6c22 2c20  1_0_arm64.whl", 
-00019e20: 6861 7368 203d 2022 7368 6132 3536 3a38  hash = "sha256:8
-00019e30: 3139 3537 3932 3166 3434 3164 3530 6166  1957921f441d50af
-00019e40: 3233 3635 3461 6136 6335 6535 6561 6639  23654aa6c5e5eaf9
-00019e50: 6230 3661 6261 3766 3061 3139 6331 3861  b06aba7f0a19c18a
-00019e60: 3533 3864 6337 6566 3239 3163 3561 3122  538dc7ef291c5a1"
-00019e70: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-00019e80: 5079 5941 4d4c 2d36 2e30 2d63 7033 3131  PyYAML-6.0-cp311
-00019e90: 2d63 7033 3131 2d6d 616e 796c 696e 7578  -cp311-manylinux
-00019ea0: 5f32 5f31 375f 6161 7263 6836 342e 6d61  _2_17_aarch64.ma
-00019eb0: 6e79 6c69 6e75 7832 3031 345f 6161 7263  nylinux2014_aarc
-00019ec0: 6836 342e 7768 6c22 2c20 6861 7368 203d  h64.whl", hash =
-00019ed0: 2022 7368 6132 3536 3a61 6661 3137 6635   "sha256:afa17f5
-00019ee0: 6263 3464 3162 3130 6166 6434 3436 3666  bc4d1b10afd4466f
-00019ef0: 6433 6134 3464 6330 6532 3435 3338 3264  d3a44dc0e245382d
-00019f00: 6563 6135 6233 6333 3533 6438 6237 3537  eca5b3c353d8b757
-00019f10: 6639 6533 6563 6238 6422 7d2c 0a20 2020  f9e3ecb8d"},.   
-00019f20: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
-00019f30: 2d36 2e30 2d63 7033 3131 2d63 7033 3131  -6.0-cp311-cp311
-00019f40: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
-00019f50: 7333 3930 782e 6d61 6e79 6c69 6e75 7832  s390x.manylinux2
-00019f60: 3031 345f 7333 3930 782e 7768 6c22 2c20  014_s390x.whl", 
-00019f70: 6861 7368 203d 2022 7368 6132 3536 3a64  hash = "sha256:d
-00019f80: 6261 6430 6539 6433 3638 6262 3938 3966  bad0e9d368bb989f
-00019f90: 3435 3135 6461 3333 3062 3838 6130 3537  4515da330b88a057
-00019fa0: 3631 3764 3136 6236 6138 3234 3530 3834  617d16b6a8245084
-00019fb0: 6631 6230 3534 3030 6632 3436 3039 6622  f1b05400f24609f"
-00019fc0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-00019fd0: 5079 5941 4d4c 2d36 2e30 2d63 7033 3131  PyYAML-6.0-cp311
-00019fe0: 2d63 7033 3131 2d6d 616e 796c 696e 7578  -cp311-manylinux
-00019ff0: 5f32 5f31 375f 7838 365f 3634 2e6d 616e  _2_17_x86_64.man
-0001a000: 796c 696e 7578 3230 3134 5f78 3836 5f36  ylinux2014_x86_6
-0001a010: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001a020: 7368 6132 3536 3a34 3332 3535 3761 6132  sha256:432557aa2
-0001a030: 6330 3938 3032 6265 3339 3436 3033 3630  c09802be39460360
-0001a040: 6464 6666 6434 3831 3536 6533 3037 3231  ddffd48156e30721
-0001a050: 6635 6538 6439 3137 6630 3164 3331 3639  f5e8d917f01d3169
-0001a060: 3432 3136 3738 3222 7d2c 0a20 2020 207b  4216782"},.    {
-0001a070: 6669 6c65 203d 2022 5079 5941 4d4c 2d36  file = "PyYAML-6
-0001a080: 2e30 2d63 7033 3131 2d63 7033 3131 2d77  .0-cp311-cp311-w
-0001a090: 696e 3332 2e77 686c 222c 2068 6173 6820  in32.whl", hash 
-0001a0a0: 3d20 2273 6861 3235 363a 6266 6165 6635  = "sha256:bfaef5
-0001a0b0: 3733 6136 3362 6138 3932 3335 3033 6432  73a63ba8923503d2
-0001a0c0: 3735 3330 3336 3235 3930 6666 3466 3537  7530362590ff4f57
-0001a0d0: 3663 3632 3664 3836 6139 6665 6439 3538  6c626d86a9fed958
-0001a0e0: 3232 6138 3235 3566 6437 227d 2c0a 2020  22a8255fd7"},.  
-0001a0f0: 2020 7b66 696c 6520 3d20 2250 7959 414d    {file = "PyYAM
-0001a100: 4c2d 362e 302d 6370 3331 312d 6370 3331  L-6.0-cp311-cp31
-0001a110: 312d 7769 6e5f 616d 6436 342e 7768 6c22  1-win_amd64.whl"
-0001a120: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001a130: 3a30 3162 3435 6330 3139 3165 3664 3636  :01b45c0191e6d66
-0001a140: 6334 3730 6236 6366 3162 3935 3331 6137  c470b6cf1b9531a7
-0001a150: 3731 6138 3363 3163 3432 3038 3237 3265  71a83c1c4208272e
-0001a160: 6164 3437 6133 6165 3466 3266 3630 3362  ad47a3ae4f2f603b
-0001a170: 6622 7d2c 0a20 2020 207b 6669 6c65 203d  f"},.    {file =
-0001a180: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
-0001a190: 362d 6370 3336 6d2d 6d61 636f 7378 5f31  6-cp36m-macosx_1
-0001a1a0: 305f 395f 7838 365f 3634 2e77 686c 222c  0_9_x86_64.whl",
-0001a1b0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001a1c0: 3839 3762 3830 3839 3037 3635 6630 3337  897b80890765f037
-0001a1d0: 6466 3334 3033 6432 3262 6162 3431 3632  df3403d22bab4162
-0001a1e0: 3763 6138 3831 3161 6535 3565 3961 3732  7ca8811ae55e9a72
-0001a1f0: 3266 6430 3339 3238 3530 6563 3464 3836  2fd0392850ec4d86
-0001a200: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001a210: 2250 7959 414d 4c2d 362e 302d 6370 3336  "PyYAML-6.0-cp36
-0001a220: 2d63 7033 366d 2d6d 616e 796c 696e 7578  -cp36m-manylinux
-0001a230: 5f32 5f31 375f 6161 7263 6836 342e 6d61  _2_17_aarch64.ma
-0001a240: 6e79 6c69 6e75 7832 3031 345f 6161 7263  nylinux2014_aarc
-0001a250: 6836 342e 7768 6c22 2c20 6861 7368 203d  h64.whl", hash =
-0001a260: 2022 7368 6132 3536 3a35 3036 3032 6166   "sha256:50602af
-0001a270: 6164 6136 6436 6362 6661 6436 3939 6230  ada6d6cbfad699b0
-0001a280: 6337 6262 3530 6435 6363 6666 6137 6534  c7bb50d5ccffa7e4
-0001a290: 3661 3364 3733 3830 3932 6166 6464 6331  6a3d738092afddc1
-0001a2a0: 6639 3735 3834 3237 6622 7d2c 0a20 2020  f9758427f"},.   
-0001a2b0: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
-0001a2c0: 2d36 2e30 2d63 7033 362d 6370 3336 6d2d  -6.0-cp36-cp36m-
-0001a2d0: 6d61 6e79 6c69 6e75 785f 325f 3137 5f73  manylinux_2_17_s
-0001a2e0: 3339 3078 2e6d 616e 796c 696e 7578 3230  390x.manylinux20
-0001a2f0: 3134 5f73 3339 3078 2e77 686c 222c 2068  14_s390x.whl", h
-0001a300: 6173 6820 3d20 2273 6861 3235 363a 3438  ash = "sha256:48
-0001a310: 6333 3436 3931 3563 3131 3466 3566 6462  c346915c114f5fdb
-0001a320: 3365 6164 3730 3331 3262 6430 3432 6139  3ead70312bd042a9
-0001a330: 3533 6138 6365 3563 3731 3036 6435 6266  53a8ce5c7106d5bf
-0001a340: 6231 6135 3235 3465 3437 6461 3932 227d  b1a5254e47da92"}
-0001a350: 2c0a 2020 2020 7b66 696c 6520 3d20 2250  ,.    {file = "P
-0001a360: 7959 414d 4c2d 362e 302d 6370 3336 2d63  yYAML-6.0-cp36-c
-0001a370: 7033 366d 2d6d 616e 796c 696e 7578 5f32  p36m-manylinux_2
-0001a380: 5f35 5f78 3836 5f36 342e 6d61 6e79 6c69  _5_x86_64.manyli
-0001a390: 6e75 7831 5f78 3836 5f36 342e 6d61 6e79  nux1_x86_64.many
-0001a3a0: 6c69 6e75 785f 325f 3132 5f78 3836 5f36  linux_2_12_x86_6
-0001a3b0: 342e 6d61 6e79 6c69 6e75 7832 3031 305f  4.manylinux2010_
-0001a3c0: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
-0001a3d0: 6820 3d20 2273 6861 3235 363a 3938 6334  h = "sha256:98c4
-0001a3e0: 6433 3665 3939 3731 3465 3535 6366 6261  d36e99714e55cfba
-0001a3f0: 6165 6536 6464 3562 6164 6263 3961 3165  aee6dd5badbc9a1e
-0001a400: 6333 3339 6562 6663 3362 3166 3532 6532  c339ebfc3b1f52e2
-0001a410: 3933 6165 6536 6262 3731 6134 227d 2c0a  93aee6bb71a4"},.
-0001a420: 2020 2020 7b66 696c 6520 3d20 2250 7959      {file = "PyY
-0001a430: 414d 4c2d 362e 302d 6370 3336 2d63 7033  AML-6.0-cp36-cp3
-0001a440: 366d 2d77 696e 3332 2e77 686c 222c 2068  6m-win32.whl", h
-0001a450: 6173 6820 3d20 2273 6861 3235 363a 3032  ash = "sha256:02
-0001a460: 3833 6333 3561 3661 3966 6266 3034 3734  83c35a6a9fbf0474
-0001a470: 3933 6533 6130 6365 3864 3739 6566 3530  93e3a0ce8d79ef50
-0001a480: 3330 3835 3263 3531 6539 6439 3131 6132  30852c51e9d911a2
-0001a490: 3762 6164 6664 6530 3630 3532 3933 227d  7badfde0605293"}
-0001a4a0: 2c0a 2020 2020 7b66 696c 6520 3d20 2250  ,.    {file = "P
-0001a4b0: 7959 414d 4c2d 362e 302d 6370 3336 2d63  yYAML-6.0-cp36-c
-0001a4c0: 7033 366d 2d77 696e 5f61 6d64 3634 2e77  p36m-win_amd64.w
-0001a4d0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001a4e0: 3235 363a 3037 3735 3133 3630 3530 3263  256:07751360502c
-0001a4f0: 6161 6331 6330 3637 6138 3133 3264 3135  aac1c067a8132d15
-0001a500: 3063 6633 6436 3133 3339 6166 3536 3931  0cf3d61339af5691
-0001a510: 6665 3965 3837 3830 3330 3430 6462 6335  fe9e87803040dbc5
-0001a520: 6462 3537 227d 2c0a 2020 2020 7b66 696c  db57"},.    {fil
-0001a530: 6520 3d20 2250 7959 414d 4c2d 362e 302d  e = "PyYAML-6.0-
-0001a540: 6370 3337 2d63 7033 376d 2d6d 6163 6f73  cp37-cp37m-macos
-0001a550: 785f 3130 5f39 5f78 3836 5f36 342e 7768  x_10_9_x86_64.wh
-0001a560: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001a570: 3536 3a38 3139 6233 3833 3061 3135 3433  56:819b3830a1543
-0001a580: 6462 3036 6334 6434 6238 3635 6537 3064  db06c4d4b865e70d
-0001a590: 6564 3235 6265 3532 6132 6530 3633 3163  ed25be52a2e0631c
-0001a5a0: 6364 3266 3661 3437 6132 3832 3266 3266  cd2f6a47a2822f2f
-0001a5b0: 6437 6322 7d2c 0a20 2020 207b 6669 6c65  d7c"},.    {file
-0001a5c0: 203d 2022 5079 5941 4d4c 2d36 2e30 2d63   = "PyYAML-6.0-c
-0001a5d0: 7033 372d 6370 3337 6d2d 6d61 6e79 6c69  p37-cp37m-manyli
-0001a5e0: 6e75 785f 325f 3137 5f61 6172 6368 3634  nux_2_17_aarch64
-0001a5f0: 2e6d 616e 796c 696e 7578 3230 3134 5f61  .manylinux2014_a
-0001a600: 6172 6368 3634 2e77 686c 222c 2068 6173  arch64.whl", has
-0001a610: 6820 3d20 2273 6861 3235 363a 3437 3366  h = "sha256:473f
-0001a620: 3965 6462 3234 3363 6231 3933 3561 6235  9edb243cb1935ab5
-0001a630: 6130 3834 6562 3233 3864 3834 3266 6238  a084eb238d842fb8
-0001a640: 6634 3034 6564 3231 3933 6139 3135 6431  f404ed2193a915d1
-0001a650: 3738 3462 3561 3662 3566 6330 227d 2c0a  784b5a6b5fc0"},.
-0001a660: 2020 2020 7b66 696c 6520 3d20 2250 7959      {file = "PyY
-0001a670: 414d 4c2d 362e 302d 6370 3337 2d63 7033  AML-6.0-cp37-cp3
-0001a680: 376d 2d6d 616e 796c 696e 7578 5f32 5f31  7m-manylinux_2_1
-0001a690: 375f 7333 3930 782e 6d61 6e79 6c69 6e75  7_s390x.manylinu
-0001a6a0: 7832 3031 345f 7333 3930 782e 7768 6c22  x2014_s390x.whl"
-0001a6b0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001a6c0: 3a30 6365 3832 6437 3631 6335 3332 6665  :0ce82d761c532fe
-0001a6d0: 3465 6333 6638 3766 6334 3536 3838 6264  4ec3f87fc45688bd
-0001a6e0: 6433 6134 6331 6463 3565 3062 3461 3139  d3a4c1dc5e0b4a19
-0001a6f0: 3831 3462 3930 3039 6132 3962 6165 6664  814b9009a29baefd
-0001a700: 3422 7d2c 0a20 2020 207b 6669 6c65 203d  4"},.    {file =
-0001a710: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
-0001a720: 372d 6370 3337 6d2d 6d61 6e79 6c69 6e75  7-cp37m-manylinu
-0001a730: 785f 325f 355f 7838 365f 3634 2e6d 616e  x_2_5_x86_64.man
-0001a740: 796c 696e 7578 315f 7838 365f 3634 2e6d  ylinux1_x86_64.m
-0001a750: 616e 796c 696e 7578 5f32 5f31 325f 7838  anylinux_2_12_x8
-0001a760: 365f 3634 2e6d 616e 796c 696e 7578 3230  6_64.manylinux20
-0001a770: 3130 5f78 3836 5f36 342e 7768 6c22 2c20  10_x86_64.whl", 
-0001a780: 6861 7368 203d 2022 7368 6132 3536 3a32  hash = "sha256:2
-0001a790: 3331 3731 3064 3537 6164 6664 3830 3965  31710d57adfd809e
-0001a7a0: 6635 6433 3431 3833 6238 6564 3165 6561  f5d34183b8ed1eea
-0001a7b0: 6533 6637 3634 3539 6331 3866 6234 6130  e3f76459c18fb4a0
-0001a7c0: 6233 3733 6164 3536 6265 6463 6464 3922  b373ad56bedcdd9"
-0001a7d0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-0001a7e0: 5079 5941 4d4c 2d36 2e30 2d63 7033 372d  PyYAML-6.0-cp37-
-0001a7f0: 6370 3337 6d2d 7769 6e33 322e 7768 6c22  cp37m-win32.whl"
-0001a800: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001a810: 3a63 3536 3837 6238 6434 3363 6635 3835  :c5687b8d43cf585
-0001a820: 3435 6164 6531 6665 3365 3035 3566 3730  45ade1fe3e055f70
-0001a830: 6561 6337 6135 6131 6130 6266 3432 3832  eac7a5a1a0bf4282
-0001a840: 3433 3038 6438 3638 3238 3961 3935 3733  4308d868289a9573
-0001a850: 3722 7d2c 0a20 2020 207b 6669 6c65 203d  7"},.    {file =
-0001a860: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
-0001a870: 372d 6370 3337 6d2d 7769 6e5f 616d 6436  7-cp37m-win_amd6
-0001a880: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001a890: 7368 6132 3536 3a64 3135 6131 3831 6431  sha256:d15a181d1
-0001a8a0: 6563 6430 6434 3237 3064 6333 3265 6462  ecd0d4270dc32edb
-0001a8b0: 3436 6637 6362 3737 3333 6337 6335 3038  46f7cb7733c7c508
-0001a8c0: 3835 3732 3738 6433 6433 3738 6431 3464  857278d3d378d14d
-0001a8d0: 3630 3664 6232 6422 7d2c 0a20 2020 207b  606db2d"},.    {
-0001a8e0: 6669 6c65 203d 2022 5079 5941 4d4c 2d36  file = "PyYAML-6
-0001a8f0: 2e30 2d63 7033 382d 6370 3338 2d6d 6163  .0-cp38-cp38-mac
-0001a900: 6f73 785f 3130 5f39 5f78 3836 5f36 342e  osx_10_9_x86_64.
-0001a910: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001a920: 6132 3536 3a30 6234 3632 3466 3337 3964  a256:0b4624f379d
-0001a930: 6162 3234 6433 3732 3566 6664 6537 3635  ab24d3725ffde765
-0001a940: 3539 6366 6636 3364 3965 6339 3465 3137  59cff63d9ec94e17
-0001a950: 3336 6235 3536 6461 6364 6665 6265 3561  36b556dacdfebe5a
-0001a960: 6236 6434 6222 7d2c 0a20 2020 207b 6669  b6d4b"},.    {fi
-0001a970: 6c65 203d 2022 5079 5941 4d4c 2d36 2e30  le = "PyYAML-6.0
-0001a980: 2d63 7033 382d 6370 3338 2d6d 616e 796c  -cp38-cp38-manyl
-0001a990: 696e 7578 5f32 5f31 375f 6161 7263 6836  inux_2_17_aarch6
-0001a9a0: 342e 6d61 6e79 6c69 6e75 7832 3031 345f  4.manylinux2014_
-0001a9b0: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
-0001a9c0: 7368 203d 2022 7368 6132 3536 3a32 3133  sh = "sha256:213
-0001a9d0: 6336 3063 6435 3031 3036 3433 3663 6338  c60cd50106436cc8
-0001a9e0: 3138 6163 6366 3562 6161 3161 6261 3631  18accf5baa1aba61
-0001a9f0: 6330 3138 3966 6636 3130 6636 3466 3461  c0189ff610f64f4a
-0001aa00: 3365 3863 3637 3236 3231 3862 6122 7d2c  3e8c6726218ba"},
-0001aa10: 0a20 2020 207b 6669 6c65 203d 2022 5079  .    {file = "Py
-0001aa20: 5941 4d4c 2d36 2e30 2d63 7033 382d 6370  YAML-6.0-cp38-cp
-0001aa30: 3338 2d6d 616e 796c 696e 7578 5f32 5f31  38-manylinux_2_1
-0001aa40: 375f 7333 3930 782e 6d61 6e79 6c69 6e75  7_s390x.manylinu
-0001aa50: 7832 3031 345f 7333 3930 782e 7768 6c22  x2014_s390x.whl"
-0001aa60: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001aa70: 3a39 6661 3630 3030 3330 3031 3363 3464  :9fa600030013c4d
-0001aa80: 6538 3136 3533 3339 6462 3933 6431 3832  e8165339db93d182
-0001aa90: 6239 3433 3130 3736 6562 3938 6562 3430  b9431076eb98eb40
-0001aaa0: 6565 3036 3837 3030 6339 6338 3133 6533  ee068700c9c813e3
-0001aab0: 3422 7d2c 0a20 2020 207b 6669 6c65 203d  4"},.    {file =
-0001aac0: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
-0001aad0: 382d 6370 3338 2d6d 616e 796c 696e 7578  8-cp38-manylinux
-0001aae0: 5f32 5f35 5f78 3836 5f36 342e 6d61 6e79  _2_5_x86_64.many
-0001aaf0: 6c69 6e75 7831 5f78 3836 5f36 342e 6d61  linux1_x86_64.ma
-0001ab00: 6e79 6c69 6e75 785f 325f 3132 5f78 3836  nylinux_2_12_x86
-0001ab10: 5f36 342e 6d61 6e79 6c69 6e75 7832 3031  _64.manylinux201
-0001ab20: 305f 7838 365f 3634 2e77 686c 222c 2068  0_x86_64.whl", h
-0001ab30: 6173 6820 3d20 2273 6861 3235 363a 3237  ash = "sha256:27
-0001ab40: 3761 3065 6632 3938 3163 6134 3035 3831  7a0ef2981ca40581
-0001ab50: 6134 3730 3933 6539 6532 6431 3362 3366  a47093e9e2d13b3f
-0001ab60: 3166 6262 6566 6661 6530 3634 6331 6432  1fbbeffae064c1d2
-0001ab70: 3162 6663 6562 6132 3033 3032 3837 227d  1bfceba2030287"}
-0001ab80: 2c0a 2020 2020 7b66 696c 6520 3d20 2250  ,.    {file = "P
-0001ab90: 7959 414d 4c2d 362e 302d 6370 3338 2d63  yYAML-6.0-cp38-c
-0001aba0: 7033 382d 7769 6e33 322e 7768 6c22 2c20  p38-win32.whl", 
-0001abb0: 6861 7368 203d 2022 7368 6132 3536 3a64  hash = "sha256:d
-0001abc0: 3465 6363 6563 6639 6164 6636 6662 6363  4eccecf9adf6fbcc
-0001abd0: 3638 3631 6133 3830 3135 6332 6136 3466  6861a38015c2a64f
-0001abe0: 3338 6239 6439 3438 3338 6163 3138 3130  38b9d94838ac1810
-0001abf0: 6139 3032 3361 3036 3039 6531 6237 3822  a9023a0609e1b78"
-0001ac00: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-0001ac10: 5079 5941 4d4c 2d36 2e30 2d63 7033 382d  PyYAML-6.0-cp38-
-0001ac20: 6370 3338 2d77 696e 5f61 6d64 3634 2e77  cp38-win_amd64.w
-0001ac30: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001ac40: 3235 363a 3165 3437 3437 6263 3237 3962  256:1e4747bc279b
-0001ac50: 3466 3631 3361 3039 6562 3634 6262 6132  4f613a09eb64bba2
-0001ac60: 6261 3630 3264 3861 3636 3634 6336 6365  ba602d8a6664c6ce
-0001ac70: 3633 3936 6134 6430 6364 3431 3361 3530  6396a4d0cd413a50
-0001ac80: 6365 3037 227d 2c0a 2020 2020 7b66 696c  ce07"},.    {fil
-0001ac90: 6520 3d20 2250 7959 414d 4c2d 362e 302d  e = "PyYAML-6.0-
-0001aca0: 6370 3339 2d63 7033 392d 6d61 636f 7378  cp39-cp39-macosx
-0001acb0: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
-0001acc0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001acd0: 363a 3035 3564 3933 3764 3635 3832 3639  6:055d937d658269
-0001ace0: 3339 6362 3034 3466 6338 6339 6230 3838  39cb044fc8c9b088
-0001acf0: 3839 6538 6337 3433 6664 6336 6133 3262  89e8c743fdc6a32b
-0001ad00: 3333 6532 3339 3066 3636 3031 3365 3434  33e2390f66013e44
-0001ad10: 3962 227d 2c0a 2020 2020 7b66 696c 6520  9b"},.    {file 
-0001ad20: 3d20 2250 7959 414d 4c2d 362e 302d 6370  = "PyYAML-6.0-cp
-0001ad30: 3339 2d63 7033 392d 6d61 636f 7378 5f31  39-cp39-macosx_1
-0001ad40: 315f 305f 6172 6d36 342e 7768 6c22 2c20  1_0_arm64.whl", 
-0001ad50: 6861 7368 203d 2022 7368 6132 3536 3a65  hash = "sha256:e
-0001ad60: 3631 6365 6161 6236 6634 3966 6238 6264  61ceaab6f49fb8bd
-0001ad70: 6661 6130 6639 3263 3462 3537 6263 6662  faa0f92c4b57bcfb
-0001ad80: 6561 3534 6330 3932 3737 6231 6234 6637  ea54c09277b1b4f7
-0001ad90: 6163 3337 3662 6662 3761 3763 3137 3422  ac376bfb7a7c174"
-0001ada0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-0001adb0: 5079 5941 4d4c 2d36 2e30 2d63 7033 392d  PyYAML-6.0-cp39-
-0001adc0: 6370 3339 2d6d 616e 796c 696e 7578 5f32  cp39-manylinux_2
-0001add0: 5f31 375f 6161 7263 6836 342e 6d61 6e79  _17_aarch64.many
-0001ade0: 6c69 6e75 7832 3031 345f 6161 7263 6836  linux2014_aarch6
-0001adf0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001ae00: 7368 6132 3536 3a64 3637 6438 3339 6564  sha256:d67d839ed
-0001ae10: 6534 6564 3162 3238 6134 6538 3930 3937  e4ed1b28a4e89097
-0001ae20: 3335 6663 3939 3261 3932 3363 6462 3834  35fc992a923cdb84
-0001ae30: 6536 3138 3534 3439 3733 6437 6466 6337  e618544973d7dfc7
-0001ae40: 3135 3430 3830 3322 7d2c 0a20 2020 207b  1540803"},.    {
-0001ae50: 6669 6c65 203d 2022 5079 5941 4d4c 2d36  file = "PyYAML-6
-0001ae60: 2e30 2d63 7033 392d 6370 3339 2d6d 616e  .0-cp39-cp39-man
-0001ae70: 796c 696e 7578 5f32 5f31 375f 7333 3930  ylinux_2_17_s390
-0001ae80: 782e 6d61 6e79 6c69 6e75 7832 3031 345f  x.manylinux2014_
-0001ae90: 7333 3930 782e 7768 6c22 2c20 6861 7368  s390x.whl", hash
-0001aea0: 203d 2022 7368 6132 3536 3a63 6261 3863   = "sha256:cba8c
-0001aeb0: 3431 3165 6632 3731 6161 3033 3764 3733  411ef271aa037d73
-0001aec0: 3537 6132 6263 3866 3965 6538 6235 3862  57a2bc8f9ee8b58b
-0001aed0: 3939 3635 3833 3164 3965 3531 6261 6637  9965831d9e51baf7
-0001aee0: 3033 3238 3064 6337 3364 3322 7d2c 0a20  03280dc73d3"},. 
-0001aef0: 2020 207b 6669 6c65 203d 2022 5079 5941     {file = "PyYA
-0001af00: 4d4c 2d36 2e30 2d63 7033 392d 6370 3339  ML-6.0-cp39-cp39
-0001af10: 2d6d 616e 796c 696e 7578 5f32 5f35 5f78  -manylinux_2_5_x
-0001af20: 3836 5f36 342e 6d61 6e79 6c69 6e75 7831  86_64.manylinux1
-0001af30: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
-0001af40: 785f 325f 3132 5f78 3836 5f36 342e 6d61  x_2_12_x86_64.ma
-0001af50: 6e79 6c69 6e75 7832 3031 305f 7838 365f  nylinux2010_x86_
-0001af60: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001af70: 2273 6861 3235 363a 3430 3532 3738 3537  "sha256:40527857
-0001af80: 3235 3262 3631 6561 6364 3164 3961 6635  252b61eacd1d9af5
-0001af90: 3030 6333 3333 3762 6138 6465 6238 6663  00c3337ba8deb8fc
-0001afa0: 3239 3839 3430 3239 3134 3836 6334 3635  298940291486c465
-0001afb0: 6338 6234 3665 6330 227d 2c0a 2020 2020  c8b46ec0"},.    
-0001afc0: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
-0001afd0: 362e 302d 6370 3339 2d63 7033 392d 7769  6.0-cp39-cp39-wi
-0001afe0: 6e33 322e 7768 6c22 2c20 6861 7368 203d  n32.whl", hash =
-0001aff0: 2022 7368 6132 3536 3a62 3562 3965 6363   "sha256:b5b9ecc
-0001b000: 6164 3734 3761 6162 6161 6666 6263 3630  ad747aabaaffbc60
-0001b010: 3634 3830 3036 3730 6630 6332 3937 6535  64800670f0c297e5
-0001b020: 3263 3132 3735 3465 6231 6439 3736 6335  2c12754eb1d976c5
-0001b030: 3765 3466 3734 6463 6222 7d2c 0a20 2020  7e4f74dcb"},.   
-0001b040: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
-0001b050: 2d36 2e30 2d63 7033 392d 6370 3339 2d77  -6.0-cp39-cp39-w
-0001b060: 696e 5f61 6d64 3634 2e77 686c 222c 2068  in_amd64.whl", h
-0001b070: 6173 6820 3d20 2273 6861 3235 363a 6233  ash = "sha256:b3
-0001b080: 6432 3637 3834 3262 6631 3235 3836 6261  d267842bf12586ba
-0001b090: 3663 3733 3466 3839 6431 6635 6238 3731  6c734f89d1f5b871
-0001b0a0: 6466 3032 3733 3135 3739 3138 6230 6363  df0273157918b0cc
-0001b0b0: 6566 6132 3964 6562 3035 6332 3163 227d  efa29deb05c21c"}
-0001b0c0: 2c0a 2020 2020 7b66 696c 6520 3d20 2250  ,.    {file = "P
-0001b0d0: 7959 414d 4c2d 362e 302e 7461 722e 677a  yYAML-6.0.tar.gz
-0001b0e0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001b0f0: 363a 3638 6662 3531 3963 3134 3330 3666  6:68fb519c14306f
-0001b100: 6563 3937 3230 6132 6135 6234 3562 6339  ec9720a2a5b45bc9
-0001b110: 6630 6338 6431 6239 6337 3261 6466 3435  f0c8d1b9c72adf45
-0001b120: 6333 3762 6165 6466 6364 3934 3963 3335  c37baedfcd949c35
-0001b130: 6132 227d 2c0a 5d0a 0a5b 5b70 6163 6b61  a2"},.]..[[packa
-0001b140: 6765 5d5d 0a6e 616d 6520 3d20 2270 7979  ge]].name = "pyy
-0001b150: 616d 6c2d 656e 762d 7461 6722 0a76 6572  aml-env-tag".ver
-0001b160: 7369 6f6e 203d 2022 302e 3122 0a64 6573  sion = "0.1".des
-0001b170: 6372 6970 7469 6f6e 203d 2022 4120 6375  cription = "A cu
-0001b180: 7374 6f6d 2059 414d 4c20 7461 6720 666f  stom YAML tag fo
-0001b190: 7220 7265 6665 7265 6e63 696e 6720 656e  r referencing en
-0001b1a0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-0001b1b0: 6c65 7320 696e 2059 414d 4c20 6669 6c65  les in YAML file
-0001b1c0: 732e 2022 0a6f 7074 696f 6e61 6c20 3d20  s. ".optional = 
-0001b1d0: 6661 6c73 650a 7079 7468 6f6e 2d76 6572  false.python-ver
-0001b1e0: 7369 6f6e 7320 3d20 223e 3d33 2e36 220a  sions = ">=3.6".
-0001b1f0: 6669 6c65 7320 3d20 5b0a 2020 2020 7b66  files = [.    {f
-0001b200: 696c 6520 3d20 2270 7979 616d 6c5f 656e  ile = "pyyaml_en
-0001b210: 765f 7461 672d 302e 312d 7079 332d 6e6f  v_tag-0.1-py3-no
-0001b220: 6e65 2d61 6e79 2e77 686c 222c 2068 6173  ne-any.whl", has
-0001b230: 6820 3d20 2273 6861 3235 363a 6166 3331  h = "sha256:af31
-0001b240: 3130 3664 6563 3861 3464 3638 6336 3032  106dec8a4d68c602
-0001b250: 3037 6331 3838 3630 3331 6362 6638 3339  07c1886031cbf839
-0001b260: 6236 3861 6137 6162 6363 6462 3139 3836  b68aa7abccdb1986
-0001b270: 3832 3030 3533 3263 3230 3639 227d 2c0a  8200532c2069"},.
-0001b280: 2020 2020 7b66 696c 6520 3d20 2270 7979      {file = "pyy
-0001b290: 616d 6c5f 656e 765f 7461 672d 302e 312e  aml_env_tag-0.1.
-0001b2a0: 7461 722e 677a 222c 2068 6173 6820 3d20  tar.gz", hash = 
-0001b2b0: 2273 6861 3235 363a 3730 3039 3236 3735  "sha256:70092675
-0001b2c0: 6264 6131 3466 6465 6333 3362 3331 6261  bda14fdec33b31ba
-0001b2d0: 3737 6537 3534 3364 6539 6464 6338 3866  77e7543de9ddc88f
-0001b2e0: 3265 3562 3939 3136 3033 3936 3537 3264  2e5b99160396572d
-0001b2f0: 3131 3532 3562 6462 227d 2c0a 5d0a 0a5b  11525bdb"},.]..[
-0001b300: 7061 636b 6167 652e 6465 7065 6e64 656e  package.dependen
-0001b310: 6369 6573 5d0a 7079 7961 6d6c 203d 2022  cies].pyyaml = "
-0001b320: 2a22 0a0a 5b5b 7061 636b 6167 655d 5d0a  *"..[[package]].
-0001b330: 6e61 6d65 203d 2022 7079 7a6d 7122 0a76  name = "pyzmq".v
-0001b340: 6572 7369 6f6e 203d 2022 3235 2e30 2e32  ersion = "25.0.2
-0001b350: 220a 6465 7363 7269 7074 696f 6e20 3d20  ".description = 
-0001b360: 2250 7974 686f 6e20 6269 6e64 696e 6773  "Python bindings
-0001b370: 2066 6f72 2030 4d51 220a 6f70 7469 6f6e   for 0MQ".option
-0001b380: 616c 203d 2066 616c 7365 0a70 7974 686f  al = false.pytho
-0001b390: 6e2d 7665 7273 696f 6e73 203d 2022 3e3d  n-versions = ">=
-0001b3a0: 332e 3622 0a66 696c 6573 203d 205b 0a20  3.6".files = [. 
-0001b3b0: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
-0001b3c0: 712d 3235 2e30 2e32 2d63 7033 3130 2d63  q-25.0.2-cp310-c
-0001b3d0: 7033 3130 2d6d 6163 6f73 785f 3130 5f31  p310-macosx_10_1
-0001b3e0: 355f 756e 6976 6572 7361 6c32 2e77 686c  5_universal2.whl
-0001b3f0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001b400: 363a 6163 3137 3865 3636 3663 3039 3763  6:ac178e666c097c
-0001b410: 3864 3364 6562 3530 3937 6235 3863 6431  8d3deb5097b58cd1
-0001b420: 3331 3630 3932 6663 3433 6538 6566 3562  316092fc43e8ef5b
-0001b430: 3566 6462 3235 3962 3531 6461 3765 3733  5fdb259b51da7e73
-0001b440: 3135 227d 2c0a 2020 2020 7b66 696c 6520  15"},.    {file 
-0001b450: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001b460: 6370 3331 302d 6370 3331 302d 6d61 636f  cp310-cp310-maco
-0001b470: 7378 5f31 305f 395f 7838 365f 3634 2e77  sx_10_9_x86_64.w
-0001b480: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001b490: 3235 363a 3635 3965 3632 6531 6362 6230  256:659e62e1cbb0
-0001b4a0: 3633 3135 3163 3532 6635 6230 3161 3338  63151c52f5b01a38
-0001b4b0: 6531 6466 3662 3534 6665 6363 6661 3365  e1df6b54feccfa3e
-0001b4c0: 3235 3039 6434 3463 3335 6361 3664 3739  2509d44c35ca6d79
-0001b4d0: 3632 6565 227d 2c0a 2020 2020 7b66 696c  62ee"},.    {fil
-0001b4e0: 6520 3d20 2270 797a 6d71 2d32 352e 302e  e = "pyzmq-25.0.
-0001b4f0: 322d 6370 3331 302d 6370 3331 302d 6d61  2-cp310-cp310-ma
-0001b500: 6e79 6c69 6e75 785f 325f 3137 5f61 6172  nylinux_2_17_aar
-0001b510: 6368 3634 2e6d 616e 796c 696e 7578 3230  ch64.manylinux20
-0001b520: 3134 5f61 6172 6368 3634 2e77 686c 222c  14_aarch64.whl",
-0001b530: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001b540: 3832 3830 6164 6138 3930 3130 3733 3561  8280ada89010735a
-0001b550: 3132 6239 3638 6563 3365 6139 6134 3638  12b968ec3ea9a468
-0001b560: 6163 3265 3034 6664 6463 6331 6365 6465  ac2e04fddcc1cede
-0001b570: 3539 6362 3766 3531 3738 3738 3362 3963  59cb7f5178783b9c
-0001b580: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001b590: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
-0001b5a0: 3331 302d 6370 3331 302d 6d61 6e79 6c69  310-cp310-manyli
-0001b5b0: 6e75 785f 325f 3137 5f69 3638 362e 6d61  nux_2_17_i686.ma
-0001b5c0: 6e79 6c69 6e75 7832 3031 345f 6936 3836  nylinux2014_i686
-0001b5d0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
-0001b5e0: 6861 3235 363a 6139 6235 6565 6235 3237  ha256:a9b5eeb527
-0001b5f0: 3861 3861 3633 3662 6230 6162 6464 3966  8a8a636bb0abdd9f
-0001b600: 6635 3037 3662 6362 6238 3336 6364 3233  f5076bcbb836cd23
-0001b610: 3032 3536 3564 6635 3366 6631 6661 3764  02565df53ff1fa7d
-0001b620: 3130 3664 3534 227d 2c0a 2020 2020 7b66  106d54"},.    {f
-0001b630: 696c 6520 3d20 2270 797a 6d71 2d32 352e  ile = "pyzmq-25.
-0001b640: 302e 322d 6370 3331 302d 6370 3331 302d  0.2-cp310-cp310-
-0001b650: 6d61 6e79 6c69 6e75 785f 325f 3137 5f78  manylinux_2_17_x
-0001b660: 3836 5f36 342e 6d61 6e79 6c69 6e75 7832  86_64.manylinux2
-0001b670: 3031 345f 7838 365f 3634 2e77 686c 222c  014_x86_64.whl",
-0001b680: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001b690: 3961 3265 3566 6534 3264 6665 3662 3733  9a2e5fe42dfe6b73
-0001b6a0: 6361 3132 3062 3937 6163 3966 3334 6266  ca120b97ac9f34bf
-0001b6b0: 6138 3431 3466 6562 3135 6530 3065 3337  a8414feb15e00e37
-0001b6c0: 3431 3564 6264 3531 6366 3232 3765 6636  415dbd51cf227ef6
-0001b6d0: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001b6e0: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
-0001b6f0: 3331 302d 6370 3331 302d 6d61 6e79 6c69  310-cp310-manyli
-0001b700: 6e75 785f 325f 3238 5f78 3836 5f36 342e  nux_2_28_x86_64.
-0001b710: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001b720: 6132 3536 3a38 3237 6266 3630 6537 3439  a256:827bf60e749
-0001b730: 6537 3861 6362 3430 3861 3663 3561 6636  e78acb408a6c5af6
-0001b740: 3638 3865 6662 6339 3939 3365 3434 6563  688efbc9993e44ec
-0001b750: 6337 3932 6230 3336 6563 3266 3462 3461  c792b036ec2f4b4a
-0001b760: 6366 3438 3522 7d2c 0a20 2020 207b 6669  cf485"},.    {fi
-0001b770: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
-0001b780: 2e32 2d63 7033 3130 2d63 7033 3130 2d6d  .2-cp310-cp310-m
-0001b790: 7573 6c6c 696e 7578 5f31 5f31 5f61 6172  usllinux_1_1_aar
-0001b7a0: 6368 3634 2e77 686c 222c 2068 6173 6820  ch64.whl", hash 
-0001b7b0: 3d20 2273 6861 3235 363a 3762 3530 3461  = "sha256:7b504a
-0001b7c0: 6534 3364 3337 6532 3832 3330 3164 6135  e43d37e282301da5
-0001b7d0: 3836 3532 3965 3264 6564 3862 3336 6434  86529e2ded8b36d4
-0001b7e0: 6565 3263 6435 6536 6462 3433 3836 3732  ee2cd5e6db438672
-0001b7f0: 3464 6465 6161 3662 6263 227d 2c0a 2020  4ddeaa6bbc"},.  
-0001b800: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
-0001b810: 2d32 352e 302e 322d 6370 3331 302d 6370  -25.0.2-cp310-cp
-0001b820: 3331 302d 6d75 736c 6c69 6e75 785f 315f  310-musllinux_1_
-0001b830: 315f 6936 3836 2e77 686c 222c 2068 6173  1_i686.whl", has
-0001b840: 6820 3d20 2273 6861 3235 363a 6362 3166  h = "sha256:cb1f
-0001b850: 3639 6130 6132 6132 6231 6161 6538 3431  69a0a2a2b1aae841
-0001b860: 3239 3739 6464 3632 3933 6363 3662 6364  2979dd6293cc6bcd
-0001b870: 6464 3434 3339 6266 3037 6534 3735 3864  dd4439bf07e4758d
-0001b880: 3836 3464 6462 3131 3233 3534 227d 2c0a  864ddb112354"},.
-0001b890: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
-0001b8a0: 6d71 2d32 352e 302e 322d 6370 3331 302d  mq-25.0.2-cp310-
-0001b8b0: 6370 3331 302d 6d75 736c 6c69 6e75 785f  cp310-musllinux_
-0001b8c0: 315f 315f 7838 365f 3634 2e77 686c 222c  1_1_x86_64.whl",
-0001b8d0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001b8e0: 3262 3963 3963 6339 3635 6364 6632 3833  2b9c9cc965cdf283
-0001b8f0: 3831 6533 3664 6135 3235 6463 6238 3966  81e36da525dcb89f
-0001b900: 6331 3537 3164 3963 3534 3830 3066 6463  c1571d9c54800fdc
-0001b910: 6437 3365 3366 3733 6132 6663 3239 6264  d73e3f73a2fc29bd
-0001b920: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001b930: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
-0001b940: 3331 302d 6370 3331 302d 7769 6e33 322e  310-cp310-win32.
-0001b950: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001b960: 6132 3536 3a32 3461 6262 6664 6262 3735  a256:24abbfdbb75
-0001b970: 6163 3530 3339 3230 3565 3732 6436 6337  ac5039205e72d6c7
-0001b980: 3566 3130 6663 3339 6439 3235 6632 6466  5f10fc39d925f2df
-0001b990: 3866 6632 3165 6263 3734 3137 3934 3838  8ff21ebc74179488
-0001b9a0: 6562 6663 6122 7d2c 0a20 2020 207b 6669  ebfca"},.    {fi
-0001b9b0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
-0001b9c0: 2e32 2d63 7033 3130 2d63 7033 3130 2d77  .2-cp310-cp310-w
-0001b9d0: 696e 5f61 6d64 3634 2e77 686c 222c 2068  in_amd64.whl", h
-0001b9e0: 6173 6820 3d20 2273 6861 3235 363a 3661  ash = "sha256:6a
-0001b9f0: 3832 3161 3530 3638 3232 6661 6335 3564  821a506822fac55d
-0001ba00: 3264 6632 3038 3561 3532 3533 3066 3638  2df2085a52530f68
-0001ba10: 6162 3135 6365 6564 3132 6436 3335 3339  ab15ceed12d63539
-0001ba20: 6164 6333 3262 6434 3431 3066 3665 227d  adc32bd4410f6e"}
-0001ba30: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
-0001ba40: 797a 6d71 2d32 352e 302e 322d 6370 3331  yzmq-25.0.2-cp31
-0001ba50: 312d 6370 3331 312d 6d61 636f 7378 5f31  1-cp311-macosx_1
-0001ba60: 305f 3135 5f75 6e69 7665 7273 616c 322e  0_15_universal2.
-0001ba70: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001ba80: 6132 3536 3a39 6166 3062 6230 3237 3765  a256:9af0bb0277e
-0001ba90: 3932 6634 3161 6633 3565 3939 3163 3234  92f41af35e991c24
-0001baa0: 3263 3963 3731 3932 3031 3639 6436 6161  2c9c71920169d6aa
-0001bab0: 3533 6164 6537 6534 3434 6633 3338 6634  53ade7e444f338f4
-0001bac0: 6338 3132 3822 7d2c 0a20 2020 207b 6669  c8128"},.    {fi
-0001bad0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
-0001bae0: 2e32 2d63 7033 3131 2d63 7033 3131 2d6d  .2-cp311-cp311-m
-0001baf0: 6163 6f73 785f 3130 5f39 5f78 3836 5f36  acosx_10_9_x86_6
-0001bb00: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001bb10: 7368 6132 3536 3a35 3461 3936 6366 3737  sha256:54a96cf77
-0001bb20: 3638 3461 3361 3533 3762 3736 6163 6661  684a3a537b76acfa
-0001bb30: 3732 3337 6231 6537 3961 3866 3864 3134  7237b1e79a8f8d14
-0001bb40: 6537 6630 3065 3031 3731 6139 3462 3334  e7f00e0171a94b34
-0001bb50: 3663 3532 3933 6522 7d2c 0a20 2020 207b  6c5293e"},.    {
-0001bb60: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
-0001bb70: 2e30 2e32 2d63 7033 3131 2d63 7033 3131  .0.2-cp311-cp311
-0001bb80: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
-0001bb90: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
-0001bba0: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
-0001bbb0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001bbc0: 3536 3a38 3836 3439 6231 3965 6465 3163  56:88649b19ede1c
-0001bbd0: 6162 3033 6239 3662 3636 6333 3634 6362  ab03b96b66c364cb
-0001bbe0: 6266 3137 6339 3533 3631 3563 6462 6338  bf17c953615cdbc8
-0001bbf0: 3434 6637 6636 6535 6631 3463 3565 3532  44f7f6e5f14c5e52
-0001bc00: 3631 6322 7d2c 0a20 2020 207b 6669 6c65  61c"},.    {file
-0001bc10: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001bc20: 2d63 7033 3131 2d63 7033 3131 2d6d 616e  -cp311-cp311-man
-0001bc30: 796c 696e 7578 5f32 5f31 375f 6936 3836  ylinux_2_17_i686
-0001bc40: 2e6d 616e 796c 696e 7578 3230 3134 5f69  .manylinux2014_i
-0001bc50: 3638 362e 7768 6c22 2c20 6861 7368 203d  686.whl", hash =
-0001bc60: 2022 7368 6132 3536 3a37 3135 6366 6637   "sha256:715cff7
-0001bc70: 3634 3461 3830 6137 3739 3539 3533 6331  644a80a7795953c1
-0001bc80: 3162 3036 3761 3735 6631 3665 6239 6663  1b067a75f16eb9fc
-0001bc90: 3639 3561 3561 3533 3331 3638 3931 6562  695a5a53316891eb
-0001bca0: 6565 3766 3363 3964 3522 7d2c 0a20 2020  ee7f3c9d5"},.   
-0001bcb0: 207b 6669 6c65 203d 2022 7079 7a6d 712d   {file = "pyzmq-
-0001bcc0: 3235 2e30 2e32 2d63 7033 3131 2d63 7033  25.0.2-cp311-cp3
-0001bcd0: 3131 2d6d 616e 796c 696e 7578 5f32 5f31  11-manylinux_2_1
-0001bce0: 375f 7838 365f 3634 2e6d 616e 796c 696e  7_x86_64.manylin
-0001bcf0: 7578 3230 3134 5f78 3836 5f36 342e 7768  ux2014_x86_64.wh
-0001bd00: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001bd10: 3536 3a33 3132 6233 6630 6630 3636 6234  56:312b3f0f066b4
-0001bd20: 6631 6431 3733 3833 6161 6535 3039 6261  f1d17383aae509ba
-0001bd30: 6366 3833 3363 6361 6635 3931 3138 3461  cf833ccaf591184a
-0001bd40: 3166 3363 3761 3136 3631 6330 3835 3036  1f3c7a1661c08506
-0001bd50: 3361 6522 7d2c 0a20 2020 207b 6669 6c65  3ae"},.    {file
-0001bd60: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001bd70: 2d63 7033 3131 2d63 7033 3131 2d6d 616e  -cp311-cp311-man
-0001bd80: 796c 696e 7578 5f32 5f32 385f 7838 365f  ylinux_2_28_x86_
-0001bd90: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001bda0: 2273 6861 3235 363a 6434 3838 6335 6338  "sha256:d488c5c8
-0001bdb0: 3633 3066 3765 3738 3265 3830 3038 3639  630f7e782e800869
-0001bdc0: 6638 3237 3434 6333 6163 6134 6163 6136  f82744c3aca4aca6
-0001bdd0: 3263 3633 3233 3265 3564 3863 3439 3064  2c63232e5d8c490d
-0001bde0: 3364 3636 3935 3661 227d 2c0a 2020 2020  3d66956a"},.    
-0001bdf0: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001be00: 352e 302e 322d 6370 3331 312d 6370 3331  5.0.2-cp311-cp31
-0001be10: 312d 6d75 736c 6c69 6e75 785f 315f 315f  1-musllinux_1_1_
-0001be20: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
-0001be30: 7368 203d 2022 7368 6132 3536 3a33 3864  sh = "sha256:38d
-0001be40: 3966 3738 6436 3962 6364 6565 6330 6331  9f78d69bcdeec0c1
-0001be50: 3165 3066 6562 3362 6337 3066 3336 6639  1e0feb3bc70f36f9
-0001be60: 6238 6334 3466 6330 3665 3564 3036 6439  b8c44fc06e5d06d9
-0001be70: 3164 6330 6132 3162 3435 3363 3722 7d2c  1dc0a21b453c7"},
-0001be80: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-0001be90: 7a6d 712d 3235 2e30 2e32 2d63 7033 3131  zmq-25.0.2-cp311
-0001bea0: 2d63 7033 3131 2d6d 7573 6c6c 696e 7578  -cp311-musllinux
-0001beb0: 5f31 5f31 5f69 3638 362e 7768 6c22 2c20  _1_1_i686.whl", 
-0001bec0: 6861 7368 203d 2022 7368 6132 3536 3a33  hash = "sha256:3
-0001bed0: 3035 3961 3661 3533 3463 3931 3065 3164  059a6a534c910e1d
-0001bee0: 3564 3036 3864 6634 3266 3630 6434 3334  5d068df42f60d434
-0001bef0: 6637 3965 3663 6336 3238 3561 6134 3639  f79e6cc6285aa469
-0001bf00: 6233 3834 6661 3932 3166 3738 6366 3822  b384fa921f78cf8"
-0001bf10: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-0001bf20: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
-0001bf30: 3131 2d63 7033 3131 2d6d 7573 6c6c 696e  11-cp311-musllin
-0001bf40: 7578 5f31 5f31 5f78 3836 5f36 342e 7768  ux_1_1_x86_64.wh
-0001bf50: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001bf60: 3536 3a36 3532 3664 3039 3762 3735 3139  56:6526d097b7519
-0001bf70: 3266 3232 3863 3039 6434 3834 3230 3835  2f228c09d4842085
-0001bf80: 3464 3533 6466 6263 3761 6262 6234 3162  4d53dfbc7abbb41b
-0001bf90: 3065 3236 6633 3633 6363 6232 3666 6263  0e26f363ccb26fbc
-0001bfa0: 3137 3722 7d2c 0a20 2020 207b 6669 6c65  177"},.    {file
-0001bfb0: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001bfc0: 2d63 7033 3131 2d63 7033 3131 2d77 696e  -cp311-cp311-win
-0001bfd0: 3332 2e77 686c 222c 2068 6173 6820 3d20  32.whl", hash = 
-0001bfe0: 2273 6861 3235 363a 3563 3566 6262 3232  "sha256:5c5fbb22
-0001bff0: 3965 3430 6138 3961 3266 6537 3364 3063  9e40a89a2fe73d0c
-0001c000: 3131 3831 3931 3666 3331 6533 3066 3235  1181916f31e30f25
-0001c010: 3363 6232 6436 6439 3162 6561 3739 3237  3cb2d6d91bea7927
-0001c020: 6332 6531 3834 3133 227d 2c0a 2020 2020  c2e18413"},.    
-0001c030: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001c040: 352e 302e 322d 6370 3331 312d 6370 3331  5.0.2-cp311-cp31
-0001c050: 312d 7769 6e5f 616d 6436 342e 7768 6c22  1-win_amd64.whl"
-0001c060: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001c070: 3a65 6431 3565 3361 3263 3363 3233 3938  :ed15e3a2c3c2398
-0001c080: 6536 6165 3563 6538 3664 3661 3331 6234  e6ae5ce86d6a31b4
-0001c090: 3532 6466 6436 6164 3463 6435 6433 3132  52dfd6ad4cd5d312
-0001c0a0: 3539 3662 3330 3932 3963 3462 3665 3138  596b30929c4b6e18
-0001c0b0: 3222 7d2c 0a20 2020 207b 6669 6c65 203d  2"},.    {file =
-0001c0c0: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
-0001c0d0: 7033 362d 6370 3336 6d2d 6d61 636f 7378  p36-cp36m-macosx
-0001c0e0: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
-0001c0f0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001c100: 363a 3033 3266 3563 3834 3833 6338 3562  6:032f5c8483c85b
-0001c110: 6639 6339 6361 3035 3933 6131 3163 3763  f9c9ca0593a11c7c
-0001c120: 3734 3964 3733 3463 6536 3864 3433 3565  749d734ce68d435e
-0001c130: 3338 6333 6637 3265 3735 3962 3938 6233  38c3f72e759b98b3
-0001c140: 6339 227d 2c0a 2020 2020 7b66 696c 6520  c9"},.    {file 
-0001c150: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001c160: 6370 3336 2d63 7033 366d 2d6d 616e 796c  cp36-cp36m-manyl
-0001c170: 696e 7578 5f32 5f31 375f 6161 7263 6836  inux_2_17_aarch6
-0001c180: 342e 6d61 6e79 6c69 6e75 7832 3031 345f  4.manylinux2014_
-0001c190: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
-0001c1a0: 7368 203d 2022 7368 6132 3536 3a33 3734  sh = "sha256:374
-0001c1b0: 6235 3535 3136 3339 3362 6664 3464 3761  b55516393bfd4d7a
-0001c1c0: 3764 6161 3663 3362 3336 6436 6464 3661  7daa6c3b36d6dd6a
-0001c1d0: 3331 6666 3964 3261 6461 6430 3833 3863  31ff9d2adad0838c
-0001c1e0: 6436 6132 3033 3132 3565 3731 3422 7d2c  d6a203125e714"},
-0001c1f0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-0001c200: 7a6d 712d 3235 2e30 2e32 2d63 7033 362d  zmq-25.0.2-cp36-
-0001c210: 6370 3336 6d2d 6d61 6e79 6c69 6e75 785f  cp36m-manylinux_
-0001c220: 325f 355f 6936 3836 2e6d 616e 796c 696e  2_5_i686.manylin
-0001c230: 7578 315f 6936 3836 2e77 686c 222c 2068  ux1_i686.whl", h
-0001c240: 6173 6820 3d20 2273 6861 3235 363a 3038  ash = "sha256:08
-0001c250: 6266 6363 3231 6235 3939 3761 3962 6534  bfcc21b5997a9be4
-0001c260: 6665 6661 3430 3533 3431 3332 3064 3865  fefa405341320d8e
-0001c270: 3766 3139 6234 6436 3834 6662 3963 3035  7f19b4d684fb9c05
-0001c280: 3830 3235 3563 3562 6436 6436 3935 227d  80255c5bd6d695"}
-0001c290: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
-0001c2a0: 797a 6d71 2d32 352e 302e 322d 6370 3336  yzmq-25.0.2-cp36
-0001c2b0: 2d63 7033 366d 2d6d 616e 796c 696e 7578  -cp36m-manylinux
-0001c2c0: 5f32 5f35 5f78 3836 5f36 342e 6d61 6e79  _2_5_x86_64.many
-0001c2d0: 6c69 6e75 7831 5f78 3836 5f36 342e 7768  linux1_x86_64.wh
-0001c2e0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001c2f0: 3536 3a31 6138 3433 6432 3661 3864 6131  56:1a843d26a8da1
-0001c300: 6237 3532 6337 3462 6330 3139 6337 6232  b752c74bc019c7b2
-0001c310: 3065 3637 3931 6565 3831 3363 6436 3837  0e6791ee813cd687
-0001c320: 3734 3439 6536 6131 3431 3535 3839 6432  7449e6a1415589d2
-0001c330: 3266 6622 7d2c 0a20 2020 207b 6669 6c65  2ff"},.    {file
-0001c340: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001c350: 2d63 7033 362d 6370 3336 6d2d 6d75 736c  -cp36-cp36m-musl
-0001c360: 6c69 6e75 785f 315f 315f 6161 7263 6836  linux_1_1_aarch6
-0001c370: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001c380: 7368 6132 3536 3a62 3438 3631 3661 3039  sha256:b48616a09
-0001c390: 6437 6466 3964 6261 6532 6634 3561 3032  d7df9dbae2f45a02
-0001c3a0: 3536 6565 6537 6237 3934 6239 3033 6464  56eee7b794b903dd
-0001c3b0: 6336 6438 3635 3761 3939 3438 3636 3962  c6d8657a9948669b
-0001c3c0: 3334 3566 3232 3022 7d2c 0a20 2020 207b  345f220"},.    {
-0001c3d0: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
-0001c3e0: 2e30 2e32 2d63 7033 362d 6370 3336 6d2d  .0.2-cp36-cp36m-
-0001c3f0: 6d75 736c 6c69 6e75 785f 315f 315f 6936  musllinux_1_1_i6
-0001c400: 3836 2e77 686c 222c 2068 6173 6820 3d20  86.whl", hash = 
-0001c410: 2273 6861 3235 363a 6434 3432 3762 3461  "sha256:d4427b4a
-0001c420: 3133 3665 3362 3766 3835 3531 3663 3736  136e3b7f85516c76
-0001c430: 6464 3265 3037 3536 6332 3265 6563 3430  dd2e0756c22eec40
-0001c440: 3236 6166 6237 3663 6131 3339 3731 3532  26afb76ca1397152
-0001c450: 6230 6361 3831 3435 227d 2c0a 2020 2020  b0ca8145"},.    
-0001c460: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001c470: 352e 302e 322d 6370 3336 2d63 7033 366d  5.0.2-cp36-cp36m
-0001c480: 2d6d 7573 6c6c 696e 7578 5f31 5f31 5f78  -musllinux_1_1_x
-0001c490: 3836 5f36 342e 7768 6c22 2c20 6861 7368  86_64.whl", hash
-0001c4a0: 203d 2022 7368 6132 3536 3a32 3662 3033   = "sha256:26b03
-0001c4b0: 3538 6538 3933 3339 3930 3530 3266 3435  58e8933990502f45
-0001c4c0: 3133 6339 3931 6339 3933 3562 3663 3036  13c991c9935b6c06
-0001c4d0: 6166 3031 3738 3761 3336 6431 3333 6237  af01787a36d133b7
-0001c4e0: 6333 3962 3164 6633 3766 6122 7d2c 0a20  c39b1df37fa"},. 
-0001c4f0: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
-0001c500: 712d 3235 2e30 2e32 2d63 7033 362d 6370  q-25.0.2-cp36-cp
-0001c510: 3336 6d2d 7769 6e33 322e 7768 6c22 2c20  36m-win32.whl", 
-0001c520: 6861 7368 203d 2022 7368 6132 3536 3a63  hash = "sha256:c
-0001c530: 3866 6564 6333 6363 6436 3263 3662 3737  8fedc3ccd62c6b77
-0001c540: 6466 6536 6634 3338 3032 3035 3761 3830  dfe6f43802057a80
-0001c550: 3361 3431 3165 6539 3666 3134 6539 3436  3a411ee96f14e946
-0001c560: 6634 6137 3665 6334 6564 3065 3131 3722  f4a76ec4ed0e117"
-0001c570: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-0001c580: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
-0001c590: 362d 6370 3336 6d2d 7769 6e5f 616d 6436  6-cp36m-win_amd6
-0001c5a0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001c5b0: 7368 6132 3536 3a32 6461 3638 3133 6237  sha256:2da6813b7
-0001c5c0: 3939 3562 3662 3164 3133 3037 3332 3963  995b6b1d1307329c
-0001c5d0: 3733 6433 6533 6265 3266 6432 6437 3865  73d3e3be2fd2d78e
-0001c5e0: 3139 6163 6663 3465 6666 3265 3237 3236  19acfc4eff2e2726
-0001c5f0: 3237 3332 3338 3822 7d2c 0a20 2020 207b  2732388"},.    {
-0001c600: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
-0001c610: 2e30 2e32 2d63 7033 372d 6370 3337 6d2d  .0.2-cp37-cp37m-
-0001c620: 6d61 636f 7378 5f31 305f 395f 7838 365f  macosx_10_9_x86_
-0001c630: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001c640: 2273 6861 3235 363a 6133 3539 3630 6338  "sha256:a35960c8
-0001c650: 6232 6636 3365 3465 6636 3766 6436 3733  b2f63e4ef67fd673
-0001c660: 3138 3531 3033 3064 6636 3865 3462 3631  1851030df68e4b61
-0001c670: 3761 3637 3135 6464 3131 6234 6231 3033  7a6715dd11b4b103
-0001c680: 3132 6431 3966 6566 227d 2c0a 2020 2020  12d19fef"},.    
-0001c690: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001c6a0: 352e 302e 322d 6370 3337 2d63 7033 376d  5.0.2-cp37-cp37m
-0001c6b0: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
-0001c6c0: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
-0001c6d0: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
-0001c6e0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001c6f0: 3536 3a65 6566 3261 3062 3838 3061 6234  56:eef2a0b880ab4
-0001c700: 3061 6361 3561 3837 3839 3333 3337 3663  0aca5a878933376c
-0001c710: 6236 6331 6563 3438 3366 6261 3732 6637  b6c1ec483fba72f7
-0001c720: 6633 3465 3031 3563 3066 3637 3563 3930  f34e015c0f675c90
-0001c730: 6232 3022 7d2c 0a20 2020 207b 6669 6c65  b20"},.    {file
-0001c740: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001c750: 2d63 7033 372d 6370 3337 6d2d 6d61 6e79  -cp37-cp37m-many
-0001c760: 6c69 6e75 785f 325f 355f 6936 3836 2e6d  linux_2_5_i686.m
-0001c770: 616e 796c 696e 7578 315f 6936 3836 2e77  anylinux1_i686.w
-0001c780: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001c790: 3235 363a 3835 3736 3237 3132 6237 3463  256:85762712b74c
-0001c7a0: 3762 6431 3865 3334 3063 3336 3339 6431  7bd18e340c3639d1
-0001c7b0: 6266 3266 3233 3733 3561 3939 3864 3633  bf2f23735a998d63
-0001c7c0: 6634 3662 6236 3538 3464 3930 3462 3565  f46bb6584d904b5e
-0001c7d0: 3430 3164 227d 2c0a 2020 2020 7b66 696c  401d"},.    {fil
-0001c7e0: 6520 3d20 2270 797a 6d71 2d32 352e 302e  e = "pyzmq-25.0.
-0001c7f0: 322d 6370 3337 2d63 7033 376d 2d6d 616e  2-cp37-cp37m-man
-0001c800: 796c 696e 7578 5f32 5f35 5f78 3836 5f36  ylinux_2_5_x86_6
-0001c810: 342e 6d61 6e79 6c69 6e75 7831 5f78 3836  4.manylinux1_x86
-0001c820: 5f36 342e 7768 6c22 2c20 6861 7368 203d  _64.whl", hash =
-0001c830: 2022 7368 6132 3536 3a36 3438 3132 6632   "sha256:64812f2
-0001c840: 3964 3665 6565 3536 3565 3132 3963 6131  9d6eee565e129ca1
-0001c850: 3462 3063 3738 3537 3434 6266 6666 3637  4b0c785744bfff67
-0001c860: 3961 3437 3237 3133 3734 3834 3130 3162  9a4727137484101b
-0001c870: 3334 3630 3264 3161 3722 7d2c 0a20 2020  34602d1a7"},.   
-0001c880: 207b 6669 6c65 203d 2022 7079 7a6d 712d   {file = "pyzmq-
-0001c890: 3235 2e30 2e32 2d63 7033 372d 6370 3337  25.0.2-cp37-cp37
-0001c8a0: 6d2d 6d75 736c 6c69 6e75 785f 315f 315f  m-musllinux_1_1_
-0001c8b0: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
-0001c8c0: 7368 203d 2022 7368 6132 3536 3a35 3130  sh = "sha256:510
-0001c8d0: 6438 6535 3562 3361 3763 6431 3366 3864  d8e55b3a7cd13f8d
-0001c8e0: 3365 3931 3231 6564 6630 6138 3733 3062  3e9121edf0a8730b
-0001c8f0: 3837 6439 3235 6432 3532 3938 6261 6365  87d925d25298bace
-0001c900: 3239 6137 6537 6263 3832 3831 3022 7d2c  29a7e7bc82810"},
-0001c910: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-0001c920: 7a6d 712d 3235 2e30 2e32 2d63 7033 372d  zmq-25.0.2-cp37-
-0001c930: 6370 3337 6d2d 6d75 736c 6c69 6e75 785f  cp37m-musllinux_
-0001c940: 315f 315f 6936 3836 2e77 686c 222c 2068  1_1_i686.whl", h
-0001c950: 6173 6820 3d20 2273 6861 3235 363a 6231  ash = "sha256:b1
-0001c960: 3634 6363 3363 3861 6362 3364 3130 3265  64cc3c8acb3d102e
-0001c970: 3331 3166 3265 6236 6633 6333 3035 3836  311f2eb6f3c30586
-0001c980: 3565 6362 3337 3765 3536 6164 6330 3135  5ecb377e56adc015
-0001c990: 6362 3531 6637 3231 6631 6464 6136 227d  cb51f721f1dda6"}
-0001c9a0: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
-0001c9b0: 797a 6d71 2d32 352e 302e 322d 6370 3337  yzmq-25.0.2-cp37
-0001c9c0: 2d63 7033 376d 2d6d 7573 6c6c 696e 7578  -cp37m-musllinux
-0001c9d0: 5f31 5f31 5f78 3836 5f36 342e 7768 6c22  _1_1_x86_64.whl"
-0001c9e0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001c9f0: 3a32 3866 6462 3932 3234 6132 3538 3133  :28fdb9224a25813
-0001ca00: 3437 3834 6139 6366 3030 3962 3539 3236  4784a9cf009b5926
-0001ca10: 3561 3964 6465 3739 3538 3266 6237 3530  5a9dde79582fb750
-0001ca20: 6434 6538 3861 3662 6362 6336 6661 3364  d4e88a6bcbc6fa3d
-0001ca30: 6322 7d2c 0a20 2020 207b 6669 6c65 203d  c"},.    {file =
-0001ca40: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
-0001ca50: 7033 372d 6370 3337 6d2d 7769 6e33 322e  p37-cp37m-win32.
-0001ca60: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001ca70: 6132 3536 3a64 6437 3731 6134 3430 6566  a256:dd771a440ef
-0001ca80: 6661 3163 3336 6433 3532 3362 6336 6261  fa1c36d3523bc6ba
-0001ca90: 3465 3534 6666 3564 3265 3534 6234 6164  4e54ff5d2e54b4ad
-0001caa0: 6363 3165 3036 3064 3866 3363 6133 3732  cc1e060d8f3ca372
-0001cab0: 3164 3232 3822 7d2c 0a20 2020 207b 6669  1d228"},.    {fi
-0001cac0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
-0001cad0: 2e32 2d63 7033 372d 6370 3337 6d2d 7769  .2-cp37-cp37m-wi
-0001cae0: 6e5f 616d 6436 342e 7768 6c22 2c20 6861  n_amd64.whl", ha
-0001caf0: 7368 203d 2022 7368 6132 3536 3a39 6264  sh = "sha256:9bd
-0001cb00: 6334 3065 6662 3637 3962 3964 6363 3339  c40efb679b9dcc39
-0001cb10: 6330 3664 3235 3632 3965 3535 3538 3165  c06d25629e55581e
-0001cb20: 3463 3466 3738 3730 6135 6538 3864 6234  4c4f7870a5e88db4
-0001cb30: 6631 6335 3163 6532 3565 3230 6422 7d2c  f1c51ce25e20d"},
-0001cb40: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-0001cb50: 7a6d 712d 3235 2e30 2e32 2d63 7033 382d  zmq-25.0.2-cp38-
-0001cb60: 6370 3338 2d6d 6163 6f73 785f 3130 5f31  cp38-macosx_10_1
-0001cb70: 355f 756e 6976 6572 7361 6c32 2e77 686c  5_universal2.whl
-0001cb80: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001cb90: 363a 3166 3832 3930 3661 3264 3865 3465  6:1f82906a2d8e4e
-0001cba0: 6533 3130 6633 3034 3837 6231 3635 6537  e310f30487b165e7
-0001cbb0: 6363 3865 6430 3963 3030 3965 3435 3032  cc8ed09c009e4502
-0001cbc0: 6461 3637 3137 3862 3033 3038 3363 3463  da67178b03083c4c
-0001cbd0: 6530 227d 2c0a 2020 2020 7b66 696c 6520  e0"},.    {file 
-0001cbe0: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001cbf0: 6370 3338 2d63 7033 382d 6d61 636f 7378  cp38-cp38-macosx
-0001cc00: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
-0001cc10: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001cc20: 363a 3231 6563 3062 6634 3833 3139 3838  6:21ec0bf4831988
-0001cc30: 6166 3433 6338 6436 3662 6133 6363 6438  af43c8d66ba3ccd8
-0001cc40: 3161 6632 6335 6537 3933 6531 6266 3637  1af2c5e793e1bf67
-0001cc50: 3930 6562 3264 3530 6532 3762 3363 3537  90eb2d50e27b3c57
-0001cc60: 3061 227d 2c0a 2020 2020 7b66 696c 6520  0a"},.    {file 
-0001cc70: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001cc80: 6370 3338 2d63 7033 382d 6d61 6e79 6c69  cp38-cp38-manyli
-0001cc90: 6e75 785f 325f 3132 5f69 3638 362e 6d61  nux_2_12_i686.ma
-0001cca0: 6e79 6c69 6e75 7832 3031 305f 6936 3836  nylinux2010_i686
-0001ccb0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
-0001ccc0: 6861 3235 363a 6162 6263 6539 3832 6131  ha256:abbce982a1
-0001ccd0: 3763 3838 6432 3331 3265 6332 6366 3736  7c88d2312ec2cf76
-0001cce0: 3733 3938 3564 3434 3466 3162 6561 6163  73985d444f1beaac
-0001ccf0: 3665 3831 3839 3432 3465 3061 3065 3034  6e8189424e0a0e04
-0001cd00: 3438 6462 6233 227d 2c0a 2020 2020 7b66  48dbb3"},.    {f
-0001cd10: 696c 6520 3d20 2270 797a 6d71 2d32 352e  ile = "pyzmq-25.
-0001cd20: 302e 322d 6370 3338 2d63 7033 382d 6d61  0.2-cp38-cp38-ma
-0001cd30: 6e79 6c69 6e75 785f 325f 3132 5f78 3836  nylinux_2_12_x86
-0001cd40: 5f36 342e 6d61 6e79 6c69 6e75 7832 3031  _64.manylinux201
-0001cd50: 305f 7838 365f 3634 2e77 686c 222c 2068  0_x86_64.whl", h
-0001cd60: 6173 6820 3d20 2273 6861 3235 363a 3965  ash = "sha256:9e
-0001cd70: 3164 3266 3264 3836 6663 3735 6564 3766  1d2f2d86fc75ed7f
-0001cd80: 3838 3435 6139 3932 6335 6636 6631 6162  8845a992c5f6f1ab
-0001cd90: 3564 6239 3937 3437 6662 3064 3738 6235  5db99747fb0d78b5
-0001cda0: 6534 3034 3664 3034 3131 3634 6432 227d  e4046d041164d2"}
-0001cdb0: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
-0001cdc0: 797a 6d71 2d32 352e 302e 322d 6370 3338  yzmq-25.0.2-cp38
-0001cdd0: 2d63 7033 382d 6d61 6e79 6c69 6e75 785f  -cp38-manylinux_
-0001cde0: 325f 3137 5f61 6172 6368 3634 2e6d 616e  2_17_aarch64.man
-0001cdf0: 796c 696e 7578 3230 3134 5f61 6172 6368  ylinux2014_aarch
-0001ce00: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001ce10: 2273 6861 3235 363a 6132 6539 3266 6632  "sha256:a2e92ff2
-0001ce20: 3061 6435 6431 3332 3636 6263 3939 3961  0ad5d13266bc999a
-0001ce30: 3239 6564 3239 6133 6235 6231 3031 6332  29ed29a3b5b101c2
-0001ce40: 3166 6466 3462 3263 6634 3230 6330 3964  1fdf4b2cf420c09d
-0001ce50: 6239 6662 3639 3065 227d 2c0a 2020 2020  b9fb690e"},.    
-0001ce60: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001ce70: 352e 302e 322d 6370 3338 2d63 7033 382d  5.0.2-cp38-cp38-
-0001ce80: 6d75 736c 6c69 6e75 785f 315f 315f 6161  musllinux_1_1_aa
-0001ce90: 7263 6836 342e 7768 6c22 2c20 6861 7368  rch64.whl", hash
-0001cea0: 203d 2022 7368 6132 3536 3a65 6462 6266   = "sha256:edbbf
-0001ceb0: 3036 6363 3237 3139 3838 3934 3730 6138  06cc2719889470a8
-0001cec0: 6432 6266 3530 3732 6262 3030 6634 3233  d2bf5072bb00f423
-0001ced0: 6531 3264 6530 6562 3966 6665 6339 3436  e12de0eb9ffec946
-0001cee0: 6332 6339 3734 3865 3134 3922 7d2c 0a20  c2c9748e149"},. 
-0001cef0: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
-0001cf00: 712d 3235 2e30 2e32 2d63 7033 382d 6370  q-25.0.2-cp38-cp
-0001cf10: 3338 2d6d 7573 6c6c 696e 7578 5f31 5f31  38-musllinux_1_1
-0001cf20: 5f69 3638 362e 7768 6c22 2c20 6861 7368  _i686.whl", hash
-0001cf30: 203d 2022 7368 6132 3536 3a37 3739 3432   = "sha256:77942
-0001cf40: 3234 3366 6634 6431 3464 3930 6331 3162  243ff4d14d90c11b
-0001cf50: 3261 6664 3865 6536 6330 3339 6234 3561  2afd8ee6c039b45a
-0001cf60: 3062 6534 6535 3366 6236 6661 3766 3565  0be4e53fb6fa7f5e
-0001cf70: 3466 6430 6235 3964 6133 3922 7d2c 0a20  4fd0b59da39"},. 
-0001cf80: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
-0001cf90: 712d 3235 2e30 2e32 2d63 7033 382d 6370  q-25.0.2-cp38-cp
-0001cfa0: 3338 2d6d 7573 6c6c 696e 7578 5f31 5f31  38-musllinux_1_1
-0001cfb0: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
-0001cfc0: 7368 203d 2022 7368 6132 3536 3a61 6230  sh = "sha256:ab0
-0001cfd0: 3436 6539 6362 3930 3264 3166 3632 6339  46e9cb902d1f62c9
-0001cfe0: 6363 3065 6361 3035 3562 3164 3131 3130  cc0eca055b1d1110
-0001cff0: 3862 6463 3237 3163 6166 3763 3231 3731  8bdc271caf7c2171
-0001d000: 3438 3732 3938 6632 3239 6235 3622 7d2c  487298f229b56"},
-0001d010: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-0001d020: 7a6d 712d 3235 2e30 2e32 2d63 7033 382d  zmq-25.0.2-cp38-
-0001d030: 6370 3338 2d77 696e 3332 2e77 686c 222c  cp38-win32.whl",
-0001d040: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001d050: 6164 3736 3163 6662 6534 3737 3233 3638  ad761cfbe4772368
-0001d060: 3032 6137 6162 3263 3038 3064 3236 3863  02a7ab2c080d268c
-0001d070: 3935 6537 3834 6665 3330 6361 6661 3765  95e784fe30cafa7e
-0001d080: 3035 3561 6163 6431 6361 3837 3765 6230  055aacd1ca877eb0
-0001d090: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001d0a0: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
-0001d0b0: 3338 2d63 7033 382d 7769 6e5f 616d 6436  38-cp38-win_amd6
-0001d0c0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001d0d0: 7368 6132 3536 3a38 3536 3037 3536 3331  sha256:856075631
-0001d0e0: 3865 6337 6334 6334 3964 3263 3334 3130  8ec7c4c49d2c3410
-0001d0f0: 3132 3136 3765 3730 3462 3561 3436 6439  12167e704b5a46d9
-0001d100: 3033 3439 3035 3835 3363 3364 3161 6465  034905853c3d1ade
-0001d110: 3466 3535 6265 6522 7d2c 0a20 2020 207b  4f55bee"},.    {
-0001d120: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
-0001d130: 2e30 2e32 2d63 7033 392d 6370 3339 2d6d  .0.2-cp39-cp39-m
-0001d140: 6163 6f73 785f 3130 5f31 355f 756e 6976  acosx_10_15_univ
-0001d150: 6572 7361 6c32 2e77 686c 222c 2068 6173  ersal2.whl", has
-0001d160: 6820 3d20 2273 6861 3235 363a 6162 3263  h = "sha256:ab2c
-0001d170: 3035 3661 6335 3033 6632 3561 3633 6636  056ac503f25a63f6
-0001d180: 6338 6336 3737 3133 3733 6532 6137 3131  c8c6771373e2a711
-0001d190: 6239 3862 3330 3436 3134 3135 3164 6662  b98b304614151dfb
-0001d1a0: 3535 3264 3364 3663 3831 6636 227d 2c0a  552d3d6c81f6"},.
-0001d1b0: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
-0001d1c0: 6d71 2d32 352e 302e 322d 6370 3339 2d63  mq-25.0.2-cp39-c
-0001d1d0: 7033 392d 6d61 636f 7378 5f31 305f 395f  p39-macosx_10_9_
-0001d1e0: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
-0001d1f0: 6820 3d20 2273 6861 3235 363a 6363 6138  h = "sha256:cca8
-0001d200: 3532 3462 3631 6330 6561 6161 3335 3035  524b61c0eaaa3505
-0001d210: 3338 3264 6339 6239 6133 6263 3831 3635  382dc9b9a3bc8165
-0001d220: 6631 6436 6330 3130 6664 6431 3435 3263  f1d6c010fdd1452c
-0001d230: 3232 3432 3235 6132 3636 3839 227d 2c0a  224225a26689"},.
-0001d240: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
-0001d250: 6d71 2d32 352e 302e 322d 6370 3339 2d63  mq-25.0.2-cp39-c
-0001d260: 7033 392d 6d61 6e79 6c69 6e75 785f 325f  p39-manylinux_2_
-0001d270: 3132 5f69 3638 362e 6d61 6e79 6c69 6e75  12_i686.manylinu
-0001d280: 7832 3031 305f 6936 3836 2e77 686c 222c  x2010_i686.whl",
-0001d290: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001d2a0: 6366 6239 6637 6561 6530 3264 3361 6334  cfb9f7eae02d3ac4
-0001d2b0: 3266 6265 6461 6433 3030 3036 6237 3430  2fbedad30006b740
-0001d2c0: 3763 3938 3461 3065 6234 3138 3961 3133  7c984a0eb4189a13
-0001d2d0: 3232 3234 3161 3230 3934 3464 3631 6535  22241a20944d61e5
-0001d2e0: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001d2f0: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
-0001d300: 3339 2d63 7033 392d 6d61 6e79 6c69 6e75  39-cp39-manylinu
-0001d310: 785f 325f 3132 5f78 3836 5f36 342e 6d61  x_2_12_x86_64.ma
-0001d320: 6e79 6c69 6e75 7832 3031 305f 7838 365f  nylinux2010_x86_
-0001d330: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001d340: 2273 6861 3235 363a 3565 6165 6165 3033  "sha256:5eaeae03
-0001d350: 3863 3638 3734 3830 3832 3133 3764 3638  8c68748082137d68
-0001d360: 3936 6435 6334 6462 3739 3237 6539 3334  96d5c4db7927e934
-0001d370: 3932 3337 6465 6430 3865 6531 6262 6439  9237ded08ee1bbd9
-0001d380: 3466 3733 3631 6339 227d 2c0a 2020 2020  4f7361c9"},.    
-0001d390: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001d3a0: 352e 302e 322d 6370 3339 2d63 7033 392d  5.0.2-cp39-cp39-
-0001d3b0: 6d61 6e79 6c69 6e75 785f 325f 3137 5f61  manylinux_2_17_a
-0001d3c0: 6172 6368 3634 2e6d 616e 796c 696e 7578  arch64.manylinux
-0001d3d0: 3230 3134 5f61 6172 6368 3634 2e77 686c  2014_aarch64.whl
-0001d3e0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001d3f0: 363a 3461 3331 3939 3261 3866 3864 3531  6:4a31992a8f8d51
-0001d400: 3636 3365 6266 3739 6466 3064 6636 6130  663ebf79df0df6a0
-0001d410: 3466 6662 3930 3530 3633 3038 3364 3638  4ffb905063083d68
-0001d420: 3264 3433 3830 6162 3864 3263 3637 3235  2d4380ab8d2c6725
-0001d430: 3763 227d 2c0a 2020 2020 7b66 696c 6520  7c"},.    {file 
-0001d440: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001d450: 6370 3339 2d63 7033 392d 6d75 736c 6c69  cp39-cp39-muslli
-0001d460: 6e75 785f 315f 315f 6161 7263 6836 342e  nux_1_1_aarch64.
-0001d470: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001d480: 6132 3536 3a36 6139 3739 6535 3964 3231  a256:6a979e59d21
-0001d490: 3834 6130 6338 6632 6564 6534 6230 3831  84a0c8f2ede4b081
-0001d4a0: 3063 6264 6438 3662 3634 6439 3964 3963  0cbdd86b64d99d9c
-0001d4b0: 6338 6130 3233 3932 3965 3430 6463 6537  c8a023929e40dce7
-0001d4c0: 6338 3663 6322 7d2c 0a20 2020 207b 6669  c86cc"},.    {fi
-0001d4d0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
-0001d4e0: 2e32 2d63 7033 392d 6370 3339 2d6d 7573  .2-cp39-cp39-mus
-0001d4f0: 6c6c 696e 7578 5f31 5f31 5f69 3638 362e  llinux_1_1_i686.
-0001d500: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001d510: 6132 3536 3a31 6631 3234 6362 3733 6631  a256:1f124cb73f1
-0001d520: 6161 3636 3534 6433 3162 3138 3338 3130  aa6654d31b183810
-0001d530: 6665 6263 3835 3035 6664 3063 3539 3761  febc8505fd0c597a
-0001d540: 6661 3132 3763 3466 3430 3037 3662 6534  fa127c4f40076be4
-0001d550: 3537 3465 3022 7d2c 0a20 2020 207b 6669  574e0"},.    {fi
-0001d560: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
-0001d570: 2e32 2d63 7033 392d 6370 3339 2d6d 7573  .2-cp39-cp39-mus
-0001d580: 6c6c 696e 7578 5f31 5f31 5f78 3836 5f36  llinux_1_1_x86_6
-0001d590: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-0001d5a0: 7368 6132 3536 3a36 3563 3139 6136 3362  sha256:65c19a63b
-0001d5b0: 3461 3833 6165 3435 6436 3231 3738 6237  4a83ae45d62178b7
-0001d5c0: 3032 3233 6164 6565 6535 6631 3266 3330  0223adeee5f12f30
-0001d5d0: 3332 3732 3662 3839 3734 3331 6236 3535  32726b897431b655
-0001d5e0: 3361 6132 3561 6622 7d2c 0a20 2020 207b  3aa25af"},.    {
-0001d5f0: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
-0001d600: 2e30 2e32 2d63 7033 392d 6370 3339 2d77  .0.2-cp39-cp39-w
-0001d610: 696e 3332 2e77 686c 222c 2068 6173 6820  in32.whl", hash 
-0001d620: 3d20 2273 6861 3235 363a 3833 6438 3232  = "sha256:83d822
-0001d630: 6538 3638 3736 3231 6265 6438 3734 3034  e8687621bed87404
-0001d640: 6166 6331 6330 3364 3833 6661 3263 6533  afc1c03d83fa2ce3
-0001d650: 3937 3333 6435 3463 3266 6435 3264 3838  9733d54c2fd52d88
-0001d660: 3239 6564 6238 6137 6666 227d 2c0a 2020  29edb8a7ff"},.  
-0001d670: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
-0001d680: 2d32 352e 302e 322d 6370 3339 2d63 7033  -25.0.2-cp39-cp3
-0001d690: 392d 7769 6e5f 616d 6436 342e 7768 6c22  9-win_amd64.whl"
-0001d6a0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001d6b0: 3a32 3436 3833 3238 3563 6336 6237 6266  :24683285cc6b7bf
-0001d6c0: 3138 6164 3337 6437 3562 3964 6230 6530  18ad37d75b9db0e0
-0001d6d0: 6665 6665 3538 3430 3465 3730 3031 6631  fefe58404e7001f1
-0001d6e0: 6438 3262 6639 6537 3231 3830 3664 6161  d82bf9e721806daa
-0001d6f0: 3722 7d2c 0a20 2020 207b 6669 6c65 203d  7"},.    {file =
-0001d700: 2022 7079 7a6d 712d 3235 2e30 2e32 2d70   "pyzmq-25.0.2-p
-0001d710: 7033 372d 7079 7079 3337 5f70 7037 332d  p37-pypy37_pp73-
-0001d720: 6d61 636f 7378 5f31 305f 395f 7838 365f  macosx_10_9_x86_
-0001d730: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001d740: 2273 6861 3235 363a 3461 3462 3432 3631  "sha256:4a4b4261
-0001d750: 6562 3866 3965 6437 3166 3633 6239 6562  eb8f9ed71f63b9eb
-0001d760: 3031 3938 6464 3763 3933 3461 6133 6233  0198dd7c934aa3b3
-0001d770: 3937 3264 6163 3538 3664 3065 6635 3032  972dac586d0ef502
-0001d780: 6261 3961 6230 3862 227d 2c0a 2020 2020  ba9ab08b"},.    
-0001d790: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001d7a0: 352e 302e 322d 7070 3337 2d70 7970 7933  5.0.2-pp37-pypy3
-0001d7b0: 375f 7070 3733 2d6d 616e 796c 696e 7578  7_pp73-manylinux
-0001d7c0: 5f32 5f31 325f 6936 3836 2e6d 616e 796c  _2_12_i686.manyl
-0001d7d0: 696e 7578 3230 3130 5f69 3638 362e 7768  inux2010_i686.wh
-0001d7e0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001d7f0: 3536 3a36 3265 6338 6439 3739 6635 3663  56:62ec8d979f56c
-0001d800: 3030 3533 6139 3262 3262 3661 3130 6666  0053a92b2b6a10ff
-0001d810: 3534 6239 6563 3861 3466 3138 3764 6232  54b9ec8a4f187db2
-0001d820: 6236 6563 3331 6565 3364 6436 6433 6361  b6ec31ee3dd6d3ca
-0001d830: 3665 3222 7d2c 0a20 2020 207b 6669 6c65  6e2"},.    {file
-0001d840: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001d850: 2d70 7033 372d 7079 7079 3337 5f70 7037  -pp37-pypy37_pp7
-0001d860: 332d 6d61 6e79 6c69 6e75 785f 325f 3132  3-manylinux_2_12
-0001d870: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
-0001d880: 7832 3031 305f 7838 365f 3634 2e77 686c  x2010_x86_64.whl
-0001d890: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001d8a0: 363a 6166 6665 6331 3437 3033 3531 3137  6:affec147035117
-0001d8b0: 3865 3839 3231 3231 6233 3431 3463 3865  8e892121b3414c8e
-0001d8c0: 6637 3830 3332 3639 6632 3037 6266 3962  f7803269f207bf9b
-0001d8d0: 6566 3835 6639 6136 6464 3131 6364 6532  ef85f9a6dd11cde2
-0001d8e0: 3634 227d 2c0a 2020 2020 7b66 696c 6520  64"},.    {file 
-0001d8f0: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001d900: 7070 3337 2d70 7970 7933 375f 7070 3733  pp37-pypy37_pp73
-0001d910: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
-0001d920: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
-0001d930: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
-0001d940: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001d950: 3536 3a66 6663 3731 3131 3134 3333 6264  56:ffc71111433bd
-0001d960: 3665 6338 3630 3761 3337 6239 3231 3166  6ec8607a37b9211f
-0001d970: 3465 6634 3265 3364 3362 3237 3163 3664  4ef42e3d3b271c6d
-0001d980: 3736 6338 3133 3636 3938 3334 3736 3462  76c813669834764b
-0001d990: 3234 3822 7d2c 0a20 2020 207b 6669 6c65  248"},.    {file
-0001d9a0: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001d9b0: 2d70 7033 372d 7079 7079 3337 5f70 7037  -pp37-pypy37_pp7
-0001d9c0: 332d 7769 6e5f 616d 6436 342e 7768 6c22  3-win_amd64.whl"
-0001d9d0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001d9e0: 3a36 6661 6463 3630 3937 3037 3134 6438  :6fadc60970714d8
-0001d9f0: 3665 6666 3237 3832 3166 3866 6230 3166  6eff27821f8fb01f
-0001da00: 3833 3238 6464 3336 6265 6264 3439 3662  8328dd36bebd496b
-0001da10: 3035 3634 6135 3030 6665 3461 3965 3335  0564a500fe4a9e35
-0001da20: 3422 7d2c 0a20 2020 207b 6669 6c65 203d  4"},.    {file =
-0001da30: 2022 7079 7a6d 712d 3235 2e30 2e32 2d70   "pyzmq-25.0.2-p
-0001da40: 7033 382d 7079 7079 3338 5f70 7037 332d  p38-pypy38_pp73-
-0001da50: 6d61 636f 7378 5f31 305f 395f 7838 365f  macosx_10_9_x86_
-0001da60: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001da70: 2273 6861 3235 363a 3236 3939 3638 6632  "sha256:269968f2
-0001da80: 6137 3663 3035 3133 3439 3061 6562 3362  a76c0513490aeb3b
-0001da90: 6130 6463 3363 3737 6237 6337 6131 3164  a0dc3c77b7c7a11d
-0001daa0: 6161 3839 3466 3964 3164 6138 3864 3461  aa894f9d1da88d4a
-0001dab0: 3064 6230 3938 3335 227d 2c0a 2020 2020  0db09835"},.    
-0001dac0: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001dad0: 352e 302e 322d 7070 3338 2d70 7970 7933  5.0.2-pp38-pypy3
-0001dae0: 385f 7070 3733 2d6d 616e 796c 696e 7578  8_pp73-manylinux
-0001daf0: 5f32 5f31 325f 6936 3836 2e6d 616e 796c  _2_12_i686.manyl
-0001db00: 696e 7578 3230 3130 5f69 3638 362e 7768  inux2010_i686.wh
-0001db10: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001db20: 3536 3a66 3763 3862 3833 3638 6538 3433  56:f7c8b8368e843
-0001db30: 3831 6165 3763 3537 6631 6635 3238 3362  81ae7c57f1f5283b
-0001db40: 3032 3963 3838 3835 3034 6161 6634 3934  029c888504aaf494
-0001db50: 3963 3332 6536 6536 6662 3235 3665 6339  9c32e6e6fb256ec9
-0001db60: 6266 3022 7d2c 0a20 2020 207b 6669 6c65  bf0"},.    {file
-0001db70: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001db80: 2d70 7033 382d 7079 7079 3338 5f70 7037  -pp38-pypy38_pp7
-0001db90: 332d 6d61 6e79 6c69 6e75 785f 325f 3132  3-manylinux_2_12
-0001dba0: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
-0001dbb0: 7832 3031 305f 7838 365f 3634 2e77 686c  x2010_x86_64.whl
-0001dbc0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001dbd0: 363a 3235 6536 3837 3361 3730 6164 3561  6:25e6873a70ad5a
-0001dbe0: 6133 3165 3461 3763 3431 6535 6538 6337  a31e4a7c41e5e8c7
-0001dbf0: 3039 3239 3665 6465 6634 6139 3233 3133  09296edef4a92313
-0001dc00: 6531 6364 3566 6338 3762 6264 3138 3734  e1cd5fc87bbd1874
-0001dc10: 6532 227d 2c0a 2020 2020 7b66 696c 6520  e2"},.    {file 
-0001dc20: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
-0001dc30: 7070 3338 2d70 7970 7933 385f 7070 3733  pp38-pypy38_pp73
-0001dc40: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
-0001dc50: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
-0001dc60: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
-0001dc70: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001dc80: 3536 3a62 3733 3330 3736 6666 3436 6537  56:b733076ff46e7
-0001dc90: 6462 3535 3034 6335 6537 3238 3466 3034  db5504c5e7284f04
-0001dca0: 6139 3835 3263 3633 3231 3463 3734 3638  a9852c63214c7468
-0001dcb0: 3862 6462 3631 3335 3830 3835 3331 3735  8bdb613580853175
-0001dcc0: 3561 3322 7d2c 0a20 2020 207b 6669 6c65  5a3"},.    {file
-0001dcd0: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001dce0: 2d70 7033 382d 7079 7079 3338 5f70 7037  -pp38-pypy38_pp7
-0001dcf0: 332d 7769 6e5f 616d 6436 342e 7768 6c22  3-win_amd64.whl"
-0001dd00: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001dd10: 3a61 3666 3661 6531 3234 3738 6664 6332  :a6f6ae12478fdc2
-0001dd20: 3661 3664 3566 6462 3231 6638 3036 6230  6a6d5fdb21f806b0
-0001dd30: 3866 6135 3430 3363 6430 3266 6433 3132  8fa5403cd02fd312
-0001dd40: 6534 6362 3566 3732 6466 3037 3866 3936  e4cb5f72df078f96
-0001dd50: 6622 7d2c 0a20 2020 207b 6669 6c65 203d  f"},.    {file =
-0001dd60: 2022 7079 7a6d 712d 3235 2e30 2e32 2d70   "pyzmq-25.0.2-p
-0001dd70: 7033 392d 7079 7079 3339 5f70 7037 332d  p39-pypy39_pp73-
-0001dd80: 6d61 636f 7378 5f31 305f 395f 7838 365f  macosx_10_9_x86_
-0001dd90: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001dda0: 2273 6861 3235 363a 3637 6461 3163 3231  "sha256:67da1c21
-0001ddb0: 3366 6264 3230 3839 3036 6162 3334 3730  3fbd208906ab3470
-0001ddc0: 6366 6666 3165 6530 3034 3838 3338 3336  cfff1ee004883836
-0001ddd0: 3531 3335 6139 6264 6463 3762 3430 6231  5135a9bddc7b40b1
-0001dde0: 3165 3664 3663 3839 227d 2c0a 2020 2020  1e6d6c89"},.    
-0001ddf0: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
-0001de00: 352e 302e 322d 7070 3339 2d70 7970 7933  5.0.2-pp39-pypy3
-0001de10: 395f 7070 3733 2d6d 616e 796c 696e 7578  9_pp73-manylinux
-0001de20: 5f32 5f31 375f 6161 7263 6836 342e 6d61  _2_17_aarch64.ma
-0001de30: 6e79 6c69 6e75 7832 3031 345f 6161 7263  nylinux2014_aarc
-0001de40: 6836 342e 7768 6c22 2c20 6861 7368 203d  h64.whl", hash =
-0001de50: 2022 7368 6132 3536 3a35 3331 6533 3664   "sha256:531e36d
-0001de60: 3966 6364 3636 6631 3864 6532 3734 3334  9fcd66f18de27434
-0001de70: 6132 3562 3531 6431 3337 6562 3534 3639  a25b51d137eb5469
-0001de80: 3331 3033 3366 3339 3265 3835 3637 3463  31033f392e85674c
-0001de90: 3761 3763 6561 3835 3322 7d2c 0a20 2020  7a7cea853"},.   
-0001dea0: 207b 6669 6c65 203d 2022 7079 7a6d 712d   {file = "pyzmq-
-0001deb0: 3235 2e30 2e32 2d70 7033 392d 7079 7079  25.0.2-pp39-pypy
-0001dec0: 3339 5f70 7037 332d 6d61 6e79 6c69 6e75  39_pp73-manylinu
-0001ded0: 785f 325f 3137 5f69 3638 362e 6d61 6e79  x_2_17_i686.many
-0001dee0: 6c69 6e75 7832 3031 345f 6936 3836 2e77  linux2014_i686.w
-0001def0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001df00: 3235 363a 3334 6136 6664 6464 3135 3966  256:34a6fddd159f
-0001df10: 6633 3861 6139 3439 3762 3265 3334 3261  f38aa9497b2e342a
-0001df20: 3535 3966 3134 3261 6233 3635 3537 3632  559f142ab3655762
-0001df30: 3834 6263 3866 3737 6362 3365 6164 3166  84bc8f77cb3ead1f
-0001df40: 3739 6335 227d 2c0a 2020 2020 7b66 696c  79c5"},.    {fil
-0001df50: 6520 3d20 2270 797a 6d71 2d32 352e 302e  e = "pyzmq-25.0.
-0001df60: 322d 7070 3339 2d70 7970 7933 395f 7070  2-pp39-pypy39_pp
-0001df70: 3733 2d6d 616e 796c 696e 7578 5f32 5f31  73-manylinux_2_1
-0001df80: 375f 7838 365f 3634 2e6d 616e 796c 696e  7_x86_64.manylin
-0001df90: 7578 3230 3134 5f78 3836 5f36 342e 7768  ux2014_x86_64.wh
-0001dfa0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001dfb0: 3536 3a62 3439 3139 3938 6566 3838 3636  56:b491998ef8866
-0001dfc0: 3632 6331 6633 6434 3965 6132 3139 3830  62c1f3d49ea21980
-0001dfd0: 3535 6139 6135 3336 6464 6637 3433 3062  55a9a536ddf7430b
-0001dfe0: 3035 3162 3231 3035 3466 3261 3538 3331  051b21054f2a5831
-0001dff0: 3830 3022 7d2c 0a20 2020 207b 6669 6c65  800"},.    {file
-0001e000: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
-0001e010: 2d70 7033 392d 7079 7079 3339 5f70 7037  -pp39-pypy39_pp7
-0001e020: 332d 6d61 6e79 6c69 6e75 785f 325f 3238  3-manylinux_2_28
-0001e030: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
-0001e040: 7368 203d 2022 7368 6132 3536 3a35 6434  sh = "sha256:5d4
-0001e050: 3936 3831 3530 3734 6533 6533 6431 3833  96815074e3e3d183
-0001e060: 6665 3263 3766 6365 6132 3130 3961 6436  fe2c7fcea2109ad6
-0001e070: 3762 3734 3038 3463 3235 3434 3831 6638  7b74084c254481f8
-0001e080: 3762 3634 6530 3465 3961 3437 3122 7d2c  7b64e04e9a471"},
-0001e090: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
-0001e0a0: 7a6d 712d 3235 2e30 2e32 2d70 7033 392d  zmq-25.0.2-pp39-
-0001e0b0: 7079 7079 3339 5f70 7037 332d 7769 6e5f  pypy39_pp73-win_
-0001e0c0: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
-0001e0d0: 203d 2022 7368 6132 3536 3a35 3661 3934   = "sha256:56a94
-0001e0e0: 6162 3164 3132 6166 3938 3262 3535 6361  ab1d12af982b55ca
-0001e0f0: 3936 6336 3835 3364 6236 6163 3835 3530  96c6853db6ac8550
-0001e100: 3565 3832 3064 3934 3538 6163 3736 3336  5e820d9458ac7636
-0001e110: 3463 3139 3938 3937 3266 3422 7d2c 0a20  4c1998972f4"},. 
-0001e120: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
-0001e130: 712d 3235 2e30 2e32 2e74 6172 2e67 7a22  q-25.0.2.tar.gz"
-0001e140: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001e150: 3a36 6238 6331 6262 6237 3065 3836 3864  :6b8c1bbb70e868d
-0001e160: 6338 3838 3031 6161 3533 3263 6165 3662  c88801aa532cae6b
-0001e170: 6434 6533 6235 3233 3337 3834 3639 3262  d4e3b5233784692b
-0001e180: 3738 3666 3137 6164 3239 3632 6535 3134  786f17ad2962e514
-0001e190: 3922 7d2c 0a5d 0a0a 5b70 6163 6b61 6765  9"},.]..[package
-0001e1a0: 2e64 6570 656e 6465 6e63 6965 735d 0a63  .dependencies].c
-0001e1b0: 6666 6920 3d20 7b76 6572 7369 6f6e 203d  ffi = {version =
-0001e1c0: 2022 2a22 2c20 6d61 726b 6572 7320 3d20   "*", markers = 
-0001e1d0: 2269 6d70 6c65 6d65 6e74 6174 696f 6e5f  "implementation_
-0001e1e0: 6e61 6d65 203d 3d20 5c22 7079 7079 5c22  name == \"pypy\"
-0001e1f0: 227d 0a0a 5b5b 7061 636b 6167 655d 5d0a  "}..[[package]].
-0001e200: 6e61 6d65 203d 2022 7265 7175 6573 7473  name = "requests
-0001e210: 220a 7665 7273 696f 6e20 3d20 2232 2e33  ".version = "2.3
-0001e220: 312e 3022 0a64 6573 6372 6970 7469 6f6e  1.0".description
-0001e230: 203d 2022 5079 7468 6f6e 2048 5454 5020   = "Python HTTP 
-0001e240: 666f 7220 4875 6d61 6e73 2e22 0a6f 7074  for Humans.".opt
-0001e250: 696f 6e61 6c20 3d20 6661 6c73 650a 7079  ional = false.py
-0001e260: 7468 6f6e 2d76 6572 7369 6f6e 7320 3d20  thon-versions = 
-0001e270: 223e 3d33 2e37 220a 6669 6c65 7320 3d20  ">=3.7".files = 
-0001e280: 5b0a 2020 2020 7b66 696c 6520 3d20 2272  [.    {file = "r
-0001e290: 6571 7565 7374 732d 322e 3331 2e30 2d70  equests-2.31.0-p
-0001e2a0: 7933 2d6e 6f6e 652d 616e 792e 7768 6c22  y3-none-any.whl"
-0001e2b0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-0001e2c0: 3a35 3863 6432 3138 3763 3031 6537 3065  :58cd2187c01e70e
-0001e2d0: 3665 3236 3530 3562 6361 3735 3137 3737  6e26505bca751777
-0001e2e0: 6161 3966 3265 6530 6237 6634 3330 3039  aa9f2ee0b7f43009
-0001e2f0: 3838 6237 3039 6634 3465 3031 3330 3033  88b709f44e013003
-0001e300: 6622 7d2c 0a20 2020 207b 6669 6c65 203d  f"},.    {file =
-0001e310: 2022 7265 7175 6573 7473 2d32 2e33 312e   "requests-2.31.
-0001e320: 302e 7461 722e 677a 222c 2068 6173 6820  0.tar.gz", hash 
-0001e330: 3d20 2273 6861 3235 363a 3934 3263 3561  = "sha256:942c5a
-0001e340: 3735 3866 3938 6437 3930 6561 6564 3161  758f98d790eaed1a
-0001e350: 3239 6362 3665 6566 6337 6666 6230 6431  29cb6eefc7ffb0d1
-0001e360: 6366 3761 6630 3563 3364 3237 3931 3635  cf7af05c3d279165
-0001e370: 3664 6264 3661 6431 6531 227d 2c0a 5d0a  6dbd6ad1e1"},.].
-0001e380: 0a5b 7061 636b 6167 652e 6465 7065 6e64  .[package.depend
-0001e390: 656e 6369 6573 5d0a 6365 7274 6966 6920  encies].certifi 
-0001e3a0: 3d20 223e 3d32 3031 372e 342e 3137 220a  = ">=2017.4.17".
-0001e3b0: 6368 6172 7365 742d 6e6f 726d 616c 697a  charset-normaliz
-0001e3c0: 6572 203d 2022 3e3d 322c 3c34 220a 6964  er = ">=2,<4".id
-0001e3d0: 6e61 203d 2022 3e3d 322e 352c 3c34 220a  na = ">=2.5,<4".
-0001e3e0: 7572 6c6c 6962 3320 3d20 223e 3d31 2e32  urllib3 = ">=1.2
-0001e3f0: 312e 312c 3c33 220a 0a5b 7061 636b 6167  1.1,<3"..[packag
-0001e400: 652e 6578 7472 6173 5d0a 736f 636b 7320  e.extras].socks 
-0001e410: 3d20 5b22 5079 536f 636b 7320 283e 3d31  = ["PySocks (>=1
-0001e420: 2e35 2e36 2c21 3d31 2e35 2e37 2922 5d0a  .5.6,!=1.5.7)"].
-0001e430: 7573 652d 6368 6172 6465 742d 6f6e 2d70  use-chardet-on-p
-0001e440: 7933 203d 205b 2263 6861 7264 6574 2028  y3 = ["chardet (
-0001e450: 3e3d 332e 302e 322c 3c36 2922 5d0a 0a5b  >=3.0.2,<6)"]..[
-0001e460: 5b70 6163 6b61 6765 5d5d 0a6e 616d 6520  [package]].name 
-0001e470: 3d20 2273 6574 7570 746f 6f6c 7322 0a76  = "setuptools".v
-0001e480: 6572 7369 6f6e 203d 2022 3637 2e38 2e30  ersion = "67.8.0
-0001e490: 220a 6465 7363 7269 7074 696f 6e20 3d20  ".description = 
-0001e4a0: 2245 6173 696c 7920 646f 776e 6c6f 6164  "Easily download
-0001e4b0: 2c20 6275 696c 642c 2069 6e73 7461 6c6c  , build, install
-0001e4c0: 2c20 7570 6772 6164 652c 2061 6e64 2075  , upgrade, and u
-0001e4d0: 6e69 6e73 7461 6c6c 2050 7974 686f 6e20  ninstall Python 
-0001e4e0: 7061 636b 6167 6573 220a 6f70 7469 6f6e  packages".option
-0001e4f0: 616c 203d 2066 616c 7365 0a70 7974 686f  al = false.pytho
-0001e500: 6e2d 7665 7273 696f 6e73 203d 2022 3e3d  n-versions = ">=
-0001e510: 332e 3722 0a66 696c 6573 203d 205b 0a20  3.7".files = [. 
-0001e520: 2020 207b 6669 6c65 203d 2022 7365 7475     {file = "setu
-0001e530: 7074 6f6f 6c73 2d36 372e 382e 302d 7079  ptools-67.8.0-py
-0001e540: 332d 6e6f 6e65 2d61 6e79 2e77 686c 222c  3-none-any.whl",
-0001e550: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001e560: 3564 6636 3162 6633 3062 6231 3063 3666  5df61bf30bb10c6f
-0001e570: 3735 3665 6231 3965 3763 3966 3362 3437  756eb19e7c9f3b47
-0001e580: 3330 3531 6634 3864 6237 3766 6464 6265  3051f48db77fddbe
-0001e590: 3036 6666 3263 6133 3037 6466 3961 3666  06ff2ca307df9a6f
-0001e5a0: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001e5b0: 2273 6574 7570 746f 6f6c 732d 3637 2e38  "setuptools-67.8
-0001e5c0: 2e30 2e74 6172 2e67 7a22 2c20 6861 7368  .0.tar.gz", hash
-0001e5d0: 203d 2022 7368 6132 3536 3a36 3236 3432   = "sha256:62642
-0001e5e0: 3335 3861 6463 3737 6666 6138 3732 3333  358adc77ffa87233
-0001e5f0: 6263 3464 3233 3534 6334 6232 3638 3264  bc4d2354c4b2682d
-0001e600: 3231 3430 3438 6635 3030 3936 3464 6265  214048f500964dbe
-0001e610: 3736 3063 6365 6466 3130 3222 7d2c 0a5d  760ccedf102"},.]
-0001e620: 0a0a 5b70 6163 6b61 6765 2e65 7874 7261  ..[package.extra
-0001e630: 735d 0a64 6f63 7320 3d20 5b22 6675 726f  s].docs = ["furo
-0001e640: 222c 2022 6a61 7261 636f 2e70 6163 6b61  ", "jaraco.packa
-0001e650: 6769 6e67 2028 3e3d 3929 222c 2022 6a61  ging (>=9)", "ja
-0001e660: 7261 636f 2e74 6964 656c 6966 7420 283e  raco.tidelift (>
-0001e670: 3d31 2e34 2922 2c20 2270 7967 6d65 6e74  =1.4)", "pygment
-0001e680: 732d 6769 7468 7562 2d6c 6578 6572 7320  s-github-lexers 
-0001e690: 283d 3d30 2e30 2e35 2922 2c20 2272 7374  (==0.0.5)", "rst
-0001e6a0: 2e6c 696e 6b65 7220 283e 3d31 2e39 2922  .linker (>=1.9)"
-0001e6b0: 2c20 2273 7068 696e 7820 283e 3d33 2e35  , "sphinx (>=3.5
-0001e6c0: 2922 2c20 2273 7068 696e 782d 6661 7669  )", "sphinx-favi
-0001e6d0: 636f 6e22 2c20 2273 7068 696e 782d 686f  con", "sphinx-ho
-0001e6e0: 7665 7278 7265 6620 283c 3229 222c 2022  verxref (<2)", "
-0001e6f0: 7370 6869 6e78 2d69 6e6c 696e 652d 7461  sphinx-inline-ta
-0001e700: 6273 222c 2022 7370 6869 6e78 2d6c 696e  bs", "sphinx-lin
-0001e710: 7422 2c20 2273 7068 696e 782d 6e6f 7466  t", "sphinx-notf
-0001e720: 6f75 6e64 2d70 6167 6520 283d 3d30 2e38  ound-page (==0.8
-0001e730: 2e33 2922 2c20 2273 7068 696e 782d 7265  .3)", "sphinx-re
-0001e740: 7265 6469 7265 6374 7322 2c20 2273 7068  redirects", "sph
-0001e750: 696e 7863 6f6e 7472 6962 2d74 6f77 6e63  inxcontrib-townc
-0001e760: 7269 6572 225d 0a74 6573 7469 6e67 203d  rier"].testing =
-0001e770: 205b 2262 7569 6c64 5b76 6972 7475 616c   ["build[virtual
-0001e780: 656e 765d 222c 2022 6669 6c65 6c6f 636b  env]", "filelock
-0001e790: 2028 3e3d 332e 342e 3029 222c 2022 666c   (>=3.4.0)", "fl
-0001e7a0: 616b 6538 2d32 3032 3022 2c20 2269 6e69  ake8-2020", "ini
-0001e7b0: 3274 6f6d 6c5b 6c69 7465 5d20 283e 3d30  2toml[lite] (>=0
-0001e7c0: 2e39 2922 2c20 226a 6172 6163 6f2e 656e  .9)", "jaraco.en
-0001e7d0: 7673 2028 3e3d 322e 3229 222c 2022 6a61  vs (>=2.2)", "ja
-0001e7e0: 7261 636f 2e70 6174 6820 283e 3d33 2e32  raco.path (>=3.2
-0001e7f0: 2e30 2922 2c20 2270 6970 2028 3e3d 3139  .0)", "pip (>=19
-0001e800: 2e31 2922 2c20 2270 6970 2d72 756e 2028  .1)", "pip-run (
-0001e810: 3e3d 382e 3829 222c 2022 7079 7465 7374  >=8.8)", "pytest
-0001e820: 2028 3e3d 3629 222c 2022 7079 7465 7374   (>=6)", "pytest
-0001e830: 2d62 6c61 636b 2028 3e3d 302e 332e 3729  -black (>=0.3.7)
-0001e840: 222c 2022 7079 7465 7374 2d63 6865 636b  ", "pytest-check
-0001e850: 646f 6373 2028 3e3d 322e 3429 222c 2022  docs (>=2.4)", "
-0001e860: 7079 7465 7374 2d63 6f76 222c 2022 7079  pytest-cov", "py
-0001e870: 7465 7374 2d65 6e61 626c 6572 2028 3e3d  test-enabler (>=
-0001e880: 312e 3329 222c 2022 7079 7465 7374 2d6d  1.3)", "pytest-m
-0001e890: 7970 7920 283e 3d30 2e39 2e31 2922 2c20  ypy (>=0.9.1)", 
-0001e8a0: 2270 7974 6573 742d 7065 7266 222c 2022  "pytest-perf", "
-0001e8b0: 7079 7465 7374 2d72 7566 6622 2c20 2270  pytest-ruff", "p
-0001e8c0: 7974 6573 742d 7469 6d65 6f75 7422 2c20  ytest-timeout", 
-0001e8d0: 2270 7974 6573 742d 7864 6973 7422 2c20  "pytest-xdist", 
-0001e8e0: 2274 6f6d 6c69 2d77 2028 3e3d 312e 302e  "tomli-w (>=1.0.
-0001e8f0: 3029 222c 2022 7669 7274 7561 6c65 6e76  0)", "virtualenv
-0001e900: 2028 3e3d 3133 2e30 2e30 2922 2c20 2277   (>=13.0.0)", "w
-0001e910: 6865 656c 225d 0a74 6573 7469 6e67 2d69  heel"].testing-i
-0001e920: 6e74 6567 7261 7469 6f6e 203d 205b 2262  ntegration = ["b
-0001e930: 7569 6c64 5b76 6972 7475 616c 656e 765d  uild[virtualenv]
-0001e940: 222c 2022 6669 6c65 6c6f 636b 2028 3e3d  ", "filelock (>=
-0001e950: 332e 342e 3029 222c 2022 6a61 7261 636f  3.4.0)", "jaraco
-0001e960: 2e65 6e76 7320 283e 3d32 2e32 2922 2c20  .envs (>=2.2)", 
-0001e970: 226a 6172 6163 6f2e 7061 7468 2028 3e3d  "jaraco.path (>=
-0001e980: 332e 322e 3029 222c 2022 7079 7465 7374  3.2.0)", "pytest
-0001e990: 222c 2022 7079 7465 7374 2d65 6e61 626c  ", "pytest-enabl
-0001e9a0: 6572 222c 2022 7079 7465 7374 2d78 6469  er", "pytest-xdi
-0001e9b0: 7374 222c 2022 746f 6d6c 6922 2c20 2276  st", "tomli", "v
-0001e9c0: 6972 7475 616c 656e 7620 283e 3d31 332e  irtualenv (>=13.
-0001e9d0: 302e 3029 222c 2022 7768 6565 6c22 5d0a  0.0)", "wheel"].
-0001e9e0: 0a5b 5b70 6163 6b61 6765 5d5d 0a6e 616d  .[[package]].nam
-0001e9f0: 6520 3d20 2273 6822 0a76 6572 7369 6f6e  e = "sh".version
-0001ea00: 203d 2022 322e 302e 3422 0a64 6573 6372   = "2.0.4".descr
-0001ea10: 6970 7469 6f6e 203d 2022 5079 7468 6f6e  iption = "Python
-0001ea20: 2073 7562 7072 6f63 6573 7320 7265 706c   subprocess repl
-0001ea30: 6163 656d 656e 7422 0a6f 7074 696f 6e61  acement".optiona
-0001ea40: 6c20 3d20 6661 6c73 650a 7079 7468 6f6e  l = false.python
-0001ea50: 2d76 6572 7369 6f6e 7320 3d20 223e 3d33  -versions = ">=3
-0001ea60: 2e38 2e31 2c3c 342e 3022 0a66 696c 6573  .8.1,<4.0".files
-0001ea70: 203d 205b 0a20 2020 207b 6669 6c65 203d   = [.    {file =
-0001ea80: 2022 7368 2d32 2e30 2e34 2d70 7933 2d6e   "sh-2.0.4-py3-n
-0001ea90: 6f6e 652d 616e 792e 7768 6c22 2c20 6861  one-any.whl", ha
-0001eaa0: 7368 203d 2022 7368 6132 3536 3a31 3432  sh = "sha256:142
-0001eab0: 3635 6134 6364 3136 3232 3432 3965 6463  65a4cd1622429edc
-0001eac0: 6633 3030 3239 3265 6339 3831 3933 3533  f300292ec9819353
-0001ead0: 3066 6231 3433 6665 3634 3262 3334 3337  0fb143fe642b3437
-0001eae0: 3032 3465 6361 3962 6565 3863 3522 7d2c  024eca9bee8c5"},
-0001eaf0: 0a20 2020 207b 6669 6c65 203d 2022 7368  .    {file = "sh
-0001eb00: 2d32 2e30 2e34 2e74 6172 2e67 7a22 2c20  -2.0.4.tar.gz", 
-0001eb10: 6861 7368 203d 2022 7368 6132 3536 3a61  hash = "sha256:a
-0001eb20: 3138 3932 3066 3038 3339 3939 3162 6339  18920f0839991bc9
-0001eb30: 6466 6464 6236 6463 6330 3036 6333 3630  dfddb6dcc006c360
-0001eb40: 6231 3036 3462 6139 3632 3537 3335 3966  b1064ba96257359f
-0001eb50: 3065 6133 3536 6539 6661 3735 6136 3022  0ea356e9fa75a60"
-0001eb60: 7d2c 0a5d 0a0a 5b5b 7061 636b 6167 655d  },.]..[[package]
-0001eb70: 5d0a 6e61 6d65 203d 2022 7369 7822 0a76  ].name = "six".v
-0001eb80: 6572 7369 6f6e 203d 2022 312e 3136 2e30  ersion = "1.16.0
-0001eb90: 220a 6465 7363 7269 7074 696f 6e20 3d20  ".description = 
-0001eba0: 2250 7974 686f 6e20 3220 616e 6420 3320  "Python 2 and 3 
-0001ebb0: 636f 6d70 6174 6962 696c 6974 7920 7574  compatibility ut
-0001ebc0: 696c 6974 6965 7322 0a6f 7074 696f 6e61  ilities".optiona
-0001ebd0: 6c20 3d20 6661 6c73 650a 7079 7468 6f6e  l = false.python
-0001ebe0: 2d76 6572 7369 6f6e 7320 3d20 223e 3d32  -versions = ">=2
-0001ebf0: 2e37 2c20 213d 332e 302e 2a2c 2021 3d33  .7, !=3.0.*, !=3
-0001ec00: 2e31 2e2a 2c20 213d 332e 322e 2a22 0a66  .1.*, !=3.2.*".f
-0001ec10: 696c 6573 203d 205b 0a20 2020 207b 6669  iles = [.    {fi
-0001ec20: 6c65 203d 2022 7369 782d 312e 3136 2e30  le = "six-1.16.0
-0001ec30: 2d70 7932 2e70 7933 2d6e 6f6e 652d 616e  -py2.py3-none-an
-0001ec40: 792e 7768 6c22 2c20 6861 7368 203d 2022  y.whl", hash = "
-0001ec50: 7368 6132 3536 3a38 6162 6232 6631 6438  sha256:8abb2f1d8
-0001ec60: 3638 3930 6132 6466 6239 3839 6639 6137  6890a2dfb989f9a7
-0001ec70: 3763 6663 6664 3365 3437 6332 6133 3534  7cfcfd3e47c2a354
-0001ec80: 6230 3131 3131 3737 3133 3236 6638 6161  b01111771326f8aa
-0001ec90: 3236 6530 3235 3422 7d2c 0a20 2020 207b  26e0254"},.    {
-0001eca0: 6669 6c65 203d 2022 7369 782d 312e 3136  file = "six-1.16
-0001ecb0: 2e30 2e74 6172 2e67 7a22 2c20 6861 7368  .0.tar.gz", hash
-0001ecc0: 203d 2022 7368 6132 3536 3a31 6536 3163   = "sha256:1e61c
-0001ecd0: 3337 3437 3761 3136 3236 3435 3865 3336  37477a1626458e36
-0001ece0: 6637 6231 6438 3261 6135 6339 6230 3934  f7b1d82aa5c9b094
-0001ecf0: 6661 3438 3032 3839 3230 3732 6534 3964  fa4802892072e49d
-0001ed00: 6539 6336 3063 3463 3932 3622 7d2c 0a5d  e9c60c4c926"},.]
-0001ed10: 0a0a 5b5b 7061 636b 6167 655d 5d0a 6e61  ..[[package]].na
-0001ed20: 6d65 203d 2022 736f 7570 7369 6576 6522  me = "soupsieve"
-0001ed30: 0a76 6572 7369 6f6e 203d 2022 322e 342e  .version = "2.4.
-0001ed40: 3122 0a64 6573 6372 6970 7469 6f6e 203d  1".description =
-0001ed50: 2022 4120 6d6f 6465 726e 2043 5353 2073   "A modern CSS s
-0001ed60: 656c 6563 746f 7220 696d 706c 656d 656e  elector implemen
-0001ed70: 7461 7469 6f6e 2066 6f72 2042 6561 7574  tation for Beaut
-0001ed80: 6966 756c 2053 6f75 702e 220a 6f70 7469  iful Soup.".opti
-0001ed90: 6f6e 616c 203d 2066 616c 7365 0a70 7974  onal = false.pyt
-0001eda0: 686f 6e2d 7665 7273 696f 6e73 203d 2022  hon-versions = "
-0001edb0: 3e3d 332e 3722 0a66 696c 6573 203d 205b  >=3.7".files = [
-0001edc0: 0a20 2020 207b 6669 6c65 203d 2022 736f  .    {file = "so
-0001edd0: 7570 7369 6576 652d 322e 342e 312d 7079  upsieve-2.4.1-py
-0001ede0: 332d 6e6f 6e65 2d61 6e79 2e77 686c 222c  3-none-any.whl",
-0001edf0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001ee00: 3163 3162 6665 6536 3831 3935 3434 6133  1c1bfee6819544a3
-0001ee10: 3434 3735 3836 6338 3839 3135 3733 3635  447586c889157365
-0001ee20: 6132 3765 3130 6438 3863 6465 3361 6433  a27e10d88cde3ad3
-0001ee30: 6461 3063 6630 6464 6636 3436 6665 6238  da0cf0ddf646feb8
-0001ee40: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001ee50: 2273 6f75 7073 6965 7665 2d32 2e34 2e31  "soupsieve-2.4.1
-0001ee60: 2e74 6172 2e67 7a22 2c20 6861 7368 203d  .tar.gz", hash =
-0001ee70: 2022 7368 6132 3536 3a38 3964 3132 6232   "sha256:89d12b2
-0001ee80: 6435 6466 6364 3263 3965 3863 3232 3332  d5dfcd2c9e8c2232
-0001ee90: 3664 6139 6439 6161 3963 6233 6466 6162  6da9d9aa9cb3dfab
-0001eea0: 3061 3833 6130 3234 6630 3537 3034 3037  0a83a024f0570407
-0001eeb0: 3665 6538 6433 3565 6122 7d2c 0a5d 0a0a  6ee8d35ea"},.]..
-0001eec0: 5b5b 7061 636b 6167 655d 5d0a 6e61 6d65  [[package]].name
-0001eed0: 203d 2022 7465 726d 636f 6c6f 7222 0a76   = "termcolor".v
-0001eee0: 6572 7369 6f6e 203d 2022 322e 332e 3022  ersion = "2.3.0"
-0001eef0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
-0001ef00: 414e 5349 2063 6f6c 6f72 2066 6f72 6d61  ANSI color forma
-0001ef10: 7474 696e 6720 666f 7220 6f75 7470 7574  tting for output
-0001ef20: 2069 6e20 7465 726d 696e 616c 220a 6f70   in terminal".op
-0001ef30: 7469 6f6e 616c 203d 2066 616c 7365 0a70  tional = false.p
-0001ef40: 7974 686f 6e2d 7665 7273 696f 6e73 203d  ython-versions =
-0001ef50: 2022 3e3d 332e 3722 0a66 696c 6573 203d   ">=3.7".files =
-0001ef60: 205b 0a20 2020 207b 6669 6c65 203d 2022   [.    {file = "
-0001ef70: 7465 726d 636f 6c6f 722d 322e 332e 302d  termcolor-2.3.0-
-0001ef80: 7079 332d 6e6f 6e65 2d61 6e79 2e77 686c  py3-none-any.whl
-0001ef90: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001efa0: 363a 3361 6662 3035 3630 3762 3839 6165  6:3afb05607b89ae
-0001efb0: 6430 6666 6532 3532 3032 3339 3965 6530  d0ffe25202399ee0
-0001efc0: 3836 3761 6434 6433 6362 3431 3830 6439  867ad4d3cb4180d9
-0001efd0: 3861 6166 3865 6566 6136 6135 6637 6434  8aaf8eefa6a5f7d4
-0001efe0: 3735 227d 2c0a 2020 2020 7b66 696c 6520  75"},.    {file 
-0001eff0: 3d20 2274 6572 6d63 6f6c 6f72 2d32 2e33  = "termcolor-2.3
-0001f000: 2e30 2e74 6172 2e67 7a22 2c20 6861 7368  .0.tar.gz", hash
-0001f010: 203d 2022 7368 6132 3536 3a62 3562 3038   = "sha256:b5b08
-0001f020: 6636 3839 3337 6631 3338 6665 3932 6636  f68937f138fe92f6
-0001f030: 6330 3839 6239 3966 3165 3264 6130 6165  c089b99f1e2da0ae
-0001f040: 3536 6335 3262 3738 6266 3730 3735 6664  56c52b78bf7075fd
-0001f050: 3935 3432 3066 6439 6135 6122 7d2c 0a5d  95420fd9a5a"},.]
-0001f060: 0a0a 5b70 6163 6b61 6765 2e65 7874 7261  ..[package.extra
-0001f070: 735d 0a74 6573 7473 203d 205b 2270 7974  s].tests = ["pyt
-0001f080: 6573 7422 2c20 2270 7974 6573 742d 636f  est", "pytest-co
-0001f090: 7622 5d0a 0a5b 5b70 6163 6b61 6765 5d5d  v"]..[[package]]
-0001f0a0: 0a6e 616d 6520 3d20 2274 696e 7963 7373  .name = "tinycss
-0001f0b0: 3222 0a76 6572 7369 6f6e 203d 2022 312e  2".version = "1.
-0001f0c0: 322e 3122 0a64 6573 6372 6970 7469 6f6e  2.1".description
-0001f0d0: 203d 2022 4120 7469 6e79 2043 5353 2070   = "A tiny CSS p
-0001f0e0: 6172 7365 7222 0a6f 7074 696f 6e61 6c20  arser".optional 
-0001f0f0: 3d20 6661 6c73 650a 7079 7468 6f6e 2d76  = false.python-v
-0001f100: 6572 7369 6f6e 7320 3d20 223e 3d33 2e37  ersions = ">=3.7
-0001f110: 220a 6669 6c65 7320 3d20 5b0a 2020 2020  ".files = [.    
-0001f120: 7b66 696c 6520 3d20 2274 696e 7963 7373  {file = "tinycss
-0001f130: 322d 312e 322e 312d 7079 332d 6e6f 6e65  2-1.2.1-py3-none
-0001f140: 2d61 6e79 2e77 686c 222c 2068 6173 6820  -any.whl", hash 
-0001f150: 3d20 2273 6861 3235 363a 3262 3830 6139  = "sha256:2b80a9
-0001f160: 3664 3431 6537 6333 3931 3462 3863 6461  6d41e7c3914b8cda
-0001f170: 3862 6337 6637 3035 6134 6439 6334 3932  8bc7f705a4d9c492
-0001f180: 3735 3631 3665 3838 3631 3033 6464 3833  75616e886103dd83
-0001f190: 3964 6663 3834 3738 3437 227d 2c0a 2020  9dfc847847"},.  
-0001f1a0: 2020 7b66 696c 6520 3d20 2274 696e 7963    {file = "tinyc
-0001f1b0: 7373 322d 312e 322e 312e 7461 722e 677a  ss2-1.2.1.tar.gz
-0001f1c0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-0001f1d0: 363a 3863 6666 3361 3866 3036 3663 3265  6:8cff3a8f066c2e
-0001f1e0: 6336 3737 6330 3664 6263 3762 3435 3631  c677c06dbc7b4561
-0001f1f0: 3938 3034 6136 3933 3834 3738 6439 6437  9804a6938478d9d7
-0001f200: 3363 3238 3462 3239 6431 3465 6362 3036  3c284b29d14ecb06
-0001f210: 3237 227d 2c0a 5d0a 0a5b 7061 636b 6167  27"},.]..[packag
-0001f220: 652e 6465 7065 6e64 656e 6369 6573 5d0a  e.dependencies].
-0001f230: 7765 6265 6e63 6f64 696e 6773 203d 2022  webencodings = "
-0001f240: 3e3d 302e 3422 0a0a 5b70 6163 6b61 6765  >=0.4"..[package
-0001f250: 2e65 7874 7261 735d 0a64 6f63 203d 205b  .extras].doc = [
-0001f260: 2273 7068 696e 7822 2c20 2273 7068 696e  "sphinx", "sphin
-0001f270: 785f 7274 645f 7468 656d 6522 5d0a 7465  x_rtd_theme"].te
-0001f280: 7374 203d 205b 2266 6c61 6b65 3822 2c20  st = ["flake8", 
-0001f290: 2269 736f 7274 222c 2022 7079 7465 7374  "isort", "pytest
-0001f2a0: 225d 0a0a 5b5b 7061 636b 6167 655d 5d0a  "]..[[package]].
-0001f2b0: 6e61 6d65 203d 2022 746f 6d6c 220a 7665  name = "toml".ve
-0001f2c0: 7273 696f 6e20 3d20 2230 2e31 302e 3222  rsion = "0.10.2"
-0001f2d0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
-0001f2e0: 5079 7468 6f6e 204c 6962 7261 7279 2066  Python Library f
-0001f2f0: 6f72 2054 6f6d 2773 204f 6276 696f 7573  or Tom's Obvious
-0001f300: 2c20 4d69 6e69 6d61 6c20 4c61 6e67 7561  , Minimal Langua
-0001f310: 6765 220a 6f70 7469 6f6e 616c 203d 2066  ge".optional = f
-0001f320: 616c 7365 0a70 7974 686f 6e2d 7665 7273  alse.python-vers
-0001f330: 696f 6e73 203d 2022 3e3d 322e 362c 2021  ions = ">=2.6, !
-0001f340: 3d33 2e30 2e2a 2c20 213d 332e 312e 2a2c  =3.0.*, !=3.1.*,
-0001f350: 2021 3d33 2e32 2e2a 220a 6669 6c65 7320   !=3.2.*".files 
-0001f360: 3d20 5b0a 2020 2020 7b66 696c 6520 3d20  = [.    {file = 
-0001f370: 2274 6f6d 6c2d 302e 3130 2e32 2d70 7932  "toml-0.10.2-py2
-0001f380: 2e70 7933 2d6e 6f6e 652d 616e 792e 7768  .py3-none-any.wh
-0001f390: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-0001f3a0: 3536 3a38 3036 3134 3361 6535 6266 6236  56:806143ae5bfb6
-0001f3b0: 6133 6336 6537 3336 6137 3634 3035 3764  a3c6e736a764057d
-0001f3c0: 6230 6536 6130 6530 3565 3333 3862 3536  b0e6a0e05e338b56
-0001f3d0: 3330 3839 3461 3566 3737 3963 6162 6234  30894a5f779cabb4
-0001f3e0: 6639 6222 7d2c 0a20 2020 207b 6669 6c65  f9b"},.    {file
-0001f3f0: 203d 2022 746f 6d6c 2d30 2e31 302e 322e   = "toml-0.10.2.
-0001f400: 7461 722e 677a 222c 2068 6173 6820 3d20  tar.gz", hash = 
-0001f410: 2273 6861 3235 363a 6233 6264 6131 6431  "sha256:b3bda1d1
-0001f420: 3038 6435 6464 3939 6634 6132 3064 3234  08d5dd99f4a20d24
-0001f430: 6439 6333 3438 6539 3163 3464 6237 6162  d9c348e91c4db7ab
-0001f440: 3162 3734 3932 3030 6264 6564 3266 3833  1b749200bded2f83
-0001f450: 3963 6362 6536 3866 227d 2c0a 5d0a 0a5b  9ccbe68f"},.]..[
-0001f460: 5b70 6163 6b61 6765 5d5d 0a6e 616d 6520  [package]].name 
-0001f470: 3d20 2274 6f6d 6c69 220a 7665 7273 696f  = "tomli".versio
-0001f480: 6e20 3d20 2232 2e30 2e31 220a 6465 7363  n = "2.0.1".desc
-0001f490: 7269 7074 696f 6e20 3d20 2241 206c 696c  ription = "A lil
-0001f4a0: 2720 544f 4d4c 2070 6172 7365 7222 0a6f  ' TOML parser".o
-0001f4b0: 7074 696f 6e61 6c20 3d20 6661 6c73 650a  ptional = false.
-0001f4c0: 7079 7468 6f6e 2d76 6572 7369 6f6e 7320  python-versions 
-0001f4d0: 3d20 223e 3d33 2e37 220a 6669 6c65 7320  = ">=3.7".files 
-0001f4e0: 3d20 5b0a 2020 2020 7b66 696c 6520 3d20  = [.    {file = 
-0001f4f0: 2274 6f6d 6c69 2d32 2e30 2e31 2d70 7933  "tomli-2.0.1-py3
-0001f500: 2d6e 6f6e 652d 616e 792e 7768 6c22 2c20  -none-any.whl", 
-0001f510: 6861 7368 203d 2022 7368 6132 3536 3a39  hash = "sha256:9
-0001f520: 3339 6465 3365 3761 3631 3631 6166 3063  39de3e7a6161af0c
-0001f530: 3838 3765 6639 3162 3764 3431 6135 3365  887ef91b7d41a53e
-0001f540: 3763 3561 3163 6139 3736 3332 3566 3432  7c5a1ca976325f42
-0001f550: 3963 6234 3665 6139 6263 3330 6563 6322  9cb46ea9bc30ecc"
-0001f560: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-0001f570: 746f 6d6c 692d 322e 302e 312e 7461 722e  tomli-2.0.1.tar.
-0001f580: 677a 222c 2068 6173 6820 3d20 2273 6861  gz", hash = "sha
-0001f590: 3235 363a 6465 3532 3663 3132 3931 3466  256:de526c12914f
-0001f5a0: 3063 3535 3064 3135 3932 3463 3632 6437  0c550d15924c62d7
-0001f5b0: 3261 6263 3438 6436 6665 3733 3634 6161  2abc48d6fe7364aa
-0001f5c0: 3837 3332 3833 3337 6133 3130 3037 6665  87328337a31007fe
-0001f5d0: 3861 3466 227d 2c0a 5d0a 0a5b 5b70 6163  8a4f"},.]..[[pac
-0001f5e0: 6b61 6765 5d5d 0a6e 616d 6520 3d20 2274  kage]].name = "t
-0001f5f0: 6f72 6e61 646f 220a 7665 7273 696f 6e20  ornado".version 
-0001f600: 3d20 2236 2e33 2e32 220a 6465 7363 7269  = "6.3.2".descri
-0001f610: 7074 696f 6e20 3d20 2254 6f72 6e61 646f  ption = "Tornado
-0001f620: 2069 7320 6120 5079 7468 6f6e 2077 6562   is a Python web
-0001f630: 2066 7261 6d65 776f 726b 2061 6e64 2061   framework and a
-0001f640: 7379 6e63 6872 6f6e 6f75 7320 6e65 7477  synchronous netw
-0001f650: 6f72 6b69 6e67 206c 6962 7261 7279 2c20  orking library, 
-0001f660: 6f72 6967 696e 616c 6c79 2064 6576 656c  originally devel
-0001f670: 6f70 6564 2061 7420 4672 6965 6e64 4665  oped at FriendFe
-0001f680: 6564 2e22 0a6f 7074 696f 6e61 6c20 3d20  ed.".optional = 
-0001f690: 6661 6c73 650a 7079 7468 6f6e 2d76 6572  false.python-ver
-0001f6a0: 7369 6f6e 7320 3d20 223e 3d20 332e 3822  sions = ">= 3.8"
-0001f6b0: 0a66 696c 6573 203d 205b 0a20 2020 207b  .files = [.    {
-0001f6c0: 6669 6c65 203d 2022 746f 726e 6164 6f2d  file = "tornado-
-0001f6d0: 362e 332e 322d 6370 3338 2d61 6269 332d  6.3.2-cp38-abi3-
-0001f6e0: 6d61 636f 7378 5f31 305f 395f 756e 6976  macosx_10_9_univ
-0001f6f0: 6572 7361 6c32 2e77 686c 222c 2068 6173  ersal2.whl", has
-0001f700: 6820 3d20 2273 6861 3235 363a 6333 3637  h = "sha256:c367
-0001f710: 6162 3663 3033 3933 6437 3131 3731 3132  ab6c0393d7117112
-0001f720: 3363 6135 3531 3563 3631 6666 3632 6665  3ca5515c61ff62fe
-0001f730: 3039 3032 3466 6136 6266 3239 3963 6431  09024fa6bf299cd1
-0001f740: 3333 3964 6339 3435 3638 3239 227d 2c0a  339dc9456829"},.
-0001f750: 2020 2020 7b66 696c 6520 3d20 2274 6f72      {file = "tor
-0001f760: 6e61 646f 2d36 2e33 2e32 2d63 7033 382d  nado-6.3.2-cp38-
-0001f770: 6162 6933 2d6d 6163 6f73 785f 3130 5f39  abi3-macosx_10_9
-0001f780: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
-0001f790: 7368 203d 2022 7368 6132 3536 3a62 3436  sh = "sha256:b46
-0001f7a0: 6136 6162 3230 6635 6337 6331 6362 3934  a6ab20f5c7c1cb94
-0001f7b0: 3963 3732 6331 3939 3461 3435 3835 6432  9c72c1994a4585d2
-0001f7c0: 6561 6130 6265 3438 3533 6635 3061 3033  eaa0be4853f50a03
-0001f7d0: 6235 3033 3165 3936 3466 6337 6322 7d2c  b5031e964fc7c"},
-0001f7e0: 0a20 2020 207b 6669 6c65 203d 2022 746f  .    {file = "to
-0001f7f0: 726e 6164 6f2d 362e 332e 322d 6370 3338  rnado-6.3.2-cp38
-0001f800: 2d61 6269 332d 6d61 6e79 6c69 6e75 785f  -abi3-manylinux_
-0001f810: 325f 3137 5f61 6172 6368 3634 2e6d 616e  2_17_aarch64.man
-0001f820: 796c 696e 7578 3230 3134 5f61 6172 6368  ylinux2014_aarch
-0001f830: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001f840: 2273 6861 3235 363a 6332 6465 3134 3036  "sha256:c2de1406
-0001f850: 3663 3461 3338 6234 6563 6262 6364 3535  6c4a38b4ecbbcd55
-0001f860: 6335 6363 3462 3533 3430 6562 3034 6631  c5cc4b5340eb04f1
-0001f870: 6335 6538 3164 6137 3435 3165 6635 3535  c5e81da7451ef555
-0001f880: 3835 3963 3833 3366 227d 2c0a 2020 2020  859c833f"},.    
-0001f890: 7b66 696c 6520 3d20 2274 6f72 6e61 646f  {file = "tornado
-0001f8a0: 2d36 2e33 2e32 2d63 7033 382d 6162 6933  -6.3.2-cp38-abi3
-0001f8b0: 2d6d 616e 796c 696e 7578 5f32 5f35 5f69  -manylinux_2_5_i
-0001f8c0: 3638 362e 6d61 6e79 6c69 6e75 7831 5f69  686.manylinux1_i
-0001f8d0: 3638 362e 6d61 6e79 6c69 6e75 785f 325f  686.manylinux_2_
-0001f8e0: 3137 5f69 3638 362e 6d61 6e79 6c69 6e75  17_i686.manylinu
-0001f8f0: 7832 3031 345f 6936 3836 2e77 686c 222c  x2014_i686.whl",
-0001f900: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001f910: 3035 3631 3530 3936 3834 3563 6635 3061  05615096845cf50a
-0001f920: 3839 3530 3236 6637 3439 3139 3562 6630  895026f749195bf0
-0001f930: 6231 3062 3839 3039 6639 6265 3637 3266  b10b8909f9be672f
-0001f940: 3530 6230 6665 3639 6362 6133 3638 6534  50b0fe69cba368e4
-0001f950: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001f960: 2274 6f72 6e61 646f 2d36 2e33 2e32 2d63  "tornado-6.3.2-c
-0001f970: 7033 382d 6162 6933 2d6d 616e 796c 696e  p38-abi3-manylin
-0001f980: 7578 5f32 5f35 5f78 3836 5f36 342e 6d61  ux_2_5_x86_64.ma
-0001f990: 6e79 6c69 6e75 7831 5f78 3836 5f36 342e  nylinux1_x86_64.
-0001f9a0: 6d61 6e79 6c69 6e75 785f 325f 3137 5f78  manylinux_2_17_x
-0001f9b0: 3836 5f36 342e 6d61 6e79 6c69 6e75 7832  86_64.manylinux2
-0001f9c0: 3031 345f 7838 365f 3634 2e77 686c 222c  014_x86_64.whl",
-0001f9d0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-0001f9e0: 3562 3137 6231 6366 3566 3833 3534 6566  5b17b1cf5f8354ef
-0001f9f0: 6133 6433 3763 3665 3238 6664 6664 3963  a3d37c6e28fdfd9c
-0001fa00: 3163 3165 3531 3232 6632 6362 3536 6461  1c1e5122f2cb56da
-0001fa10: 6331 3231 6163 3631 6261 6134 3763 6265  c121ac61baa47cbe
-0001fa20: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-0001fa30: 2274 6f72 6e61 646f 2d36 2e33 2e32 2d63  "tornado-6.3.2-c
-0001fa40: 7033 382d 6162 6933 2d6d 7573 6c6c 696e  p38-abi3-musllin
-0001fa50: 7578 5f31 5f31 5f61 6172 6368 3634 2e77  ux_1_1_aarch64.w
-0001fa60: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001fa70: 3235 363a 3239 6537 3163 3834 3761 3335  256:29e71c847a35
-0001fa80: 6636 6531 3063 6133 6235 6332 3939 3061  f6e10ca3b5c2990a
-0001fa90: 3532 6365 3338 6232 3333 3031 3964 3865  52ce38b233019d8e
-0001faa0: 3835 3862 3735 3565 6136 6365 3464 6364  858b755ea6ce4dcd
-0001fab0: 6431 3964 227d 2c0a 2020 2020 7b66 696c  d19d"},.    {fil
-0001fac0: 6520 3d20 2274 6f72 6e61 646f 2d36 2e33  e = "tornado-6.3
-0001fad0: 2e32 2d63 7033 382d 6162 6933 2d6d 7573  .2-cp38-abi3-mus
-0001fae0: 6c6c 696e 7578 5f31 5f31 5f69 3638 362e  llinux_1_1_i686.
-0001faf0: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-0001fb00: 6132 3536 3a38 3334 6165 3735 3430 6164  a256:834ae7540ad
-0001fb10: 3361 3833 3139 3961 3864 6138 6639 6632  3a83199a8da8f9f2
-0001fb20: 6433 3833 6533 6333 6435 3133 3061 3332  d383e3c3d5130a32
-0001fb30: 3838 3839 6534 6363 3939 3161 6363 3831  8889e4cc991acc81
-0001fb40: 6538 3761 3022 7d2c 0a20 2020 207b 6669  e87a0"},.    {fi
-0001fb50: 6c65 203d 2022 746f 726e 6164 6f2d 362e  le = "tornado-6.
-0001fb60: 332e 322d 6370 3338 2d61 6269 332d 6d75  3.2-cp38-abi3-mu
-0001fb70: 736c 6c69 6e75 785f 315f 315f 7838 365f  sllinux_1_1_x86_
-0001fb80: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-0001fb90: 2273 6861 3235 363a 3661 3038 3438 6631  "sha256:6a0848f1
-0001fba0: 6165 6130 6431 3936 6137 6334 6636 3737  aea0d196a7c4f677
-0001fbb0: 3231 3937 6362 6532 6162 6334 3236 3666  2197cbe2abc4266f
-0001fbc0: 3833 3662 3061 6163 3736 3934 3738 3732  836b0aac76947872
-0001fbd0: 6364 3239 6234 3131 227d 2c0a 2020 2020  cd29b411"},.    
-0001fbe0: 7b66 696c 6520 3d20 2274 6f72 6e61 646f  {file = "tornado
-0001fbf0: 2d36 2e33 2e32 2d63 7033 382d 6162 6933  -6.3.2-cp38-abi3
-0001fc00: 2d77 696e 3332 2e77 686c 222c 2068 6173  -win32.whl", has
-0001fc10: 6820 3d20 2273 6861 3235 363a 3765 6663  h = "sha256:7efc
-0001fc20: 6263 6333 3062 3763 3635 3465 6236 6138  bcc30b7c654eb6a8
-0001fc30: 6339 6339 6461 3738 3761 3835 3163 3138  c9c9da787a851c18
-0001fc40: 6638 6363 6434 6135 6133 6139 3562 3035  f8ccd4a5a3a95b05
-0001fc50: 6337 6163 6366 6130 3638 6432 227d 2c0a  c7accfa068d2"},.
-0001fc60: 2020 2020 7b66 696c 6520 3d20 2274 6f72      {file = "tor
-0001fc70: 6e61 646f 2d36 2e33 2e32 2d63 7033 382d  nado-6.3.2-cp38-
-0001fc80: 6162 6933 2d77 696e 5f61 6d64 3634 2e77  abi3-win_amd64.w
-0001fc90: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-0001fca0: 3235 363a 3063 3332 3565 3636 6338 3132  256:0c325e66c812
-0001fcb0: 3363 3630 3665 6561 3333 3038 3439 3736  3c606eea33084976
-0001fcc0: 6338 3332 6161 3465 3736 3662 3764 6666  c832aa4e766b7dff
-0001fcd0: 3861 6564 6437 3538 3765 6134 3461 3630  8aedd7587ea44a60
-0001fce0: 3463 6466 227d 2c0a 2020 2020 7b66 696c  4cdf"},.    {fil
-0001fcf0: 6520 3d20 2274 6f72 6e61 646f 2d36 2e33  e = "tornado-6.3
-0001fd00: 2e32 2e74 6172 2e67 7a22 2c20 6861 7368  .2.tar.gz", hash
-0001fd10: 203d 2022 7368 6132 3536 3a34 6239 3237   = "sha256:4b927
-0001fd20: 6334 6631 3962 3731 6536 3237 6231 3366  c4f19b71e627b13f
-0001fd30: 3364 6232 3332 3465 3461 6536 3630 3532  3db2324e4ae66052
-0001fd40: 3731 3433 6639 6531 6632 6532 6662 3430  7143f9e1f2e2fb40
-0001fd50: 3466 3361 3138 3765 3262 6122 7d2c 0a5d  4f3a187e2ba"},.]
-0001fd60: 0a0a 5b5b 7061 636b 6167 655d 5d0a 6e61  ..[[package]].na
-0001fd70: 6d65 203d 2022 7472 6169 746c 6574 7322  me = "traitlets"
-0001fd80: 0a76 6572 7369 6f6e 203d 2022 352e 392e  .version = "5.9.
-0001fd90: 3022 0a64 6573 6372 6970 7469 6f6e 203d  0".description =
-0001fda0: 2022 5472 6169 746c 6574 7320 5079 7468   "Traitlets Pyth
-0001fdb0: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
-0001fdc0: 2073 7973 7465 6d22 0a6f 7074 696f 6e61   system".optiona
-0001fdd0: 6c20 3d20 6661 6c73 650a 7079 7468 6f6e  l = false.python
-0001fde0: 2d76 6572 7369 6f6e 7320 3d20 223e 3d33  -versions = ">=3
-0001fdf0: 2e37 220a 6669 6c65 7320 3d20 5b0a 2020  .7".files = [.  
-0001fe00: 2020 7b66 696c 6520 3d20 2274 7261 6974    {file = "trait
-0001fe10: 6c65 7473 2d35 2e39 2e30 2d70 7933 2d6e  lets-5.9.0-py3-n
-0001fe20: 6f6e 652d 616e 792e 7768 6c22 2c20 6861  one-any.whl", ha
-0001fe30: 7368 203d 2022 7368 6132 3536 3a39 6536  sh = "sha256:9e6
-0001fe40: 6563 3038 3032 3539 6239 6135 3934 3063  ec080259b9a5940c
-0001fe50: 3739 3764 3538 6236 3133 6235 6533 3134  797d58b613b5e314
-0001fe60: 3431 6332 3235 3762 3837 6332 6537 3935  41c2257b87c2e795
-0001fe70: 6335 3232 3861 6538 3064 3264 3822 7d2c  c5228ae80d2d8"},
-0001fe80: 0a20 2020 207b 6669 6c65 203d 2022 7472  .    {file = "tr
-0001fe90: 6169 746c 6574 732d 352e 392e 302e 7461  aitlets-5.9.0.ta
-0001fea0: 722e 677a 222c 2068 6173 6820 3d20 2273  r.gz", hash = "s
-0001feb0: 6861 3235 363a 6636 6364 6532 3161 3963  ha256:f6cde21a9c
-0001fec0: 3638 6366 3735 3661 6630 3230 3335 6637  68cf756af02035f7
-0001fed0: 3264 3561 3732 3362 6636 3037 6538 3632  2d5a723bf607e862
-0001fee0: 6537 6265 3333 6563 6535 3035 6162 6634  e7be33ece505abf4
-0001fef0: 6133 6261 6439 227d 2c0a 5d0a 0a5b 7061  a3bad9"},.]..[pa
-0001ff00: 636b 6167 652e 6578 7472 6173 5d0a 646f  ckage.extras].do
-0001ff10: 6373 203d 205b 226d 7973 742d 7061 7273  cs = ["myst-pars
-0001ff20: 6572 222c 2022 7079 6461 7461 2d73 7068  er", "pydata-sph
-0001ff30: 696e 782d 7468 656d 6522 2c20 2273 7068  inx-theme", "sph
-0001ff40: 696e 7822 5d0a 7465 7374 203d 205b 2261  inx"].test = ["a
-0001ff50: 7267 636f 6d70 6c65 7465 2028 3e3d 322e  rgcomplete (>=2.
-0001ff60: 3029 222c 2022 7072 652d 636f 6d6d 6974  0)", "pre-commit
-0001ff70: 222c 2022 7079 7465 7374 222c 2022 7079  ", "pytest", "py
-0001ff80: 7465 7374 2d6d 6f63 6b22 5d0a 0a5b 5b70  test-mock"]..[[p
-0001ff90: 6163 6b61 6765 5d5d 0a6e 616d 6520 3d20  ackage]].name = 
-0001ffa0: 2274 7970 6573 2d70 7979 616d 6c22 0a76  "types-pyyaml".v
-0001ffb0: 6572 7369 6f6e 203d 2022 362e 302e 3132  ersion = "6.0.12
-0001ffc0: 2e31 3022 0a64 6573 6372 6970 7469 6f6e  .10".description
-0001ffd0: 203d 2022 5479 7069 6e67 2073 7475 6273   = "Typing stubs
-0001ffe0: 2066 6f72 2050 7959 414d 4c22 0a6f 7074   for PyYAML".opt
-0001fff0: 696f 6e61 6c20 3d20 6661 6c73 650a 7079  ional = false.py
-00020000: 7468 6f6e 2d76 6572 7369 6f6e 7320 3d20  thon-versions = 
-00020010: 222a 220a 6669 6c65 7320 3d20 5b0a 2020  "*".files = [.  
-00020020: 2020 7b66 696c 6520 3d20 2274 7970 6573    {file = "types
-00020030: 2d50 7959 414d 4c2d 362e 302e 3132 2e31  -PyYAML-6.0.12.1
-00020040: 302e 7461 722e 677a 222c 2068 6173 6820  0.tar.gz", hash 
-00020050: 3d20 2273 6861 3235 363a 6562 6162 3364  = "sha256:ebab3d
-00020060: 3037 3030 6239 3436 3535 3337 3234 6165  0700b946553724ae
-00020070: 3663 6136 3336 6561 3933 3263 3162 3038  6ca636ea932c1b08
-00020080: 3638 3730 3164 3461 6631 3231 3633 3065  68701d4af121630e
-00020090: 3738 6436 3935 6663 3937 227d 2c0a 2020  78d695fc97"},.  
-000200a0: 2020 7b66 696c 6520 3d20 2274 7970 6573    {file = "types
-000200b0: 5f50 7959 414d 4c2d 362e 302e 3132 2e31  _PyYAML-6.0.12.1
-000200c0: 302d 7079 332d 6e6f 6e65 2d61 6e79 2e77  0-py3-none-any.w
-000200d0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-000200e0: 3235 363a 3636 3266 6134 3434 3936 3365  256:662fa444963e
-000200f0: 6666 3962 3638 3132 3064 3730 6364 6131  ff9b68120d70cda1
-00020100: 6166 3561 3566 3261 6135 3739 3030 3030  af5a5f2aa5790000
-00020110: 3363 3230 3036 6437 3632 3634 3530 6561  3c2006d7626450ea
-00020120: 6165 3566 227d 2c0a 5d0a 0a5b 5b70 6163  ae5f"},.]..[[pac
-00020130: 6b61 6765 5d5d 0a6e 616d 6520 3d20 2274  kage]].name = "t
-00020140: 7970 696e 672d 6578 7465 6e73 696f 6e73  yping-extensions
-00020150: 220a 7665 7273 696f 6e20 3d20 2234 2e36  ".version = "4.6
-00020160: 2e32 220a 6465 7363 7269 7074 696f 6e20  .2".description 
-00020170: 3d20 2242 6163 6b70 6f72 7465 6420 616e  = "Backported an
-00020180: 6420 4578 7065 7269 6d65 6e74 616c 2054  d Experimental T
-00020190: 7970 6520 4869 6e74 7320 666f 7220 5079  ype Hints for Py
-000201a0: 7468 6f6e 2033 2e37 2b22 0a6f 7074 696f  thon 3.7+".optio
-000201b0: 6e61 6c20 3d20 6661 6c73 650a 7079 7468  nal = false.pyth
-000201c0: 6f6e 2d76 6572 7369 6f6e 7320 3d20 223e  on-versions = ">
-000201d0: 3d33 2e37 220a 6669 6c65 7320 3d20 5b0a  =3.7".files = [.
-000201e0: 2020 2020 7b66 696c 6520 3d20 2274 7970      {file = "typ
-000201f0: 696e 675f 6578 7465 6e73 696f 6e73 2d34  ing_extensions-4
-00020200: 2e36 2e32 2d70 7933 2d6e 6f6e 652d 616e  .6.2-py3-none-an
-00020210: 792e 7768 6c22 2c20 6861 7368 203d 2022  y.whl", hash = "
-00020220: 7368 6132 3536 3a33 6138 6233 3666 3133  sha256:3a8b36f13
-00020230: 6464 3566 6463 3564 3162 3136 6665 3331  dd5fdc5d1b16fe31
-00020240: 3766 3536 3638 3534 3564 6537 3766 6130  7f5668545de77fa0
-00020250: 6238 6530 3230 3036 3338 3166 6434 3964  b8e02006381fd49d
-00020260: 3733 3161 6239 3822 7d2c 0a20 2020 207b  731ab98"},.    {
-00020270: 6669 6c65 203d 2022 7479 7069 6e67 5f65  file = "typing_e
-00020280: 7874 656e 7369 6f6e 732d 342e 362e 322e  xtensions-4.6.2.
-00020290: 7461 722e 677a 222c 2068 6173 6820 3d20  tar.gz", hash = 
-000202a0: 2273 6861 3235 363a 3036 3030 3632 3434  "sha256:06006244
-000202b0: 6337 3061 6338 6565 3833 6661 3832 3832  c70ac8ee83fa8282
-000202c0: 6362 3138 3866 3639 3762 3864 6232 3562  cb188f697b8db25b
-000202d0: 6338 6234 6466 3037 6265 3138 3733 6334  c8b4df07be1873c4
-000202e0: 3338 3937 3036 3063 227d 2c0a 5d0a 0a5b  3897060c"},.]..[
-000202f0: 5b70 6163 6b61 6765 5d5d 0a6e 616d 6520  [package]].name 
-00020300: 3d20 2275 726c 6c69 6233 220a 7665 7273  = "urllib3".vers
-00020310: 696f 6e20 3d20 2231 2e32 362e 3136 220a  ion = "1.26.16".
-00020320: 6465 7363 7269 7074 696f 6e20 3d20 2248  description = "H
-00020330: 5454 5020 6c69 6272 6172 7920 7769 7468  TTP library with
-00020340: 2074 6872 6561 642d 7361 6665 2063 6f6e   thread-safe con
-00020350: 6e65 6374 696f 6e20 706f 6f6c 696e 672c  nection pooling,
-00020360: 2066 696c 6520 706f 7374 2c20 616e 6420   file post, and 
-00020370: 6d6f 7265 2e22 0a6f 7074 696f 6e61 6c20  more.".optional 
-00020380: 3d20 6661 6c73 650a 7079 7468 6f6e 2d76  = false.python-v
-00020390: 6572 7369 6f6e 7320 3d20 223e 3d32 2e37  ersions = ">=2.7
-000203a0: 2c20 213d 332e 302e 2a2c 2021 3d33 2e31  , !=3.0.*, !=3.1
-000203b0: 2e2a 2c20 213d 332e 322e 2a2c 2021 3d33  .*, !=3.2.*, !=3
-000203c0: 2e33 2e2a 2c20 213d 332e 342e 2a2c 2021  .3.*, !=3.4.*, !
-000203d0: 3d33 2e35 2e2a 220a 6669 6c65 7320 3d20  =3.5.*".files = 
-000203e0: 5b0a 2020 2020 7b66 696c 6520 3d20 2275  [.    {file = "u
-000203f0: 726c 6c69 6233 2d31 2e32 362e 3136 2d70  rllib3-1.26.16-p
-00020400: 7932 2e70 7933 2d6e 6f6e 652d 616e 792e  y2.py3-none-any.
-00020410: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-00020420: 6132 3536 3a38 6433 3661 6661 3736 3136  a256:8d36afa7616
-00020430: 6438 6162 3731 3436 3038 3431 3162 3461  d8ab714608411b4a
-00020440: 3362 3133 6535 3866 3436 3361 6565 3531  3b13e58f463aee51
-00020450: 3930 3234 3537 3865 3036 3265 3134 3164  9024578e062e141d
-00020460: 6365 3230 6622 7d2c 0a20 2020 207b 6669  ce20f"},.    {fi
-00020470: 6c65 203d 2022 7572 6c6c 6962 332d 312e  le = "urllib3-1.
-00020480: 3236 2e31 362e 7461 722e 677a 222c 2068  26.16.tar.gz", h
-00020490: 6173 6820 3d20 2273 6861 3235 363a 3866  ash = "sha256:8f
-000204a0: 3133 3566 3635 3032 3735 3662 6465 3662  135f6502756bde6b
-000204b0: 3261 3962 3238 3938 3964 6635 6662 6538  2a9b28989df5fbe8
-000204c0: 3763 3939 3730 6365 6361 6136 3930 3431  7c9970cecaa69041
-000204d0: 6564 6363 6537 6630 3538 3962 3134 227d  edcce7f0589b14"}
-000204e0: 2c0a 5d0a 0a5b 7061 636b 6167 652e 6578  ,.]..[package.ex
-000204f0: 7472 6173 5d0a 6272 6f74 6c69 203d 205b  tras].brotli = [
-00020500: 2262 726f 746c 6920 283e 3d31 2e30 2e39  "brotli (>=1.0.9
-00020510: 2922 2c20 2262 726f 746c 6963 6666 6920  )", "brotlicffi 
-00020520: 283e 3d30 2e38 2e30 2922 2c20 2262 726f  (>=0.8.0)", "bro
-00020530: 746c 6970 7920 283e 3d30 2e36 2e30 2922  tlipy (>=0.6.0)"
-00020540: 5d0a 7365 6375 7265 203d 205b 2263 6572  ].secure = ["cer
-00020550: 7469 6669 222c 2022 6372 7970 746f 6772  tifi", "cryptogr
-00020560: 6170 6879 2028 3e3d 312e 332e 3429 222c  aphy (>=1.3.4)",
-00020570: 2022 6964 6e61 2028 3e3d 322e 302e 3029   "idna (>=2.0.0)
-00020580: 222c 2022 6970 6164 6472 6573 7322 2c20  ", "ipaddress", 
-00020590: 2270 794f 7065 6e53 534c 2028 3e3d 302e  "pyOpenSSL (>=0.
-000205a0: 3134 2922 2c20 2275 726c 6c69 6233 2d73  14)", "urllib3-s
-000205b0: 6563 7572 652d 6578 7472 6122 5d0a 736f  ecure-extra"].so
-000205c0: 636b 7320 3d20 5b22 5079 536f 636b 7320  cks = ["PySocks 
-000205d0: 283e 3d31 2e35 2e36 2c21 3d31 2e35 2e37  (>=1.5.6,!=1.5.7
-000205e0: 2c3c 322e 3029 225d 0a0a 5b5b 7061 636b  ,<2.0)"]..[[pack
-000205f0: 6167 655d 5d0a 6e61 6d65 203d 2022 7669  age]].name = "vi
-00020600: 7274 7561 6c65 6e76 220a 7665 7273 696f  rtualenv".versio
-00020610: 6e20 3d20 2232 302e 3233 2e30 220a 6465  n = "20.23.0".de
-00020620: 7363 7269 7074 696f 6e20 3d20 2256 6972  scription = "Vir
-00020630: 7475 616c 2050 7974 686f 6e20 456e 7669  tual Python Envi
-00020640: 726f 6e6d 656e 7420 6275 696c 6465 7222  ronment builder"
-00020650: 0a6f 7074 696f 6e61 6c20 3d20 6661 6c73  .optional = fals
-00020660: 650a 7079 7468 6f6e 2d76 6572 7369 6f6e  e.python-version
-00020670: 7320 3d20 223e 3d33 2e37 220a 6669 6c65  s = ">=3.7".file
-00020680: 7320 3d20 5b0a 2020 2020 7b66 696c 6520  s = [.    {file 
-00020690: 3d20 2276 6972 7475 616c 656e 762d 3230  = "virtualenv-20
-000206a0: 2e32 332e 302d 7079 332d 6e6f 6e65 2d61  .23.0-py3-none-a
-000206b0: 6e79 2e77 686c 222c 2068 6173 6820 3d20  ny.whl", hash = 
-000206c0: 2273 6861 3235 363a 3661 6265 6337 3637  "sha256:6abec767
-000206d0: 3065 3538 3032 6135 3238 3335 3766 6463  0e5802a528357fdc
-000206e0: 3735 6232 3662 3966 3537 6435 6439 3266  75b26b9f57d5d92f
-000206f0: 3239 6335 3436 3262 6130 6662 6534 3566  29c5462ba0fbe45f
-00020700: 6561 6363 3638 3565 227d 2c0a 2020 2020  eacc685e"},.    
-00020710: 7b66 696c 6520 3d20 2276 6972 7475 616c  {file = "virtual
-00020720: 656e 762d 3230 2e32 332e 302e 7461 722e  env-20.23.0.tar.
-00020730: 677a 222c 2068 6173 6820 3d20 2273 6861  gz", hash = "sha
-00020740: 3235 363a 6138 3563 6161 3535 3463 6564  256:a85caa554ced
-00020750: 3063 3061 6662 6430 6436 3338 6537 6532  0c0afbd0d638e7e2
-00020760: 6437 6235 6639 3264 3233 3437 3864 3035  d7b5f92d23478d05
-00020770: 6431 3761 3736 6461 6561 6338 6632 3739  d17a76daeac8f279
-00020780: 6639 3234 227d 2c0a 5d0a 0a5b 7061 636b  f924"},.]..[pack
-00020790: 6167 652e 6465 7065 6e64 656e 6369 6573  age.dependencies
-000207a0: 5d0a 6469 7374 6c69 6220 3d20 223e 3d30  ].distlib = ">=0
-000207b0: 2e33 2e36 2c3c 3122 0a66 696c 656c 6f63  .3.6,<1".fileloc
-000207c0: 6b20 3d20 223e 3d33 2e31 312c 3c34 220a  k = ">=3.11,<4".
-000207d0: 706c 6174 666f 726d 6469 7273 203d 2022  platformdirs = "
-000207e0: 3e3d 332e 322c 3c34 220a 0a5b 7061 636b  >=3.2,<4"..[pack
-000207f0: 6167 652e 6578 7472 6173 5d0a 646f 6373  age.extras].docs
-00020800: 203d 205b 2266 7572 6f20 283e 3d32 3032   = ["furo (>=202
-00020810: 332e 332e 3237 2922 2c20 2270 726f 7365  3.3.27)", "prose
-00020820: 6c69 6e74 2028 3e3d 302e 3133 2922 2c20  lint (>=0.13)", 
-00020830: 2273 7068 696e 7820 283e 3d36 2e31 2e33  "sphinx (>=6.1.3
-00020840: 2922 2c20 2273 7068 696e 782d 6172 6770  )", "sphinx-argp
-00020850: 6172 7365 2028 3e3d 302e 3429 222c 2022  arse (>=0.4)", "
-00020860: 7370 6869 6e78 636f 6e74 7269 622d 746f  sphinxcontrib-to
-00020870: 776e 6372 6965 7220 283e 3d30 2e32 2e31  wncrier (>=0.2.1
-00020880: 6130 2922 2c20 2274 6f77 6e63 7269 6572  a0)", "towncrier
-00020890: 2028 3e3d 3232 2e31 3229 225d 0a74 6573   (>=22.12)"].tes
-000208a0: 7420 3d20 5b22 636f 7664 6566 6175 6c74  t = ["covdefault
-000208b0: 7320 283e 3d32 2e33 2922 2c20 2263 6f76  s (>=2.3)", "cov
-000208c0: 6572 6167 6520 283e 3d37 2e32 2e33 2922  erage (>=7.2.3)"
-000208d0: 2c20 2263 6f76 6572 6167 652d 656e 6162  , "coverage-enab
-000208e0: 6c65 2d73 7562 7072 6f63 6573 7320 283e  le-subprocess (>
-000208f0: 3d31 2922 2c20 2266 6c61 6b79 2028 3e3d  =1)", "flaky (>=
-00020900: 332e 3729 222c 2022 7061 636b 6167 696e  3.7)", "packagin
-00020910: 6720 283e 3d32 332e 3129 222c 2022 7079  g (>=23.1)", "py
-00020920: 7465 7374 2028 3e3d 372e 332e 3129 222c  test (>=7.3.1)",
-00020930: 2022 7079 7465 7374 2d65 6e76 2028 3e3d   "pytest-env (>=
-00020940: 302e 382e 3129 222c 2022 7079 7465 7374  0.8.1)", "pytest
-00020950: 2d66 7265 657a 6567 756e 2028 3e3d 302e  -freezegun (>=0.
-00020960: 342e 3229 222c 2022 7079 7465 7374 2d6d  4.2)", "pytest-m
-00020970: 6f63 6b20 283e 3d33 2e31 3029 222c 2022  ock (>=3.10)", "
-00020980: 7079 7465 7374 2d72 616e 646f 6d6c 7920  pytest-randomly 
-00020990: 283e 3d33 2e31 3229 222c 2022 7079 7465  (>=3.12)", "pyte
-000209a0: 7374 2d74 696d 656f 7574 2028 3e3d 322e  st-timeout (>=2.
-000209b0: 3129 222c 2022 7365 7475 7074 6f6f 6c73  1)", "setuptools
-000209c0: 2028 3e3d 3637 2e37 2e31 2922 2c20 2274   (>=67.7.1)", "t
-000209d0: 696d 652d 6d61 6368 696e 6520 283e 3d32  ime-machine (>=2
-000209e0: 2e39 2922 5d0a 0a5b 5b70 6163 6b61 6765  .9)"]..[[package
-000209f0: 5d5d 0a6e 616d 6520 3d20 2277 6174 6368  ]].name = "watch
-00020a00: 646f 6722 0a76 6572 7369 6f6e 203d 2022  dog".version = "
-00020a10: 332e 302e 3022 0a64 6573 6372 6970 7469  3.0.0".descripti
-00020a20: 6f6e 203d 2022 4669 6c65 7379 7374 656d  on = "Filesystem
-00020a30: 2065 7665 6e74 7320 6d6f 6e69 746f 7269   events monitori
-00020a40: 6e67 220a 6f70 7469 6f6e 616c 203d 2066  ng".optional = f
-00020a50: 616c 7365 0a70 7974 686f 6e2d 7665 7273  alse.python-vers
-00020a60: 696f 6e73 203d 2022 3e3d 332e 3722 0a66  ions = ">=3.7".f
-00020a70: 696c 6573 203d 205b 0a20 2020 207b 6669  iles = [.    {fi
-00020a80: 6c65 203d 2022 7761 7463 6864 6f67 2d33  le = "watchdog-3
-00020a90: 2e30 2e30 2d63 7033 3130 2d63 7033 3130  .0.0-cp310-cp310
-00020aa0: 2d6d 6163 6f73 785f 3130 5f39 5f75 6e69  -macosx_10_9_uni
-00020ab0: 7665 7273 616c 322e 7768 6c22 2c20 6861  versal2.whl", ha
-00020ac0: 7368 203d 2022 7368 6132 3536 3a33 3336  sh = "sha256:336
-00020ad0: 6164 6663 3666 3563 6334 6530 3337 6435  adfc6f5cc4e037d5
-00020ae0: 3264 6233 3131 3934 6637 3538 3166 6637  2db31194f7581ff7
-00020af0: 3434 6236 3733 3832 6562 3630 3231 6338  44b67382eb6021c8
-00020b00: 3638 3332 3265 3332 6565 6634 3122 7d2c  68322e32eef41"},
-00020b10: 0a20 2020 207b 6669 6c65 203d 2022 7761  .    {file = "wa
-00020b20: 7463 6864 6f67 2d33 2e30 2e30 2d63 7033  tchdog-3.0.0-cp3
-00020b30: 3130 2d63 7033 3130 2d6d 6163 6f73 785f  10-cp310-macosx_
-00020b40: 3130 5f39 5f78 3836 5f36 342e 7768 6c22  10_9_x86_64.whl"
-00020b50: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00020b60: 3a61 3730 6138 6463 6465 3931 6265 3532  :a70a8dcde91be52
-00020b70: 3363 3335 6232 6266 3936 3139 3665 6463  3c35b2bf96196edc
-00020b80: 3537 3330 6564 6233 3437 6533 3734 6337  5730edb347e374c7
-00020b90: 6465 3763 6432 3063 3433 6564 3935 3339  de7cd20c43ed9539
-00020ba0: 3722 7d2c 0a20 2020 207b 6669 6c65 203d  7"},.    {file =
-00020bb0: 2022 7761 7463 6864 6f67 2d33 2e30 2e30   "watchdog-3.0.0
-00020bc0: 2d63 7033 3130 2d63 7033 3130 2d6d 6163  -cp310-cp310-mac
-00020bd0: 6f73 785f 3131 5f30 5f61 726d 3634 2e77  osx_11_0_arm64.w
-00020be0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
-00020bf0: 3235 363a 6164 6664 6561 6232 6461 3739  256:adfdeab2da79
-00020c00: 6561 3266 3736 6638 3765 6234 3261 3361  ea2f76f87eb42a3a
-00020c10: 6231 3936 3661 3533 3133 6535 6136 3961  b1966a5313e5a69a
-00020c20: 3032 3133 6133 6363 3036 6566 3639 3262  0213a3cc06ef692b
-00020c30: 3065 3936 227d 2c0a 2020 2020 7b66 696c  0e96"},.    {fil
-00020c40: 6520 3d20 2277 6174 6368 646f 672d 332e  e = "watchdog-3.
-00020c50: 302e 302d 6370 3331 312d 6370 3331 312d  0.0-cp311-cp311-
-00020c60: 6d61 636f 7378 5f31 305f 395f 756e 6976  macosx_10_9_univ
-00020c70: 6572 7361 6c32 2e77 686c 222c 2068 6173  ersal2.whl", has
-00020c80: 6820 3d20 2273 6861 3235 363a 3262 3537  h = "sha256:2b57
-00020c90: 6131 6537 3330 6166 3331 3536 6431 3362  a1e730af3156d13b
-00020ca0: 3766 6464 6466 6332 3364 6561 3634 3837  7fdddfc23dea6487
-00020cb0: 6663 6563 6132 3966 6337 3563 3561 3836  fceca29fc75c5a86
-00020cc0: 3862 6565 6432 3931 3737 6165 227d 2c0a  8beed29177ae"},.
-00020cd0: 2020 2020 7b66 696c 6520 3d20 2277 6174      {file = "wat
-00020ce0: 6368 646f 672d 332e 302e 302d 6370 3331  chdog-3.0.0-cp31
-00020cf0: 312d 6370 3331 312d 6d61 636f 7378 5f31  1-cp311-macosx_1
-00020d00: 305f 395f 7838 365f 3634 2e77 686c 222c  0_9_x86_64.whl",
-00020d10: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
-00020d20: 3761 6465 3838 6430 6437 3738 6231 6232  7ade88d0d778b1b2
-00020d30: 3232 6164 6562 6363 3039 3237 3432 3866  22adebcc0927428f
-00020d40: 3838 3364 6230 3730 3137 3631 3861 3565  883db07017618a5e
-00020d50: 3638 3466 6430 3362 3833 3334 3262 6439  684fd03b83342bd9
-00020d60: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
-00020d70: 2277 6174 6368 646f 672d 332e 302e 302d  "watchdog-3.0.0-
-00020d80: 6370 3331 312d 6370 3331 312d 6d61 636f  cp311-cp311-maco
-00020d90: 7378 5f31 315f 305f 6172 6d36 342e 7768  sx_11_0_arm64.wh
-00020da0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-00020db0: 3536 3a37 6534 3437 6431 3732 6166 3532  56:7e447d172af52
-00020dc0: 6164 3230 3464 3139 3938 3237 3339 6161  ad204d19982739aa
-00020dd0: 3233 3436 3234 3563 6335 6261 3666 3537  2346245cc5ba6f57
-00020de0: 3964 3136 6461 6334 6266 6563 3232 3664  9d16dac4bfec226d
-00020df0: 3265 3722 7d2c 0a20 2020 207b 6669 6c65  2e7"},.    {file
-00020e00: 203d 2022 7761 7463 6864 6f67 2d33 2e30   = "watchdog-3.0
-00020e10: 2e30 2d63 7033 372d 6370 3337 6d2d 6d61  .0-cp37-cp37m-ma
-00020e20: 636f 7378 5f31 305f 395f 7838 365f 3634  cosx_10_9_x86_64
-00020e30: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
-00020e40: 6861 3235 363a 3966 6163 3433 6137 3436  ha256:9fac43a746
-00020e50: 3665 6237 3365 3634 6139 3934 3061 6339  6eb73e64a9940ac9
-00020e60: 6564 3633 3639 6261 6133 3962 3362 6632  ed6369baa39b3bf2
-00020e70: 3231 6165 3233 3439 3361 3965 6334 6430  21ae23493a9ec4d0
-00020e80: 3032 3236 3734 227d 2c0a 2020 2020 7b66  022674"},.    {f
-00020e90: 696c 6520 3d20 2277 6174 6368 646f 672d  ile = "watchdog-
-00020ea0: 332e 302e 302d 6370 3338 2d63 7033 382d  3.0.0-cp38-cp38-
-00020eb0: 6d61 636f 7378 5f31 305f 395f 756e 6976  macosx_10_9_univ
-00020ec0: 6572 7361 6c32 2e77 686c 222c 2068 6173  ersal2.whl", has
-00020ed0: 6820 3d20 2273 6861 3235 363a 3861 6539  h = "sha256:8ae9
-00020ee0: 6364 6134 3166 6131 3134 6532 3866 6166  cda41fa114e28faf
-00020ef0: 3836 6362 3133 3764 3735 3161 3137 6666  86cb137d751a17ff
-00020f00: 6430 3331 3664 3163 3334 6363 6632 3233  d0316d1c34ccf223
-00020f10: 3565 3861 3834 3336 3563 3766 227d 2c0a  5e8a84365c7f"},.
-00020f20: 2020 2020 7b66 696c 6520 3d20 2277 6174      {file = "wat
-00020f30: 6368 646f 672d 332e 302e 302d 6370 3338  chdog-3.0.0-cp38
-00020f40: 2d63 7033 382d 6d61 636f 7378 5f31 305f  -cp38-macosx_10_
-00020f50: 395f 7838 365f 3634 2e77 686c 222c 2068  9_x86_64.whl", h
-00020f60: 6173 6820 3d20 2273 6861 3235 363a 3235  ash = "sha256:25
-00020f70: 6637 3062 3461 6135 3362 6437 3433 3732  f70b4aa53bd74372
-00020f80: 3963 3734 3735 6437 6563 3431 3039 3361  9c7475d7ec41093a
-00020f90: 3538 3035 3238 6231 3030 6539 6138 6335  580528b100e9a8c5
-00020fa0: 6235 6566 6538 3839 3935 3932 6663 227d  b5efe8899592fc"}
-00020fb0: 2c0a 2020 2020 7b66 696c 6520 3d20 2277  ,.    {file = "w
-00020fc0: 6174 6368 646f 672d 332e 302e 302d 6370  atchdog-3.0.0-cp
-00020fd0: 3338 2d63 7033 382d 6d61 636f 7378 5f31  38-cp38-macosx_1
-00020fe0: 315f 305f 6172 6d36 342e 7768 6c22 2c20  1_0_arm64.whl", 
-00020ff0: 6861 7368 203d 2022 7368 6132 3536 3a34  hash = "sha256:4
-00021000: 6639 3430 3639 6562 3136 3635 3764 3263  f94069eb16657d2c
-00021010: 3666 6161 6461 3436 3234 6333 3934 3634  6faada4624c39464
-00021020: 6636 3563 3035 3630 3661 6635 3062 6237  f65c05606af50bb7
-00021030: 3930 3265 3033 3665 3332 3139 6265 3322  902e036e3219be3"
-00021040: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-00021050: 7761 7463 6864 6f67 2d33 2e30 2e30 2d63  watchdog-3.0.0-c
-00021060: 7033 392d 6370 3339 2d6d 6163 6f73 785f  p39-cp39-macosx_
-00021070: 3130 5f39 5f75 6e69 7665 7273 616c 322e  10_9_universal2.
-00021080: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
-00021090: 6132 3536 3a37 6335 6638 3462 3531 3934  a256:7c5f84b5194
-000210a0: 6332 3464 6435 3733 6661 3634 3732 3638  c24dd573fa647268
-000210b0: 3562 3261 3237 6363 3561 3137 6665 3566  5b2a27cc5a17fe5f
-000210c0: 3762 3666 6434 3033 3435 3337 3863 6136  7b6fd40345378ca6
-000210d0: 3831 3265 3322 7d2c 0a20 2020 207b 6669  812e3"},.    {fi
-000210e0: 6c65 203d 2022 7761 7463 6864 6f67 2d33  le = "watchdog-3
-000210f0: 2e30 2e30 2d63 7033 392d 6370 3339 2d6d  .0.0-cp39-cp39-m
-00021100: 6163 6f73 785f 3130 5f39 5f78 3836 5f36  acosx_10_9_x86_6
-00021110: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-00021120: 7368 6132 3536 3a33 6161 3766 3661 3132  sha256:3aa7f6a12
-00021130: 6538 3331 6464 6665 3738 6364 6434 6638  e831ddfe78cdd4f8
-00021140: 3939 3661 6639 6366 3333 3466 6436 3334  996af9cf334fd634
-00021150: 3635 3331 6231 3663 6563 3631 6333 6233  6531b16cec61c3b3
-00021160: 6330 6438 6461 3022 7d2c 0a20 2020 207b  c0d8da0"},.    {
-00021170: 6669 6c65 203d 2022 7761 7463 6864 6f67  file = "watchdog
-00021180: 2d33 2e30 2e30 2d63 7033 392d 6370 3339  -3.0.0-cp39-cp39
-00021190: 2d6d 6163 6f73 785f 3131 5f30 5f61 726d  -macosx_11_0_arm
-000211a0: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
-000211b0: 2273 6861 3235 363a 3233 3362 3538 3137  "sha256:233b5817
-000211c0: 3933 3236 3835 6433 3961 3738 3936 6231  932685d39a7896b1
-000211d0: 3039 3033 3533 6663 3865 6663 3165 6639  090353fc8efc1ef9
-000211e0: 3963 3963 3035 3465 3436 6338 3030 3235  9c9c054e46c80025
-000211f0: 3631 3235 3266 6238 227d 2c0a 2020 2020  61252fb8"},.    
-00021200: 7b66 696c 6520 3d20 2277 6174 6368 646f  {file = "watchdo
-00021210: 672d 332e 302e 302d 7070 3337 2d70 7970  g-3.0.0-pp37-pyp
-00021220: 7933 375f 7070 3733 2d6d 6163 6f73 785f  y37_pp73-macosx_
-00021230: 3130 5f39 5f78 3836 5f36 342e 7768 6c22  10_9_x86_64.whl"
-00021240: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00021250: 3a31 3362 6262 6234 3632 6565 3432 6563  :13bbbb462ee42ec
-00021260: 3363 3537 3233 6531 3230 3562 6538 6365  3c5723e1205be8ce
-00021270: 6437 3736 6630 3562 3130 3065 3437 3337  d776f05b100e4737
-00021280: 3531 3863 3637 6338 3332 3563 6636 3130  518c67c8325cf610
-00021290: 3022 7d2c 0a20 2020 207b 6669 6c65 203d  0"},.    {file =
-000212a0: 2022 7761 7463 6864 6f67 2d33 2e30 2e30   "watchdog-3.0.0
-000212b0: 2d70 7033 382d 7079 7079 3338 5f70 7037  -pp38-pypy38_pp7
-000212c0: 332d 6d61 636f 7378 5f31 305f 395f 7838  3-macosx_10_9_x8
-000212d0: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
-000212e0: 3d20 2273 6861 3235 363a 3866 3363 6565  = "sha256:8f3cee
-000212f0: 6364 3230 6437 3130 3637 6337 6664 3463  cd20d71067c7fd4c
-00021300: 3965 3833 3264 3465 3232 3538 3433 3138  9e832d4e22584318
-00021310: 3938 3363 6162 6330 3133 6462 6633 6637  983cabc013dbf3f7
-00021320: 3065 6139 3564 6533 3436 227d 2c0a 2020  0ea95de346"},.  
-00021330: 2020 7b66 696c 6520 3d20 2277 6174 6368    {file = "watch
-00021340: 646f 672d 332e 302e 302d 7070 3339 2d70  dog-3.0.0-pp39-p
-00021350: 7970 7933 395f 7070 3733 2d6d 6163 6f73  ypy39_pp73-macos
-00021360: 785f 3130 5f39 5f78 3836 5f36 342e 7768  x_10_9_x86_64.wh
-00021370: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-00021380: 3536 3a63 3964 3863 3865 6337 6566 6238  56:c9d8c8ec7efb8
-00021390: 3837 3333 3363 6637 3165 3332 3865 3339  87333cf71e328e39
-000213a0: 6366 6662 6637 3731 6438 6638 6639 3564  cffbf771d8f8f95d
-000213b0: 3330 3865 6134 3132 3562 6635 6639 3062  308ea4125bf5f90b
-000213c0: 6136 3422 7d2c 0a20 2020 207b 6669 6c65  a64"},.    {file
-000213d0: 203d 2022 7761 7463 6864 6f67 2d33 2e30   = "watchdog-3.0
-000213e0: 2e30 2d70 7933 2d6e 6f6e 652d 6d61 6e79  .0-py3-none-many
-000213f0: 6c69 6e75 7832 3031 345f 6161 7263 6836  linux2014_aarch6
-00021400: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
-00021410: 7368 6132 3536 3a30 6530 3661 6238 3835  sha256:0e06ab885
-00021420: 3861 3736 6531 3231 3965 3638 6337 3537  8a76e1219e68c757
-00021430: 3364 6665 6261 3964 6431 6330 3231 3934  3dfeba9dd1c02194
-00021440: 3736 6335 6134 3464 3533 3333 6230 3164  76c5a44d5333b01d
-00021450: 3765 3137 3433 6122 7d2c 0a20 2020 207b  7e1743a"},.    {
-00021460: 6669 6c65 203d 2022 7761 7463 6864 6f67  file = "watchdog
-00021470: 2d33 2e30 2e30 2d70 7933 2d6e 6f6e 652d  -3.0.0-py3-none-
-00021480: 6d61 6e79 6c69 6e75 7832 3031 345f 6172  manylinux2014_ar
-00021490: 6d76 376c 2e77 686c 222c 2068 6173 6820  mv7l.whl", hash 
-000214a0: 3d20 2273 6861 3235 363a 6430 3065 3662  = "sha256:d00e6b
-000214b0: 6534 3836 6166 6662 3537 3831 3436 3834  e486affb57814684
-000214c0: 3537 6232 3161 3663 6265 3834 3863 3333  57b21a6cbe848c33
-000214d0: 6566 3433 6639 6561 3461 3733 6234 3838  ef43f9ea4a73b488
-000214e0: 3265 3566 3138 3861 3434 227d 2c0a 2020  2e5f188a44"},.  
-000214f0: 2020 7b66 696c 6520 3d20 2277 6174 6368    {file = "watch
-00021500: 646f 672d 332e 302e 302d 7079 332d 6e6f  dog-3.0.0-py3-no
-00021510: 6e65 2d6d 616e 796c 696e 7578 3230 3134  ne-manylinux2014
-00021520: 5f69 3638 362e 7768 6c22 2c20 6861 7368  _i686.whl", hash
-00021530: 203d 2022 7368 6132 3536 3a63 3037 3235   = "sha256:c0725
-00021540: 3330 3838 3236 3563 3336 3364 3164 6466  3088265c363d1ddf
-00021550: 3462 3363 6462 3830 3864 3539 6130 3436  4b3cdb808d59a046
-00021560: 3865 6364 3031 3737 3730 6564 3731 3639  8ecd017770ed7169
-00021570: 3931 3632 3062 3866 3737 6122 7d2c 0a20  91620b8f77a"},. 
-00021580: 2020 207b 6669 6c65 203d 2022 7761 7463     {file = "watc
-00021590: 6864 6f67 2d33 2e30 2e30 2d70 7933 2d6e  hdog-3.0.0-py3-n
-000215a0: 6f6e 652d 6d61 6e79 6c69 6e75 7832 3031  one-manylinux201
-000215b0: 345f 7070 6336 342e 7768 6c22 2c20 6861  4_ppc64.whl", ha
-000215c0: 7368 203d 2022 7368 6132 3536 3a35 3131  sh = "sha256:511
-000215d0: 3333 3334 6366 3863 6630 6163 3863 6434  3334cf8cf0ac8cd4
-000215e0: 3565 3166 3833 3039 6136 3033 3239 3162  5e1f8309a603291b
-000215f0: 3631 3431 3931 6339 6164 6433 3464 3333  614191c9add34d33
-00021600: 3037 3537 3237 6139 3637 3730 3922 7d2c  075727a967709"},
-00021610: 0a20 2020 207b 6669 6c65 203d 2022 7761  .    {file = "wa
-00021620: 7463 6864 6f67 2d33 2e30 2e30 2d70 7933  tchdog-3.0.0-py3
-00021630: 2d6e 6f6e 652d 6d61 6e79 6c69 6e75 7832  -none-manylinux2
-00021640: 3031 345f 7070 6336 346c 652e 7768 6c22  014_ppc64le.whl"
-00021650: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00021660: 3a35 3166 3930 6637 3362 3436 3937 6261  :51f90f73b4697ba
-00021670: 6339 6339 6137 3833 3934 6333 6163 6262  c9c9a78394c3acbb
-00021680: 6433 3331 6363 6433 3635 3563 3131 6265  d331ccd3655c11be
-00021690: 3161 3135 6165 3666 6532 3839 6138 6338  1a15ae6fe289a8c8
-000216a0: 3322 7d2c 0a20 2020 207b 6669 6c65 203d  3"},.    {file =
-000216b0: 2022 7761 7463 6864 6f67 2d33 2e30 2e30   "watchdog-3.0.0
-000216c0: 2d70 7933 2d6e 6f6e 652d 6d61 6e79 6c69  -py3-none-manyli
-000216d0: 6e75 7832 3031 345f 7333 3930 782e 7768  nux2014_s390x.wh
-000216e0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
-000216f0: 3536 3a62 6130 3765 3932 3735 3663 3937  56:ba07e92756c97
-00021700: 6533 6163 6130 3931 3262 3563 6263 3465  e3aca0912b5cbc4e
-00021710: 3561 6438 3032 6634 3535 3732 3132 3738  5ad802f455721278
-00021720: 3865 3732 6137 3261 3437 6666 3337 3639  8e72a72a47ff3769
-00021730: 3530 6422 7d2c 0a20 2020 207b 6669 6c65  50d"},.    {file
-00021740: 203d 2022 7761 7463 6864 6f67 2d33 2e30   = "watchdog-3.0
-00021750: 2e30 2d70 7933 2d6e 6f6e 652d 6d61 6e79  .0-py3-none-many
-00021760: 6c69 6e75 7832 3031 345f 7838 365f 3634  linux2014_x86_64
-00021770: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
-00021780: 6861 3235 363a 6434 3239 6332 3433 3063  ha256:d429c2430c
-00021790: 3933 6237 3930 3339 3134 6534 6462 3961  93b7903914e4db9a
-000217a0: 3936 3663 3766 3262 3036 3864 6432 6562  966c7f2b068dd2eb
-000217b0: 6464 3266 6139 6239 6365 3039 3463 3764  dd2fa9b9ce094c7d
-000217c0: 3435 3966 3333 227d 2c0a 2020 2020 7b66  459f33"},.    {f
-000217d0: 696c 6520 3d20 2277 6174 6368 646f 672d  ile = "watchdog-
-000217e0: 332e 302e 302d 7079 332d 6e6f 6e65 2d77  3.0.0-py3-none-w
-000217f0: 696e 3332 2e77 686c 222c 2068 6173 6820  in32.whl", hash 
-00021800: 3d20 2273 6861 3235 363a 3365 6437 6337  = "sha256:3ed7c7
-00021810: 3161 3964 6363 6665 3833 3863 3266 3062  1a9dccfe838c2f0b
-00021820: 3633 3134 6564 3064 3962 3232 6537 3764  6314ed0d9b22e77d
-00021830: 3236 3863 3637 6530 3135 3435 3061 3239  268c67e015450a29
-00021840: 3033 3661 3831 6636 3066 227d 2c0a 2020  036a81f60f"},.  
-00021850: 2020 7b66 696c 6520 3d20 2277 6174 6368    {file = "watch
-00021860: 646f 672d 332e 302e 302d 7079 332d 6e6f  dog-3.0.0-py3-no
-00021870: 6e65 2d77 696e 5f61 6d64 3634 2e77 686c  ne-win_amd64.whl
-00021880: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
-00021890: 363a 3463 3939 3536 6432 3762 6530 6262  6:4c9956d27be0bb
-000218a0: 3038 6663 3566 3330 6439 6430 3137 3961  08fc5f30d9d0179a
-000218b0: 3835 3534 3336 6536 3535 6630 3436 6432  855436e655f046d2
-000218c0: 3838 6532 6263 6331 3161 6466 6165 3839  88e2bcc11adfae89
-000218d0: 3363 227d 2c0a 2020 2020 7b66 696c 6520  3c"},.    {file 
-000218e0: 3d20 2277 6174 6368 646f 672d 332e 302e  = "watchdog-3.0.
-000218f0: 302d 7079 332d 6e6f 6e65 2d77 696e 5f69  0-py3-none-win_i
-00021900: 6136 342e 7768 6c22 2c20 6861 7368 203d  a64.whl", hash =
-00021910: 2022 7368 6132 3536 3a35 6439 6633 6131   "sha256:5d9f3a1
-00021920: 3065 3032 6437 3337 3163 6439 3239 6235  0e02d7371cd929b5
-00021930: 6438 6631 3165 3837 6434 6261 6438 3930  d8f11e87d4bad890
-00021940: 3231 3265 6433 3930 3166 3962 3464 3638  212ed3901f9b4d68
-00021950: 3736 3762 6565 3735 3922 7d2c 0a20 2020  767bee759"},.   
-00021960: 207b 6669 6c65 203d 2022 7761 7463 6864   {file = "watchd
-00021970: 6f67 2d33 2e30 2e30 2e74 6172 2e67 7a22  og-3.0.0.tar.gz"
-00021980: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00021990: 3a34 6439 3861 3332 3035 3935 6461 3761  :4d98a320595da7a
-000219a0: 3763 3561 3138 6663 3438 6362 3633 3363  7c5a18fc48cb633c
-000219b0: 3265 3733 6364 6137 3866 3933 6361 6332  2e73cda78f93cac2
-000219c0: 6566 3432 6434 3262 6636 3039 6133 3366  ef42d42bf609a33f
-000219d0: 3922 7d2c 0a5d 0a0a 5b70 6163 6b61 6765  9"},.]..[package
-000219e0: 2e65 7874 7261 735d 0a77 6174 6368 6d65  .extras].watchme
-000219f0: 646f 203d 205b 2250 7959 414d 4c20 283e  do = ["PyYAML (>
-00021a00: 3d33 2e31 3029 225d 0a0a 5b5b 7061 636b  =3.10)"]..[[pack
-00021a10: 6167 655d 5d0a 6e61 6d65 203d 2022 7765  age]].name = "we
-00021a20: 6265 6e63 6f64 696e 6773 220a 7665 7273  bencodings".vers
-00021a30: 696f 6e20 3d20 2230 2e35 2e31 220a 6465  ion = "0.5.1".de
-00021a40: 7363 7269 7074 696f 6e20 3d20 2243 6861  scription = "Cha
-00021a50: 7261 6374 6572 2065 6e63 6f64 696e 6720  racter encoding 
-00021a60: 616c 6961 7365 7320 666f 7220 6c65 6761  aliases for lega
-00021a70: 6379 2077 6562 2063 6f6e 7465 6e74 220a  cy web content".
-00021a80: 6f70 7469 6f6e 616c 203d 2066 616c 7365  optional = false
-00021a90: 0a70 7974 686f 6e2d 7665 7273 696f 6e73  .python-versions
-00021aa0: 203d 2022 2a22 0a66 696c 6573 203d 205b   = "*".files = [
-00021ab0: 0a20 2020 207b 6669 6c65 203d 2022 7765  .    {file = "we
-00021ac0: 6265 6e63 6f64 696e 6773 2d30 2e35 2e31  bencodings-0.5.1
-00021ad0: 2d70 7932 2e70 7933 2d6e 6f6e 652d 616e  -py2.py3-none-an
-00021ae0: 792e 7768 6c22 2c20 6861 7368 203d 2022  y.whl", hash = "
-00021af0: 7368 6132 3536 3a61 3061 6631 3231 3366  sha256:a0af1213f
-00021b00: 3363 3232 3236 3439 3761 3937 6532 6233  3c2226497a97e2b3
-00021b10: 6161 3031 6137 6534 6265 6534 6634 3033  aa01a7e4bee4f403
-00021b20: 6639 3562 6531 3666 6339 6163 6432 3934  f95be16fc9acd294
-00021b30: 3735 3134 6137 3822 7d2c 0a20 2020 207b  7514a78"},.    {
-00021b40: 6669 6c65 203d 2022 7765 6265 6e63 6f64  file = "webencod
-00021b50: 696e 6773 2d30 2e35 2e31 2e74 6172 2e67  ings-0.5.1.tar.g
-00021b60: 7a22 2c20 6861 7368 203d 2022 7368 6132  z", hash = "sha2
-00021b70: 3536 3a62 3336 6131 6332 3435 6632 6433  56:b36a1c245f2d3
-00021b80: 3034 3936 3565 6234 6530 6138 3238 3438  04965eb4e0a82848
-00021b90: 3337 3932 3431 6463 3034 6238 3635 6166  379241dc04b865af
-00021ba0: 6363 3461 6162 3136 3734 3835 3837 6531  cc4aab16748587e1
-00021bb0: 3932 3322 7d2c 0a5d 0a0a 5b5b 7061 636b  923"},.]..[[pack
-00021bc0: 6167 655d 5d0a 6e61 6d65 203d 2022 7768  age]].name = "wh
-00021bd0: 6565 6c22 0a76 6572 7369 6f6e 203d 2022  eel".version = "
-00021be0: 302e 3430 2e30 220a 6465 7363 7269 7074  0.40.0".descript
-00021bf0: 696f 6e20 3d20 2241 2062 7569 6c74 2d70  ion = "A built-p
-00021c00: 6163 6b61 6765 2066 6f72 6d61 7420 666f  ackage format fo
-00021c10: 7220 5079 7468 6f6e 220a 6f70 7469 6f6e  r Python".option
-00021c20: 616c 203d 2066 616c 7365 0a70 7974 686f  al = false.pytho
-00021c30: 6e2d 7665 7273 696f 6e73 203d 2022 3e3d  n-versions = ">=
-00021c40: 332e 3722 0a66 696c 6573 203d 205b 0a20  3.7".files = [. 
-00021c50: 2020 207b 6669 6c65 203d 2022 7768 6565     {file = "whee
-00021c60: 6c2d 302e 3430 2e30 2d70 7933 2d6e 6f6e  l-0.40.0-py3-non
-00021c70: 652d 616e 792e 7768 6c22 2c20 6861 7368  e-any.whl", hash
-00021c80: 203d 2022 7368 6132 3536 3a64 3233 3662   = "sha256:d236b
-00021c90: 3230 6537 6362 3532 3264 6166 3233 3930  20e7cb522daf2390
-00021ca0: 6661 3834 6335 3565 6561 3831 6335 6333  fa84c55eea81c5c3
-00021cb0: 3031 3930 6639 3066 3239 6165 3263 6131  0190f90f29ae2ca1
-00021cc0: 6164 3833 3535 6266 3234 3722 7d2c 0a20  ad8355bf247"},. 
-00021cd0: 2020 207b 6669 6c65 203d 2022 7768 6565     {file = "whee
-00021ce0: 6c2d 302e 3430 2e30 2e74 6172 2e67 7a22  l-0.40.0.tar.gz"
-00021cf0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
-00021d00: 3a63 6431 3139 3666 3366 6165 6532 6233  :cd1196f3faee2b3
-00021d10: 3139 3638 6436 3236 6531 3733 3163 3934  1968d626e1731c94
-00021d20: 6639 3963 6264 6236 3763 6635 6134 3665  f99cbdb67cf5a46e
-00021d30: 3466 3536 3536 6362 6565 3737 3338 3837  4f5656cbee773887
-00021d40: 3322 7d2c 0a5d 0a0a 5b70 6163 6b61 6765  3"},.]..[package
-00021d50: 2e65 7874 7261 735d 0a74 6573 7420 3d20  .extras].test = 
-00021d60: 5b22 7079 7465 7374 2028 3e3d 362e 302e  ["pytest (>=6.0.
-00021d70: 3029 225d 0a0a 5b5b 7061 636b 6167 655d  0)"]..[[package]
-00021d80: 5d0a 6e61 6d65 203d 2022 7a69 7070 220a  ].name = "zipp".
-00021d90: 7665 7273 696f 6e20 3d20 2233 2e31 352e  version = "3.15.
-00021da0: 3022 0a64 6573 6372 6970 7469 6f6e 203d  0".description =
-00021db0: 2022 4261 636b 706f 7274 206f 6620 7061   "Backport of pa
-00021dc0: 7468 6c69 622d 636f 6d70 6174 6962 6c65  thlib-compatible
-00021dd0: 206f 626a 6563 7420 7772 6170 7065 7220   object wrapper 
-00021de0: 666f 7220 7a69 7020 6669 6c65 7322 0a6f  for zip files".o
-00021df0: 7074 696f 6e61 6c20 3d20 6661 6c73 650a  ptional = false.
-00021e00: 7079 7468 6f6e 2d76 6572 7369 6f6e 7320  python-versions 
-00021e10: 3d20 223e 3d33 2e37 220a 6669 6c65 7320  = ">=3.7".files 
-00021e20: 3d20 5b0a 2020 2020 7b66 696c 6520 3d20  = [.    {file = 
-00021e30: 227a 6970 702d 332e 3135 2e30 2d70 7933  "zipp-3.15.0-py3
-00021e40: 2d6e 6f6e 652d 616e 792e 7768 6c22 2c20  -none-any.whl", 
-00021e50: 6861 7368 203d 2022 7368 6132 3536 3a34  hash = "sha256:4
-00021e60: 3839 3034 6663 3736 6136 3065 3534 3261  8904fc76a60e542a
-00021e70: 6631 3531 6164 6564 3935 3732 3663 3161  f151aded95726c1a
-00021e80: 3563 3334 6564 3433 6162 3431 3334 6235  5c34ed43ab4134b5
-00021e90: 3937 3636 3563 3836 6437 6164 3535 3622  97665c86d7ad556"
-00021ea0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
-00021eb0: 7a69 7070 2d33 2e31 352e 302e 7461 722e  zipp-3.15.0.tar.
-00021ec0: 677a 222c 2068 6173 6820 3d20 2273 6861  gz", hash = "sha
-00021ed0: 3235 363a 3131 3239 3239 6164 3634 3964  256:112929ad649d
-00021ee0: 6139 3431 6332 3364 6535 3066 3335 3661  a941c23de50f356a
-00021ef0: 3262 3535 3730 6339 3534 6236 3531 3530  2b5570c954b65150
-00021f00: 3634 3262 6363 6464 3636 6266 3139 3464  642bccdd66bf194d
-00021f10: 3232 3462 227d 2c0a 5d0a 0a5b 7061 636b  224b"},.]..[pack
-00021f20: 6167 652e 6578 7472 6173 5d0a 646f 6373  age.extras].docs
-00021f30: 203d 205b 2266 7572 6f22 2c20 226a 6172   = ["furo", "jar
-00021f40: 6163 6f2e 7061 636b 6167 696e 6720 283e  aco.packaging (>
-00021f50: 3d39 2922 2c20 226a 6172 6163 6f2e 7469  =9)", "jaraco.ti
-00021f60: 6465 6c69 6674 2028 3e3d 312e 3429 222c  delift (>=1.4)",
-00021f70: 2022 7273 742e 6c69 6e6b 6572 2028 3e3d   "rst.linker (>=
-00021f80: 312e 3929 222c 2022 7370 6869 6e78 2028  1.9)", "sphinx (
-00021f90: 3e3d 332e 3529 222c 2022 7370 6869 6e78  >=3.5)", "sphinx
-00021fa0: 2d6c 696e 7422 5d0a 7465 7374 696e 6720  -lint"].testing 
-00021fb0: 3d20 5b22 6269 672d 4f22 2c20 2266 6c61  = ["big-O", "fla
-00021fc0: 6b65 3820 283c 3529 222c 2022 6a61 7261  ke8 (<5)", "jara
-00021fd0: 636f 2e66 756e 6374 6f6f 6c73 222c 2022  co.functools", "
-00021fe0: 6a61 7261 636f 2e69 7465 7274 6f6f 6c73  jaraco.itertools
-00021ff0: 222c 2022 6d6f 7265 2d69 7465 7274 6f6f  ", "more-itertoo
-00022000: 6c73 222c 2022 7079 7465 7374 2028 3e3d  ls", "pytest (>=
-00022010: 3629 222c 2022 7079 7465 7374 2d62 6c61  6)", "pytest-bla
-00022020: 636b 2028 3e3d 302e 332e 3729 222c 2022  ck (>=0.3.7)", "
-00022030: 7079 7465 7374 2d63 6865 636b 646f 6373  pytest-checkdocs
-00022040: 2028 3e3d 322e 3429 222c 2022 7079 7465   (>=2.4)", "pyte
-00022050: 7374 2d63 6f76 222c 2022 7079 7465 7374  st-cov", "pytest
-00022060: 2d65 6e61 626c 6572 2028 3e3d 312e 3329  -enabler (>=1.3)
-00022070: 222c 2022 7079 7465 7374 2d66 6c61 6b65  ", "pytest-flake
-00022080: 3822 2c20 2270 7974 6573 742d 6d79 7079  8", "pytest-mypy
-00022090: 2028 3e3d 302e 392e 3129 225d 0a0a 5b6d   (>=0.9.1)"]..[m
-000220a0: 6574 6164 6174 615d 0a6c 6f63 6b2d 7665  etadata].lock-ve
-000220b0: 7273 696f 6e20 3d20 2232 2e30 220a 7079  rsion = "2.0".py
-000220c0: 7468 6f6e 2d76 6572 7369 6f6e 7320 3d20  thon-versions = 
-000220d0: 225e 332e 382e 3122 0a63 6f6e 7465 6e74  "^3.8.1".content
-000220e0: 2d68 6173 6820 3d20 2237 6337 3430 6162  -hash = "7c740ab
-000220f0: 6530 3133 6363 3536 6162 3464 3563 6238  e013cc56ab4d5cb8
-00022100: 3436 3165 3162 6161 3663 3437 3838 3736  461e1baa6c478876
-00022110: 6365 6663 3866 6566 3562 3631 6463 3365  cefc8fef5b61dc3e
-00022120: 6536 6366 3164 6435 3922 0a              e6cf1dd59".
+00018e70: 655d 5d0a 6e61 6d65 203d 2022 7079 7468  e]].name = "pyth
+00018e80: 6f6e 2d64 6f74 656e 7622 0a76 6572 7369  on-dotenv".versi
+00018e90: 6f6e 203d 2022 302e 3231 2e31 220a 6465  on = "0.21.1".de
+00018ea0: 7363 7269 7074 696f 6e20 3d20 2252 6561  scription = "Rea
+00018eb0: 6420 6b65 792d 7661 6c75 6520 7061 6972  d key-value pair
+00018ec0: 7320 6672 6f6d 2061 202e 656e 7620 6669  s from a .env fi
+00018ed0: 6c65 2061 6e64 2073 6574 2074 6865 6d20  le and set them 
+00018ee0: 6173 2065 6e76 6972 6f6e 6d65 6e74 2076  as environment v
+00018ef0: 6172 6961 626c 6573 220a 6f70 7469 6f6e  ariables".option
+00018f00: 616c 203d 2066 616c 7365 0a70 7974 686f  al = false.pytho
+00018f10: 6e2d 7665 7273 696f 6e73 203d 2022 3e3d  n-versions = ">=
+00018f20: 332e 3722 0a66 696c 6573 203d 205b 0a20  3.7".files = [. 
+00018f30: 2020 207b 6669 6c65 203d 2022 7079 7468     {file = "pyth
+00018f40: 6f6e 2d64 6f74 656e 762d 302e 3231 2e31  on-dotenv-0.21.1
+00018f50: 2e74 6172 2e67 7a22 2c20 6861 7368 203d  .tar.gz", hash =
+00018f60: 2022 7368 6132 3536 3a31 6339 3364 6538   "sha256:1c93de8
+00018f70: 6636 3336 6364 6533 6365 3337 3732 3932  f636cde3ce377292
+00018f80: 3831 3864 3065 3434 3062 3665 3435 6138  818d0e440b6e45a8
+00018f90: 3266 3231 3563 3337 3434 3937 3931 3531  2f215c3744979151
+00018fa0: 6661 3831 3531 6334 3922 7d2c 0a20 2020  fa8151c49"},.   
+00018fb0: 207b 6669 6c65 203d 2022 7079 7468 6f6e   {file = "python
+00018fc0: 5f64 6f74 656e 762d 302e 3231 2e31 2d70  _dotenv-0.21.1-p
+00018fd0: 7933 2d6e 6f6e 652d 616e 792e 7768 6c22  y3-none-any.whl"
+00018fe0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00018ff0: 3a34 3165 3132 6530 3331 3862 6562 6338  :41e12e0318bebc8
+00019000: 3539 6663 6334 6439 3764 3464 6238 6432  59fcc4d97d4db8d2
+00019010: 3061 6432 3137 3231 6136 6161 3530 3437  0ad21721a6aa5047
+00019020: 6464 3539 6630 3930 3339 3163 6235 3439  dd59f090391cb549
+00019030: 6122 7d2c 0a5d 0a0a 5b70 6163 6b61 6765  a"},.]..[package
+00019040: 2e65 7874 7261 735d 0a63 6c69 203d 205b  .extras].cli = [
+00019050: 2263 6c69 636b 2028 3e3d 352e 3029 225d  "click (>=5.0)"]
+00019060: 0a0a 5b5b 7061 636b 6167 655d 5d0a 6e61  ..[[package]].na
+00019070: 6d65 203d 2022 7079 746b 646f 6373 220a  me = "pytkdocs".
+00019080: 7665 7273 696f 6e20 3d20 2230 2e31 362e  version = "0.16.
+00019090: 3122 0a64 6573 6372 6970 7469 6f6e 203d  1".description =
+000190a0: 2022 4c6f 6164 2050 7974 686f 6e20 6f62   "Load Python ob
+000190b0: 6a65 6374 7320 646f 6375 6d65 6e74 6174  jects documentat
+000190c0: 696f 6e2e 220a 6f70 7469 6f6e 616c 203d  ion.".optional =
+000190d0: 2066 616c 7365 0a70 7974 686f 6e2d 7665   false.python-ve
+000190e0: 7273 696f 6e73 203d 2022 3e3d 332e 3722  rsions = ">=3.7"
+000190f0: 0a66 696c 6573 203d 205b 0a20 2020 207b  .files = [.    {
+00019100: 6669 6c65 203d 2022 7079 746b 646f 6373  file = "pytkdocs
+00019110: 2d30 2e31 362e 312d 7079 332d 6e6f 6e65  -0.16.1-py3-none
+00019120: 2d61 6e79 2e77 686c 222c 2068 6173 6820  -any.whl", hash 
+00019130: 3d20 2273 6861 3235 363a 6138 6333 6634  = "sha256:a8c3f4
+00019140: 3665 6365 6630 6239 3238 3634 6363 3539  6ecef0b92864cc59
+00019150: 3865 3931 3031 6539 6334 6366 3833 3265  8e9101e9c4cf832e
+00019160: 6262 6632 3238 6635 3063 3834 6161 3564  bbf228f50c84aa5d
+00019170: 6438 3530 6161 6333 3739 227d 2c0a 2020  d850aac379"},.  
+00019180: 2020 7b66 696c 6520 3d20 2270 7974 6b64    {file = "pytkd
+00019190: 6f63 732d 302e 3136 2e31 2e74 6172 2e67  ocs-0.16.1.tar.g
+000191a0: 7a22 2c20 6861 7368 203d 2022 7368 6132  z", hash = "sha2
+000191b0: 3536 3a65 3263 6366 3664 6665 3964 6262  56:e2ccf6dfe9dbb
+000191c0: 6365 6230 3938 3138 3637 3366 3034 3066  ceb09818673f040f
+000191d0: 3161 3763 3332 6564 3062 6666 6232 6437  1a7c32ed0bffb2d7
+000191e0: 3039 6230 3662 6536 3435 3363 3430 3236  09b06be6453c4026
+000191f0: 3034 3522 7d2c 0a5d 0a0a 5b70 6163 6b61  045"},.]..[packa
+00019200: 6765 2e64 6570 656e 6465 6e63 6965 735d  ge.dependencies]
+00019210: 0a61 7374 756e 7061 7273 6520 3d20 7b76  .astunparse = {v
+00019220: 6572 7369 6f6e 203d 2022 3e3d 312e 3622  ersion = ">=1.6"
+00019230: 2c20 6d61 726b 6572 7320 3d20 2270 7974  , markers = "pyt
+00019240: 686f 6e5f 7665 7273 696f 6e20 3c20 5c22  hon_version < \"
+00019250: 332e 395c 2222 7d0a 0a5b 7061 636b 6167  3.9\""}..[packag
+00019260: 652e 6578 7472 6173 5d0a 6e75 6d70 792d  e.extras].numpy-
+00019270: 7374 796c 6520 3d20 5b22 646f 6373 7472  style = ["docstr
+00019280: 696e 675f 7061 7273 6572 2028 3e3d 302e  ing_parser (>=0.
+00019290: 3729 225d 0a0a 5b5b 7061 636b 6167 655d  7)"]..[[package]
+000192a0: 5d0a 6e61 6d65 203d 2022 7079 7769 6e33  ].name = "pywin3
+000192b0: 3222 0a76 6572 7369 6f6e 203d 2022 3330  2".version = "30
+000192c0: 3622 0a64 6573 6372 6970 7469 6f6e 203d  6".description =
+000192d0: 2022 5079 7468 6f6e 2066 6f72 2057 696e   "Python for Win
+000192e0: 646f 7720 4578 7465 6e73 696f 6e73 220a  dow Extensions".
+000192f0: 6f70 7469 6f6e 616c 203d 2066 616c 7365  optional = false
+00019300: 0a70 7974 686f 6e2d 7665 7273 696f 6e73  .python-versions
+00019310: 203d 2022 2a22 0a66 696c 6573 203d 205b   = "*".files = [
+00019320: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+00019330: 7769 6e33 322d 3330 362d 6370 3331 302d  win32-306-cp310-
+00019340: 6370 3331 302d 7769 6e33 322e 7768 6c22  cp310-win32.whl"
+00019350: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00019360: 3a30 3664 3334 3230 6135 3135 3562 6136  :06d3420a5155ba6
+00019370: 3566 3062 3732 6632 3639 3962 3562 6163  5f0b72f2699b5bac
+00019380: 6633 3130 3966 3336 6163 6265 3839 3233  f3109f36acbe8923
+00019390: 3736 3563 3232 3933 3861 3639 6466 6338  765c22938a69dfc8
+000193a0: 6422 7d2c 0a20 2020 207b 6669 6c65 203d  d"},.    {file =
+000193b0: 2022 7079 7769 6e33 322d 3330 362d 6370   "pywin32-306-cp
+000193c0: 3331 302d 6370 3331 302d 7769 6e5f 616d  310-cp310-win_am
+000193d0: 6436 342e 7768 6c22 2c20 6861 7368 203d  d64.whl", hash =
+000193e0: 2022 7368 6132 3536 3a38 3466 3434 3731   "sha256:84f4471
+000193f0: 6462 6361 3138 3837 6561 3338 3033 6438  dbca1887ea3803d8
+00019400: 3834 3861 3136 3136 3432 3961 6339 3461  848a1616429ac94a
+00019410: 3461 3864 3035 6634 6263 3963 3564 6366  4a8d05f4bc9c5dcf
+00019420: 6434 3263 6139 3963 3822 7d2c 0a20 2020  d42ca99c8"},.   
+00019430: 207b 6669 6c65 203d 2022 7079 7769 6e33   {file = "pywin3
+00019440: 322d 3330 362d 6370 3331 312d 6370 3331  2-306-cp311-cp31
+00019450: 312d 7769 6e33 322e 7768 6c22 2c20 6861  1-win32.whl", ha
+00019460: 7368 203d 2022 7368 6132 3536 3a65 3635  sh = "sha256:e65
+00019470: 3032 3831 3333 6431 3562 3634 6432 6564  028133d15b64d2ed
+00019480: 3866 3036 6464 3966 6263 3236 3833 3532  8f06dd9fbc268352
+00019490: 3437 3864 3466 3932 3839 6536 3963 3139  478d4f9289e69c19
+000194a0: 3065 6364 3638 3138 6236 3430 3722 7d2c  0ecd6818b6407"},
+000194b0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+000194c0: 7769 6e33 322d 3330 362d 6370 3331 312d  win32-306-cp311-
+000194d0: 6370 3331 312d 7769 6e5f 616d 6436 342e  cp311-win_amd64.
+000194e0: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+000194f0: 6132 3536 3a61 3736 3339 6635 3163 3138  a256:a7639f51c18
+00019500: 3463 3032 3732 6539 3366 3234 3465 6232  4c0272e93f244eb2
+00019510: 3464 6166 6361 3962 3138 3535 3730 3764  4dafca9b1855707d
+00019520: 3934 6331 3932 6434 6130 6234 6330 3165  94c192d4a0b4c01e
+00019530: 3131 3030 6522 7d2c 0a20 2020 207b 6669  1100e"},.    {fi
+00019540: 6c65 203d 2022 7079 7769 6e33 322d 3330  le = "pywin32-30
+00019550: 362d 6370 3331 312d 6370 3331 312d 7769  6-cp311-cp311-wi
+00019560: 6e5f 6172 6d36 342e 7768 6c22 2c20 6861  n_arm64.whl", ha
+00019570: 7368 203d 2022 7368 6132 3536 3a37 3064  sh = "sha256:70d
+00019580: 6261 3063 3931 3364 3139 6639 3432 6132  ba0c913d19f942a2
+00019590: 6462 3235 3231 3764 3961 3162 3732 3663  db25217d9a1b726c
+000195a0: 3237 3866 3438 3361 3931 3966 3161 6266  278f483a919f1abf
+000195b0: 6564 3739 6339 6366 3634 6433 6122 7d2c  ed79c9cf64d3a"},
+000195c0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+000195d0: 7769 6e33 322d 3330 362d 6370 3331 322d  win32-306-cp312-
+000195e0: 6370 3331 322d 7769 6e33 322e 7768 6c22  cp312-win32.whl"
+000195f0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00019600: 3a33 3833 3232 3964 3531 3536 3537 6634  :383229d515657f4
+00019610: 6533 6564 3133 3433 6461 3862 6531 3031  e3ed1343da8be101
+00019620: 3030 3035 3632 6266 3531 3435 3931 6666  000562bf514591ff
+00019630: 3338 3361 6539 3430 6361 6436 3534 3538  383ae940cad65458
+00019640: 6222 7d2c 0a20 2020 207b 6669 6c65 203d  b"},.    {file =
+00019650: 2022 7079 7769 6e33 322d 3330 362d 6370   "pywin32-306-cp
+00019660: 3331 322d 6370 3331 322d 7769 6e5f 616d  312-cp312-win_am
+00019670: 6436 342e 7768 6c22 2c20 6861 7368 203d  d64.whl", hash =
+00019680: 2022 7368 6132 3536 3a33 3732 3537 3739   "sha256:3725779
+00019690: 3463 3161 6433 3965 6539 6265 3635 3264  4c1ad39ee9be652d
+000196a0: 6130 3436 3264 6332 6533 3934 6338 3135  a0462dc2e394c815
+000196b0: 3964 6664 3931 3361 3861 3465 3865 6236  9dfd913a8a4e8eb6
+000196c0: 6664 3334 3664 6130 6522 7d2c 0a20 2020  fd346da0e"},.   
+000196d0: 207b 6669 6c65 203d 2022 7079 7769 6e33   {file = "pywin3
+000196e0: 322d 3330 362d 6370 3331 322d 6370 3331  2-306-cp312-cp31
+000196f0: 322d 7769 6e5f 6172 6d36 342e 7768 6c22  2-win_arm64.whl"
+00019700: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00019710: 3a35 3832 3165 6335 3266 3664 3332 3161  :5821ec52f6d321a
+00019720: 6135 3965 3264 6237 6530 6133 3562 3939  a59e2db7e0a35b99
+00019730: 3764 6536 3063 3230 3139 3433 3535 3764  7de60c201943557d
+00019740: 3130 3861 6639 6434 6165 3165 6337 3034  108af9d4ae1ec704
+00019750: 3022 7d2c 0a20 2020 207b 6669 6c65 203d  0"},.    {file =
+00019760: 2022 7079 7769 6e33 322d 3330 362d 6370   "pywin32-306-cp
+00019770: 3337 2d63 7033 376d 2d77 696e 3332 2e77  37-cp37m-win32.w
+00019780: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+00019790: 3235 363a 3163 3733 6561 3961 3064 3232  256:1c73ea9a0d22
+000197a0: 3833 6438 3839 3030 3139 3938 3035 3966  83d889001998059f
+000197b0: 3565 6161 6261 3362 3632 3338 6637 3637  5eaaba3b6238f767
+000197c0: 6339 6366 3238 3333 6231 3365 3661 3638  c9cf2833b13e6a68
+000197d0: 3566 3635 227d 2c0a 2020 2020 7b66 696c  5f65"},.    {fil
+000197e0: 6520 3d20 2270 7977 696e 3332 2d33 3036  e = "pywin32-306
+000197f0: 2d63 7033 372d 6370 3337 6d2d 7769 6e5f  -cp37-cp37m-win_
+00019800: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+00019810: 203d 2022 7368 6132 3536 3a37 3263 3566   = "sha256:72c5f
+00019820: 3632 3135 3432 6437 6264 6434 6664 6237  621542d7bdd4fdb7
+00019830: 3136 3232 3762 6530 6464 3366 3835 3635  16227be0dd3f8565
+00019840: 6331 3162 3238 3062 6536 3331 3562 3036  c11b280be6315b06
+00019850: 6163 6533 3534 3837 6433 3622 7d2c 0a20  ace35487d36"},. 
+00019860: 2020 207b 6669 6c65 203d 2022 7079 7769     {file = "pywi
+00019870: 6e33 322d 3330 362d 6370 3338 2d63 7033  n32-306-cp38-cp3
+00019880: 382d 7769 6e33 322e 7768 6c22 2c20 6861  8-win32.whl", ha
+00019890: 7368 203d 2022 7368 6132 3536 3a65 3463  sh = "sha256:e4c
+000198a0: 3039 3265 3235 3839 6235 6366 3064 3336  092e2589b5cf0d36
+000198b0: 3538 3439 6537 3365 3032 6333 3931 6331  5849e73e02c391c1
+000198c0: 3334 3939 3538 6335 6163 3365 3964 3563  349958c5ac3e9d5c
+000198d0: 6362 3961 3238 6530 3137 6233 6122 7d2c  cb9a28e017b3a"},
+000198e0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+000198f0: 7769 6e33 322d 3330 362d 6370 3338 2d63  win32-306-cp38-c
+00019900: 7033 382d 7769 6e5f 616d 6436 342e 7768  p38-win_amd64.wh
+00019910: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+00019920: 3536 3a65 3861 6331 6165 3336 3031 6265  56:e8ac1ae3601be
+00019930: 6536 6361 3966 3763 6234 6235 3336 3362  e6ca9f7cb4b5363b
+00019940: 6631 6330 6261 6462 3933 3565 6632 3433  f1c0badb935ef243
+00019950: 6334 3733 3366 6639 6133 3933 6231 3639  c4733ff9a393b169
+00019960: 3063 3022 7d2c 0a20 2020 207b 6669 6c65  0c0"},.    {file
+00019970: 203d 2022 7079 7769 6e33 322d 3330 362d   = "pywin32-306-
+00019980: 6370 3339 2d63 7033 392d 7769 6e33 322e  cp39-cp39-win32.
+00019990: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+000199a0: 6132 3536 3a65 3235 6664 3562 3438 3562  a256:e25fd5b485b
+000199b0: 3535 6163 3963 3035 3766 3637 6439 3462  55ac9c057f67d94b
+000199c0: 6332 3033 6633 6636 3539 3530 3738 6431  c203f3f6595078d1
+000199d0: 6662 3362 3435 3863 3963 3238 6237 3135  fb3b458c9c28b715
+000199e0: 3361 3830 3222 7d2c 0a20 2020 207b 6669  3a802"},.    {fi
+000199f0: 6c65 203d 2022 7079 7769 6e33 322d 3330  le = "pywin32-30
+00019a00: 362d 6370 3339 2d63 7033 392d 7769 6e5f  6-cp39-cp39-win_
+00019a10: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+00019a20: 203d 2022 7368 6132 3536 3a33 3962 3631   = "sha256:39b61
+00019a30: 6331 3532 3732 3833 3362 3563 3332 3961  c15272833b5c329a
+00019a40: 3239 3839 3939 3964 6361 6538 3336 6231  2989999dcae836b1
+00019a50: 6565 6436 3530 3235 3261 6231 6237 6266  eed650252ab1b7bf
+00019a60: 6265 3164 3539 6633 3066 3422 7d2c 0a5d  be1d59f30f4"},.]
+00019a70: 0a0a 5b5b 7061 636b 6167 655d 5d0a 6e61  ..[[package]].na
+00019a80: 6d65 203d 2022 7079 7961 6d6c 220a 7665  me = "pyyaml".ve
+00019a90: 7273 696f 6e20 3d20 2236 2e30 220a 6465  rsion = "6.0".de
+00019aa0: 7363 7269 7074 696f 6e20 3d20 2259 414d  scription = "YAM
+00019ab0: 4c20 7061 7273 6572 2061 6e64 2065 6d69  L parser and emi
+00019ac0: 7474 6572 2066 6f72 2050 7974 686f 6e22  tter for Python"
+00019ad0: 0a6f 7074 696f 6e61 6c20 3d20 6661 6c73  .optional = fals
+00019ae0: 650a 7079 7468 6f6e 2d76 6572 7369 6f6e  e.python-version
+00019af0: 7320 3d20 223e 3d33 2e36 220a 6669 6c65  s = ">=3.6".file
+00019b00: 7320 3d20 5b0a 2020 2020 7b66 696c 6520  s = [.    {file 
+00019b10: 3d20 2250 7959 414d 4c2d 362e 302d 6370  = "PyYAML-6.0-cp
+00019b20: 3331 302d 6370 3331 302d 6d61 636f 7378  310-cp310-macosx
+00019b30: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
+00019b40: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+00019b50: 363a 6434 6462 3763 3761 6566 3038 3538  6:d4db7c7aef0858
+00019b60: 3732 6566 3635 6138 6664 3764 3664 3039  72ef65a8fd7d6d09
+00019b70: 6131 3461 6539 3166 3639 3164 6563 3365  a14ae91f691dec3e
+00019b80: 3837 6565 3565 6530 3533 3964 3531 3666  87ee5ee0539d516f
+00019b90: 3533 227d 2c0a 2020 2020 7b66 696c 6520  53"},.    {file 
+00019ba0: 3d20 2250 7959 414d 4c2d 362e 302d 6370  = "PyYAML-6.0-cp
+00019bb0: 3331 302d 6370 3331 302d 6d61 636f 7378  310-cp310-macosx
+00019bc0: 5f31 315f 305f 6172 6d36 342e 7768 6c22  _11_0_arm64.whl"
+00019bd0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00019be0: 3a39 6466 3765 6433 6233 6432 6530 6563  :9df7ed3b3d2e0ec
+00019bf0: 6665 3039 6531 3437 3431 6238 3537 6466  fe09e14741b857df
+00019c00: 3433 6164 6235 6133 6464 6164 6339 3139  43adb5a3ddadc919
+00019c10: 6132 6439 3466 6264 6637 3866 6561 3533  a2d94fbdf78fea53
+00019c20: 6322 7d2c 0a20 2020 207b 6669 6c65 203d  c"},.    {file =
+00019c30: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
+00019c40: 3130 2d63 7033 3130 2d6d 616e 796c 696e  10-cp310-manylin
+00019c50: 7578 5f32 5f31 375f 6161 7263 6836 342e  ux_2_17_aarch64.
+00019c60: 6d61 6e79 6c69 6e75 7832 3031 345f 6161  manylinux2014_aa
+00019c70: 7263 6836 342e 7768 6c22 2c20 6861 7368  rch64.whl", hash
+00019c80: 203d 2022 7368 6132 3536 3a37 3766 3339   = "sha256:77f39
+00019c90: 3665 3665 6634 6337 3366 6463 3333 6139  6e6ef4c73fdc33a9
+00019ca0: 3135 3734 3436 3436 3666 3163 6666 3535  157446466f1cff55
+00019cb0: 3364 3937 3962 6430 3065 6362 3634 3338  3d979bd00ecb6438
+00019cc0: 3537 3630 6336 6261 6264 6322 7d2c 0a20  5760c6babdc"},. 
+00019cd0: 2020 207b 6669 6c65 203d 2022 5079 5941     {file = "PyYA
+00019ce0: 4d4c 2d36 2e30 2d63 7033 3130 2d63 7033  ML-6.0-cp310-cp3
+00019cf0: 3130 2d6d 616e 796c 696e 7578 5f32 5f31  10-manylinux_2_1
+00019d00: 375f 7333 3930 782e 6d61 6e79 6c69 6e75  7_s390x.manylinu
+00019d10: 7832 3031 345f 7333 3930 782e 7768 6c22  x2014_s390x.whl"
+00019d20: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00019d30: 3a61 3830 6137 3830 3436 6137 3233 3631  :a80a78046a72361
+00019d40: 6465 3733 6638 6633 3935 6631 6631 6534  de73f8f395f1f1e4
+00019d50: 3966 3935 3663 3662 6538 3832 6565 6435  9f956c6be882eed5
+00019d60: 3835 3035 6131 3566 3365 3433 3039 3632  8505a15f3e430962
+00019d70: 6222 7d2c 0a20 2020 207b 6669 6c65 203d  b"},.    {file =
+00019d80: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
+00019d90: 3130 2d63 7033 3130 2d6d 616e 796c 696e  10-cp310-manylin
+00019da0: 7578 5f32 5f35 5f78 3836 5f36 342e 6d61  ux_2_5_x86_64.ma
+00019db0: 6e79 6c69 6e75 7831 5f78 3836 5f36 342e  nylinux1_x86_64.
+00019dc0: 6d61 6e79 6c69 6e75 785f 325f 3132 5f78  manylinux_2_12_x
+00019dd0: 3836 5f36 342e 6d61 6e79 6c69 6e75 7832  86_64.manylinux2
+00019de0: 3031 305f 7838 365f 3634 2e77 686c 222c  010_x86_64.whl",
+00019df0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
+00019e00: 6638 3466 6263 3938 6230 3139 6665 6632  f84fbc98b019fef2
+00019e10: 6565 3961 3163 6233 6365 3933 6533 3138  ee9a1cb3ce93e318
+00019e20: 3761 3664 6630 6232 3533 3861 3635 3162  7a6df0b2538a651b
+00019e30: 6662 3839 3032 3534 6261 3966 3930 6235  fb890254ba9f90b5
+00019e40: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
+00019e50: 2250 7959 414d 4c2d 362e 302d 6370 3331  "PyYAML-6.0-cp31
+00019e60: 302d 6370 3331 302d 7769 6e33 322e 7768  0-cp310-win32.wh
+00019e70: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+00019e80: 3536 3a32 6364 3564 6633 6465 3438 3835  56:2cd5df3de4885
+00019e90: 3765 6430 3534 3462 3334 6532 6434 3065  7ed0544b34e2d40e
+00019ea0: 3966 6163 3434 3539 3330 3033 3966 3363  9fac445930039f3c
+00019eb0: 6665 3462 6363 3539 3261 3166 3833 3664  fe4bcc592a1f836d
+00019ec0: 3531 3322 7d2c 0a20 2020 207b 6669 6c65  513"},.    {file
+00019ed0: 203d 2022 5079 5941 4d4c 2d36 2e30 2d63   = "PyYAML-6.0-c
+00019ee0: 7033 3130 2d63 7033 3130 2d77 696e 5f61  p310-cp310-win_a
+00019ef0: 6d64 3634 2e77 686c 222c 2068 6173 6820  md64.whl", hash 
+00019f00: 3d20 2273 6861 3235 363a 6461 6634 3936  = "sha256:daf496
+00019f10: 6335 3861 3863 3532 3038 3364 6630 3962  c58a8c52083df09b
+00019f20: 3830 6338 3630 3030 3531 3934 3031 3463  80c860005194014c
+00019f30: 3336 3938 3639 3864 3161 3537 6362 6366  3698698d1a57cbcf
+00019f40: 6131 3832 3134 3261 3361 227d 2c0a 2020  a182142a3a"},.  
+00019f50: 2020 7b66 696c 6520 3d20 2250 7959 414d    {file = "PyYAM
+00019f60: 4c2d 362e 302d 6370 3331 312d 6370 3331  L-6.0-cp311-cp31
+00019f70: 312d 6d61 636f 7378 5f31 305f 395f 7838  1-macosx_10_9_x8
+00019f80: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
+00019f90: 3d20 2273 6861 3235 363a 6434 6230 6261  = "sha256:d4b0ba
+00019fa0: 3935 3132 3531 3935 3232 6231 3138 3039  9512519522b11809
+00019fb0: 3032 3537 6265 3131 3362 3934 3638 6438  0257be113b9468d8
+00019fc0: 3034 6231 3964 3633 6337 3164 6263 6634  04b19d63c71dbcf4
+00019fd0: 6134 3866 6133 3233 3538 227d 2c0a 2020  a48fa32358"},.  
+00019fe0: 2020 7b66 696c 6520 3d20 2250 7959 414d    {file = "PyYAM
+00019ff0: 4c2d 362e 302d 6370 3331 312d 6370 3331  L-6.0-cp311-cp31
+0001a000: 312d 6d61 636f 7378 5f31 315f 305f 6172  1-macosx_11_0_ar
+0001a010: 6d36 342e 7768 6c22 2c20 6861 7368 203d  m64.whl", hash =
+0001a020: 2022 7368 6132 3536 3a38 3139 3537 3932   "sha256:8195792
+0001a030: 3166 3434 3164 3530 6166 3233 3635 3461  1f441d50af23654a
+0001a040: 6136 6335 6535 6561 6639 6230 3661 6261  a6c5e5eaf9b06aba
+0001a050: 3766 3061 3139 6331 3861 3533 3864 6337  7f0a19c18a538dc7
+0001a060: 6566 3239 3163 3561 3122 7d2c 0a20 2020  ef291c5a1"},.   
+0001a070: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
+0001a080: 2d36 2e30 2d63 7033 3131 2d63 7033 3131  -6.0-cp311-cp311
+0001a090: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
+0001a0a0: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
+0001a0b0: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
+0001a0c0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+0001a0d0: 3536 3a61 6661 3137 6635 6263 3464 3162  56:afa17f5bc4d1b
+0001a0e0: 3130 6166 6434 3436 3666 6433 6134 3464  10afd4466fd3a44d
+0001a0f0: 6330 6532 3435 3338 3264 6563 6135 6233  c0e245382deca5b3
+0001a100: 6333 3533 6438 6237 3537 6639 6533 6563  c353d8b757f9e3ec
+0001a110: 6238 6422 7d2c 0a20 2020 207b 6669 6c65  b8d"},.    {file
+0001a120: 203d 2022 5079 5941 4d4c 2d36 2e30 2d63   = "PyYAML-6.0-c
+0001a130: 7033 3131 2d63 7033 3131 2d6d 616e 796c  p311-cp311-manyl
+0001a140: 696e 7578 5f32 5f31 375f 7333 3930 782e  inux_2_17_s390x.
+0001a150: 6d61 6e79 6c69 6e75 7832 3031 345f 7333  manylinux2014_s3
+0001a160: 3930 782e 7768 6c22 2c20 6861 7368 203d  90x.whl", hash =
+0001a170: 2022 7368 6132 3536 3a64 6261 6430 6539   "sha256:dbad0e9
+0001a180: 6433 3638 6262 3938 3966 3435 3135 6461  d368bb989f4515da
+0001a190: 3333 3062 3838 6130 3537 3631 3764 3136  330b88a057617d16
+0001a1a0: 6236 6138 3234 3530 3834 6631 6230 3534  b6a8245084f1b054
+0001a1b0: 3030 6632 3436 3039 6622 7d2c 0a20 2020  00f24609f"},.   
+0001a1c0: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
+0001a1d0: 2d36 2e30 2d63 7033 3131 2d63 7033 3131  -6.0-cp311-cp311
+0001a1e0: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
+0001a1f0: 7838 365f 3634 2e6d 616e 796c 696e 7578  x86_64.manylinux
+0001a200: 3230 3134 5f78 3836 5f36 342e 7768 6c22  2014_x86_64.whl"
+0001a210: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001a220: 3a34 3332 3535 3761 6132 6330 3938 3032  :432557aa2c09802
+0001a230: 6265 3339 3436 3033 3630 6464 6666 6434  be39460360ddffd4
+0001a240: 3831 3536 6533 3037 3231 6635 6538 6439  8156e30721f5e8d9
+0001a250: 3137 6630 3164 3331 3639 3432 3136 3738  17f01d3169421678
+0001a260: 3222 7d2c 0a20 2020 207b 6669 6c65 203d  2"},.    {file =
+0001a270: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
+0001a280: 3131 2d63 7033 3131 2d77 696e 3332 2e77  11-cp311-win32.w
+0001a290: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+0001a2a0: 3235 363a 6266 6165 6635 3733 6136 3362  256:bfaef573a63b
+0001a2b0: 6138 3932 3335 3033 6432 3735 3330 3336  a8923503d2753036
+0001a2c0: 3235 3930 6666 3466 3537 3663 3632 3664  2590ff4f576c626d
+0001a2d0: 3836 6139 6665 6439 3538 3232 6138 3235  86a9fed95822a825
+0001a2e0: 3566 6437 227d 2c0a 2020 2020 7b66 696c  5fd7"},.    {fil
+0001a2f0: 6520 3d20 2250 7959 414d 4c2d 362e 302d  e = "PyYAML-6.0-
+0001a300: 6370 3331 312d 6370 3331 312d 7769 6e5f  cp311-cp311-win_
+0001a310: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+0001a320: 203d 2022 7368 6132 3536 3a30 3162 3435   = "sha256:01b45
+0001a330: 6330 3139 3165 3664 3636 6334 3730 6236  c0191e6d66c470b6
+0001a340: 6366 3162 3935 3331 6137 3731 6138 3363  cf1b9531a771a83c
+0001a350: 3163 3432 3038 3237 3265 6164 3437 6133  1c4208272ead47a3
+0001a360: 6165 3466 3266 3630 3362 6622 7d2c 0a20  ae4f2f603bf"},. 
+0001a370: 2020 207b 6669 6c65 203d 2022 5079 5941     {file = "PyYA
+0001a380: 4d4c 2d36 2e30 2d63 7033 362d 6370 3336  ML-6.0-cp36-cp36
+0001a390: 6d2d 6d61 636f 7378 5f31 305f 395f 7838  m-macosx_10_9_x8
+0001a3a0: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
+0001a3b0: 3d20 2273 6861 3235 363a 3839 3762 3830  = "sha256:897b80
+0001a3c0: 3839 3037 3635 6630 3337 6466 3334 3033  890765f037df3403
+0001a3d0: 6432 3262 6162 3431 3632 3763 6138 3831  d22bab41627ca881
+0001a3e0: 3161 6535 3565 3961 3732 3266 6430 3339  1ae55e9a722fd039
+0001a3f0: 3238 3530 6563 3464 3836 227d 2c0a 2020  2850ec4d86"},.  
+0001a400: 2020 7b66 696c 6520 3d20 2250 7959 414d    {file = "PyYAM
+0001a410: 4c2d 362e 302d 6370 3336 2d63 7033 366d  L-6.0-cp36-cp36m
+0001a420: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
+0001a430: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
+0001a440: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
+0001a450: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+0001a460: 3536 3a35 3036 3032 6166 6164 6136 6436  56:50602afada6d6
+0001a470: 6362 6661 6436 3939 6230 6337 6262 3530  cbfad699b0c7bb50
+0001a480: 6435 6363 6666 6137 6534 3661 3364 3733  d5ccffa7e46a3d73
+0001a490: 3830 3932 6166 6464 6331 6639 3735 3834  8092afddc1f97584
+0001a4a0: 3237 6622 7d2c 0a20 2020 207b 6669 6c65  27f"},.    {file
+0001a4b0: 203d 2022 5079 5941 4d4c 2d36 2e30 2d63   = "PyYAML-6.0-c
+0001a4c0: 7033 362d 6370 3336 6d2d 6d61 6e79 6c69  p36-cp36m-manyli
+0001a4d0: 6e75 785f 325f 3137 5f73 3339 3078 2e6d  nux_2_17_s390x.m
+0001a4e0: 616e 796c 696e 7578 3230 3134 5f73 3339  anylinux2014_s39
+0001a4f0: 3078 2e77 686c 222c 2068 6173 6820 3d20  0x.whl", hash = 
+0001a500: 2273 6861 3235 363a 3438 6333 3436 3931  "sha256:48c34691
+0001a510: 3563 3131 3466 3566 6462 3365 6164 3730  5c114f5fdb3ead70
+0001a520: 3331 3262 6430 3432 6139 3533 6138 6365  312bd042a953a8ce
+0001a530: 3563 3731 3036 6435 6266 6231 6135 3235  5c7106d5bfb1a525
+0001a540: 3465 3437 6461 3932 227d 2c0a 2020 2020  4e47da92"},.    
+0001a550: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
+0001a560: 362e 302d 6370 3336 2d63 7033 366d 2d6d  6.0-cp36-cp36m-m
+0001a570: 616e 796c 696e 7578 5f32 5f35 5f78 3836  anylinux_2_5_x86
+0001a580: 5f36 342e 6d61 6e79 6c69 6e75 7831 5f78  _64.manylinux1_x
+0001a590: 3836 5f36 342e 6d61 6e79 6c69 6e75 785f  86_64.manylinux_
+0001a5a0: 325f 3132 5f78 3836 5f36 342e 6d61 6e79  2_12_x86_64.many
+0001a5b0: 6c69 6e75 7832 3031 305f 7838 365f 3634  linux2010_x86_64
+0001a5c0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001a5d0: 6861 3235 363a 3938 6334 6433 3665 3939  ha256:98c4d36e99
+0001a5e0: 3731 3465 3535 6366 6261 6165 6536 6464  714e55cfbaaee6dd
+0001a5f0: 3562 6164 6263 3961 3165 6333 3339 6562  5badbc9a1ec339eb
+0001a600: 6663 3362 3166 3532 6532 3933 6165 6536  fc3b1f52e293aee6
+0001a610: 6262 3731 6134 227d 2c0a 2020 2020 7b66  bb71a4"},.    {f
+0001a620: 696c 6520 3d20 2250 7959 414d 4c2d 362e  ile = "PyYAML-6.
+0001a630: 302d 6370 3336 2d63 7033 366d 2d77 696e  0-cp36-cp36m-win
+0001a640: 3332 2e77 686c 222c 2068 6173 6820 3d20  32.whl", hash = 
+0001a650: 2273 6861 3235 363a 3032 3833 6333 3561  "sha256:0283c35a
+0001a660: 3661 3966 6266 3034 3734 3933 6533 6130  6a9fbf047493e3a0
+0001a670: 6365 3864 3739 6566 3530 3330 3835 3263  ce8d79ef5030852c
+0001a680: 3531 6539 6439 3131 6132 3762 6164 6664  51e9d911a27badfd
+0001a690: 6530 3630 3532 3933 227d 2c0a 2020 2020  e0605293"},.    
+0001a6a0: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
+0001a6b0: 362e 302d 6370 3336 2d63 7033 366d 2d77  6.0-cp36-cp36m-w
+0001a6c0: 696e 5f61 6d64 3634 2e77 686c 222c 2068  in_amd64.whl", h
+0001a6d0: 6173 6820 3d20 2273 6861 3235 363a 3037  ash = "sha256:07
+0001a6e0: 3735 3133 3630 3530 3263 6161 6331 6330  751360502caac1c0
+0001a6f0: 3637 6138 3133 3264 3135 3063 6633 6436  67a8132d150cf3d6
+0001a700: 3133 3339 6166 3536 3931 6665 3965 3837  1339af5691fe9e87
+0001a710: 3830 3330 3430 6462 6335 6462 3537 227d  803040dbc5db57"}
+0001a720: 2c0a 2020 2020 7b66 696c 6520 3d20 2250  ,.    {file = "P
+0001a730: 7959 414d 4c2d 362e 302d 6370 3337 2d63  yYAML-6.0-cp37-c
+0001a740: 7033 376d 2d6d 6163 6f73 785f 3130 5f39  p37m-macosx_10_9
+0001a750: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
+0001a760: 7368 203d 2022 7368 6132 3536 3a38 3139  sh = "sha256:819
+0001a770: 6233 3833 3061 3135 3433 6462 3036 6334  b3830a1543db06c4
+0001a780: 6434 6238 3635 6537 3064 6564 3235 6265  d4b865e70ded25be
+0001a790: 3532 6132 6530 3633 3163 6364 3266 3661  52a2e0631ccd2f6a
+0001a7a0: 3437 6132 3832 3266 3266 6437 6322 7d2c  47a2822f2fd7c"},
+0001a7b0: 0a20 2020 207b 6669 6c65 203d 2022 5079  .    {file = "Py
+0001a7c0: 5941 4d4c 2d36 2e30 2d63 7033 372d 6370  YAML-6.0-cp37-cp
+0001a7d0: 3337 6d2d 6d61 6e79 6c69 6e75 785f 325f  37m-manylinux_2_
+0001a7e0: 3137 5f61 6172 6368 3634 2e6d 616e 796c  17_aarch64.manyl
+0001a7f0: 696e 7578 3230 3134 5f61 6172 6368 3634  inux2014_aarch64
+0001a800: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001a810: 6861 3235 363a 3437 3366 3965 6462 3234  ha256:473f9edb24
+0001a820: 3363 6231 3933 3561 6235 6130 3834 6562  3cb1935ab5a084eb
+0001a830: 3233 3864 3834 3266 6238 6634 3034 6564  238d842fb8f404ed
+0001a840: 3231 3933 6139 3135 6431 3738 3462 3561  2193a915d1784b5a
+0001a850: 3662 3566 6330 227d 2c0a 2020 2020 7b66  6b5fc0"},.    {f
+0001a860: 696c 6520 3d20 2250 7959 414d 4c2d 362e  ile = "PyYAML-6.
+0001a870: 302d 6370 3337 2d63 7033 376d 2d6d 616e  0-cp37-cp37m-man
+0001a880: 796c 696e 7578 5f32 5f31 375f 7333 3930  ylinux_2_17_s390
+0001a890: 782e 6d61 6e79 6c69 6e75 7832 3031 345f  x.manylinux2014_
+0001a8a0: 7333 3930 782e 7768 6c22 2c20 6861 7368  s390x.whl", hash
+0001a8b0: 203d 2022 7368 6132 3536 3a30 6365 3832   = "sha256:0ce82
+0001a8c0: 6437 3631 6335 3332 6665 3465 6333 6638  d761c532fe4ec3f8
+0001a8d0: 3766 6334 3536 3838 6264 6433 6134 6331  7fc45688bdd3a4c1
+0001a8e0: 6463 3565 3062 3461 3139 3831 3462 3930  dc5e0b4a19814b90
+0001a8f0: 3039 6132 3962 6165 6664 3422 7d2c 0a20  09a29baefd4"},. 
+0001a900: 2020 207b 6669 6c65 203d 2022 5079 5941     {file = "PyYA
+0001a910: 4d4c 2d36 2e30 2d63 7033 372d 6370 3337  ML-6.0-cp37-cp37
+0001a920: 6d2d 6d61 6e79 6c69 6e75 785f 325f 355f  m-manylinux_2_5_
+0001a930: 7838 365f 3634 2e6d 616e 796c 696e 7578  x86_64.manylinux
+0001a940: 315f 7838 365f 3634 2e6d 616e 796c 696e  1_x86_64.manylin
+0001a950: 7578 5f32 5f31 325f 7838 365f 3634 2e6d  ux_2_12_x86_64.m
+0001a960: 616e 796c 696e 7578 3230 3130 5f78 3836  anylinux2010_x86
+0001a970: 5f36 342e 7768 6c22 2c20 6861 7368 203d  _64.whl", hash =
+0001a980: 2022 7368 6132 3536 3a32 3331 3731 3064   "sha256:231710d
+0001a990: 3537 6164 6664 3830 3965 6635 6433 3431  57adfd809ef5d341
+0001a9a0: 3833 6238 6564 3165 6561 6533 6637 3634  83b8ed1eeae3f764
+0001a9b0: 3539 6331 3866 6234 6130 6233 3733 6164  59c18fb4a0b373ad
+0001a9c0: 3536 6265 6463 6464 3922 7d2c 0a20 2020  56bedcdd9"},.   
+0001a9d0: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
+0001a9e0: 2d36 2e30 2d63 7033 372d 6370 3337 6d2d  -6.0-cp37-cp37m-
+0001a9f0: 7769 6e33 322e 7768 6c22 2c20 6861 7368  win32.whl", hash
+0001aa00: 203d 2022 7368 6132 3536 3a63 3536 3837   = "sha256:c5687
+0001aa10: 6238 6434 3363 6635 3835 3435 6164 6531  b8d43cf58545ade1
+0001aa20: 6665 3365 3035 3566 3730 6561 6337 6135  fe3e055f70eac7a5
+0001aa30: 6131 6130 6266 3432 3832 3433 3038 6438  a1a0bf42824308d8
+0001aa40: 3638 3238 3961 3935 3733 3722 7d2c 0a20  68289a95737"},. 
+0001aa50: 2020 207b 6669 6c65 203d 2022 5079 5941     {file = "PyYA
+0001aa60: 4d4c 2d36 2e30 2d63 7033 372d 6370 3337  ML-6.0-cp37-cp37
+0001aa70: 6d2d 7769 6e5f 616d 6436 342e 7768 6c22  m-win_amd64.whl"
+0001aa80: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001aa90: 3a64 3135 6131 3831 6431 6563 6430 6434  :d15a181d1ecd0d4
+0001aaa0: 3237 3064 6333 3265 6462 3436 6637 6362  270dc32edb46f7cb
+0001aab0: 3737 3333 6337 6335 3038 3835 3732 3738  7733c7c508857278
+0001aac0: 6433 6433 3738 6431 3464 3630 3664 6232  d3d378d14d606db2
+0001aad0: 6422 7d2c 0a20 2020 207b 6669 6c65 203d  d"},.    {file =
+0001aae0: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
+0001aaf0: 382d 6370 3338 2d6d 6163 6f73 785f 3130  8-cp38-macosx_10
+0001ab00: 5f39 5f78 3836 5f36 342e 7768 6c22 2c20  _9_x86_64.whl", 
+0001ab10: 6861 7368 203d 2022 7368 6132 3536 3a30  hash = "sha256:0
+0001ab20: 6234 3632 3466 3337 3964 6162 3234 6433  b4624f379dab24d3
+0001ab30: 3732 3566 6664 6537 3635 3539 6366 6636  725ffde76559cff6
+0001ab40: 3364 3965 6339 3465 3137 3336 6235 3536  3d9ec94e1736b556
+0001ab50: 6461 6364 6665 6265 3561 6236 6434 6222  dacdfebe5ab6d4b"
+0001ab60: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001ab70: 5079 5941 4d4c 2d36 2e30 2d63 7033 382d  PyYAML-6.0-cp38-
+0001ab80: 6370 3338 2d6d 616e 796c 696e 7578 5f32  cp38-manylinux_2
+0001ab90: 5f31 375f 6161 7263 6836 342e 6d61 6e79  _17_aarch64.many
+0001aba0: 6c69 6e75 7832 3031 345f 6161 7263 6836  linux2014_aarch6
+0001abb0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001abc0: 7368 6132 3536 3a32 3133 6336 3063 6435  sha256:213c60cd5
+0001abd0: 3031 3036 3433 3663 6338 3138 6163 6366  0106436cc818accf
+0001abe0: 3562 6161 3161 6261 3631 6330 3138 3966  5baa1aba61c0189f
+0001abf0: 6636 3130 6636 3466 3461 3365 3863 3637  f610f64f4a3e8c67
+0001ac00: 3236 3231 3862 6122 7d2c 0a20 2020 207b  26218ba"},.    {
+0001ac10: 6669 6c65 203d 2022 5079 5941 4d4c 2d36  file = "PyYAML-6
+0001ac20: 2e30 2d63 7033 382d 6370 3338 2d6d 616e  .0-cp38-cp38-man
+0001ac30: 796c 696e 7578 5f32 5f31 375f 7333 3930  ylinux_2_17_s390
+0001ac40: 782e 6d61 6e79 6c69 6e75 7832 3031 345f  x.manylinux2014_
+0001ac50: 7333 3930 782e 7768 6c22 2c20 6861 7368  s390x.whl", hash
+0001ac60: 203d 2022 7368 6132 3536 3a39 6661 3630   = "sha256:9fa60
+0001ac70: 3030 3330 3031 3363 3464 6538 3136 3533  0030013c4de81653
+0001ac80: 3339 6462 3933 6431 3832 6239 3433 3130  39db93d182b94310
+0001ac90: 3736 6562 3938 6562 3430 6565 3036 3837  76eb98eb40ee0687
+0001aca0: 3030 6339 6338 3133 6533 3422 7d2c 0a20  00c9c813e34"},. 
+0001acb0: 2020 207b 6669 6c65 203d 2022 5079 5941     {file = "PyYA
+0001acc0: 4d4c 2d36 2e30 2d63 7033 382d 6370 3338  ML-6.0-cp38-cp38
+0001acd0: 2d6d 616e 796c 696e 7578 5f32 5f35 5f78  -manylinux_2_5_x
+0001ace0: 3836 5f36 342e 6d61 6e79 6c69 6e75 7831  86_64.manylinux1
+0001acf0: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
+0001ad00: 785f 325f 3132 5f78 3836 5f36 342e 6d61  x_2_12_x86_64.ma
+0001ad10: 6e79 6c69 6e75 7832 3031 305f 7838 365f  nylinux2010_x86_
+0001ad20: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
+0001ad30: 2273 6861 3235 363a 3237 3761 3065 6632  "sha256:277a0ef2
+0001ad40: 3938 3163 6134 3035 3831 6134 3730 3933  981ca40581a47093
+0001ad50: 6539 6532 6431 3362 3366 3166 6262 6566  e9e2d13b3f1fbbef
+0001ad60: 6661 6530 3634 6331 6432 3162 6663 6562  fae064c1d21bfceb
+0001ad70: 6132 3033 3032 3837 227d 2c0a 2020 2020  a2030287"},.    
+0001ad80: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
+0001ad90: 362e 302d 6370 3338 2d63 7033 382d 7769  6.0-cp38-cp38-wi
+0001ada0: 6e33 322e 7768 6c22 2c20 6861 7368 203d  n32.whl", hash =
+0001adb0: 2022 7368 6132 3536 3a64 3465 6363 6563   "sha256:d4eccec
+0001adc0: 6639 6164 6636 6662 6363 3638 3631 6133  f9adf6fbcc6861a3
+0001add0: 3830 3135 6332 6136 3466 3338 6239 6439  8015c2a64f38b9d9
+0001ade0: 3438 3338 6163 3138 3130 6139 3032 3361  4838ac1810a9023a
+0001adf0: 3036 3039 6531 6237 3822 7d2c 0a20 2020  0609e1b78"},.   
+0001ae00: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
+0001ae10: 2d36 2e30 2d63 7033 382d 6370 3338 2d77  -6.0-cp38-cp38-w
+0001ae20: 696e 5f61 6d64 3634 2e77 686c 222c 2068  in_amd64.whl", h
+0001ae30: 6173 6820 3d20 2273 6861 3235 363a 3165  ash = "sha256:1e
+0001ae40: 3437 3437 6263 3237 3962 3466 3631 3361  4747bc279b4f613a
+0001ae50: 3039 6562 3634 6262 6132 6261 3630 3264  09eb64bba2ba602d
+0001ae60: 3861 3636 3634 6336 6365 3633 3936 6134  8a6664c6ce6396a4
+0001ae70: 6430 6364 3431 3361 3530 6365 3037 227d  d0cd413a50ce07"}
+0001ae80: 2c0a 2020 2020 7b66 696c 6520 3d20 2250  ,.    {file = "P
+0001ae90: 7959 414d 4c2d 362e 302d 6370 3339 2d63  yYAML-6.0-cp39-c
+0001aea0: 7033 392d 6d61 636f 7378 5f31 305f 395f  p39-macosx_10_9_
+0001aeb0: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
+0001aec0: 6820 3d20 2273 6861 3235 363a 3035 3564  h = "sha256:055d
+0001aed0: 3933 3764 3635 3832 3639 3339 6362 3034  937d65826939cb04
+0001aee0: 3466 6338 6339 6230 3838 3839 6538 6337  4fc8c9b08889e8c7
+0001aef0: 3433 6664 6336 6133 3262 3333 6532 3339  43fdc6a32b33e239
+0001af00: 3066 3636 3031 3365 3434 3962 227d 2c0a  0f66013e449b"},.
+0001af10: 2020 2020 7b66 696c 6520 3d20 2250 7959      {file = "PyY
+0001af20: 414d 4c2d 362e 302d 6370 3339 2d63 7033  AML-6.0-cp39-cp3
+0001af30: 392d 6d61 636f 7378 5f31 315f 305f 6172  9-macosx_11_0_ar
+0001af40: 6d36 342e 7768 6c22 2c20 6861 7368 203d  m64.whl", hash =
+0001af50: 2022 7368 6132 3536 3a65 3631 6365 6161   "sha256:e61ceaa
+0001af60: 6236 6634 3966 6238 6264 6661 6130 6639  b6f49fb8bdfaa0f9
+0001af70: 3263 3462 3537 6263 6662 6561 3534 6330  2c4b57bcfbea54c0
+0001af80: 3932 3737 6231 6234 6637 6163 3337 3662  9277b1b4f7ac376b
+0001af90: 6662 3761 3763 3137 3422 7d2c 0a20 2020  fb7a7c174"},.   
+0001afa0: 207b 6669 6c65 203d 2022 5079 5941 4d4c   {file = "PyYAML
+0001afb0: 2d36 2e30 2d63 7033 392d 6370 3339 2d6d  -6.0-cp39-cp39-m
+0001afc0: 616e 796c 696e 7578 5f32 5f31 375f 6161  anylinux_2_17_aa
+0001afd0: 7263 6836 342e 6d61 6e79 6c69 6e75 7832  rch64.manylinux2
+0001afe0: 3031 345f 6161 7263 6836 342e 7768 6c22  014_aarch64.whl"
+0001aff0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001b000: 3a64 3637 6438 3339 6564 6534 6564 3162  :d67d839ede4ed1b
+0001b010: 3238 6134 6538 3930 3937 3335 6663 3939  28a4e8909735fc99
+0001b020: 3261 3932 3363 6462 3834 6536 3138 3534  2a923cdb84e61854
+0001b030: 3439 3733 6437 6466 6337 3135 3430 3830  4973d7dfc7154080
+0001b040: 3322 7d2c 0a20 2020 207b 6669 6c65 203d  3"},.    {file =
+0001b050: 2022 5079 5941 4d4c 2d36 2e30 2d63 7033   "PyYAML-6.0-cp3
+0001b060: 392d 6370 3339 2d6d 616e 796c 696e 7578  9-cp39-manylinux
+0001b070: 5f32 5f31 375f 7333 3930 782e 6d61 6e79  _2_17_s390x.many
+0001b080: 6c69 6e75 7832 3031 345f 7333 3930 782e  linux2014_s390x.
+0001b090: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+0001b0a0: 6132 3536 3a63 6261 3863 3431 3165 6632  a256:cba8c411ef2
+0001b0b0: 3731 6161 3033 3764 3733 3537 6132 6263  71aa037d7357a2bc
+0001b0c0: 3866 3965 6538 6235 3862 3939 3635 3833  8f9ee8b58b996583
+0001b0d0: 3164 3965 3531 6261 6637 3033 3238 3064  1d9e51baf703280d
+0001b0e0: 6337 3364 3322 7d2c 0a20 2020 207b 6669  c73d3"},.    {fi
+0001b0f0: 6c65 203d 2022 5079 5941 4d4c 2d36 2e30  le = "PyYAML-6.0
+0001b100: 2d63 7033 392d 6370 3339 2d6d 616e 796c  -cp39-cp39-manyl
+0001b110: 696e 7578 5f32 5f35 5f78 3836 5f36 342e  inux_2_5_x86_64.
+0001b120: 6d61 6e79 6c69 6e75 7831 5f78 3836 5f36  manylinux1_x86_6
+0001b130: 342e 6d61 6e79 6c69 6e75 785f 325f 3132  4.manylinux_2_12
+0001b140: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
+0001b150: 7832 3031 305f 7838 365f 3634 2e77 686c  x2010_x86_64.whl
+0001b160: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001b170: 363a 3430 3532 3738 3537 3235 3262 3631  6:40527857252b61
+0001b180: 6561 6364 3164 3961 6635 3030 6333 3333  eacd1d9af500c333
+0001b190: 3762 6138 6465 6238 6663 3239 3839 3430  7ba8deb8fc298940
+0001b1a0: 3239 3134 3836 6334 3635 6338 6234 3665  291486c465c8b46e
+0001b1b0: 6330 227d 2c0a 2020 2020 7b66 696c 6520  c0"},.    {file 
+0001b1c0: 3d20 2250 7959 414d 4c2d 362e 302d 6370  = "PyYAML-6.0-cp
+0001b1d0: 3339 2d63 7033 392d 7769 6e33 322e 7768  39-cp39-win32.wh
+0001b1e0: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+0001b1f0: 3536 3a62 3562 3965 6363 6164 3734 3761  56:b5b9eccad747a
+0001b200: 6162 6161 6666 6263 3630 3634 3830 3036  abaaffbc60648006
+0001b210: 3730 6630 6332 3937 6535 3263 3132 3735  70f0c297e52c1275
+0001b220: 3465 6231 6439 3736 6335 3765 3466 3734  4eb1d976c57e4f74
+0001b230: 6463 6222 7d2c 0a20 2020 207b 6669 6c65  dcb"},.    {file
+0001b240: 203d 2022 5079 5941 4d4c 2d36 2e30 2d63   = "PyYAML-6.0-c
+0001b250: 7033 392d 6370 3339 2d77 696e 5f61 6d64  p39-cp39-win_amd
+0001b260: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
+0001b270: 2273 6861 3235 363a 6233 6432 3637 3834  "sha256:b3d26784
+0001b280: 3262 6631 3235 3836 6261 3663 3733 3466  2bf12586ba6c734f
+0001b290: 3839 6431 6635 6238 3731 6466 3032 3733  89d1f5b871df0273
+0001b2a0: 3135 3739 3138 6230 6363 6566 6132 3964  157918b0ccefa29d
+0001b2b0: 6562 3035 6332 3163 227d 2c0a 2020 2020  eb05c21c"},.    
+0001b2c0: 7b66 696c 6520 3d20 2250 7959 414d 4c2d  {file = "PyYAML-
+0001b2d0: 362e 302e 7461 722e 677a 222c 2068 6173  6.0.tar.gz", has
+0001b2e0: 6820 3d20 2273 6861 3235 363a 3638 6662  h = "sha256:68fb
+0001b2f0: 3531 3963 3134 3330 3666 6563 3937 3230  519c14306fec9720
+0001b300: 6132 6135 6234 3562 6339 6630 6338 6431  a2a5b45bc9f0c8d1
+0001b310: 6239 6337 3261 6466 3435 6333 3762 6165  b9c72adf45c37bae
+0001b320: 6466 6364 3934 3963 3335 6132 227d 2c0a  dfcd949c35a2"},.
+0001b330: 5d0a 0a5b 5b70 6163 6b61 6765 5d5d 0a6e  ]..[[package]].n
+0001b340: 616d 6520 3d20 2270 7979 616d 6c2d 656e  ame = "pyyaml-en
+0001b350: 762d 7461 6722 0a76 6572 7369 6f6e 203d  v-tag".version =
+0001b360: 2022 302e 3122 0a64 6573 6372 6970 7469   "0.1".descripti
+0001b370: 6f6e 203d 2022 4120 6375 7374 6f6d 2059  on = "A custom Y
+0001b380: 414d 4c20 7461 6720 666f 7220 7265 6665  AML tag for refe
+0001b390: 7265 6e63 696e 6720 656e 7669 726f 6e6d  rencing environm
+0001b3a0: 656e 7420 7661 7269 6162 6c65 7320 696e  ent variables in
+0001b3b0: 2059 414d 4c20 6669 6c65 732e 2022 0a6f   YAML files. ".o
+0001b3c0: 7074 696f 6e61 6c20 3d20 6661 6c73 650a  ptional = false.
+0001b3d0: 7079 7468 6f6e 2d76 6572 7369 6f6e 7320  python-versions 
+0001b3e0: 3d20 223e 3d33 2e36 220a 6669 6c65 7320  = ">=3.6".files 
+0001b3f0: 3d20 5b0a 2020 2020 7b66 696c 6520 3d20  = [.    {file = 
+0001b400: 2270 7979 616d 6c5f 656e 765f 7461 672d  "pyyaml_env_tag-
+0001b410: 302e 312d 7079 332d 6e6f 6e65 2d61 6e79  0.1-py3-none-any
+0001b420: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001b430: 6861 3235 363a 6166 3331 3130 3664 6563  ha256:af31106dec
+0001b440: 3861 3464 3638 6336 3032 3037 6331 3838  8a4d68c60207c188
+0001b450: 3630 3331 6362 6638 3339 6236 3861 6137  6031cbf839b68aa7
+0001b460: 6162 6363 6462 3139 3836 3832 3030 3533  abccdb1986820053
+0001b470: 3263 3230 3639 227d 2c0a 2020 2020 7b66  2c2069"},.    {f
+0001b480: 696c 6520 3d20 2270 7979 616d 6c5f 656e  ile = "pyyaml_en
+0001b490: 765f 7461 672d 302e 312e 7461 722e 677a  v_tag-0.1.tar.gz
+0001b4a0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001b4b0: 363a 3730 3039 3236 3735 6264 6131 3466  6:70092675bda14f
+0001b4c0: 6465 6333 3362 3331 6261 3737 6537 3534  dec33b31ba77e754
+0001b4d0: 3364 6539 6464 6338 3866 3265 3562 3939  3de9ddc88f2e5b99
+0001b4e0: 3136 3033 3936 3537 3264 3131 3532 3562  160396572d11525b
+0001b4f0: 6462 227d 2c0a 5d0a 0a5b 7061 636b 6167  db"},.]..[packag
+0001b500: 652e 6465 7065 6e64 656e 6369 6573 5d0a  e.dependencies].
+0001b510: 7079 7961 6d6c 203d 2022 2a22 0a0a 5b5b  pyyaml = "*"..[[
+0001b520: 7061 636b 6167 655d 5d0a 6e61 6d65 203d  package]].name =
+0001b530: 2022 7079 7a6d 7122 0a76 6572 7369 6f6e   "pyzmq".version
+0001b540: 203d 2022 3235 2e30 2e32 220a 6465 7363   = "25.0.2".desc
+0001b550: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
+0001b560: 6e20 6269 6e64 696e 6773 2066 6f72 2030  n bindings for 0
+0001b570: 4d51 220a 6f70 7469 6f6e 616c 203d 2066  MQ".optional = f
+0001b580: 616c 7365 0a70 7974 686f 6e2d 7665 7273  alse.python-vers
+0001b590: 696f 6e73 203d 2022 3e3d 332e 3622 0a66  ions = ">=3.6".f
+0001b5a0: 696c 6573 203d 205b 0a20 2020 207b 6669  iles = [.    {fi
+0001b5b0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
+0001b5c0: 2e32 2d63 7033 3130 2d63 7033 3130 2d6d  .2-cp310-cp310-m
+0001b5d0: 6163 6f73 785f 3130 5f31 355f 756e 6976  acosx_10_15_univ
+0001b5e0: 6572 7361 6c32 2e77 686c 222c 2068 6173  ersal2.whl", has
+0001b5f0: 6820 3d20 2273 6861 3235 363a 6163 3137  h = "sha256:ac17
+0001b600: 3865 3636 3663 3039 3763 3864 3364 6562  8e666c097c8d3deb
+0001b610: 3530 3937 6235 3863 6431 3331 3630 3932  5097b58cd1316092
+0001b620: 6663 3433 6538 6566 3562 3566 6462 3235  fc43e8ef5b5fdb25
+0001b630: 3962 3531 6461 3765 3733 3135 227d 2c0a  9b51da7e7315"},.
+0001b640: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001b650: 6d71 2d32 352e 302e 322d 6370 3331 302d  mq-25.0.2-cp310-
+0001b660: 6370 3331 302d 6d61 636f 7378 5f31 305f  cp310-macosx_10_
+0001b670: 395f 7838 365f 3634 2e77 686c 222c 2068  9_x86_64.whl", h
+0001b680: 6173 6820 3d20 2273 6861 3235 363a 3635  ash = "sha256:65
+0001b690: 3965 3632 6531 6362 6230 3633 3135 3163  9e62e1cbb063151c
+0001b6a0: 3532 6635 6230 3161 3338 6531 6466 3662  52f5b01a38e1df6b
+0001b6b0: 3534 6665 6363 6661 3365 3235 3039 6434  54feccfa3e2509d4
+0001b6c0: 3463 3335 6361 3664 3739 3632 6565 227d  4c35ca6d7962ee"}
+0001b6d0: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
+0001b6e0: 797a 6d71 2d32 352e 302e 322d 6370 3331  yzmq-25.0.2-cp31
+0001b6f0: 302d 6370 3331 302d 6d61 6e79 6c69 6e75  0-cp310-manylinu
+0001b700: 785f 325f 3137 5f61 6172 6368 3634 2e6d  x_2_17_aarch64.m
+0001b710: 616e 796c 696e 7578 3230 3134 5f61 6172  anylinux2014_aar
+0001b720: 6368 3634 2e77 686c 222c 2068 6173 6820  ch64.whl", hash 
+0001b730: 3d20 2273 6861 3235 363a 3832 3830 6164  = "sha256:8280ad
+0001b740: 6138 3930 3130 3733 3561 3132 6239 3638  a89010735a12b968
+0001b750: 6563 3365 6139 6134 3638 6163 3265 3034  ec3ea9a468ac2e04
+0001b760: 6664 6463 6331 6365 6465 3539 6362 3766  fddcc1cede59cb7f
+0001b770: 3531 3738 3738 3362 3963 227d 2c0a 2020  5178783b9c"},.  
+0001b780: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
+0001b790: 2d32 352e 302e 322d 6370 3331 302d 6370  -25.0.2-cp310-cp
+0001b7a0: 3331 302d 6d61 6e79 6c69 6e75 785f 325f  310-manylinux_2_
+0001b7b0: 3137 5f69 3638 362e 6d61 6e79 6c69 6e75  17_i686.manylinu
+0001b7c0: 7832 3031 345f 6936 3836 2e77 686c 222c  x2014_i686.whl",
+0001b7d0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
+0001b7e0: 6139 6235 6565 6235 3237 3861 3861 3633  a9b5eeb5278a8a63
+0001b7f0: 3662 6230 6162 6464 3966 6635 3037 3662  6bb0abdd9ff5076b
+0001b800: 6362 6238 3336 6364 3233 3032 3536 3564  cbb836cd2302565d
+0001b810: 6635 3366 6631 6661 3764 3130 3664 3534  f53ff1fa7d106d54
+0001b820: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
+0001b830: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
+0001b840: 3331 302d 6370 3331 302d 6d61 6e79 6c69  310-cp310-manyli
+0001b850: 6e75 785f 325f 3137 5f78 3836 5f36 342e  nux_2_17_x86_64.
+0001b860: 6d61 6e79 6c69 6e75 7832 3031 345f 7838  manylinux2014_x8
+0001b870: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
+0001b880: 3d20 2273 6861 3235 363a 3961 3265 3566  = "sha256:9a2e5f
+0001b890: 6534 3264 6665 3662 3733 6361 3132 3062  e42dfe6b73ca120b
+0001b8a0: 3937 6163 3966 3334 6266 6138 3431 3466  97ac9f34bfa8414f
+0001b8b0: 6562 3135 6530 3065 3337 3431 3564 6264  eb15e00e37415dbd
+0001b8c0: 3531 6366 3232 3765 6636 227d 2c0a 2020  51cf227ef6"},.  
+0001b8d0: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
+0001b8e0: 2d32 352e 302e 322d 6370 3331 302d 6370  -25.0.2-cp310-cp
+0001b8f0: 3331 302d 6d61 6e79 6c69 6e75 785f 325f  310-manylinux_2_
+0001b900: 3238 5f78 3836 5f36 342e 7768 6c22 2c20  28_x86_64.whl", 
+0001b910: 6861 7368 203d 2022 7368 6132 3536 3a38  hash = "sha256:8
+0001b920: 3237 6266 3630 6537 3439 6537 3861 6362  27bf60e749e78acb
+0001b930: 3430 3861 3663 3561 6636 3638 3865 6662  408a6c5af6688efb
+0001b940: 6339 3939 3365 3434 6563 6337 3932 6230  c9993e44ecc792b0
+0001b950: 3336 6563 3266 3462 3461 6366 3438 3522  36ec2f4b4acf485"
+0001b960: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001b970: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
+0001b980: 3130 2d63 7033 3130 2d6d 7573 6c6c 696e  10-cp310-musllin
+0001b990: 7578 5f31 5f31 5f61 6172 6368 3634 2e77  ux_1_1_aarch64.w
+0001b9a0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+0001b9b0: 3235 363a 3762 3530 3461 6534 3364 3337  256:7b504ae43d37
+0001b9c0: 6532 3832 3330 3164 6135 3836 3532 3965  e282301da586529e
+0001b9d0: 3264 6564 3862 3336 6434 6565 3263 6435  2ded8b36d4ee2cd5
+0001b9e0: 6536 6462 3433 3836 3732 3464 6465 6161  e6db4386724ddeaa
+0001b9f0: 3662 6263 227d 2c0a 2020 2020 7b66 696c  6bbc"},.    {fil
+0001ba00: 6520 3d20 2270 797a 6d71 2d32 352e 302e  e = "pyzmq-25.0.
+0001ba10: 322d 6370 3331 302d 6370 3331 302d 6d75  2-cp310-cp310-mu
+0001ba20: 736c 6c69 6e75 785f 315f 315f 6936 3836  sllinux_1_1_i686
+0001ba30: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001ba40: 6861 3235 363a 6362 3166 3639 6130 6132  ha256:cb1f69a0a2
+0001ba50: 6132 6231 6161 6538 3431 3239 3739 6464  a2b1aae8412979dd
+0001ba60: 3632 3933 6363 3662 6364 6464 3434 3339  6293cc6bcddd4439
+0001ba70: 6266 3037 6534 3735 3864 3836 3464 6462  bf07e4758d864ddb
+0001ba80: 3131 3233 3534 227d 2c0a 2020 2020 7b66  112354"},.    {f
+0001ba90: 696c 6520 3d20 2270 797a 6d71 2d32 352e  ile = "pyzmq-25.
+0001baa0: 302e 322d 6370 3331 302d 6370 3331 302d  0.2-cp310-cp310-
+0001bab0: 6d75 736c 6c69 6e75 785f 315f 315f 7838  musllinux_1_1_x8
+0001bac0: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
+0001bad0: 3d20 2273 6861 3235 363a 3262 3963 3963  = "sha256:2b9c9c
+0001bae0: 6339 3635 6364 6632 3833 3831 6533 3664  c965cdf28381e36d
+0001baf0: 6135 3235 6463 6238 3966 6331 3537 3164  a525dcb89fc1571d
+0001bb00: 3963 3534 3830 3066 6463 6437 3365 3366  9c54800fdcd73e3f
+0001bb10: 3733 6132 6663 3239 6264 227d 2c0a 2020  73a2fc29bd"},.  
+0001bb20: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
+0001bb30: 2d32 352e 302e 322d 6370 3331 302d 6370  -25.0.2-cp310-cp
+0001bb40: 3331 302d 7769 6e33 322e 7768 6c22 2c20  310-win32.whl", 
+0001bb50: 6861 7368 203d 2022 7368 6132 3536 3a32  hash = "sha256:2
+0001bb60: 3461 6262 6664 6262 3735 6163 3530 3339  4abbfdbb75ac5039
+0001bb70: 3230 3565 3732 6436 6337 3566 3130 6663  205e72d6c75f10fc
+0001bb80: 3339 6439 3235 6632 6466 3866 6632 3165  39d925f2df8ff21e
+0001bb90: 6263 3734 3137 3934 3838 6562 6663 6122  bc74179488ebfca"
+0001bba0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001bbb0: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
+0001bbc0: 3130 2d63 7033 3130 2d77 696e 5f61 6d64  10-cp310-win_amd
+0001bbd0: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
+0001bbe0: 2273 6861 3235 363a 3661 3832 3161 3530  "sha256:6a821a50
+0001bbf0: 3638 3232 6661 6335 3564 3264 6632 3038  6822fac55d2df208
+0001bc00: 3561 3532 3533 3066 3638 6162 3135 6365  5a52530f68ab15ce
+0001bc10: 6564 3132 6436 3335 3339 6164 6333 3262  ed12d63539adc32b
+0001bc20: 6434 3431 3066 3665 227d 2c0a 2020 2020  d4410f6e"},.    
+0001bc30: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
+0001bc40: 352e 302e 322d 6370 3331 312d 6370 3331  5.0.2-cp311-cp31
+0001bc50: 312d 6d61 636f 7378 5f31 305f 3135 5f75  1-macosx_10_15_u
+0001bc60: 6e69 7665 7273 616c 322e 7768 6c22 2c20  niversal2.whl", 
+0001bc70: 6861 7368 203d 2022 7368 6132 3536 3a39  hash = "sha256:9
+0001bc80: 6166 3062 6230 3237 3765 3932 6634 3161  af0bb0277e92f41a
+0001bc90: 6633 3565 3939 3163 3234 3263 3963 3731  f35e991c242c9c71
+0001bca0: 3932 3031 3639 6436 6161 3533 6164 6537  920169d6aa53ade7
+0001bcb0: 6534 3434 6633 3338 6634 6338 3132 3822  e444f338f4c8128"
+0001bcc0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001bcd0: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
+0001bce0: 3131 2d63 7033 3131 2d6d 6163 6f73 785f  11-cp311-macosx_
+0001bcf0: 3130 5f39 5f78 3836 5f36 342e 7768 6c22  10_9_x86_64.whl"
+0001bd00: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001bd10: 3a35 3461 3936 6366 3737 3638 3461 3361  :54a96cf77684a3a
+0001bd20: 3533 3762 3736 6163 6661 3732 3337 6231  537b76acfa7237b1
+0001bd30: 6537 3961 3866 3864 3134 6537 6630 3065  e79a8f8d14e7f00e
+0001bd40: 3031 3731 6139 3462 3334 3663 3532 3933  0171a94b346c5293
+0001bd50: 6522 7d2c 0a20 2020 207b 6669 6c65 203d  e"},.    {file =
+0001bd60: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
+0001bd70: 7033 3131 2d63 7033 3131 2d6d 616e 796c  p311-cp311-manyl
+0001bd80: 696e 7578 5f32 5f31 375f 6161 7263 6836  inux_2_17_aarch6
+0001bd90: 342e 6d61 6e79 6c69 6e75 7832 3031 345f  4.manylinux2014_
+0001bda0: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
+0001bdb0: 7368 203d 2022 7368 6132 3536 3a38 3836  sh = "sha256:886
+0001bdc0: 3439 6231 3965 6465 3163 6162 3033 6239  49b19ede1cab03b9
+0001bdd0: 3662 3636 6333 3634 6362 6266 3137 6339  6b66c364cbbf17c9
+0001bde0: 3533 3631 3563 6462 6338 3434 6637 6636  53615cdbc844f7f6
+0001bdf0: 6535 6631 3463 3565 3532 3631 6322 7d2c  e5f14c5e5261c"},
+0001be00: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001be10: 7a6d 712d 3235 2e30 2e32 2d63 7033 3131  zmq-25.0.2-cp311
+0001be20: 2d63 7033 3131 2d6d 616e 796c 696e 7578  -cp311-manylinux
+0001be30: 5f32 5f31 375f 6936 3836 2e6d 616e 796c  _2_17_i686.manyl
+0001be40: 696e 7578 3230 3134 5f69 3638 362e 7768  inux2014_i686.wh
+0001be50: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+0001be60: 3536 3a37 3135 6366 6637 3634 3461 3830  56:715cff7644a80
+0001be70: 6137 3739 3539 3533 6331 3162 3036 3761  a7795953c11b067a
+0001be80: 3735 6631 3665 6239 6663 3639 3561 3561  75f16eb9fc695a5a
+0001be90: 3533 3331 3638 3931 6562 6565 3766 3363  53316891ebee7f3c
+0001bea0: 3964 3522 7d2c 0a20 2020 207b 6669 6c65  9d5"},.    {file
+0001beb0: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
+0001bec0: 2d63 7033 3131 2d63 7033 3131 2d6d 616e  -cp311-cp311-man
+0001bed0: 796c 696e 7578 5f32 5f31 375f 7838 365f  ylinux_2_17_x86_
+0001bee0: 3634 2e6d 616e 796c 696e 7578 3230 3134  64.manylinux2014
+0001bef0: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
+0001bf00: 7368 203d 2022 7368 6132 3536 3a33 3132  sh = "sha256:312
+0001bf10: 6233 6630 6630 3636 6234 6631 6431 3733  b3f0f066b4f1d173
+0001bf20: 3833 6161 6535 3039 6261 6366 3833 3363  83aae509bacf833c
+0001bf30: 6361 6635 3931 3138 3461 3166 3363 3761  caf591184a1f3c7a
+0001bf40: 3136 3631 6330 3835 3036 3361 6522 7d2c  1661c085063ae"},
+0001bf50: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001bf60: 7a6d 712d 3235 2e30 2e32 2d63 7033 3131  zmq-25.0.2-cp311
+0001bf70: 2d63 7033 3131 2d6d 616e 796c 696e 7578  -cp311-manylinux
+0001bf80: 5f32 5f32 385f 7838 365f 3634 2e77 686c  _2_28_x86_64.whl
+0001bf90: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001bfa0: 363a 6434 3838 6335 6338 3633 3066 3765  6:d488c5c8630f7e
+0001bfb0: 3738 3265 3830 3038 3639 6638 3237 3434  782e800869f82744
+0001bfc0: 6333 6163 6134 6163 6136 3263 3633 3233  c3aca4aca62c6323
+0001bfd0: 3265 3564 3863 3439 3064 3364 3636 3935  2e5d8c490d3d6695
+0001bfe0: 3661 227d 2c0a 2020 2020 7b66 696c 6520  6a"},.    {file 
+0001bff0: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001c000: 6370 3331 312d 6370 3331 312d 6d75 736c  cp311-cp311-musl
+0001c010: 6c69 6e75 785f 315f 315f 6161 7263 6836  linux_1_1_aarch6
+0001c020: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001c030: 7368 6132 3536 3a33 3864 3966 3738 6436  sha256:38d9f78d6
+0001c040: 3962 6364 6565 6330 6331 3165 3066 6562  9bcdeec0c11e0feb
+0001c050: 3362 6337 3066 3336 6639 6238 6334 3466  3bc70f36f9b8c44f
+0001c060: 6330 3665 3564 3036 6439 3164 6330 6132  c06e5d06d91dc0a2
+0001c070: 3162 3435 3363 3722 7d2c 0a20 2020 207b  1b453c7"},.    {
+0001c080: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
+0001c090: 2e30 2e32 2d63 7033 3131 2d63 7033 3131  .0.2-cp311-cp311
+0001c0a0: 2d6d 7573 6c6c 696e 7578 5f31 5f31 5f69  -musllinux_1_1_i
+0001c0b0: 3638 362e 7768 6c22 2c20 6861 7368 203d  686.whl", hash =
+0001c0c0: 2022 7368 6132 3536 3a33 3035 3961 3661   "sha256:3059a6a
+0001c0d0: 3533 3463 3931 3065 3164 3564 3036 3864  534c910e1d5d068d
+0001c0e0: 6634 3266 3630 6434 3334 6637 3965 3663  f42f60d434f79e6c
+0001c0f0: 6336 3238 3561 6134 3639 6233 3834 6661  c6285aa469b384fa
+0001c100: 3932 3166 3738 6366 3822 7d2c 0a20 2020  921f78cf8"},.   
+0001c110: 207b 6669 6c65 203d 2022 7079 7a6d 712d   {file = "pyzmq-
+0001c120: 3235 2e30 2e32 2d63 7033 3131 2d63 7033  25.0.2-cp311-cp3
+0001c130: 3131 2d6d 7573 6c6c 696e 7578 5f31 5f31  11-musllinux_1_1
+0001c140: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
+0001c150: 7368 203d 2022 7368 6132 3536 3a36 3532  sh = "sha256:652
+0001c160: 3664 3039 3762 3735 3139 3266 3232 3863  6d097b75192f228c
+0001c170: 3039 6434 3834 3230 3835 3464 3533 6466  09d48420854d53df
+0001c180: 6263 3761 6262 6234 3162 3065 3236 6633  bc7abbb41b0e26f3
+0001c190: 3633 6363 6232 3666 6263 3137 3722 7d2c  63ccb26fbc177"},
+0001c1a0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001c1b0: 7a6d 712d 3235 2e30 2e32 2d63 7033 3131  zmq-25.0.2-cp311
+0001c1c0: 2d63 7033 3131 2d77 696e 3332 2e77 686c  -cp311-win32.whl
+0001c1d0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001c1e0: 363a 3563 3566 6262 3232 3965 3430 6138  6:5c5fbb229e40a8
+0001c1f0: 3961 3266 6537 3364 3063 3131 3831 3931  9a2fe73d0c118191
+0001c200: 3666 3331 6533 3066 3235 3363 6232 6436  6f31e30f253cb2d6
+0001c210: 6439 3162 6561 3739 3237 6332 6531 3834  d91bea7927c2e184
+0001c220: 3133 227d 2c0a 2020 2020 7b66 696c 6520  13"},.    {file 
+0001c230: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001c240: 6370 3331 312d 6370 3331 312d 7769 6e5f  cp311-cp311-win_
+0001c250: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+0001c260: 203d 2022 7368 6132 3536 3a65 6431 3565   = "sha256:ed15e
+0001c270: 3361 3263 3363 3233 3938 6536 6165 3563  3a2c3c2398e6ae5c
+0001c280: 6538 3664 3661 3331 6234 3532 6466 6436  e86d6a31b452dfd6
+0001c290: 6164 3463 6435 6433 3132 3539 3662 3330  ad4cd5d312596b30
+0001c2a0: 3932 3963 3462 3665 3138 3222 7d2c 0a20  929c4b6e182"},. 
+0001c2b0: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
+0001c2c0: 712d 3235 2e30 2e32 2d63 7033 362d 6370  q-25.0.2-cp36-cp
+0001c2d0: 3336 6d2d 6d61 636f 7378 5f31 305f 395f  36m-macosx_10_9_
+0001c2e0: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
+0001c2f0: 6820 3d20 2273 6861 3235 363a 3033 3266  h = "sha256:032f
+0001c300: 3563 3834 3833 6338 3562 6639 6339 6361  5c8483c85bf9c9ca
+0001c310: 3035 3933 6131 3163 3763 3734 3964 3733  0593a11c7c749d73
+0001c320: 3463 6536 3864 3433 3565 3338 6333 6637  4ce68d435e38c3f7
+0001c330: 3265 3735 3962 3938 6233 6339 227d 2c0a  2e759b98b3c9"},.
+0001c340: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001c350: 6d71 2d32 352e 302e 322d 6370 3336 2d63  mq-25.0.2-cp36-c
+0001c360: 7033 366d 2d6d 616e 796c 696e 7578 5f32  p36m-manylinux_2
+0001c370: 5f31 375f 6161 7263 6836 342e 6d61 6e79  _17_aarch64.many
+0001c380: 6c69 6e75 7832 3031 345f 6161 7263 6836  linux2014_aarch6
+0001c390: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001c3a0: 7368 6132 3536 3a33 3734 6235 3535 3136  sha256:374b55516
+0001c3b0: 3339 3362 6664 3464 3761 3764 6161 3663  393bfd4d7a7daa6c
+0001c3c0: 3362 3336 6436 6464 3661 3331 6666 3964  3b36d6dd6a31ff9d
+0001c3d0: 3261 6461 6430 3833 3863 6436 6132 3033  2adad0838cd6a203
+0001c3e0: 3132 3565 3731 3422 7d2c 0a20 2020 207b  125e714"},.    {
+0001c3f0: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
+0001c400: 2e30 2e32 2d63 7033 362d 6370 3336 6d2d  .0.2-cp36-cp36m-
+0001c410: 6d61 6e79 6c69 6e75 785f 325f 355f 6936  manylinux_2_5_i6
+0001c420: 3836 2e6d 616e 796c 696e 7578 315f 6936  86.manylinux1_i6
+0001c430: 3836 2e77 686c 222c 2068 6173 6820 3d20  86.whl", hash = 
+0001c440: 2273 6861 3235 363a 3038 6266 6363 3231  "sha256:08bfcc21
+0001c450: 6235 3939 3761 3962 6534 6665 6661 3430  b5997a9be4fefa40
+0001c460: 3533 3431 3332 3064 3865 3766 3139 6234  5341320d8e7f19b4
+0001c470: 6436 3834 6662 3963 3035 3830 3235 3563  d684fb9c0580255c
+0001c480: 3562 6436 6436 3935 227d 2c0a 2020 2020  5bd6d695"},.    
+0001c490: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
+0001c4a0: 352e 302e 322d 6370 3336 2d63 7033 366d  5.0.2-cp36-cp36m
+0001c4b0: 2d6d 616e 796c 696e 7578 5f32 5f35 5f78  -manylinux_2_5_x
+0001c4c0: 3836 5f36 342e 6d61 6e79 6c69 6e75 7831  86_64.manylinux1
+0001c4d0: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
+0001c4e0: 7368 203d 2022 7368 6132 3536 3a31 6138  sh = "sha256:1a8
+0001c4f0: 3433 6432 3661 3864 6131 6237 3532 6337  43d26a8da1b752c7
+0001c500: 3462 6330 3139 6337 6232 3065 3637 3931  4bc019c7b20e6791
+0001c510: 6565 3831 3363 6436 3837 3734 3439 6536  ee813cd6877449e6
+0001c520: 6131 3431 3535 3839 6432 3266 6622 7d2c  a1415589d22ff"},
+0001c530: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001c540: 7a6d 712d 3235 2e30 2e32 2d63 7033 362d  zmq-25.0.2-cp36-
+0001c550: 6370 3336 6d2d 6d75 736c 6c69 6e75 785f  cp36m-musllinux_
+0001c560: 315f 315f 6161 7263 6836 342e 7768 6c22  1_1_aarch64.whl"
+0001c570: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001c580: 3a62 3438 3631 3661 3039 6437 6466 3964  :b48616a09d7df9d
+0001c590: 6261 6532 6634 3561 3032 3536 6565 6537  bae2f45a0256eee7
+0001c5a0: 6237 3934 6239 3033 6464 6336 6438 3635  b794b903ddc6d865
+0001c5b0: 3761 3939 3438 3636 3962 3334 3566 3232  7a9948669b345f22
+0001c5c0: 3022 7d2c 0a20 2020 207b 6669 6c65 203d  0"},.    {file =
+0001c5d0: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
+0001c5e0: 7033 362d 6370 3336 6d2d 6d75 736c 6c69  p36-cp36m-muslli
+0001c5f0: 6e75 785f 315f 315f 6936 3836 2e77 686c  nux_1_1_i686.whl
+0001c600: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001c610: 363a 6434 3432 3762 3461 3133 3665 3362  6:d4427b4a136e3b
+0001c620: 3766 3835 3531 3663 3736 6464 3265 3037  7f85516c76dd2e07
+0001c630: 3536 6332 3265 6563 3430 3236 6166 6237  56c22eec4026afb7
+0001c640: 3663 6131 3339 3731 3532 6230 6361 3831  6ca1397152b0ca81
+0001c650: 3435 227d 2c0a 2020 2020 7b66 696c 6520  45"},.    {file 
+0001c660: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001c670: 6370 3336 2d63 7033 366d 2d6d 7573 6c6c  cp36-cp36m-musll
+0001c680: 696e 7578 5f31 5f31 5f78 3836 5f36 342e  inux_1_1_x86_64.
+0001c690: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+0001c6a0: 6132 3536 3a32 3662 3033 3538 6538 3933  a256:26b0358e893
+0001c6b0: 3339 3930 3530 3266 3435 3133 6339 3931  3990502f4513c991
+0001c6c0: 6339 3933 3562 3663 3036 6166 3031 3738  c9935b6c06af0178
+0001c6d0: 3761 3336 6431 3333 6237 6333 3962 3164  7a36d133b7c39b1d
+0001c6e0: 6633 3766 6122 7d2c 0a20 2020 207b 6669  f37fa"},.    {fi
+0001c6f0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
+0001c700: 2e32 2d63 7033 362d 6370 3336 6d2d 7769  .2-cp36-cp36m-wi
+0001c710: 6e33 322e 7768 6c22 2c20 6861 7368 203d  n32.whl", hash =
+0001c720: 2022 7368 6132 3536 3a63 3866 6564 6333   "sha256:c8fedc3
+0001c730: 6363 6436 3263 3662 3737 6466 6536 6634  ccd62c6b77dfe6f4
+0001c740: 3338 3032 3035 3761 3830 3361 3431 3165  3802057a803a411e
+0001c750: 6539 3666 3134 6539 3436 6634 6137 3665  e96f14e946f4a76e
+0001c760: 6334 6564 3065 3131 3722 7d2c 0a20 2020  c4ed0e117"},.   
+0001c770: 207b 6669 6c65 203d 2022 7079 7a6d 712d   {file = "pyzmq-
+0001c780: 3235 2e30 2e32 2d63 7033 362d 6370 3336  25.0.2-cp36-cp36
+0001c790: 6d2d 7769 6e5f 616d 6436 342e 7768 6c22  m-win_amd64.whl"
+0001c7a0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001c7b0: 3a32 6461 3638 3133 6237 3939 3562 3662  :2da6813b7995b6b
+0001c7c0: 3164 3133 3037 3332 3963 3733 6433 6533  1d1307329c73d3e3
+0001c7d0: 6265 3266 6432 6437 3865 3139 6163 6663  be2fd2d78e19acfc
+0001c7e0: 3465 6666 3265 3237 3236 3237 3332 3338  4eff2e2726273238
+0001c7f0: 3822 7d2c 0a20 2020 207b 6669 6c65 203d  8"},.    {file =
+0001c800: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
+0001c810: 7033 372d 6370 3337 6d2d 6d61 636f 7378  p37-cp37m-macosx
+0001c820: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
+0001c830: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001c840: 363a 6133 3539 3630 6338 6232 6636 3365  6:a35960c8b2f63e
+0001c850: 3465 6636 3766 6436 3733 3138 3531 3033  4ef67fd673185103
+0001c860: 3064 6636 3865 3462 3631 3761 3637 3135  0df68e4b617a6715
+0001c870: 6464 3131 6234 6231 3033 3132 6431 3966  dd11b4b10312d19f
+0001c880: 6566 227d 2c0a 2020 2020 7b66 696c 6520  ef"},.    {file 
+0001c890: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001c8a0: 6370 3337 2d63 7033 376d 2d6d 616e 796c  cp37-cp37m-manyl
+0001c8b0: 696e 7578 5f32 5f31 375f 6161 7263 6836  inux_2_17_aarch6
+0001c8c0: 342e 6d61 6e79 6c69 6e75 7832 3031 345f  4.manylinux2014_
+0001c8d0: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
+0001c8e0: 7368 203d 2022 7368 6132 3536 3a65 6566  sh = "sha256:eef
+0001c8f0: 3261 3062 3838 3061 6234 3061 6361 3561  2a0b880ab40aca5a
+0001c900: 3837 3839 3333 3337 3663 6236 6331 6563  878933376cb6c1ec
+0001c910: 3438 3366 6261 3732 6637 6633 3465 3031  483fba72f7f34e01
+0001c920: 3563 3066 3637 3563 3930 6232 3022 7d2c  5c0f675c90b20"},
+0001c930: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001c940: 7a6d 712d 3235 2e30 2e32 2d63 7033 372d  zmq-25.0.2-cp37-
+0001c950: 6370 3337 6d2d 6d61 6e79 6c69 6e75 785f  cp37m-manylinux_
+0001c960: 325f 355f 6936 3836 2e6d 616e 796c 696e  2_5_i686.manylin
+0001c970: 7578 315f 6936 3836 2e77 686c 222c 2068  ux1_i686.whl", h
+0001c980: 6173 6820 3d20 2273 6861 3235 363a 3835  ash = "sha256:85
+0001c990: 3736 3237 3132 6237 3463 3762 6431 3865  762712b74c7bd18e
+0001c9a0: 3334 3063 3336 3339 6431 6266 3266 3233  340c3639d1bf2f23
+0001c9b0: 3733 3561 3939 3864 3633 6634 3662 6236  735a998d63f46bb6
+0001c9c0: 3538 3464 3930 3462 3565 3430 3164 227d  584d904b5e401d"}
+0001c9d0: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
+0001c9e0: 797a 6d71 2d32 352e 302e 322d 6370 3337  yzmq-25.0.2-cp37
+0001c9f0: 2d63 7033 376d 2d6d 616e 796c 696e 7578  -cp37m-manylinux
+0001ca00: 5f32 5f35 5f78 3836 5f36 342e 6d61 6e79  _2_5_x86_64.many
+0001ca10: 6c69 6e75 7831 5f78 3836 5f36 342e 7768  linux1_x86_64.wh
+0001ca20: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+0001ca30: 3536 3a36 3438 3132 6632 3964 3665 6565  56:64812f29d6eee
+0001ca40: 3536 3565 3132 3963 6131 3462 3063 3738  565e129ca14b0c78
+0001ca50: 3537 3434 6266 6666 3637 3961 3437 3237  5744bfff679a4727
+0001ca60: 3133 3734 3834 3130 3162 3334 3630 3264  137484101b34602d
+0001ca70: 3161 3722 7d2c 0a20 2020 207b 6669 6c65  1a7"},.    {file
+0001ca80: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
+0001ca90: 2d63 7033 372d 6370 3337 6d2d 6d75 736c  -cp37-cp37m-musl
+0001caa0: 6c69 6e75 785f 315f 315f 6161 7263 6836  linux_1_1_aarch6
+0001cab0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001cac0: 7368 6132 3536 3a35 3130 6438 6535 3562  sha256:510d8e55b
+0001cad0: 3361 3763 6431 3366 3864 3365 3931 3231  3a7cd13f8d3e9121
+0001cae0: 6564 6630 6138 3733 3062 3837 6439 3235  edf0a8730b87d925
+0001caf0: 6432 3532 3938 6261 6365 3239 6137 6537  d25298bace29a7e7
+0001cb00: 6263 3832 3831 3022 7d2c 0a20 2020 207b  bc82810"},.    {
+0001cb10: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
+0001cb20: 2e30 2e32 2d63 7033 372d 6370 3337 6d2d  .0.2-cp37-cp37m-
+0001cb30: 6d75 736c 6c69 6e75 785f 315f 315f 6936  musllinux_1_1_i6
+0001cb40: 3836 2e77 686c 222c 2068 6173 6820 3d20  86.whl", hash = 
+0001cb50: 2273 6861 3235 363a 6231 3634 6363 3363  "sha256:b164cc3c
+0001cb60: 3861 6362 3364 3130 3265 3331 3166 3265  8acb3d102e311f2e
+0001cb70: 6236 6633 6333 3035 3836 3565 6362 3337  b6f3c305865ecb37
+0001cb80: 3765 3536 6164 6330 3135 6362 3531 6637  7e56adc015cb51f7
+0001cb90: 3231 6631 6464 6136 227d 2c0a 2020 2020  21f1dda6"},.    
+0001cba0: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
+0001cbb0: 352e 302e 322d 6370 3337 2d63 7033 376d  5.0.2-cp37-cp37m
+0001cbc0: 2d6d 7573 6c6c 696e 7578 5f31 5f31 5f78  -musllinux_1_1_x
+0001cbd0: 3836 5f36 342e 7768 6c22 2c20 6861 7368  86_64.whl", hash
+0001cbe0: 203d 2022 7368 6132 3536 3a32 3866 6462   = "sha256:28fdb
+0001cbf0: 3932 3234 6132 3538 3133 3437 3834 6139  9224a258134784a9
+0001cc00: 6366 3030 3962 3539 3236 3561 3964 6465  cf009b59265a9dde
+0001cc10: 3739 3538 3266 6237 3530 6434 6538 3861  79582fb750d4e88a
+0001cc20: 3662 6362 6336 6661 3364 6322 7d2c 0a20  6bcbc6fa3dc"},. 
+0001cc30: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
+0001cc40: 712d 3235 2e30 2e32 2d63 7033 372d 6370  q-25.0.2-cp37-cp
+0001cc50: 3337 6d2d 7769 6e33 322e 7768 6c22 2c20  37m-win32.whl", 
+0001cc60: 6861 7368 203d 2022 7368 6132 3536 3a64  hash = "sha256:d
+0001cc70: 6437 3731 6134 3430 6566 6661 3163 3336  d771a440effa1c36
+0001cc80: 6433 3532 3362 6336 6261 3465 3534 6666  d3523bc6ba4e54ff
+0001cc90: 3564 3265 3534 6234 6164 6363 3165 3036  5d2e54b4adcc1e06
+0001cca0: 3064 3866 3363 6133 3732 3164 3232 3822  0d8f3ca3721d228"
+0001ccb0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001ccc0: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
+0001ccd0: 372d 6370 3337 6d2d 7769 6e5f 616d 6436  7-cp37m-win_amd6
+0001cce0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001ccf0: 7368 6132 3536 3a39 6264 6334 3065 6662  sha256:9bdc40efb
+0001cd00: 3637 3962 3964 6363 3339 6330 3664 3235  679b9dcc39c06d25
+0001cd10: 3632 3965 3535 3538 3165 3463 3466 3738  629e55581e4c4f78
+0001cd20: 3730 6135 6538 3864 6234 6631 6335 3163  70a5e88db4f1c51c
+0001cd30: 6532 3565 3230 6422 7d2c 0a20 2020 207b  e25e20d"},.    {
+0001cd40: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
+0001cd50: 2e30 2e32 2d63 7033 382d 6370 3338 2d6d  .0.2-cp38-cp38-m
+0001cd60: 6163 6f73 785f 3130 5f31 355f 756e 6976  acosx_10_15_univ
+0001cd70: 6572 7361 6c32 2e77 686c 222c 2068 6173  ersal2.whl", has
+0001cd80: 6820 3d20 2273 6861 3235 363a 3166 3832  h = "sha256:1f82
+0001cd90: 3930 3661 3264 3865 3465 6533 3130 6633  906a2d8e4ee310f3
+0001cda0: 3034 3837 6231 3635 6537 6363 3865 6430  0487b165e7cc8ed0
+0001cdb0: 3963 3030 3965 3435 3032 6461 3637 3137  9c009e4502da6717
+0001cdc0: 3862 3033 3038 3363 3463 6530 227d 2c0a  8b03083c4ce0"},.
+0001cdd0: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001cde0: 6d71 2d32 352e 302e 322d 6370 3338 2d63  mq-25.0.2-cp38-c
+0001cdf0: 7033 382d 6d61 636f 7378 5f31 305f 395f  p38-macosx_10_9_
+0001ce00: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
+0001ce10: 6820 3d20 2273 6861 3235 363a 3231 6563  h = "sha256:21ec
+0001ce20: 3062 6634 3833 3139 3838 6166 3433 6338  0bf4831988af43c8
+0001ce30: 6436 3662 6133 6363 6438 3161 6632 6335  d66ba3ccd81af2c5
+0001ce40: 6537 3933 6531 6266 3637 3930 6562 3264  e793e1bf6790eb2d
+0001ce50: 3530 6532 3762 3363 3537 3061 227d 2c0a  50e27b3c570a"},.
+0001ce60: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001ce70: 6d71 2d32 352e 302e 322d 6370 3338 2d63  mq-25.0.2-cp38-c
+0001ce80: 7033 382d 6d61 6e79 6c69 6e75 785f 325f  p38-manylinux_2_
+0001ce90: 3132 5f69 3638 362e 6d61 6e79 6c69 6e75  12_i686.manylinu
+0001cea0: 7832 3031 305f 6936 3836 2e77 686c 222c  x2010_i686.whl",
+0001ceb0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
+0001cec0: 6162 6263 6539 3832 6131 3763 3838 6432  abbce982a17c88d2
+0001ced0: 3331 3265 6332 6366 3736 3733 3938 3564  312ec2cf7673985d
+0001cee0: 3434 3466 3162 6561 6163 3665 3831 3839  444f1beaac6e8189
+0001cef0: 3432 3465 3061 3065 3034 3438 6462 6233  424e0a0e0448dbb3
+0001cf00: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
+0001cf10: 2270 797a 6d71 2d32 352e 302e 322d 6370  "pyzmq-25.0.2-cp
+0001cf20: 3338 2d63 7033 382d 6d61 6e79 6c69 6e75  38-cp38-manylinu
+0001cf30: 785f 325f 3132 5f78 3836 5f36 342e 6d61  x_2_12_x86_64.ma
+0001cf40: 6e79 6c69 6e75 7832 3031 305f 7838 365f  nylinux2010_x86_
+0001cf50: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
+0001cf60: 2273 6861 3235 363a 3965 3164 3266 3264  "sha256:9e1d2f2d
+0001cf70: 3836 6663 3735 6564 3766 3838 3435 6139  86fc75ed7f8845a9
+0001cf80: 3932 6335 6636 6631 6162 3564 6239 3937  92c5f6f1ab5db997
+0001cf90: 3437 6662 3064 3738 6235 6534 3034 3664  47fb0d78b5e4046d
+0001cfa0: 3034 3131 3634 6432 227d 2c0a 2020 2020  041164d2"},.    
+0001cfb0: 7b66 696c 6520 3d20 2270 797a 6d71 2d32  {file = "pyzmq-2
+0001cfc0: 352e 302e 322d 6370 3338 2d63 7033 382d  5.0.2-cp38-cp38-
+0001cfd0: 6d61 6e79 6c69 6e75 785f 325f 3137 5f61  manylinux_2_17_a
+0001cfe0: 6172 6368 3634 2e6d 616e 796c 696e 7578  arch64.manylinux
+0001cff0: 3230 3134 5f61 6172 6368 3634 2e77 686c  2014_aarch64.whl
+0001d000: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001d010: 363a 6132 6539 3266 6632 3061 6435 6431  6:a2e92ff20ad5d1
+0001d020: 3332 3636 6263 3939 3961 3239 6564 3239  3266bc999a29ed29
+0001d030: 6133 6235 6231 3031 6332 3166 6466 3462  a3b5b101c21fdf4b
+0001d040: 3263 6634 3230 6330 3964 6239 6662 3639  2cf420c09db9fb69
+0001d050: 3065 227d 2c0a 2020 2020 7b66 696c 6520  0e"},.    {file 
+0001d060: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001d070: 6370 3338 2d63 7033 382d 6d75 736c 6c69  cp38-cp38-muslli
+0001d080: 6e75 785f 315f 315f 6161 7263 6836 342e  nux_1_1_aarch64.
+0001d090: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+0001d0a0: 6132 3536 3a65 6462 6266 3036 6363 3237  a256:edbbf06cc27
+0001d0b0: 3139 3838 3934 3730 6138 6432 6266 3530  19889470a8d2bf50
+0001d0c0: 3732 6262 3030 6634 3233 6531 3264 6530  72bb00f423e12de0
+0001d0d0: 6562 3966 6665 6339 3436 6332 6339 3734  eb9ffec946c2c974
+0001d0e0: 3865 3134 3922 7d2c 0a20 2020 207b 6669  8e149"},.    {fi
+0001d0f0: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
+0001d100: 2e32 2d63 7033 382d 6370 3338 2d6d 7573  .2-cp38-cp38-mus
+0001d110: 6c6c 696e 7578 5f31 5f31 5f69 3638 362e  llinux_1_1_i686.
+0001d120: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+0001d130: 6132 3536 3a37 3739 3432 3234 3366 6634  a256:77942243ff4
+0001d140: 6431 3464 3930 6331 3162 3261 6664 3865  d14d90c11b2afd8e
+0001d150: 6536 6330 3339 6234 3561 3062 6534 6535  e6c039b45a0be4e5
+0001d160: 3366 6236 6661 3766 3565 3466 6430 6235  3fb6fa7f5e4fd0b5
+0001d170: 3964 6133 3922 7d2c 0a20 2020 207b 6669  9da39"},.    {fi
+0001d180: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
+0001d190: 2e32 2d63 7033 382d 6370 3338 2d6d 7573  .2-cp38-cp38-mus
+0001d1a0: 6c6c 696e 7578 5f31 5f31 5f78 3836 5f36  llinux_1_1_x86_6
+0001d1b0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001d1c0: 7368 6132 3536 3a61 6230 3436 6539 6362  sha256:ab046e9cb
+0001d1d0: 3930 3264 3166 3632 6339 6363 3065 6361  902d1f62c9cc0eca
+0001d1e0: 3035 3562 3164 3131 3130 3862 6463 3237  055b1d11108bdc27
+0001d1f0: 3163 6166 3763 3231 3731 3438 3732 3938  1caf7c2171487298
+0001d200: 6632 3239 6235 3622 7d2c 0a20 2020 207b  f229b56"},.    {
+0001d210: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
+0001d220: 2e30 2e32 2d63 7033 382d 6370 3338 2d77  .0.2-cp38-cp38-w
+0001d230: 696e 3332 2e77 686c 222c 2068 6173 6820  in32.whl", hash 
+0001d240: 3d20 2273 6861 3235 363a 6164 3736 3163  = "sha256:ad761c
+0001d250: 6662 6534 3737 3233 3638 3032 6137 6162  fbe477236802a7ab
+0001d260: 3263 3038 3064 3236 3863 3935 6537 3834  2c080d268c95e784
+0001d270: 6665 3330 6361 6661 3765 3035 3561 6163  fe30cafa7e055aac
+0001d280: 6431 6361 3837 3765 6230 227d 2c0a 2020  d1ca877eb0"},.  
+0001d290: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
+0001d2a0: 2d32 352e 302e 322d 6370 3338 2d63 7033  -25.0.2-cp38-cp3
+0001d2b0: 382d 7769 6e5f 616d 6436 342e 7768 6c22  8-win_amd64.whl"
+0001d2c0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001d2d0: 3a38 3536 3037 3536 3331 3865 6337 6334  :8560756318ec7c4
+0001d2e0: 6334 3964 3263 3334 3130 3132 3136 3765  c49d2c341012167e
+0001d2f0: 3730 3462 3561 3436 6439 3033 3439 3035  704b5a46d9034905
+0001d300: 3835 3363 3364 3161 6465 3466 3535 6265  853c3d1ade4f55be
+0001d310: 6522 7d2c 0a20 2020 207b 6669 6c65 203d  e"},.    {file =
+0001d320: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
+0001d330: 7033 392d 6370 3339 2d6d 6163 6f73 785f  p39-cp39-macosx_
+0001d340: 3130 5f31 355f 756e 6976 6572 7361 6c32  10_15_universal2
+0001d350: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001d360: 6861 3235 363a 6162 3263 3035 3661 6335  ha256:ab2c056ac5
+0001d370: 3033 6632 3561 3633 6636 6338 6336 3737  03f25a63f6c8c677
+0001d380: 3133 3733 6532 6137 3131 6239 3862 3330  1373e2a711b98b30
+0001d390: 3436 3134 3135 3164 6662 3535 3264 3364  4614151dfb552d3d
+0001d3a0: 3663 3831 6636 227d 2c0a 2020 2020 7b66  6c81f6"},.    {f
+0001d3b0: 696c 6520 3d20 2270 797a 6d71 2d32 352e  ile = "pyzmq-25.
+0001d3c0: 302e 322d 6370 3339 2d63 7033 392d 6d61  0.2-cp39-cp39-ma
+0001d3d0: 636f 7378 5f31 305f 395f 7838 365f 3634  cosx_10_9_x86_64
+0001d3e0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001d3f0: 6861 3235 363a 6363 6138 3532 3462 3631  ha256:cca8524b61
+0001d400: 6330 6561 6161 3335 3035 3338 3264 6339  c0eaaa3505382dc9
+0001d410: 6239 6133 6263 3831 3635 6631 6436 6330  b9a3bc8165f1d6c0
+0001d420: 3130 6664 6431 3435 3263 3232 3432 3235  10fdd1452c224225
+0001d430: 6132 3636 3839 227d 2c0a 2020 2020 7b66  a26689"},.    {f
+0001d440: 696c 6520 3d20 2270 797a 6d71 2d32 352e  ile = "pyzmq-25.
+0001d450: 302e 322d 6370 3339 2d63 7033 392d 6d61  0.2-cp39-cp39-ma
+0001d460: 6e79 6c69 6e75 785f 325f 3132 5f69 3638  nylinux_2_12_i68
+0001d470: 362e 6d61 6e79 6c69 6e75 7832 3031 305f  6.manylinux2010_
+0001d480: 6936 3836 2e77 686c 222c 2068 6173 6820  i686.whl", hash 
+0001d490: 3d20 2273 6861 3235 363a 6366 6239 6637  = "sha256:cfb9f7
+0001d4a0: 6561 6530 3264 3361 6334 3266 6265 6461  eae02d3ac42fbeda
+0001d4b0: 6433 3030 3036 6237 3430 3763 3938 3461  d30006b7407c984a
+0001d4c0: 3065 6234 3138 3961 3133 3232 3234 3161  0eb4189a1322241a
+0001d4d0: 3230 3934 3464 3631 6535 227d 2c0a 2020  20944d61e5"},.  
+0001d4e0: 2020 7b66 696c 6520 3d20 2270 797a 6d71    {file = "pyzmq
+0001d4f0: 2d32 352e 302e 322d 6370 3339 2d63 7033  -25.0.2-cp39-cp3
+0001d500: 392d 6d61 6e79 6c69 6e75 785f 325f 3132  9-manylinux_2_12
+0001d510: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
+0001d520: 7832 3031 305f 7838 365f 3634 2e77 686c  x2010_x86_64.whl
+0001d530: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001d540: 363a 3565 6165 6165 3033 3863 3638 3734  6:5eaeae038c6874
+0001d550: 3830 3832 3133 3764 3638 3936 6435 6334  8082137d6896d5c4
+0001d560: 6462 3739 3237 6539 3334 3932 3337 6465  db7927e9349237de
+0001d570: 6430 3865 6531 6262 6439 3466 3733 3631  d08ee1bbd94f7361
+0001d580: 6339 227d 2c0a 2020 2020 7b66 696c 6520  c9"},.    {file 
+0001d590: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001d5a0: 6370 3339 2d63 7033 392d 6d61 6e79 6c69  cp39-cp39-manyli
+0001d5b0: 6e75 785f 325f 3137 5f61 6172 6368 3634  nux_2_17_aarch64
+0001d5c0: 2e6d 616e 796c 696e 7578 3230 3134 5f61  .manylinux2014_a
+0001d5d0: 6172 6368 3634 2e77 686c 222c 2068 6173  arch64.whl", has
+0001d5e0: 6820 3d20 2273 6861 3235 363a 3461 3331  h = "sha256:4a31
+0001d5f0: 3939 3261 3866 3864 3531 3636 3365 6266  992a8f8d51663ebf
+0001d600: 3739 6466 3064 6636 6130 3466 6662 3930  79df0df6a04ffb90
+0001d610: 3530 3633 3038 3364 3638 3264 3433 3830  5063083d682d4380
+0001d620: 6162 3864 3263 3637 3235 3763 227d 2c0a  ab8d2c67257c"},.
+0001d630: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001d640: 6d71 2d32 352e 302e 322d 6370 3339 2d63  mq-25.0.2-cp39-c
+0001d650: 7033 392d 6d75 736c 6c69 6e75 785f 315f  p39-musllinux_1_
+0001d660: 315f 6161 7263 6836 342e 7768 6c22 2c20  1_aarch64.whl", 
+0001d670: 6861 7368 203d 2022 7368 6132 3536 3a36  hash = "sha256:6
+0001d680: 6139 3739 6535 3964 3231 3834 6130 6338  a979e59d2184a0c8
+0001d690: 6632 6564 6534 6230 3831 3063 6264 6438  f2ede4b0810cbdd8
+0001d6a0: 3662 3634 6439 3964 3963 6338 6130 3233  6b64d99d9cc8a023
+0001d6b0: 3932 3965 3430 6463 6537 6338 3663 6322  929e40dce7c86cc"
+0001d6c0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001d6d0: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
+0001d6e0: 392d 6370 3339 2d6d 7573 6c6c 696e 7578  9-cp39-musllinux
+0001d6f0: 5f31 5f31 5f69 3638 362e 7768 6c22 2c20  _1_1_i686.whl", 
+0001d700: 6861 7368 203d 2022 7368 6132 3536 3a31  hash = "sha256:1
+0001d710: 6631 3234 6362 3733 6631 6161 3636 3534  f124cb73f1aa6654
+0001d720: 6433 3162 3138 3338 3130 6665 6263 3835  d31b183810febc85
+0001d730: 3035 6664 3063 3539 3761 6661 3132 3763  05fd0c597afa127c
+0001d740: 3466 3430 3037 3662 6534 3537 3465 3022  4f40076be4574e0"
+0001d750: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001d760: 7079 7a6d 712d 3235 2e30 2e32 2d63 7033  pyzmq-25.0.2-cp3
+0001d770: 392d 6370 3339 2d6d 7573 6c6c 696e 7578  9-cp39-musllinux
+0001d780: 5f31 5f31 5f78 3836 5f36 342e 7768 6c22  _1_1_x86_64.whl"
+0001d790: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001d7a0: 3a36 3563 3139 6136 3362 3461 3833 6165  :65c19a63b4a83ae
+0001d7b0: 3435 6436 3231 3738 6237 3032 3233 6164  45d62178b70223ad
+0001d7c0: 6565 6535 6631 3266 3330 3332 3732 3662  eee5f12f3032726b
+0001d7d0: 3839 3734 3331 6236 3535 3361 6132 3561  897431b6553aa25a
+0001d7e0: 6622 7d2c 0a20 2020 207b 6669 6c65 203d  f"},.    {file =
+0001d7f0: 2022 7079 7a6d 712d 3235 2e30 2e32 2d63   "pyzmq-25.0.2-c
+0001d800: 7033 392d 6370 3339 2d77 696e 3332 2e77  p39-cp39-win32.w
+0001d810: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+0001d820: 3235 363a 3833 6438 3232 6538 3638 3736  256:83d822e86876
+0001d830: 3231 6265 6438 3734 3034 6166 6331 6330  21bed87404afc1c0
+0001d840: 3364 3833 6661 3263 6533 3937 3333 6435  3d83fa2ce39733d5
+0001d850: 3463 3266 6435 3264 3838 3239 6564 6238  4c2fd52d8829edb8
+0001d860: 6137 6666 227d 2c0a 2020 2020 7b66 696c  a7ff"},.    {fil
+0001d870: 6520 3d20 2270 797a 6d71 2d32 352e 302e  e = "pyzmq-25.0.
+0001d880: 322d 6370 3339 2d63 7033 392d 7769 6e5f  2-cp39-cp39-win_
+0001d890: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+0001d8a0: 203d 2022 7368 6132 3536 3a32 3436 3833   = "sha256:24683
+0001d8b0: 3238 3563 6336 6237 6266 3138 6164 3337  285cc6b7bf18ad37
+0001d8c0: 6437 3562 3964 6230 6530 6665 6665 3538  d75b9db0e0fefe58
+0001d8d0: 3430 3465 3730 3031 6631 6438 3262 6639  404e7001f1d82bf9
+0001d8e0: 6537 3231 3830 3664 6161 3722 7d2c 0a20  e721806daa7"},. 
+0001d8f0: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
+0001d900: 712d 3235 2e30 2e32 2d70 7033 372d 7079  q-25.0.2-pp37-py
+0001d910: 7079 3337 5f70 7037 332d 6d61 636f 7378  py37_pp73-macosx
+0001d920: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
+0001d930: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001d940: 363a 3461 3462 3432 3631 6562 3866 3965  6:4a4b4261eb8f9e
+0001d950: 6437 3166 3633 6239 6562 3031 3938 6464  d71f63b9eb0198dd
+0001d960: 3763 3933 3461 6133 6233 3937 3264 6163  7c934aa3b3972dac
+0001d970: 3538 3664 3065 6635 3032 6261 3961 6230  586d0ef502ba9ab0
+0001d980: 3862 227d 2c0a 2020 2020 7b66 696c 6520  8b"},.    {file 
+0001d990: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001d9a0: 7070 3337 2d70 7970 7933 375f 7070 3733  pp37-pypy37_pp73
+0001d9b0: 2d6d 616e 796c 696e 7578 5f32 5f31 325f  -manylinux_2_12_
+0001d9c0: 6936 3836 2e6d 616e 796c 696e 7578 3230  i686.manylinux20
+0001d9d0: 3130 5f69 3638 362e 7768 6c22 2c20 6861  10_i686.whl", ha
+0001d9e0: 7368 203d 2022 7368 6132 3536 3a36 3265  sh = "sha256:62e
+0001d9f0: 6338 6439 3739 6635 3663 3030 3533 6139  c8d979f56c0053a9
+0001da00: 3262 3262 3661 3130 6666 3534 6239 6563  2b2b6a10ff54b9ec
+0001da10: 3861 3466 3138 3764 6232 6236 6563 3331  8a4f187db2b6ec31
+0001da20: 6565 3364 6436 6433 6361 3665 3222 7d2c  ee3dd6d3ca6e2"},
+0001da30: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001da40: 7a6d 712d 3235 2e30 2e32 2d70 7033 372d  zmq-25.0.2-pp37-
+0001da50: 7079 7079 3337 5f70 7037 332d 6d61 6e79  pypy37_pp73-many
+0001da60: 6c69 6e75 785f 325f 3132 5f78 3836 5f36  linux_2_12_x86_6
+0001da70: 342e 6d61 6e79 6c69 6e75 7832 3031 305f  4.manylinux2010_
+0001da80: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
+0001da90: 6820 3d20 2273 6861 3235 363a 6166 6665  h = "sha256:affe
+0001daa0: 6331 3437 3033 3531 3137 3865 3839 3231  c1470351178e8921
+0001dab0: 3231 6233 3431 3463 3865 6637 3830 3332  21b3414c8ef78032
+0001dac0: 3639 6632 3037 6266 3962 6566 3835 6639  69f207bf9bef85f9
+0001dad0: 6136 6464 3131 6364 6532 3634 227d 2c0a  a6dd11cde264"},.
+0001dae0: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001daf0: 6d71 2d32 352e 302e 322d 7070 3337 2d70  mq-25.0.2-pp37-p
+0001db00: 7970 7933 375f 7070 3733 2d6d 616e 796c  ypy37_pp73-manyl
+0001db10: 696e 7578 5f32 5f31 375f 6161 7263 6836  inux_2_17_aarch6
+0001db20: 342e 6d61 6e79 6c69 6e75 7832 3031 345f  4.manylinux2014_
+0001db30: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
+0001db40: 7368 203d 2022 7368 6132 3536 3a66 6663  sh = "sha256:ffc
+0001db50: 3731 3131 3134 3333 6264 3665 6338 3630  71111433bd6ec860
+0001db60: 3761 3337 6239 3231 3166 3465 6634 3265  7a37b9211f4ef42e
+0001db70: 3364 3362 3237 3163 3664 3736 6338 3133  3d3b271c6d76c813
+0001db80: 3636 3938 3334 3736 3462 3234 3822 7d2c  669834764b248"},
+0001db90: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001dba0: 7a6d 712d 3235 2e30 2e32 2d70 7033 372d  zmq-25.0.2-pp37-
+0001dbb0: 7079 7079 3337 5f70 7037 332d 7769 6e5f  pypy37_pp73-win_
+0001dbc0: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+0001dbd0: 203d 2022 7368 6132 3536 3a36 6661 6463   = "sha256:6fadc
+0001dbe0: 3630 3937 3037 3134 6438 3665 6666 3237  60970714d86eff27
+0001dbf0: 3832 3166 3866 6230 3166 3833 3238 6464  821f8fb01f8328dd
+0001dc00: 3336 6265 6264 3439 3662 3035 3634 6135  36bebd496b0564a5
+0001dc10: 3030 6665 3461 3965 3335 3422 7d2c 0a20  00fe4a9e354"},. 
+0001dc20: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
+0001dc30: 712d 3235 2e30 2e32 2d70 7033 382d 7079  q-25.0.2-pp38-py
+0001dc40: 7079 3338 5f70 7037 332d 6d61 636f 7378  py38_pp73-macosx
+0001dc50: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
+0001dc60: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001dc70: 363a 3236 3939 3638 6632 6137 3663 3035  6:269968f2a76c05
+0001dc80: 3133 3439 3061 6562 3362 6130 6463 3363  13490aeb3ba0dc3c
+0001dc90: 3737 6237 6337 6131 3164 6161 3839 3466  77b7c7a11daa894f
+0001dca0: 3964 3164 6138 3864 3461 3064 6230 3938  9d1da88d4a0db098
+0001dcb0: 3335 227d 2c0a 2020 2020 7b66 696c 6520  35"},.    {file 
+0001dcc0: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001dcd0: 7070 3338 2d70 7970 7933 385f 7070 3733  pp38-pypy38_pp73
+0001dce0: 2d6d 616e 796c 696e 7578 5f32 5f31 325f  -manylinux_2_12_
+0001dcf0: 6936 3836 2e6d 616e 796c 696e 7578 3230  i686.manylinux20
+0001dd00: 3130 5f69 3638 362e 7768 6c22 2c20 6861  10_i686.whl", ha
+0001dd10: 7368 203d 2022 7368 6132 3536 3a66 3763  sh = "sha256:f7c
+0001dd20: 3862 3833 3638 6538 3433 3831 6165 3763  8b8368e84381ae7c
+0001dd30: 3537 6631 6635 3238 3362 3032 3963 3838  57f1f5283b029c88
+0001dd40: 3835 3034 6161 6634 3934 3963 3332 6536  8504aaf4949c32e6
+0001dd50: 6536 6662 3235 3665 6339 6266 3022 7d2c  e6fb256ec9bf0"},
+0001dd60: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001dd70: 7a6d 712d 3235 2e30 2e32 2d70 7033 382d  zmq-25.0.2-pp38-
+0001dd80: 7079 7079 3338 5f70 7037 332d 6d61 6e79  pypy38_pp73-many
+0001dd90: 6c69 6e75 785f 325f 3132 5f78 3836 5f36  linux_2_12_x86_6
+0001dda0: 342e 6d61 6e79 6c69 6e75 7832 3031 305f  4.manylinux2010_
+0001ddb0: 7838 365f 3634 2e77 686c 222c 2068 6173  x86_64.whl", has
+0001ddc0: 6820 3d20 2273 6861 3235 363a 3235 6536  h = "sha256:25e6
+0001ddd0: 3837 3361 3730 6164 3561 6133 3165 3461  873a70ad5aa31e4a
+0001dde0: 3763 3431 6535 6538 6337 3039 3239 3665  7c41e5e8c709296e
+0001ddf0: 6465 6634 6139 3233 3133 6531 6364 3566  def4a92313e1cd5f
+0001de00: 6338 3762 6264 3138 3734 6532 227d 2c0a  c87bbd1874e2"},.
+0001de10: 2020 2020 7b66 696c 6520 3d20 2270 797a      {file = "pyz
+0001de20: 6d71 2d32 352e 302e 322d 7070 3338 2d70  mq-25.0.2-pp38-p
+0001de30: 7970 7933 385f 7070 3733 2d6d 616e 796c  ypy38_pp73-manyl
+0001de40: 696e 7578 5f32 5f31 375f 6161 7263 6836  inux_2_17_aarch6
+0001de50: 342e 6d61 6e79 6c69 6e75 7832 3031 345f  4.manylinux2014_
+0001de60: 6161 7263 6836 342e 7768 6c22 2c20 6861  aarch64.whl", ha
+0001de70: 7368 203d 2022 7368 6132 3536 3a62 3733  sh = "sha256:b73
+0001de80: 3330 3736 6666 3436 6537 6462 3535 3034  3076ff46e7db5504
+0001de90: 6335 6537 3238 3466 3034 6139 3835 3263  c5e7284f04a9852c
+0001dea0: 3633 3231 3463 3734 3638 3862 6462 3631  63214c74688bdb61
+0001deb0: 3335 3830 3835 3331 3735 3561 3322 7d2c  35808531755a3"},
+0001dec0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001ded0: 7a6d 712d 3235 2e30 2e32 2d70 7033 382d  zmq-25.0.2-pp38-
+0001dee0: 7079 7079 3338 5f70 7037 332d 7769 6e5f  pypy38_pp73-win_
+0001def0: 616d 6436 342e 7768 6c22 2c20 6861 7368  amd64.whl", hash
+0001df00: 203d 2022 7368 6132 3536 3a61 3666 3661   = "sha256:a6f6a
+0001df10: 6531 3234 3738 6664 6332 3661 3664 3566  e12478fdc26a6d5f
+0001df20: 6462 3231 6638 3036 6230 3866 6135 3430  db21f806b08fa540
+0001df30: 3363 6430 3266 6433 3132 6534 6362 3566  3cd02fd312e4cb5f
+0001df40: 3732 6466 3037 3866 3936 6622 7d2c 0a20  72df078f96f"},. 
+0001df50: 2020 207b 6669 6c65 203d 2022 7079 7a6d     {file = "pyzm
+0001df60: 712d 3235 2e30 2e32 2d70 7033 392d 7079  q-25.0.2-pp39-py
+0001df70: 7079 3339 5f70 7037 332d 6d61 636f 7378  py39_pp73-macosx
+0001df80: 5f31 305f 395f 7838 365f 3634 2e77 686c  _10_9_x86_64.whl
+0001df90: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001dfa0: 363a 3637 6461 3163 3231 3366 6264 3230  6:67da1c213fbd20
+0001dfb0: 3839 3036 6162 3334 3730 6366 6666 3165  8906ab3470cfff1e
+0001dfc0: 6530 3034 3838 3338 3336 3531 3335 6139  e0048838365135a9
+0001dfd0: 6264 6463 3762 3430 6231 3165 3664 3663  bddc7b40b11e6d6c
+0001dfe0: 3839 227d 2c0a 2020 2020 7b66 696c 6520  89"},.    {file 
+0001dff0: 3d20 2270 797a 6d71 2d32 352e 302e 322d  = "pyzmq-25.0.2-
+0001e000: 7070 3339 2d70 7970 7933 395f 7070 3733  pp39-pypy39_pp73
+0001e010: 2d6d 616e 796c 696e 7578 5f32 5f31 375f  -manylinux_2_17_
+0001e020: 6161 7263 6836 342e 6d61 6e79 6c69 6e75  aarch64.manylinu
+0001e030: 7832 3031 345f 6161 7263 6836 342e 7768  x2014_aarch64.wh
+0001e040: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+0001e050: 3536 3a35 3331 6533 3664 3966 6364 3636  56:531e36d9fcd66
+0001e060: 6631 3864 6532 3734 3334 6132 3562 3531  f18de27434a25b51
+0001e070: 6431 3337 6562 3534 3639 3331 3033 3366  d137eb546931033f
+0001e080: 3339 3265 3835 3637 3463 3761 3763 6561  392e85674c7a7cea
+0001e090: 3835 3322 7d2c 0a20 2020 207b 6669 6c65  853"},.    {file
+0001e0a0: 203d 2022 7079 7a6d 712d 3235 2e30 2e32   = "pyzmq-25.0.2
+0001e0b0: 2d70 7033 392d 7079 7079 3339 5f70 7037  -pp39-pypy39_pp7
+0001e0c0: 332d 6d61 6e79 6c69 6e75 785f 325f 3137  3-manylinux_2_17
+0001e0d0: 5f69 3638 362e 6d61 6e79 6c69 6e75 7832  _i686.manylinux2
+0001e0e0: 3031 345f 6936 3836 2e77 686c 222c 2068  014_i686.whl", h
+0001e0f0: 6173 6820 3d20 2273 6861 3235 363a 3334  ash = "sha256:34
+0001e100: 6136 6664 6464 3135 3966 6633 3861 6139  a6fddd159ff38aa9
+0001e110: 3439 3762 3265 3334 3261 3535 3966 3134  497b2e342a559f14
+0001e120: 3261 6233 3635 3537 3632 3834 6263 3866  2ab365576284bc8f
+0001e130: 3737 6362 3365 6164 3166 3739 6335 227d  77cb3ead1f79c5"}
+0001e140: 2c0a 2020 2020 7b66 696c 6520 3d20 2270  ,.    {file = "p
+0001e150: 797a 6d71 2d32 352e 302e 322d 7070 3339  yzmq-25.0.2-pp39
+0001e160: 2d70 7970 7933 395f 7070 3733 2d6d 616e  -pypy39_pp73-man
+0001e170: 796c 696e 7578 5f32 5f31 375f 7838 365f  ylinux_2_17_x86_
+0001e180: 3634 2e6d 616e 796c 696e 7578 3230 3134  64.manylinux2014
+0001e190: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
+0001e1a0: 7368 203d 2022 7368 6132 3536 3a62 3439  sh = "sha256:b49
+0001e1b0: 3139 3938 6566 3838 3636 3632 6331 6633  1998ef886662c1f3
+0001e1c0: 6434 3965 6132 3139 3830 3535 6139 6135  d49ea2198055a9a5
+0001e1d0: 3336 6464 6637 3433 3062 3035 3162 3231  36ddf7430b051b21
+0001e1e0: 3035 3466 3261 3538 3331 3830 3022 7d2c  054f2a5831800"},
+0001e1f0: 0a20 2020 207b 6669 6c65 203d 2022 7079  .    {file = "py
+0001e200: 7a6d 712d 3235 2e30 2e32 2d70 7033 392d  zmq-25.0.2-pp39-
+0001e210: 7079 7079 3339 5f70 7037 332d 6d61 6e79  pypy39_pp73-many
+0001e220: 6c69 6e75 785f 325f 3238 5f78 3836 5f36  linux_2_28_x86_6
+0001e230: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001e240: 7368 6132 3536 3a35 6434 3936 3831 3530  sha256:5d4968150
+0001e250: 3734 6533 6533 6431 3833 6665 3263 3766  74e3e3d183fe2c7f
+0001e260: 6365 6132 3130 3961 6436 3762 3734 3038  cea2109ad67b7408
+0001e270: 3463 3235 3434 3831 6638 3762 3634 6530  4c254481f87b64e0
+0001e280: 3465 3961 3437 3122 7d2c 0a20 2020 207b  4e9a471"},.    {
+0001e290: 6669 6c65 203d 2022 7079 7a6d 712d 3235  file = "pyzmq-25
+0001e2a0: 2e30 2e32 2d70 7033 392d 7079 7079 3339  .0.2-pp39-pypy39
+0001e2b0: 5f70 7037 332d 7769 6e5f 616d 6436 342e  _pp73-win_amd64.
+0001e2c0: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+0001e2d0: 6132 3536 3a35 3661 3934 6162 3164 3132  a256:56a94ab1d12
+0001e2e0: 6166 3938 3262 3535 6361 3936 6336 3835  af982b55ca96c685
+0001e2f0: 3364 6236 6163 3835 3530 3565 3832 3064  3db6ac85505e820d
+0001e300: 3934 3538 6163 3736 3336 3463 3139 3938  9458ac76364c1998
+0001e310: 3937 3266 3422 7d2c 0a20 2020 207b 6669  972f4"},.    {fi
+0001e320: 6c65 203d 2022 7079 7a6d 712d 3235 2e30  le = "pyzmq-25.0
+0001e330: 2e32 2e74 6172 2e67 7a22 2c20 6861 7368  .2.tar.gz", hash
+0001e340: 203d 2022 7368 6132 3536 3a36 6238 6331   = "sha256:6b8c1
+0001e350: 6262 6237 3065 3836 3864 6338 3838 3031  bbb70e868dc88801
+0001e360: 6161 3533 3263 6165 3662 6434 6533 6235  aa532cae6bd4e3b5
+0001e370: 3233 3337 3834 3639 3262 3738 3666 3137  233784692b786f17
+0001e380: 6164 3239 3632 6535 3134 3922 7d2c 0a5d  ad2962e5149"},.]
+0001e390: 0a0a 5b70 6163 6b61 6765 2e64 6570 656e  ..[package.depen
+0001e3a0: 6465 6e63 6965 735d 0a63 6666 6920 3d20  dencies].cffi = 
+0001e3b0: 7b76 6572 7369 6f6e 203d 2022 2a22 2c20  {version = "*", 
+0001e3c0: 6d61 726b 6572 7320 3d20 2269 6d70 6c65  markers = "imple
+0001e3d0: 6d65 6e74 6174 696f 6e5f 6e61 6d65 203d  mentation_name =
+0001e3e0: 3d20 5c22 7079 7079 5c22 227d 0a0a 5b5b  = \"pypy\""}..[[
+0001e3f0: 7061 636b 6167 655d 5d0a 6e61 6d65 203d  package]].name =
+0001e400: 2022 7265 7175 6573 7473 220a 7665 7273   "requests".vers
+0001e410: 696f 6e20 3d20 2232 2e33 312e 3022 0a64  ion = "2.31.0".d
+0001e420: 6573 6372 6970 7469 6f6e 203d 2022 5079  escription = "Py
+0001e430: 7468 6f6e 2048 5454 5020 666f 7220 4875  thon HTTP for Hu
+0001e440: 6d61 6e73 2e22 0a6f 7074 696f 6e61 6c20  mans.".optional 
+0001e450: 3d20 6661 6c73 650a 7079 7468 6f6e 2d76  = false.python-v
+0001e460: 6572 7369 6f6e 7320 3d20 223e 3d33 2e37  ersions = ">=3.7
+0001e470: 220a 6669 6c65 7320 3d20 5b0a 2020 2020  ".files = [.    
+0001e480: 7b66 696c 6520 3d20 2272 6571 7565 7374  {file = "request
+0001e490: 732d 322e 3331 2e30 2d70 7933 2d6e 6f6e  s-2.31.0-py3-non
+0001e4a0: 652d 616e 792e 7768 6c22 2c20 6861 7368  e-any.whl", hash
+0001e4b0: 203d 2022 7368 6132 3536 3a35 3863 6432   = "sha256:58cd2
+0001e4c0: 3138 3763 3031 6537 3065 3665 3236 3530  187c01e70e6e2650
+0001e4d0: 3562 6361 3735 3137 3737 6161 3966 3265  5bca751777aa9f2e
+0001e4e0: 6530 6237 6634 3330 3039 3838 6237 3039  e0b7f4300988b709
+0001e4f0: 6634 3465 3031 3330 3033 6622 7d2c 0a20  f44e013003f"},. 
+0001e500: 2020 207b 6669 6c65 203d 2022 7265 7175     {file = "requ
+0001e510: 6573 7473 2d32 2e33 312e 302e 7461 722e  ests-2.31.0.tar.
+0001e520: 677a 222c 2068 6173 6820 3d20 2273 6861  gz", hash = "sha
+0001e530: 3235 363a 3934 3263 3561 3735 3866 3938  256:942c5a758f98
+0001e540: 6437 3930 6561 6564 3161 3239 6362 3665  d790eaed1a29cb6e
+0001e550: 6566 6337 6666 6230 6431 6366 3761 6630  efc7ffb0d1cf7af0
+0001e560: 3563 3364 3237 3931 3635 3664 6264 3661  5c3d2791656dbd6a
+0001e570: 6431 6531 227d 2c0a 5d0a 0a5b 7061 636b  d1e1"},.]..[pack
+0001e580: 6167 652e 6465 7065 6e64 656e 6369 6573  age.dependencies
+0001e590: 5d0a 6365 7274 6966 6920 3d20 223e 3d32  ].certifi = ">=2
+0001e5a0: 3031 372e 342e 3137 220a 6368 6172 7365  017.4.17".charse
+0001e5b0: 742d 6e6f 726d 616c 697a 6572 203d 2022  t-normalizer = "
+0001e5c0: 3e3d 322c 3c34 220a 6964 6e61 203d 2022  >=2,<4".idna = "
+0001e5d0: 3e3d 322e 352c 3c34 220a 7572 6c6c 6962  >=2.5,<4".urllib
+0001e5e0: 3320 3d20 223e 3d31 2e32 312e 312c 3c33  3 = ">=1.21.1,<3
+0001e5f0: 220a 0a5b 7061 636b 6167 652e 6578 7472  "..[package.extr
+0001e600: 6173 5d0a 736f 636b 7320 3d20 5b22 5079  as].socks = ["Py
+0001e610: 536f 636b 7320 283e 3d31 2e35 2e36 2c21  Socks (>=1.5.6,!
+0001e620: 3d31 2e35 2e37 2922 5d0a 7573 652d 6368  =1.5.7)"].use-ch
+0001e630: 6172 6465 742d 6f6e 2d70 7933 203d 205b  ardet-on-py3 = [
+0001e640: 2263 6861 7264 6574 2028 3e3d 332e 302e  "chardet (>=3.0.
+0001e650: 322c 3c36 2922 5d0a 0a5b 5b70 6163 6b61  2,<6)"]..[[packa
+0001e660: 6765 5d5d 0a6e 616d 6520 3d20 2273 6574  ge]].name = "set
+0001e670: 7570 746f 6f6c 7322 0a76 6572 7369 6f6e  uptools".version
+0001e680: 203d 2022 3637 2e38 2e30 220a 6465 7363   = "67.8.0".desc
+0001e690: 7269 7074 696f 6e20 3d20 2245 6173 696c  ription = "Easil
+0001e6a0: 7920 646f 776e 6c6f 6164 2c20 6275 696c  y download, buil
+0001e6b0: 642c 2069 6e73 7461 6c6c 2c20 7570 6772  d, install, upgr
+0001e6c0: 6164 652c 2061 6e64 2075 6e69 6e73 7461  ade, and uninsta
+0001e6d0: 6c6c 2050 7974 686f 6e20 7061 636b 6167  ll Python packag
+0001e6e0: 6573 220a 6f70 7469 6f6e 616c 203d 2066  es".optional = f
+0001e6f0: 616c 7365 0a70 7974 686f 6e2d 7665 7273  alse.python-vers
+0001e700: 696f 6e73 203d 2022 3e3d 332e 3722 0a66  ions = ">=3.7".f
+0001e710: 696c 6573 203d 205b 0a20 2020 207b 6669  iles = [.    {fi
+0001e720: 6c65 203d 2022 7365 7475 7074 6f6f 6c73  le = "setuptools
+0001e730: 2d36 372e 382e 302d 7079 332d 6e6f 6e65  -67.8.0-py3-none
+0001e740: 2d61 6e79 2e77 686c 222c 2068 6173 6820  -any.whl", hash 
+0001e750: 3d20 2273 6861 3235 363a 3564 6636 3162  = "sha256:5df61b
+0001e760: 6633 3062 6231 3063 3666 3735 3665 6231  f30bb10c6f756eb1
+0001e770: 3965 3763 3966 3362 3437 3330 3531 6634  9e7c9f3b473051f4
+0001e780: 3864 6237 3766 6464 6265 3036 6666 3263  8db77fddbe06ff2c
+0001e790: 6133 3037 6466 3961 3666 227d 2c0a 2020  a307df9a6f"},.  
+0001e7a0: 2020 7b66 696c 6520 3d20 2273 6574 7570    {file = "setup
+0001e7b0: 746f 6f6c 732d 3637 2e38 2e30 2e74 6172  tools-67.8.0.tar
+0001e7c0: 2e67 7a22 2c20 6861 7368 203d 2022 7368  .gz", hash = "sh
+0001e7d0: 6132 3536 3a36 3236 3432 3335 3861 6463  a256:62642358adc
+0001e7e0: 3737 6666 6138 3732 3333 6263 3464 3233  77ffa87233bc4d23
+0001e7f0: 3534 6334 6232 3638 3264 3231 3430 3438  54c4b2682d214048
+0001e800: 6635 3030 3936 3464 6265 3736 3063 6365  f500964dbe760cce
+0001e810: 6466 3130 3222 7d2c 0a5d 0a0a 5b70 6163  df102"},.]..[pac
+0001e820: 6b61 6765 2e65 7874 7261 735d 0a64 6f63  kage.extras].doc
+0001e830: 7320 3d20 5b22 6675 726f 222c 2022 6a61  s = ["furo", "ja
+0001e840: 7261 636f 2e70 6163 6b61 6769 6e67 2028  raco.packaging (
+0001e850: 3e3d 3929 222c 2022 6a61 7261 636f 2e74  >=9)", "jaraco.t
+0001e860: 6964 656c 6966 7420 283e 3d31 2e34 2922  idelift (>=1.4)"
+0001e870: 2c20 2270 7967 6d65 6e74 732d 6769 7468  , "pygments-gith
+0001e880: 7562 2d6c 6578 6572 7320 283d 3d30 2e30  ub-lexers (==0.0
+0001e890: 2e35 2922 2c20 2272 7374 2e6c 696e 6b65  .5)", "rst.linke
+0001e8a0: 7220 283e 3d31 2e39 2922 2c20 2273 7068  r (>=1.9)", "sph
+0001e8b0: 696e 7820 283e 3d33 2e35 2922 2c20 2273  inx (>=3.5)", "s
+0001e8c0: 7068 696e 782d 6661 7669 636f 6e22 2c20  phinx-favicon", 
+0001e8d0: 2273 7068 696e 782d 686f 7665 7278 7265  "sphinx-hoverxre
+0001e8e0: 6620 283c 3229 222c 2022 7370 6869 6e78  f (<2)", "sphinx
+0001e8f0: 2d69 6e6c 696e 652d 7461 6273 222c 2022  -inline-tabs", "
+0001e900: 7370 6869 6e78 2d6c 696e 7422 2c20 2273  sphinx-lint", "s
+0001e910: 7068 696e 782d 6e6f 7466 6f75 6e64 2d70  phinx-notfound-p
+0001e920: 6167 6520 283d 3d30 2e38 2e33 2922 2c20  age (==0.8.3)", 
+0001e930: 2273 7068 696e 782d 7265 7265 6469 7265  "sphinx-reredire
+0001e940: 6374 7322 2c20 2273 7068 696e 7863 6f6e  cts", "sphinxcon
+0001e950: 7472 6962 2d74 6f77 6e63 7269 6572 225d  trib-towncrier"]
+0001e960: 0a74 6573 7469 6e67 203d 205b 2262 7569  .testing = ["bui
+0001e970: 6c64 5b76 6972 7475 616c 656e 765d 222c  ld[virtualenv]",
+0001e980: 2022 6669 6c65 6c6f 636b 2028 3e3d 332e   "filelock (>=3.
+0001e990: 342e 3029 222c 2022 666c 616b 6538 2d32  4.0)", "flake8-2
+0001e9a0: 3032 3022 2c20 2269 6e69 3274 6f6d 6c5b  020", "ini2toml[
+0001e9b0: 6c69 7465 5d20 283e 3d30 2e39 2922 2c20  lite] (>=0.9)", 
+0001e9c0: 226a 6172 6163 6f2e 656e 7673 2028 3e3d  "jaraco.envs (>=
+0001e9d0: 322e 3229 222c 2022 6a61 7261 636f 2e70  2.2)", "jaraco.p
+0001e9e0: 6174 6820 283e 3d33 2e32 2e30 2922 2c20  ath (>=3.2.0)", 
+0001e9f0: 2270 6970 2028 3e3d 3139 2e31 2922 2c20  "pip (>=19.1)", 
+0001ea00: 2270 6970 2d72 756e 2028 3e3d 382e 3829  "pip-run (>=8.8)
+0001ea10: 222c 2022 7079 7465 7374 2028 3e3d 3629  ", "pytest (>=6)
+0001ea20: 222c 2022 7079 7465 7374 2d62 6c61 636b  ", "pytest-black
+0001ea30: 2028 3e3d 302e 332e 3729 222c 2022 7079   (>=0.3.7)", "py
+0001ea40: 7465 7374 2d63 6865 636b 646f 6373 2028  test-checkdocs (
+0001ea50: 3e3d 322e 3429 222c 2022 7079 7465 7374  >=2.4)", "pytest
+0001ea60: 2d63 6f76 222c 2022 7079 7465 7374 2d65  -cov", "pytest-e
+0001ea70: 6e61 626c 6572 2028 3e3d 312e 3329 222c  nabler (>=1.3)",
+0001ea80: 2022 7079 7465 7374 2d6d 7970 7920 283e   "pytest-mypy (>
+0001ea90: 3d30 2e39 2e31 2922 2c20 2270 7974 6573  =0.9.1)", "pytes
+0001eaa0: 742d 7065 7266 222c 2022 7079 7465 7374  t-perf", "pytest
+0001eab0: 2d72 7566 6622 2c20 2270 7974 6573 742d  -ruff", "pytest-
+0001eac0: 7469 6d65 6f75 7422 2c20 2270 7974 6573  timeout", "pytes
+0001ead0: 742d 7864 6973 7422 2c20 2274 6f6d 6c69  t-xdist", "tomli
+0001eae0: 2d77 2028 3e3d 312e 302e 3029 222c 2022  -w (>=1.0.0)", "
+0001eaf0: 7669 7274 7561 6c65 6e76 2028 3e3d 3133  virtualenv (>=13
+0001eb00: 2e30 2e30 2922 2c20 2277 6865 656c 225d  .0.0)", "wheel"]
+0001eb10: 0a74 6573 7469 6e67 2d69 6e74 6567 7261  .testing-integra
+0001eb20: 7469 6f6e 203d 205b 2262 7569 6c64 5b76  tion = ["build[v
+0001eb30: 6972 7475 616c 656e 765d 222c 2022 6669  irtualenv]", "fi
+0001eb40: 6c65 6c6f 636b 2028 3e3d 332e 342e 3029  lelock (>=3.4.0)
+0001eb50: 222c 2022 6a61 7261 636f 2e65 6e76 7320  ", "jaraco.envs 
+0001eb60: 283e 3d32 2e32 2922 2c20 226a 6172 6163  (>=2.2)", "jarac
+0001eb70: 6f2e 7061 7468 2028 3e3d 332e 322e 3029  o.path (>=3.2.0)
+0001eb80: 222c 2022 7079 7465 7374 222c 2022 7079  ", "pytest", "py
+0001eb90: 7465 7374 2d65 6e61 626c 6572 222c 2022  test-enabler", "
+0001eba0: 7079 7465 7374 2d78 6469 7374 222c 2022  pytest-xdist", "
+0001ebb0: 746f 6d6c 6922 2c20 2276 6972 7475 616c  tomli", "virtual
+0001ebc0: 656e 7620 283e 3d31 332e 302e 3029 222c  env (>=13.0.0)",
+0001ebd0: 2022 7768 6565 6c22 5d0a 0a5b 5b70 6163   "wheel"]..[[pac
+0001ebe0: 6b61 6765 5d5d 0a6e 616d 6520 3d20 2273  kage]].name = "s
+0001ebf0: 6822 0a76 6572 7369 6f6e 203d 2022 322e  h".version = "2.
+0001ec00: 302e 3422 0a64 6573 6372 6970 7469 6f6e  0.4".description
+0001ec10: 203d 2022 5079 7468 6f6e 2073 7562 7072   = "Python subpr
+0001ec20: 6f63 6573 7320 7265 706c 6163 656d 656e  ocess replacemen
+0001ec30: 7422 0a6f 7074 696f 6e61 6c20 3d20 6661  t".optional = fa
+0001ec40: 6c73 650a 7079 7468 6f6e 2d76 6572 7369  lse.python-versi
+0001ec50: 6f6e 7320 3d20 223e 3d33 2e38 2e31 2c3c  ons = ">=3.8.1,<
+0001ec60: 342e 3022 0a66 696c 6573 203d 205b 0a20  4.0".files = [. 
+0001ec70: 2020 207b 6669 6c65 203d 2022 7368 2d32     {file = "sh-2
+0001ec80: 2e30 2e34 2d70 7933 2d6e 6f6e 652d 616e  .0.4-py3-none-an
+0001ec90: 792e 7768 6c22 2c20 6861 7368 203d 2022  y.whl", hash = "
+0001eca0: 7368 6132 3536 3a31 3432 3635 6134 6364  sha256:14265a4cd
+0001ecb0: 3136 3232 3432 3965 6463 6633 3030 3239  1622429edcf30029
+0001ecc0: 3265 6339 3831 3933 3533 3066 6231 3433  2ec98193530fb143
+0001ecd0: 6665 3634 3262 3334 3337 3032 3465 6361  fe642b3437024eca
+0001ece0: 3962 6565 3863 3522 7d2c 0a20 2020 207b  9bee8c5"},.    {
+0001ecf0: 6669 6c65 203d 2022 7368 2d32 2e30 2e34  file = "sh-2.0.4
+0001ed00: 2e74 6172 2e67 7a22 2c20 6861 7368 203d  .tar.gz", hash =
+0001ed10: 2022 7368 6132 3536 3a61 3138 3932 3066   "sha256:a18920f
+0001ed20: 3038 3339 3939 3162 6339 6466 6464 6236  0839991bc9dfddb6
+0001ed30: 6463 6330 3036 6333 3630 6231 3036 3462  dcc006c360b1064b
+0001ed40: 6139 3632 3537 3335 3966 3065 6133 3536  a96257359f0ea356
+0001ed50: 6539 6661 3735 6136 3022 7d2c 0a5d 0a0a  e9fa75a60"},.]..
+0001ed60: 5b5b 7061 636b 6167 655d 5d0a 6e61 6d65  [[package]].name
+0001ed70: 203d 2022 7369 7822 0a76 6572 7369 6f6e   = "six".version
+0001ed80: 203d 2022 312e 3136 2e30 220a 6465 7363   = "1.16.0".desc
+0001ed90: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
+0001eda0: 6e20 3220 616e 6420 3320 636f 6d70 6174  n 2 and 3 compat
+0001edb0: 6962 696c 6974 7920 7574 696c 6974 6965  ibility utilitie
+0001edc0: 7322 0a6f 7074 696f 6e61 6c20 3d20 6661  s".optional = fa
+0001edd0: 6c73 650a 7079 7468 6f6e 2d76 6572 7369  lse.python-versi
+0001ede0: 6f6e 7320 3d20 223e 3d32 2e37 2c20 213d  ons = ">=2.7, !=
+0001edf0: 332e 302e 2a2c 2021 3d33 2e31 2e2a 2c20  3.0.*, !=3.1.*, 
+0001ee00: 213d 332e 322e 2a22 0a66 696c 6573 203d  !=3.2.*".files =
+0001ee10: 205b 0a20 2020 207b 6669 6c65 203d 2022   [.    {file = "
+0001ee20: 7369 782d 312e 3136 2e30 2d70 7932 2e70  six-1.16.0-py2.p
+0001ee30: 7933 2d6e 6f6e 652d 616e 792e 7768 6c22  y3-none-any.whl"
+0001ee40: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+0001ee50: 3a38 6162 6232 6631 6438 3638 3930 6132  :8abb2f1d86890a2
+0001ee60: 6466 6239 3839 6639 6137 3763 6663 6664  dfb989f9a77cfcfd
+0001ee70: 3365 3437 6332 6133 3534 6230 3131 3131  3e47c2a354b01111
+0001ee80: 3737 3133 3236 6638 6161 3236 6530 3235  771326f8aa26e025
+0001ee90: 3422 7d2c 0a20 2020 207b 6669 6c65 203d  4"},.    {file =
+0001eea0: 2022 7369 782d 312e 3136 2e30 2e74 6172   "six-1.16.0.tar
+0001eeb0: 2e67 7a22 2c20 6861 7368 203d 2022 7368  .gz", hash = "sh
+0001eec0: 6132 3536 3a31 6536 3163 3337 3437 3761  a256:1e61c37477a
+0001eed0: 3136 3236 3435 3865 3336 6637 6231 6438  1626458e36f7b1d8
+0001eee0: 3261 6135 6339 6230 3934 6661 3438 3032  2aa5c9b094fa4802
+0001eef0: 3839 3230 3732 6534 3964 6539 6336 3063  892072e49de9c60c
+0001ef00: 3463 3932 3622 7d2c 0a5d 0a0a 5b5b 7061  4c926"},.]..[[pa
+0001ef10: 636b 6167 655d 5d0a 6e61 6d65 203d 2022  ckage]].name = "
+0001ef20: 736f 7570 7369 6576 6522 0a76 6572 7369  soupsieve".versi
+0001ef30: 6f6e 203d 2022 322e 342e 3122 0a64 6573  on = "2.4.1".des
+0001ef40: 6372 6970 7469 6f6e 203d 2022 4120 6d6f  cription = "A mo
+0001ef50: 6465 726e 2043 5353 2073 656c 6563 746f  dern CSS selecto
+0001ef60: 7220 696d 706c 656d 656e 7461 7469 6f6e  r implementation
+0001ef70: 2066 6f72 2042 6561 7574 6966 756c 2053   for Beautiful S
+0001ef80: 6f75 702e 220a 6f70 7469 6f6e 616c 203d  oup.".optional =
+0001ef90: 2066 616c 7365 0a70 7974 686f 6e2d 7665   false.python-ve
+0001efa0: 7273 696f 6e73 203d 2022 3e3d 332e 3722  rsions = ">=3.7"
+0001efb0: 0a66 696c 6573 203d 205b 0a20 2020 207b  .files = [.    {
+0001efc0: 6669 6c65 203d 2022 736f 7570 7369 6576  file = "soupsiev
+0001efd0: 652d 322e 342e 312d 7079 332d 6e6f 6e65  e-2.4.1-py3-none
+0001efe0: 2d61 6e79 2e77 686c 222c 2068 6173 6820  -any.whl", hash 
+0001eff0: 3d20 2273 6861 3235 363a 3163 3162 6665  = "sha256:1c1bfe
+0001f000: 6536 3831 3935 3434 6133 3434 3735 3836  e6819544a3447586
+0001f010: 6338 3839 3135 3733 3635 6132 3765 3130  c889157365a27e10
+0001f020: 6438 3863 6465 3361 6433 6461 3063 6630  d88cde3ad3da0cf0
+0001f030: 6464 6636 3436 6665 6238 227d 2c0a 2020  ddf646feb8"},.  
+0001f040: 2020 7b66 696c 6520 3d20 2273 6f75 7073    {file = "soups
+0001f050: 6965 7665 2d32 2e34 2e31 2e74 6172 2e67  ieve-2.4.1.tar.g
+0001f060: 7a22 2c20 6861 7368 203d 2022 7368 6132  z", hash = "sha2
+0001f070: 3536 3a38 3964 3132 6232 6435 6466 6364  56:89d12b2d5dfcd
+0001f080: 3263 3965 3863 3232 3332 3664 6139 6439  2c9e8c22326da9d9
+0001f090: 6161 3963 6233 6466 6162 3061 3833 6130  aa9cb3dfab0a83a0
+0001f0a0: 3234 6630 3537 3034 3037 3665 6538 6433  24f05704076ee8d3
+0001f0b0: 3565 6122 7d2c 0a5d 0a0a 5b5b 7061 636b  5ea"},.]..[[pack
+0001f0c0: 6167 655d 5d0a 6e61 6d65 203d 2022 7465  age]].name = "te
+0001f0d0: 726d 636f 6c6f 7222 0a76 6572 7369 6f6e  rmcolor".version
+0001f0e0: 203d 2022 322e 332e 3022 0a64 6573 6372   = "2.3.0".descr
+0001f0f0: 6970 7469 6f6e 203d 2022 414e 5349 2063  iption = "ANSI c
+0001f100: 6f6c 6f72 2066 6f72 6d61 7474 696e 6720  olor formatting 
+0001f110: 666f 7220 6f75 7470 7574 2069 6e20 7465  for output in te
+0001f120: 726d 696e 616c 220a 6f70 7469 6f6e 616c  rminal".optional
+0001f130: 203d 2066 616c 7365 0a70 7974 686f 6e2d   = false.python-
+0001f140: 7665 7273 696f 6e73 203d 2022 3e3d 332e  versions = ">=3.
+0001f150: 3722 0a66 696c 6573 203d 205b 0a20 2020  7".files = [.   
+0001f160: 207b 6669 6c65 203d 2022 7465 726d 636f   {file = "termco
+0001f170: 6c6f 722d 322e 332e 302d 7079 332d 6e6f  lor-2.3.0-py3-no
+0001f180: 6e65 2d61 6e79 2e77 686c 222c 2068 6173  ne-any.whl", has
+0001f190: 6820 3d20 2273 6861 3235 363a 3361 6662  h = "sha256:3afb
+0001f1a0: 3035 3630 3762 3839 6165 6430 6666 6532  05607b89aed0ffe2
+0001f1b0: 3532 3032 3339 3965 6530 3836 3761 6434  5202399ee0867ad4
+0001f1c0: 6433 6362 3431 3830 6439 3861 6166 3865  d3cb4180d98aaf8e
+0001f1d0: 6566 6136 6135 6637 6434 3735 227d 2c0a  efa6a5f7d475"},.
+0001f1e0: 2020 2020 7b66 696c 6520 3d20 2274 6572      {file = "ter
+0001f1f0: 6d63 6f6c 6f72 2d32 2e33 2e30 2e74 6172  mcolor-2.3.0.tar
+0001f200: 2e67 7a22 2c20 6861 7368 203d 2022 7368  .gz", hash = "sh
+0001f210: 6132 3536 3a62 3562 3038 6636 3839 3337  a256:b5b08f68937
+0001f220: 6631 3338 6665 3932 6636 6330 3839 6239  f138fe92f6c089b9
+0001f230: 3966 3165 3264 6130 6165 3536 6335 3262  9f1e2da0ae56c52b
+0001f240: 3738 6266 3730 3735 6664 3935 3432 3066  78bf7075fd95420f
+0001f250: 6439 6135 6122 7d2c 0a5d 0a0a 5b70 6163  d9a5a"},.]..[pac
+0001f260: 6b61 6765 2e65 7874 7261 735d 0a74 6573  kage.extras].tes
+0001f270: 7473 203d 205b 2270 7974 6573 7422 2c20  ts = ["pytest", 
+0001f280: 2270 7974 6573 742d 636f 7622 5d0a 0a5b  "pytest-cov"]..[
+0001f290: 5b70 6163 6b61 6765 5d5d 0a6e 616d 6520  [package]].name 
+0001f2a0: 3d20 2274 696e 7963 7373 3222 0a76 6572  = "tinycss2".ver
+0001f2b0: 7369 6f6e 203d 2022 312e 322e 3122 0a64  sion = "1.2.1".d
+0001f2c0: 6573 6372 6970 7469 6f6e 203d 2022 4120  escription = "A 
+0001f2d0: 7469 6e79 2043 5353 2070 6172 7365 7222  tiny CSS parser"
+0001f2e0: 0a6f 7074 696f 6e61 6c20 3d20 6661 6c73  .optional = fals
+0001f2f0: 650a 7079 7468 6f6e 2d76 6572 7369 6f6e  e.python-version
+0001f300: 7320 3d20 223e 3d33 2e37 220a 6669 6c65  s = ">=3.7".file
+0001f310: 7320 3d20 5b0a 2020 2020 7b66 696c 6520  s = [.    {file 
+0001f320: 3d20 2274 696e 7963 7373 322d 312e 322e  = "tinycss2-1.2.
+0001f330: 312d 7079 332d 6e6f 6e65 2d61 6e79 2e77  1-py3-none-any.w
+0001f340: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+0001f350: 3235 363a 3262 3830 6139 3664 3431 6537  256:2b80a96d41e7
+0001f360: 6333 3931 3462 3863 6461 3862 6337 6637  c3914b8cda8bc7f7
+0001f370: 3035 6134 6439 6334 3932 3735 3631 3665  05a4d9c49275616e
+0001f380: 3838 3631 3033 6464 3833 3964 6663 3834  886103dd839dfc84
+0001f390: 3738 3437 227d 2c0a 2020 2020 7b66 696c  7847"},.    {fil
+0001f3a0: 6520 3d20 2274 696e 7963 7373 322d 312e  e = "tinycss2-1.
+0001f3b0: 322e 312e 7461 722e 677a 222c 2068 6173  2.1.tar.gz", has
+0001f3c0: 6820 3d20 2273 6861 3235 363a 3863 6666  h = "sha256:8cff
+0001f3d0: 3361 3866 3036 3663 3265 6336 3737 6330  3a8f066c2ec677c0
+0001f3e0: 3664 6263 3762 3435 3631 3938 3034 6136  6dbc7b45619804a6
+0001f3f0: 3933 3834 3738 6439 6437 3363 3238 3462  938478d9d73c284b
+0001f400: 3239 6431 3465 6362 3036 3237 227d 2c0a  29d14ecb0627"},.
+0001f410: 5d0a 0a5b 7061 636b 6167 652e 6465 7065  ]..[package.depe
+0001f420: 6e64 656e 6369 6573 5d0a 7765 6265 6e63  ndencies].webenc
+0001f430: 6f64 696e 6773 203d 2022 3e3d 302e 3422  odings = ">=0.4"
+0001f440: 0a0a 5b70 6163 6b61 6765 2e65 7874 7261  ..[package.extra
+0001f450: 735d 0a64 6f63 203d 205b 2273 7068 696e  s].doc = ["sphin
+0001f460: 7822 2c20 2273 7068 696e 785f 7274 645f  x", "sphinx_rtd_
+0001f470: 7468 656d 6522 5d0a 7465 7374 203d 205b  theme"].test = [
+0001f480: 2266 6c61 6b65 3822 2c20 2269 736f 7274  "flake8", "isort
+0001f490: 222c 2022 7079 7465 7374 225d 0a0a 5b5b  ", "pytest"]..[[
+0001f4a0: 7061 636b 6167 655d 5d0a 6e61 6d65 203d  package]].name =
+0001f4b0: 2022 746f 6d6c 220a 7665 7273 696f 6e20   "toml".version 
+0001f4c0: 3d20 2230 2e31 302e 3222 0a64 6573 6372  = "0.10.2".descr
+0001f4d0: 6970 7469 6f6e 203d 2022 5079 7468 6f6e  iption = "Python
+0001f4e0: 204c 6962 7261 7279 2066 6f72 2054 6f6d   Library for Tom
+0001f4f0: 2773 204f 6276 696f 7573 2c20 4d69 6e69  's Obvious, Mini
+0001f500: 6d61 6c20 4c61 6e67 7561 6765 220a 6f70  mal Language".op
+0001f510: 7469 6f6e 616c 203d 2066 616c 7365 0a70  tional = false.p
+0001f520: 7974 686f 6e2d 7665 7273 696f 6e73 203d  ython-versions =
+0001f530: 2022 3e3d 322e 362c 2021 3d33 2e30 2e2a   ">=2.6, !=3.0.*
+0001f540: 2c20 213d 332e 312e 2a2c 2021 3d33 2e32  , !=3.1.*, !=3.2
+0001f550: 2e2a 220a 6669 6c65 7320 3d20 5b0a 2020  .*".files = [.  
+0001f560: 2020 7b66 696c 6520 3d20 2274 6f6d 6c2d    {file = "toml-
+0001f570: 302e 3130 2e32 2d70 7932 2e70 7933 2d6e  0.10.2-py2.py3-n
+0001f580: 6f6e 652d 616e 792e 7768 6c22 2c20 6861  one-any.whl", ha
+0001f590: 7368 203d 2022 7368 6132 3536 3a38 3036  sh = "sha256:806
+0001f5a0: 3134 3361 6535 6266 6236 6133 6336 6537  143ae5bfb6a3c6e7
+0001f5b0: 3336 6137 3634 3035 3764 6230 6536 6130  36a764057db0e6a0
+0001f5c0: 6530 3565 3333 3862 3536 3330 3839 3461  e05e338b5630894a
+0001f5d0: 3566 3737 3963 6162 6234 6639 6222 7d2c  5f779cabb4f9b"},
+0001f5e0: 0a20 2020 207b 6669 6c65 203d 2022 746f  .    {file = "to
+0001f5f0: 6d6c 2d30 2e31 302e 322e 7461 722e 677a  ml-0.10.2.tar.gz
+0001f600: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001f610: 363a 6233 6264 6131 6431 3038 6435 6464  6:b3bda1d108d5dd
+0001f620: 3939 6634 6132 3064 3234 6439 6333 3438  99f4a20d24d9c348
+0001f630: 6539 3163 3464 6237 6162 3162 3734 3932  e91c4db7ab1b7492
+0001f640: 3030 6264 6564 3266 3833 3963 6362 6536  00bded2f839ccbe6
+0001f650: 3866 227d 2c0a 5d0a 0a5b 5b70 6163 6b61  8f"},.]..[[packa
+0001f660: 6765 5d5d 0a6e 616d 6520 3d20 2274 6f6d  ge]].name = "tom
+0001f670: 6c69 220a 7665 7273 696f 6e20 3d20 2232  li".version = "2
+0001f680: 2e30 2e31 220a 6465 7363 7269 7074 696f  .0.1".descriptio
+0001f690: 6e20 3d20 2241 206c 696c 2720 544f 4d4c  n = "A lil' TOML
+0001f6a0: 2070 6172 7365 7222 0a6f 7074 696f 6e61   parser".optiona
+0001f6b0: 6c20 3d20 6661 6c73 650a 7079 7468 6f6e  l = false.python
+0001f6c0: 2d76 6572 7369 6f6e 7320 3d20 223e 3d33  -versions = ">=3
+0001f6d0: 2e37 220a 6669 6c65 7320 3d20 5b0a 2020  .7".files = [.  
+0001f6e0: 2020 7b66 696c 6520 3d20 2274 6f6d 6c69    {file = "tomli
+0001f6f0: 2d32 2e30 2e31 2d70 7933 2d6e 6f6e 652d  -2.0.1-py3-none-
+0001f700: 616e 792e 7768 6c22 2c20 6861 7368 203d  any.whl", hash =
+0001f710: 2022 7368 6132 3536 3a39 3339 6465 3365   "sha256:939de3e
+0001f720: 3761 3631 3631 6166 3063 3838 3765 6639  7a6161af0c887ef9
+0001f730: 3162 3764 3431 6135 3365 3763 3561 3163  1b7d41a53e7c5a1c
+0001f740: 6139 3736 3332 3566 3432 3963 6234 3665  a976325f429cb46e
+0001f750: 6139 6263 3330 6563 6322 7d2c 0a20 2020  a9bc30ecc"},.   
+0001f760: 207b 6669 6c65 203d 2022 746f 6d6c 692d   {file = "tomli-
+0001f770: 322e 302e 312e 7461 722e 677a 222c 2068  2.0.1.tar.gz", h
+0001f780: 6173 6820 3d20 2273 6861 3235 363a 6465  ash = "sha256:de
+0001f790: 3532 3663 3132 3931 3466 3063 3535 3064  526c12914f0c550d
+0001f7a0: 3135 3932 3463 3632 6437 3261 6263 3438  15924c62d72abc48
+0001f7b0: 6436 6665 3733 3634 6161 3837 3332 3833  d6fe7364aa873283
+0001f7c0: 3337 6133 3130 3037 6665 3861 3466 227d  37a31007fe8a4f"}
+0001f7d0: 2c0a 5d0a 0a5b 5b70 6163 6b61 6765 5d5d  ,.]..[[package]]
+0001f7e0: 0a6e 616d 6520 3d20 2274 6f72 6e61 646f  .name = "tornado
+0001f7f0: 220a 7665 7273 696f 6e20 3d20 2236 2e33  ".version = "6.3
+0001f800: 2e32 220a 6465 7363 7269 7074 696f 6e20  .2".description 
+0001f810: 3d20 2254 6f72 6e61 646f 2069 7320 6120  = "Tornado is a 
+0001f820: 5079 7468 6f6e 2077 6562 2066 7261 6d65  Python web frame
+0001f830: 776f 726b 2061 6e64 2061 7379 6e63 6872  work and asynchr
+0001f840: 6f6e 6f75 7320 6e65 7477 6f72 6b69 6e67  onous networking
+0001f850: 206c 6962 7261 7279 2c20 6f72 6967 696e   library, origin
+0001f860: 616c 6c79 2064 6576 656c 6f70 6564 2061  ally developed a
+0001f870: 7420 4672 6965 6e64 4665 6564 2e22 0a6f  t FriendFeed.".o
+0001f880: 7074 696f 6e61 6c20 3d20 6661 6c73 650a  ptional = false.
+0001f890: 7079 7468 6f6e 2d76 6572 7369 6f6e 7320  python-versions 
+0001f8a0: 3d20 223e 3d20 332e 3822 0a66 696c 6573  = ">= 3.8".files
+0001f8b0: 203d 205b 0a20 2020 207b 6669 6c65 203d   = [.    {file =
+0001f8c0: 2022 746f 726e 6164 6f2d 362e 332e 322d   "tornado-6.3.2-
+0001f8d0: 6370 3338 2d61 6269 332d 6d61 636f 7378  cp38-abi3-macosx
+0001f8e0: 5f31 305f 395f 756e 6976 6572 7361 6c32  _10_9_universal2
+0001f8f0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001f900: 6861 3235 363a 6333 3637 6162 3663 3033  ha256:c367ab6c03
+0001f910: 3933 6437 3131 3731 3132 3363 6135 3531  93d71171123ca551
+0001f920: 3563 3631 6666 3632 6665 3039 3032 3466  5c61ff62fe09024f
+0001f930: 6136 6266 3239 3963 6431 3333 3964 6339  a6bf299cd1339dc9
+0001f940: 3435 3638 3239 227d 2c0a 2020 2020 7b66  456829"},.    {f
+0001f950: 696c 6520 3d20 2274 6f72 6e61 646f 2d36  ile = "tornado-6
+0001f960: 2e33 2e32 2d63 7033 382d 6162 6933 2d6d  .3.2-cp38-abi3-m
+0001f970: 6163 6f73 785f 3130 5f39 5f78 3836 5f36  acosx_10_9_x86_6
+0001f980: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+0001f990: 7368 6132 3536 3a62 3436 6136 6162 3230  sha256:b46a6ab20
+0001f9a0: 6635 6337 6331 6362 3934 3963 3732 6331  f5c7c1cb949c72c1
+0001f9b0: 3939 3461 3435 3835 6432 6561 6130 6265  994a4585d2eaa0be
+0001f9c0: 3438 3533 6635 3061 3033 6235 3033 3165  4853f50a03b5031e
+0001f9d0: 3936 3466 6337 6322 7d2c 0a20 2020 207b  964fc7c"},.    {
+0001f9e0: 6669 6c65 203d 2022 746f 726e 6164 6f2d  file = "tornado-
+0001f9f0: 362e 332e 322d 6370 3338 2d61 6269 332d  6.3.2-cp38-abi3-
+0001fa00: 6d61 6e79 6c69 6e75 785f 325f 3137 5f61  manylinux_2_17_a
+0001fa10: 6172 6368 3634 2e6d 616e 796c 696e 7578  arch64.manylinux
+0001fa20: 3230 3134 5f61 6172 6368 3634 2e77 686c  2014_aarch64.whl
+0001fa30: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001fa40: 363a 6332 6465 3134 3036 3663 3461 3338  6:c2de14066c4a38
+0001fa50: 6234 6563 6262 6364 3535 6335 6363 3462  b4ecbbcd55c5cc4b
+0001fa60: 3533 3430 6562 3034 6631 6335 6538 3164  5340eb04f1c5e81d
+0001fa70: 6137 3435 3165 6635 3535 3835 3963 3833  a7451ef555859c83
+0001fa80: 3366 227d 2c0a 2020 2020 7b66 696c 6520  3f"},.    {file 
+0001fa90: 3d20 2274 6f72 6e61 646f 2d36 2e33 2e32  = "tornado-6.3.2
+0001faa0: 2d63 7033 382d 6162 6933 2d6d 616e 796c  -cp38-abi3-manyl
+0001fab0: 696e 7578 5f32 5f35 5f69 3638 362e 6d61  inux_2_5_i686.ma
+0001fac0: 6e79 6c69 6e75 7831 5f69 3638 362e 6d61  nylinux1_i686.ma
+0001fad0: 6e79 6c69 6e75 785f 325f 3137 5f69 3638  nylinux_2_17_i68
+0001fae0: 362e 6d61 6e79 6c69 6e75 7832 3031 345f  6.manylinux2014_
+0001faf0: 6936 3836 2e77 686c 222c 2068 6173 6820  i686.whl", hash 
+0001fb00: 3d20 2273 6861 3235 363a 3035 3631 3530  = "sha256:056150
+0001fb10: 3936 3834 3563 6635 3061 3839 3530 3236  96845cf50a895026
+0001fb20: 6637 3439 3139 3562 6630 6231 3062 3839  f749195bf0b10b89
+0001fb30: 3039 6639 6265 3637 3266 3530 6230 6665  09f9be672f50b0fe
+0001fb40: 3639 6362 6133 3638 6534 227d 2c0a 2020  69cba368e4"},.  
+0001fb50: 2020 7b66 696c 6520 3d20 2274 6f72 6e61    {file = "torna
+0001fb60: 646f 2d36 2e33 2e32 2d63 7033 382d 6162  do-6.3.2-cp38-ab
+0001fb70: 6933 2d6d 616e 796c 696e 7578 5f32 5f35  i3-manylinux_2_5
+0001fb80: 5f78 3836 5f36 342e 6d61 6e79 6c69 6e75  _x86_64.manylinu
+0001fb90: 7831 5f78 3836 5f36 342e 6d61 6e79 6c69  x1_x86_64.manyli
+0001fba0: 6e75 785f 325f 3137 5f78 3836 5f36 342e  nux_2_17_x86_64.
+0001fbb0: 6d61 6e79 6c69 6e75 7832 3031 345f 7838  manylinux2014_x8
+0001fbc0: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
+0001fbd0: 3d20 2273 6861 3235 363a 3562 3137 6231  = "sha256:5b17b1
+0001fbe0: 6366 3566 3833 3534 6566 6133 6433 3763  cf5f8354efa3d37c
+0001fbf0: 3665 3238 6664 6664 3963 3163 3165 3531  6e28fdfd9c1c1e51
+0001fc00: 3232 6632 6362 3536 6461 6331 3231 6163  22f2cb56dac121ac
+0001fc10: 3631 6261 6134 3763 6265 227d 2c0a 2020  61baa47cbe"},.  
+0001fc20: 2020 7b66 696c 6520 3d20 2274 6f72 6e61    {file = "torna
+0001fc30: 646f 2d36 2e33 2e32 2d63 7033 382d 6162  do-6.3.2-cp38-ab
+0001fc40: 6933 2d6d 7573 6c6c 696e 7578 5f31 5f31  i3-musllinux_1_1
+0001fc50: 5f61 6172 6368 3634 2e77 686c 222c 2068  _aarch64.whl", h
+0001fc60: 6173 6820 3d20 2273 6861 3235 363a 3239  ash = "sha256:29
+0001fc70: 6537 3163 3834 3761 3335 6636 6531 3063  e71c847a35f6e10c
+0001fc80: 6133 6235 6332 3939 3061 3532 6365 3338  a3b5c2990a52ce38
+0001fc90: 6232 3333 3031 3964 3865 3835 3862 3735  b233019d8e858b75
+0001fca0: 3565 6136 6365 3464 6364 6431 3964 227d  5ea6ce4dcdd19d"}
+0001fcb0: 2c0a 2020 2020 7b66 696c 6520 3d20 2274  ,.    {file = "t
+0001fcc0: 6f72 6e61 646f 2d36 2e33 2e32 2d63 7033  ornado-6.3.2-cp3
+0001fcd0: 382d 6162 6933 2d6d 7573 6c6c 696e 7578  8-abi3-musllinux
+0001fce0: 5f31 5f31 5f69 3638 362e 7768 6c22 2c20  _1_1_i686.whl", 
+0001fcf0: 6861 7368 203d 2022 7368 6132 3536 3a38  hash = "sha256:8
+0001fd00: 3334 6165 3735 3430 6164 3361 3833 3139  34ae7540ad3a8319
+0001fd10: 3961 3864 6138 6639 6632 6433 3833 6533  9a8da8f9f2d383e3
+0001fd20: 6333 6435 3133 3061 3332 3838 3839 6534  c3d5130a328889e4
+0001fd30: 6363 3939 3161 6363 3831 6538 3761 3022  cc991acc81e87a0"
+0001fd40: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+0001fd50: 746f 726e 6164 6f2d 362e 332e 322d 6370  tornado-6.3.2-cp
+0001fd60: 3338 2d61 6269 332d 6d75 736c 6c69 6e75  38-abi3-musllinu
+0001fd70: 785f 315f 315f 7838 365f 3634 2e77 686c  x_1_1_x86_64.whl
+0001fd80: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+0001fd90: 363a 3661 3038 3438 6631 6165 6130 6431  6:6a0848f1aea0d1
+0001fda0: 3936 6137 6334 6636 3737 3231 3937 6362  96a7c4f6772197cb
+0001fdb0: 6532 6162 6334 3236 3666 3833 3662 3061  e2abc4266f836b0a
+0001fdc0: 6163 3736 3934 3738 3732 6364 3239 6234  ac76947872cd29b4
+0001fdd0: 3131 227d 2c0a 2020 2020 7b66 696c 6520  11"},.    {file 
+0001fde0: 3d20 2274 6f72 6e61 646f 2d36 2e33 2e32  = "tornado-6.3.2
+0001fdf0: 2d63 7033 382d 6162 6933 2d77 696e 3332  -cp38-abi3-win32
+0001fe00: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+0001fe10: 6861 3235 363a 3765 6663 6263 6333 3062  ha256:7efcbcc30b
+0001fe20: 3763 3635 3465 6236 6138 6339 6339 6461  7c654eb6a8c9c9da
+0001fe30: 3738 3761 3835 3163 3138 6638 6363 6434  787a851c18f8ccd4
+0001fe40: 6135 6133 6139 3562 3035 6337 6163 6366  a5a3a95b05c7accf
+0001fe50: 6130 3638 6432 227d 2c0a 2020 2020 7b66  a068d2"},.    {f
+0001fe60: 696c 6520 3d20 2274 6f72 6e61 646f 2d36  ile = "tornado-6
+0001fe70: 2e33 2e32 2d63 7033 382d 6162 6933 2d77  .3.2-cp38-abi3-w
+0001fe80: 696e 5f61 6d64 3634 2e77 686c 222c 2068  in_amd64.whl", h
+0001fe90: 6173 6820 3d20 2273 6861 3235 363a 3063  ash = "sha256:0c
+0001fea0: 3332 3565 3636 6338 3132 3363 3630 3665  325e66c8123c606e
+0001feb0: 6561 3333 3038 3439 3736 6338 3332 6161  ea33084976c832aa
+0001fec0: 3465 3736 3662 3764 6666 3861 6564 6437  4e766b7dff8aedd7
+0001fed0: 3538 3765 6134 3461 3630 3463 6466 227d  587ea44a604cdf"}
+0001fee0: 2c0a 2020 2020 7b66 696c 6520 3d20 2274  ,.    {file = "t
+0001fef0: 6f72 6e61 646f 2d36 2e33 2e32 2e74 6172  ornado-6.3.2.tar
+0001ff00: 2e67 7a22 2c20 6861 7368 203d 2022 7368  .gz", hash = "sh
+0001ff10: 6132 3536 3a34 6239 3237 6334 6631 3962  a256:4b927c4f19b
+0001ff20: 3731 6536 3237 6231 3366 3364 6232 3332  71e627b13f3db232
+0001ff30: 3465 3461 6536 3630 3532 3731 3433 6639  4e4ae660527143f9
+0001ff40: 6531 6632 6532 6662 3430 3466 3361 3138  e1f2e2fb404f3a18
+0001ff50: 3765 3262 6122 7d2c 0a5d 0a0a 5b5b 7061  7e2ba"},.]..[[pa
+0001ff60: 636b 6167 655d 5d0a 6e61 6d65 203d 2022  ckage]].name = "
+0001ff70: 7472 6169 746c 6574 7322 0a76 6572 7369  traitlets".versi
+0001ff80: 6f6e 203d 2022 352e 392e 3022 0a64 6573  on = "5.9.0".des
+0001ff90: 6372 6970 7469 6f6e 203d 2022 5472 6169  cription = "Trai
+0001ffa0: 746c 6574 7320 5079 7468 6f6e 2063 6f6e  tlets Python con
+0001ffb0: 6669 6775 7261 7469 6f6e 2073 7973 7465  figuration syste
+0001ffc0: 6d22 0a6f 7074 696f 6e61 6c20 3d20 6661  m".optional = fa
+0001ffd0: 6c73 650a 7079 7468 6f6e 2d76 6572 7369  lse.python-versi
+0001ffe0: 6f6e 7320 3d20 223e 3d33 2e37 220a 6669  ons = ">=3.7".fi
+0001fff0: 6c65 7320 3d20 5b0a 2020 2020 7b66 696c  les = [.    {fil
+00020000: 6520 3d20 2274 7261 6974 6c65 7473 2d35  e = "traitlets-5
+00020010: 2e39 2e30 2d70 7933 2d6e 6f6e 652d 616e  .9.0-py3-none-an
+00020020: 792e 7768 6c22 2c20 6861 7368 203d 2022  y.whl", hash = "
+00020030: 7368 6132 3536 3a39 6536 6563 3038 3032  sha256:9e6ec0802
+00020040: 3539 6239 6135 3934 3063 3739 3764 3538  59b9a5940c797d58
+00020050: 6236 3133 6235 6533 3134 3431 6332 3235  b613b5e31441c225
+00020060: 3762 3837 6332 6537 3935 6335 3232 3861  7b87c2e795c5228a
+00020070: 6538 3064 3264 3822 7d2c 0a20 2020 207b  e80d2d8"},.    {
+00020080: 6669 6c65 203d 2022 7472 6169 746c 6574  file = "traitlet
+00020090: 732d 352e 392e 302e 7461 722e 677a 222c  s-5.9.0.tar.gz",
+000200a0: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
+000200b0: 6636 6364 6532 3161 3963 3638 6366 3735  f6cde21a9c68cf75
+000200c0: 3661 6630 3230 3335 6637 3264 3561 3732  6af02035f72d5a72
+000200d0: 3362 6636 3037 6538 3632 6537 6265 3333  3bf607e862e7be33
+000200e0: 6563 6535 3035 6162 6634 6133 6261 6439  ece505abf4a3bad9
+000200f0: 227d 2c0a 5d0a 0a5b 7061 636b 6167 652e  "},.]..[package.
+00020100: 6578 7472 6173 5d0a 646f 6373 203d 205b  extras].docs = [
+00020110: 226d 7973 742d 7061 7273 6572 222c 2022  "myst-parser", "
+00020120: 7079 6461 7461 2d73 7068 696e 782d 7468  pydata-sphinx-th
+00020130: 656d 6522 2c20 2273 7068 696e 7822 5d0a  eme", "sphinx"].
+00020140: 7465 7374 203d 205b 2261 7267 636f 6d70  test = ["argcomp
+00020150: 6c65 7465 2028 3e3d 322e 3029 222c 2022  lete (>=2.0)", "
+00020160: 7072 652d 636f 6d6d 6974 222c 2022 7079  pre-commit", "py
+00020170: 7465 7374 222c 2022 7079 7465 7374 2d6d  test", "pytest-m
+00020180: 6f63 6b22 5d0a 0a5b 5b70 6163 6b61 6765  ock"]..[[package
+00020190: 5d5d 0a6e 616d 6520 3d20 2274 7970 6573  ]].name = "types
+000201a0: 2d70 7979 616d 6c22 0a76 6572 7369 6f6e  -pyyaml".version
+000201b0: 203d 2022 362e 302e 3132 2e31 3022 0a64   = "6.0.12.10".d
+000201c0: 6573 6372 6970 7469 6f6e 203d 2022 5479  escription = "Ty
+000201d0: 7069 6e67 2073 7475 6273 2066 6f72 2050  ping stubs for P
+000201e0: 7959 414d 4c22 0a6f 7074 696f 6e61 6c20  yYAML".optional 
+000201f0: 3d20 6661 6c73 650a 7079 7468 6f6e 2d76  = false.python-v
+00020200: 6572 7369 6f6e 7320 3d20 222a 220a 6669  ersions = "*".fi
+00020210: 6c65 7320 3d20 5b0a 2020 2020 7b66 696c  les = [.    {fil
+00020220: 6520 3d20 2274 7970 6573 2d50 7959 414d  e = "types-PyYAM
+00020230: 4c2d 362e 302e 3132 2e31 302e 7461 722e  L-6.0.12.10.tar.
+00020240: 677a 222c 2068 6173 6820 3d20 2273 6861  gz", hash = "sha
+00020250: 3235 363a 6562 6162 3364 3037 3030 6239  256:ebab3d0700b9
+00020260: 3436 3535 3337 3234 6165 3663 6136 3336  46553724ae6ca636
+00020270: 6561 3933 3263 3162 3038 3638 3730 3164  ea932c1b0868701d
+00020280: 3461 6631 3231 3633 3065 3738 6436 3935  4af121630e78d695
+00020290: 6663 3937 227d 2c0a 2020 2020 7b66 696c  fc97"},.    {fil
+000202a0: 6520 3d20 2274 7970 6573 5f50 7959 414d  e = "types_PyYAM
+000202b0: 4c2d 362e 302e 3132 2e31 302d 7079 332d  L-6.0.12.10-py3-
+000202c0: 6e6f 6e65 2d61 6e79 2e77 686c 222c 2068  none-any.whl", h
+000202d0: 6173 6820 3d20 2273 6861 3235 363a 3636  ash = "sha256:66
+000202e0: 3266 6134 3434 3936 3365 6666 3962 3638  2fa444963eff9b68
+000202f0: 3132 3064 3730 6364 6131 6166 3561 3566  120d70cda1af5a5f
+00020300: 3261 6135 3739 3030 3030 3363 3230 3036  2aa57900003c2006
+00020310: 6437 3632 3634 3530 6561 6165 3566 227d  d7626450eaae5f"}
+00020320: 2c0a 5d0a 0a5b 5b70 6163 6b61 6765 5d5d  ,.]..[[package]]
+00020330: 0a6e 616d 6520 3d20 2274 7970 696e 672d  .name = "typing-
+00020340: 6578 7465 6e73 696f 6e73 220a 7665 7273  extensions".vers
+00020350: 696f 6e20 3d20 2234 2e36 2e32 220a 6465  ion = "4.6.2".de
+00020360: 7363 7269 7074 696f 6e20 3d20 2242 6163  scription = "Bac
+00020370: 6b70 6f72 7465 6420 616e 6420 4578 7065  kported and Expe
+00020380: 7269 6d65 6e74 616c 2054 7970 6520 4869  rimental Type Hi
+00020390: 6e74 7320 666f 7220 5079 7468 6f6e 2033  nts for Python 3
+000203a0: 2e37 2b22 0a6f 7074 696f 6e61 6c20 3d20  .7+".optional = 
+000203b0: 6661 6c73 650a 7079 7468 6f6e 2d76 6572  false.python-ver
+000203c0: 7369 6f6e 7320 3d20 223e 3d33 2e37 220a  sions = ">=3.7".
+000203d0: 6669 6c65 7320 3d20 5b0a 2020 2020 7b66  files = [.    {f
+000203e0: 696c 6520 3d20 2274 7970 696e 675f 6578  ile = "typing_ex
+000203f0: 7465 6e73 696f 6e73 2d34 2e36 2e32 2d70  tensions-4.6.2-p
+00020400: 7933 2d6e 6f6e 652d 616e 792e 7768 6c22  y3-none-any.whl"
+00020410: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00020420: 3a33 6138 6233 3666 3133 6464 3566 6463  :3a8b36f13dd5fdc
+00020430: 3564 3162 3136 6665 3331 3766 3536 3638  5d1b16fe317f5668
+00020440: 3534 3564 6537 3766 6130 6238 6530 3230  545de77fa0b8e020
+00020450: 3036 3338 3166 6434 3964 3733 3161 6239  06381fd49d731ab9
+00020460: 3822 7d2c 0a20 2020 207b 6669 6c65 203d  8"},.    {file =
+00020470: 2022 7479 7069 6e67 5f65 7874 656e 7369   "typing_extensi
+00020480: 6f6e 732d 342e 362e 322e 7461 722e 677a  ons-4.6.2.tar.gz
+00020490: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+000204a0: 363a 3036 3030 3632 3434 6337 3061 6338  6:06006244c70ac8
+000204b0: 6565 3833 6661 3832 3832 6362 3138 3866  ee83fa8282cb188f
+000204c0: 3639 3762 3864 6232 3562 6338 6234 6466  697b8db25bc8b4df
+000204d0: 3037 6265 3138 3733 6334 3338 3937 3036  07be1873c4389706
+000204e0: 3063 227d 2c0a 5d0a 0a5b 5b70 6163 6b61  0c"},.]..[[packa
+000204f0: 6765 5d5d 0a6e 616d 6520 3d20 2275 726c  ge]].name = "url
+00020500: 6c69 6233 220a 7665 7273 696f 6e20 3d20  lib3".version = 
+00020510: 2231 2e32 362e 3136 220a 6465 7363 7269  "1.26.16".descri
+00020520: 7074 696f 6e20 3d20 2248 5454 5020 6c69  ption = "HTTP li
+00020530: 6272 6172 7920 7769 7468 2074 6872 6561  brary with threa
+00020540: 642d 7361 6665 2063 6f6e 6e65 6374 696f  d-safe connectio
+00020550: 6e20 706f 6f6c 696e 672c 2066 696c 6520  n pooling, file 
+00020560: 706f 7374 2c20 616e 6420 6d6f 7265 2e22  post, and more."
+00020570: 0a6f 7074 696f 6e61 6c20 3d20 6661 6c73  .optional = fals
+00020580: 650a 7079 7468 6f6e 2d76 6572 7369 6f6e  e.python-version
+00020590: 7320 3d20 223e 3d32 2e37 2c20 213d 332e  s = ">=2.7, !=3.
+000205a0: 302e 2a2c 2021 3d33 2e31 2e2a 2c20 213d  0.*, !=3.1.*, !=
+000205b0: 332e 322e 2a2c 2021 3d33 2e33 2e2a 2c20  3.2.*, !=3.3.*, 
+000205c0: 213d 332e 342e 2a2c 2021 3d33 2e35 2e2a  !=3.4.*, !=3.5.*
+000205d0: 220a 6669 6c65 7320 3d20 5b0a 2020 2020  ".files = [.    
+000205e0: 7b66 696c 6520 3d20 2275 726c 6c69 6233  {file = "urllib3
+000205f0: 2d31 2e32 362e 3136 2d70 7932 2e70 7933  -1.26.16-py2.py3
+00020600: 2d6e 6f6e 652d 616e 792e 7768 6c22 2c20  -none-any.whl", 
+00020610: 6861 7368 203d 2022 7368 6132 3536 3a38  hash = "sha256:8
+00020620: 6433 3661 6661 3736 3136 6438 6162 3731  d36afa7616d8ab71
+00020630: 3436 3038 3431 3162 3461 3362 3133 6535  4608411b4a3b13e5
+00020640: 3866 3436 3361 6565 3531 3930 3234 3537  8f463aee51902457
+00020650: 3865 3036 3265 3134 3164 6365 3230 6622  8e062e141dce20f"
+00020660: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+00020670: 7572 6c6c 6962 332d 312e 3236 2e31 362e  urllib3-1.26.16.
+00020680: 7461 722e 677a 222c 2068 6173 6820 3d20  tar.gz", hash = 
+00020690: 2273 6861 3235 363a 3866 3133 3566 3635  "sha256:8f135f65
+000206a0: 3032 3735 3662 6465 3662 3261 3962 3238  02756bde6b2a9b28
+000206b0: 3938 3964 6635 6662 6538 3763 3939 3730  989df5fbe87c9970
+000206c0: 6365 6361 6136 3930 3431 6564 6363 6537  cecaa69041edcce7
+000206d0: 6630 3538 3962 3134 227d 2c0a 5d0a 0a5b  f0589b14"},.]..[
+000206e0: 7061 636b 6167 652e 6578 7472 6173 5d0a  package.extras].
+000206f0: 6272 6f74 6c69 203d 205b 2262 726f 746c  brotli = ["brotl
+00020700: 6920 283e 3d31 2e30 2e39 2922 2c20 2262  i (>=1.0.9)", "b
+00020710: 726f 746c 6963 6666 6920 283e 3d30 2e38  rotlicffi (>=0.8
+00020720: 2e30 2922 2c20 2262 726f 746c 6970 7920  .0)", "brotlipy 
+00020730: 283e 3d30 2e36 2e30 2922 5d0a 7365 6375  (>=0.6.0)"].secu
+00020740: 7265 203d 205b 2263 6572 7469 6669 222c  re = ["certifi",
+00020750: 2022 6372 7970 746f 6772 6170 6879 2028   "cryptography (
+00020760: 3e3d 312e 332e 3429 222c 2022 6964 6e61  >=1.3.4)", "idna
+00020770: 2028 3e3d 322e 302e 3029 222c 2022 6970   (>=2.0.0)", "ip
+00020780: 6164 6472 6573 7322 2c20 2270 794f 7065  address", "pyOpe
+00020790: 6e53 534c 2028 3e3d 302e 3134 2922 2c20  nSSL (>=0.14)", 
+000207a0: 2275 726c 6c69 6233 2d73 6563 7572 652d  "urllib3-secure-
+000207b0: 6578 7472 6122 5d0a 736f 636b 7320 3d20  extra"].socks = 
+000207c0: 5b22 5079 536f 636b 7320 283e 3d31 2e35  ["PySocks (>=1.5
+000207d0: 2e36 2c21 3d31 2e35 2e37 2c3c 322e 3029  .6,!=1.5.7,<2.0)
+000207e0: 225d 0a0a 5b5b 7061 636b 6167 655d 5d0a  "]..[[package]].
+000207f0: 6e61 6d65 203d 2022 7669 7274 7561 6c65  name = "virtuale
+00020800: 6e76 220a 7665 7273 696f 6e20 3d20 2232  nv".version = "2
+00020810: 302e 3233 2e30 220a 6465 7363 7269 7074  0.23.0".descript
+00020820: 696f 6e20 3d20 2256 6972 7475 616c 2050  ion = "Virtual P
+00020830: 7974 686f 6e20 456e 7669 726f 6e6d 656e  ython Environmen
+00020840: 7420 6275 696c 6465 7222 0a6f 7074 696f  t builder".optio
+00020850: 6e61 6c20 3d20 6661 6c73 650a 7079 7468  nal = false.pyth
+00020860: 6f6e 2d76 6572 7369 6f6e 7320 3d20 223e  on-versions = ">
+00020870: 3d33 2e37 220a 6669 6c65 7320 3d20 5b0a  =3.7".files = [.
+00020880: 2020 2020 7b66 696c 6520 3d20 2276 6972      {file = "vir
+00020890: 7475 616c 656e 762d 3230 2e32 332e 302d  tualenv-20.23.0-
+000208a0: 7079 332d 6e6f 6e65 2d61 6e79 2e77 686c  py3-none-any.whl
+000208b0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+000208c0: 363a 3661 6265 6337 3637 3065 3538 3032  6:6abec7670e5802
+000208d0: 6135 3238 3335 3766 6463 3735 6232 3662  a528357fdc75b26b
+000208e0: 3966 3537 6435 6439 3266 3239 6335 3436  9f57d5d92f29c546
+000208f0: 3262 6130 6662 6534 3566 6561 6363 3638  2ba0fbe45feacc68
+00020900: 3565 227d 2c0a 2020 2020 7b66 696c 6520  5e"},.    {file 
+00020910: 3d20 2276 6972 7475 616c 656e 762d 3230  = "virtualenv-20
+00020920: 2e32 332e 302e 7461 722e 677a 222c 2068  .23.0.tar.gz", h
+00020930: 6173 6820 3d20 2273 6861 3235 363a 6138  ash = "sha256:a8
+00020940: 3563 6161 3535 3463 6564 3063 3061 6662  5caa554ced0c0afb
+00020950: 6430 6436 3338 6537 6532 6437 6235 6639  d0d638e7e2d7b5f9
+00020960: 3264 3233 3437 3864 3035 6431 3761 3736  2d23478d05d17a76
+00020970: 6461 6561 6338 6632 3739 6639 3234 227d  daeac8f279f924"}
+00020980: 2c0a 5d0a 0a5b 7061 636b 6167 652e 6465  ,.]..[package.de
+00020990: 7065 6e64 656e 6369 6573 5d0a 6469 7374  pendencies].dist
+000209a0: 6c69 6220 3d20 223e 3d30 2e33 2e36 2c3c  lib = ">=0.3.6,<
+000209b0: 3122 0a66 696c 656c 6f63 6b20 3d20 223e  1".filelock = ">
+000209c0: 3d33 2e31 312c 3c34 220a 706c 6174 666f  =3.11,<4".platfo
+000209d0: 726d 6469 7273 203d 2022 3e3d 332e 322c  rmdirs = ">=3.2,
+000209e0: 3c34 220a 0a5b 7061 636b 6167 652e 6578  <4"..[package.ex
+000209f0: 7472 6173 5d0a 646f 6373 203d 205b 2266  tras].docs = ["f
+00020a00: 7572 6f20 283e 3d32 3032 332e 332e 3237  uro (>=2023.3.27
+00020a10: 2922 2c20 2270 726f 7365 6c69 6e74 2028  )", "proselint (
+00020a20: 3e3d 302e 3133 2922 2c20 2273 7068 696e  >=0.13)", "sphin
+00020a30: 7820 283e 3d36 2e31 2e33 2922 2c20 2273  x (>=6.1.3)", "s
+00020a40: 7068 696e 782d 6172 6770 6172 7365 2028  phinx-argparse (
+00020a50: 3e3d 302e 3429 222c 2022 7370 6869 6e78  >=0.4)", "sphinx
+00020a60: 636f 6e74 7269 622d 746f 776e 6372 6965  contrib-towncrie
+00020a70: 7220 283e 3d30 2e32 2e31 6130 2922 2c20  r (>=0.2.1a0)", 
+00020a80: 2274 6f77 6e63 7269 6572 2028 3e3d 3232  "towncrier (>=22
+00020a90: 2e31 3229 225d 0a74 6573 7420 3d20 5b22  .12)"].test = ["
+00020aa0: 636f 7664 6566 6175 6c74 7320 283e 3d32  covdefaults (>=2
+00020ab0: 2e33 2922 2c20 2263 6f76 6572 6167 6520  .3)", "coverage 
+00020ac0: 283e 3d37 2e32 2e33 2922 2c20 2263 6f76  (>=7.2.3)", "cov
+00020ad0: 6572 6167 652d 656e 6162 6c65 2d73 7562  erage-enable-sub
+00020ae0: 7072 6f63 6573 7320 283e 3d31 2922 2c20  process (>=1)", 
+00020af0: 2266 6c61 6b79 2028 3e3d 332e 3729 222c  "flaky (>=3.7)",
+00020b00: 2022 7061 636b 6167 696e 6720 283e 3d32   "packaging (>=2
+00020b10: 332e 3129 222c 2022 7079 7465 7374 2028  3.1)", "pytest (
+00020b20: 3e3d 372e 332e 3129 222c 2022 7079 7465  >=7.3.1)", "pyte
+00020b30: 7374 2d65 6e76 2028 3e3d 302e 382e 3129  st-env (>=0.8.1)
+00020b40: 222c 2022 7079 7465 7374 2d66 7265 657a  ", "pytest-freez
+00020b50: 6567 756e 2028 3e3d 302e 342e 3229 222c  egun (>=0.4.2)",
+00020b60: 2022 7079 7465 7374 2d6d 6f63 6b20 283e   "pytest-mock (>
+00020b70: 3d33 2e31 3029 222c 2022 7079 7465 7374  =3.10)", "pytest
+00020b80: 2d72 616e 646f 6d6c 7920 283e 3d33 2e31  -randomly (>=3.1
+00020b90: 3229 222c 2022 7079 7465 7374 2d74 696d  2)", "pytest-tim
+00020ba0: 656f 7574 2028 3e3d 322e 3129 222c 2022  eout (>=2.1)", "
+00020bb0: 7365 7475 7074 6f6f 6c73 2028 3e3d 3637  setuptools (>=67
+00020bc0: 2e37 2e31 2922 2c20 2274 696d 652d 6d61  .7.1)", "time-ma
+00020bd0: 6368 696e 6520 283e 3d32 2e39 2922 5d0a  chine (>=2.9)"].
+00020be0: 0a5b 5b70 6163 6b61 6765 5d5d 0a6e 616d  .[[package]].nam
+00020bf0: 6520 3d20 2277 6174 6368 646f 6722 0a76  e = "watchdog".v
+00020c00: 6572 7369 6f6e 203d 2022 332e 302e 3022  ersion = "3.0.0"
+00020c10: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
+00020c20: 4669 6c65 7379 7374 656d 2065 7665 6e74  Filesystem event
+00020c30: 7320 6d6f 6e69 746f 7269 6e67 220a 6f70  s monitoring".op
+00020c40: 7469 6f6e 616c 203d 2066 616c 7365 0a70  tional = false.p
+00020c50: 7974 686f 6e2d 7665 7273 696f 6e73 203d  ython-versions =
+00020c60: 2022 3e3d 332e 3722 0a66 696c 6573 203d   ">=3.7".files =
+00020c70: 205b 0a20 2020 207b 6669 6c65 203d 2022   [.    {file = "
+00020c80: 7761 7463 6864 6f67 2d33 2e30 2e30 2d63  watchdog-3.0.0-c
+00020c90: 7033 3130 2d63 7033 3130 2d6d 6163 6f73  p310-cp310-macos
+00020ca0: 785f 3130 5f39 5f75 6e69 7665 7273 616c  x_10_9_universal
+00020cb0: 322e 7768 6c22 2c20 6861 7368 203d 2022  2.whl", hash = "
+00020cc0: 7368 6132 3536 3a33 3336 6164 6663 3666  sha256:336adfc6f
+00020cd0: 3563 6334 6530 3337 6435 3264 6233 3131  5cc4e037d52db311
+00020ce0: 3934 6637 3538 3166 6637 3434 6236 3733  94f7581ff744b673
+00020cf0: 3832 6562 3630 3231 6338 3638 3332 3265  82eb6021c868322e
+00020d00: 3332 6565 6634 3122 7d2c 0a20 2020 207b  32eef41"},.    {
+00020d10: 6669 6c65 203d 2022 7761 7463 6864 6f67  file = "watchdog
+00020d20: 2d33 2e30 2e30 2d63 7033 3130 2d63 7033  -3.0.0-cp310-cp3
+00020d30: 3130 2d6d 6163 6f73 785f 3130 5f39 5f78  10-macosx_10_9_x
+00020d40: 3836 5f36 342e 7768 6c22 2c20 6861 7368  86_64.whl", hash
+00020d50: 203d 2022 7368 6132 3536 3a61 3730 6138   = "sha256:a70a8
+00020d60: 6463 6465 3931 6265 3532 3363 3335 6232  dcde91be523c35b2
+00020d70: 6266 3936 3139 3665 6463 3537 3330 6564  bf96196edc5730ed
+00020d80: 6233 3437 6533 3734 6337 6465 3763 6432  b347e374c7de7cd2
+00020d90: 3063 3433 6564 3935 3339 3722 7d2c 0a20  0c43ed95397"},. 
+00020da0: 2020 207b 6669 6c65 203d 2022 7761 7463     {file = "watc
+00020db0: 6864 6f67 2d33 2e30 2e30 2d63 7033 3130  hdog-3.0.0-cp310
+00020dc0: 2d63 7033 3130 2d6d 6163 6f73 785f 3131  -cp310-macosx_11
+00020dd0: 5f30 5f61 726d 3634 2e77 686c 222c 2068  _0_arm64.whl", h
+00020de0: 6173 6820 3d20 2273 6861 3235 363a 6164  ash = "sha256:ad
+00020df0: 6664 6561 6232 6461 3739 6561 3266 3736  fdeab2da79ea2f76
+00020e00: 6638 3765 6234 3261 3361 6231 3936 3661  f87eb42a3ab1966a
+00020e10: 3533 3133 6535 6136 3961 3032 3133 6133  5313e5a69a0213a3
+00020e20: 6363 3036 6566 3639 3262 3065 3936 227d  cc06ef692b0e96"}
+00020e30: 2c0a 2020 2020 7b66 696c 6520 3d20 2277  ,.    {file = "w
+00020e40: 6174 6368 646f 672d 332e 302e 302d 6370  atchdog-3.0.0-cp
+00020e50: 3331 312d 6370 3331 312d 6d61 636f 7378  311-cp311-macosx
+00020e60: 5f31 305f 395f 756e 6976 6572 7361 6c32  _10_9_universal2
+00020e70: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+00020e80: 6861 3235 363a 3262 3537 6131 6537 3330  ha256:2b57a1e730
+00020e90: 6166 3331 3536 6431 3362 3766 6464 6466  af3156d13b7fdddf
+00020ea0: 6332 3364 6561 3634 3837 6663 6563 6132  c23dea6487fceca2
+00020eb0: 3966 6337 3563 3561 3836 3862 6565 6432  9fc75c5a868beed2
+00020ec0: 3931 3737 6165 227d 2c0a 2020 2020 7b66  9177ae"},.    {f
+00020ed0: 696c 6520 3d20 2277 6174 6368 646f 672d  ile = "watchdog-
+00020ee0: 332e 302e 302d 6370 3331 312d 6370 3331  3.0.0-cp311-cp31
+00020ef0: 312d 6d61 636f 7378 5f31 305f 395f 7838  1-macosx_10_9_x8
+00020f00: 365f 3634 2e77 686c 222c 2068 6173 6820  6_64.whl", hash 
+00020f10: 3d20 2273 6861 3235 363a 3761 6465 3838  = "sha256:7ade88
+00020f20: 6430 6437 3738 6231 6232 3232 6164 6562  d0d778b1b222adeb
+00020f30: 6363 3039 3237 3432 3866 3838 3364 6230  cc0927428f883db0
+00020f40: 3730 3137 3631 3861 3565 3638 3466 6430  7017618a5e684fd0
+00020f50: 3362 3833 3334 3262 6439 227d 2c0a 2020  3b83342bd9"},.  
+00020f60: 2020 7b66 696c 6520 3d20 2277 6174 6368    {file = "watch
+00020f70: 646f 672d 332e 302e 302d 6370 3331 312d  dog-3.0.0-cp311-
+00020f80: 6370 3331 312d 6d61 636f 7378 5f31 315f  cp311-macosx_11_
+00020f90: 305f 6172 6d36 342e 7768 6c22 2c20 6861  0_arm64.whl", ha
+00020fa0: 7368 203d 2022 7368 6132 3536 3a37 6534  sh = "sha256:7e4
+00020fb0: 3437 6431 3732 6166 3532 6164 3230 3464  47d172af52ad204d
+00020fc0: 3139 3938 3237 3339 6161 3233 3436 3234  19982739aa234624
+00020fd0: 3563 6335 6261 3666 3537 3964 3136 6461  5cc5ba6f579d16da
+00020fe0: 6334 6266 6563 3232 3664 3265 3722 7d2c  c4bfec226d2e7"},
+00020ff0: 0a20 2020 207b 6669 6c65 203d 2022 7761  .    {file = "wa
+00021000: 7463 6864 6f67 2d33 2e30 2e30 2d63 7033  tchdog-3.0.0-cp3
+00021010: 372d 6370 3337 6d2d 6d61 636f 7378 5f31  7-cp37m-macosx_1
+00021020: 305f 395f 7838 365f 3634 2e77 686c 222c  0_9_x86_64.whl",
+00021030: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
+00021040: 3966 6163 3433 6137 3436 3665 6237 3365  9fac43a7466eb73e
+00021050: 3634 6139 3934 3061 6339 6564 3633 3639  64a9940ac9ed6369
+00021060: 6261 6133 3962 3362 6632 3231 6165 3233  baa39b3bf221ae23
+00021070: 3439 3361 3965 6334 6430 3032 3236 3734  493a9ec4d0022674
+00021080: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
+00021090: 2277 6174 6368 646f 672d 332e 302e 302d  "watchdog-3.0.0-
+000210a0: 6370 3338 2d63 7033 382d 6d61 636f 7378  cp38-cp38-macosx
+000210b0: 5f31 305f 395f 756e 6976 6572 7361 6c32  _10_9_universal2
+000210c0: 2e77 686c 222c 2068 6173 6820 3d20 2273  .whl", hash = "s
+000210d0: 6861 3235 363a 3861 6539 6364 6134 3166  ha256:8ae9cda41f
+000210e0: 6131 3134 6532 3866 6166 3836 6362 3133  a114e28faf86cb13
+000210f0: 3764 3735 3161 3137 6666 6430 3331 3664  7d751a17ffd0316d
+00021100: 3163 3334 6363 6632 3233 3565 3861 3834  1c34ccf2235e8a84
+00021110: 3336 3563 3766 227d 2c0a 2020 2020 7b66  365c7f"},.    {f
+00021120: 696c 6520 3d20 2277 6174 6368 646f 672d  ile = "watchdog-
+00021130: 332e 302e 302d 6370 3338 2d63 7033 382d  3.0.0-cp38-cp38-
+00021140: 6d61 636f 7378 5f31 305f 395f 7838 365f  macosx_10_9_x86_
+00021150: 3634 2e77 686c 222c 2068 6173 6820 3d20  64.whl", hash = 
+00021160: 2273 6861 3235 363a 3235 6637 3062 3461  "sha256:25f70b4a
+00021170: 6135 3362 6437 3433 3732 3963 3734 3735  a53bd743729c7475
+00021180: 6437 6563 3431 3039 3361 3538 3035 3238  d7ec41093a580528
+00021190: 6231 3030 6539 6138 6335 6235 6566 6538  b100e9a8c5b5efe8
+000211a0: 3839 3935 3932 6663 227d 2c0a 2020 2020  899592fc"},.    
+000211b0: 7b66 696c 6520 3d20 2277 6174 6368 646f  {file = "watchdo
+000211c0: 672d 332e 302e 302d 6370 3338 2d63 7033  g-3.0.0-cp38-cp3
+000211d0: 382d 6d61 636f 7378 5f31 315f 305f 6172  8-macosx_11_0_ar
+000211e0: 6d36 342e 7768 6c22 2c20 6861 7368 203d  m64.whl", hash =
+000211f0: 2022 7368 6132 3536 3a34 6639 3430 3639   "sha256:4f94069
+00021200: 6562 3136 3635 3764 3263 3666 6161 6461  eb16657d2c6faada
+00021210: 3436 3234 6333 3934 3634 6636 3563 3035  4624c39464f65c05
+00021220: 3630 3661 6635 3062 6237 3930 3265 3033  606af50bb7902e03
+00021230: 3665 3332 3139 6265 3322 7d2c 0a20 2020  6e3219be3"},.   
+00021240: 207b 6669 6c65 203d 2022 7761 7463 6864   {file = "watchd
+00021250: 6f67 2d33 2e30 2e30 2d63 7033 392d 6370  og-3.0.0-cp39-cp
+00021260: 3339 2d6d 6163 6f73 785f 3130 5f39 5f75  39-macosx_10_9_u
+00021270: 6e69 7665 7273 616c 322e 7768 6c22 2c20  niversal2.whl", 
+00021280: 6861 7368 203d 2022 7368 6132 3536 3a37  hash = "sha256:7
+00021290: 6335 6638 3462 3531 3934 6332 3464 6435  c5f84b5194c24dd5
+000212a0: 3733 6661 3634 3732 3638 3562 3261 3237  73fa6472685b2a27
+000212b0: 6363 3561 3137 6665 3566 3762 3666 6434  cc5a17fe5f7b6fd4
+000212c0: 3033 3435 3337 3863 6136 3831 3265 3322  0345378ca6812e3"
+000212d0: 7d2c 0a20 2020 207b 6669 6c65 203d 2022  },.    {file = "
+000212e0: 7761 7463 6864 6f67 2d33 2e30 2e30 2d63  watchdog-3.0.0-c
+000212f0: 7033 392d 6370 3339 2d6d 6163 6f73 785f  p39-cp39-macosx_
+00021300: 3130 5f39 5f78 3836 5f36 342e 7768 6c22  10_9_x86_64.whl"
+00021310: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00021320: 3a33 6161 3766 3661 3132 6538 3331 6464  :3aa7f6a12e831dd
+00021330: 6665 3738 6364 6434 6638 3939 3661 6639  fe78cdd4f8996af9
+00021340: 6366 3333 3466 6436 3334 3635 3331 6231  cf334fd6346531b1
+00021350: 3663 6563 3631 6333 6233 6330 6438 6461  6cec61c3b3c0d8da
+00021360: 3022 7d2c 0a20 2020 207b 6669 6c65 203d  0"},.    {file =
+00021370: 2022 7761 7463 6864 6f67 2d33 2e30 2e30   "watchdog-3.0.0
+00021380: 2d63 7033 392d 6370 3339 2d6d 6163 6f73  -cp39-cp39-macos
+00021390: 785f 3131 5f30 5f61 726d 3634 2e77 686c  x_11_0_arm64.whl
+000213a0: 222c 2068 6173 6820 3d20 2273 6861 3235  ", hash = "sha25
+000213b0: 363a 3233 3362 3538 3137 3933 3236 3835  6:233b5817932685
+000213c0: 6433 3961 3738 3936 6231 3039 3033 3533  d39a7896b1090353
+000213d0: 6663 3865 6663 3165 6639 3963 3963 3035  fc8efc1ef99c9c05
+000213e0: 3465 3436 6338 3030 3235 3631 3235 3266  4e46c8002561252f
+000213f0: 6238 227d 2c0a 2020 2020 7b66 696c 6520  b8"},.    {file 
+00021400: 3d20 2277 6174 6368 646f 672d 332e 302e  = "watchdog-3.0.
+00021410: 302d 7070 3337 2d70 7970 7933 375f 7070  0-pp37-pypy37_pp
+00021420: 3733 2d6d 6163 6f73 785f 3130 5f39 5f78  73-macosx_10_9_x
+00021430: 3836 5f36 342e 7768 6c22 2c20 6861 7368  86_64.whl", hash
+00021440: 203d 2022 7368 6132 3536 3a31 3362 6262   = "sha256:13bbb
+00021450: 6234 3632 6565 3432 6563 3363 3537 3233  b462ee42ec3c5723
+00021460: 6531 3230 3562 6538 6365 6437 3736 6630  e1205be8ced776f0
+00021470: 3562 3130 3065 3437 3337 3531 3863 3637  5b100e4737518c67
+00021480: 6338 3332 3563 6636 3130 3022 7d2c 0a20  c8325cf6100"},. 
+00021490: 2020 207b 6669 6c65 203d 2022 7761 7463     {file = "watc
+000214a0: 6864 6f67 2d33 2e30 2e30 2d70 7033 382d  hdog-3.0.0-pp38-
+000214b0: 7079 7079 3338 5f70 7037 332d 6d61 636f  pypy38_pp73-maco
+000214c0: 7378 5f31 305f 395f 7838 365f 3634 2e77  sx_10_9_x86_64.w
+000214d0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+000214e0: 3235 363a 3866 3363 6565 6364 3230 6437  256:8f3ceecd20d7
+000214f0: 3130 3637 6337 6664 3463 3965 3833 3264  1067c7fd4c9e832d
+00021500: 3465 3232 3538 3433 3138 3938 3363 6162  4e22584318983cab
+00021510: 6330 3133 6462 6633 6637 3065 6139 3564  c013dbf3f70ea95d
+00021520: 6533 3436 227d 2c0a 2020 2020 7b66 696c  e346"},.    {fil
+00021530: 6520 3d20 2277 6174 6368 646f 672d 332e  e = "watchdog-3.
+00021540: 302e 302d 7070 3339 2d70 7970 7933 395f  0.0-pp39-pypy39_
+00021550: 7070 3733 2d6d 6163 6f73 785f 3130 5f39  pp73-macosx_10_9
+00021560: 5f78 3836 5f36 342e 7768 6c22 2c20 6861  _x86_64.whl", ha
+00021570: 7368 203d 2022 7368 6132 3536 3a63 3964  sh = "sha256:c9d
+00021580: 3863 3865 6337 6566 6238 3837 3333 3363  8c8ec7efb887333c
+00021590: 6637 3165 3332 3865 3339 6366 6662 6637  f71e328e39cffbf7
+000215a0: 3731 6438 6638 6639 3564 3330 3865 6134  71d8f8f95d308ea4
+000215b0: 3132 3562 6635 6639 3062 6136 3422 7d2c  125bf5f90ba64"},
+000215c0: 0a20 2020 207b 6669 6c65 203d 2022 7761  .    {file = "wa
+000215d0: 7463 6864 6f67 2d33 2e30 2e30 2d70 7933  tchdog-3.0.0-py3
+000215e0: 2d6e 6f6e 652d 6d61 6e79 6c69 6e75 7832  -none-manylinux2
+000215f0: 3031 345f 6161 7263 6836 342e 7768 6c22  014_aarch64.whl"
+00021600: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00021610: 3a30 6530 3661 6238 3835 3861 3736 6531  :0e06ab8858a76e1
+00021620: 3231 3965 3638 6337 3537 3364 6665 6261  219e68c7573dfeba
+00021630: 3964 6431 6330 3231 3934 3736 6335 6134  9dd1c0219476c5a4
+00021640: 3464 3533 3333 6230 3164 3765 3137 3433  4d5333b01d7e1743
+00021650: 6122 7d2c 0a20 2020 207b 6669 6c65 203d  a"},.    {file =
+00021660: 2022 7761 7463 6864 6f67 2d33 2e30 2e30   "watchdog-3.0.0
+00021670: 2d70 7933 2d6e 6f6e 652d 6d61 6e79 6c69  -py3-none-manyli
+00021680: 6e75 7832 3031 345f 6172 6d76 376c 2e77  nux2014_armv7l.w
+00021690: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+000216a0: 3235 363a 6430 3065 3662 6534 3836 6166  256:d00e6be486af
+000216b0: 6662 3537 3831 3436 3834 3537 6232 3161  fb5781468457b21a
+000216c0: 3663 6265 3834 3863 3333 6566 3433 6639  6cbe848c33ef43f9
+000216d0: 6561 3461 3733 6234 3838 3265 3566 3138  ea4a73b4882e5f18
+000216e0: 3861 3434 227d 2c0a 2020 2020 7b66 696c  8a44"},.    {fil
+000216f0: 6520 3d20 2277 6174 6368 646f 672d 332e  e = "watchdog-3.
+00021700: 302e 302d 7079 332d 6e6f 6e65 2d6d 616e  0.0-py3-none-man
+00021710: 796c 696e 7578 3230 3134 5f69 3638 362e  ylinux2014_i686.
+00021720: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+00021730: 6132 3536 3a63 3037 3235 3330 3838 3236  a256:c0725308826
+00021740: 3563 3336 3364 3164 6466 3462 3363 6462  5c363d1ddf4b3cdb
+00021750: 3830 3864 3539 6130 3436 3865 6364 3031  808d59a0468ecd01
+00021760: 3737 3730 6564 3731 3639 3931 3632 3062  7770ed716991620b
+00021770: 3866 3737 6122 7d2c 0a20 2020 207b 6669  8f77a"},.    {fi
+00021780: 6c65 203d 2022 7761 7463 6864 6f67 2d33  le = "watchdog-3
+00021790: 2e30 2e30 2d70 7933 2d6e 6f6e 652d 6d61  .0.0-py3-none-ma
+000217a0: 6e79 6c69 6e75 7832 3031 345f 7070 6336  nylinux2014_ppc6
+000217b0: 342e 7768 6c22 2c20 6861 7368 203d 2022  4.whl", hash = "
+000217c0: 7368 6132 3536 3a35 3131 3333 3334 6366  sha256:5113334cf
+000217d0: 3863 6630 6163 3863 6434 3565 3166 3833  8cf0ac8cd45e1f83
+000217e0: 3039 6136 3033 3239 3162 3631 3431 3931  09a603291b614191
+000217f0: 6339 6164 6433 3464 3333 3037 3537 3237  c9add34d33075727
+00021800: 6139 3637 3730 3922 7d2c 0a20 2020 207b  a967709"},.    {
+00021810: 6669 6c65 203d 2022 7761 7463 6864 6f67  file = "watchdog
+00021820: 2d33 2e30 2e30 2d70 7933 2d6e 6f6e 652d  -3.0.0-py3-none-
+00021830: 6d61 6e79 6c69 6e75 7832 3031 345f 7070  manylinux2014_pp
+00021840: 6336 346c 652e 7768 6c22 2c20 6861 7368  c64le.whl", hash
+00021850: 203d 2022 7368 6132 3536 3a35 3166 3930   = "sha256:51f90
+00021860: 6637 3362 3436 3937 6261 6339 6339 6137  f73b4697bac9c9a7
+00021870: 3833 3934 6333 6163 6262 6433 3331 6363  8394c3acbbd331cc
+00021880: 6433 3635 3563 3131 6265 3161 3135 6165  d3655c11be1a15ae
+00021890: 3666 6532 3839 6138 6338 3322 7d2c 0a20  6fe289a8c83"},. 
+000218a0: 2020 207b 6669 6c65 203d 2022 7761 7463     {file = "watc
+000218b0: 6864 6f67 2d33 2e30 2e30 2d70 7933 2d6e  hdog-3.0.0-py3-n
+000218c0: 6f6e 652d 6d61 6e79 6c69 6e75 7832 3031  one-manylinux201
+000218d0: 345f 7333 3930 782e 7768 6c22 2c20 6861  4_s390x.whl", ha
+000218e0: 7368 203d 2022 7368 6132 3536 3a62 6130  sh = "sha256:ba0
+000218f0: 3765 3932 3735 3663 3937 6533 6163 6130  7e92756c97e3aca0
+00021900: 3931 3262 3563 6263 3465 3561 6438 3032  912b5cbc4e5ad802
+00021910: 6634 3535 3732 3132 3738 3865 3732 6137  f4557212788e72a7
+00021920: 3261 3437 6666 3337 3639 3530 6422 7d2c  2a47ff376950d"},
+00021930: 0a20 2020 207b 6669 6c65 203d 2022 7761  .    {file = "wa
+00021940: 7463 6864 6f67 2d33 2e30 2e30 2d70 7933  tchdog-3.0.0-py3
+00021950: 2d6e 6f6e 652d 6d61 6e79 6c69 6e75 7832  -none-manylinux2
+00021960: 3031 345f 7838 365f 3634 2e77 686c 222c  014_x86_64.whl",
+00021970: 2068 6173 6820 3d20 2273 6861 3235 363a   hash = "sha256:
+00021980: 6434 3239 6332 3433 3063 3933 6237 3930  d429c2430c93b790
+00021990: 3339 3134 6534 6462 3961 3936 3663 3766  3914e4db9a966c7f
+000219a0: 3262 3036 3864 6432 6562 6464 3266 6139  2b068dd2ebdd2fa9
+000219b0: 6239 6365 3039 3463 3764 3435 3966 3333  b9ce094c7d459f33
+000219c0: 227d 2c0a 2020 2020 7b66 696c 6520 3d20  "},.    {file = 
+000219d0: 2277 6174 6368 646f 672d 332e 302e 302d  "watchdog-3.0.0-
+000219e0: 7079 332d 6e6f 6e65 2d77 696e 3332 2e77  py3-none-win32.w
+000219f0: 686c 222c 2068 6173 6820 3d20 2273 6861  hl", hash = "sha
+00021a00: 3235 363a 3365 6437 6337 3161 3964 6363  256:3ed7c71a9dcc
+00021a10: 6665 3833 3863 3266 3062 3633 3134 6564  fe838c2f0b6314ed
+00021a20: 3064 3962 3232 6537 3764 3236 3863 3637  0d9b22e77d268c67
+00021a30: 6530 3135 3435 3061 3239 3033 3661 3831  e015450a29036a81
+00021a40: 6636 3066 227d 2c0a 2020 2020 7b66 696c  f60f"},.    {fil
+00021a50: 6520 3d20 2277 6174 6368 646f 672d 332e  e = "watchdog-3.
+00021a60: 302e 302d 7079 332d 6e6f 6e65 2d77 696e  0.0-py3-none-win
+00021a70: 5f61 6d64 3634 2e77 686c 222c 2068 6173  _amd64.whl", has
+00021a80: 6820 3d20 2273 6861 3235 363a 3463 3939  h = "sha256:4c99
+00021a90: 3536 6432 3762 6530 6262 3038 6663 3566  56d27be0bb08fc5f
+00021aa0: 3330 6439 6430 3137 3961 3835 3534 3336  30d9d0179a855436
+00021ab0: 6536 3535 6630 3436 6432 3838 6532 6263  e655f046d288e2bc
+00021ac0: 6331 3161 6466 6165 3839 3363 227d 2c0a  c11adfae893c"},.
+00021ad0: 2020 2020 7b66 696c 6520 3d20 2277 6174      {file = "wat
+00021ae0: 6368 646f 672d 332e 302e 302d 7079 332d  chdog-3.0.0-py3-
+00021af0: 6e6f 6e65 2d77 696e 5f69 6136 342e 7768  none-win_ia64.wh
+00021b00: 6c22 2c20 6861 7368 203d 2022 7368 6132  l", hash = "sha2
+00021b10: 3536 3a35 6439 6633 6131 3065 3032 6437  56:5d9f3a10e02d7
+00021b20: 3337 3163 6439 3239 6235 6438 6631 3165  371cd929b5d8f11e
+00021b30: 3837 6434 6261 6438 3930 3231 3265 6433  87d4bad890212ed3
+00021b40: 3930 3166 3962 3464 3638 3736 3762 6565  901f9b4d68767bee
+00021b50: 3735 3922 7d2c 0a20 2020 207b 6669 6c65  759"},.    {file
+00021b60: 203d 2022 7761 7463 6864 6f67 2d33 2e30   = "watchdog-3.0
+00021b70: 2e30 2e74 6172 2e67 7a22 2c20 6861 7368  .0.tar.gz", hash
+00021b80: 203d 2022 7368 6132 3536 3a34 6439 3861   = "sha256:4d98a
+00021b90: 3332 3035 3935 6461 3761 3763 3561 3138  320595da7a7c5a18
+00021ba0: 6663 3438 6362 3633 3363 3265 3733 6364  fc48cb633c2e73cd
+00021bb0: 6137 3866 3933 6361 6332 6566 3432 6434  a78f93cac2ef42d4
+00021bc0: 3262 6636 3039 6133 3366 3922 7d2c 0a5d  2bf609a33f9"},.]
+00021bd0: 0a0a 5b70 6163 6b61 6765 2e65 7874 7261  ..[package.extra
+00021be0: 735d 0a77 6174 6368 6d65 646f 203d 205b  s].watchmedo = [
+00021bf0: 2250 7959 414d 4c20 283e 3d33 2e31 3029  "PyYAML (>=3.10)
+00021c00: 225d 0a0a 5b5b 7061 636b 6167 655d 5d0a  "]..[[package]].
+00021c10: 6e61 6d65 203d 2022 7765 6265 6e63 6f64  name = "webencod
+00021c20: 696e 6773 220a 7665 7273 696f 6e20 3d20  ings".version = 
+00021c30: 2230 2e35 2e31 220a 6465 7363 7269 7074  "0.5.1".descript
+00021c40: 696f 6e20 3d20 2243 6861 7261 6374 6572  ion = "Character
+00021c50: 2065 6e63 6f64 696e 6720 616c 6961 7365   encoding aliase
+00021c60: 7320 666f 7220 6c65 6761 6379 2077 6562  s for legacy web
+00021c70: 2063 6f6e 7465 6e74 220a 6f70 7469 6f6e   content".option
+00021c80: 616c 203d 2066 616c 7365 0a70 7974 686f  al = false.pytho
+00021c90: 6e2d 7665 7273 696f 6e73 203d 2022 2a22  n-versions = "*"
+00021ca0: 0a66 696c 6573 203d 205b 0a20 2020 207b  .files = [.    {
+00021cb0: 6669 6c65 203d 2022 7765 6265 6e63 6f64  file = "webencod
+00021cc0: 696e 6773 2d30 2e35 2e31 2d70 7932 2e70  ings-0.5.1-py2.p
+00021cd0: 7933 2d6e 6f6e 652d 616e 792e 7768 6c22  y3-none-any.whl"
+00021ce0: 2c20 6861 7368 203d 2022 7368 6132 3536  , hash = "sha256
+00021cf0: 3a61 3061 6631 3231 3366 3363 3232 3236  :a0af1213f3c2226
+00021d00: 3439 3761 3937 6532 6233 6161 3031 6137  497a97e2b3aa01a7
+00021d10: 6534 6265 6534 6634 3033 6639 3562 6531  e4bee4f403f95be1
+00021d20: 3666 6339 6163 6432 3934 3735 3134 6137  6fc9acd2947514a7
+00021d30: 3822 7d2c 0a20 2020 207b 6669 6c65 203d  8"},.    {file =
+00021d40: 2022 7765 6265 6e63 6f64 696e 6773 2d30   "webencodings-0
+00021d50: 2e35 2e31 2e74 6172 2e67 7a22 2c20 6861  .5.1.tar.gz", ha
+00021d60: 7368 203d 2022 7368 6132 3536 3a62 3336  sh = "sha256:b36
+00021d70: 6131 6332 3435 6632 6433 3034 3936 3565  a1c245f2d304965e
+00021d80: 6234 6530 6138 3238 3438 3337 3932 3431  b4e0a82848379241
+00021d90: 6463 3034 6238 3635 6166 6363 3461 6162  dc04b865afcc4aab
+00021da0: 3136 3734 3835 3837 6531 3932 3322 7d2c  16748587e1923"},
+00021db0: 0a5d 0a0a 5b5b 7061 636b 6167 655d 5d0a  .]..[[package]].
+00021dc0: 6e61 6d65 203d 2022 7768 6565 6c22 0a76  name = "wheel".v
+00021dd0: 6572 7369 6f6e 203d 2022 302e 3430 2e30  ersion = "0.40.0
+00021de0: 220a 6465 7363 7269 7074 696f 6e20 3d20  ".description = 
+00021df0: 2241 2062 7569 6c74 2d70 6163 6b61 6765  "A built-package
+00021e00: 2066 6f72 6d61 7420 666f 7220 5079 7468   format for Pyth
+00021e10: 6f6e 220a 6f70 7469 6f6e 616c 203d 2066  on".optional = f
+00021e20: 616c 7365 0a70 7974 686f 6e2d 7665 7273  alse.python-vers
+00021e30: 696f 6e73 203d 2022 3e3d 332e 3722 0a66  ions = ">=3.7".f
+00021e40: 696c 6573 203d 205b 0a20 2020 207b 6669  iles = [.    {fi
+00021e50: 6c65 203d 2022 7768 6565 6c2d 302e 3430  le = "wheel-0.40
+00021e60: 2e30 2d70 7933 2d6e 6f6e 652d 616e 792e  .0-py3-none-any.
+00021e70: 7768 6c22 2c20 6861 7368 203d 2022 7368  whl", hash = "sh
+00021e80: 6132 3536 3a64 3233 3662 3230 6537 6362  a256:d236b20e7cb
+00021e90: 3532 3264 6166 3233 3930 6661 3834 6335  522daf2390fa84c5
+00021ea0: 3565 6561 3831 6335 6333 3031 3930 6639  5eea81c5c30190f9
+00021eb0: 3066 3239 6165 3263 6131 6164 3833 3535  0f29ae2ca1ad8355
+00021ec0: 6266 3234 3722 7d2c 0a20 2020 207b 6669  bf247"},.    {fi
+00021ed0: 6c65 203d 2022 7768 6565 6c2d 302e 3430  le = "wheel-0.40
+00021ee0: 2e30 2e74 6172 2e67 7a22 2c20 6861 7368  .0.tar.gz", hash
+00021ef0: 203d 2022 7368 6132 3536 3a63 6431 3139   = "sha256:cd119
+00021f00: 3666 3366 6165 6532 6233 3139 3638 6436  6f3faee2b31968d6
+00021f10: 3236 6531 3733 3163 3934 6639 3963 6264  26e1731c94f99cbd
+00021f20: 6236 3763 6635 6134 3665 3466 3536 3536  b67cf5a46e4f5656
+00021f30: 6362 6565 3737 3338 3837 3322 7d2c 0a5d  cbee7738873"},.]
+00021f40: 0a0a 5b70 6163 6b61 6765 2e65 7874 7261  ..[package.extra
+00021f50: 735d 0a74 6573 7420 3d20 5b22 7079 7465  s].test = ["pyte
+00021f60: 7374 2028 3e3d 362e 302e 3029 225d 0a0a  st (>=6.0.0)"]..
+00021f70: 5b5b 7061 636b 6167 655d 5d0a 6e61 6d65  [[package]].name
+00021f80: 203d 2022 7a69 7070 220a 7665 7273 696f   = "zipp".versio
+00021f90: 6e20 3d20 2233 2e31 352e 3022 0a64 6573  n = "3.15.0".des
+00021fa0: 6372 6970 7469 6f6e 203d 2022 4261 636b  cription = "Back
+00021fb0: 706f 7274 206f 6620 7061 7468 6c69 622d  port of pathlib-
+00021fc0: 636f 6d70 6174 6962 6c65 206f 626a 6563  compatible objec
+00021fd0: 7420 7772 6170 7065 7220 666f 7220 7a69  t wrapper for zi
+00021fe0: 7020 6669 6c65 7322 0a6f 7074 696f 6e61  p files".optiona
+00021ff0: 6c20 3d20 6661 6c73 650a 7079 7468 6f6e  l = false.python
+00022000: 2d76 6572 7369 6f6e 7320 3d20 223e 3d33  -versions = ">=3
+00022010: 2e37 220a 6669 6c65 7320 3d20 5b0a 2020  .7".files = [.  
+00022020: 2020 7b66 696c 6520 3d20 227a 6970 702d    {file = "zipp-
+00022030: 332e 3135 2e30 2d70 7933 2d6e 6f6e 652d  3.15.0-py3-none-
+00022040: 616e 792e 7768 6c22 2c20 6861 7368 203d  any.whl", hash =
+00022050: 2022 7368 6132 3536 3a34 3839 3034 6663   "sha256:48904fc
+00022060: 3736 6136 3065 3534 3261 6631 3531 6164  76a60e542af151ad
+00022070: 6564 3935 3732 3663 3161 3563 3334 6564  ed95726c1a5c34ed
+00022080: 3433 6162 3431 3334 6235 3937 3636 3563  43ab4134b597665c
+00022090: 3836 6437 6164 3535 3622 7d2c 0a20 2020  86d7ad556"},.   
+000220a0: 207b 6669 6c65 203d 2022 7a69 7070 2d33   {file = "zipp-3
+000220b0: 2e31 352e 302e 7461 722e 677a 222c 2068  .15.0.tar.gz", h
+000220c0: 6173 6820 3d20 2273 6861 3235 363a 3131  ash = "sha256:11
+000220d0: 3239 3239 6164 3634 3964 6139 3431 6332  2929ad649da941c2
+000220e0: 3364 6535 3066 3335 3661 3262 3535 3730  3de50f356a2b5570
+000220f0: 6339 3534 6236 3531 3530 3634 3262 6363  c954b65150642bcc
+00022100: 6464 3636 6266 3139 3464 3232 3462 227d  dd66bf194d224b"}
+00022110: 2c0a 5d0a 0a5b 7061 636b 6167 652e 6578  ,.]..[package.ex
+00022120: 7472 6173 5d0a 646f 6373 203d 205b 2266  tras].docs = ["f
+00022130: 7572 6f22 2c20 226a 6172 6163 6f2e 7061  uro", "jaraco.pa
+00022140: 636b 6167 696e 6720 283e 3d39 2922 2c20  ckaging (>=9)", 
+00022150: 226a 6172 6163 6f2e 7469 6465 6c69 6674  "jaraco.tidelift
+00022160: 2028 3e3d 312e 3429 222c 2022 7273 742e   (>=1.4)", "rst.
+00022170: 6c69 6e6b 6572 2028 3e3d 312e 3929 222c  linker (>=1.9)",
+00022180: 2022 7370 6869 6e78 2028 3e3d 332e 3529   "sphinx (>=3.5)
+00022190: 222c 2022 7370 6869 6e78 2d6c 696e 7422  ", "sphinx-lint"
+000221a0: 5d0a 7465 7374 696e 6720 3d20 5b22 6269  ].testing = ["bi
+000221b0: 672d 4f22 2c20 2266 6c61 6b65 3820 283c  g-O", "flake8 (<
+000221c0: 3529 222c 2022 6a61 7261 636f 2e66 756e  5)", "jaraco.fun
+000221d0: 6374 6f6f 6c73 222c 2022 6a61 7261 636f  ctools", "jaraco
+000221e0: 2e69 7465 7274 6f6f 6c73 222c 2022 6d6f  .itertools", "mo
+000221f0: 7265 2d69 7465 7274 6f6f 6c73 222c 2022  re-itertools", "
+00022200: 7079 7465 7374 2028 3e3d 3629 222c 2022  pytest (>=6)", "
+00022210: 7079 7465 7374 2d62 6c61 636b 2028 3e3d  pytest-black (>=
+00022220: 302e 332e 3729 222c 2022 7079 7465 7374  0.3.7)", "pytest
+00022230: 2d63 6865 636b 646f 6373 2028 3e3d 322e  -checkdocs (>=2.
+00022240: 3429 222c 2022 7079 7465 7374 2d63 6f76  4)", "pytest-cov
+00022250: 222c 2022 7079 7465 7374 2d65 6e61 626c  ", "pytest-enabl
+00022260: 6572 2028 3e3d 312e 3329 222c 2022 7079  er (>=1.3)", "py
+00022270: 7465 7374 2d66 6c61 6b65 3822 2c20 2270  test-flake8", "p
+00022280: 7974 6573 742d 6d79 7079 2028 3e3d 302e  ytest-mypy (>=0.
+00022290: 392e 3129 225d 0a0a 5b6d 6574 6164 6174  9.1)"]..[metadat
+000222a0: 615d 0a6c 6f63 6b2d 7665 7273 696f 6e20  a].lock-version 
+000222b0: 3d20 2232 2e30 220a 7079 7468 6f6e 2d76  = "2.0".python-v
+000222c0: 6572 7369 6f6e 7320 3d20 225e 332e 382e  ersions = "^3.8.
+000222d0: 3122 0a63 6f6e 7465 6e74 2d68 6173 6820  1".content-hash 
+000222e0: 3d20 2265 6631 6363 6263 3436 3833 3935  = "ef1ccbc468395
+000222f0: 6435 3730 6662 3832 3035 3436 6563 3638  d570fb820546ec68
+00022300: 6364 3864 3263 3763 6439 6562 6535 6365  cd8d2c7cd9ebe5ce
+00022310: 3865 3362 3734 3633 3763 3436 6462 3034  8e3b74637c46db04
+00022320: 6634 3522 0a                             f45".
```

### Comparing `containers_sugar-1.6.1/pyproject.toml` & `containers_sugar-1.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "containers-sugar"
-version = "1.6.1"  # semantic-release
+version = "1.7.0"  # semantic-release
 description = "Simplify the usage of containers"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 include = [
   "*.cfg",
   "*.ini",
   "*.js",
@@ -39,14 +39,15 @@
 [tool.poetry.dependencies]
 python = "^3.8.1"
 Jinja2 = "<3.1.0"
 sh = "^2.0.0"
 pyyaml = ">=5"
 colorama = "^0.4.6"
 urllib3 = "<2"
+python-dotenv = "^0.21.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7"
 blue = "^0.9.1"
 isort = "^5"
 pre-commit = "2"
 flake8 = "^4"
```

### Comparing `containers_sugar-1.6.1/PKG-INFO` & `containers_sugar-1.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: containers-sugar
-Version: 1.6.1
+Version: 1.7.0
 Summary: Simplify the usage of containers
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (<3.1.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: pyyaml (>=5)
 Requires-Dist: sh (>=2.0.0,<3.0.0)
 Requires-Dist: urllib3 (<2)
```

