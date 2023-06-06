# Comparing `tmp/eclipse_zenoh-0.7.0rc0.tar.gz` & `tmp/eclipse_zenoh-0.7.2rc0.tar.gz`

## Comparing `eclipse_zenoh-0.7.0rc0.tar` & `eclipse_zenoh-0.7.2rc0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 eclipse_zenoh-0.7.0rc0/Cargo.toml
--rw-r--r--   0      501       20     1088 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0      501       20      228 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0      501       20      878 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0      501       20     1384 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.github/workflows/ci.yml
--rw-r--r--   0      501       20     3611 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.github/workflows/release.yml
--rw-r--r--   0      501       20      569 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.gitignore
--rw-r--r--   0      501       20     1017 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/.readthedocs.yml
--rw-r--r--   0      501       20      119 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/CHANGELOG.md
--rw-r--r--   0      501       20     1692 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/CONTRIBUTING.md
--rw-r--r--   0      501       20      620 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/CONTRIBUTORS.md
--rw-r--r--   0      501       20    24371 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/LICENSE
--rw-r--r--   0      501       20       91 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/MANIFEST.in
--rw-r--r--   0      501       20     1253 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/NOTICE.md
--rw-r--r--   0      501       20     4719 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/README.md
--rw-r--r--   0      501       20      634 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/docs/Makefile
--rw-r--r--   0      501       20     3196 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/docs/conf.py
--rw-r--r--   0      501       20     2341 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/docs/index.rst
--rw-r--r--   0      501       20      795 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/docs/make.bat
--rw-r--r--   0      501       20      172 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/docs/requirements.txt
--rw-r--r--   0      501       20     4306 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/README.md
--rw-r--r--   0      501       20     2362 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_delete.py
--rw-r--r--   0      501       20     3268 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_get.py
--rw-r--r--   0      501       20     2161 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_info.py
--rw-r--r--   0      501       20     2821 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_pub.py
--rw-r--r--   0      501       20     2466 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_pub_thr.py
--rw-r--r--   0      501       20     2760 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_pull.py
--rw-r--r--   0      501       20     3441 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_put.py
--rw-r--r--   0      501       20     3255 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_queryable.py
--rw-r--r--   0      501       20      675 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_scout.py
--rw-r--r--   0      501       20     3550 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_storage.py
--rw-r--r--   0      501       20     3053 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_sub.py
--rw-r--r--   0      501       20     3210 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_sub_queued.py
--rw-r--r--   0      501       20     3418 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/examples/z_sub_thr.py
--rw-r--r--   0      501       20     1612 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/pyproject.toml
--rw-r--r--   0      501       20       20 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/requirements-dev.txt
--rw-r--r--   0      501       20        6 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/rust-toolchain
--rw-r--r--   0      501       20     2928 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/closures.rs
--rw-r--r--   0      501       20     2880 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/config.rs
--rw-r--r--   0      501       20    10404 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/enums.rs
--rw-r--r--   0      501       20     3068 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/keyexpr.rs
--rw-r--r--   0      501       20     3654 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/lib.rs
--rw-r--r--   0      501       20     2461 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/queryable.rs
--rw-r--r--   0      501       20    11201 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/session.rs
--rw-r--r--   0      501       20     8912 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/src/value.rs
--rw-r--r--   0      501       20     6950 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/tests/examples_check.py
--rw-r--r--   0      501       20     1726 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/__init__.py
--rw-r--r--   0      501       20     8803 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/closures.py
--rw-r--r--   0      501       20     1840 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/config.py
--rw-r--r--   0      501       20     8448 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/enums.py
--rw-r--r--   0      501       20     8008 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/keyexpr.py
--rw-r--r--   0      501       20     2506 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/queryable.py
--rw-r--r--   0      501       20    10303 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/session.py
--rw-r--r--   0      501       20     7126 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh/value.py
--rw-r--r--   0      501       20    33031 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/zenoh-dragon.png
--rw-r--r--   0      501       20    67898 2022-12-21 12:47:31.000000 eclipse_zenoh-0.7.0rc0/Cargo.lock
--rw-r--r--   0        0        0     6319 1970-01-01 00:00:00.000000 eclipse_zenoh-0.7.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 eclipse_zenoh-0.7.2rc0/Cargo.toml
+-rw-r--r--   0      501       20     1088 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0      501       20      228 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0      501       20      878 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0      501       20      656 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.github/release.yml
+-rw-r--r--   0      501       20     1384 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.github/workflows/ci.yml
+-rw-r--r--   0      501       20     3557 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.github/workflows/release.yml
+-rw-r--r--   0      501       20      569 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.gitignore
+-rw-r--r--   0      501       20     1017 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/.readthedocs.yml
+-rw-r--r--   0      501       20      119 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/CHANGELOG.md
+-rw-r--r--   0      501       20     1692 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/CONTRIBUTING.md
+-rw-r--r--   0      501       20      620 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/CONTRIBUTORS.md
+-rw-r--r--   0      501       20    24371 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/LICENSE
+-rw-r--r--   0      501       20       91 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/MANIFEST.in
+-rw-r--r--   0      501       20     1253 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/NOTICE.md
+-rw-r--r--   0      501       20     4704 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/README.md
+-rw-r--r--   0      501       20      634 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/docs/Makefile
+-rw-r--r--   0      501       20     3230 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/docs/conf.py
+-rw-r--r--   0      501       20     4251 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/docs/index.rst
+-rw-r--r--   0      501       20      795 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/docs/make.bat
+-rw-r--r--   0      501       20      173 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/docs/requirements.txt
+-rw-r--r--   0      501       20     3898 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/README.md
+-rw-r--r--   0      501       20     2362 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_delete.py
+-rw-r--r--   0      501       20     3272 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_get.py
+-rw-r--r--   0      501       20     2161 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_info.py
+-rw-r--r--   0      501       20     2821 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_pub.py
+-rw-r--r--   0      501       20     2466 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_pub_thr.py
+-rw-r--r--   0      501       20     2760 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_pull.py
+-rw-r--r--   0      501       20     3441 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_put.py
+-rw-r--r--   0      501       20     3250 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_queryable.py
+-rw-r--r--   0      501       20      632 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_scout.py
+-rw-r--r--   0      501       20     3550 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_storage.py
+-rw-r--r--   0      501       20     3053 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_sub.py
+-rw-r--r--   0      501       20     3210 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_sub_queued.py
+-rw-r--r--   0      501       20     3654 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/examples/z_sub_thr.py
+-rw-r--r--   0      501       20     1612 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/pyproject.toml
+-rw-r--r--   0      501       20       20 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/requirements-dev.txt
+-rw-r--r--   0      501       20        7 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/rust-toolchain
+-rw-r--r--   0      501       20     6042 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/closures.rs
+-rw-r--r--   0      501       20     2880 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/config.rs
+-rw-r--r--   0      501       20    10404 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/enums.rs
+-rw-r--r--   0      501       20     3068 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/keyexpr.rs
+-rw-r--r--   0      501       20     3694 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/lib.rs
+-rw-r--r--   0      501       20     2461 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/queryable.rs
+-rw-r--r--   0      501       20    11383 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/session.rs
+-rw-r--r--   0      501       20     9263 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/src/value.rs
+-rw-r--r--   0      501       20     6950 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/tests/examples_check.py
+-rw-r--r--   0      501       20     2522 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/__init__.py
+-rw-r--r--   0      501       20     9204 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/closures.py
+-rw-r--r--   0      501       20     1844 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/config.py
+-rw-r--r--   0      501       20     8452 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/enums.py
+-rw-r--r--   0      501       20     8168 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/keyexpr.py
+-rw-r--r--   0      501       20     2412 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/queryable.py
+-rw-r--r--   0      501       20    16599 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/session.py
+-rw-r--r--   0      501       20     7427 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh/value.py
+-rw-r--r--   0      501       20    33031 2023-06-06 15:02:19.000000 eclipse_zenoh-0.7.2rc0/zenoh-dragon.png
+-rw-r--r--   0      501       20    74800 2023-06-06 15:05:50.000000 eclipse_zenoh-0.7.2rc0/Cargo.lock
+-rw-r--r--   0        0        0     6335 1970-01-01 00:00:00.000000 eclipse_zenoh-0.7.2rc0/PKG-INFO
```

### Comparing `eclipse_zenoh-0.7.0rc0/Cargo.toml` & `eclipse_zenoh-0.7.2rc0/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -10,43 +10,50 @@
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 #
 # Contributors:
 #   ZettaScale Zenoh Team, <zenoh@zettascale.tech>
 #
 #
 [package]
-name = "eclipse-zenoh"
-version = "0.7.0-rc"
+name = "zenoh-python"
+version = "0.7.2-rc"
 authors = [
     "kydos <angelo@icorsaro.net>",
     "Julien Enoch <julien@enoch.fr>",
     "Olivier Hécart <olivier.hecart@adlinktech.com>",
     "Luca Cominardi <luca.cominardi@gmail.com>",
     "Pierre Avital <pierre.avital@adlinktech.com>",
 ]
-
-edition = "2018"
+edition = "2021"
+license = "EPL-2.0 OR Apache-2.0"
+categories = ["network-programming"]
+description = "The Zenoh Python API"
+readme = "README.md"
 
 [lib]
 name = "zenoh"
 crate-type = ["cdylib"]
 
 [features]
 complete_n = ["zenoh/complete_n"]
 
+[badges]
+maintenance = { status = "actively-developed" }
+
 [dependencies]
 async-std = "=1.12.0"
 env_logger = "0.10.0"
+flume = "0.10.14"
 form_urlencoded = "1.1.0"
-futures = "0.3.25"
+futures = "0.3.26"
 json5 = "0.4.1"
 log = "0.4.17"
-pyo3 = { version = "0.17.3", features = ["extension-module", "abi3-py37"] }
-serde_json = "1.0.89"
-uhlc = "0.5.1"
+pyo3 = { version = "0.18.1", features = ["extension-module", "abi3-py37"] }
+serde_json = "1.0.94"
+uhlc = "0.6.0"
 validated_struct = "2.1.0"
-zenoh = { version = "0.7.0-rc", features = [
+zenoh = { version = "0.7.2-rc", features = [
     "unstable",
 ] }
-zenoh-buffers = { version = "0.7.0-rc" }
-zenoh-cfg-properties = { version = "0.7.0-rc" }
-zenoh-core = { version = "0.7.0-rc" }
+zenoh-buffers = { version = "0.7.2-rc" }
+zenoh-cfg-properties = { version = "0.7.2-rc" }
+zenoh-core = { version = "0.7.2-rc" }
```

### Comparing `eclipse_zenoh-0.7.0rc0/.github/ISSUE_TEMPLATE/bug_report.yml` & `eclipse_zenoh-0.7.2rc0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/.github/ISSUE_TEMPLATE/feature_request.yml` & `eclipse_zenoh-0.7.2rc0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/.github/workflows/ci.yml` & `eclipse_zenoh-0.7.2rc0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/.github/workflows/release.yml` & `eclipse_zenoh-0.7.2rc0/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,14 @@
   linux-armv6:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v2
       - name: Install Rust toolchain
         uses: actions-rs/toolchain@v1
         with:
-          toolchain: stable
           profile: minimal
           target: arm-unknown-linux-gnueabihf
           default: true
       - name: install cross toolchain
         run: |
           brew tap messense/macos-cross-toolchains
           brew install arm-unknown-linux-gnueabihf
@@ -115,11 +114,10 @@
         with:
           name: wheels
           path: dist
       - name: Check dist
         run: ls -al ./dist/*
       - name: publish
         if: github.event_name == 'release' && github.event.action == 'published'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
-          user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `eclipse_zenoh-0.7.0rc0/.gitignore` & `eclipse_zenoh-0.7.2rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/.readthedocs.yml` & `eclipse_zenoh-0.7.2rc0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/CONTRIBUTING.md` & `eclipse_zenoh-0.7.2rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/CONTRIBUTORS.md` & `eclipse_zenoh-0.7.2rc0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/LICENSE` & `eclipse_zenoh-0.7.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/NOTICE.md` & `eclipse_zenoh-0.7.2rc0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/README.md` & `eclipse_zenoh-0.7.2rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,8 +85,8 @@
 
 
 -------------------------------
 ## Running the Examples
 
 The simplest way to run some of the example is to get a Docker image of the **zenoh** network router (see https://github.com/eclipse-zenoh/zenoh#how-to-test-it) and then to run the examples on your machine.
 
-Then, run the zenoh-python examples following the instructions in [examples/zenoh/README.md](https://github.com/eclipse-zenoh/zenoh-python/blob/master/examples/zenoh/README.md)
+Then, run the zenoh-python examples following the instructions in [examples/README.md](https://github.com/eclipse-zenoh/zenoh-python/tree/master/examples#readme)
```

### Comparing `eclipse_zenoh-0.7.0rc0/docs/Makefile` & `eclipse_zenoh-0.7.2rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/docs/conf.py` & `eclipse_zenoh-0.7.2rc0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'zenoh-python'
 copyright = '2020, ZettaScale Zenoh team, <zenoh@zettascale.tech>'
 author = 'ZettaScale Zenoh team, <zenoh@zettascale.tech>'
 
 # The full version, including alpha/beta/rc tags
-release = '0.7.0-rc'
+release = '0.7.2-rc'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -73,14 +73,15 @@
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', '**/*.rs']
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = None
 
+autodoc_typehints = "description"
 autodoc_mock_imports = ['zenoh']
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `eclipse_zenoh-0.7.0rc0/docs/make.bat` & `eclipse_zenoh-0.7.2rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/README.md` & `eclipse_zenoh-0.7.2rc0/examples/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -41,45 +41,45 @@
 
    Typical usage:
    ```bash
       python3 z_put.py
    ```
    or
    ```bash
-      python3 z_put.py -k /demo/example/test -v 'Hello World'
+      python3 z_put.py -k demo/example/test -v 'Hello World'
    ```
 
 ### z_pub
 
    Declares a resource with a path and a publisher on this resource. Then puts a value using the numerical resource id.
    The path/value will be received by all matching subscribers, for instance the [z_sub](#z_sub)
    and [z_storage](#z_storage) examples.
 
    Typical usage:
    ```bash
       python3 z_pub.py
    ```
    or
    ```bash
-      python3 z_pub.py -k /demo/example/test -v 'Hello World'
+      python3 z_pub.py -k demo/example/test -v 'Hello World'
    ```
 
 ### z_sub
 
    Creates a subscriber with a key expression.
    The subscriber will be notified of each put made on any key expression matching
    the subscriber's key expression, and will print this notification.
 
    Typical usage:
    ```bash
       python3 z_sub.py
    ```
    or
    ```bash
-      python3 z_sub.py -k '/demo/**'
+      python3 z_sub.py -k 'demo/**'
    ```
 
 ### z_pull
 
    Creates a pull subscriber with a selector.
    The pull subscriber will receive each put made on any key expression matching
    the subscriber's key expression and will pull on demand and print the received
@@ -87,45 +87,45 @@
 
    Typical usage:
    ```bash
       python3 z_pull.py
    ```
    or
    ```bash
-      python3 z_pull.py -k '/demo/**'
+      python3 z_pull.py -k 'demo/**'
    ```
 
 ### z_get
 
    Sends a query message for a selector.
    The queryables with a matching path or selector (for instance [z_queryable](#z_queryable) and [z_storage](#z_storage))
    will receive this query and reply with paths/values that will be received by the query callback.
 
    Typical usage:
    ```bash
       python3 z_get.py
    ```
    or
    ```bash
-      python3 z_get.py -s '/demo/**'
+      python3 z_get.py -s 'demo/**'
    ```
 
 ### z_queryable
 
    Creates a queryable function with a key expression.
    This queryable function will be triggered by each call to a get operation on zenoh
    with a selector that matches the key expression, and will return a value to the querier.
 
    Typical usage:
    ```bash
       python3 z_queryable.py
    ```
    or
    ```bash
-      python3 z_queryable.py -k /demo/example/queryable -v 'This is the result'
+      python3 z_queryable.py -k demo/example/queryable -v 'This is the result'
    ```
 
 ### z_storage
 
    Trivial implementation of a storage in memory.
    This examples creates a subscriber and a queryable on the same key expression.
    The subscriber callback will store the received key/values in an hashmap.
@@ -134,15 +134,15 @@
 
    Typical usage:
    ```bash
       python3 z_storage.py
    ```
    or
    ```bash
-      python3 z_storage.py -k '/demo/**'
+      python3 z_storage.py -k 'demo/**'
    ```
 
 ### z_pub_thr & z_sub_thr
 
    Pub/Sub throughput test.
    This example allows to perform throughput measurements between a pubisher performing
    put operations and a subscriber receiving notifications of those puts.
@@ -152,13 +152,7 @@
       python3 z_sub_thr.py
    ```
 
    Typical Publisher usage:
    ```bash
       python3 z_pub_thr.py 1024
    ```
-
-### asyncio
-
-In `asyncio` directory there are similar examples than thse described above, but leveraging Python's [asyncio](https://docs.python.org/fr/3/library/asyncio.html).
-
-Especially, the `asyncio/z_get_parallel.py` and `asyncio/z_queryable.py` examples show how a zenoh application can issue concurent queries and how another zenoh application can concurrently compute replies to those queries.
```

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_delete.py` & `eclipse_zenoh-0.7.2rc0/examples/z_delete.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_get.py` & `eclipse_zenoh-0.7.2rc0/examples/z_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,41 +51,42 @@
                     help='An optional value to send in the query.')
 parser.add_argument('--config', '-c', dest='config',
                     metavar='FILE',
                     type=str,
                     help='A configuration file.')
 
 args = parser.parse_args()
-conf = zenoh.Config.from_file(args.config) if args.config is not None else zenoh.Config()
+conf = zenoh.Config.from_file(
+    args.config) if args.config is not None else zenoh.Config()
 if args.mode is not None:
     conf.insert_json5(zenoh.config.MODE_KEY, json.dumps(args.mode))
 if args.connect is not None:
     conf.insert_json5(zenoh.config.CONNECT_KEY, json.dumps(args.connect))
 if args.listen is not None:
     conf.insert_json5(zenoh.config.LISTEN_KEY, json.dumps(args.listen))
 selector = args.selector
 target = {
     'ALL': QueryTarget.ALL(),
     'BEST_MATCHING': QueryTarget.BEST_MATCHING(),
     'ALL_COMPLETE': QueryTarget.ALL_COMPLETE(),
-    }.get(args.target)
+}.get(args.target)
 
 # Zenoh code  --- --- --- --- --- --- --- --- --- --- ---
 
 # initiate logging
 zenoh.init_logger()
 
 print("Opening session...")
 session = zenoh.open(conf)
 
 print("Sending Query '{}'...".format(selector))
-replies = session.get(selector, zenoh.ListCollector(), target=target, value=args.value)
-for reply in replies():
+replies = session.get(selector, zenoh.Queue(), target=target, value=args.value)
+for reply in replies.receiver:
     try:
         print(">> Received ('{}': '{}')"
-            .format(reply.ok.key_expr, reply.ok.payload.decode("utf-8")))
+              .format(reply.ok.key_expr, reply.ok.payload.decode("utf-8")))
     except:
         print(">> Received (ERROR: '{}')"
-            .format(reply.err.payload.decode("utf-8")))
+              .format(reply.err.payload.decode("utf-8")))
 
 
 session.close()
```

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_info.py` & `eclipse_zenoh-0.7.2rc0/examples/z_info.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_pub.py` & `eclipse_zenoh-0.7.2rc0/examples/z_pub.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_pub_thr.py` & `eclipse_zenoh-0.7.2rc0/examples/z_pub_thr.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_pull.py` & `eclipse_zenoh-0.7.2rc0/examples/z_pull.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_put.py` & `eclipse_zenoh-0.7.2rc0/examples/z_put.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_queryable.py` & `eclipse_zenoh-0.7.2rc0/examples/z_queryable.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,15 @@
                     help='Declare the queryable as complete w.r.t. the key expression.')
 parser.add_argument('--config', '-c', dest='config',
                     metavar='FILE',
                     type=str,
                     help='A configuration file.')
 
 args = parser.parse_args()
-conf = zenoh.Config.from_file(
-    args.config) if args.config is not None else zenoh.Config()
+conf = zenoh.Config.from_file(args.config) if args.config is not None else zenoh.Config()
 if args.mode is not None:
     conf.insert_json5(zenoh.config.MODE_KEY, json.dumps(args.mode))
 if args.connect is not None:
     conf.insert_json5(zenoh.config.CONNECT_KEY, json.dumps(args.connect))
 if args.listen is not None:
     conf.insert_json5(zenoh.config.LISTEN_KEY, json.dumps(args.listen))
 key = args.key
```

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_scout.py` & `eclipse_zenoh-0.7.2rc0/examples/z_scout.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,12 +16,9 @@
 
 # initiate logging
 zenoh.init_logger()
 
 print("Scouting...")
 scout = zenoh.scout(what = "peer|router", timeout=1.0)
 
-def dbg(x):
-    print(x)
-    return x
-for hello in dbg(scout.receiver()):
+for hello in scout.receiver():
     print(hello)
```

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_storage.py` & `eclipse_zenoh-0.7.2rc0/examples/z_storage.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_sub.py` & `eclipse_zenoh-0.7.2rc0/examples/z_sub.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_sub_queued.py` & `eclipse_zenoh-0.7.2rc0/examples/z_sub_queued.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/examples/z_sub_thr.py` & `eclipse_zenoh-0.7.2rc0/examples/z_sub_thr.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     print(f"Received {total} messages in {end - global_start}: averaged {total / (end - global_start):.6f} msgs/sec")
 
 # initiate logging
 zenoh.init_logger()
 
 session = zenoh.open(conf)
 
-sub = session.declare_subscriber("test/thr", (listener, report), reliability=Reliability.RELIABLE())
+# By explicitly constructing the `Closure`, the `Queue` that's normally inserted between the callback and zenoh is removed.
+# Only do this if your callback runs faster than the minimum expected delay between two samples.
+sub = session.declare_subscriber("test/thr", zenoh.Closure((listener, report)), reliability=Reliability.RELIABLE())
 
 print("Enter 'q' to quit...")
 c = '\0'
 while c != 'q':
     c = sys.stdin.read(1)
     if c == '':
         time.sleep(1)
```

### Comparing `eclipse_zenoh-0.7.0rc0/pyproject.toml` & `eclipse_zenoh-0.7.2rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/src/config.rs` & `eclipse_zenoh-0.7.2rc0/src/config.rs`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/src/enums.rs` & `eclipse_zenoh-0.7.2rc0/src/enums.rs`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/src/keyexpr.rs` & `eclipse_zenoh-0.7.2rc0/src/keyexpr.rs`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/src/lib.rs` & `eclipse_zenoh-0.7.2rc0/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         }
     }
 }
 
 #[pymodule]
 fn zenoh(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<config::_Config>()?;
+    m.add_class::<closures::_Queue>()?;
     m.add_class::<keyexpr::_KeyExpr>()?;
     m.add_class::<keyexpr::_Selector>()?;
     m.add_class::<session::_Session>()?;
     m.add_class::<session::_Publisher>()?;
     m.add_class::<session::_Subscriber>()?;
     m.add_class::<session::_PullSubscriber>()?;
     m.add_class::<session::_Scout>()?;
```

### Comparing `eclipse_zenoh-0.7.0rc0/src/queryable.rs` & `eclipse_zenoh-0.7.2rc0/src/queryable.rs`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/src/session.rs` & `eclipse_zenoh-0.7.2rc0/src/session.rs`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,16 @@
             *config = _Config(PyConfig::Notifier(session.config().clone()))
         }
         Ok(_Session(Arc::new(session)))
     }
     pub fn config(&self) -> _Config {
         _Config(PyConfig::Notifier(self.0.config().clone()))
     }
-    #[args(kwargs = "**")]
+
+    #[pyo3(signature = (key_expr, value, **kwargs))]
     pub fn put(
         &self,
         key_expr: &crate::keyexpr::_KeyExpr,
         value: &PyAny,
         kwargs: Option<&PyDict>,
     ) -> PyResult<()> {
         let s = &self.0;
@@ -85,15 +86,16 @@
                 Ok(priority) => builder = builder.priority(priority.0),
                 Err(crate::ExtractError::Other(e)) => return Err(e),
                 _ => {}
             }
         }
         builder.res_sync().map_err(|e| e.to_pyerr())
     }
-    #[args(kwargs = "**")]
+
+    #[pyo3(signature = (key_expr, **kwargs))]
     pub fn delete(
         &self,
         key_expr: &crate::keyexpr::_KeyExpr,
         kwargs: Option<&PyDict>,
     ) -> PyResult<()> {
         let s = &self.0;
         let k = &key_expr.0;
@@ -116,15 +118,15 @@
                 Err(crate::ExtractError::Other(e)) => return Err(e),
                 _ => {}
             }
         }
         builder.res_sync().map_err(|e| e.to_pyerr())
     }
 
-    #[args(kwargs = "**")]
+    #[pyo3(signature = (selector, callback, **kwargs))]
     pub fn get(
         &self,
         selector: &_Selector,
         callback: &PyAny,
         kwargs: Option<&PyDict>,
     ) -> PyResult<()> {
         let callback: PyClosure<(_Reply,)> = <_ as TryInto<_>>::try_into(callback)?;
@@ -152,15 +154,15 @@
     pub fn declare_keyexpr(&self, key_expr: &_KeyExpr) -> PyResult<_KeyExpr> {
         match self.0.declare_keyexpr(&key_expr.0).res_sync() {
             Ok(k) => Ok(_KeyExpr(k.into_owned())),
             Err(e) => Err(e.to_pyerr()),
         }
     }
 
-    #[args(kwargs = "**")]
+    #[pyo3(signature = (key_expr, callback, **kwargs))]
     pub fn declare_queryable(
         &self,
         key_expr: _KeyExpr,
         callback: &PyAny,
         kwargs: Option<&PyDict>,
     ) -> PyResult<_Queryable> {
         let callback: PyClosure<(_Query,)> = <_ as TryInto<_>>::try_into(callback)?;
@@ -174,15 +176,15 @@
         }
         match builder.res_sync() {
             Ok(o) => Ok(_Queryable(o)),
             Err(e) => Err(e.to_pyerr()),
         }
     }
 
-    #[args(kwargs = "**")]
+    #[pyo3(signature = (key_expr, **kwargs))]
     pub fn declare_publisher(
         &self,
         key_expr: _KeyExpr,
         kwargs: Option<&PyDict>,
     ) -> PyResult<_Publisher> {
         let mut builder = self.0.declare_publisher(key_expr.0);
         if let Some(kwargs) = kwargs {
@@ -199,15 +201,15 @@
         }
         match builder.res_sync() {
             Ok(o) => Ok(_Publisher(o)),
             Err(e) => Err(e.to_pyerr()),
         }
     }
 
-    #[args(kwargs = "**")]
+    #[pyo3(signature = (key_expr, callback, **kwargs))]
     pub fn declare_subscriber(
         &self,
         key_expr: &_KeyExpr,
         callback: &PyAny,
         kwargs: Option<&PyDict>,
     ) -> PyResult<_Subscriber> {
         let callback: PyClosure<(_Sample,)> = <_ as TryInto<_>>::try_into(callback)?;
@@ -219,15 +221,15 @@
                 _ => {}
             }
         }
         let subscriber = builder.res().map_err(|e| e.to_pyerr())?;
         Ok(_Subscriber(subscriber))
     }
 
-    #[args(kwargs = "**")]
+    #[pyo3(signature = (key_expr, callback, **kwargs))]
     pub fn declare_pull_subscriber(
         &self,
         key_expr: &_KeyExpr,
         callback: &PyAny,
         kwargs: Option<&PyDict>,
     ) -> PyResult<_PullSubscriber> {
         let callback: PyClosure<(_Sample,)> = <_ as TryInto<_>>::try_into(callback)?;
```

### Comparing `eclipse_zenoh-0.7.0rc0/src/value.rs` & `eclipse_zenoh-0.7.2rc0/src/value.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,28 @@
             Payload::Zenoh(buf) => buf,
             Payload::Python(buf) => Python::with_gil(|py| ZBuf::from(buf.as_bytes(py).to_owned())),
         }
     }
     pub(crate) fn into_pybytes(self) -> Py<PyBytes> {
         match self {
             Payload::Zenoh(buf) => {
-                Python::with_gil(|py| Py::from(PyBytes::new(py, buf.contiguous().as_ref())))
+                let len = buf.len();
+                Python::with_gil(|py| {
+                    Py::from(
+                        PyBytes::new_with(py, len, |mut bytes| {
+                            for slice in buf.slices() {
+                                let len = slice.len();
+                                bytes[..len].copy_from_slice(slice);
+                                bytes = &mut bytes[len..];
+                            }
+                            Ok(())
+                        })
+                        .unwrap(),
+                    )
+                })
             }
             Payload::Python(buf) => buf,
         }
     }
 }
 impl From<ZBuf> for Payload {
     fn from(buf: ZBuf) -> Self {
@@ -313,26 +326,22 @@
     #[getter]
     pub fn zid(&self) -> Option<_ZenohId> {
         self.0.zid.map(_ZenohId)
     }
     #[getter]
     pub fn whatami(&self) -> Option<&'static str> {
         match self.0.whatami {
-            Some(zenoh::config::whatami::WhatAmI::Client) => Some("client"),
-            Some(zenoh::config::whatami::WhatAmI::Peer) => Some("peer"),
-            Some(zenoh::config::whatami::WhatAmI::Router) => Some("router"),
-            None => None,
+            zenoh::config::whatami::WhatAmI::Client => Some("client"),
+            zenoh::config::whatami::WhatAmI::Peer => Some("peer"),
+            zenoh::config::whatami::WhatAmI::Router => Some("router"),
         }
     }
     #[getter]
     pub fn locators(&self) -> Vec<String> {
-        match &self.0.locators {
-            Some(locators) => locators.iter().map(|l| l.to_string()).collect(),
-            None => Vec::new(),
-        }
+        self.0.locators.iter().map(|l| l.to_string()).collect()
     }
     pub fn __str__(&self) -> String {
         self.0.to_string()
     }
 }
 impl From<Hello> for _Hello {
     fn from(h: Hello) -> Self {
```

### Comparing `eclipse_zenoh-0.7.0rc0/tests/examples_check.py` & `eclipse_zenoh-0.7.2rc0/tests/examples_check.py`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/__init__.py` & `eclipse_zenoh-0.7.2rc0/zenoh/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,25 +18,55 @@
 from .enums import CongestionControl, Encoding, Priority, QueryConsolidation, QueryTarget, Reliability, SampleKind
 from .value import Hello, Value, IntoValue, IValue, Sample, IntoSample, ZenohId, Timestamp, Reply
 from .closures import Closure, IClosure, IntoClosure, Handler, IHandler, IntoHandler, ListCollector, Queue
 from .queryable import Queryable, Query
 from typing import Any
 
 def open(*args, **kwargs):
+    """
+    Open a zenoh-net Session.
+
+    :param config: The configuration of the zenoh-net session
+    :type config: Config
+    :rtype: Session
+
+    :Example:
+
+    >>> import zenoh
+    >>> s = zenoh.open(zenoh.Config())
+    """
     return Session(*args, **kwargs)
 
 class Scout:
     def __init__(self, inner, receiver):
         self._inner_ = inner
         self.receiver = receiver
     
     def stop(self):
         self._inner_ = None
 
 def scout(handler: IntoHandler[Hello, Any, Any] = None, what: str = None, config: Config = None, timeout=None):
+    """
+    Scout for routers and/or peers.
+
+    This spawns a task that periodically sends scout messages for a specified duration and returns
+    a list of received :class:`Hello` messages.
+
+    :param what: The kind of zenoh process to scout for
+    :param config: The configuration to use for scouting
+    :param timeout: the duration of scout (in seconds)
+    :param handler:
+    :rtype: list of :class:`Hello`
+
+    :Example:
+
+    >>> import zenoh
+    >>> for hello in zenoh.scout(what = "peer|router", timeout=1.0).receiver():
+    ...     print(hello)
+    """
     from threading import Timer
     if handler is None:
         handler = ListCollector()
     handler = Handler(handler, lambda x: Hello._upgrade_(x))
     scout = _scout(handler.closure, config, what)
     scout = Scout(scout, handler.receiver)
     if timeout:
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/closures.py` & `eclipse_zenoh-0.7.2rc0/zenoh/closures.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 #
 import abc
 from typing import Generic, Callable, Union, Any, TypeVar, Tuple, List
 from threading import Condition, Thread
 from collections import deque
 import time
 
+from .zenoh import _Queue
+
 In = TypeVar("In")
 Out = TypeVar("Out")
 Receiver = TypeVar("Receiver")
 CallbackCall = Callable[[In], Out]
 CallbackDrop = Callable[[], None]
 
 class IClosure(Generic[In, Out]):
     """
-    A Closure is a pair of a `call` function that will be used as a callback,
-    and a `drop` function that will be called when the closure is destroyed.
+    A Closure is a pair of a ``call`` function that will be used as a callback,
+    and a ``drop`` function that will be called when the closure is destroyed.
     """
     @property
     @abc.abstractmethod
     def call(self) -> Callable[[In], Out]:
         """
         Returns the closure's call function as a lambda.
         """
@@ -67,50 +69,72 @@
     def receiver(self) -> Receiver:
         "The part of the handler that should be used as the receiver when the handler is channel-like."
         ...
 
 IntoClosure = Union[IHandler[In, Out, Any], IClosure[In, Out], Tuple[CallbackCall, CallbackDrop], CallbackCall]
 class Closure(IClosure, Generic[In, Out]):
     """
-    A Closure is a pair of a `call` function that will be used as a callback,
-    and a `drop` function that will be called when the closure is destroyed.
+    A Closure is a pair of a ``call`` function that will be used as a callback,
+    and a ``drop`` function that will be called when the closure is destroyed.
     """
-    def __init__(self, closure: IntoClosure[In, Out], type_adaptor: Callable[[Any], In] = None):
+    def __init__(self, closure: IntoClosure[In, Out], type_adaptor: Callable[[Any], In] = None, prevent_direct_calls=False):
         _call_ = None
-        self._drop_ = lambda: None
+        _drop_ = lambda: None
         if isinstance(closure, IHandler):
             closure = closure.closure
             # dev-note: do not elif here, the  next if will catch the obtained closure.
         if isinstance(closure, IClosure):
             _call_ = closure.call
-            self._drop_ = closure.drop
+            _drop_ = closure.drop
         elif isinstance(closure, tuple):
-            _call_, self._drop_ = closure
+            _call_, _drop_ = closure
         elif callable(closure):
             _call_ = closure
         else:
             raise TypeError("Unexpected type as input for zenoh.Closure")
         if type_adaptor is not None:
-            self._call_ = lambda *args: _call_(type_adaptor(*args))
+            adapted = lambda *args: _call_(type_adaptor(*args))
+        else:
+            adapted = _call_
+        if prevent_direct_calls:
+            queue = Queue(128)
+            def readqueue():
+                for x in queue:
+                    adapted(*x)
+                    x = None
+            t = Thread(target=readqueue)
+            t.start()
+            self._call_ = lambda *args: queue.put(args)
+            def drop():
+                queue.close()
+                t.join()
+                _drop_()
+            self._drop_ = drop
         else:
             self._call_ = _call_
+            self._drop_ = _drop_
+
     @property
     def call(self) -> Callable[[In], Out]:
         return self._call_
 
     @property
     def drop(self) -> Callable[[], None]:
         return self._drop_
 
 IntoHandler = Union[IHandler[In, Out, Receiver], IClosure[In, Out],  Tuple[IClosure, Receiver], Tuple[CallbackCall,CallbackDrop, Receiver], Tuple[CallbackCall,CallbackDrop], CallbackCall]
 class Handler(IHandler, Generic[In, Out, Receiver]):
     """
     A Handler is a value that may be converted into a callback closure for zenoh to use on one side, while possibly providing a receiver for the data that zenoh would provide through that callback.
+
+    Note that the values will be piped onto a ``Queue`` before being sent to your handler by another Thread unless either:
+        a) ``input`` is already an instance of ``Closure`` or ``Handler`` where ``input.closure`` is an instance of ``Closure``
+        b) ``prevent_direct_calls`` is set to ``False``
     """
-    def __init__(self, input: IntoHandler[In, Out, Receiver], type_adaptor: Callable[[Any], In] = None):
+    def __init__(self, input: IntoHandler[In, Out, Receiver], type_adaptor: Callable[[Any], In] = None, prevent_direct_calls = True):
         self._receiver_ = None
         if isinstance(input, IHandler):
             self._receiver_ = input.receiver
             self._closure_ = input.closure
         elif isinstance(input, IClosure):
             self._closure_ = input
         elif isinstance(input, tuple):
@@ -119,15 +143,15 @@
             elif len(input) == 3:
                 call, drop, self._receiver_ = input
                 self._closure_ = (call, drop)
             else:
                 self._closure_ = input
         else:
             self._closure_ = input
-        self._closure_ = Closure(self._closure_, type_adaptor)
+        self._closure_ = Closure(self._closure_, type_adaptor, prevent_direct_calls and not isinstance(self._closure_, Closure))
 
     @property
     def closure(self) -> IClosure[In, Out]:
         return self._closure_
     @property
     def receiver(self) -> Receiver:
         return self._receiver_
@@ -164,88 +188,65 @@
                 if not self._done_:
                     self._cv_.wait(timeout=self.timeout)
                 return self._vec_
         return wait
 
 class Queue(IHandler[In, None, 'Queue'], Generic[In]):
     """
-    A simple single-producer, single-consumer queue implementation.
+    A binding for a Rust multi-producer, single-consumer queue implementation.
 
     When used as a handler, it provides itself as the receiver, and will provide a
     callback that appends elements to the queue.
+
+    Can be bounded by passing a maximum size as ``bound``.
     """
-    def __init__(self, timeout=None):
-        self._vec_ = deque()
-        self._cv_ = Condition()
-        self._done_ = False
+    def __init__(self, bound: int = None):
+        self._inner_ = _Queue(bound)
     
     @property
     def closure(self) -> IClosure[In, None]:
         def call(x): self.put(x)
         def drop(): self.close()
         return Closure((call, drop))
     
     @property
     def receiver(self) -> 'Queue':
         return self
     
     def put(self, value):
         """
         Puts one element on the queue.
+
+        Raises a ``PyBrokenPipeError`` if the Queue has been closed.
         """
-        with self._cv_:
-            self._vec_.append(value)
-            self._cv_.notify()
+        return self._inner_.put(value)
 
 
-    def get(self, timeout=None):
+    def get(self, timeout: float = None):
         """
         Gets one element from the queue.
 
-        Raises a `StopIteration` exception if the queue was closed before the timeout ran out.
-        Raises a `TimeoutError` if the timeout ran out.
+        Raises a ``StopIteration`` exception if the queue was closed before the timeout ran out,
+        this allows using the Queue as an iterator in for-loops.
+        Raises a ``TimeoutError`` if the timeout ran out.
         """
-        try:
-            return self._vec_.pop()
-        except IndexError:
-            pass
-        if self._done_:
-            raise StopIteration()
-        with self._cv_:
-            self._cv_.wait(timeout=timeout)
-            try:
-                return self._vec_.pop()
-            except IndexError:
-                pass
-        if self._done_:
-            raise StopIteration()
-        else:
-            raise TimeoutError()
+        return self._inner_.get(timeout)
     
     def close(self):
-        with self._cv_:
-            self._done_ = True
-            self._cv_.notify()
+        return self._inner_.close()
     
-    def get_remaining(self, timeout=None) -> List[In]:
+    def get_remaining(self, timeout: float = None) -> List[In]:
         """
         Awaits the closing of the queue, returning the remaining queued values in a list.
-        The values inserted into the queue up until this happens will be available through `get`.
+        The values inserted into the queue up until this happens will be available through ``get``.
 
-        Raises a `TimeoutError` if the timeout in seconds provided was exceeded before closing.
+        Raises a ``TimeoutError`` if the timeout in seconds provided was exceeded before closing,
+        whose ``args[0]`` will contain the elements that were collected before timing out.
         """
-        end = (time.time() + timeout) if timeout is not None else None
-        while not self._done_:
-            with self._cv_:
-                self._cv_.wait(timeout=(timeout - time.time()) if timeout else None)
-                if self._done_:
-                    return
-                elif time.time() >= end:
-                    raise TimeoutError()
-        return list(self._vec_)
+        return self._inner_.get_remaining()
 
     def __iter__(self):
         return self
     def __next__(self):
         return self.get()
 
 if __name__ == "__main__":
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/config.py` & `eclipse_zenoh-0.7.2rc0/zenoh/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         The file's extension must be json, json5 or yaml.
         """
         c = super(Config, Config).from_file(filename)
         return c
     @staticmethod
     def from_obj(obj):
         """
-        Reads the configuration from `obj` as if it was a JSON file.
+        Reads the configuration from ``obj`` as if it was a JSON file.
         """
         c = Config.from_json5(json.dumps(obj))
         return c
     @staticmethod
     def from_json5(json: str):
         """
         Reads the configuration from a JSON5 string.
@@ -41,15 +41,15 @@
         JSON5 is a superset of JSON, so any JSON string is a valid input for this function.
         """
         c =  super(Config, Config).from_json5(json)
         return c
     
     def get_json(self, path: str) -> str:
         """
-        Returns the part of the configuration at `path`,
+        Returns the part of the configuration at ``path``,
         in a JSON-serialized form.
         """
         return super().get_json(path)
     
     def insert_json5(self, path: str, value: str) -> str:
         """
         Inserts the provided value (read from JSON) at the given path in the configuration.
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/enums.py` & `eclipse_zenoh-0.7.2rc0/zenoh/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .zenoh import _Encoding, _SampleKind, _CongestionControl, _Priority, _Reliability, _QueryTarget, _QueryConsolidation
 
 class Priority(_Priority):
     """
     The priority of a sending operation.
 
     They are ordered à la Linux priority:
-    `Priority.REAL_TIME() < Priority.INTERACTIVE_HIGH() < Priority.INTERACTIVE_LOW() < Priority.DATA() < Priority.BACKGROUND()`
+    ``Priority.REAL_TIME() < Priority.INTERACTIVE_HIGH() < Priority.INTERACTIVE_LOW() < Priority.DATA() < Priority.BACKGROUND()``
     """
     def __new__(cls, inner: _SampleKind):
         return super().__new__(cls, inner)
     @staticmethod
     def REAL_TIME() -> 'Priority':
         return Priority(_Priority.REAL_TIME)
     @staticmethod
@@ -180,15 +180,15 @@
         "Informs the network that dropping some messages is acceptable"
         return Reliability(_Reliability.BEST_EFFORT)
     @staticmethod
     def RELIABLE() -> 'CongestionControl':
         """
         Informs the network that this subscriber wishes for all publications to reliably reach it.
 
-        Note that if a publisher puts a sample with the `CongestionControl.DROP()` option, this reliability
+        Note that if a publisher puts a sample with the ``CongestionControl.DROP()`` option, this reliability
         requirement may be infringed to prevent slow readers from blocking the network.
         """
         return Reliability(_Reliability.RELIABLE)
     def __eq__(self, other) -> bool:
         return super().__eq__(other)
     def __ne__(self, other) -> bool:
         return not self.__eq__(other)
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/keyexpr.py` & `eclipse_zenoh-0.7.2rc0/zenoh/keyexpr.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,42 +16,44 @@
 
 IntoKeyExpr = Union['KeyExpr', _KeyExpr, str]
 
 class KeyExpr(_KeyExpr):
     """
     Zenoh's address space is designed around keys which serve as the names of ressources.
 
-    Keys are slash-separated lists of non-empty UTF8 strings. They may not contain the following characters: `$*#?`.
+    Keys are slash-separated lists of non-empty UTF8 strings. They may not contain the following characters: ``$*#?``.
     
     Zenoh's operations are executed on key expressions, a small language that allows the definition
     of sets of keys via the use of wildcards:
-    - `*` is the single-chunk wildcard, and will match any chunk: "a/*/c" will match "a/b/c", "a/hello/c", etc...
-    - `**` is the 0 or more chunks wildcard: "a/**/c" matches "a/c", "a/b/c", "a/b/hello/c"...
-    - `$*` is the subchunk wildcard, it will match any amount of non-/ characters: "a/b$*" matches "a/b", "a/because", "a/blue"... but not "a/c" nor "a/blue/c"
+
+     - ``*`` is the single-chunk wildcard, and will match any chunk: ``a/*/c`` will match ``a/b/c``, ``a/hello/c``, etc...
+     - ``**`` is the 0 or more chunks wildcard: ``a/**/c`` matches ``a/c``, ``a/b/c``, ``a/b/hello/c``, etc...
+     - ``$*`` is the subchunk wildcard, it will match any amount of non-/ characters: ``a/b$*`` matches ``a/b``, ``a/because``, ``a/blue``... but not ``a/c`` nor ``a/blue/c``
     
     To allow for better performance and gain the property that two key expressions define the same
     set if and only if they are the same string, the rules of canon form are mandatory for a key
     expression to be propagated by a Zenoh network:
-    - `**/**` may not exist, as it could always be replaced by the shorter `**`,
-    - `**/*` may not exist, and must be written as its equivalent `*/**` instead,
-    - `$*` may not exist alone in a chunk, as it must be written `*` instead.
 
-    The `KeyExpr.autocanonize` constructor exists to correct eventual infrigements of the canonization rules.
+     - ``**/**`` may not exist, as it could always be replaced by the shorter ``**``,
+     - ``**/*`` may not exist, and must be written as its equivalent ``*/**`` instead,
+     - ``$*`` may not exist alone in a chunk, as it must be written ``*`` instead.
+
+    The ``KeyExpr.autocanonize`` constructor exists to correct eventual infrigements of the canonization rules.
 
     A KeyExpr is a string that has been validated to be a valid Key Expression.
     """
     def __new__(cls, expr: IntoKeyExpr):
         """
         The default constructor for KeyExpr will ensure that the passed expression is valid.
         It won't however try to correct expressions that aren't canon.
 
-        You may use `KeyExpr.autocanonize(expr)` instead if you are unsure if the expression
+        You may use ``KeyExpr.autocanonize(expr)`` instead if you are unsure if the expression
         you will use for construction will be canon.
 
-        Raises a zenoh.ZError exception if `expr` is not a valid key expression.
+        Raises a zenoh.ZError exception if ``expr`` is not a valid key expression.
         """
         if isinstance(expr, KeyExpr):
             return expr
         elif isinstance(expr, _KeyExpr):
             return _KeyExpr.__new__(cls, expr)
         else:
             return _KeyExpr.__new__(cls, _KeyExpr.new(expr))
@@ -61,97 +63,101 @@
 
     @staticmethod
     def autocanonize(expr: str) -> 'KeyExpr':
         """
         This alternative constructor for key expressions will attempt to canonize the passed
         expression before checking if it is valid.
 
-        Raises a zenoh.ZError exception if `expr` is not a valid key expression.
+        Raises a zenoh.ZError exception if ``expr`` is not a valid key expression.
         """
         if isinstance(expr, KeyExpr):
             return expr
         else:
             e = _KeyExpr.autocanonize(expr)
             return KeyExpr(e.as_str())
     
-    def intersects(self, other: 'KeyExpr') -> bool:
+    def intersects(self, other: IntoKeyExpr) -> bool:
         """
-        This method returns `True` if there exists at least one key that belongs to both sets
-        defined by `self` and `other`. 
+        This method returns ``True`` if there exists at least one key that belongs to both sets
+        defined by ``self`` and ``other``. 
         """
-        return super().intersects(other)
+        return super().intersects(KeyExpr(other))
     
-    def includes(self, other: 'KeyExpr') -> bool:
+    def includes(self, other: IntoKeyExpr) -> bool:
         """
-        This method returns `True` if all of the keys defined by `other` also belong to the set
-        defined by `self`.
+        This method returns ``True`` if all of the keys defined by ``other`` also belong to the set
+        defined by ``self``.
         """
-        return super().includes(other)
+        return super().includes(KeyExpr(other))
     
     def undeclare(self, session: 'Session'):
         """
         Undeclares a key expression previously declared on the session.
         """
         super().undeclare(session)
     
-    def __eq__(self, other: 'KeyExpr') -> bool:
+    def __eq__(self, other: IntoKeyExpr) -> bool:
         """
         Corresponds to set equality.
         """
-        return super().__eq__(other)
+        return super().__eq__(KeyExpr(other))
     
     def __truediv__(self, other: IntoKeyExpr) -> 'KeyExpr':
         """
-        Joins two key expressions with a `/`.
+        Joins two key expressions with a ``/``.
 
-        Raises a zenoh.ZError exception if `other` is not a valid key expression.
+        Raises a zenoh.ZError exception if ``other`` is not a valid key expression.
         """
         return KeyExpr.autocanonize(f"{self}/{other}")
     
     def __str__(self):
         return super().__str__()
     
     def __hash__(self):
         return super().__hash__()
 
 IntoSelector = Union['Selector', _Selector, IntoKeyExpr]
 class Selector(_Selector):
     """
     A selector is the combination of a [Key Expression](crate::prelude::KeyExpr), which defines the
-    set of keys that are relevant to an operation, and a `parameters`, a set of key-value pairs
+    set of keys that are relevant to an operation, and a ``parameters``, a set of key-value pairs
     with a few uses:
-    * specifying arguments to a queryable, allowing the passing of Remote Procedure Call parameters
-    * filtering by value,
-    * filtering by metadata, such as the timestamp of a value,
+
+     * specifying arguments to a queryable, allowing the passing of Remote Procedure Call parameters
+     * filtering by value,
+     * filtering by metadata, such as the timestamp of a value,
 
     When in string form, selectors look a lot like a URI, with similar semantics:
-    * the `key_expr` before the first `?` must be a valid key expression.
-    * the `parameters` after the first `?` should be encoded like the query section of a URL:
-      * key-value pairs are separated by `&`,
-      * the key and value are separated by the first `=`,
-      * in the absence of `=`, the value is considered to be the empty string,
-      * both key and value should use percent-encoding to escape characters,
-      * defining a value for the same key twice is considered undefined behavior.
+
+     * the ``key_expr`` before the first ``?`` must be a valid key expression.
+     * the ``parameters`` after the first ``?`` should be encoded like the query section of a URL:
+
+        * key-value pairs are separated by ``&``,
+        * the key and value are separated by the first ``=``,
+        * in the absence of ``=``, the value is considered to be the empty string,
+        * both key and value should use percent-encoding to escape characters,
+        * defining a value for the same key twice is considered undefined behavior.
 
     Zenoh intends to standardize the usage of a set of keys. To avoid conflicting with RPC parameters,
     the Zenoh team has settled on reserving the set of keys that start with non-alphanumeric characters.
 
     This document will summarize the standardized keys for which Zenoh provides helpers to facilitate
     coherent behavior for some operations.
 
     Queryable implementers are encouraged to prefer these standardized keys when implementing their
     associated features, and to prefix their own keys to avoid having conflicting keys with other
     queryables.
 
     Here are the currently standardized keys for Zenoh:
-    * `_time`: used to express interest in only values dated within a certain time range, values for
-      this key must be readable by the [Zenoh Time DSL](zenoh_util::time_range::TimeRange) for the value to be considered valid.
-    * `_filter`: *TBD* Zenoh intends to provide helper tools to allow the value associated with
-      this key to be treated as a predicate that the value should fulfill before being returned.
-      A DSL will be designed by the Zenoh team to express these predicates.
+
+     * ``_time``: used to express interest in only values dated within a certain time range, values for
+       this key must be readable by the [Zenoh Time DSL](zenoh_util::time_range::TimeRange) for the value to be considered valid.
+     * ``_filter``: *TBD* Zenoh intends to provide helper tools to allow the value associated with
+       this key to be treated as a predicate that the value should fulfill before being returned.
+       A DSL will be designed by the Zenoh team to express these predicates.
     """
     def __new__(cls, selector: IntoSelector):
         if isinstance(selector, Selector):
             return selector
         if isinstance(selector, _Selector):
             return Selector._upgrade_(selector)
         return Selector._upgrade_(super().new(str(selector)))
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/queryable.py` & `eclipse_zenoh-0.7.2rc0/zenoh/queryable.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 class Queryable:
     """
     A handle to a queryable.
     
     Its main purpose is to keep the queryable active as long as it exists.
 
-    When constructed through `Session.declare_queryable(session, keyexpr, handler)`, it exposes `handler`'s receiver
-    through `self.receiver`.
+    When constructed through ``Session.declare_queryable(session, keyexpr, handler)``, it exposes ``handler``'s receiver
+    through ``self.receiver``.
     """
     def __init__(self, inner: _Queryable, receiver):
         self._inner_ = inner
         self.receiver = receiver
     
     def undeclare(self):
         "Stops the queryable."
@@ -41,15 +41,15 @@
     def key_expr(self) -> KeyExpr:
         "The query's targeted key expression"
         return KeyExpr(super().key_expr)
     @property
     def parameters(self) -> str:
         """
         The query's value selector.
-        If you'd rather not bother with parsing it yourself, use `self.decode_parameters()` instead.
+        If you'd rather not bother with parsing it yourself, use ``self.decode_parameters()`` instead.
         """
         return super().parameters
         
     def decode_parameters(self) -> Dict[str, str]:
         """
         Decodes the value selector into a dictionary.
 
@@ -62,16 +62,14 @@
         The query's selector as a whole.
         """
         return Selector._upgrade_(super().selector)
     @property
     def value(self) -> Optional[Value]:
         """
         The query's value.
-
-        This API is currently marked as `unstable`: the Zenoh team may change it in future releases.
         """
         return Value._upgrade_(super().value)
     def reply(self, sample: Sample):
         """
         Allows you to reply to a query.
         You may send any amount of replies to a single query, including 0.
         """
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/session.py` & `eclipse_zenoh-0.7.2rc0/zenoh/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,45 +20,45 @@
 from .closures import IntoHandler, Handler, Receiver
 from .enums import *
 from .value import IntoValue, Value, Sample, Reply, ZenohId
 from .queryable import Queryable, Query
 
 
 class Publisher:
-    "Use `Publisher`s (constructed with `Session.declare_publisher`) when you want to send values often for the same key expression, as declaring them informs Zenoh that this is you intent, and optimizations will be set up to do so."
+    "Use ``Publisher`` (constructed with ``Session.declare_publisher``) when you want to send values often for the same key expression, as declaring them informs Zenoh that this is you intent, and optimizations will be set up to do so."
 
     def __init__(self, p: _Publisher):
         self._inner_ = p
 
     def put(self, value: IntoValue, encoding: Encoding = None):
-        "An optimised version of `session.put(self.key_expr, value, encoding=encoding)"
+        "An optimised version of ``session.put(self.key_expr, value, encoding=encoding)``"
         self._inner_.put(Value(value, encoding))
 
     def delete(self):
-        "An optimised version of `session.delete(self.key_expr)"
+        "An optimised version of ``session.delete(self.key_expr)``"
         self._inner_.delete()
 
     @property
     def key_expr(self) -> KeyExpr:
-        "This `Publisher`'s key expression"
+        "This ``Publisher``'s key expression"
         return KeyExpr(self._inner_.key_expr)
 
     def undeclare(self):
         "Stops the publisher."
         self._inner_ = None
 
 
 class Subscriber:
     """
     A handle to a subscription.
 
     Its main purpose is to keep the subscription active as long as it exists.
 
-    When constructed through `Session.declare_subscriber(session, keyexpr, handler)`, it exposes `handler`'s receiver
-    through `self.receiver`.
+    When constructed through ``Session.declare_subscriber(session, keyexpr, handler)``, it exposes ``handler``'s receiver
+    through ``self.receiver``.
     """
 
     def __init__(self, s: _Subscriber, receiver=None):
         self._subscriber_ = s
         self.receiver = receiver
 
     def undeclare(self):
@@ -68,18 +68,18 @@
 
 class PullSubscriber:
     """
     A handle to a pull subscription.
 
     Its main purpose is to keep the subscription active as long as it exists.
 
-    When constructed through `Session.declare_pull_subscriber(session, keyexpr, handler)`, it exposes `handler`'s receiver
-    through `self.receiver`.
+    When constructed through ``Session.declare_pull_subscriber(session, keyexpr, handler)``, it exposes ``handler``'s receiver
+    through ``self.receiver``.
 
-    Calling `self.pull()` will prompt the Zenoh network to send a new sample when available.
+    Calling ``self.pull()`` will prompt the Zenoh network to send a new sample when available.
     """
 
     def __init__(self, s: _PullSubscriber, receiver=None):
         self._subscriber_ = s
         self.receiver = receiver
 
     def pull(self):
@@ -93,149 +93,293 @@
         "Undeclares the subscription"
         self._subscriber_ = None
 
 
 class Session(_Session):
     """
     A Zenoh Session, the core interraction point with a Zenoh network.
+
+    Note that most applications will only need a single instance of ``Session``. You should _never_ construct one session per publisher/subscriber, as this will significantly increase the size of your Zenoh network, while preventing potential locality-based optimizations.
     """
     def __new__(cls, config: Union[Config, Any] = None):
         if config is None:
             return super().__new__(cls)
         elif isinstance(config, _Config):
             return super().__new__(cls, config)
         else:
             return super().__new__(cls, Config.from_obj(config))
 
     def put(self, keyexpr: IntoKeyExpr, value: IntoValue, encoding=None,
             priority: Priority = None, congestion_control: CongestionControl = None,
             sample_kind: SampleKind = None):
         """
         Sends a value over Zenoh.
+
+        Subscribers on an expression that intersect with ``keyexpr`` will receive the sample.
+        Storages will store the value if ``keyexpr`` is non-wild, or update the values for all known keys that are included in ``keyexpr`` if it is wild.
+
+        :param keyexpr: The key expression to publish
+        :param value: The value to send
+        :param priority: The priority to use when routing the published data
+        :param congestion_control: The congestion control to use when routing the published data
+        :param sample_kind: The kind of sample to send
+
+        :Examples:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> s.put('key/expression', 'value')
         """
         value = Value(value, encoding)
         keyexpr = KeyExpr(keyexpr)
         kwargs = dict()
         if priority is not None:
             kwargs['priority'] = priority
         if congestion_control is not None:
             kwargs['congestion_control'] = congestion_control
         if sample_kind is not None:
             kwargs['sample_kind'] = sample_kind
         return super().put(keyexpr, value, **kwargs)
 
     def config(self) -> Config:
-        """
-        Returns a configuration object that can be used to alter the session's configuration at runtime.
+        """Returns a configuration object that can be used to alter the session's configuration at runtime.
 
         Note that in Python specifically, the config you passed to the session becomes the result of this
         function if you passed one, letting you keep using it.
         """
         return super().config()
 
     def delete(self, keyexpr: IntoKeyExpr,
                priority: Priority = None, congestion_control: CongestionControl = None):
         """
-        Deletes a value.
+        Deletes the values associated with the keys included in ``keyexpr``.
+        
+        This uses the same mechanisms as ``session.put``, and will be received by subscribers.
+        This operation is especially useful with storages.
+
+        :param keyexpr: The key expression to publish
+        :param priority: The priority to use when routing the delete
+        :param congestion_control: The congestion control to use when routing the delete
+
+        :Examples:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> s.delete('key/expression')
         """
         keyexpr = KeyExpr(keyexpr)
         kwargs = dict()
         if priority is not None:
             kwargs['priority'] = priority
         if congestion_control is not None:
             kwargs['congestion_control'] = congestion_control
         return super().delete(keyexpr, **kwargs)
 
     def get(self, selector: IntoSelector, handler: IntoHandler[Reply, Any, Receiver], consolidation: QueryConsolidation = None, target: QueryTarget = None, value: IntoValue = None) -> Receiver:
         """
-        Emits a query.
+        Emits a query, which queryables with intersecting selectors will be able to reply to.
+
+        The replies are provided to the given `handler` as instances of the `Reply` class.
+        The `handler` can typically be a queue, a single callback or a pair of callbacks.
+        The `handler`'s receiver is returned by the `get` function.
+
+        :param selector: The selection of keys to query
+        :param handler:
+        :param consolidation: The consolidation to apply to replies
+        :param target: The queryables that should be target to this query
+        :param value: An optional value to attach to this query
+        :return: The receiver of the handler
+        :rtype: Receiver
+
+        :Examples:
+
+        Using a queue:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> for reply in s.get('key/expression', zenoh.Queue()):
+        ...     try:
+        ...         print(f"Received '{reply.ok.key_expr}': '{reply.ok.payload.decode('utf-8')}'")
+        ...     except:
+        ...         print(f"Received ERROR: '{reply.err.payload.decode('utf-8')}'")
+
+        Using a single callback:
+
+        >>> s.get('key/expression', lambda reply:
+        ...     print(f"Received '{reply.ok.key_expr}': '{reply.ok.payload.decode('utf-8')}'")
+        ...     if reply.ok is not None else print(f"Received ERROR: '{reply.err.payload.decode('utf-8')}'"))
+
+        Using a reply callback and a termination callback:
+
+        >>> s.get('key/expression', (
+        ...     lambda reply:
+        ...         print(f"Received '{reply.ok.key_expr}': '{reply.ok.payload.decode('utf-8')}'")
+        ...         if reply.ok is not None else print(f"Received ERROR: '{reply.err.payload.decode('utf-8')}'"),
+        ...     lambda:
+        ...         print("No more replies")))
         """
         handler = Handler(handler, lambda x: Reply(x))
         kwargs = dict()
         if consolidation is not None:
-            kwargs["conconsolidation"] = consolidation
+            kwargs["consolidation"] = consolidation
         if target is not None:
             kwargs["target"] = target
         if value is not None:
             kwargs["value"] = Value(value)
         super().get(Selector(selector), handler.closure, **kwargs)
         return handler.receiver
 
     def declare_keyexpr(self, keyexpr: IntoKeyExpr) -> KeyExpr:
-        """
-        Informs Zenoh that you intend to use the provided Key Expression repeatedly.
+        """Informs Zenoh that you intend to use the provided Key Expression repeatedly.
+
+        This function returns an optimized representation of the passed ``keyexpr``.
 
-        This function returns an optimized representation of the passed `keyexpr`.
+        It is generally not needed to declare key expressions, as declaring a subscriber, 
+        a queryable, or a publisher will also inform Zenoh of your intent to use their
+        key expressions repeatedly.
         """
         return KeyExpr(super().declare_keyexpr(KeyExpr(keyexpr)))
 
     def declare_queryable(self, keyexpr: IntoKeyExpr, handler: IntoHandler[Query, Any, Any], complete: bool = None):
-        """
-        Declares a queryable, which will receive queries intersecting with `keyexpr`.
-
-        These queries are passed to the `handler` as instances of the `Query`class, which lets you respond when applicatble.
+        """Declares a queryable, which will receive queries intersecting with ``keyexpr``.
 
-        The `handler`'s receiver is returned as the `receiver` field of the return value.
+        These queries are passed to the `handler` as instances of the `Query` class.
+        The `handler` can typically be a queue or a callback.
+        The `handler`'s receiver is returned as the `receiver` field of the returned `Queryable`.
+        The replies can be sent back by calling the `reply`function of the `Query`.
+
+        :Examples:
+
+        Using a callback:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> qabl = s.declare_queryable('key/expression', lambda query:
+        ...     query.reply(zenoh.Sample('key/expression', 'value')))
+
+        Using a queue:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> qabl = s.declare_queryable('key/expression', zenoh.Queue())
+        >>> while True:
+        ...     query = qabl.receiver.get()
+        ...     query.reply(zenoh.Sample('key/expression', 'value'))
+        ...     del query
 
         IMPORTANT: due to how RAII and Python work, you MUST bind this function's return value to a variable in order for it to function as expected.
         This is because as soon as a value is no longer referenced in Python, that value's destructor will run, which will undeclare your queryable, stopping it immediately.
         """
         handler = Handler(handler, lambda x: Query(x))
         kwargs = dict()
         if complete is not None:
             kwargs['complete'] = complete
         inner = super().declare_queryable(KeyExpr(keyexpr), handler.closure, **kwargs)
         return Queryable(inner, handler.receiver)
 
     def declare_publisher(self, keyexpr: IntoKeyExpr, priority: Priority = None, congestion_control: CongestionControl = None):
         """
-        Declares a publisher, which you may use to send values repeatedly onto a same key expression.
+        Declares a publisher, which may be used to send values repeatedly onto a same key expression.
+
+        Written resources that match the given key will only be sent on the network
+        if matching subscribers exist in the system.
+
+        :param keyexpr: The key expression to publish to
+        :param priority: The priority to use when routing the published data
+        :param congestion_control: The congestion control to use when routing the published data
+        :rtype: Publisher
+
+        :Examples:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> pub = s.declare_publisher('key/expression')
+        >>> pub.put('value')
         """
         kwargs = dict()
         if priority is not None:
             kwargs['priority'] = priority
         if congestion_control is not None:
             kwargs['congestion_control'] = congestion_control
         return Publisher(super().declare_publisher(KeyExpr(keyexpr), **kwargs))
 
     def declare_subscriber(self, keyexpr: IntoKeyExpr, handler: IntoHandler[Sample, Any, Any], reliability: Reliability = None) -> Subscriber:
         """
-        Declares a subscriber, which will receive any published sample with a key expression intersecting `keyexpr`.
+        Declares a subscriber, which will receive any published sample with a key expression intersecting ``keyexpr``.
 
-        These samples are passed to the `handler`'s closure as instances of the `Sample` class.
+        These samples are provided to the `handler` as instances of the `Sample` class.
+        The `handler` can typically be a queue or a callback.
+        The `handler`'s receiver is returned as the `receiver` field of the returned `Subscriber`.
+
+        :param keyexpr: The key expression to subscribe to
+        :param handler:
+        :param reliability: the reliability to use when routing the subscribed samples
+        :rtype: Subscriber
+
+        :Examples:
 
-        The `handler`'s receiver is returned as the `receiver` field of the return value.
+        Using a callback:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> sub = s.declare_subscriber('key/expression', lambda sample:
+        ...     print(f"Received '{sample.key_expr}': '{sample.payload.decode('utf-8')}'")
+
+        Using a queue:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> sub = s.declare_subscriber('key/expression', zenoh.Queue())
+        >>> for sample in sub.receiver:
+        >>>     print(f"{sample.key_expr}: {sample.payload.decode('utf-8')}")
 
         IMPORTANT: due to how RAII and Python work, you MUST bind this function's return value to a variable in order for it to function as expected.
         This is because as soon as a value is no longer referenced in Python, that value's destructor will run, which will undeclare your subscriber, deactivating the subscription immediately.
         """
         handler = Handler(handler, lambda x: Sample._upgrade_(x))
         kwargs = dict()
         if reliability is not None:
             kwargs['reliability'] = reliability
         s = super().declare_subscriber(KeyExpr(keyexpr), handler.closure, **kwargs)
         return Subscriber(s, handler.receiver)
 
     def declare_pull_subscriber(self, keyexpr: IntoKeyExpr, handler: IntoHandler[Sample, Any, Any], reliability: Reliability = None) -> PullSubscriber:
         """
-        Declares a pull-mode subscriber, which will receive a single published sample with a key expression intersecting `keyexpr` any time its `pull` method is called.
+        Declares a pull-mode subscriber, which will receive a single published sample with a key expression intersecting ``keyexpr`` any time its ``pull`` method is called.
 
         These samples are passed to the `handler`'s closure as instances of the `Sample` class.
+        The `handler` can typically be a queue or a callback.
+        The `handler`'s receiver is returned as the `receiver` field of the returned `PullSubscriber`.
 
-        The `handler`'s receiver is returned as the `receiver` field of the return value.
+        :param keyexpr: The key expression to subscribe to
+        :param handler:
+        :param reliability: the reliability to use when routing the subscribed samples
+        :rtype: PullSubscriber
+
+        :Examples:
+
+        >>> import zenoh
+        >>> s = zenoh.open({})
+        >>> sub = s.declare_pull_subscriber('key/expression', lambda sample:
+        ...     print(f"Received '{sample.key_expr}': '{sample.payload.decode('utf-8')}'"))
+        ...
+        >>> sub.pull()
         """
         handler = Handler(handler, lambda x: Sample._upgrade_(x))
         kwargs = dict()
         if reliability is not None:
             kwargs['reliability'] = reliability
         s = super().declare_pull_subscriber(KeyExpr(keyexpr), handler.closure, **kwargs)
         return PullSubscriber(s, handler.receiver)
 
     def close(self):
-        "Closes the Session"
+        """Attempts to close the Session.
+        
+        The session will only be closed if all publishers, subscribers and queryables based on it have been undeclared, and there are no more python references to it.
+        """
         pass
 
     def info(self):
         "Returns an accessor for informations about this Session"
         return Info(self)
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh/value.py` & `eclipse_zenoh-0.7.2rc0/zenoh/value.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,41 +20,44 @@
 from .keyexpr import KeyExpr, IntoKeyExpr
 
 class IValue:
     "The IValue interface exposes how to recover a value's payload in a binary-serialized format, as well as that format's encoding."
     @property
     @abc.abstractmethod
     def payload(self) -> bytes:
+        "The value itself, as an array of bytes"
         ...
     
     @property
     @abc.abstractmethod
     def encoding(self) -> Encoding:
+        "The value's encoding"
         ...
 
 IntoValue = Union[IValue, bytes, str, int, float, object]
 
 class Value(_Value, IValue):
     """
     A Value is a pair of a binary payload, and a mime-type-like encoding string.
     
-    When constructed with `encoding==None`, the encoding will be selected depending on the payload's type.
+    When constructed with ``encoding==None``, the encoding will be selected depending on the payload's type.
     """
     def __new__(cls, payload: IntoValue, encoding: Encoding=None):
         if encoding is None:
             if isinstance(payload, Value):
                 return payload
             return Value.autoencode(payload)
         else:
             if not isinstance(payload, bytes):
                 raise TypeError("`encoding` was passed, but `payload` is not of type `bytes`")
             return Value.new(payload, encoding)
     
     @staticmethod
     def autoencode(value: IntoValue) -> 'Value':
+        "Automatically encodes the value based on its type"
         if isinstance(value, IValue):
             return Value.new(value.payload, value.encoding)
         if isinstance(value, bytes):
             return Value.new(value, Encoding.APP_OCTET_STREAM())
         if isinstance(value, str):
             return Value.new(value.encode(), Encoding.TEXT_PLAIN())
         if isinstance(value, int):
@@ -134,19 +137,19 @@
         return KeyExpr(super().key_expr)
     @property
     def value(self) -> Value:
         "The sample's value"
         return Value._upgrade_(super().value)
     @property
     def payload(self) -> bytes:
-        "A shortcut to `self.value.payload`"
+        "A shortcut to ``self.value.payload``"
         return super().payload
     @property
     def encoding(self) -> Encoding:
-        "A shortcut to `self.value.encoding`"
+        "A shortcut to ``self.value.encoding``"
         return Encoding(super().encoding)
     @property
     def kind(self) -> SampleKind:
         "The sample's kind"
         return SampleKind(super().kind)
     @property
     def timestamp(self) -> Optional[Timestamp]:
@@ -156,34 +159,39 @@
     @staticmethod
     def _upgrade_(inner: _Sample) -> 'Sample':
         if isinstance(inner, Sample):
             return inner
         return _Sample.__new__(Sample, inner)
 
 class Reply(_Reply):
+    """
+    A reply to a query (``Session.get``).
+    
+    A single query can result in multiple replies from multiple queryables.
+    """
     def __new__(cls, inner: _Reply):
         return super().__new__(cls, inner)
     @property
     def replier_id(self) -> ZenohId:
         "The reply's sender's id."
         return ZenohId._upgrade_(super().replier_id)
     @property
     def ok(self) -> Sample:
         """
         The reply's inner data sample.
 
-        Raises a ZError if the `self` is actually an `err` reply.
+        Raises a ``ZError`` if the ``self`` is actually an ``err`` reply.
         """
         return Sample._upgrade_(super().ok)
     @property
     def err(self) -> Value:
         """
         The reply's error value.
 
-        Raises a ZError if the `self` is actually an `ok` reply.
+        Raises a ``ZError`` if the ``self`` is actually an ``ok`` reply.
         """
         return Value._upgrade_(super().err)
 
 class Hello(_Hello):
     "Represents a single Zenoh node discovered through scouting."
     @property
     def zid(self) -> ZenohId:
```

### Comparing `eclipse_zenoh-0.7.0rc0/zenoh-dragon.png` & `eclipse_zenoh-0.7.2rc0/zenoh-dragon.png`

 * *Files identical despite different names*

### Comparing `eclipse_zenoh-0.7.0rc0/Cargo.lock` & `eclipse_zenoh-0.7.2rc0/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -10,42 +10,53 @@
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
+name = "ahash"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.66"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "216261ddc8289130e551ddcd5ce8a064710c0d064a4d2895c67151c92b5443f6"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "array-init"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
 
 [[package]]
 name = "async-attributes"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3203e79f4dd9bdda415ed03cf14dae5a2bf775c683a00f94e9cd1faf0f596e5"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "async-channel"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf46fee83e5ccffc220104713af3292ff9bc7c64c7de289f66dae8e38d826833"
@@ -53,17 +64,17 @@
  "concurrent-queue",
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.5.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17adb73da160dfb475c183343c8cccd80721ea5a605d3eb57125f0a7b7a92d0b"
+checksum = "6fa3dc5f2a8564f07759c008b9109dc0d39de92a88d5588b8a5036d286383afb"
 dependencies = [
  "async-lock",
  "async-task",
  "concurrent-queue",
  "fastrand",
  "futures-lite",
  "slab",
@@ -83,69 +94,67 @@
  "futures-lite",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "async-io"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c374dda1ed3e7d8f0d9ba58715f924862c63eae6849c92d3a18e7fbde9e2794"
+checksum = "0fc5b45d93ef0529756f812ca52e44c221b35341892d3dcc34132ac02f3dd2af"
 dependencies = [
  "async-lock",
  "autocfg",
+ "cfg-if",
  "concurrent-queue",
  "futures-lite",
- "libc",
  "log",
  "parking",
  "polling",
+ "rustix",
  "slab",
- "socket2",
+ "socket2 0.4.9",
  "waker-fn",
- "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "async-lock"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8101efe8695a6c17e02911402145357e718ac92d3ff88ae8419e84b1707b685"
+checksum = "fa24f727524730b077666307f2734b4a1a1c57acb79193127dcc8914d5242dd7"
 dependencies = [
  "event-listener",
- "futures-lite",
 ]
 
 [[package]]
 name = "async-process"
-version = "1.6.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6381ead98388605d0d9ff86371043b5aa922a3905824244de40dc263a14fcba4"
+checksum = "7a9d28b1d97e08915212e2e45310d47854eafa69600756fc735fb788f75199c9"
 dependencies = [
  "async-io",
  "async-lock",
  "autocfg",
  "blocking",
  "cfg-if",
  "event-listener",
  "futures-lite",
- "libc",
+ "rustix",
  "signal-hook",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-rustls"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93b21a03b7c21702a0110f9f8d228763a533570deb376119042dabf33c37a01a"
+checksum = "29479d362e242e320fa8f5c831940a5b83c1679af014068196cd20d4bf497b6b"
 dependencies = [
  "futures-io",
  "rustls",
- "webpki",
 ]
 
 [[package]]
 name = "async-std"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62565bb4402e926b29953c785397c6dc0391b7b446e45008b0049eb43cec6f5d"
@@ -170,34 +179,34 @@
  "pin-utils",
  "slab",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.3.0"
+version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a40729d2133846d9ed0ea60a8b9541bccddab49cd30f0715a1da672fe9a2524"
+checksum = "ecc7ab41815b3c653ccd2978ec3255c81349336702dfdf62ee6f7069b12a3aae"
 
 [[package]]
 name = "async-trait"
-version = "0.1.59"
+version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31e6e93155431f3931513b243d371981bb2770112b370c82745a1d19d2f99364"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "atomic-waker"
-version = "1.0.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065374052e7df7ee4047b1160cca5e1467a12351a40b3da123c870ba0b8eda2a"
+checksum = "1181e1e0d1fce796a03db1ae795d67167da795f9cf4a39c37589e85ef57f26d3"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
@@ -215,99 +224,106 @@
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "base64ct"
-version = "1.5.3"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b645a089122eccb6111b4f81cbc1a49f5900ac4666bb93ac027feaecf15607bf"
+checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c67b173a56acffd6d2326fb7ab938ba0b00a71480e14902b2591c87bc5741e8"
+checksum = "77231a1c8f801696fc0123ec6150ce92cffb8e164a02afb9c8ddee0e9b65ad65"
 dependencies = [
  "async-channel",
  "async-lock",
  "async-task",
  "atomic-waker",
  "fastrand",
  "futures-lite",
+ "log",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfb24e866b15a1af2a1b663f10c6b6b8f397a84aadb828f12e5b289ec23a3a3c"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cache-padded"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1db59621ec70f09c5e9b597b220c7a2b43611f4710dc03ceb8748637775692c"
+checksum = "981520c98f422fcc584dc1a95c334e6953900b9106bc47a9839b81790009eb21"
 
 [[package]]
 name = "cc"
-version = "1.0.77"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9f73505338f7d905b19d18738976aae232eb46b8efc15554ffc56deb5d9ebe4"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cipher"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1873270f8f7942c191139cb8a40fd228da6c3fd2fc376d7e92d47aa14aeb59e"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
  "bitflags",
  "clap_lex",
  "indexmap",
  "strsim",
  "termcolor",
@@ -321,57 +337,57 @@
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.0.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd7bef69dc86e3c610e4e7aed41035e2a7ed12e72dd7530f61327a6579a4390b"
+checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "const-oid"
-version = "0.9.1"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cec318a675afcb6a1ea1d4340e2d377e56e47c266f28043ceccbf4412ddfdd3b"
+checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -379,114 +395,79 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "ctor"
-version = "0.1.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
-dependencies = [
- "quote",
- "syn",
-]
-
-[[package]]
 name = "der"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1a467a65c5e759bce6e65eaf91cc29f466cdc57cb65777bd646872a8a1fd4de"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "const-oid",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dirs"
-version = "4.0.0"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
 dependencies = [
  "dirs-sys",
 ]
 
 [[package]]
 name = "dirs-sys"
-version = "0.3.7"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
+ "option-ext",
  "redox_users",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "eclipse-zenoh"
-version = "0.7.0-rc"
-dependencies = [
- "async-std",
- "env_logger",
- "form_urlencoded",
- "futures",
- "json5",
- "log",
- "pyo3",
- "serde_json",
- "uhlc",
- "validated_struct",
- "zenoh",
- "zenoh-buffers",
- "zenoh-cfg-properties",
- "zenoh-core",
-]
-
-[[package]]
-name = "either"
-version = "1.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
-
-[[package]]
 name = "env_logger"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
 dependencies = [
  "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -499,17 +480,17 @@
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "fastrand"
-version = "1.8.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
@@ -522,117 +503,123 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
 dependencies = [
  "futures-core",
  "futures-sink",
  "nanorand",
  "pin-project",
- "spin 0.9.4",
+ "spin 0.9.8",
 ]
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38390104763dc37a5145a53c29c63c1290b5d316d6086ec32c293f6736051bb0"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52ba265a92256105f45b719605a571ffe2d1f0fea3807304b522c1d778f79eed"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04909a7a7e4633ae6c4a9ab280aeb86da1236243a77b694a49eacd659a4bd3ac"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7acc85df6714c176ab5edf386123fafe217be88c0840ec11f199441134a074e2"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00f5fb52a06bdcadeb54e8d3671f8888a39697dcb0b81b23b55174030427f4eb"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-lite"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
+checksum = "49a9d51ce47660b1e808d3c990b4709f2f415d928835a17dfd16991515c46bce"
 dependencies = [
  "fastrand",
  "futures-core",
  "futures-io",
  "memchr",
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-macro"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdfb8ce053d86b91919aad980c220b1fb8401a9394410e1c289ed7e66b61835d"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39c15cf1a4aa79df40f1bb462fb39676d0ad9e366c2a33b590d7c66f4f81fcf9"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ffb393ac5d9a6eaa9d3fdf37ae2776656b706e200c8e16b1bdb227f5198e6ea"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "197676987abd2f9cadff84926f410af1c183608d36641465df73ae8211dc65d6"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -640,27 +627,27 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -680,42 +667,51 @@
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe69f1cbdb6e28af2bac214e943b99ce8a0a06b447d15d3e61161b0423139f3f"
 dependencies = [
  "proc-macro-hack",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "glob"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b919933a397b79c37e33b77bb2aa3dc8eb6e165ad809e58ff75bc7db2e34574"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "gloo-timers"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98c4a8d6391675c6b2ee1a6c8d06e8e2d03605c44cec1270675985a4c2a5500b"
+checksum = "9b995a66bb87bebce9a0f4a95aed01daca4872c050bfcb21653361c03bc35e5c"
 dependencies = [
  "futures-channel",
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
+dependencies = [
+ "ahash",
+]
+
+[[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
@@ -726,14 +722,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "hmac"
@@ -742,42 +744,69 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "home"
-version = "0.5.4"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "747309b4b440c06d57b0b25f2aee03ee9b5e5397d288c60e21fc709bb98a7408"
+checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
 dependencies = [
- "winapi",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "http"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
 ]
 
 [[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
+name = "idna"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inout"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
@@ -791,63 +820,55 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.3"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46112a93252b123d31a119a8d1a1ac19deac4fac6e0e8b0df58f0d4e5870e63c"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipnetwork"
-version = "0.19.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f84f1612606f3753f205a4e9a2efd6fe5b4c573a6269b2cc6c3003d44a0d127"
+checksum = "bf466541e9d546596ee94f9f69590f89473455f88372423e0008fc1a7daf100e"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.1"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927609f78c2913a6f6ac3c27a4fe87f43e2a35367c0c4b0f8265e8f49a104330"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.42.0",
-]
-
-[[package]]
-name = "itertools"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
-dependencies = [
- "either",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4217ad341ebadf8d8e724e264f13e593e0648f5b3e94b3896a5df283be015ecc"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json5"
 version = "0.4.1"
@@ -857,22 +878,31 @@
  "pest",
  "pest_derive",
  "serde",
 ]
 
 [[package]]
 name = "keccak"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3afef3b6eff9ce9d8ff9b3601125eec7f0c8cbac7abd14f355d053fa56c98768"
+checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
 dependencies = [
  "cpufeatures",
 ]
 
 [[package]]
+name = "keyed-set"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b79e110283e09081809ca488cf3a9709270c6d4d4c4a32674c39cc438366615a"
+dependencies = [
+ "hashbrown 0.13.2",
+]
+
+[[package]]
 name = "kv-log-macro"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0de8b303297635ad57c9f5059fd9cee7a47f8e8daa09df0fcd07dd39fb22977f"
 dependencies = [
  "log",
 ]
@@ -884,110 +914,117 @@
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
  "spin 0.5.2",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.138"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db6d7e329c562c5dfab7a46a2afabc8b987ab9a4834c9d1ca04dc54c1546cef8"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.3"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f9f08d8963a6c613f4b1a78f4f4a4dbfadf8e6545b2d72861731e4858b8b47f"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 dependencies = [
- "cfg-if",
  "value-bag",
 ]
 
 [[package]]
+name = "lz4_flex"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b8c72594ac26bfd34f2d99dfced2edfaddfe8a476e3ff2ca0eb293d925c4f83"
+dependencies = [
+ "twox-hash",
+]
+
+[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.5"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "log",
  "wasi",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nanorand"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "nix"
-version = "0.26.1"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46a58d1d356c6597d08cde02c2f09d785b09e28711837b1ed667dc652c08a694"
+checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
 dependencies = [
  "bitflags",
  "cfg-if",
  "libc",
  "memoffset 0.7.1",
  "pin-utils",
  "static_assertions",
@@ -1045,83 +1082,89 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.14.0"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6058e64324c71e02bc2b150e4f3bc8286db6c83092132ffa3f6b1eab0f9def5"
+checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
- "hermit-abi 0.1.19",
+ "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "ordered-float"
-version = "3.4.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d84eb1409416d254e4a9c8fa56cc24701755025b458f0fcd8e59e1f5f40c23bf"
+checksum = "2fc2dbde8f8a79f2102cc474ceb0ad68e3b80b85289ea62389b60e66777e4213"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "parking"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
+checksum = "14f2252c834a40ed9bb5422029649578e63aa341ac401f74e719dd1afda8394e"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.42.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.9"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1de2e551fb905ac83f73f7aedf2f0cb4a0da7e35efa24a202a936269f1f18e1"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "pem-rfc7468"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24d159833a9105500e0398934e205e0773f0b27529557134ecfc51c27646adac"
 dependencies = [
@@ -1132,84 +1175,84 @@
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "pest"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc8bed3549e0f9b0a2a78bf7c0018237a2cdf085eecbbc048e52612438e4e9d0"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdc078600d06ff90d4ed238f0119d84ab5d43dbaad278b0e33a8820293b32344"
+checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28a1af60b1c4148bb269006a750cff8e2ea36aff34d2d96cf7be0b14d1bed23c"
+checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fec8605d59fc2ae0c6c1aefc0c7c7a9769732017c0ce07f7a9cfffa7b4404f20"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
 dependencies = [
  "once_cell",
  "pest",
- "sha1",
+ "sha2",
 ]
 
 [[package]]
 name = "petgraph"
-version = "0.6.2"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6d5014253a1331579ce62aa67443b4a658c5e7dd03d4bc6d302b94474888143"
+checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1240,251 +1283,253 @@
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "pnet"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0caaf5b11fd907ff15cf14a4477bfabca4b37ab9e447a4f8dead969a59cdafad"
+checksum = "cd959a8268165518e2bf5546ba84c7b3222744435616381df3c456fe8d983576"
 dependencies = [
+ "ipnetwork",
  "pnet_base",
  "pnet_datalink",
  "pnet_packet",
+ "pnet_sys",
  "pnet_transport",
 ]
 
 [[package]]
 name = "pnet_base"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d3a993d49e5fd5d4d854d6999d4addca1f72d86c65adf224a36757161c02b6"
+checksum = "872e46346144ebf35219ccaa64b1dffacd9c6f188cd7d012bd6977a2a838f42e"
 dependencies = [
  "no-std-net",
 ]
 
 [[package]]
 name = "pnet_datalink"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e466faf03a98ad27f6e15cd27a2b7cc89e73e640a43527742977bc503c37f8aa"
+checksum = "c302da22118d2793c312a35fb3da6846cb0fab6c3ad53fd67e37809b06cdafce"
 dependencies = [
  "ipnetwork",
  "libc",
  "pnet_base",
  "pnet_sys",
  "winapi",
 ]
 
 [[package]]
 name = "pnet_macros"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48dd52a5211fac27e7acb14cfc9f30ae16ae0e956b7b779c8214c74559cef4c3"
+checksum = "2a780e80005c2e463ec25a6e9f928630049a10b43945fea83207207d4a7606f4"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pnet_macros_support"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89de095dc7739349559913aed1ef6a11e73ceade4897dadc77c5e09de6740750"
+checksum = "e6d932134f32efd7834eb8b16d42418dac87086347d1bc7d142370ef078582bc"
 dependencies = [
  "pnet_base",
 ]
 
 [[package]]
 name = "pnet_packet"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc3b5111e697c39c8b9795b9fdccbc301ab696699e88b9ea5a4e4628978f495f"
+checksum = "8bde678bbd85cb1c2d99dc9fc596e57f03aa725f84f3168b0eaf33eeccb41706"
 dependencies = [
  "glob",
  "pnet_base",
  "pnet_macros",
  "pnet_macros_support",
 ]
 
 [[package]]
 name = "pnet_sys"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "328e231f0add6d247d82421bf3790b4b33b39c8930637f428eef24c4c6a90805"
+checksum = "faf7a58b2803d818a374be9278a1fe8f88fce14b936afbe225000cfcd9c73f16"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "pnet_transport"
-version = "0.31.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff597185e6f1f5671b3122e4dba892a1c73e17c17e723d7669bd9299cbe7f124"
+checksum = "813d1c0e4defbe7ee22f6fe1755f122b77bfb5abe77145b1b5baaf463cab9249"
 dependencies = [
  "libc",
  "pnet_base",
  "pnet_packet",
  "pnet_sys",
 ]
 
 [[package]]
 name = "polling"
-version = "2.5.1"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "166ca89eb77fd403230b9c156612965a81e094ec6ec3aa13663d4c8b113fa748"
+checksum = "4b2d323e8ca7996b3e23126511a523f7e62924d93ecd5ae73b333815b0eb3dce"
 dependencies = [
  "autocfg",
+ "bitflags",
  "cfg-if",
+ "concurrent-queue",
  "libc",
  "log",
- "wepoll-ffi",
- "windows-sys 0.42.0",
+ "pin-project-lite",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro-hack"
-version = "0.5.19"
+version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbf0c48bc1d91375ae5c3cd81e3722dff1abcf81a30960240640d223f59fe0e5"
+checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quinn"
-version = "0.9.3"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445cbfe2382fa023c4f2f3c7e1c95c03dcc1df2bf23cebcb2b13e1402c4394d1"
+checksum = "21252f1c0fc131f1b69182db8f34837e8a69737b8251dff75636a9be0518c324"
 dependencies = [
  "bytes",
  "pin-project-lite",
  "quinn-proto",
  "quinn-udp",
  "rustc-hash",
  "rustls",
  "thiserror",
  "tokio",
  "tracing",
- "webpki",
 ]
 
 [[package]]
 name = "quinn-proto"
-version = "0.9.2"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72ef4ced82a24bb281af338b9e8f94429b6eca01b4e66d899f40031f074e74c9"
+checksum = "85af4ed6ee5a89f26a26086e9089a6643650544c025158449a3626ebf72884b3"
 dependencies = [
  "bytes",
  "rand",
  "ring",
  "rustc-hash",
  "rustls",
  "rustls-native-certs",
  "slab",
  "thiserror",
  "tinyvec",
  "tracing",
- "webpki",
 ]
 
 [[package]]
 name = "quinn-udp"
-version = "0.3.2"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "641538578b21f5e5c8ea733b736895576d0fe329bb883b937db6f4d163dbaaf4"
+checksum = "6df19e284d93757a9fb91d63672f7741b129246a669db09d1c0063071debc0c0"
 dependencies = [
+ "bytes",
  "libc",
- "quinn-proto",
- "socket2",
+ "socket2 0.5.3",
  "tracing",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1521,40 +1566,49 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.0"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "ring"
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
@@ -1565,39 +1619,38 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "ringbuffer-spsc"
-version = "0.1.8"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae677c20a3502f9d82efa27b24aa0d9ca49ee458c43f0fc7bb0a8db3c6b69b6"
+checksum = "2fd1938faa63a2362ee1747afb2d10567d0fb1413b9cbd6198a8541485c4f773"
 dependencies = [
  "array-init",
  "cache-padded",
 ]
 
 [[package]]
 name = "rsa"
-version = "0.7.2"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "094052d5470cbcef561cb848a7209968c9f12dfa6d668f4bca048ac5de51099c"
+checksum = "55a77d189da1fee555ad95b7e50e7457d91c0e089ec68ca69ad2989413bbdab4"
 dependencies = [
  "byteorder",
  "digest",
  "num-bigint-dig",
  "num-integer",
  "num-iter",
  "num-traits",
  "pkcs1",
  "pkcs8",
  "rand_core",
  "signature",
- "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
@@ -1611,36 +1664,36 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.5"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3807b5d10909833d3e9acd1eb5fb988f79376ff10fce42937de71a449c4c588"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.20.7"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "539a2bfe908f471bfa933876bd1eb6a19cf2176d375f82ef7f99530a40e48c2c"
+checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
 dependencies = [
  "log",
  "ring",
+ "rustls-webpki",
  "sct",
- "webpki",
 ]
 
 [[package]]
 name = "rustls-native-certs"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0167bac7a9f490495f3c33013e7722b53cb087ecbe082fb0c6387c96f634ea50"
@@ -1649,35 +1702,44 @@
  "rustls-pemfile",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.1"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+dependencies = [
+ "base64 0.21.2",
+]
+
+[[package]]
+name = "rustls-webpki"
+version = "0.100.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0864aeff53f8c05aa08d86e5ef839d3dfcf07aeba2db32f12db0ef716e87bd55"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
 dependencies = [
- "base64",
+ "ring",
+ "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.11"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "schannel"
-version = "0.1.20"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d6731146462ea25d9244b2ed5fd1d716d25c52e4d54aa4fb0f3c4e9854dbe2"
+checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
- "lazy_static",
- "windows-sys 0.36.1",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
@@ -1690,77 +1752,77 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.7.0"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bc1bb97804af6631813c55739f771071e0f2ed33ee20b68c86ec505d906356c"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
  "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.6.1"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0160a13a177a45bfb43ce71c01580998474f556ad854dcbca936dd2841a5c556"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e25dfac463d778e353db5be2449d1cce89bd6fd23c9f1ea21310ce6e5a1b29c4"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.149"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "256b9932320c590e707b94576e3cc1f7c9024d0ee6612dfbcf1cb106cbe8e055"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.149"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4eae9b04cbffdfd550eb462ed33bc6a1b68c935127d008b27444d08380f94e4"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.89"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "020ff22c755c2ed3f8cf162dbb41a7268d934702f3ed3631656ea597e08fc3db"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.14"
+version = "0.9.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d232d893b10de3eb7258ff01974d6ee20663d8e833263c99409d4b13a0209da"
+checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -1773,97 +1835,118 @@
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
-name = "sha3"
+name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf0c33fae925bdc080598b84bc15c55e7b9a4a43b3c704da051f977469691c9"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
+name = "sha3"
+version = "0.10.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75872d278a8f37ef87fa0ddbda7802605cb18344497949862c0d4dcb291eba60"
 dependencies = [
  "digest",
  "keccak",
 ]
 
 [[package]]
 name = "shellexpand"
-version = "3.0.0"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd1c7ddea665294d484c39fd0c0d2b7e35bbfe10035c5fe1854741a57f6880e1"
+checksum = "da03fa3b94cc19e3ebfc88c4229c49d8f08cdbd1228870a45f0ffdf84988e14b"
 dependencies = [
  "dirs",
 ]
 
 [[package]]
 name = "signal-hook"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a253b5e89e2698464fc26b545c9edceb338e18a89effeeecfea192c3025be29d"
+checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "signature"
-version = "1.6.4"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74233d3b3b2f6d4b006dc19dee745e73e2a6bfb6f93607cd3b02bd5b00797d7c"
+checksum = "5e1788eed21689f9cf370582dfc467ef36ed9c707f073528ddafa8d83e3b8500"
 dependencies = [
  "digest",
  "rand_core",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4614a76b2a8be0058caa9dbbaf66d988527d86d003c11a94fbd335d7661edcef"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "socket2"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e2d2db9033d13a1567121ddd7a095ee144db4e1ca1b1bda3419bc0da294ebd"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "socket2"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2538b18701741680e0322a2302176d3253a35388e2e62f172f64f4f16605f877"
+dependencies = [
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "spin"
-version = "0.9.4"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6002a767bff9e83f8eeecf883ecb8011875a21ae8da43bffb817a57e78cc09"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "spki"
 version = "0.6.0"
@@ -1896,175 +1979,266 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "subtle"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "1.0.105"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60b9b43d45702de4c839cb9b51d9f529c5dd26a4aff255b42b1ebc03e88ee908"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.37"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10deb33631e3c9018b9baf9dcbbc4f737320d2b576bac10f6aefa048fa407e3e"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.37"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "982d17546b47146b28f7c22e3d08465f6b8903d0ea13c1660d9d84a6e7adcdbb"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
+name = "token-cell"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4a2b964fdb303b08a4eab04d7c1bad2bca33f8eee334ccd28802f1041c6eb87"
+dependencies = [
+ "paste",
+]
 
 [[package]]
 name = "tokio"
-version = "1.23.0"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eab6d665857cc6ca78d6e80303a02cea7a7851e85dfbd77cbdc09bd129f1ef46"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
+ "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
- "socket2",
- "windows-sys 0.42.0",
+ "socket2 0.4.9",
+ "tokio-macros",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "tokio-macros"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "tokio-tungstenite"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54319c93411147bced34cb5609a80e0a8e44c5999c93903a81cd866630ec0bfd"
+dependencies = [
+ "futures-util",
+ "log",
+ "tokio",
+ "tungstenite",
 ]
 
 [[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
+ "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
+name = "tungstenite"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30ee6ab729cd4cf0fd55218530c4522ed30b7b6081752839b68fcec8d0960788"
+dependencies = [
+ "base64 0.13.1",
+ "byteorder",
+ "bytes",
+ "http",
+ "httparse",
+ "log",
+ "rand",
+ "sha1",
+ "thiserror",
+ "url",
+ "utf-8",
+]
+
+[[package]]
+name = "twox-hash"
+version = "1.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
+dependencies = [
+ "cfg-if",
+ "static_assertions",
+]
+
+[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "uhlc"
-version = "0.5.1"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7908438f98a5824af02b34c2b31fb369c5764ef835d26df0badbb9897fb28245"
+checksum = "af1438496174a601a35fb41bf9bc408e47384b1df52ddc1252e75ef0ab811322"
 dependencies = [
  "hex",
  "humantime",
  "lazy_static",
  "log",
+ "rand",
  "serde",
- "uuid",
+ "spin 0.9.8",
 ]
 
 [[package]]
+name = "unicode-bidi"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+
+[[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+
+[[package]]
+name = "unicode-normalization"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.4"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e5fa573d8ac5f1a856f8d7be41d390ee973daf97c806b2c1a465e4e1406e68"
+checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
@@ -2072,22 +2246,39 @@
 name = "unzip-n"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e7e85a0596447f0f2ac090e16bc4c516c6fe91771fb0c0ccf7fa3dae896b9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "url"
+version = "2.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
 ]
 
 [[package]]
+name = "utf-8"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
+
+[[package]]
 name = "uuid"
-version = "1.2.2"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "422ee0de9031b5b948b97a8fc04e3aa35230001a722ddd27943e0be31564ce4c"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "validated_struct"
 version = "2.1.0"
@@ -2104,27 +2295,23 @@
 name = "validated_struct_macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d4444a980afa9ef0d29c2a3f4d952ec0495a7a996a9c78b52698b71bc21edb4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "unzip-n",
 ]
 
 [[package]]
 name = "value-bag"
-version = "1.0.0-alpha.9"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2209b78d1249f7e6f3293657c9779fe31ced465df091bbd433a1cf88e916ec55"
-dependencies = [
- "ctor",
- "version_check",
-]
+checksum = "a4d330786735ea358f3bc09eea4caa098569c1c93f342d9aca0514915022fe7e"
 
 [[package]]
 name = "vec_map"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
 
@@ -2144,83 +2331,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.33"
+version = "0.4.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23639446165ca5a5de86ae1d8896b737ae80319560fbaa4c2887b7da6e7ebd7d"
+checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -2230,31 +2417,22 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.22.5"
+version = "0.22.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "368bfe657969fb01238bb756d351dcade285e0f6fcbd36dcb23359a5169975be"
+checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
 dependencies = [
  "webpki",
 ]
 
 [[package]]
-name = "wepoll-ffi"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d743fdedc5c64377b5fc2bc036b01c7fd642205a0d96356034ae3404d49eb7fb"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2279,122 +2457,145 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.36.1"
+version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_msvc 0.36.1",
- "windows_i686_gnu 0.36.1",
- "windows_i686_msvc 0.36.1",
- "windows_x86_64_gnu 0.36.1",
- "windows_x86_64_msvc 0.36.1",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc 0.42.0",
- "windows_i686_gnu 0.42.0",
- "windows_i686_msvc 0.42.0",
- "windows_x86_64_gnu 0.42.0",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc 0.42.0",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "zenoh"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44140d6ebcf2e52ee48acad0e9d960c2b1e868eec021da2538e58373d615fc18"
+checksum = "44ace030c48cef01c4fcaf3797d1ab74f95a882ddeb04098da6ebd82e6bc27de"
 dependencies = [
  "async-global-executor",
  "async-std",
  "async-trait",
- "base64",
+ "base64 0.21.2",
  "env_logger",
  "event-listener",
  "flume",
  "form_urlencoded",
  "futures",
  "git-version",
  "hex",
@@ -2403,375 +2604,442 @@
  "ordered-float",
  "petgraph",
  "rand",
  "regex",
  "rustc_version",
  "serde",
  "serde_json",
- "socket2",
+ "socket2 0.5.3",
  "stop-token",
  "uhlc",
  "uuid",
  "vec_map",
  "zenoh-buffers",
  "zenoh-cfg-properties",
+ "zenoh-codec",
  "zenoh-collections",
  "zenoh-config",
  "zenoh-core",
  "zenoh-crypto",
  "zenoh-link",
+ "zenoh-macros",
  "zenoh-plugin-trait",
  "zenoh-protocol",
- "zenoh-protocol-core",
+ "zenoh-result",
  "zenoh-sync",
  "zenoh-transport",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-buffers"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "244d54f1228d3c53fc69483faafcfcc1b4d670b60cffce17696fc49fbc7a6608"
+checksum = "e2a820c28fc18d3102843219e8fbcdb2b76ed522af5bdf5c5b8cee43a4d3c549"
 dependencies = [
- "async-std",
- "hex",
  "zenoh-collections",
- "zenoh-core",
 ]
 
 [[package]]
 name = "zenoh-cfg-properties"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a963395194bf1b64f67d89333e8089f01568ec7ac28c305847f505452a98006e"
+checksum = "08d3ada269cab26d1d36acb53bddbda703f528c6c5e8369c70f506a3dc47a0f9"
 dependencies = [
- "zenoh-core",
- "zenoh-macros",
+ "zenoh-result",
 ]
 
 [[package]]
-name = "zenoh-collections"
-version = "0.7.0-rc"
+name = "zenoh-codec"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e256d7aff2c9af765d77efbfae7fcb708d2d7f4e179aa201bff2f81ad7a3845"
+checksum = "26a335017307325b945695321ab104053169400c392a441bf9a8cbb66a45e20f"
 dependencies = [
- "async-std",
- "async-trait",
- "flume",
- "log",
- "zenoh-core",
- "zenoh-sync",
+ "uhlc",
+ "zenoh-buffers",
+ "zenoh-protocol",
 ]
 
 [[package]]
+name = "zenoh-collections"
+version = "0.7.2-rc"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3cb3a70ff748ca530a44c4ac4e301138117a34f4899558c15fefb143f826f1a7"
+
+[[package]]
 name = "zenoh-config"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bad1ff61abf28c57e8879ec4286fa29becf7e9bf12555df9a7faddff3bc9ea1b"
+checksum = "163e56bb816e795ef4d77171779c0c154c17b5b2c6c81df4ad3d720e43508964"
 dependencies = [
  "flume",
  "json5",
  "num_cpus",
  "serde",
  "serde_json",
  "serde_yaml",
  "validated_struct",
  "zenoh-cfg-properties",
  "zenoh-core",
- "zenoh-protocol-core",
+ "zenoh-protocol",
+ "zenoh-result",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-core"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b0f55158f3f83555db74d4cf5ebc34f90df5d2992cc0de67eba69b99628605e"
+checksum = "680ee2dea516a2ecb8446691ebb9914d0cd54c223d3a1759d422d8ddfe585727"
 dependencies = [
- "anyhow",
  "async-std",
  "lazy_static",
- "zenoh-macros",
+ "zenoh-result",
 ]
 
 [[package]]
 name = "zenoh-crypto"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "653ba15479a0e3f1a94d7f079babc52f742f3a2bd995c59bc250cfc9a789dbbc"
+checksum = "41e2b1c3850d7f052daa24823c4b496610d0b150d3624e08d9383d7b9c97714b"
 dependencies = [
  "aes",
  "hmac",
  "rand",
  "rand_chacha",
  "sha3",
- "zenoh-core",
+ "zenoh-result",
+]
+
+[[package]]
+name = "zenoh-keyexpr"
+version = "0.7.2-rc"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecf3b237a6d2ac9df0b4204fe5a178ddb586a4a7e7dd73fe680e0cb0517dab86"
+dependencies = [
+ "hashbrown 0.13.2",
+ "keyed-set",
+ "rand",
+ "serde",
+ "token-cell",
+ "zenoh-result",
 ]
 
 [[package]]
 name = "zenoh-link"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e58770c73cf0b5ec8fbe104d609eec83f9bc3463ea23a583c8b465de77f7d27"
+checksum = "cec4563b1c587dc56d8dfa193e7d572794445171239c704083fc668edb939375"
 dependencies = [
  "async-std",
  "async-trait",
  "zenoh-cfg-properties",
  "zenoh-config",
- "zenoh-core",
  "zenoh-link-commons",
  "zenoh-link-quic",
  "zenoh-link-tcp",
  "zenoh-link-tls",
  "zenoh-link-udp",
  "zenoh-link-unixsock_stream",
- "zenoh-protocol-core",
+ "zenoh-link-ws",
+ "zenoh-protocol",
+ "zenoh-result",
 ]
 
 [[package]]
 name = "zenoh-link-commons"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21aab9eeb2aba53e37aae57467ffca1268d209811c5e2f39761aab4c1343bce3"
+checksum = "6a4cd6695c8ef48d6e4b1d94afefff756a3c1c67ae76c7da72b1d7a99611b009"
 dependencies = [
  "async-std",
  "async-trait",
  "flume",
  "serde",
+ "typenum",
  "zenoh-buffers",
  "zenoh-cfg-properties",
- "zenoh-core",
+ "zenoh-codec",
  "zenoh-protocol",
- "zenoh-protocol-core",
+ "zenoh-result",
 ]
 
 [[package]]
 name = "zenoh-link-quic"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9f1354094eb4d5e4b864b5aa385efce46f94a43f6ba57dd9ea9a017e6e74176"
+checksum = "bbfe8ff3a44c697e34bf982a8a207ae6b8eb359370e69e0d1e65fa5fc1fe23d1"
 dependencies = [
  "async-std",
  "async-trait",
  "futures",
  "log",
  "quinn",
  "rustls",
  "rustls-native-certs",
  "rustls-pemfile",
  "webpki",
  "zenoh-cfg-properties",
  "zenoh-config",
  "zenoh-core",
  "zenoh-link-commons",
- "zenoh-protocol-core",
+ "zenoh-protocol",
+ "zenoh-result",
  "zenoh-sync",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-link-tcp"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55ffc29707a50680dba124dd4d8bc3bc19feb158db8312433bfc3078f7b8f1ef"
+checksum = "4697617272f345363134afc9121b36fdab17b5f8ec8072209b8298a2e82e0964"
 dependencies = [
  "async-std",
  "async-trait",
  "log",
  "zenoh-core",
  "zenoh-link-commons",
- "zenoh-protocol-core",
+ "zenoh-protocol",
+ "zenoh-result",
  "zenoh-sync",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-link-tls"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a5630b3a218c7179191dab78ebc45da1837793951bddb8fda4f5900b47da552"
+checksum = "3d66f1b553261ab8162ecc4c6244911a637f2e647fb651ba61e933782db44741"
 dependencies = [
  "async-rustls",
  "async-std",
  "async-trait",
  "futures",
  "log",
  "rustls-pemfile",
  "webpki",
  "webpki-roots",
  "zenoh-cfg-properties",
  "zenoh-config",
  "zenoh-core",
  "zenoh-link-commons",
- "zenoh-protocol-core",
+ "zenoh-protocol",
+ "zenoh-result",
  "zenoh-sync",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-link-udp"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176494947bd3a6aa10baa469afa4572635822683830808cd71d5554ce15dfebb"
+checksum = "0a4ffd1810e0a7f722b801f86618f8f2bc6622a6e4988216993b9239785a1c27"
 dependencies = [
  "async-std",
  "async-trait",
  "log",
- "socket2",
+ "socket2 0.5.3",
+ "zenoh-buffers",
  "zenoh-collections",
  "zenoh-core",
  "zenoh-link-commons",
- "zenoh-protocol-core",
+ "zenoh-protocol",
+ "zenoh-result",
  "zenoh-sync",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-link-unixsock_stream"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d9974305820f92478490ba8b8f119eb5b7d7b4998a7125d1510f6e69f3f81d1"
+checksum = "235ff6a7fc8fba0367f02007d79664c0d1566a6aa4c5afafa7e52680c95b0c95"
 dependencies = [
  "async-std",
  "async-trait",
  "futures",
  "log",
  "nix",
  "uuid",
  "zenoh-core",
  "zenoh-link-commons",
- "zenoh-protocol-core",
+ "zenoh-protocol",
+ "zenoh-result",
+ "zenoh-sync",
+]
+
+[[package]]
+name = "zenoh-link-ws"
+version = "0.7.2-rc"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7aeeacdce03376fe41a5792efeffc401322ec299e49f51e7083a64b920b4e27"
+dependencies = [
+ "async-std",
+ "async-trait",
+ "futures-util",
+ "log",
+ "tokio",
+ "tokio-tungstenite",
+ "url",
+ "zenoh-core",
+ "zenoh-link-commons",
+ "zenoh-protocol",
+ "zenoh-result",
  "zenoh-sync",
+ "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-macros"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a9ac20b120990778cca204ee46c43a37ed4ffbc331e95702615490f9c169de8"
+checksum = "439e4a80f251b2eccb0fc3d3930dee15c9a510873a2aedc0fe3825b03b662eb5"
 dependencies = [
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.109",
  "unzip-n",
+ "zenoh-keyexpr",
 ]
 
 [[package]]
 name = "zenoh-plugin-trait"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3b8bfb8e2625e1150dab46b7a4433f866aa06af763237d564b1aa8f6aaf0b29"
+checksum = "c76064f47c2b4e5e250f0981d4cda4ac6043cc6cf3625b6bc8c7dae38c0cf403"
 dependencies = [
  "libloading",
  "log",
  "serde_json",
- "zenoh-core",
  "zenoh-macros",
+ "zenoh-result",
  "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-protocol"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "174a00456e29d941a4230148fd184953e95883bde47a4cfc1a508e0aaec89a89"
+checksum = "e52290acad7decbae601bce3b6c394d584c41ca93d948aac27be964eeb38ee48"
+dependencies = [
+ "hex",
+ "rand",
+ "serde",
+ "uhlc",
+ "uuid",
+ "zenoh-buffers",
+ "zenoh-keyexpr",
+ "zenoh-result",
+]
+
+[[package]]
+name = "zenoh-python"
+version = "0.7.2-rc"
 dependencies = [
+ "async-std",
+ "env_logger",
+ "flume",
+ "form_urlencoded",
+ "futures",
+ "json5",
  "log",
+ "pyo3",
+ "serde_json",
  "uhlc",
+ "validated_struct",
+ "zenoh",
  "zenoh-buffers",
+ "zenoh-cfg-properties",
  "zenoh-core",
- "zenoh-protocol-core",
 ]
 
 [[package]]
-name = "zenoh-protocol-core"
-version = "0.7.0-rc"
+name = "zenoh-result"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf3eaea2095d2c13fefdae25aca813b3644fc15e1441e16a4398b5113033753"
+checksum = "42ae11e6ca8e51c51299097351f7b09833047bfa2bf6e0b9db8a4ff9496038c0"
 dependencies = [
- "hex",
- "itertools",
- "lazy_static",
- "rand",
- "serde",
- "uhlc",
- "uuid",
- "zenoh-core",
+ "anyhow",
 ]
 
 [[package]]
 name = "zenoh-sync"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "821070b62a55d4c8a22e1e06c939c1f2d94767e660df9fcbea377781f72f59bf"
+checksum = "8e4954bb734cc609e657be29afb33feb571b5eb0a042cc3b4c163ea75aae1e1d"
 dependencies = [
  "async-std",
  "event-listener",
  "flume",
  "futures",
  "tokio",
+ "zenoh-buffers",
+ "zenoh-collections",
  "zenoh-core",
 ]
 
 [[package]]
 name = "zenoh-transport"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce4387cfc02cb86383de8e65ab1eb204e3908c5f1db9e6b4defd8ad530c9ddea"
+checksum = "63ad8510f54f7dfe6cbc42588a01c68b3381e5106863c3e2ee025d736b62663e"
 dependencies = [
  "async-executor",
  "async-global-executor",
  "async-std",
  "async-trait",
  "flume",
  "log",
+ "lz4_flex",
  "paste",
  "rand",
  "ringbuffer-spsc",
  "rsa",
  "serde",
  "zenoh-buffers",
  "zenoh-cfg-properties",
+ "zenoh-codec",
  "zenoh-collections",
  "zenoh-config",
  "zenoh-core",
  "zenoh-crypto",
  "zenoh-link",
  "zenoh-protocol",
- "zenoh-protocol-core",
+ "zenoh-result",
  "zenoh-sync",
+ "zenoh-util",
 ]
 
 [[package]]
 name = "zenoh-util"
-version = "0.7.0-rc"
+version = "0.7.2-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54646455dad3940535e97cce03f1b604265177349133903d989bc72e00011404"
+checksum = "a3cb03293bad61dd89ae47f52ad2ab08866857d14fb59b6358526c8128e2343d"
 dependencies = [
  "async-std",
+ "async-trait",
  "clap",
+ "flume",
  "futures",
  "hex",
  "home",
  "humantime",
  "lazy_static",
  "libc",
  "libloading",
  "log",
  "pnet",
  "pnet_datalink",
  "shellexpand",
  "winapi",
- "zenoh-cfg-properties",
- "zenoh-collections",
  "zenoh-core",
- "zenoh-crypto",
- "zenoh-sync",
+ "zenoh-protocol",
+ "zenoh-result",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

### Comparing `eclipse_zenoh-0.7.0rc0/PKG-INFO` & `eclipse_zenoh-0.7.2rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eclipse-zenoh
-Version: 0.7.0rc0
+Version: 0.7.2rc0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Rust
 Classifier: Intended Audience :: Developers
@@ -16,19 +16,20 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
 License-File: NOTICE.md
 Summary: The python API for Eclipse zenoh
 Author: kydos <angelo@icorsaro.net>, Julien Enoch <julien@enoch.fr>, Olivier Hécart <olivier.hecart@adlinktech.com>, Luca Cominardi <luca.cominardi@gmail.com>, Pierre Avital <pierre.avital@adlinktech.com>
 Author-email: kydos <angelo@icorsaro.net>, Julien Enoch <julien@enoch.fr>, Olivier Hécart <olivier.hecart@adlinktech.com>, Luca Cominardi <luca.cominardi@gmail.com>, Pierre Avital <pierre.avital@adlinktech.com>
+License: EPL-2.0 OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://readthedocs.org/projects/zenoh-python/
-Project-URL: Bug Tracker, https://github.com/eclipse-zenoh/zenoh-python/issues
 Project-URL: Source Code, https://github.com/eclipse-zenoh/zenoh-python
+Project-URL: Bug Tracker, https://github.com/eclipse-zenoh/zenoh-python/issues
+Project-URL: Documentation, https://readthedocs.org/projects/zenoh-python/
 
 <img src="https://raw.githubusercontent.com/eclipse-zenoh/zenoh/master/zenoh-dragon.png" height="150">
 
 [![CI](https://github.com/eclipse-zenoh/zenoh-python/workflows/CI/badge.svg)](https://github.com/eclipse-zenoh/zenoh-python/actions?query=workflow%3A%22CI%22)
 [![Documentation Status](https://readthedocs.org/projects/zenoh-python/badge/?version=latest)](https://zenoh-python.readthedocs.io/en/latest/?badge=latest)
 [![Discussion](https://img.shields.io/badge/discussion-on%20github-blue)](https://github.com/eclipse-zenoh/roadmap/discussions)
 [![Discord](https://img.shields.io/badge/chat-on%20discord-blue)](https://discord.gg/2GJ958VuHs)
@@ -113,9 +114,9 @@
 
 
 -------------------------------
 ## Running the Examples
 
 The simplest way to run some of the example is to get a Docker image of the **zenoh** network router (see https://github.com/eclipse-zenoh/zenoh#how-to-test-it) and then to run the examples on your machine.
 
-Then, run the zenoh-python examples following the instructions in [examples/zenoh/README.md](https://github.com/eclipse-zenoh/zenoh-python/blob/master/examples/zenoh/README.md)
+Then, run the zenoh-python examples following the instructions in [examples/README.md](https://github.com/eclipse-zenoh/zenoh-python/tree/master/examples#readme)
```

