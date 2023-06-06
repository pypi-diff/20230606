# Comparing `tmp/color_palette_extract-0.4.0.tar.gz` & `tmp/color_palette_extract-0.5.0.tar.gz`

## Comparing `color_palette_extract-0.4.0.tar` & `color_palette_extract-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 color_palette_extract-0.4.0/Cargo.toml
--rwxr-xr-x   0     1001      123      242 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/.github/workflows/build-wheels.sh
--rw-r--r--   0     1001      123     2835 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/.github/workflows/build.yml
--rw-r--r--   0     1001      123      685 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/.gitignore
--rw-r--r--   0     1001      123       24 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/README.md
--rw-r--r--   0     1001      123      329 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/pyproject.toml
--rw-r--r--   0     1001      123      292 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/run.py
--rw-r--r--   0     1001      123     1493 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/src/lib.rs
--rw-r--r--   0     1001      123     6155 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/airbnb.png
--rw-r--r--   0     1001      123  1152390 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/instagram.png
--rw-r--r--   0     1001      123     8948 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/instagram.svg
--rw-r--r--   0     1001      123    10752 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/mastercard.webp
--rw-r--r--   0     1001      123    49709 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/test.jpg
--rw-r--r--   0     1001      123     5286 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/test2.png
--rw-r--r--   0     1001      123     2557 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/test3.jpeg
--rw-r--r--   0     1001      123    32261 2023-05-31 07:33:51.000000 color_palette_extract-0.4.0/Cargo.lock
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 color_palette_extract-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 color_palette_extract-0.5.0/Cargo.toml
+-rwxr-xr-x   0     1001      123      242 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/.github/workflows/build-wheels.sh
+-rw-r--r--   0     1001      123     2542 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0     1001      123      685 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/.gitignore
+-rw-r--r--   0     1001      123       24 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/README.md
+-rw-r--r--   0     1001      123      329 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/pyproject.toml
+-rwxr-xr-x   0     1001      123     1041 2023-06-06 07:22:03.000000 color_palette_extract-0.5.0/run-maturin-action.sh
+-rw-r--r--   0     1001      123      292 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/run.py
+-rw-r--r--   0     1001      123     1493 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      123     6155 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/airbnb.png
+-rw-r--r--   0     1001      123  1152390 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/instagram.png
+-rw-r--r--   0     1001      123     8948 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/instagram.svg
+-rw-r--r--   0     1001      123    10752 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/mastercard.webp
+-rw-r--r--   0     1001      123    49709 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/test.jpg
+-rw-r--r--   0     1001      123     5286 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/test2.png
+-rw-r--r--   0     1001      123     2557 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/test/test3.jpeg
+-rw-r--r--   0     1001      123    32261 2023-06-06 07:21:33.000000 color_palette_extract-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 color_palette_extract-0.5.0/PKG-INFO
```

### Comparing `color_palette_extract-0.4.0/.github/workflows/build.yml` & `color_palette_extract-0.5.0/.github/workflows/build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -7,33 +7,26 @@
   # push:
   #   tags:
   #      - 'v*'
 
 jobs:
   linux-wheels:
     runs-on: ubuntu-latest
-    # container: quay.io/pypa/manylinux1_x86_64
+    strategy:
+      matrix:
+        target: [x86_64, i686, aarch64]
     steps:
-      - uses: actions/checkout@v1
-      - uses: actions-rs/toolchain@v1
-        with:
-          profile: minimal
-          toolchain: stable
-          override: true
-      - uses: messense/maturin-action@v1
+      - uses: actions/checkout@v3
+      - uses: PyO3/maturin-action@v1
         with:
+          target: ${{ matrix.target }}
           maturin-version: latest
           command: build
+          manylinux: auto
           args: --release --sdist -i 3.8 3.9 3.10 3.11
-      #  - name: Build wheels
-      #    run: |
-      #      curl https://sh.rustup.rs -sSf | sh -s -- -y
-      #      source $HOME/.cargo/env
-      #      rustup default nightly-2019-12-11
-      #      bash .github/workflows/build-wheels.sh
       - uses: actions/upload-artifact@v1
         with:
           name: linux-wheels
           path: target/wheels/
 
   osx-wheels:
     runs-on: macos-latest
```

### Comparing `color_palette_extract-0.4.0/.gitignore` & `color_palette_extract-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/src/lib.rs` & `color_palette_extract-0.5.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/airbnb.png` & `color_palette_extract-0.5.0/test/airbnb.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/instagram.png` & `color_palette_extract-0.5.0/test/instagram.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/instagram.svg` & `color_palette_extract-0.5.0/test/instagram.svg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/mastercard.webp` & `color_palette_extract-0.5.0/test/mastercard.webp`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/test.jpg` & `color_palette_extract-0.5.0/test/test.jpg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/test2.png` & `color_palette_extract-0.5.0/test/test2.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/test/test3.jpeg` & `color_palette_extract-0.5.0/test/test3.jpeg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.4.0/Cargo.lock` & `color_palette_extract-0.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "color_palette_extract"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "colors-transform",
  "dominant_color",
  "image",
  "pyo3",
  "pyo3-file",
 ]
```

