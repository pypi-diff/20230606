# Comparing `tmp/rlviser_py-0.1.0.tar.gz` & `tmp/rlviser_py-0.1.1.tar.gz`

## Comparing `rlviser_py-0.1.0.tar` & `rlviser_py-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 rlviser_py-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2813 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/.gitignore
--rw-r--r--   0     1001      123      390 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123       74 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/rustfmt.toml
--rw-r--r--   0     1001      123    32523 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/src/bytes.rs
--rw-r--r--   0     1001      123      995 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/src/gym.rs
--rw-r--r--   0     1001      123     4237 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     1351 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/src/socket.rs
--rw-r--r--   0     1001      123     7866 2023-06-06 12:43:40.000000 rlviser_py-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 rlviser_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 rlviser_py-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2774 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/.gitignore
+-rw-r--r--   0     1001      123     1070 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/LICENSE
+-rw-r--r--   0     1001      123      490 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/README.md
+-rw-r--r--   0     1001      123      390 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123      255 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/rlviser_py.pyi
+-rw-r--r--   0     1001      123       74 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/rustfmt.toml
+-rw-r--r--   0     1001      123    32523 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/bytes.rs
+-rw-r--r--   0     1001      123      995 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/gym.rs
+-rw-r--r--   0     1001      123     4209 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     1351 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/socket.rs
+-rw-r--r--   0     1001      123     7635 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.1.1/PKG-INFO
```

### Comparing `rlviser_py-0.1.0/.github/workflows/CI.yml` & `rlviser_py-0.1.1/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,14 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows, macos, sdist]
-    permissions:
-      id-token: write
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `rlviser_py-0.1.0/.gitignore` & `rlviser_py-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.0/src/bytes.rs` & `rlviser_py-0.1.1/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.0/src/gym.rs` & `rlviser_py-0.1.1/src/gym.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.0/src/lib.rs` & `rlviser_py-0.1.1/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         connection_point_offset: Vec3A::new(-33.75, 29.5, 20.755),
     },
     dodge_deadzone: 0.5,
 };
 
 /// Reads the RLGym state and sends it to RLViser to render
 #[pyfunction]
-fn render_rlgym(gym_state: GymState) -> PyResult<()> {
+fn render_rlgym(gym_state: GymState) {
     // construct the game state
     let game_state = GameState {
         tick_count: TICK_COUNT.fetch_add(1, Ordering::SeqCst),
         tick_rate: TICK_RATE,
         ball: BallState {
             pos: gym_state.ball.position.into(),
             vel: gym_state.ball.linear_velocity.into(),
@@ -121,16 +121,14 @@
                 },
                 config: OCTANE,
             })
             .collect(),
     };
 
     socket::send_game_state(&game_state).unwrap();
-
-    Ok(())
 }
 
 /// Send the quit signal to RLViser
 #[pyfunction]
 fn quit() {
     socket::quit().unwrap();
 }
```

### Comparing `rlviser_py-0.1.0/src/socket.rs` & `rlviser_py-0.1.1/src/socket.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.0/Cargo.lock` & `rlviser_py-0.1.1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.145"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc86cde3ff845662b8f4ef6cb50ea0e20c524eb3d29ae048287e06a1b3fa6a81"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -71,23 +71,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
@@ -162,24 +162,24 @@
 checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "glam",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
@@ -220,71 +220,62 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

