# Comparing `tmp/mpacklog-2.0.0.tar.gz` & `tmp/mpacklog-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpacklog-2.0.0.tar", last modified: Thu Sep  1 10:30:54 2022, max compression
+gzip compressed data, was "mpacklog-3.0.0.tar", last modified: Tue Jun  6 15:05:58 2023, max compression
```

## Comparing `mpacklog-2.0.0.tar` & `mpacklog-3.0.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
--rw-r--r--   0        0        0      654 2022-08-17 08:35:13.643458 mpacklog-2.0.0/.bazelrc
--rw-r--r--   0        0        0     4523 2022-08-17 08:18:50.613221 mpacklog-2.0.0/.clang-format
--rw-r--r--   0        0        0     1631 2022-08-23 22:01:35.302377 mpacklog-2.0.0/.github/workflows/bazel.yml
--rw-r--r--   0        0        0      386 2022-08-23 12:06:37.953764 mpacklog-2.0.0/.gitignore
--rw-r--r--   0        0        0      490 2022-08-23 21:41:50.059009 mpacklog-2.0.0/BUILD
--rw-r--r--   0        0        0      358 2022-09-01 08:18:46.337508 mpacklog-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      902 2022-08-17 08:14:43.722246 mpacklog-2.0.0/CPPLINT.cfg
--rw-r--r--   0        0        0   112700 2022-09-01 10:30:27.977615 mpacklog-2.0.0/Doxyfile
--rw-r--r--   0        0        0    11357 2022-08-17 08:09:56.237259 mpacklog-2.0.0/LICENSE
--rw-r--r--   0        0        0     3234 2022-09-01 10:21:28.280852 mpacklog-2.0.0/README.md
--rw-r--r--   0        0        0      740 2022-08-17 08:39:36.371066 mpacklog-2.0.0/WORKSPACE
--rw-r--r--   0        0        0      772 2022-09-01 08:05:25.877590 mpacklog-2.0.0/__init__.py
--rw-r--r--   0        0        0      456 2022-08-17 09:12:22.361261 mpacklog-2.0.0/doc/Makefile
--rw-r--r--   0        0        0    53061 2022-08-17 09:11:14.828090 mpacklog-2.0.0/doc/doxygen-awesome.css
--rw-r--r--   0        0        0      205 2022-08-23 21:35:09.964549 mpacklog-2.0.0/mpacklog/BUILD
--rw-r--r--   0        0        0      786 2022-09-01 10:30:21.472338 mpacklog-2.0.0/mpacklog/__init__.py
--rw-r--r--   0        0        0     4008 2022-08-23 16:41:34.555528 mpacklog-2.0.0/mpacklog/cli/__init__.py
--rw-r--r--   0        0        0     1741 2022-08-23 16:29:24.463557 mpacklog-2.0.0/mpacklog/cli/csv_printer.py
--rw-r--r--   0        0        0     1585 2022-08-23 16:09:56.815338 mpacklog-2.0.0/mpacklog/cli/field_printer.py
--rw-r--r--   0        0        0     4707 2022-08-23 15:54:00.400600 mpacklog-2.0.0/mpacklog/cli/fields.py
--rw-r--r--   0        0        0     1457 2022-08-23 16:10:06.871369 mpacklog-2.0.0/mpacklog/cli/json_printer.py
--rw-r--r--   0        0        0     1182 2022-08-23 16:09:45.463302 mpacklog-2.0.0/mpacklog/cli/printer.py
--rw-r--r--   0        0        0     5000 2022-08-23 16:39:10.865264 mpacklog-2.0.0/mpacklog/cli/script_printer.py
--rw-r--r--   0        0        0      777 2022-09-01 10:25:31.734252 mpacklog-2.0.0/mpacklog/cpp/BUILD
--rw-r--r--   0        0        0     2828 2022-09-01 10:25:31.734252 mpacklog-2.0.0/mpacklog/cpp/CircularBuffer.h
--rw-r--r--   0        0        0     2243 2022-09-01 10:25:31.734252 mpacklog-2.0.0/mpacklog/cpp/Logger.cpp
--rw-r--r--   0        0        0     4188 2022-09-01 10:25:31.738252 mpacklog-2.0.0/mpacklog/cpp/Logger.h
--rw-r--r--   0        0        0      389 2022-09-01 10:25:31.738252 mpacklog-2.0.0/mpacklog/cpp/tests/BUILD
--rw-r--r--   0        0        0     1385 2022-09-01 10:25:31.738252 mpacklog-2.0.0/mpacklog/cpp/tests/CircularBufferTest.cpp
--rw-r--r--   0        0        0      807 2022-09-01 10:25:31.738252 mpacklog-2.0.0/mpacklog/cpp/tests/LoggerTest.cpp
--rw-r--r--   0        0        0      329 2022-09-01 08:06:12.758255 mpacklog-2.0.0/mpacklog/python/BUILD
--rw-r--r--   0        0        0      749 2022-09-01 08:05:45.974272 mpacklog-2.0.0/mpacklog/python/__init__.py
--rw-r--r--   0        0        0     1737 2022-09-01 08:16:31.034214 mpacklog-2.0.0/mpacklog/python/logger.py
--rw-r--r--   0        0        0     1416 2022-08-23 21:54:01.781789 mpacklog-2.0.0/mpacklog/python/serialize.py
--rw-r--r--   0        0        0      447 2022-09-01 08:13:08.180921 mpacklog-2.0.0/mpacklog/python/tests/BUILD
--rw-r--r--   0        0        0     1439 2022-09-01 08:18:12.258700 mpacklog-2.0.0/mpacklog/python/tests/logger_test.py
--rw-r--r--   0        0        0     1283 2022-08-23 21:56:14.390108 mpacklog-2.0.0/mpacklog/python/tests/serialize_test.py
--rw-r--r--   0        0        0     1334 2022-08-23 21:51:54.973319 mpacklog-2.0.0/pyproject.toml
--rwxr-xr-x   0        0        0     1376 2022-08-17 08:10:52.182454 mpacklog-2.0.0/tools/bazelisk
--rw-r--r--   0        0        0      321 2022-08-17 08:10:52.182454 mpacklog-2.0.0/tools/lint/BUILD
--rw-r--r--   0        0        0     1966 2022-08-17 08:10:52.182454 mpacklog-2.0.0/tools/lint/clang_format_lint.py
--rw-r--r--   0        0        0     5481 2022-08-17 08:10:52.182454 mpacklog-2.0.0/tools/lint/cpplint.bzl
--rw-r--r--   0        0        0     1124 2022-08-17 08:10:52.182454 mpacklog-2.0.0/tools/lint/lint.bzl
--rw-r--r--   0        0        0      188 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/BUILD
--rw-r--r--   0        0        0      564 2022-08-17 08:11:47.019496 mpacklog-2.0.0/tools/workspace/default.bzl
--rw-r--r--   0        0        0      987 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/generate_file.bzl
--rw-r--r--   0        0        0     1862 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/github_archive.bzl
--rw-r--r--   0        0        0      426 2022-08-17 08:40:08.975488 mpacklog-2.0.0/tools/workspace/install_python_deps.bzl
--rw-r--r--   0        0        0      188 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/mypy_integration/BUILD
--rw-r--r--   0        0        0      125 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/mypy_integration/package.BUILD
--rw-r--r--   0        0        0      726 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/mypy_integration/repository.bzl
--rw-r--r--   0        0        0      188 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/palimpsest/BUILD
--rw-r--r--   0        0        0      439 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/palimpsest/repository.bzl
--rw-r--r--   0        0        0      121 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/pip_mpack_logs/BUILD
--rw-r--r--   0        0        0       34 2022-08-17 08:37:48.945639 mpacklog-2.0.0/tools/workspace/pip_mpack_logs/requirements.txt
--rw-r--r--   0        0        0      188 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/pycodestyle/BUILD
--rw-r--r--   0        0        0     1308 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/pycodestyle/package.BUILD
--rw-r--r--   0        0        0      529 2022-08-17 08:11:25.555102 mpacklog-2.0.0/tools/workspace/pycodestyle/repository.bzl
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 mpacklog-2.0.0/setup.py
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 mpacklog-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-03-07 11:10:44.266851 mpacklog-3.0.0/.bazelrc
+-rw-r--r--   0        0        0     4523 2023-03-07 11:10:44.266851 mpacklog-3.0.0/.clang-format
+-rw-r--r--   0        0        0     2088 2023-05-16 13:41:04.724887 mpacklog-3.0.0/.github/workflows/bazel.yml
+-rw-r--r--   0        0        0      398 2023-06-06 15:04:27.225112 mpacklog-3.0.0/.gitignore
+-rw-r--r--   0        0        0      490 2023-03-07 11:10:44.266851 mpacklog-3.0.0/BUILD
+-rw-r--r--   0        0        0      658 2023-06-06 15:05:34.143909 mpacklog-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      902 2023-03-07 11:10:44.266851 mpacklog-3.0.0/CPPLINT.cfg
+-rw-r--r--   0        0        0   112700 2023-04-26 08:26:46.182014 mpacklog-3.0.0/Doxyfile
+-rw-r--r--   0        0        0    11357 2023-03-07 11:10:44.270851 mpacklog-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3820 2023-06-06 15:04:27.225112 mpacklog-3.0.0/README.md
+-rw-r--r--   0        0        0      591 2023-05-16 13:41:04.724887 mpacklog-3.0.0/WORKSPACE
+-rw-r--r--   0        0        0      812 2023-06-06 15:04:27.225112 mpacklog-3.0.0/__init__.py
+-rw-r--r--   0        0        0      456 2023-03-07 11:10:44.270851 mpacklog-3.0.0/doc/Makefile
+-rw-r--r--   0        0        0    53061 2023-03-07 11:10:44.274851 mpacklog-3.0.0/doc/doxygen-awesome.css
+-rw-r--r--   0        0        0      174 2023-04-04 17:32:52.558347 mpacklog-3.0.0/mpacklog/BUILD
+-rw-r--r--   0        0        0      870 2023-06-06 15:04:27.225112 mpacklog-3.0.0/mpacklog/__init__.py
+-rw-r--r--   0        0        0     4008 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cli/__init__.py
+-rw-r--r--   0        0        0     1741 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cli/csv_printer.py
+-rw-r--r--   0        0        0     1585 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cli/field_printer.py
+-rw-r--r--   0        0        0     4707 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cli/fields.py
+-rw-r--r--   0        0        0     1457 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cli/json_printer.py
+-rw-r--r--   0        0        0     1182 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cli/printer.py
+-rw-r--r--   0        0        0     4969 2023-04-04 17:33:02.646222 mpacklog-3.0.0/mpacklog/cli/script_printer.py
+-rw-r--r--   0        0        0      746 2023-04-04 17:32:54.734320 mpacklog-3.0.0/mpacklog/cpp/BUILD
+-rw-r--r--   0        0        0     2828 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cpp/CircularBuffer.h
+-rw-r--r--   0        0        0     2314 2023-04-26 08:25:29.479855 mpacklog-3.0.0/mpacklog/cpp/Logger.cpp
+-rw-r--r--   0        0        0     4188 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cpp/Logger.h
+-rw-r--r--   0        0        0      358 2023-04-04 17:33:05.614186 mpacklog-3.0.0/mpacklog/cpp/tests/BUILD
+-rw-r--r--   0        0        0     1385 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cpp/tests/CircularBufferTest.cpp
+-rw-r--r--   0        0        0      807 2023-03-07 11:10:44.274851 mpacklog-3.0.0/mpacklog/cpp/tests/LoggerTest.cpp
+-rw-r--r--   0        0        0      471 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/BUILD
+-rw-r--r--   0        0        0      818 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/__init__.py
+-rw-r--r--   0        0        0     1742 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/async_logger.py
+-rw-r--r--   0        0        0     1416 2023-03-07 11:10:44.278851 mpacklog-3.0.0/mpacklog/python/serialize.py
+-rw-r--r--   0        0        0     1905 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/sync_logger.py
+-rw-r--r--   0        0        0      556 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/tests/BUILD
+-rw-r--r--   0        0        0     1465 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/tests/async_logger_test.py
+-rw-r--r--   0        0        0     1283 2023-03-07 11:10:44.278851 mpacklog-3.0.0/mpacklog/python/tests/serialize_test.py
+-rw-r--r--   0        0        0     1728 2023-06-06 15:04:27.229112 mpacklog-3.0.0/mpacklog/python/tests/sync_logger_test.py
+-rw-r--r--   0        0        0     1389 2023-05-16 13:22:32.194985 mpacklog-3.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1665 2023-06-06 15:04:27.229112 mpacklog-3.0.0/tools/bazelisk
+-rw-r--r--   0        0        0      321 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/lint/BUILD
+-rw-r--r--   0        0        0     1966 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/lint/clang_format_lint.py
+-rw-r--r--   0        0        0     5481 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/lint/cpplint.bzl
+-rw-r--r--   0        0        0     1123 2023-04-04 17:32:50.386374 mpacklog-3.0.0/tools/lint/lint.bzl
+-rw-r--r--   0        0        0      188 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/BUILD
+-rw-r--r--   0        0        0      441 2023-05-05 09:55:40.737571 mpacklog-3.0.0/tools/workspace/default.bzl
+-rw-r--r--   0        0        0      987 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/generate_file.bzl
+-rw-r--r--   0        0        0     1862 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/github_archive.bzl
+-rw-r--r--   0        0        0      426 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/install_python_deps.bzl
+-rw-r--r--   0        0        0      188 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/palimpsest/BUILD
+-rw-r--r--   0        0        0      439 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/palimpsest/repository.bzl
+-rw-r--r--   0        0        0      121 2023-05-16 13:41:04.724887 mpacklog-3.0.0/tools/workspace/pip_mpacklog/BUILD
+-rw-r--r--   0        0        0      425 2023-05-16 13:41:04.724887 mpacklog-3.0.0/tools/workspace/pip_mpacklog/parse_deps.bzl
+-rw-r--r--   0        0        0       50 2023-05-16 13:41:04.724887 mpacklog-3.0.0/tools/workspace/pip_mpacklog/requirements_lock.txt
+-rw-r--r--   0        0        0      188 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/pycodestyle/BUILD
+-rw-r--r--   0        0        0     1308 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/pycodestyle/package.BUILD
+-rw-r--r--   0        0        0      529 2023-03-07 11:10:44.278851 mpacklog-3.0.0/tools/workspace/pycodestyle/repository.bzl
+-rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 mpacklog-3.0.0/PKG-INFO
```

### Comparing `mpacklog-2.0.0/.bazelrc` & `mpacklog-3.0.0/.bazelrc`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 build --compilation_mode=fastbuild
-build --compiler=compiler
 build --copt="-Werror=return-type"
-build --cpu=k8
 build --cxxopt=-std=c++17
 
 coverage --combined_report=lcov
 coverage --compilation_mode=fastbuild
-coverage --compiler=compiler
 coverage --copt="-Werror=return-type"
-coverage --cpu=k8
 coverage --cxxopt=-std=c++17
 coverage --instrument_test_targets
 
 test --compilation_mode=fastbuild
-test --compiler=compiler
 test --copt="-Werror=return-type"
-test --cpu=k8
 test --cxxopt=-std=c++17
 test --test_output=errors
 
 # Run linter only, not unit tests
 # Usage: bazel test --config lint //...
 test:lint --build_tests_only
 test:lint --test_tag_filters=lint
```

### Comparing `mpacklog-2.0.0/.clang-format` & `mpacklog-3.0.0/.clang-format`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/.github/workflows/bazel.yml` & `mpacklog-3.0.0/.github/workflows/bazel.yml`

 * *Files 24% similar despite different names*

```diff
@@ -9,24 +9,36 @@
 
 jobs:
     build:
         runs-on: ${{ matrix.os }}
         strategy:
             fail-fast: false
             matrix:
-                os: [ubuntu-latest]
+                os: [ubuntu-latest, macos-latest]
         steps:
             - name: "Checkout sources"
               uses: actions/checkout@v2
 
-            - name: "Install Eigen and NumPy"
-              run: sudo apt-get install -y libeigen3-dev python3-numpy
+            - name: "Install Eigen (Linux)"
+              if: runner.os == 'Linux'
+              run: sudo apt-get install -y libeigen3-dev
+
+            - name: "Install Eigen (macOS)"
+              if: runner.os == 'macOS'
+              run: |
+                 brew update
+                 brew install eigen
+
+            - name: "Install Python"
+              uses: actions/setup-python@v4
+              with:
+                python-version: "3.10"
 
             - name: "Install PyPI dependencies"
-              run: pip install aiofiles msgpack
+              run: pip3 install clang-format numpy six
 
             - name: "Build the library"
               env:
                   BAZELISK_GITHUB_TOKEN: ${{ secrets.BAZELISK_GITHUB_TOKEN }}
               run: |
                   tools/bazelisk build //...
 
@@ -39,15 +51,17 @@
             - name: "Check unit tests"
               env:
                   BAZELISK_GITHUB_TOKEN: ${{ secrets.BAZELISK_GITHUB_TOKEN }}
               run: |
                   tools/bazelisk test //...
 
             - name: "Report test coverage"
+              if: runner.os == 'Linux'
               run: |
                   tools/bazelisk coverage --combined_report=lcov --instrument_test_targets //...
 
             - name: "Submit report to Coveralls"
+              if: runner.os == 'Linux'
               uses: coverallsapp/github-action@1.1.3
               with:
                   github-token: ${{ secrets.github_token }}
-                  path-to-lcov: bazel-out/_coverage/_coverage_report.dat
+                  path-to-lcov: ${{ github.workspace }}/bazel-out/_coverage/_coverage_report.dat
```

### Comparing `mpacklog-2.0.0/CPPLINT.cfg` & `mpacklog-3.0.0/CPPLINT.cfg`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/Doxyfile` & `mpacklog-3.0.0/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "mpacklog — Log dictionaries to file using MessagePack"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER         = v2.0.0
+PROJECT_NUMBER         = v2.1.0
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `mpacklog-2.0.0/LICENSE` & `mpacklog-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/README.md` & `mpacklog-3.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # mpacklog
 
-[![Build](https://img.shields.io/github/workflow/status/stephane-caron/mpacklog/Bazel)](https://github.com/stephane-caron/mpacklog/actions)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/mpacklog/bazel.yml?branch=main)](https://github.com/stephane-caron/mpacklog/actions)
 [![Coverage](https://coveralls.io/repos/github/stephane-caron/mpacklog/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/mpacklog?branch=main)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/mpacklog/)
-![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
-[![Release](https://img.shields.io/github/v/release/stephane-caron/mpacklog.svg?sort=semver)](https://github.com/stephane-caron/mpacklog/releases)
-<!-- ![Status](https://img.shields.io/pypi/status/mpacklog) -->
 
 Log dictionaries to MessagePack files in C++ and Python.
 
 ## Installation
 
-### Python
-
-```console
-pip install mpacklog
-```
+### C++ with Bazel
 
-### Bazel
+![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
+[![C++ release](https://img.shields.io/github/v/release/stephane-caron/mpacklog.svg?sort=semver)](https://github.com/stephane-caron/mpacklog/releases)
 
 Add a git repository rule to your Bazel ``WORKSPACE``:
 
 ```python
 load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")
 
 git_repository(
     name = "mpacklog",
     remote = "https://github.com/stephane-caron/mpacklog.git",
-    tag = "v1.0.0",
+    tag = "v2.0.0",
 )
 ```
 
 You can then use the ``@mpacklog`` dependency for C++ targets, or the
 ``@mpacklog//:python`` dependency for Python targets.
 
+### Python
+
+[![PyPI version](https://img.shields.io/pypi/v/mpacklog)](https://pypi.org/project/mpacklog/)
+[![PyPI downloads](https://static.pepy.tech/badge/mpacklog)](https://pepy.tech/project/mpacklog)
+
+```console
+$ pip install mpacklog
+```
+
 ## Usage
 
 ### C++
 
 The C++ implementation uses multi-threading. Add messages to the log using the [`put`](https://scaron.info/doc/mpacklog/classmpacklog_1_1Logger.html#af0c278a990b1275b306e89013bb1fac6) function, they will be written to file in the background.
 
 ```cpp
@@ -54,38 +57,55 @@
         logger.put(dict):
     }
 }
 ```
 
 ### Python
 
-The Python implementation uses asynchronous I/O. Add messages to the log using the [`put`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#aa0f928ac07280acd132627d8545a7e18) function, have them written to file in the separate [`write`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#acbea9c05c465423efc3f38a25ed699d2) coroutine.
+The Python implementation provides both a synchronous and an asynchronous API. 
+
+#### Asynchronous API
+Add messages to the log using the [`put`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#aa0f928ac07280acd132627d8545a7e18) function, have them written to file in the separate [`write`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#acbea9c05c465423efc3f38a25ed699d2) coroutine.
 
 ```python
 import asyncio
 import mpacklog
 
 async def main():
-    logger = mpacklog.Logger("output.mpack")
-
-    await asyncio.gather(
-        main_loop(logger),
-        logger.write(),
-    )
+    logger = mpacklog.AsyncLogger("output.mpack")
+    await asyncio.gather(main_loop(logger), logger.write())
 
 async def main_loop(logger):
     for bar in range(1000):
         await asyncio.sleep(1e-3)
         await logger.put({"foo": bar, "something": "else"})
     await logger.stop()
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+#### Synchronous API
+The Synchronous API is very similar to the Asynchronous API, except it doesn't provide a ``stop`` method and the 
+``put`` and ``write`` methods are blocking.
+
+```python
+import mpacklog
+
+logger = mpacklog.SyncLogger("output.mpack")
+
+for bar in range(1000):
+    logger.put({"foo": bar, "something": "else"})
+
+# Flush all messages to the file
+logger.write()
+
+```
+
 ## Command-line
 
 If you ``pip``-installed mpacklog, you can use the ``mpacklog`` command to dump logs to JSON:
 
 ```console
 mpacklog dump my_log.mpack
 ```
```

### Comparing `mpacklog-2.0.0/WORKSPACE` & `mpacklog-3.0.0/WORKSPACE`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # -*- python -*-
 #
 # Copyright 2022 Stéphane Caron
 
 workspace(name = "mpacklog")
 
-BAZEL_VERSION = "4.1.0"
-BAZEL_VERSION_SHA_HOST = "0eb2e378d2782e7810753e2162245ad1179c1bb12f848c692b4a595b4edf779b"
-BAZEL_VERSION_SHA_PI = "02fcc51686a2f7b360a629747134d62dec885012454fac4c8634fc525884201f"
-
 load("//tools/workspace:default.bzl", "add_default_repositories")
 add_default_repositories()
 
 # @palimpsest is a default repository
 load("@palimpsest//tools/workspace:default.bzl", add_palimpsest_repositories = "add_default_repositories")
 add_palimpsest_repositories()
 
 # We can load this now that @rules_python has been added as a @palimpsest repository
-load("//tools/workspace:install_python_deps.bzl", "install_python_deps")
-install_python_deps()
+load("//tools/workspace/pip_mpacklog:parse_deps.bzl", "parse_deps")
+parse_deps()
+load("@pip_mpacklog//:requirements.bzl", "install_deps")
+install_deps()
```

### Comparing `mpacklog-2.0.0/__init__.py` & `mpacklog-3.0.0/mpacklog/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,12 +15,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Log dictionaries to file using the MessagePack serialization format.
 """
 
-from .mpacklog.python import Logger
+__version__ = "3.0.0"
+
+from .python.async_logger import AsyncLogger
+from .python.sync_logger import SyncLogger
 
 __all__ = [
-    "Logger",
+    "AsyncLogger",
+    "SyncLogger",
 ]
```

### Comparing `mpacklog-2.0.0/doc/doxygen-awesome.css` & `mpacklog-3.0.0/doc/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/__init__.py` & `mpacklog-3.0.0/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Log dictionaries to file using the MessagePack serialization format.
 """
 
-__version__ = "2.0.0"
-
-from .python import Logger
+from .mpacklog.python import AsyncLogger, SyncLogger
 
 __all__ = [
-    "Logger",
+    "AsyncLogger",
+    "SyncLogger",
 ]
```

### Comparing `mpacklog-2.0.0/mpacklog/cli/__init__.py` & `mpacklog-3.0.0/mpacklog/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cli/csv_printer.py` & `mpacklog-3.0.0/mpacklog/cli/csv_printer.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cli/field_printer.py` & `mpacklog-3.0.0/mpacklog/cli/field_printer.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cli/fields.py` & `mpacklog-3.0.0/mpacklog/cli/fields.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cli/json_printer.py` & `mpacklog-3.0.0/mpacklog/cli/json_printer.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cli/printer.py` & `mpacklog-3.0.0/mpacklog/cli/printer.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cli/script_printer.py` & `mpacklog-3.0.0/mpacklog/cli/script_printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     main = "start_ipython.py",
     data = ["{path.basename(data_file)}"],
     deps = [
         # add dependencies here
     ],
 )
 
-add_lint_tests(enable_clang_format_lint = True)"""
+add_lint_tests()"""
             )
         with open(main_file, "w") as output:
             output.write(
                 f"""#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Data extracted with `dump_log` from:
```

### Comparing `mpacklog-2.0.0/mpacklog/cpp/CircularBuffer.h` & `mpacklog-3.0.0/mpacklog/cpp/CircularBuffer.h`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cpp/Logger.cpp` & `mpacklog-3.0.0/mpacklog/cpp/Logger.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,19 @@
     flags |= std::ofstream::app;
   }
   file_.open(path, flags);
   if (!file_) {
     throw std::runtime_error("Cannot open " + path + " for writing");
   }
   thread_ = std::thread([this]() {
+#ifdef __APPLE__
+    pthread_setname_np("logger_thread");
+#else
     pthread_setname_np(pthread_self(), "logger_thread");
+#endif
     while (keep_going_) {
       flush_buffer();
 
       // The sleep duration doesn't have a big influence, no need to wake up
       // too often. This value assumes a > 1 ms long control period.
       std::this_thread::sleep_for(std::chrono::microseconds(100));
     }
```

### Comparing `mpacklog-2.0.0/mpacklog/cpp/Logger.h` & `mpacklog-3.0.0/mpacklog/cpp/Logger.h`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cpp/tests/CircularBufferTest.cpp` & `mpacklog-3.0.0/mpacklog/cpp/tests/CircularBufferTest.cpp`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/cpp/tests/LoggerTest.cpp` & `mpacklog-3.0.0/mpacklog/cpp/tests/LoggerTest.cpp`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/python/__init__.py` & `mpacklog-3.0.0/mpacklog/python/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,12 +15,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """!
 Python library for an agent to interact with a spine.
 """
 
-from .logger import Logger
+from .async_logger import AsyncLogger
+from .sync_logger import SyncLogger
 
 __all__ = [
-    "Logger",
+    "AsyncLogger",
+    "SyncLogger"
 ]
```

### Comparing `mpacklog-2.0.0/mpacklog/python/logger.py` & `mpacklog-3.0.0/mpacklog/python/async_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import aiofiles
 import msgpack
 
 from .serialize import serialize
 
 
-class Logger:
+class AsyncLogger:
 
     """!
     Logger with Asynchronous I/O.
     """
 
     def __init__(self, path):
         self.__keep_going = True
```

### Comparing `mpacklog-2.0.0/mpacklog/python/serialize.py` & `mpacklog-3.0.0/mpacklog/python/serialize.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/mpacklog/python/tests/logger_test.py` & `mpacklog-3.0.0/mpacklog/python/tests/async_logger_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 """
 
 import os
 import tempfile
 import unittest
 from unittest import IsolatedAsyncioTestCase
 
-from mpacklog.python.logger import Logger
+from mpacklog.python.async_logger import AsyncLogger
 
 
-class TestLogger(IsolatedAsyncioTestCase):
+class TestAsyncLogger(IsolatedAsyncioTestCase):
     async def test_put(self):
         tmp_file = tempfile.mktemp(suffix=".mpack")
-        logger = Logger(tmp_file)
+        logger = AsyncLogger(tmp_file)
         self.assertTrue(logger.queue.empty())
         await logger.put({"foo": 42, "something": "else"})
         self.assertFalse(logger.queue.empty())
 
     async def test_stop_and_write(self):
         tmp_file = tempfile.mktemp(suffix=".mpack")
         self.assertFalse(os.path.exists(tmp_file))
 
-        logger = Logger(tmp_file)
+        logger = AsyncLogger(tmp_file)
         await logger.stop()
         await logger.write()
         self.assertTrue(os.path.exists(tmp_file))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mpacklog-2.0.0/mpacklog/python/tests/serialize_test.py` & `mpacklog-3.0.0/mpacklog/python/tests/serialize_test.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/pyproject.toml` & `mpacklog-3.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
     "aiofiles >=0.7.0",
     "msgpack >=1.0.2",
 ]
+keywords = ["messagepack", "serialization", "logging"]
 
 [project.optional-dependencies]
 doc = ["sphinx"]
 
 [project.scripts]
 mpacklog = "mpacklog.cli:main"
```

### Comparing `mpacklog-2.0.0/tools/bazelisk` & `mpacklog-3.0.0/tools/bazelisk`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/bin/bash
 #
 # Copyright 2018 The Bazel Authors
 # Copyright 2022 Stéphane Caron
+# Copyright 2023 Inria
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,18 +31,26 @@
   esac
 done
 
 os="$(uname -s | tr "[:upper:]" "[:lower:]")"
 readonly os
 
 # Value of BAZELISK_GITHUB_TOKEN is set as a secret in the GitHub workflow.
-readonly bazelisk_version="v1.6.1"
-readonly url="https://github.com/bazelbuild/bazelisk/releases/download/${bazelisk_version}/bazelisk-${os}-amd64"
-bazel="${TMPDIR:-/tmp}/bazelisk"
+readonly BAZELISK_VERSION="v1.16.0"
+readonly BAZELISK_URL="https://github.com/bazelbuild/bazelisk/releases/download/${BAZELISK_VERSION}/bazelisk-${os}-amd64"
+
+readonly CURDIR=$(cd -- "$(dirname -- "${BASH_SOURCE[0]}")" &> /dev/null && pwd)
+
+bazel="${CURDIR}/bazel"
 readonly bazel
 
-curl -L -sSf -o "${bazel}" "${url}"
-chmod a+x "${bazel}"
+if [ -f "${bazel}" ]; then
+    echo "Using existing Bazel binary from ${bazel}..."
+else
+    echo "Downloading Bazel binary from ${BAZELISK_URL}..."
+    curl -L -Sf --progress-bar -o "${bazel}" "${BAZELISK_URL}"
+    chmod a+x "${bazel}"
+fi
 
 set -x
 "${bazel}" version
 "${bazel}" ${@:1:99}
```

### Comparing `mpacklog-2.0.0/tools/lint/clang_format_lint.py` & `mpacklog-3.0.0/tools/lint/clang_format_lint.py`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/tools/lint/cpplint.bzl` & `mpacklog-3.0.0/tools/lint/cpplint.bzl`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/tools/lint/lint.bzl` & `mpacklog-3.0.0/tools/lint/lint.bzl`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def add_lint_tests(
         cpplint_data = None,
         cpplint_extra_srcs = None,
         bazel_lint_ignore = None,
         bazel_lint_extra_srcs = None,
         bazel_lint_exclude = None,
-        enable_clang_format_lint = False):
+        enable_clang_format_lint = True):
     """
     For every rule in the BUILD file so far, and for all Bazel files in this
     directory, adds test rules that run Drake's standard lint suite over the
     sources.  Thus, BUILD file authors should call this function at the *end*
     of every BUILD file.
 
     Refer to the specific linters for their semantics and argument details:
```

### Comparing `mpacklog-2.0.0/tools/workspace/generate_file.bzl` & `mpacklog-3.0.0/tools/workspace/generate_file.bzl`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/tools/workspace/github_archive.bzl` & `mpacklog-3.0.0/tools/workspace/github_archive.bzl`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/tools/workspace/pycodestyle/package.BUILD` & `mpacklog-3.0.0/tools/workspace/pycodestyle/package.BUILD`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/tools/workspace/pycodestyle/repository.bzl` & `mpacklog-3.0.0/tools/workspace/pycodestyle/repository.bzl`

 * *Files identical despite different names*

### Comparing `mpacklog-2.0.0/PKG-INFO` & `mpacklog-3.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: mpacklog
-Version: 2.0.0
+Version: 3.0.0
 Summary: Log dictionaries to file using the MessagePack serialization format.
+Keywords: messagepack,serialization,logging
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -23,48 +24,51 @@
 Project-URL: Documentation, https://scaron.info/doc/mpacklog/
 Project-URL: Source, https://github.com/stephane-caron/mpacklog
 Project-URL: Tracker, https://github.com/stephane-caron/mpacklog/issues
 Provides-Extra: doc
 
 # mpacklog
 
-[![Build](https://img.shields.io/github/workflow/status/stephane-caron/mpacklog/Bazel)](https://github.com/stephane-caron/mpacklog/actions)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/mpacklog/bazel.yml?branch=main)](https://github.com/stephane-caron/mpacklog/actions)
 [![Coverage](https://coveralls.io/repos/github/stephane-caron/mpacklog/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/mpacklog?branch=main)
 [![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://scaron.info/doc/mpacklog/)
-![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
-[![Release](https://img.shields.io/github/v/release/stephane-caron/mpacklog.svg?sort=semver)](https://github.com/stephane-caron/mpacklog/releases)
-<!-- ![Status](https://img.shields.io/pypi/status/mpacklog) -->
 
 Log dictionaries to MessagePack files in C++ and Python.
 
 ## Installation
 
-### Python
-
-```console
-pip install mpacklog
-```
+### C++ with Bazel
 
-### Bazel
+![C++ version](https://img.shields.io/badge/C++-17/20-blue.svg?style=flat)
+[![C++ release](https://img.shields.io/github/v/release/stephane-caron/mpacklog.svg?sort=semver)](https://github.com/stephane-caron/mpacklog/releases)
 
 Add a git repository rule to your Bazel ``WORKSPACE``:
 
 ```python
 load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")
 
 git_repository(
     name = "mpacklog",
     remote = "https://github.com/stephane-caron/mpacklog.git",
-    tag = "v1.0.0",
+    tag = "v2.0.0",
 )
 ```
 
 You can then use the ``@mpacklog`` dependency for C++ targets, or the
 ``@mpacklog//:python`` dependency for Python targets.
 
+### Python
+
+[![PyPI version](https://img.shields.io/pypi/v/mpacklog)](https://pypi.org/project/mpacklog/)
+[![PyPI downloads](https://static.pepy.tech/badge/mpacklog)](https://pepy.tech/project/mpacklog)
+
+```console
+$ pip install mpacklog
+```
+
 ## Usage
 
 ### C++
 
 The C++ implementation uses multi-threading. Add messages to the log using the [`put`](https://scaron.info/doc/mpacklog/classmpacklog_1_1Logger.html#af0c278a990b1275b306e89013bb1fac6) function, they will be written to file in the background.
 
 ```cpp
@@ -81,38 +85,55 @@
         logger.put(dict):
     }
 }
 ```
 
 ### Python
 
-The Python implementation uses asynchronous I/O. Add messages to the log using the [`put`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#aa0f928ac07280acd132627d8545a7e18) function, have them written to file in the separate [`write`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#acbea9c05c465423efc3f38a25ed699d2) coroutine.
+The Python implementation provides both a synchronous and an asynchronous API. 
+
+#### Asynchronous API
+Add messages to the log using the [`put`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#aa0f928ac07280acd132627d8545a7e18) function, have them written to file in the separate [`write`](https://scaron.info/doc/mpacklog/classmpacklog_1_1mpacklog_1_1python_1_1logger_1_1Logger.html#acbea9c05c465423efc3f38a25ed699d2) coroutine.
 
 ```python
 import asyncio
 import mpacklog
 
 async def main():
-    logger = mpacklog.Logger("output.mpack")
-
-    await asyncio.gather(
-        main_loop(logger),
-        logger.write(),
-    )
+    logger = mpacklog.AsyncLogger("output.mpack")
+    await asyncio.gather(main_loop(logger), logger.write())
 
 async def main_loop(logger):
     for bar in range(1000):
         await asyncio.sleep(1e-3)
         await logger.put({"foo": bar, "something": "else"})
     await logger.stop()
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+#### Synchronous API
+The Synchronous API is very similar to the Asynchronous API, except it doesn't provide a ``stop`` method and the 
+``put`` and ``write`` methods are blocking.
+
+```python
+import mpacklog
+
+logger = mpacklog.SyncLogger("output.mpack")
+
+for bar in range(1000):
+    logger.put({"foo": bar, "something": "else"})
+
+# Flush all messages to the file
+logger.write()
+
+```
+
 ## Command-line
 
 If you ``pip``-installed mpacklog, you can use the ``mpacklog`` command to dump logs to JSON:
 
 ```console
 mpacklog dump my_log.mpack
 ```
```

