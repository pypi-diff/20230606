# Comparing `tmp/pynamer-2.1.0.tar.gz` & `tmp/pynamer-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.1.0.tar", last modified: Tue Jun  6 14:08:37 2023, max compression
+gzip compressed data, was "pynamer-2.1.1.tar", last modified: Tue Jun  6 14:53:14 2023, max compression
```

## Comparing `pynamer-2.1.0.tar` & `pynamer-2.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.139580 pynamer-2.1.0/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.0/AUTHORS.md
--rw-rw-rw-   0        0        0    10298 2023-06-06 14:08:25.000000 pynamer-2.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.0/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    18770 2023-06-06 14:08:37.139580 pynamer-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    17213 2023-06-02 18:15:07.000000 pynamer-2.1.0/README.md
--rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1842 2023-06-06 14:08:37.139580 pynamer-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:08:36.954576 pynamer-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.023642 pynamer-2.1.0/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.0/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-06 14:08:25.000000 pynamer-2.1.0/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.0/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2354 2023-06-04 10:27:28.000000 pynamer-2.1.0/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      823 2023-06-04 16:16:48.000000 pynamer-2.1.0/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.039263 pynamer-2.1.0/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.0/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7639 2023-06-04 10:50:40.000000 pynamer-2.1.0/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.0/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.0/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.0/src/pynamer/utils.py
--rw-rw-rw-   0        0        0    10643 2023-06-06 14:04:47.000000 pynamer-2.1.0/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.039263 pynamer-2.1.0/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18770 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 14:08:36.000000 pynamer-2.1.0/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 14:08:37.139580 pynamer-2.1.0/tests/
--rw-rw-rw-   0        0        0     2063 2023-06-04 10:27:28.000000 pynamer-2.1.0/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.0/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.0/tests/test_get_homepage.py
--rw-rw-rw-   0        0        0     1927 2023-06-06 13:17:15.000000 pynamer-2.1.0/tests/test_github_meta.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.0/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.0/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.0/tests/test_utils_search_json.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.0/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.0/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:53:14.922544 pynamer-2.1.1/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.1/AUTHORS.md
+-rw-rw-rw-   0        0        0    10463 2023-06-06 14:53:03.000000 pynamer-2.1.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    18770 2023-06-06 14:53:14.922544 pynamer-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17213 2023-06-02 18:15:07.000000 pynamer-2.1.1/README.md
+-rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1860 2023-06-06 14:53:14.922544 pynamer-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:53:14.822245 pynamer-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 14:53:14.869129 pynamer-2.1.1/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.1/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-06 14:53:03.000000 pynamer-2.1.1/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.1/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2354 2023-06-04 10:27:28.000000 pynamer-2.1.1/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      823 2023-06-04 16:16:48.000000 pynamer-2.1.1/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:53:14.884748 pynamer-2.1.1/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.1/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7623 2023-06-06 14:49:53.000000 pynamer-2.1.1/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.1/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.1/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.1/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    10643 2023-06-06 14:04:47.000000 pynamer-2.1.1/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-06 14:53:14.884748 pynamer-2.1.1/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18770 2023-06-06 14:53:14.000000 pynamer-2.1.1/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-06-06 14:53:14.000000 pynamer-2.1.1/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 14:53:14.000000 pynamer-2.1.1/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 14:53:14.000000 pynamer-2.1.1/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2023-06-06 14:53:14.000000 pynamer-2.1.1/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 14:53:14.000000 pynamer-2.1.1/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 14:53:14.922544 pynamer-2.1.1/tests/
+-rw-rw-rw-   0        0        0     2063 2023-06-04 10:27:28.000000 pynamer-2.1.1/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.1/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.1/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     1927 2023-06-06 13:17:15.000000 pynamer-2.1.1/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.1/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.1/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.1/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.1/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.1/tests/test_write_output_file.py
```

### Comparing `pynamer-2.1.0/CHANGELOG.md` & `pynamer-2.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.1 (2023-06-06)
+### Fix
+* Missing dependencies ([`cd5027f`](https://github.com/Stephen-RA-King/pynamer/commit/cd5027fe5bbd95694658448b25ce5702f1fca986))
+
 ## v2.1.0 (2023-06-06)
 ### Feature
 * Option to display github statistics ([`4ce5654`](https://github.com/Stephen-RA-King/pynamer/commit/4ce5654dcc6447b0518de9fd64f4c15fc6258e0f))
 
 ## v2.0.3 (2023-06-02)
 ### Fix
 * Json formatting ([`892a454`](https://github.com/Stephen-RA-King/pynamer/commit/892a454d47c868973978e54be89f472ae351b455))
```

### Comparing `pynamer-2.1.0/LICENSE` & `pynamer-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/PKG-INFO` & `pynamer-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.0
+Version: 2.1.1
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-2.1.0/README.md` & `pynamer-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/pyproject.toml` & `pynamer-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/setup.cfg` & `pynamer-2.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -70,47 +70,48 @@
 00000450: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
 00000460: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
 00000470: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 00000480: 3d33 2e39 0d0a 696e 7374 616c 6c5f 7265  =3.9..install_re
 00000490: 7175 6972 6573 203d 200d 0a09 6273 340d  quires = ...bs4.
 000004a0: 0a09 6275 696c 640d 0a09 636f 6c6f 7261  ..build...colora
 000004b0: 6d61 0d0a 096a 696e 6a61 320d 0a09 7061  ma...jinja2...pa
-000004c0: 636b 6167 696e 670d 0a09 7079 7961 6d6c  ckaging...pyyaml
-000004d0: 0d0a 0972 6571 7565 7374 730d 0a09 7269  ...requests...ri
-000004e0: 6368 0d0a 0974 7164 6d0d 0a09 7477 696e  ch...tqdm...twin
-000004f0: 650d 0a09 7768 6565 6c0d 0a0d 0a5b 6f70  e...wheel....[op
-00000500: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000510: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000520: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
-00000530: 636b 6167 655f 6461 7461 5d0d 0a70 796e  ckage_data]..pyn
-00000540: 616d 6572 203d 200d 0a09 5245 4144 4d45  amer = ...README
-00000550: 2e6d 640d 0a09 636f 6e66 6967 2e70 790d  .md...config.py.
-00000560: 0a09 7072 6f6a 6563 745f 6e61 6d65 0d0a  ..project_name..
-00000570: 0970 726f 6a65 6374 5f6e 616d 652f 5f5f  .project_name/__
-00000580: 696e 6974 5f5f 2e70 790d 0a09 7365 7475  init__.py...setu
-00000590: 702e 7478 740d 0a09 7365 7475 705f 6261  p.txt...setup_ba
-000005a0: 7365 2e74 7874 0d0a 0975 7469 6c73 2e70  se.txt...utils.p
-000005b0: 790d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  y....[options.en
-000005c0: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-000005d0: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-000005e0: 0a09 7079 6e61 6d65 7220 3d20 7079 6e61  ..pynamer = pyna
-000005f0: 6d65 722e 7079 6e61 6d65 723a 6d61 696e  mer.pynamer:main
-00000600: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 646f  ....[flake8]..do
-00000610: 6373 7472 696e 672d 636f 6e76 656e 7469  cstring-conventi
-00000620: 6f6e 203d 206e 756d 7079 0d0a 6d61 782d  on = numpy..max-
-00000630: 636f 6d70 6c65 7869 7479 203d 2031 380d  complexity = 18.
-00000640: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
-00000650: 203d 2038 380d 0a73 656c 6563 7420 3d20   = 88..select = 
-00000660: 422c 2042 392c 2043 2c20 442c 2045 2c20  B, B9, C, D, E, 
-00000670: 462c 204e 2c20 570d 0a65 7863 6c75 6465  F, N, W..exclude
-00000680: 203d 2074 6573 7473 2f2a 2c2e 746f 782f   = tests/*,.tox/
-00000690: 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f 2a2c  *,.nox/*,docs/*,
-000006a0: 2e67 6974 2f2a 2c2e 6769 7468 7562 2f2a  .git/*,.github/*
-000006b0: 0d0a 6967 6e6f 7265 203d 200d 0a09 4532  ..ignore = ...E2
-000006c0: 3033 2c0d 0a09 5735 3033 2c0d 0a70 6572  03,...W503,..per
-000006d0: 2d66 696c 652d 6967 6e6f 7265 7320 3d20  -file-ignores = 
-000006e0: 0d0a 0970 796e 616d 6572 2e70 793a 4339  ...pynamer.py:C9
-000006f0: 3031 0d0a 0962 7569 6c64 6572 2e70 793a  01...builder.py:
-00000700: 4339 3031 0d0a 0d0a 5b65 6767 5f69 6e66  C901....[egg_inf
-00000710: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000720: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000730: 0d0a                                     ..
+000004c0: 636b 6167 696e 670d 0a09 7079 7468 6f6e  ckaging...python
+000004d0: 2d64 6174 6575 7469 6c0d 0a09 7079 7961  -dateutil...pyya
+000004e0: 6d6c 0d0a 0972 6571 7565 7374 730d 0a09  ml...requests...
+000004f0: 7269 6368 0d0a 0974 7164 6d0d 0a09 7477  rich...tqdm...tw
+00000500: 696e 650d 0a09 7768 6565 6c0d 0a0d 0a5b  ine...wheel....[
+00000510: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000520: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000530: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
+00000540: 7061 636b 6167 655f 6461 7461 5d0d 0a70  package_data]..p
+00000550: 796e 616d 6572 203d 200d 0a09 5245 4144  ynamer = ...READ
+00000560: 4d45 2e6d 640d 0a09 636f 6e66 6967 2e70  ME.md...config.p
+00000570: 790d 0a09 7072 6f6a 6563 745f 6e61 6d65  y...project_name
+00000580: 0d0a 0970 726f 6a65 6374 5f6e 616d 652f  ...project_name/
+00000590: 5f5f 696e 6974 5f5f 2e70 790d 0a09 7365  __init__.py...se
+000005a0: 7475 702e 7478 740d 0a09 7365 7475 705f  tup.txt...setup_
+000005b0: 6261 7365 2e74 7874 0d0a 0975 7469 6c73  base.txt...utils
+000005c0: 2e70 790d 0a0d 0a5b 6f70 7469 6f6e 732e  .py....[options.
+000005d0: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+000005e0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+000005f0: 200d 0a09 7079 6e61 6d65 7220 3d20 7079   ...pynamer = py
+00000600: 6e61 6d65 722e 7079 6e61 6d65 723a 6d61  namer.pynamer:ma
+00000610: 696e 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  in....[flake8]..
+00000620: 646f 6373 7472 696e 672d 636f 6e76 656e  docstring-conven
+00000630: 7469 6f6e 203d 206e 756d 7079 0d0a 6d61  tion = numpy..ma
+00000640: 782d 636f 6d70 6c65 7869 7479 203d 2031  x-complexity = 1
+00000650: 380d 0a6d 6178 2d6c 696e 652d 6c65 6e67  8..max-line-leng
+00000660: 7468 203d 2038 380d 0a73 656c 6563 7420  th = 88..select 
+00000670: 3d20 422c 2042 392c 2043 2c20 442c 2045  = B, B9, C, D, E
+00000680: 2c20 462c 204e 2c20 570d 0a65 7863 6c75  , F, N, W..exclu
+00000690: 6465 203d 2074 6573 7473 2f2a 2c2e 746f  de = tests/*,.to
+000006a0: 782f 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f  x/*,.nox/*,docs/
+000006b0: 2a2c 2e67 6974 2f2a 2c2e 6769 7468 7562  *,.git/*,.github
+000006c0: 2f2a 0d0a 6967 6e6f 7265 203d 200d 0a09  /*..ignore = ...
+000006d0: 4532 3033 2c0d 0a09 5735 3033 2c0d 0a70  E203,...W503,..p
+000006e0: 6572 2d66 696c 652d 6967 6e6f 7265 7320  er-file-ignores 
+000006f0: 3d20 0d0a 0970 796e 616d 6572 2e70 793a  = ...pynamer.py:
+00000700: 4339 3031 0d0a 0962 7569 6c64 6572 2e70  C901...builder.p
+00000710: 793a 4339 3031 0d0a 0d0a 5b65 6767 5f69  y:C901....[egg_i
+00000720: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000730: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000740: 0d0a 0d0a                                ....
```

### Comparing `pynamer-2.1.0/src/pynamer/__init__.py` & `pynamer-2.1.1/src/pynamer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.1.0/src/pynamer/builder.py` & `pynamer-2.1.1/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/src/pynamer/cli.py` & `pynamer-2.1.1/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/src/pynamer/config.py` & `pynamer-2.1.1/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/src/pynamer/pynamer.py` & `pynamer-2.1.1/src/pynamer/pynamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     args, parser = _parse_args(sys.argv[1:])
     logger.debug(" args: %s", args)
 
     if args.generate:
         _generate_pypi_index()
 
     if args.version:
-        _check_version()  # type: ignore
+        _check_version()
 
     if args.projects == "None" and args.file == "None" and args.register:
         _feedback("You need to specify a project name to register it", "error")
         raise SystemExit()
 
     if args.projects == "None" and args.file == "None" and args.meta:
         _feedback(
```

### Comparing `pynamer-2.1.0/src/pynamer/utils.py` & `pynamer-2.1.1/src/pynamer/utils.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/src/pynamer/validators.py` & `pynamer-2.1.1/src/pynamer/validators.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.1/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.0
+Version: 2.1.1
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-2.1.0/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.1/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_args.py` & `pynamer-2.1.1/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_build_dist.py` & `pynamer-2.1.1/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_cleanup.py` & `pynamer-2.1.1/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_create_setup_file.py` & `pynamer-2.1.1/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_defaults.py` & `pynamer-2.1.1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_delete_director.py` & `pynamer-2.1.1/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_feedback.py` & `pynamer-2.1.1/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_final_analysis.py` & `pynamer-2.1.1/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_find_pypirc_file.py` & `pynamer-2.1.1/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_generate_pypi_index.py` & `pynamer-2.1.1/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_get_homepage.py` & `pynamer-2.1.1/tests/test_get_homepage.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_github_meta.py` & `pynamer-2.1.1/tests/test_github_meta.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_ping_json.py` & `pynamer-2.1.1/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_ping_project.py` & `pynamer-2.1.1/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_process_input_file.py` & `pynamer-2.1.1/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_pypi_search.py` & `pynamer-2.1.1/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_pypi_search_index.py` & `pynamer-2.1.1/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_rename_project_dir.py` & `pynamer-2.1.1/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_upload_dist.py` & `pynamer-2.1.1/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_utils_search_json.py` & `pynamer-2.1.1/tests/test_utils_search_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_utils_version.py` & `pynamer-2.1.1/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.0/tests/test_write_output_file.py` & `pynamer-2.1.1/tests/test_write_output_file.py`

 * *Files identical despite different names*

