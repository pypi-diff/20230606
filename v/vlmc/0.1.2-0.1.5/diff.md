# Comparing `tmp/vlmc-0.1.2.tar.gz` & `tmp/vlmc-0.1.5.tar.gz`

## Comparing `vlmc-0.1.2.tar` & `vlmc-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 vlmc-0.1.2/Cargo.toml
--rw-r--r--   0      501       20       43 2023-06-06 13:43:19.000000 vlmc-0.1.2/.gitignore
--rw-r--r--   0      501       20       68 2023-06-06 15:00:46.000000 vlmc-0.1.2/CHANGELOG.md
--rw-r--r--   0      501       20     3369 2023-06-06 13:43:19.000000 vlmc-0.1.2/README.md
--rw-r--r--   0      501       20      570 2023-06-06 14:59:14.000000 vlmc-0.1.2/pyproject.toml
--rw-r--r--   0      501       20     5537 2023-06-06 13:43:19.000000 vlmc-0.1.2/src/lib.rs
--rw-r--r--   0      501       20     3439 2023-06-06 13:43:19.000000 vlmc-0.1.2/src/peres_shield.rs
--rw-r--r--   0      501       20     9705 2023-06-06 15:00:54.000000 vlmc-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 vlmc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 vlmc-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      123     2676 2023-06-06 17:44:45.000000 vlmc-0.1.5/.github/workflows/build_release.yml
+-rw-r--r--   0     1001      123       43 2023-06-06 17:44:45.000000 vlmc-0.1.5/.gitignore
+-rw-r--r--   0     1001      123     3951 2023-06-06 17:44:45.000000 vlmc-0.1.5/README.md
+-rw-r--r--   0     1001      123       10 2023-06-06 17:46:47.000000 vlmc-0.1.5/dist/vlmc-0.1.5.tar.gz
+-rw-r--r--   0     1001      123      571 2023-06-06 17:44:45.000000 vlmc-0.1.5/pyproject.toml
+-rw-r--r--   0     1001      123     5537 2023-06-06 17:44:45.000000 vlmc-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      123     3439 2023-06-06 17:44:45.000000 vlmc-0.1.5/src/peres_shield.rs
+-rw-r--r--   0     1001      123     9705 2023-06-06 17:44:45.000000 vlmc-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 vlmc-0.1.5/PKG-INFO
```

### Comparing `vlmc-0.1.2/README.md` & `vlmc-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,53 @@
 # Variable Length Markov Model (VLMC)
 Implementation of Variable Length Markov Chains (VLMC) for Python.
 Suffix tree building is done top-down using the ![Peres-Shield](https://link.springer.com/chapter/10.1007/11557067_24) order estimation method.
 It is written in Rust and ported to Python with PyO3.
 
-# Instalation
-You can install using `pip`.
+## Installation
 
-```shell
+### Installation with pip 
+
+Pre-built packages for many Linux, Windows, and OSX systems are available
+in [PyPI](https://pypi.org/project/vlmc/) and can be installed with:
+
+```sh
 pip install vlmc
 ```
+On uncommon architectures, you may need to first
+[install Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html)
+(i.e., the Rust programming language) first, and a subsequent
+`pip install vlmc` will try to compile the package for your CPU architecture and operating system.
+
+### Compilation from source
+
+You need to [install Rust/Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html).
+
+Installation uses [maturin](https://github.com/PyO3/maturin#maturin) for compiling and installing the Rust extension.
+Maturin is best used within a Python virtual environment:
+
+```sh
+# activate your desired virtual environment first, then:
+pip install maturin
+git clone https://github.com/antonio-leitao/vlmc.git
+cd vlmc
+# build and install the package:
+maturin develop --release
+```
 
 # Basic Usage
 
 ```python
 import vlmc
 tree = vlmc.VLMC(max_depth, alphabet_size, n_jobs=-1)
 ```
 Parameters:
--`max_depth`: Maximum depth of tree. Subsequences whose length exceed the `max_depth` will not be considered nor counted. 
--`alphabet_size`: Total number of symbols in the alphabet. This number has to be bigger than the highest integer encountered, else it will cause runtime errors. 
--`n_jobs`: Number of subprocesses to spawn when running the vlmc. Choose `-1` for using all available processes.  
+- `max_depth`: Maximum depth of tree. Subsequences whose length exceed the `max_depth` will not be considered nor counted. 
+- `alphabet_size`: Total number of symbols in the alphabet. This number has to be bigger than the highest integer encountered, else it will cause runtime errors. 
+- `n_jobs`: Number of subprocesses to spawn when running the vlmc. Choose `-1` for using all available processes.  
 
 # Methods
 
 ### `fit`
 
 ```python
 data = [
@@ -35,75 +59,58 @@
 
 tree.fit(data)
 ```
 > **Note**
 > fit method returns `None` and not `self`. This is by design as to not expose the rust object to python.
 
 Parameters:
--`data`: List of lists containing sequences of discrete values to fit on. Values are assumed to be integers form `0` to `alphabet_size`. List is expected to be two dimensional.
+- `data`: List of lists containing sequences of discrete values to fit on. Values are assumed to be integers form `0` to `alphabet_size`. List is expected to be two dimensional.
 
 ### `get_suffix`
 Given a sequence, returns the longest suffix that is present in the VLMC.
 
 ```python
 suffix = tree.get_suffix(sequence)
 ```
 Arguments:
--`sequence`: list of integers representing a sequence of discrete varaibles. 
+- `sequence`: list of integers representing a sequence of discrete varaibles. 
 Returns:
 - `suffix` : longest suffix of sequence that is present in the VLMC. 
 
 ### `get_counts`
 Gets the total number of occurences of a given sequence of integers.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 counts = tree.get_counts(sequence)
 ```
 Arguments:
--`sequence`: list of integers representing a sequence of discrete varaibles. 
+- `sequence`: list of integers representing a sequence of discrete varaibles. 
 Returns:
 - `counts` : integer 
 
 ### `get_distribution`
 Gets the vector of probabilities over the entire alphabet for the given sequence.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 probabilities = tree.get_distribution(sequence)
 ```
 Arguments:
--`sequence`: list of integers representing a sequence of discrete variables. 
+- `sequence`: list of integers representing a sequence of discrete variables. 
 Returns:
 - `probabilities` : list of floats representing the probability of observing a specific state (index) as the next symbol.
 
 ### `get_contexts`
 
 ```python
 contexts = tree.get_contexts()
 ```
 Returns:
--`contexts`: list of relevant contexts according to the Peres-Shield tree prunning method. Contexts are ordered by length.
-
-
-## Parameters
-
-### `contexts`
-```python
-contexts = tree.contexts
-```
-Returns:
-- `contexts` : list of sequences of each node in the tree, each relevant context.
-### `adjacency_matrix`
-```python
-matrix, labels = tree.adjacency_matrix
-```
-Returns:
-- `matrix` : adjacency matrix representing the suffix tree.
-- `labels` : list of sequences associated with each node of the tree.
+- `contexts`: list of relevant contexts according to the Peres-Shield tree prunning method. Contexts are ordered by length.
 
 # TODO
 ### Paralelization
 After experimentation the best possible idea for paralelization would be to create different hashmaps for each sunsequence length.
 Hashmaps are then joined from longest to smallest.
 The hashmap at `max_depth + 1` can be discarded after.
 Could be very fast depending on merging algo.
```

### Comparing `vlmc-0.1.2/pyproject.toml` & `vlmc-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+[build-system]
+requires = ["maturin>=0.14,<0.15"]
+build-backend = "maturin"
+
+[tool.maturin]
+# "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
+features = ["pyo3/extension-module"]
+
 [project]
 name = "vlmc"
-version = "0.1.2"
+version = "0.1.5"
 authors = [
   { name="António Leitão", email="aleitao@novaims.unl.pt" },
 ]
 description = "Variable Length Markov Chain"
 readme = "README.md"
 requires-python = ">=3.10"
 
 [project.urls]
 homepage = "https://github.com/antonio-leitao/vlmc"
 repository = "https://github.com/antonio-leitao/vlmc"
 
-[build-system]
-requires = ["maturin>=0.14,<0.15"]
-build-backend = "maturin"
-
-[tool.maturin]
-# "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
-features = ["pyo3/extension-module"]
```

### Comparing `vlmc-0.1.2/src/lib.rs` & `vlmc-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `vlmc-0.1.2/src/peres_shield.rs` & `vlmc-0.1.5/src/peres_shield.rs`

 * *Files identical despite different names*

### Comparing `vlmc-0.1.2/Cargo.lock` & `vlmc-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "vlmc"
-version = "0.1.2"
+version = "0.1.5"
 dependencies = [
  "hashbrown",
  "pyo3",
  "rand",
 ]
 
 [[package]]
```

### Comparing `vlmc-0.1.2/PKG-INFO` & `vlmc-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,63 @@
 Metadata-Version: 2.1
 Name: vlmc
-Version: 0.1.2
+Version: 0.1.5
 Summary: Variable Length Markov Chain
 Author-email: António Leitão <aleitao@novaims.unl.pt>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/antonio-leitao/vlmc
 Project-URL: repository, https://github.com/antonio-leitao/vlmc
 
 # Variable Length Markov Model (VLMC)
 Implementation of Variable Length Markov Chains (VLMC) for Python.
 Suffix tree building is done top-down using the ![Peres-Shield](https://link.springer.com/chapter/10.1007/11557067_24) order estimation method.
 It is written in Rust and ported to Python with PyO3.
 
-# Instalation
-You can install using `pip`.
+## Installation
 
-```shell
+### Installation with pip 
+
+Pre-built packages for many Linux, Windows, and OSX systems are available
+in [PyPI](https://pypi.org/project/vlmc/) and can be installed with:
+
+```sh
 pip install vlmc
 ```
+On uncommon architectures, you may need to first
+[install Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html)
+(i.e., the Rust programming language) first, and a subsequent
+`pip install vlmc` will try to compile the package for your CPU architecture and operating system.
+
+### Compilation from source
+
+You need to [install Rust/Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html).
+
+Installation uses [maturin](https://github.com/PyO3/maturin#maturin) for compiling and installing the Rust extension.
+Maturin is best used within a Python virtual environment:
+
+```sh
+# activate your desired virtual environment first, then:
+pip install maturin
+git clone https://github.com/antonio-leitao/vlmc.git
+cd vlmc
+# build and install the package:
+maturin develop --release
+```
 
 # Basic Usage
 
 ```python
 import vlmc
 tree = vlmc.VLMC(max_depth, alphabet_size, n_jobs=-1)
 ```
 Parameters:
--`max_depth`: Maximum depth of tree. Subsequences whose length exceed the `max_depth` will not be considered nor counted. 
--`alphabet_size`: Total number of symbols in the alphabet. This number has to be bigger than the highest integer encountered, else it will cause runtime errors. 
--`n_jobs`: Number of subprocesses to spawn when running the vlmc. Choose `-1` for using all available processes.  
+- `max_depth`: Maximum depth of tree. Subsequences whose length exceed the `max_depth` will not be considered nor counted. 
+- `alphabet_size`: Total number of symbols in the alphabet. This number has to be bigger than the highest integer encountered, else it will cause runtime errors. 
+- `n_jobs`: Number of subprocesses to spawn when running the vlmc. Choose `-1` for using all available processes.  
 
 # Methods
 
 ### `fit`
 
 ```python
 data = [
@@ -45,75 +69,58 @@
 
 tree.fit(data)
 ```
 > **Note**
 > fit method returns `None` and not `self`. This is by design as to not expose the rust object to python.
 
 Parameters:
--`data`: List of lists containing sequences of discrete values to fit on. Values are assumed to be integers form `0` to `alphabet_size`. List is expected to be two dimensional.
+- `data`: List of lists containing sequences of discrete values to fit on. Values are assumed to be integers form `0` to `alphabet_size`. List is expected to be two dimensional.
 
 ### `get_suffix`
 Given a sequence, returns the longest suffix that is present in the VLMC.
 
 ```python
 suffix = tree.get_suffix(sequence)
 ```
 Arguments:
--`sequence`: list of integers representing a sequence of discrete varaibles. 
+- `sequence`: list of integers representing a sequence of discrete varaibles. 
 Returns:
 - `suffix` : longest suffix of sequence that is present in the VLMC. 
 
 ### `get_counts`
 Gets the total number of occurences of a given sequence of integers.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 counts = tree.get_counts(sequence)
 ```
 Arguments:
--`sequence`: list of integers representing a sequence of discrete varaibles. 
+- `sequence`: list of integers representing a sequence of discrete varaibles. 
 Returns:
 - `counts` : integer 
 
 ### `get_distribution`
 Gets the vector of probabilities over the entire alphabet for the given sequence.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 probabilities = tree.get_distribution(sequence)
 ```
 Arguments:
--`sequence`: list of integers representing a sequence of discrete variables. 
+- `sequence`: list of integers representing a sequence of discrete variables. 
 Returns:
 - `probabilities` : list of floats representing the probability of observing a specific state (index) as the next symbol.
 
 ### `get_contexts`
 
 ```python
 contexts = tree.get_contexts()
 ```
 Returns:
--`contexts`: list of relevant contexts according to the Peres-Shield tree prunning method. Contexts are ordered by length.
-
-
-## Parameters
-
-### `contexts`
-```python
-contexts = tree.contexts
-```
-Returns:
-- `contexts` : list of sequences of each node in the tree, each relevant context.
-### `adjacency_matrix`
-```python
-matrix, labels = tree.adjacency_matrix
-```
-Returns:
-- `matrix` : adjacency matrix representing the suffix tree.
-- `labels` : list of sequences associated with each node of the tree.
+- `contexts`: list of relevant contexts according to the Peres-Shield tree prunning method. Contexts are ordered by length.
 
 # TODO
 ### Paralelization
 After experimentation the best possible idea for paralelization would be to create different hashmaps for each sunsequence length.
 Hashmaps are then joined from longest to smallest.
 The hashmap at `max_depth + 1` can be discarded after.
 Could be very fast depending on merging algo.
```

