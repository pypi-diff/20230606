# Comparing `tmp/lzstring_optimized-0.5.0.tar.gz` & `tmp/lzstring_optimized-0.6.0.tar.gz`

## Comparing `lzstring_optimized-0.5.0.tar` & `lzstring_optimized-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 lzstring_optimized-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123     6148 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.DS_Store
--rw-r--r--   0     1001      123      242 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.github/workflows/build-wheels.sh
--rw-r--r--   0     1001      123     2847 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.github/workflows/build.yaml
--rw-r--r--   0     1001      123        6 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.gitignore
--rw-r--r--   0     1001      123       69 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/README.md
--rw-r--r--   0     1001      123       34 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/lzstring_optimized/__init__.py
--rw-r--r--   0     1001      123      102 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/lzstring_optimized/lzstring_optimized.pyi
--rw-r--r--   0     1001      123        0 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/lzstring_optimized/py.typed
--rw-r--r--   0     1001      123      195 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/pyproject.toml
--rw-r--r--   0     1001      123      432 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/run.py
--rw-r--r--   0     1001      123     2042 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123     6863 2023-05-25 14:18:47.000000 lzstring_optimized-0.5.0/Cargo.lock
--rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 lzstring_optimized-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 lzstring_optimized-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      123     6148 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/.DS_Store
+-rw-r--r--   0     1001      123      242 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/.github/workflows/build-wheels.sh
+-rw-r--r--   0     1001      123     2542 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123        6 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/.gitignore
+-rw-r--r--   0     1001      123       69 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/README.md
+-rw-r--r--   0     1001      123       34 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/lzstring_optimized/__init__.py
+-rw-r--r--   0     1001      123      102 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/lzstring_optimized/lzstring_optimized.pyi
+-rw-r--r--   0     1001      123        0 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/lzstring_optimized/py.typed
+-rw-r--r--   0     1001      123      195 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/pyproject.toml
+-rwxr-xr-x   0     1001      123     1050 2023-06-06 07:23:51.000000 lzstring_optimized-0.6.0/run-maturin-action.sh
+-rw-r--r--   0     1001      123      432 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/run.py
+-rw-r--r--   0     1001      123     2042 2023-06-06 07:22:50.000000 lzstring_optimized-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      123     6863 2023-06-06 07:24:18.000000 lzstring_optimized-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 lzstring_optimized-0.6.0/PKG-INFO
```

### Comparing `lzstring_optimized-0.5.0/.DS_Store` & `lzstring_optimized-0.6.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `lzstring_optimized-0.5.0/.github/workflows/build.yaml` & `lzstring_optimized-0.6.0/.github/workflows/build.yaml`

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
@@ -99,9 +92,8 @@
         run: ls wheels
 
       - name: Publish a Python distribution to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages_dir: wheels/
-          verify_metadata: false
-          
+          verify_metadata: false
```

### Comparing `lzstring_optimized-0.5.0/src/lib.rs` & `lzstring_optimized-0.6.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lzstring_optimized-0.5.0/Cargo.lock` & `lzstring_optimized-0.6.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 [[package]]
 name = "lz-str"
 version = "0.1.0"
 source = "git+https://github.com/spl0i7/lz-str-rs#c47180bbedfc840c31369378459a5aafd352fac1"
 
 [[package]]
 name = "lzstring_optimized"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "lz-str",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
```

