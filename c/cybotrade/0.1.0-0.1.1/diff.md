# Comparing `tmp/cybotrade-0.1.0.tar.gz` & `tmp/cybotrade-0.1.1.tar.gz`

## Comparing `cybotrade-0.1.0.tar` & `cybotrade-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,58 @@
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 cybotrade-0.1.0/Cargo.toml
--rw-rw-r--   0        0        0      960 2023-06-04 17:50:45.000000 cybotrade-0.1.0/Dockerfile
--rw-r--r--   0        0        0       58 2023-06-03 07:58:34.000000 cybotrade-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0      783 2023-06-03 15:22:50.000000 cybotrade-0.1.0/README.md
--rw-r--r--   0        0        0      362 2023-06-03 15:52:13.000000 cybotrade-0.1.0/cybotrade/__init__.py
--rw-r--r--   0        0        0      199 2023-06-03 15:22:59.000000 cybotrade-0.1.0/noxfile.py
--rwxr-xr-x   0        0        0  4654072 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/bin/protoc
--rw-r--r--   0        0        0     5909 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/any.proto
--rw-r--r--   0        0        0     7734 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/api.proto
--rw-r--r--   0        0        0     8754 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/compiler/plugin.proto
--rw-r--r--   0        0        0    38497 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     4895 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/duration.proto
--rw-r--r--   0        0        0     2363 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/empty.proto
--rw-r--r--   0        0        0     8185 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/field_mask.proto
--rw-r--r--   0        0        0     2341 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/source_context.proto
--rw-r--r--   0        0        0     3779 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/struct.proto
--rw-r--r--   0        0        0     6459 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/timestamp.proto
--rw-r--r--   0        0        0     6126 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/type.proto
--rw-r--r--   0        0        0     4042 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/include/google/protobuf/wrappers.proto
--r-xr-xr-x   0        0        0      721 1980-01-01 00:00:00.000000 cybotrade-0.1.0/proto/readme.txt
--rw-r--r--   0        0        0  1585982 2023-06-04 17:51:20.000000 cybotrade-0.1.0/protoc-21.12-linux-x86_64.zip
--rwxrwxr-x   0        0        0      411 2023-06-04 17:43:28.000000 cybotrade-0.1.0/publish.sh
--rw-r--r--   0        0        0      124 2023-06-03 15:23:03.000000 cybotrade-0.1.0/pyproject.toml
--rw-rw-r--   0        0        0      127 2023-06-03 19:51:49.000000 cybotrade-0.1.0/pytest.ini
--rw-rw-r--   0        0        0       32 2023-06-03 19:51:26.000000 cybotrade-0.1.0/pytest.ini.example
--rw-r--r--   0        0        0      106 2023-06-03 20:19:50.000000 cybotrade-0.1.0/requirements-dev.txt
--rw-rw-r--   0        0        0     5358 2023-06-03 20:41:33.000000 cybotrade-0.1.0/src/datahub.rs
--rw-r--r--   0        0        0      826 2023-06-03 20:34:49.000000 cybotrade-0.1.0/src/lib.rs
--rw-rw-r--   0        0        0     5686 2023-06-04 16:39:15.000000 cybotrade-0.1.0/src/market_collector.rs
--rw-r--r--   0        0        0      299 2023-06-03 20:09:21.000000 cybotrade-0.1.0/tests/test_cybotrade.py
--rw-r--r--   0        0        0      917 2023-06-03 20:27:52.000000 cybotrade-0.1.0/tests/test_datahub.py
--rw-r--r--   0        0        0      944 2023-06-04 16:24:41.000000 cybotrade-0.1.0/tests/test_market_collector.py
--rw-rw-r--   0        0        0    81079 2023-06-04 04:57:10.000000 cybotrade-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 cybotrade-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cybotrade-0.1.1/Cargo.toml
+-rw-rw-r--   0        0        0       32 2023-06-03 15:55:28.000000 cybotrade-0.1.1/.cargo/config.toml
+-rw-rw-r--   0        0        0        9 2023-06-03 15:50:42.000000 cybotrade-0.1.1/.conda_config
+-rw-rw-r--   0        0        0       27 2023-06-06 10:13:28.000000 cybotrade-0.1.1/.dockerignore
+-rw-rw-r--   0        0        0      681 2023-06-06 09:41:00.000000 cybotrade-0.1.1/.gitignore
+-rw-rw-r--   0        0        0      164 2023-06-05 17:37:47.000000 cybotrade-0.1.1/.vscode/settings.json
+-rw-rw-r--   0        0        0      960 2023-06-04 17:50:45.000000 cybotrade-0.1.1/Dockerfile
+-rw-r--r--   0        0        0       58 2023-06-03 07:58:34.000000 cybotrade-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     1756 2023-06-05 03:27:21.000000 cybotrade-0.1.1/README.md
+-rw-r--r--   0        0        0      362 2023-06-05 04:15:04.000000 cybotrade-0.1.1/cybotrade/__init__.py
+-rw-rw-r--   0        0        0        0 2023-06-05 04:33:06.000000 cybotrade-0.1.1/cybotrade/datahub.py
+-rw-rw-r--   0        0        0     1555 2023-06-05 17:26:44.000000 cybotrade-0.1.1/cybotrade/datahub.pyi
+-rw-rw-r--   0        0        0        0 2023-06-05 04:37:56.000000 cybotrade-0.1.1/cybotrade/market_collector.py
+-rw-rw-r--   0        0        0     3273 2023-06-06 10:11:47.000000 cybotrade-0.1.1/cybotrade/market_collector.pyi
+-rw-rw-r--   0        0        0        0 2023-06-05 17:32:38.000000 cybotrade-0.1.1/cybotrade/models.py
+-rw-rw-r--   0        0        0     3531 2023-06-06 10:10:26.000000 cybotrade-0.1.1/cybotrade/models.pyi
+-rw-rw-r--   0        0        0        0 2023-06-05 03:51:51.000000 cybotrade-0.1.1/cybotrade/py.typed
+-rw-rw-r--   0        0        0        0 2023-06-05 18:49:41.000000 cybotrade-0.1.1/cybotrade/trader.py
+-rw-rw-r--   0        0        0     6201 2023-06-06 03:59:08.000000 cybotrade-0.1.1/cybotrade/trader.pyi
+-rw-r--r--   0        0        0      199 2023-06-03 15:22:59.000000 cybotrade-0.1.1/noxfile.py
+-rwxr-xr-x   0        0        0  4654072 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/bin/protoc
+-rw-r--r--   0        0        0     5909 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/any.proto
+-rw-r--r--   0        0        0     7734 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/api.proto
+-rw-r--r--   0        0        0     8754 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/compiler/plugin.proto
+-rw-r--r--   0        0        0    38497 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     4895 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/duration.proto
+-rw-r--r--   0        0        0     2363 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/empty.proto
+-rw-r--r--   0        0        0     8185 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/field_mask.proto
+-rw-r--r--   0        0        0     2341 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/source_context.proto
+-rw-r--r--   0        0        0     3779 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/struct.proto
+-rw-r--r--   0        0        0     6459 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/timestamp.proto
+-rw-r--r--   0        0        0     6126 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/type.proto
+-rw-r--r--   0        0        0     4042 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/include/google/protobuf/wrappers.proto
+-r-xr-xr-x   0        0        0      721 1980-01-01 00:00:00.000000 cybotrade-0.1.1/proto/readme.txt
+-rw-r--r--   0        0        0  1585982 2023-06-06 10:26:53.000000 cybotrade-0.1.1/protoc-21.12-linux-x86_64.zip
+-rwxrwxr-x   0        0        0      411 2023-06-04 17:43:28.000000 cybotrade-0.1.1/publish.sh
+-rw-r--r--   0        0        0      124 2023-06-06 09:37:47.000000 cybotrade-0.1.1/pyproject.toml
+-rw-rw-r--   0        0        0       32 2023-06-03 19:51:26.000000 cybotrade-0.1.1/pytest.ini.example
+-rw-r--r--   0        0        0      132 2023-06-05 17:38:07.000000 cybotrade-0.1.1/requirements-dev.txt
+-rw-rw-r--   0        0        0     3109 2023-06-05 17:23:56.000000 cybotrade-0.1.1/src/datahub.rs
+-rw-rw-r--   0        0        0       87 2023-06-06 08:23:39.000000 cybotrade-0.1.1/src/error.rs
+-rw-r--r--   0        0        0     1412 2023-06-06 08:22:27.000000 cybotrade-0.1.1/src/lib.rs
+-rw-rw-r--   0        0        0     4855 2023-06-06 10:08:34.000000 cybotrade-0.1.1/src/market_collector.rs
+-rw-rw-r--   0        0        0    34687 2023-06-06 10:08:02.000000 cybotrade-0.1.1/src/models.rs
+-rw-rw-r--   0        0        0      510 2023-06-06 08:21:48.000000 cybotrade-0.1.1/src/notification.rs
+-rw-rw-r--   0        0        0     7411 2023-06-06 09:37:22.000000 cybotrade-0.1.1/src/strategy/live_strategy.rs
+-rw-rw-r--   0        0        0       88 2023-06-06 07:58:09.000000 cybotrade-0.1.1/src/strategy/mod.rs
+-rw-rw-r--   0        0        0     1524 2023-06-06 09:33:38.000000 cybotrade-0.1.1/src/strategy/strategy.rs
+-rw-rw-r--   0        0        0       68 2023-06-06 06:15:15.000000 cybotrade-0.1.1/src/trader/mod.rs
+-rw-rw-r--   0        0        0     8583 2023-06-06 07:30:23.000000 cybotrade-0.1.1/src/trader/py.rs
+-rw-rw-r--   0        0        0    11079 2023-06-06 07:29:50.000000 cybotrade-0.1.1/src/trader/trader.rs
+-rw-rw-r--   0        0        0      260 2023-06-06 06:19:39.000000 cybotrade-0.1.1/src/utils.rs
+-rw-r--r--   0        0        0      320 2023-06-05 05:26:17.000000 cybotrade-0.1.1/tests/test_cybotrade.py
+-rw-r--r--   0        0        0      755 2023-06-05 17:25:56.000000 cybotrade-0.1.1/tests/test_datahub.py
+-rw-rw-r--   0        0        0      764 2023-06-05 17:49:09.000000 cybotrade-0.1.1/tests/test_market_collector.py
+-rw-r--r--   0        0        0     2547 2023-06-06 05:04:36.000000 cybotrade-0.1.1/tests/test_trader.py
+-rw-rw-r--   0        0        0   100353 2023-06-06 09:21:17.000000 cybotrade-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1981 1970-01-01 00:00:00.000000 cybotrade-0.1.1/PKG-INFO
```

### Comparing `cybotrade-0.1.0/Cargo.toml` & `cybotrade-0.1.1/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,23 @@
 
 [lib]
 name = "cybotrade"
 crate-type = ["cdylib"]
 
 [dependencies]
 datahub = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/datahub.git" }
-# bqapi = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bqapi.git" }
-bq-core = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bq.git" } # Should remove (add Environment export in market-collector)
+bq-exchanges = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bq.git" }
 market-collector = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bq.git" }
-# bqapi-management = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bqapi.git" }
+bqapi = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bqapi.git" }
+bqapi-management = { version = "0.1", git = "ssh://git@bitbucket.org/balaena-quant/bqapi.git" }
 
-pyo3 = { version = "0.18", features = ["extension-module"] }
+pyo3 = { version = "0.18", features = ["extension-module", "chrono"] }
 pyo3-log = "0.8"
 pyo3-asyncio = { version = "0.18", features = ["attributes", "tokio-runtime"] }
+tracing = "0.1"
 log = "0.4"
 tokio = "1.28"
-chrono = "0.4"
+chrono = "0.4"
+anyhow = "1.0"
+serde = "1.0"
+uuid = "1.3"
+serde_json = "1.0"
```

### Comparing `cybotrade-0.1.0/Dockerfile` & `cybotrade-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/bin/protoc` & `cybotrade-0.1.1/proto/bin/protoc`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/any.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/api.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/api.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/compiler/plugin.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/compiler/plugin.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/descriptor.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/duration.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/duration.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/empty.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/empty.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/field_mask.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/field_mask.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/source_context.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/source_context.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/struct.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/struct.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/timestamp.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/timestamp.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/type.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/include/google/protobuf/wrappers.proto` & `cybotrade-0.1.1/proto/include/google/protobuf/wrappers.proto`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/proto/readme.txt` & `cybotrade-0.1.1/proto/readme.txt`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/protoc-21.12-linux-x86_64.zip` & `cybotrade-0.1.1/protoc-21.12-linux-x86_64.zip`

 * *Files identical despite different names*

### Comparing `cybotrade-0.1.0/Cargo.lock` & `cybotrade-0.1.1/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -107,14 +107,25 @@
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
+name = "argon2"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db4ce4441f99dbd377ca8a8f57b698c44d0d6e712d8329b5040da5a64aa1ce73"
+dependencies = [
+ "base64ct",
+ "blake2",
+ "password-hash",
+]
+
+[[package]]
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "async-broadcast"
@@ -182,14 +193,300 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "aws-config"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56a636c44c77fa18bdba56126a34d30cfe5538fe88f7d34988fa731fee143ddd"
+dependencies = [
+ "aws-http",
+ "aws-sdk-sso",
+ "aws-sdk-sts",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-json",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "hex",
+ "http",
+ "hyper",
+ "ring",
+ "time 0.3.21",
+ "tokio",
+ "tower",
+ "tracing",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-endpoint"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ca8f374874f6459aaa88dc861d7f5d834ca1ff97668eae190e97266b5f6c3fb"
+dependencies = [
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "aws-types",
+ "http",
+ "regex",
+ "tracing",
+]
+
+[[package]]
+name = "aws-http"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "78d41e19e779b73463f5f0c21b3aacc995f4ba783ab13a7ae9f5dfb159a551b4"
+dependencies = [
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "http",
+ "http-body",
+ "lazy_static",
+ "percent-encoding",
+ "pin-project-lite",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sdk-secretsmanager"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b60a73c8e0afa05093c01bd979b48727ca59dc154173ea2c46af26d05a2f39a"
+dependencies = [
+ "aws-endpoint",
+ "aws-http",
+ "aws-sig-auth",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-json",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "fastrand",
+ "http",
+ "tokio-stream",
+ "tower",
+]
+
+[[package]]
+name = "aws-sdk-sso"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86dcb1cb71aa8763b327542ead410424515cff0cde5b753eedd2917e09c63734"
+dependencies = [
+ "aws-endpoint",
+ "aws-http",
+ "aws-sig-auth",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-json",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "http",
+ "tokio-stream",
+ "tower",
+]
+
+[[package]]
+name = "aws-sdk-sts"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fdfcf584297c666f6b472d5368a78de3bc714b6e0a53d7fbf76c3e347c292ab1"
+dependencies = [
+ "aws-endpoint",
+ "aws-http",
+ "aws-sig-auth",
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-query",
+ "aws-smithy-types",
+ "aws-smithy-xml",
+ "aws-types",
+ "bytes",
+ "http",
+ "tower",
+]
+
+[[package]]
+name = "aws-sig-auth"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12cbe7b2be9e185c1fbce27fc9c41c66b195b32d89aa099f98768d9544221308"
+dependencies = [
+ "aws-sigv4",
+ "aws-smithy-http",
+ "aws-types",
+ "http",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sigv4"
+version = "0.51.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c0b2658d2cb66dbf02f0e8dee80810ef1e0ca3530ede463e0ef994c301087d1"
+dependencies = [
+ "aws-smithy-http",
+ "form_urlencoded",
+ "hex",
+ "http",
+ "once_cell",
+ "percent-encoding",
+ "regex",
+ "ring",
+ "time 0.3.21",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-async"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b3442b4c5d3fc39891a2e5e625735fba6b24694887d49c6518460fde98247a9"
+dependencies = [
+ "futures-util",
+ "pin-project-lite",
+ "tokio",
+ "tokio-stream",
+]
+
+[[package]]
+name = "aws-smithy-client"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ff28d553714f8f54cd921227934fc13a536a1c03f106e56b362fd57e16d450ad"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-http-tower",
+ "aws-smithy-types",
+ "bytes",
+ "fastrand",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-rustls",
+ "lazy_static",
+ "pin-project-lite",
+ "tokio",
+ "tower",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-http"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf58ed4fefa61dbf038e5421a521cbc2c448ef69deff0ab1d915d8a10eda5664"
+dependencies = [
+ "aws-smithy-types",
+ "bytes",
+ "bytes-utils",
+ "futures-core",
+ "http",
+ "http-body",
+ "hyper",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "pin-utils",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-http-tower"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "20c96d7bd35e7cf96aca1134b2f81b1b59ffe493f7c6539c051791cbbf7a42d3"
+dependencies = [
+ "aws-smithy-http",
+ "bytes",
+ "http",
+ "http-body",
+ "pin-project-lite",
+ "tower",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-json"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d8324ba98c8a94187723cc16c37aefa09504646ee65c3d2c3af495bab5ea701b"
+dependencies = [
+ "aws-smithy-types",
+]
+
+[[package]]
+name = "aws-smithy-query"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83834ed2ff69ea6f6657baf205267dc2c0abe940703503a3e5d60ce23be3d306"
+dependencies = [
+ "aws-smithy-types",
+ "urlencoding",
+]
+
+[[package]]
+name = "aws-smithy-types"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b02e06ea63498c43bc0217ea4d16605d4e58d85c12fc23f6572ff6d0a840c61"
+dependencies = [
+ "itoa",
+ "num-integer",
+ "ryu",
+ "time 0.3.21",
+]
+
+[[package]]
+name = "aws-smithy-xml"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "246e9f83dd1fdf5d347fa30ae4ad30a9d1d42ce4cd74a93d94afa874646f94cd"
+dependencies = [
+ "xmlparser",
+]
+
+[[package]]
+name = "aws-types"
+version = "0.51.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05701d32da168b44f7ee63147781aed8723e792cc131cb9b18363b5393f17f70"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-client",
+ "aws-smithy-http",
+ "aws-smithy-types",
+ "http",
+ "rustc_version",
+ "tracing",
+ "zeroize",
+]
+
+[[package]]
 name = "axum"
 version = "0.6.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
 dependencies = [
  "async-trait",
  "axum-core",
@@ -203,15 +500,19 @@
  "matchit",
  "memchr",
  "mime",
  "percent-encoding",
  "pin-project-lite",
  "rustversion",
  "serde",
+ "serde_json",
+ "serde_path_to_error",
+ "serde_urlencoded",
  "sync_wrapper",
+ "tokio",
  "tower",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
 name = "axum-core"
@@ -227,26 +528,72 @@
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "axum-extra"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "febf23ab04509bd7672e6abe76bd8277af31b679e89fa5ffc6087dc289a448a3"
+dependencies = [
+ "axum",
+ "axum-core",
+ "bytes",
+ "futures-util",
+ "http",
+ "http-body",
+ "mime",
+ "pin-project-lite",
+ "serde",
+ "tokio",
+ "tower",
+ "tower-http",
+ "tower-layer",
+ "tower-service",
+]
+
+[[package]]
+name = "axum-macros"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2bb524613be645939e280b7279f7b017f98cf7f5ef084ec374df373530e73277"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ea22880d78093b0cbe17c89f64a7d457941e65759157ec6cb31a31d652b05e5"
+
+[[package]]
+name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
+name = "base64ct"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitvec"
@@ -257,14 +604,23 @@
  "funty",
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
+name = "blake2"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
+dependencies = [
+ "digest",
+]
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
@@ -283,15 +639,15 @@
 name = "borsh-derive"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0754613691538d51f329cce9af41d7b7ca150bc973056f1156611489475f54f7"
 dependencies = [
  "borsh-derive-internal",
  "borsh-schema-derive-internal",
- "proc-macro-crate",
+ "proc-macro-crate 0.1.5",
  "proc-macro2",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "borsh-derive-internal"
 version = "0.10.3"
@@ -313,15 +669,15 @@
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "bq-core"
 version = "0.1.11"
-source = "git+ssh://git@bitbucket.org/balaena-quant/bq.git#bcec49f8f8a166355b37a472ee7dd7415c5e7c60"
+source = "git+ssh://git@bitbucket.org/balaena-quant/bq.git#c63954dc95fb0b459faa4e73c0460784d177033d"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "bytes",
  "chrono",
  "coarsetime",
@@ -346,15 +702,15 @@
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "bq-exchanges"
 version = "0.1.20"
-source = "git+ssh://git@bitbucket.org/balaena-quant/bq.git#bcec49f8f8a166355b37a472ee7dd7415c5e7c60"
+source = "git+ssh://git@bitbucket.org/balaena-quant/bq.git#c63954dc95fb0b459faa4e73c0460784d177033d"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bq-core",
  "chrono",
  "function_name",
@@ -377,14 +733,104 @@
  "tracing",
  "tracing-subscriber",
  "url",
  "uuid",
 ]
 
 [[package]]
+name = "bqapi"
+version = "0.1.2"
+source = "git+ssh://git@bitbucket.org/balaena-quant/bqapi.git#f9b6513a690a6ddf7ce84523be31b109bb7b4986"
+dependencies = [
+ "base64 0.21.2",
+ "bqapi-llama",
+ "bqapi-management",
+ "tonic 0.9.2",
+]
+
+[[package]]
+name = "bqapi-llama"
+version = "0.1.0"
+source = "git+ssh://git@bitbucket.org/balaena-quant/bqapi.git#f9b6513a690a6ddf7ce84523be31b109bb7b4986"
+dependencies = [
+ "anyhow",
+ "axum",
+ "axum-extra",
+ "axum-macros",
+ "base64 0.21.2",
+ "bq-exchanges",
+ "bqapi-management",
+ "chrono",
+ "clap",
+ "dashmap",
+ "dotenvy",
+ "futures",
+ "hyper",
+ "lazy_static",
+ "prost",
+ "prost-wkt",
+ "prost-wkt-build",
+ "prost-wkt-types",
+ "regex",
+ "serde",
+ "serde_json",
+ "time 0.3.21",
+ "tokio",
+ "tonic 0.9.2",
+ "tonic-build 0.9.2",
+ "tonic-reflection 0.9.2",
+ "tower",
+ "tracing",
+ "tracing-appender",
+ "tracing-subscriber",
+]
+
+[[package]]
+name = "bqapi-management"
+version = "0.1.2"
+source = "git+ssh://git@bitbucket.org/balaena-quant/bqapi.git#f9b6513a690a6ddf7ce84523be31b109bb7b4986"
+dependencies = [
+ "anyhow",
+ "argon2",
+ "aws-config",
+ "aws-sdk-secretsmanager",
+ "base64 0.20.0",
+ "bq-core",
+ "chrono",
+ "clap",
+ "dotenv",
+ "futures",
+ "hyper",
+ "lazy_static",
+ "num_cpus",
+ "openssl",
+ "prost",
+ "prost-wkt",
+ "prost-wkt-build",
+ "prost-wkt-types",
+ "rand",
+ "rand_core",
+ "rdkafka",
+ "regex",
+ "serde",
+ "serde_json",
+ "sqlx",
+ "thiserror",
+ "tokio",
+ "tonic 0.9.2",
+ "tonic-build 0.9.2",
+ "tonic-reflection 0.9.2",
+ "tower",
+ "tracing",
+ "tracing-subscriber",
+ "uuid",
+ "validator",
+]
+
+[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytecheck"
@@ -417,14 +863,24 @@
 [[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
+name = "bytes-utils"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e47d3a8076e283f3acd27400535992edb3ba4b5bb72f8891ad8fbe7932a7d4b9"
+dependencies = [
+ "bytes",
+ "either",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
@@ -439,24 +895,24 @@
 checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
- "time",
+ "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.1"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4ed2379f8603fa2b7509891660e802b88c70a79a6427a70abb5968054de2c28"
+checksum = "401a4694d2bf92537b6867d94de48c4842089645fdcdf6c71865b175d836e9c2"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
@@ -465,36 +921,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
+ "once_cell",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.1"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59e9ef9a08ee1c0e1f2e162121665ac45ac3783b0f897db7244ae75ad9a8f65b"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
+name = "cmake"
+version = "0.1.50"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "coarsetime"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a90d114103adbc625300f346d4d09dfb4ab1c4a8df6868435dd903392ecf4354"
 dependencies = [
  "libc",
  "once_cell",
@@ -545,14 +1011,24 @@
 [[package]]
 name = "crc-catalog"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9cace84e55f07e7301bae1c519df89cdad8cc3cd868413d3fdbdeca9ff3db484"
 
 [[package]]
+name = "crossbeam-channel"
+version = "0.5.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-queue"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d1cfb3ea8a53f37c40dea2c7bedcbd88bdfae54f5e2175d6ecaff1c988353add"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
@@ -577,23 +1053,30 @@
  "typenum",
 ]
 
 [[package]]
 name = "cybotrade"
 version = "0.1.0"
 dependencies = [
- "bq-core",
+ "anyhow",
+ "bq-exchanges",
+ "bqapi",
+ "bqapi-management",
  "chrono",
  "datahub",
  "log",
  "market-collector",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
+ "serde",
+ "serde_json",
  "tokio",
+ "tracing",
+ "uuid",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
@@ -767,17 +1250,17 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "function_name"
 version = "0.3.0"
@@ -1046,14 +1529,20 @@
 dependencies = [
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "http-range-header"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0bfe8eed0a9285ef776bb792479ea3834e8b94e13d615c2f66d03dd50a435a29"
+
+[[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "httpdate"
@@ -1090,18 +1579,18 @@
 version = "0.23.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1788965e61b367cd03a62950836d5cd41560c3577d90e40e0819373194d1661c"
 dependencies = [
  "http",
  "hyper",
  "log",
- "rustls",
+ "rustls 0.20.8",
  "rustls-native-certs",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.23.4",
 ]
 
 [[package]]
 name = "hyper-timeout"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbb958482e8c7be4bc3cf272a766a2b0bf1a6755e7a6ae777f017a31d11b13b1"
@@ -1133,17 +1622,28 @@
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "418a0a6fab821475f634efe3ccc45c013f742efe03d853e8d3355d5cb850ecf8"
+dependencies = [
+ "matches",
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
+name = "idna"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
@@ -1231,17 +1731,29 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.145"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "fc86cde3ff845662b8f4ef6cb50ea0e20c524eb3d29ae048287e06a1b3fa6a81"
+
+[[package]]
+name = "libz-sys"
+version = "1.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+ "vcpkg",
+]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
@@ -1266,37 +1778,52 @@
 version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "market-collector"
 version = "0.1.9"
-source = "git+ssh://git@bitbucket.org/balaena-quant/bq.git#bcec49f8f8a166355b37a472ee7dd7415c5e7c60"
+source = "git+ssh://git@bitbucket.org/balaena-quant/bq.git#c63954dc95fb0b459faa4e73c0460784d177033d"
 dependencies = [
  "anyhow",
  "bq-exchanges",
  "clap",
  "dotenv",
  "flume",
  "futures",
  "prost",
  "prost-wkt",
  "prost-wkt-build",
  "prost-wkt-types",
  "serde",
  "serde_json",
  "tokio",
- "tonic",
- "tonic-build",
- "tonic-reflection",
+ "tonic 0.8.3",
+ "tonic-build 0.8.4",
+ "tonic-reflection 0.6.0",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
+name = "matchers"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
+dependencies = [
+ "regex-automata",
+]
+
+[[package]]
+name = "matches"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2532096657941c2fea9c289d370a250971c689d4f143798ff67113ec042024a5"
+
+[[package]]
 name = "matchit"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b87248edafb776e59e6ee64a79086f65890d3510f2c656c000bf2a7e8a0aea40"
 
 [[package]]
 name = "md-5"
@@ -1418,14 +1945,24 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -1437,18 +1974,39 @@
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
+name = "num_enum"
+version = "0.5.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f646caf906c20226733ed5b1374287eb97e3c2a5c227ce668c1f2ce20ae57c9"
+dependencies = [
+ "num_enum_derive",
+]
+
+[[package]]
+name = "num_enum_derive"
+version = "0.5.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dcbff9bc912032c62bf65ef1d5aea88983b420f4f839db1e9b0c281a25c9c799"
+dependencies = [
+ "proc-macro-crate 1.3.1",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "once_cell"
-version = "1.17.2"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "openssl"
 version = "0.10.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
 dependencies = [
@@ -1541,24 +2099,35 @@
  "libc",
  "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "password-hash"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7676374caaee8a325c9e7a2ae557f216c5563a171d6997b0ef8a65af35147700"
+dependencies = [
+ "base64ct",
+ "rand_core",
+ "subtle",
+]
+
+[[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
@@ -1626,14 +2195,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d6ea3c4595b96363c13943497db34af4460fb474a95c43f4446ad341b8c9785"
 dependencies = [
  "toml",
 ]
 
 [[package]]
+name = "proc-macro-crate"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
+dependencies = [
+ "once_cell",
+ "toml_edit",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
@@ -1761,14 +2340,15 @@
 [[package]]
 name = "pyo3"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
+ "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
@@ -1818,17 +2398,17 @@
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9c8b57fe71fb5dcf38970ebedc2b1531cf1c14b1b9b4c560a182a57e115575c"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
@@ -1907,14 +2487,45 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
+name = "rdkafka"
+version = "0.29.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd7c5d6d17442bcb9f943aae96d67d98c6d36af60442dd5da62aaa7fcbb25c48"
+dependencies = [
+ "futures-channel",
+ "futures-util",
+ "libc",
+ "log",
+ "rdkafka-sys",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "slab",
+ "tokio",
+]
+
+[[package]]
+name = "rdkafka-sys"
+version = "4.4.0+1.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87ac9d87c3aba1748e3112318459f2ac8bff80bfff7359e338e0463549590249"
+dependencies = [
+ "cmake",
+ "libc",
+ "libz-sys",
+ "num_enum",
+ "pkg-config",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
@@ -1937,25 +2548,40 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.2",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+dependencies = [
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-syntax"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rend"
 version = "0.4.0"
@@ -2033,14 +2659,23 @@
 checksum = "0e773fd3da1ed42472fdf3cfdb4972948a555bc3d73f5e0bdb99d17e7b54c687"
 dependencies = [
  "quote",
  "rust_decimal",
 ]
 
 [[package]]
+name = "rustc_version"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
+
+[[package]]
 name = "rustix"
 version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno",
@@ -2059,14 +2694,26 @@
  "log",
  "ring",
  "sct",
  "webpki",
 ]
 
 [[package]]
+name = "rustls"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-webpki",
+ "sct",
+]
+
+[[package]]
 name = "rustls-native-certs"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0167bac7a9f490495f3c33013e7722b53cb087ecbe082fb0c6387c96f634ea50"
 dependencies = [
  "openssl-probe",
  "rustls-pemfile",
@@ -2080,14 +2727,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
 dependencies = [
  "base64 0.21.2",
 ]
 
 [[package]]
+name = "rustls-webpki"
+version = "0.100.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "ryu"
@@ -2146,14 +2803,20 @@
 checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
+name = "semver"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+
+[[package]]
 name = "serde"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
@@ -2177,14 +2840,23 @@
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_path_to_error"
+version = "0.1.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7f05c1d5476066defcdfacce1f52fc3cae3af1d3089727100c02ae92e5abbe0"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
 dependencies = [
  "form_urlencoded",
  "itoa",
@@ -2343,14 +3015,15 @@
  "smallvec",
  "sqlformat",
  "sqlx-rt",
  "stringprep",
  "thiserror",
  "tokio-stream",
  "url",
+ "uuid",
  "whoami",
 ]
 
 [[package]]
 name = "sqlx-macros"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2515,14 +3188,41 @@
 dependencies = [
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
+name = "time"
+version = "0.3.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
+dependencies = [
+ "itoa",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
@@ -2602,20 +3302,30 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
 dependencies = [
- "rustls",
+ "rustls 0.20.8",
  "tokio",
  "webpki",
 ]
 
 [[package]]
+name = "tokio-rustls"
+version = "0.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e0d409377ff5b1e3ca6437aa86c1eb7d40c134bfec254e44c830defa92669db5"
+dependencies = [
+ "rustls 0.21.1",
+ "tokio",
+]
+
+[[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
@@ -2626,18 +3336,18 @@
 name = "tokio-tungstenite"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54319c93411147bced34cb5609a80e0a8e44c5999c93903a81cd866630ec0bfd"
 dependencies = [
  "futures-util",
  "log",
- "rustls",
+ "rustls 0.20.8",
  "rustls-native-certs",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.23.4",
  "tungstenite",
  "webpki",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.7.8"
@@ -2658,14 +3368,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "toml_datetime"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
+
+[[package]]
+name = "toml_edit"
+version = "0.19.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
+dependencies = [
+ "indexmap",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
 name = "tonic"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f219fad3b929bef19b1f86fbc0358d35daed8f2cac972037ac0dc10bbb8d5fb"
 dependencies = [
  "async-stream",
  "async-trait",
@@ -2690,38 +3417,95 @@
  "tower-layer",
  "tower-service",
  "tracing",
  "tracing-futures",
 ]
 
 [[package]]
+name = "tonic"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
+dependencies = [
+ "async-stream",
+ "async-trait",
+ "axum",
+ "base64 0.21.2",
+ "bytes",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-timeout",
+ "percent-encoding",
+ "pin-project",
+ "prost",
+ "rustls-pemfile",
+ "tokio",
+ "tokio-rustls 0.24.0",
+ "tokio-stream",
+ "tower",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
 name = "tonic-build"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bf5e9b9c0f7e0a7c027dcfaba7b2c60816c7049171f679d99ee2ff65d0de8c4"
 dependencies = [
  "prettyplease",
  "proc-macro2",
  "prost-build",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "tonic-build"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6fdaae4c2c638bb70fe42803a26fbd6fc6ac8c72f5c59f67ecc2a2dcabf4b07"
+dependencies = [
+ "prettyplease",
+ "proc-macro2",
+ "prost-build",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "tonic-reflection"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67494bad4dda4c9bffae901dfe14e2b2c0f760adb4706dc10beeb81799f7f7b2"
 dependencies = [
  "bytes",
  "prost",
  "prost-types",
  "tokio",
  "tokio-stream",
- "tonic",
+ "tonic 0.8.3",
+]
+
+[[package]]
+name = "tonic-reflection"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0543d7092032041fbeac1f2c84304537553421a11a623c2301b12ef0264862c7"
+dependencies = [
+ "prost",
+ "prost-types",
+ "tokio",
+ "tokio-stream",
+ "tonic 0.9.2",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -2737,14 +3521,32 @@
  "tokio-util",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
+name = "tower-http"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d1d42a9b3f3ec46ba828e8d376aec14592ea199f70a06a548587ecd1c4ab658"
+dependencies = [
+ "bitflags",
+ "bytes",
+ "futures-core",
+ "futures-util",
+ "http",
+ "http-body",
+ "http-range-header",
+ "pin-project-lite",
+ "tower-layer",
+ "tower-service",
+]
+
+[[package]]
 name = "tower-layer"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
 
 [[package]]
 name = "tower-service"
@@ -2755,20 +3557,32 @@
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
+name = "tracing-appender"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09d48f71a791638519505cefafe162606f706c25592e4bde4d97600c0195312e"
+dependencies = [
+ "crossbeam-channel",
+ "time 0.3.21",
+ "tracing-subscriber",
+]
+
+[[package]]
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -2818,20 +3632,25 @@
 
 [[package]]
 name = "tracing-subscriber"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
+ "matchers",
  "nu-ansi-term",
+ "once_cell",
+ "regex",
  "serde",
  "serde_json",
  "sharded-slab",
  "smallvec",
  "thread_local",
+ "time 0.3.21",
+ "tracing",
  "tracing-core",
  "tracing-log",
  "tracing-serde",
 ]
 
 [[package]]
 name = "try-lock"
@@ -2848,15 +3667,15 @@
  "base64 0.13.1",
  "byteorder",
  "bytes",
  "http",
  "httparse",
  "log",
  "rand",
- "rustls",
+ "rustls 0.20.8",
  "sha1",
  "thiserror",
  "url",
  "utf-8",
  "webpki",
 ]
 
@@ -2939,24 +3758,30 @@
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
- "idna",
+ "idna 0.4.0",
  "percent-encoding",
 ]
 
 [[package]]
+name = "urlencoding"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
+
+[[package]]
 name = "utf-8"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
 
 [[package]]
 name = "utf8parse"
@@ -2969,14 +3794,41 @@
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 dependencies = [
  "getrandom",
  "rand",
  "serde",
+ "uuid-macro-internal",
+]
+
+[[package]]
+name = "uuid-macro-internal"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f67b459f42af2e6e1ee213cb9da4dbd022d3320788c3fb3e1b893093f1e45da"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "validator"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32ad5bf234c7d3ad1042e5252b7eddb2c4669ee23f32c7dd0e9b7705f07ef591"
+dependencies = [
+ "idna 0.2.3",
+ "lazy_static",
+ "regex",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "url",
 ]
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
@@ -3285,14 +4137,35 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
+name = "winnow"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
+
+[[package]]
+name = "xmlparser"
+version = "0.13.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
+
+[[package]]
+name = "zeroize"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

