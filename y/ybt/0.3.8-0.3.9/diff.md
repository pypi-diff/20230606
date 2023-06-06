# Comparing `tmp/ybt-0.3.8.tar.gz` & `tmp/ybt-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ybt-0.3.8.tar", last modified: Thu Aug  2 09:13:35 2018, max compression
+gzip compressed data, was "dist/ybt-0.3.9.tar", last modified: Thu Aug  2 11:57:53 2018, max compression
```

## Comparing `ybt-0.3.8.tar` & `ybt-0.3.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:35.000000 ybt-0.3.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1842 2018-08-02 09:13:04.000000 ybt-0.3.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2559 2018-08-02 09:13:04.000000 ybt-0.3.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11360 2018-08-02 09:13:04.000000 ybt-0.3.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2018-08-02 09:13:04.000000 ybt-0.3.8/NOTICE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:35.000000 ybt-0.3.8/yabt/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8344 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/target_extraction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5581 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/target_utils_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26741 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/docker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9258 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/extend.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:35.000000 ybt-0.3.8/yabt/builders/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2186 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/apt_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2529 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/proto_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4552 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/docker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/alias.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6907 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/proto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5560 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/cpp_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15574 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/cpp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/fortests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1720 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/ruby.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/python_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1299 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/filegroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9946 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/custom_installer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/targetgroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/extcommand.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3377 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/grunt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3282 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/apt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1939 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/dockerapp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/nodejs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5042 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/builders/python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9821 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9469 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/target_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3209 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/pkgmgmt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      771 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/ybtbin.sh.tmpl
--rw-rw-r--   0 travis    (2000) travis    (2000)    12765 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5619 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5346 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/yabt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4293 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/docker_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8866 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/target_extraction_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11613 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/caching.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15371 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/graph_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5775 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/glob.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8405 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2884 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/extend_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/buildfile_parser_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2884 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/buildfile_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22713 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/buildcontext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/buildfile_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3328 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/scm.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:35.000000 ybt-0.3.8/yabt/scm_providers/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/scm_providers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1883 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/scm_providers/git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6120 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2051 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/utils_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1034 2018-08-02 09:13:04.000000 ybt-0.3.8/yabt/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2018-08-02 09:13:35.000000 ybt-0.3.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2018-08-02 09:13:04.000000 ybt-0.3.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      850 2018-08-02 09:13:35.000000 ybt-0.3.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      850 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      711 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2018-08-02 09:13:35.000000 ybt-0.3.8/ybt.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:53.000000 ybt-0.3.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1842 2018-08-02 11:57:19.000000 ybt-0.3.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2559 2018-08-02 11:57:19.000000 ybt-0.3.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11360 2018-08-02 11:57:19.000000 ybt-0.3.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      122 2018-08-02 11:57:19.000000 ybt-0.3.9/NOTICE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:53.000000 ybt-0.3.9/yabt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8344 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/target_extraction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5581 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/target_utils_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26741 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/docker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9258 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/extend.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:53.000000 ybt-0.3.9/yabt/builders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2186 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/apt_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2529 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/proto_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4552 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/docker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/alias.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6907 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/proto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5560 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/cpp_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15970 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/cpp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/fortests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1720 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/ruby.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/python_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1299 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/filegroup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9946 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/custom_installer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1049 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/targetgroup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1931 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/extcommand.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3377 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/grunt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3282 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/apt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1939 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/dockerapp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/nodejs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5042 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/builders/python.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9821 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9469 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/target_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3209 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/pkgmgmt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      789 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      771 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/ybtbin.sh.tmpl
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12765 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/graph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5619 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5346 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/yabt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4293 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/docker_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8866 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/target_extraction_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11613 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/caching.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15371 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/graph_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5775 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/glob.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8405 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2884 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/extend_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/buildfile_parser_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2884 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/buildfile_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22713 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/buildcontext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/buildfile_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3328 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/scm.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:53.000000 ybt-0.3.9/yabt/scm_providers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/scm_providers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1883 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/scm_providers/git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6120 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2051 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/utils_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1034 2018-08-02 11:57:19.000000 ybt-0.3.9/yabt/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2018-08-02 11:57:53.000000 ybt-0.3.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       88 2018-08-02 11:57:19.000000 ybt-0.3.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      850 2018-08-02 11:57:53.000000 ybt-0.3.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      850 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      711 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2018-08-02 11:57:53.000000 ybt-0.3.9/ybt.egg-info/SOURCES.txt
```

### Comparing `ybt-0.3.8/README.rst` & `ybt-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/setup.py` & `ybt-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/LICENSE` & `ybt-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/target_extraction.py` & `ybt-0.3.9/yabt/target_extraction.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/target_utils_test.py` & `ybt-0.3.9/yabt/target_utils_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/docker.py` & `ybt-0.3.9/yabt/docker.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/extend.py` & `ybt-0.3.9/yabt/extend.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/apt_test.py` & `ybt-0.3.9/yabt/builders/apt_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/proto_test.py` & `ybt-0.3.9/yabt/builders/proto_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/docker.py` & `ybt-0.3.9/yabt/builders/docker.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/alias.py` & `ybt-0.3.9/yabt/builders/alias.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/proto.py` & `ybt-0.3.9/yabt/builders/proto.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/cpp_test.py` & `ybt-0.3.9/yabt/builders/cpp_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/cpp.py` & `ybt-0.3.9/yabt/builders/cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,21 +74,27 @@
             'compile_flags', build_context.conf, target, []))
         self.link_flags = list(self.get(
             'link_flags', build_context.conf, target, []))
         self.include_path = list(self.get(
             'include_path', build_context.conf, target, []))
 
         def generate_extra_params():
-            yield from (dep.props.build_params
-                        for dep in build_context.generate_all_deps(target))
-            yield target.props.build_params
             if extra_params:
                 yield extra_params
+            yield target.props.build_params
+            # using topological order here because linker `-l<lib>` flags
+            # are sensitive to the order that they appear in!
+            # so if this target depends on, for example, both libsoft and
+            # libfftw, and also libsoft requires symbols that are defined in
+            # libfftw, then `-lfftw` must appear *after* `-lsoft`.
+            yield from (
+                dep.props.build_params for dep in
+                build_context.walk_target_deps_topological_order(target))
 
-        for build_params in generate_extra_params():
+        for build_params in reversed(list(generate_extra_params())):
             self.compile_flags.extend(
                 listify(build_params.get('extra_compile_flags')))
             self.link_flags.extend(
                 listify(build_params.get('extra_link_flags')))
 
     def as_dict(self):
         return {key: getattr(self, key)
```

### Comparing `ybt-0.3.8/yabt/builders/fortests.py` & `ybt-0.3.9/yabt/builders/fortests.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/ruby.py` & `ybt-0.3.9/yabt/builders/ruby.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/python_test.py` & `ybt-0.3.9/yabt/builders/python_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/filegroup.py` & `ybt-0.3.9/yabt/builders/filegroup.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/custom_installer.py` & `ybt-0.3.9/yabt/builders/custom_installer.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/targetgroup.py` & `ybt-0.3.9/yabt/builders/targetgroup.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/extcommand.py` & `ybt-0.3.9/yabt/builders/extcommand.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/grunt.py` & `ybt-0.3.9/yabt/builders/grunt.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/apt.py` & `ybt-0.3.9/yabt/builders/apt.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/dockerapp.py` & `ybt-0.3.9/yabt/builders/dockerapp.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/nodejs.py` & `ybt-0.3.9/yabt/builders/nodejs.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/builders/python.py` & `ybt-0.3.9/yabt/builders/python.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/cli.py` & `ybt-0.3.9/yabt/cli.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/target_utils.py` & `ybt-0.3.9/yabt/target_utils.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/pkgmgmt.py` & `ybt-0.3.9/yabt/pkgmgmt.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/__init__.py` & `ybt-0.3.9/yabt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 ~~~~~~~~~~~~~~~~~
 
 :author: Itamar Ostricher
 """
 
 
 __author__ = 'Itamar Ostricher'
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 __oneliner__ = 'Yet another Build Tool'
```

### Comparing `ybt-0.3.8/yabt/ybtbin.sh.tmpl` & `ybt-0.3.9/yabt/ybtbin.sh.tmpl`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/graph.py` & `ybt-0.3.9/yabt/graph.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/config.py` & `ybt-0.3.9/yabt/config.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/yabt.py` & `ybt-0.3.9/yabt/yabt.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/docker_test.py` & `ybt-0.3.9/yabt/docker_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/target_extraction_test.py` & `ybt-0.3.9/yabt/target_extraction_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/caching.py` & `ybt-0.3.9/yabt/caching.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/graph_test.py` & `ybt-0.3.9/yabt/graph_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/glob.py` & `ybt-0.3.9/yabt/glob.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/utils.py` & `ybt-0.3.9/yabt/utils.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/extend_test.py` & `ybt-0.3.9/yabt/extend_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/buildfile_parser_test.py` & `ybt-0.3.9/yabt/buildfile_parser_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/logging.py` & `ybt-0.3.9/yabt/logging.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/buildfile_utils.py` & `ybt-0.3.9/yabt/buildfile_utils.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/buildcontext.py` & `ybt-0.3.9/yabt/buildcontext.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/buildfile_parser.py` & `ybt-0.3.9/yabt/buildfile_parser.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/scm.py` & `ybt-0.3.9/yabt/scm.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/scm_providers/git.py` & `ybt-0.3.9/yabt/scm_providers/git.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/artifact.py` & `ybt-0.3.9/yabt/artifact.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/utils_test.py` & `ybt-0.3.9/yabt/utils_test.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/yabt/compat.py` & `ybt-0.3.9/yabt/compat.py`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/PKG-INFO` & `ybt-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybt
-Version: 0.3.8
+Version: 0.3.9
 Summary: Yet another Build Tool
 Home-page: https://yabt.ostrich.io/
 Author: Itamar Ostricher
 Author-email: yabt@ostricher.com
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ybt-0.3.8/ybt.egg-info/PKG-INFO` & `ybt-0.3.9/ybt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ybt
-Version: 0.3.8
+Version: 0.3.9
 Summary: Yet another Build Tool
 Home-page: https://yabt.ostrich.io/
 Author: Itamar Ostricher
 Author-email: yabt@ostricher.com
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ybt-0.3.8/ybt.egg-info/entry_points.txt` & `ybt-0.3.9/ybt.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ybt-0.3.8/ybt.egg-info/SOURCES.txt` & `ybt-0.3.9/ybt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

