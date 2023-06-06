# Comparing `tmp/torch_exid-0.1.4.tar.gz` & `tmp/torch_exid-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_exid-0.1.4.tar", max compression
+gzip compressed data, was "torch_exid-0.1.5.tar", max compression
```

## Comparing `torch_exid-0.1.4.tar` & `torch_exid-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:57:48.668360 torch_exid-0.1.4/LICENSE
--rw-r--r--   0        0        0     3500 2023-05-30 12:08:05.911047 torch_exid-0.1.4/README.md
--rw-r--r--   0        0        0      562 2023-06-04 14:53:35.947847 torch_exid-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-04 14:52:11.381620 torch_exid-0.1.4/src/torch_exid/__init__.py
--rw-r--r--   0        0        0     6176 2023-06-04 14:49:57.051163 torch_exid-0.1.4/src/torch_exid/exid.py
--rw-r--r--   0        0        0     4432 2023-06-04 14:54:02.712331 torch_exid-0.1.4/setup.py
--rw-r--r--   0        0        0     4107 2023-06-04 14:54:02.712498 torch_exid-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:57:48.668360 torch_exid-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4131 2023-06-06 20:14:36.443368 torch_exid-0.1.5/README.md
+-rw-r--r--   0        0        0      562 2023-06-06 19:28:20.715656 torch_exid-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-06 20:04:59.962615 torch_exid-0.1.5/src/torch_exid/__init__.py
+-rw-r--r--   0        0        0     6490 2023-06-06 20:06:28.167125 torch_exid-0.1.5/src/torch_exid/exid.py
+-rw-r--r--   0        0        0     5087 2023-06-06 20:15:28.517129 torch_exid-0.1.5/setup.py
+-rw-r--r--   0        0        0     4738 2023-06-06 20:15:28.517314 torch_exid-0.1.5/PKG-INFO
```

### Comparing `torch_exid-0.1.4/LICENSE` & `torch_exid-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_exid-0.1.4/README.md` & `torch_exid-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -90,14 +90,38 @@
 # Will print out "1, 4, 9"
 for n in ds:
     print(n)
 ```
 
 In addition to the above, any arguments or keyword arguments for the [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) superclass can also be passed.
 
+## Methods
+
+### skip_next: Callable[[None], None]
+This method allows the skipping of the next item that would be yielded by the `generator`. Using `skip_next` will not affect the `limit` or `offset`.
+```python
+class EvensDataset(ExtendedIterableDataset):
+    def generator(self) -> Iterator[int]:
+        n = 0
+        while True:
+            if n % 2 != 0:
+                self.skip_next()
+
+            yield n
+            n += 1
+
+ds = EvensDataset(limit=5)
+
+# Will print out "0, 2, 4, 6, 8"
+for n in ds:
+    print(n)
+```
+
+In other words, it allows you to bypass the next item without modifying the overall iteration parameters.
+
 ## Contributing
 Contributions are greatly appreciated! Improvement can be made by submitting issues, proposing new features, or submitting pull requests with bug fixes or new functionalities.
 
 ### Getting started with contributing
 Here are the steps to get started with development:
 ```bash
 # Clone the repository:
```

### Comparing `torch_exid-0.1.4/pyproject.toml` & `torch_exid-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch_exid"
-version = "0.1.4"
+version = "0.1.5"
 description = "An extension of PyTorch IterableDataset, this package introduces functionalities for shuffling, limiting, and offsetting data."
 authors = ["Artem Legotin <hello@artemlegotin.com>"]
 readme = "README.md"
 homepage = "https://github.com/arlegotin/torch_exid"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `torch_exid-0.1.4/src/torch_exid/exid.py` & `torch_exid-0.1.5/src/torch_exid/exid.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,25 +49,32 @@
         that data should be extracted from this instance.
         """
         if transforms_required and not transforms:
             raise ValueError(
                 f"ExtendedIterableDataset requires transforms in order to avoid bugs. Please read the comment above"
             )
 
-        self.shuffle_buffer = shuffle_buffer
-        self.shuffle_seed = (
+        self.shuffle_buffer: int = shuffle_buffer
+        self.shuffle_seed: int = (
             shuffle_seed if shuffle_seed is not None else Random().randint(0, 999331)
         )
-        self.buffer = []
+        self.buffer: List[Any] = []
 
-        self.offset = offset
-        self.limit = limit
-        self.counter = 0
+        self.offset: int = offset
+        self.limit: int = limit
+        self.counter: int = 0
+
+        self._skip_next: bool = False
+
+        self.transforms: List[Callable[[Any], Any]] = (
+            transforms if transforms is not None else []
+        )
 
-        self.transforms = transforms if transforms is not None else []
+    def skip_next(self):
+        self._skip_next = True
 
     def generator(self) -> Iterator[Any]:
         """
         Should yield items. This method should be implemented in subclasses.
 
         Raises
         ------
@@ -148,23 +155,27 @@
 
         while True:
             try:
                 if not self.limit_allows_one_more:
                     raise StopIteration
 
                 x = next(gen)
+                x = self.transform_x(x)
 
-                if self.counter < self.offset:
-                    self.counter += 1
+                if self._skip_next:
+                    self._skip_next = False
                     continue
 
-                yield self.transform_x(x)
-
                 self.counter += 1
 
+                if self.counter - 1 < self.offset:
+                    continue
+
+                yield x
+
             except StopIteration:
                 break
 
     def generator_with_buffer(self) -> Iterator[Any]:
         """
         Generates items with a shuffle buffer.
         If the buffer size is greater than 1, items are buffered and shuffled before being yielded.
@@ -189,14 +200,15 @@
         else:
             for x in self.generator_with_conditions():
                 yield x
 
         # Reset the counter and the buffer
         self.counter = 0
         self.buffer = []
+        self._skip_next = False
 
     def __iter__(self) -> Iterator[Any]:
         """
         Generates items with a shuffle buffer.
         If the buffer size is greater than 1, items are buffered and shuffled before being yielded.
         If the buffer size is 1 or less, items are yielded as they are generated.
```

### Comparing `torch_exid-0.1.4/setup.py` & `torch_exid-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'torch-exid',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'An extension of PyTorch IterableDataset, this package introduces functionalities for shuffling, limiting, and offsetting data.',
-    'long_description': '# Extended Iterable Dataset for PyTorch\nAn extension of PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset), this package introduces functionalities for shuffling, limiting, and offsetting data.\n\n## Installation\n\nDirectly from [PyPI](https://pypi.org/project/torch_exid/):\n```bash\npip install torch-exid\n```\n\nOr using [Poetry](https://python-poetry.org/):\n```bash\npoetry add torch-exid\n```\n\n## Usage\nBegin by subclassing `ExtendedIterableDataset` and implement the `generator` method to yield items.\n\nHere\'s a simple example using an `IntegersDataset`:\n```python\nfrom torch_exid import ExtendedIterableDataset\n\nclass IntegersDataset(ExtendedIterableDataset):\n    def generator(self) -> Iterator[int]:\n        n = 0\n        while True:\n            yield n\n            n += 1\n\n# Will print out integers 0, 1, ..., 9:\nfor n in IntegersDataset(limit=10):\n    print(n)\n```\n\n## Constructor Parameters\n`ExtendedIterableDataset` introduces several parameters to provide additional control:\n\n### limit: int\nSets the maximum number of data points to return. If negative, all data points are returned. Default is `-1` (return all data).\n```python\n# Will print out "0, 1, 2"\nfor n in IntegersDataset(limit=3)\n    print(n)\n```\n\n### offset: int\nDetermines the number of initial data points to skip. Default is `0`.\n```python\n# Will print out "2, 3, 4"\nfor n in IntegersDataset(limit=3, offset=2)\n    print(n)\n```\n\n### shuffle_buffer: int\nThis specifies the buffer size for shuffling. If greater than `1`, data is buffered and shuffled prior to being returned. If set to `1` (default), no shuffling occurs.\n\n```python\n# Will print out "0, 1, 3, 2" for the first time...\nfor n in IntegersDataset(limit=4, shuffle_buffer=2)\n    print(n)\n\n# ...and 1, 0, 2, 3 second time\nfor n in IntegersDataset(limit=4, shuffle_buffer=2)\n    print(n)\n```\n\n### shuffle_seed: int\nDefines the seed for the random number generator used in shuffling. If not provided, a random seed is used:\n\n```python\n# Will print out "1, 0, 3, 2" both times:\nfor n in IntegersDataset(limit=4, shuffle_buffer=2, shuffle_seed=42)\n    print(n)\n\nfor n in IntegersDataset(limit=4, shuffle_buffer=2, shuffle_seed=42)\n    print(n)\n```\n\n### transforms: List[Callable[[Any], Any]]\nA list of transformations to apply to the data. Default is an empty list.\n```python\nds = IntegersDataset(\n    limit=3,\n    transforms=[\n        lambda n: n + 1,\n        lambda n: n ** 2,\n    ],\n)\n\n# Will print out "1, 4, 9"\nfor n in ds:\n    print(n)\n```\n\nIn addition to the above, any arguments or keyword arguments for the [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) superclass can also be passed.\n\n## Contributing\nContributions are greatly appreciated! Improvement can be made by submitting issues, proposing new features, or submitting pull requests with bug fixes or new functionalities.\n\n### Getting started with contributing\nHere are the steps to get started with development:\n```bash\n# Clone the repository:\ngit clone https://github.com/arlegotin/torch_exid.git\ncd torch_exid\n\n# Install the project and its dependencies using Poetry:\npoetry install\n\n# Spawn a shell within the virtual environment:\npoetry shell\n\n# Run tests to ensure everything is working correctly:\npytest tests/\n```\n\nPlease ensure all changes are accompanied by relevant unit tests, and that all tests pass before submitting a pull request. This helps maintain the quality and reliability of the project.\n',
+    'long_description': '# Extended Iterable Dataset for PyTorch\nAn extension of PyTorch [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset), this package introduces functionalities for shuffling, limiting, and offsetting data.\n\n## Installation\n\nDirectly from [PyPI](https://pypi.org/project/torch_exid/):\n```bash\npip install torch-exid\n```\n\nOr using [Poetry](https://python-poetry.org/):\n```bash\npoetry add torch-exid\n```\n\n## Usage\nBegin by subclassing `ExtendedIterableDataset` and implement the `generator` method to yield items.\n\nHere\'s a simple example using an `IntegersDataset`:\n```python\nfrom torch_exid import ExtendedIterableDataset\n\nclass IntegersDataset(ExtendedIterableDataset):\n    def generator(self) -> Iterator[int]:\n        n = 0\n        while True:\n            yield n\n            n += 1\n\n# Will print out integers 0, 1, ..., 9:\nfor n in IntegersDataset(limit=10):\n    print(n)\n```\n\n## Constructor Parameters\n`ExtendedIterableDataset` introduces several parameters to provide additional control:\n\n### limit: int\nSets the maximum number of data points to return. If negative, all data points are returned. Default is `-1` (return all data).\n```python\n# Will print out "0, 1, 2"\nfor n in IntegersDataset(limit=3)\n    print(n)\n```\n\n### offset: int\nDetermines the number of initial data points to skip. Default is `0`.\n```python\n# Will print out "2, 3, 4"\nfor n in IntegersDataset(limit=3, offset=2)\n    print(n)\n```\n\n### shuffle_buffer: int\nThis specifies the buffer size for shuffling. If greater than `1`, data is buffered and shuffled prior to being returned. If set to `1` (default), no shuffling occurs.\n\n```python\n# Will print out "0, 1, 3, 2" for the first time...\nfor n in IntegersDataset(limit=4, shuffle_buffer=2)\n    print(n)\n\n# ...and 1, 0, 2, 3 second time\nfor n in IntegersDataset(limit=4, shuffle_buffer=2)\n    print(n)\n```\n\n### shuffle_seed: int\nDefines the seed for the random number generator used in shuffling. If not provided, a random seed is used:\n\n```python\n# Will print out "1, 0, 3, 2" both times:\nfor n in IntegersDataset(limit=4, shuffle_buffer=2, shuffle_seed=42)\n    print(n)\n\nfor n in IntegersDataset(limit=4, shuffle_buffer=2, shuffle_seed=42)\n    print(n)\n```\n\n### transforms: List[Callable[[Any], Any]]\nA list of transformations to apply to the data. Default is an empty list.\n```python\nds = IntegersDataset(\n    limit=3,\n    transforms=[\n        lambda n: n + 1,\n        lambda n: n ** 2,\n    ],\n)\n\n# Will print out "1, 4, 9"\nfor n in ds:\n    print(n)\n```\n\nIn addition to the above, any arguments or keyword arguments for the [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) superclass can also be passed.\n\n## Methods\n\n### skip_next: Callable[[None], None]\nThis method allows the skipping of the next item that would be yielded by the `generator`. Using `skip_next` will not affect the `limit` or `offset`.\n```python\nclass EvensDataset(ExtendedIterableDataset):\n    def generator(self) -> Iterator[int]:\n        n = 0\n        while True:\n            if n % 2 != 0:\n                self.skip_next()\n\n            yield n\n            n += 1\n\nds = EvensDataset(limit=5)\n\n# Will print out "0, 2, 4, 6, 8"\nfor n in ds:\n    print(n)\n```\n\nIn other words, it allows you to bypass the next item without modifying the overall iteration parameters.\n\n## Contributing\nContributions are greatly appreciated! Improvement can be made by submitting issues, proposing new features, or submitting pull requests with bug fixes or new functionalities.\n\n### Getting started with contributing\nHere are the steps to get started with development:\n```bash\n# Clone the repository:\ngit clone https://github.com/arlegotin/torch_exid.git\ncd torch_exid\n\n# Install the project and its dependencies using Poetry:\npoetry install\n\n# Spawn a shell within the virtual environment:\npoetry shell\n\n# Run tests to ensure everything is working correctly:\npytest tests/\n```\n\nPlease ensure all changes are accompanied by relevant unit tests, and that all tests pass before submitting a pull request. This helps maintain the quality and reliability of the project.\n',
     'author': 'Artem Legotin',
     'author_email': 'hello@artemlegotin.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/arlegotin/torch_exid',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `torch_exid-0.1.4/PKG-INFO` & `torch_exid-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-exid
-Version: 0.1.4
+Version: 0.1.5
 Summary: An extension of PyTorch IterableDataset, this package introduces functionalities for shuffling, limiting, and offsetting data.
 Home-page: https://github.com/arlegotin/torch_exid
 Author: Artem Legotin
 Author-email: hello@artemlegotin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -105,14 +105,38 @@
 # Will print out "1, 4, 9"
 for n in ds:
     print(n)
 ```
 
 In addition to the above, any arguments or keyword arguments for the [IterableDataset](https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset) superclass can also be passed.
 
+## Methods
+
+### skip_next: Callable[[None], None]
+This method allows the skipping of the next item that would be yielded by the `generator`. Using `skip_next` will not affect the `limit` or `offset`.
+```python
+class EvensDataset(ExtendedIterableDataset):
+    def generator(self) -> Iterator[int]:
+        n = 0
+        while True:
+            if n % 2 != 0:
+                self.skip_next()
+
+            yield n
+            n += 1
+
+ds = EvensDataset(limit=5)
+
+# Will print out "0, 2, 4, 6, 8"
+for n in ds:
+    print(n)
+```
+
+In other words, it allows you to bypass the next item without modifying the overall iteration parameters.
+
 ## Contributing
 Contributions are greatly appreciated! Improvement can be made by submitting issues, proposing new features, or submitting pull requests with bug fixes or new functionalities.
 
 ### Getting started with contributing
 Here are the steps to get started with development:
 ```bash
 # Clone the repository:
```

