# Comparing `tmp/pynamer-2.0.3.tar.gz` & `tmp/pynamer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.0.3.tar", last modified: Fri Jun  2 19:53:05 2023, max compression
+gzip compressed data, was "pynamer-2.1.0.tar", last modified: Tue Jun  6 14:08:37 2023, max compression
```

## Comparing `pynamer-2.0.3.tar` & `pynamer-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.269421 pynamer-2.0.3/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.3/AUTHORS.md
--rw-rw-rw-   0        0        0    10114 2023-06-02 19:52:49.000000 pynamer-2.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.3/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    18796 2023-06-02 19:53:05.270421 pynamer-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    17213 2023-06-02 18:15:07.000000 pynamer-2.0.3/README.md
--rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1818 2023-06-02 19:53:05.272434 pynamer-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:04.933347 pynamer-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.017348 pynamer-2.0.3/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.3/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1929 2023-06-02 19:52:50.000000 pynamer-2.0.3/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.0.3/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2210 2023-05-28 18:04:31.000000 pynamer-2.0.3/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      726 2023-05-25 17:08:55.000000 pynamer-2.0.3/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.027346 pynamer-2.0.3/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.3/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7524 2023-05-31 13:31:21.000000 pynamer-2.0.3/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.3/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.3/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     9587 2023-05-31 14:18:45.000000 pynamer-2.0.3/src/pynamer/utils.py
--rw-rw-rw-   0        0        0     8280 2023-06-02 19:50:27.000000 pynamer-2.0.3/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.025348 pynamer-2.0.3/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18796 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1130 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 19:53:04.000000 pynamer-2.0.3/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:05.267449 pynamer-2.0.3/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1700 2023-06-02 19:42:16.000000 pynamer-2.0.3/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.3/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.0.3/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.3/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.139580 pynamer-2.1.0/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.0/AUTHORS.md
+-rw-rw-rw-   0        0        0    10298 2023-06-06 14:08:25.000000 pynamer-2.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18770 2023-06-06 14:08:37.139580 pynamer-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17213 2023-06-02 18:15:07.000000 pynamer-2.1.0/README.md
+-rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1842 2023-06-06 14:08:37.139580 pynamer-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:08:36.954576 pynamer-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.023642 pynamer-2.1.0/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.0/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-06 14:08:25.000000 pynamer-2.1.0/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.0/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2354 2023-06-04 10:27:28.000000 pynamer-2.1.0/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      823 2023-06-04 16:16:48.000000 pynamer-2.1.0/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.039263 pynamer-2.1.0/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.0/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7639 2023-06-04 10:50:40.000000 pynamer-2.1.0/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.0/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.0/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.0/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    10643 2023-06-06 14:04:47.000000 pynamer-2.1.0/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.039263 pynamer-2.1.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18770 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.139580 pynamer-2.1.0/tests/
+-rw-rw-rw-   0        0        0     2063 2023-06-04 10:27:28.000000 pynamer-2.1.0/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.0/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.0/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     1927 2023-06-06 13:17:15.000000 pynamer-2.1.0/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.0/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.0/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.0/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_write_output_file.py
```

### Comparing `pynamer-2.0.3/CHANGELOG.md` & `pynamer-2.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.0 (2023-06-06)
+### Feature
+* Option to display github statistics ([`4ce5654`](https://github.com/Stephen-RA-King/pynamer/commit/4ce5654dcc6447b0518de9fd64f4c15fc6258e0f))
+
 ## v2.0.3 (2023-06-02)
 ### Fix
 * Json formatting ([`892a454`](https://github.com/Stephen-RA-King/pynamer/commit/892a454d47c868973978e54be89f472ae351b455))
 
 ## v2.0.2 (2023-05-31)
 ### Fix
 * Account for nonetype returned in json data ([`39f245c`](https://github.com/Stephen-RA-King/pynamer/commit/39f245c41b17add26ed9399dbb3c376cd395d79b))
```

### Comparing `pynamer-2.0.3/LICENSE` & `pynamer-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/PKG-INFO` & `pynamer-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.3
+Version: 2.1.0
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -21,15 +21,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.md
 
 _**Utility to find an available package name in the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
```

### Comparing `pynamer-2.0.3/README.md` & `pynamer-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/pyproject.toml` & `pynamer-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/setup.cfg` & `pynamer-2.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -29,86 +29,88 @@
 000001c0: 7465 7068 656e 2d52 412d 4b69 6e67 2f70  tephen-RA-King/p
 000001d0: 796e 616d 6572 0d0a 646f 776e 6c6f 6164  ynamer..download
 000001e0: 5f75 726c 203d 2068 7474 7073 3a2f 2f67  _url = https://g
 000001f0: 6974 6875 622e 636f 6d2f 5374 6570 6865  ithub.com/Stephe
 00000200: 6e2d 5241 2d4b 696e 672f 7079 6e61 6d65  n-RA-King/pyname
 00000210: 722f 6172 6368 6976 652f 7265 6673 2f68  r/archive/refs/h
 00000220: 6561 6473 2f6d 6169 6e2e 7a69 700d 0a6c  eads/main.zip..l
-00000230: 6963 656e 7365 203d 204d 4954 0d0a 636c  icense = MIT..cl
-00000240: 6173 7369 6669 6572 7320 3d20 0d0a 0944  assifiers = ...D
-00000250: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-00000260: 7320 3a3a 2035 202d 2050 726f 6475 6374  s :: 5 - Product
-00000270: 696f 6e2f 5374 6162 6c65 0d0a 0945 6e76  ion/Stable...Env
-00000280: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
-00000290: 6f6c 650d 0a09 496e 7465 6e64 6564 2041  ole...Intended A
-000002a0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-000002b0: 6f70 6572 730d 0a09 4c69 6365 6e73 6520  opers...License 
-000002c0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000002d0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-000002e0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-000002f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000300: 656e 740d 0a09 4e61 7475 7261 6c20 4c61  ent...Natural La
-00000310: 6e67 7561 6765 203a 3a20 456e 676c 6973  nguage :: Englis
-00000320: 680d 0a09 5072 6f67 7261 6d6d 696e 6720  h...Programming 
-00000330: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000340: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
-00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000360: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
-00000370: 204f 6e6c 790d 0a09 5072 6f67 7261 6d6d   Only...Programm
-00000380: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000390: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-000003a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003c0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
-000003d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003e0: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-000003f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000400: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000410: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
-00000420: 6669 6e64 3a0d 0a70 726f 6a65 6374 5f75  find:..project_u
-00000430: 726c 7320 3d20 0d0a 696e 636c 7564 655f  rls = ..include_
-00000440: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000450: 7275 650d 0a70 7974 686f 6e5f 7265 7175  rue..python_requ
-00000460: 6972 6573 203d 203e 3d33 2e39 0d0a 696e  ires = >=3.9..in
-00000470: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000480: 200d 0a09 6273 340d 0a09 6275 696c 640d   ...bs4...build.
-00000490: 0a09 636f 6c6f 7261 6d61 0d0a 096a 696e  ..colorama...jin
-000004a0: 6a61 320d 0a09 7061 636b 6167 696e 670d  ja2...packaging.
-000004b0: 0a09 7079 7961 6d6c 0d0a 0972 6571 7565  ..pyyaml...reque
-000004c0: 7374 730d 0a09 7269 6368 0d0a 0974 7164  sts...rich...tqd
-000004d0: 6d0d 0a09 7477 696e 650d 0a09 7768 6565  m...twine...whee
-000004e0: 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  l....[options.pa
-000004f0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000500: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
-00000510: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-00000520: 7461 5d0d 0a70 796e 616d 6572 203d 200d  ta]..pynamer = .
-00000530: 0a09 5245 4144 4d45 2e6d 640d 0a09 636f  ..README.md...co
-00000540: 6e66 6967 2e70 790d 0a09 7072 6f6a 6563  nfig.py...projec
-00000550: 745f 6e61 6d65 0d0a 0970 726f 6a65 6374  t_name...project
-00000560: 5f6e 616d 652f 5f5f 696e 6974 5f5f 2e70  _name/__init__.p
-00000570: 790d 0a09 7365 7475 702e 7478 740d 0a09  y...setup.txt...
-00000580: 7365 7475 705f 6261 7365 2e74 7874 0d0a  setup_base.txt..
-00000590: 0975 7469 6c73 2e70 790d 0a0d 0a5b 6f70  .utils.py....[op
-000005a0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-000005b0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-000005c0: 6970 7473 203d 200d 0a09 7079 6e61 6d65  ipts = ...pyname
-000005d0: 7220 3d20 7079 6e61 6d65 722e 7079 6e61  r = pynamer.pyna
-000005e0: 6d65 723a 6d61 696e 0d0a 0d0a 5b66 6c61  mer:main....[fla
-000005f0: 6b65 385d 0d0a 646f 6373 7472 696e 672d  ke8]..docstring-
-00000600: 636f 6e76 656e 7469 6f6e 203d 206e 756d  convention = num
-00000610: 7079 0d0a 6d61 782d 636f 6d70 6c65 7869  py..max-complexi
-00000620: 7479 203d 2031 380d 0a6d 6178 2d6c 696e  ty = 18..max-lin
-00000630: 652d 6c65 6e67 7468 203d 2038 380d 0a73  e-length = 88..s
-00000640: 656c 6563 7420 3d20 422c 2042 392c 2043  elect = B, B9, C
-00000650: 2c20 442c 2045 2c20 462c 204e 2c20 570d  , D, E, F, N, W.
-00000660: 0a65 7863 6c75 6465 203d 2074 6573 7473  .exclude = tests
-00000670: 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a  /*,.tox/*,.nox/*
-00000680: 2c64 6f63 732f 2a2c 2e67 6974 2f2a 2c2e  ,docs/*,.git/*,.
-00000690: 6769 7468 7562 2f2a 0d0a 6967 6e6f 7265  github/*..ignore
-000006a0: 203d 200d 0a09 4532 3033 2c0d 0a09 5735   = ...E203,...W5
-000006b0: 3033 2c0d 0a70 6572 2d66 696c 652d 6967  03,..per-file-ig
-000006c0: 6e6f 7265 7320 3d20 0d0a 0970 796e 616d  nores = ...pynam
-000006d0: 6572 2e70 793a 4339 3031 0d0a 0962 7569  er.py:C901...bui
-000006e0: 6c64 6572 2e70 793a 4339 3031 0d0a 0d0a  lder.py:C901....
-000006f0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000700: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000710: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000230: 6963 656e 7365 203d 204d 4954 0d0a 6c69  icense = MIT..li
+00000240: 6365 6e73 655f 6669 6c65 203d 204c 4943  cense_file = LIC
+00000250: 454e 5345 0d0a 636c 6173 7369 6669 6572  ENSE..classifier
+00000260: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
+00000270: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+00000280: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00000290: 6c65 0d0a 0945 6e76 6972 6f6e 6d65 6e74  le...Environment
+000002a0: 203a 3a20 436f 6e73 6f6c 650d 0a09 496e   :: Console...In
+000002b0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+000002c0: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+000002d0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000002e0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000002f0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+00000300: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+00000310: 496e 6465 7065 6e64 656e 740d 0a09 4e61  Independent...Na
+00000320: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
+00000330: 3a20 456e 676c 6973 680d 0a09 5072 6f67  : English...Prog
+00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+00000360: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000370: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000380: 203a 3a20 3320 3a3a 204f 6e6c 790d 0a09   :: 3 :: Only...
+00000390: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003b0: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
+000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003d0: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+000003e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000003f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000400: 3a3a 2033 2e31 310d 0a0d 0a5b 6f70 7469  :: 3.11....[opti
+00000410: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+00000420: 7220 3d20 0d0a 093d 7372 630d 0a70 6163  r = ...=src..pac
+00000430: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+00000440: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000450: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000460: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
+00000470: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000480: 3d33 2e39 0d0a 696e 7374 616c 6c5f 7265  =3.9..install_re
+00000490: 7175 6972 6573 203d 200d 0a09 6273 340d  quires = ...bs4.
+000004a0: 0a09 6275 696c 640d 0a09 636f 6c6f 7261  ..build...colora
+000004b0: 6d61 0d0a 096a 696e 6a61 320d 0a09 7061  ma...jinja2...pa
+000004c0: 636b 6167 696e 670d 0a09 7079 7961 6d6c  ckaging...pyyaml
+000004d0: 0d0a 0972 6571 7565 7374 730d 0a09 7269  ...requests...ri
+000004e0: 6368 0d0a 0974 7164 6d0d 0a09 7477 696e  ch...tqdm...twin
+000004f0: 650d 0a09 7768 6565 6c0d 0a0d 0a5b 6f70  e...wheel....[op
+00000500: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000510: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000520: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+00000530: 636b 6167 655f 6461 7461 5d0d 0a70 796e  ckage_data]..pyn
+00000540: 616d 6572 203d 200d 0a09 5245 4144 4d45  amer = ...README
+00000550: 2e6d 640d 0a09 636f 6e66 6967 2e70 790d  .md...config.py.
+00000560: 0a09 7072 6f6a 6563 745f 6e61 6d65 0d0a  ..project_name..
+00000570: 0970 726f 6a65 6374 5f6e 616d 652f 5f5f  .project_name/__
+00000580: 696e 6974 5f5f 2e70 790d 0a09 7365 7475  init__.py...setu
+00000590: 702e 7478 740d 0a09 7365 7475 705f 6261  p.txt...setup_ba
+000005a0: 7365 2e74 7874 0d0a 0975 7469 6c73 2e70  se.txt...utils.p
+000005b0: 790d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  y....[options.en
+000005c0: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+000005d0: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+000005e0: 0a09 7079 6e61 6d65 7220 3d20 7079 6e61  ..pynamer = pyna
+000005f0: 6d65 722e 7079 6e61 6d65 723a 6d61 696e  mer.pynamer:main
+00000600: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 646f  ....[flake8]..do
+00000610: 6373 7472 696e 672d 636f 6e76 656e 7469  cstring-conventi
+00000620: 6f6e 203d 206e 756d 7079 0d0a 6d61 782d  on = numpy..max-
+00000630: 636f 6d70 6c65 7869 7479 203d 2031 380d  complexity = 18.
+00000640: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+00000650: 203d 2038 380d 0a73 656c 6563 7420 3d20   = 88..select = 
+00000660: 422c 2042 392c 2043 2c20 442c 2045 2c20  B, B9, C, D, E, 
+00000670: 462c 204e 2c20 570d 0a65 7863 6c75 6465  F, N, W..exclude
+00000680: 203d 2074 6573 7473 2f2a 2c2e 746f 782f   = tests/*,.tox/
+00000690: 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f 2a2c  *,.nox/*,docs/*,
+000006a0: 2e67 6974 2f2a 2c2e 6769 7468 7562 2f2a  .git/*,.github/*
+000006b0: 0d0a 6967 6e6f 7265 203d 200d 0a09 4532  ..ignore = ...E2
+000006c0: 3033 2c0d 0a09 5735 3033 2c0d 0a70 6572  03,...W503,..per
+000006d0: 2d66 696c 652d 6967 6e6f 7265 7320 3d20  -file-ignores = 
+000006e0: 0d0a 0970 796e 616d 6572 2e70 793a 4339  ...pynamer.py:C9
+000006f0: 3031 0d0a 0962 7569 6c64 6572 2e70 793a  01...builder.py:
+00000700: 4339 3031 0d0a 0d0a 5b65 6767 5f69 6e66  C901....[egg_inf
+00000710: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000720: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000730: 0d0a                                     ..
```

### Comparing `pynamer-2.0.3/src/pynamer/__init__.py` & `pynamer-2.1.0/src/pynamer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.0.3"
+__version__ = "2.1.0"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
@@ -57,21 +57,21 @@
 project_count_file_trv = project_path.joinpath("project_count.pickle")
 pypi_index_file_trv = project_path.joinpath("pypi_index")
 meta_file_trv = project_path.joinpath("meta.pickle")
 
 
 if setup_file_trv.is_file():
     setup_text = setup_file_trv.read_text(encoding="utf-8")
-else:
+else:  # pragma: no cover
     raise SystemExit("The package has a structural problem")
 
 
 if project_count_file_trv.is_file():
     project_count = pickle.loads(project_count_file_trv.read_bytes())
-else:
+else:  # pragma: no cover
     project_count = 455256
 
 
 if meta_file_trv.is_file():
     meta = pickle.loads(meta_file_trv.read_bytes())
-else:
+else:  # pragma: no cover
     meta = {}
```

### Comparing `pynamer-2.0.3/src/pynamer/builder.py` & `pynamer-2.1.0/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/src/pynamer/cli.py` & `pynamer-2.1.0/src/pynamer/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,21 @@
         "-m",
         "--meta",
         action="store_true",
         help="input new meta data when registering (Author and email address)",
     )
 
     parser.add_argument(
+        "-s",
+        "--stats",
+        action="store_true",
+        help="display GitHub stats if available",
+    )
+
+    parser.add_argument(
         "-w",
         "--webbrowser",
         action="store_true",
         help="open the project on PyPI in a webbrowser",
     )
 
     parser.add_argument(
```

### Comparing `pynamer-2.0.3/src/pynamer/config.py` & `pynamer-2.1.0/src/pynamer/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,11 +18,13 @@
     project_count: int = project_count
     package_version: str = "0.0.0"
     description: str = "placeholder"
     pypi_search_url: str = "https://pypi.org/search/"
     pypi_project_url: str = "https://pypi.org/project/"
     pypi_json_url: str = "https://pypi.org/pypi/"
     pypi_simple_index_url: str = "https://pypi.org/simple/"
+    github_api_url = "https://api.github.com/repos/"
+    github_base_url = "https://github.com/"
     idlemode: int = 1 if "idlelib.run" in sys.modules else 0
 
 
 config = Config()
```

### Comparing `pynamer-2.0.3/src/pynamer/pynamer.py` & `pynamer-2.1.0/src/pynamer/pynamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,22 +110,25 @@
         others_table.add_column("Released", style="bold yellow")
         others_table.add_column("Description", style="bold cyan")
 
         # perform the tests
         # Test 1
         if _ping_project(new_project):
             test_results.append(1)
-            json_data = _ping_json(new_project)
+            if args.stats is True:
+                json_data = _ping_json(new_project, stats=True)
+            else:
+                json_data = _ping_json(new_project)
             test_table.add_row(
-                "1", "Basic http get to project URL", "[red]FOUND[/red]", json_data
+                "1", "Check PyPI project URL", "[red]FOUND[/red]", json_data
             )
         else:
             test_results.append(0)
             test_table.add_row(
-                "1", "Basic http get to project URL", "[green]NOT FOUND[/green]", ""
+                "1", "Check PyPI project URL", "[green]NOT FOUND[/green]", ""
             )
 
         # Test 2
         if _pypi_search_index(new_project):
             test_results.append(1)
             test_table.add_row(
                 "2",
@@ -144,25 +147,25 @@
 
         # Test 3
         match, others, others_total = _pypi_search(new_project)
         if match:
             test_results.append(1)
             test_table.add_row(
                 "3",
-                "Check PyPI search",
+                "Check PyPI search API",
                 "[red]FOUND[/red]",
                 f"Exact match found: {len(match)}, Others found: {others_total}",
             )
             for items in match:
                 match_table.add_row(items[0], items[1], items[2], items[3])
         else:
             test_results.append(0)
             test_table.add_row(
                 "3",
-                "Check PyPI search",
+                "Check PyPI search API",
                 "[green]NOT FOUND[/green]",
                 f"Exact match found: 0, Others found: {others_total}",
             )
 
         # Create Verbose Table
         if others:
             for items in others:
```

### Comparing `pynamer-2.0.3/src/pynamer/utils.py` & `pynamer-2.1.0/src/pynamer/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 # Local modules
 from . import logger, project_count_file_trv, pypi_index_file_trv
 from .config import config
 
 
 def _check_integrity() -> None:
-    pass
+    pass  # pragma: no cover
 
 
 def _reset() -> None:
-    pass
+    pass  # pragma: no cover
 
 
 def _feedback(message: str, feedback_type: str) -> None:
     """Generates a formatted messages appropriate to the message type.
 
     Args:
         message:        Text to be echoed.
@@ -57,14 +57,37 @@
                 + Back.BLACK
                 + Style.BRIGHT
                 + f"ERROR: {message}"
                 + Style.RESET_ALL
             )
 
 
+def _search_json(json_data: dict, project_name: str) -> list:
+    github_links = []
+    pattern = re.compile(r"https?://github.com/[\w\-/]+")
+
+    def check_value(value: dict) -> None:
+        if isinstance(value, str):
+            match = pattern.search(value)
+            if match and value.endswith(project_name):
+                github_links.append(match.group(0))
+                return
+
+        elif isinstance(value, list):
+            for item in value:
+                check_value(item)
+
+        elif isinstance(value, dict):
+            for val in value.values():
+                check_value(val)
+
+    check_value(json_data)
+    return github_links
+
+
 def _find_pypirc_file(filename: str = ".pypirc") -> None:
     """Function to iterate over paths in the PATH environment variable to find a file.
 
      Designed to find a .pypirc file starting with the current working directory.
      If identified will update the config.pypirc variable, so it can be used elsewhere.
 
     Args:
```

### Comparing `pynamer-2.0.3/src/pynamer/validators.py` & `pynamer-2.1.0/src/pynamer/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 import string
 from datetime import datetime
 from typing import Any, Union
 
 # Third party modules
 import requests
 from bs4 import BeautifulSoup
+from dateutil.parser import isoparse
 from rich.console import Console
 from rich.table import Table
 
 # Local modules
 from . import logger, pypi_index_file_trv
 from .config import config
-from .utils import _generate_pypi_index
+from .utils import _generate_pypi_index, _search_json
 
 
 def _is_valid_package_name(project_name: str) -> bool:
     """Function does a basic check of project name validity.
 
     Args:
         project_name:   the name of the project to test.
@@ -32,14 +33,71 @@
     pattern = r"^[a-z][_\-a-z0-9]*$"
     if re.match(pattern, project_name) is not None:
         return True
     else:
         return False
 
 
+def _get_homepage(project_json: dict, project_name: str) -> tuple[str, str]:
+    home_url = project_json["info"]["home_page"]
+
+    if "github.com" in home_url and home_url.endswith(project_name):
+        return "".join(["Homepage: ", home_url]), home_url
+
+    if "github.io" in home_url:
+        for item in (".github.io", "https://"):
+            home_url = home_url.replace(item, "")
+        home_url = home_url.rstrip("/")
+        home_url = "".join([config.github_base_url, home_url])
+        return "".join(["Homepage: ", home_url]), home_url
+
+    homepages = _search_json(project_json, project_name)
+    for home_url in homepages:
+        if "github.com" in home_url and home_url.endswith(project_name):
+            return "".join(["Homepage: ", home_url]), home_url
+
+    if home_url != "":
+        return "".join(["Homepage: ", home_url]), home_url
+
+    return "Homepage: None", ""
+
+
+def _github_meta(url: str) -> str:
+    return_text = "\n\nGitHub Stats\n------------\n"
+    repo_api_url = "".join(
+        [config.github_api_url, url.replace(r"https://github.com/", "")]
+    )
+    try:
+        json_raw = requests.get(repo_api_url, timeout=5)
+    except requests.RequestException:
+        return "".join([return_text, "GitHub can not be contacted"])
+
+    if json_raw.status_code == 200:
+        repo_json = json_raw.json()
+        return "".join(
+            [
+                return_text,
+                f"stars:    {repo_json['stargazers_count']}",
+                "\n",
+                f"forks:    {repo_json['forks']}",
+                "\n",
+                f"license:  {repo_json['license']['name']}",
+                "\n",
+                f"watching: {repo_json['subscribers_count']}",
+                "\n",
+                f"created:  {isoparse(repo_json['created_at']).date()}",
+                "\n",
+                f"updated:  {isoparse(repo_json['updated_at']).date()}",
+            ]
+        )
+    if json_raw.status_code == 404:
+        return "".join([return_text, "repository does not exist"])
+    return ""
+
+
 def _ping_project(project_name: str) -> bool:
     """Determines if the URL to the project exists in PyPIs project area.
 
     Args:
         project_name:   the name of the project to test.
 
     Returns:
@@ -59,15 +117,15 @@
     if project_ping.status_code == 200:
         logger.debug("%s FOUND in the project area of PyPI", project_name)
         return True
     logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
     return False
 
 
-def _ping_json(project_name: str) -> str:
+def _ping_json(project_name: str, stats: bool = False) -> str:
     """Collects some details about the project if it exists.
 
     Args:
         project_name:   the name of the project to test.
 
     Raises:
         SystemExit:     If any requests.RequestException occurs.
@@ -77,35 +135,43 @@
     try:
         project_json_raw = requests.get(url_json, timeout=5)
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
     if project_json_raw.status_code == 200:
         project_json = json.loads(project_json_raw.content)
+
+        homepage_text, homepage_url = _get_homepage(project_json, project_name)
+
         author = (
-            "".join(["Author:  ", project_json["info"]["author"]])
+            "".join(["Author:   ", project_json["info"]["author"]])
             if project_json["info"]["author"]
-            else "Author:  None"
+            else "Author:   None"
         )
         version = (
-            "".join(["Version: ", project_json["info"]["version"]])
+            "".join(["Version:  ", project_json["info"]["version"]])
             if project_json["info"]["version"]
-            else "Version: None"
+            else "Version:  None"
         )
         email = (
-            "".join(["Email:   ", project_json["info"]["author_email"]])
+            "".join(["Email:    ", project_json["info"]["author_email"]])
             if project_json["info"]["author_email"]
-            else "Email:   None"
+            else "Email:    None"
         )
         summary = (
-            "".join(["Summary: ", project_json["info"]["summary"]])
+            "".join(["Summary:  ", project_json["info"]["summary"]])
             if project_json["info"]["summary"]
-            else "Summary: None"
+            else "Summary:  None"
         )
-        result = "".join([summary, "\n", author, "\n", email, "\n", version])
+        result = "".join(
+            [summary, "\n", author, "\n", email, "\n", version, "\n", homepage_text]
+        )
+
+        if "github" in homepage_url and stats is True:
+            result = "".join([result, _github_meta(homepage_url)])
         return result
     logger.debug("No response from JSON URL")
     return ""
 
 
 def _pypi_search_index(project_name: str) -> bool:
     """Open the generated index file and search for the project name.
```

### Comparing `pynamer-2.0.3/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.0/src/pynamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.3
+Version: 2.1.0
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -21,15 +21,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.md
 
 _**Utility to find an available package name in the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
```

### Comparing `pynamer-2.0.3/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.0/src/pynamer.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,17 +29,20 @@
 tests/test_create_setup_file.py
 tests/test_defaults.py
 tests/test_delete_director.py
 tests/test_feedback.py
 tests/test_final_analysis.py
 tests/test_find_pypirc_file.py
 tests/test_generate_pypi_index.py
+tests/test_get_homepage.py
+tests/test_github_meta.py
 tests/test_is_valid_package_name.py
 tests/test_ping_json.py
 tests/test_ping_project.py
 tests/test_process_input_file.py
 tests/test_pypi_search.py
 tests/test_pypi_search_index.py
 tests/test_rename_project_dir.py
 tests/test_upload_dist.py
+tests/test_utils_search_json.py
 tests/test_utils_version.py
 tests/test_write_output_file.py
```

### Comparing `pynamer-2.0.3/tests/test_args.py` & `pynamer-2.1.0/tests/test_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,112 @@
-#!/usr/bin/env python3
-# Core Library modules
-
-# Core Library modules
-
-
-# First party modules
-from pynamer import pynamer
-
-
-def test_default_args():
-    args, parser = pynamer._parse_args([])
-    assert args.projects == "None"
-    assert args.register is False
-    assert args.dryrun is False
-    assert args.file == "None"
-    assert args.output == "None"
-    assert args.nocleanup is False
-    assert args.verbose is False
-    assert args.generate is False
-
-
-def test_args_project():
-    args, parser = pynamer._parse_args(
-        [
-            "pynball",
-        ]
-    )
-    assert args.projects == ["pynball"]
-
-
-def test_args_projects():
-    args, parser = pynamer._parse_args(
-        [
-            "pynball",
-            "pizazz",
-        ]
-    )
-    assert args.projects == ["pynball", "pizazz"]
-
-
-def test_args_register():
-    args, parser = pynamer._parse_args(
-        [
-            "-r",
-        ]
-    )
-    assert args.register is True
-
-
-def test_args_dryrun():
-    args, parser = pynamer._parse_args(
-        [
-            "-d",
-        ]
-    )
-    assert args.dryrun is True
-
-
-def test_args_file():
-    args, parser = pynamer._parse_args(["-f", "input_file"])
-    assert args.file == "input_file"
-
-
-def test_args_output():
-    args, parser = pynamer._parse_args(["-o", "output_file"])
-    assert args.output == "output_file"
-
-
-def test_args_nocleanup():
-    args, parser = pynamer._parse_args(
-        [
-            "-n",
-        ]
-    )
-    assert args.nocleanup is True
-
-
-def test_args_verbose():
-    args, parser = pynamer._parse_args(
-        [
-            "-v",
-        ]
-    )
-    assert args.verbose is True
-
-
-def test_args_generate():
-    args, parser = pynamer._parse_args(
-        [
-            "-g",
-        ]
-    )
-    assert args.generate is True
+#!/usr/bin/env python3
+# Core Library modules
+
+# Core Library modules
+
+
+# First party modules
+from pynamer import pynamer
+
+
+def test_default_args():
+    args, parser = pynamer._parse_args([])
+    assert args.projects == "None"
+    assert args.register is False
+    assert args.dryrun is False
+    assert args.file == "None"
+    assert args.output == "None"
+    assert args.nocleanup is False
+    assert args.verbose is False
+    assert args.generate is False
+
+
+def test_args_project():
+    args, parser = pynamer._parse_args(
+        [
+            "pynball",
+        ]
+    )
+    assert args.projects == ["pynball"]
+
+
+def test_args_projects():
+    args, parser = pynamer._parse_args(
+        [
+            "pynball",
+            "pizazz",
+        ]
+    )
+    assert args.projects == ["pynball", "pizazz"]
+
+
+def test_args_register():
+    args, parser = pynamer._parse_args(
+        [
+            "-r",
+        ]
+    )
+    assert args.register is True
+
+
+def test_args_dryrun():
+    args, parser = pynamer._parse_args(
+        [
+            "-d",
+        ]
+    )
+    assert args.dryrun is True
+
+
+def test_args_file():
+    args, parser = pynamer._parse_args(["-f", "input_file"])
+    assert args.file == "input_file"
+
+
+def test_args_output():
+    args, parser = pynamer._parse_args(["-o", "output_file"])
+    assert args.output == "output_file"
+
+
+def test_args_nocleanup():
+    args, parser = pynamer._parse_args(
+        [
+            "-n",
+        ]
+    )
+    assert args.nocleanup is True
+
+
+def test_args_verbose():
+    args, parser = pynamer._parse_args(
+        [
+            "-v",
+        ]
+    )
+    assert args.verbose is True
+
+
+def test_args_generate():
+    args, parser = pynamer._parse_args(
+        [
+            "-g",
+        ]
+    )
+    assert args.generate is True
+
+
+def test_args_webbrowser():
+    args, parser = pynamer._parse_args(
+        [
+            "-w",
+        ]
+    )
+    assert args.webbrowser is True
+
+
+def test_args_stats():
+    args, parser = pynamer._parse_args(
+        [
+            "-s",
+        ]
+    )
+    assert args.stats is True
```

### Comparing `pynamer-2.0.3/tests/test_build_dist.py` & `pynamer-2.1.0/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_cleanup.py` & `pynamer-2.1.0/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_create_setup_file.py` & `pynamer-2.1.0/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_defaults.py` & `pynamer-2.1.0/tests/test_defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,8 +48,9 @@
     assert pynamer.config.original_project_name == "project_name"
     assert pynamer.config.no_cleanup is False
     assert pynamer.config.package_version == "0.0.0"
     assert pynamer.config.pypi_search_url == "https://pypi.org/search/"
     assert pynamer.config.pypi_project_url == "https://pypi.org/project/"
     assert pynamer.config.pypi_json_url == "https://pypi.org/pypi/"
     assert pynamer.config.pypi_simple_index_url == "https://pypi.org/simple/"
+    assert pynamer.config.github_api_url == "https://api.github.com/repos/"
     assert pynamer.config.idlemode == 0
```

### Comparing `pynamer-2.0.3/tests/test_delete_director.py` & `pynamer-2.1.0/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_feedback.py` & `pynamer-2.1.0/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_final_analysis.py` & `pynamer-2.1.0/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_find_pypirc_file.py` & `pynamer-2.1.0/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_generate_pypi_index.py` & `pynamer-2.1.0/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_ping_json.py` & `pynamer-2.1.0/tests/test_utils_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,56 +2,49 @@
 # Core Library modules
 import pickle
 from pathlib import Path
 
 # Third party modules
 import pytest
 import requests
+from colorama import Back, Fore, Style
 from requests.exceptions import ConnectTimeout
 
 # First party modules
-from pynamer import pynamer
+import pynamer
 
 BASE_DIR = Path(__file__).parents[0]
 
-expected_response_found = """Summary: Utility command line tool to manage python versions
-Author:  Stephen R A King
-Email:   sking.github@gmail.com
-Version: 1.5.5"""
-
 
 def my_custom_get_found(url, **kwargs):
-    # Implement your custom logic here
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynball.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def my_custom_get_not_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_zeedonk.pickle"
+    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynamer.pickle"
     _pickle_bytes = _pickle_file.read_bytes()
     pickle_content = pickle.loads(_pickle_bytes)
     return pickle_content
 
 
-def test_ping_json_found(monkeypatch):
+def test_utils_version_old(monkeypatch, capfd):
     monkeypatch.setattr(requests, "get", my_custom_get_found)
-    result = pynamer._ping_json("pynball")
-    assert result == expected_response_found
+    monkeypatch.setattr(pynamer, "__version__", "1.0.0")
+    result = f"{Fore.YELLOW}{Back.BLACK}{Style.BRIGHT}1.0.0 : (There is a newer version available: 1.1.0){Style.RESET_ALL}\n"
+    pynamer.utils._check_version()
+    captured = capfd.readouterr()
+    assert captured.out == result
 
 
-def test_ping_json_not_found(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_not_found)
-    result = pynamer._ping_json("zeedonk")
-    assert result == ""
+def test_utils_version(monkeypatch, capfd):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    monkeypatch.setattr(pynamer, "__version__", "1.1.0")
+    result = f"{Fore.GREEN}{Style.BRIGHT}1.1.0 : (You have the most recent version){Style.RESET_ALL}\n"
+    pynamer.utils._check_version()
+    captured = capfd.readouterr()
+    assert captured.out == result
 
 
 def test_ping_json_error(monkeypatch):
     def mock_requests_error(*args, **kwargs):
         raise ConnectTimeout("Connection timed out")
 
     monkeypatch.setattr(requests, "get", mock_requests_error)
-
     with pytest.raises(SystemExit) as excinfo:
-        pynamer._ping_json("pynball")
+        pypi_version, message, result = pynamer.utils._check_version()
     assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-2.0.3/tests/test_ping_project.py` & `pynamer-2.1.0/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_process_input_file.py` & `pynamer-2.1.0/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_pypi_search.py` & `pynamer-2.1.0/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_pypi_search_index.py` & `pynamer-2.1.0/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_rename_project_dir.py` & `pynamer-2.1.0/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_upload_dist.py` & `pynamer-2.1.0/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.3/tests/test_write_output_file.py` & `pynamer-2.1.0/tests/test_write_output_file.py`

 * *Files identical despite different names*

