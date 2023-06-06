# Comparing `tmp/pytest-embedded-idf-1.3.0.tar.gz` & `tmp/pytest-embedded-idf-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-idf-1.3.0.tar", last modified: Wed May 31 13:09:03 2023, max compression
+gzip compressed data, was "pytest-embedded-idf-1.3.1.tar", last modified: Tue Jun  6 08:56:25 2023, max compression
```

## Comparing `pytest-embedded-idf-1.3.0.tar` & `pytest-embedded-idf-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/unity_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/setup.py
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1544 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/PKG-INFO
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      520 2023-06-06 08:04:34.000000 pytest-embedded-idf-1.3.1/README.md
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:25.722213 pytest-embedded-idf-1.3.1/pytest_embedded_idf/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      598 2023-05-31 13:02:58.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/__init__.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     8830 2023-06-02 06:32:41.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/app.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)    11005 2023-06-06 08:04:34.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/dut.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1055 2023-06-02 06:32:41.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/linux.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     9584 2023-06-02 06:32:41.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/serial.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)    25144 2023-06-06 08:04:34.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf/unity_tester.py
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1544 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/PKG-INFO
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      413 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/SOURCES.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)        1 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/dependency_links.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       85 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/requires.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       20 2023-06-06 08:56:25.000000 pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/top_level.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       38 2023-06-06 08:56:25.725546 pytest-embedded-idf-1.3.1/setup.cfg
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1911 2023-06-06 08:49:39.000000 pytest-embedded-idf-1.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-embedded-idf-1.3.0/PKG-INFO` & `pytest-embedded-idf-1.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for esp-idf project
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
-Description: ### pytest-embedded-idf
-        
-        pytest embedded service for esp-idf project
-        
-        Extra Functionalities:
-        
-        === "`pytest-embedded-serial-esp` activated"
-        
-            - `app`: parse the built binary by idf rules and gather more information.
-            - `serial`: auto flash the built binary into the target board at the beginning when running test cases.
-        
-        === "`pytest-embedded-serial-esp` NOT activated"
-        
-            - `app`: parse the built binary by idf rules and gather more information.
-        
-        Used CLI Options:
-        
-        - `part-tool`
-        
-Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: serial
+
+### pytest-embedded-idf
+
+pytest embedded service for esp-idf project
+
+Extra Functionalities:
+
+```{eval-rst}
+.. tabs::
+
+   .. group-tab:: `pytest-embedded-serial-esp` activated
+
+        - `app`: parse the built binary by idf rules and gather more information.
+        - `serial`: auto flash the built binary into the target board at the beginning when running test cases.
+
+   .. group-tab:: `pytest-embedded-serial-esp` NOT activated
+
+        - `app`: parse the built binary by idf rules and gather more information.
+```
```

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf/__init__.py` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf/app.py` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf/dut.py` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf/dut.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         """
         Handle errors by panic_handler_script or check core dumps via UART or partition table.
         Write the decoded or read core dumps into separated files.
 
         For UART and panic output, would read the `_pexpect_logfile` file.
         For partition, would read the flash according to the partition table. needs a valid `parttool_path`.
 
-        Notes:
+        Note:
             - May include multiple core dumps, since each test case may include several unity test cases.
             - May have duplicated core dumps, since after the core dump happened, the target chip would reboot
             automatically.
 
         Returns:
             None
         """
```

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf/linux.py` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf/linux.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf/serial.py` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf/serial.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf/unity_tester.py` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf/unity_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,32 +34,29 @@
 ]
 
 
 @dataclass
 class UnittestMenuCase:
     """
     Dataclass of esp-idf unit test cases parsed from test menu
-
-    Attributes:
-        index: The index of the case, which can be used to run this case.
-        name: The name of the case.
-        type: Type of this case, which can be `normal` `multi_stage` or `multi_device`.
-        keywords: List of additional keywords of this case. For now, we have `disable` and `ignore`.
-        groups: List of groups of this case, this is usually the component which this case belongs to.
-        attributes: Dict of attributes of this case, which is used to describe timeout duration,
-            test environment, etc.
-        subcases: List of dict of subcases of this case, if this case is a `multi_stage` or `multi_device` one.
     """
 
+    #: The index of the case, which can be used to run this case.
     index: int
+    #: The name of the case.
     name: str
+    #: Type of this case, which can be `normal` `multi_stage` or `multi_device`.
     type: str
+    #: List of additional keywords of this case. For now, we have `disable` and `ignore`.
     keywords: t.List[str]
+    #: List of groups of this case, this is usually the component which this case belongs to.
     groups: t.List[str]
+    #: Dict of attributes of this case, which is used to describe timeout duration,
     attributes: t.Dict[str, t.Any]
+    #: List of dict of subcases of this case, if this case is a `multi_stage` or `multi_device` one.
     subcases: t.List[t.Dict[str, t.Any]]
 
     @property
     def is_ignored(self):
         return 'ignore' in self.keywords or 'disable' in self.keywords
 
 
@@ -71,20 +68,34 @@
     def __init__(self, *args, **kwargs):
         self._test_menu: t.List[UnittestMenuCase] = None  # type: ignore
 
         self._hard_reset_func: t.Optional[t.Callable] = None
 
         super().__init__(*args, **kwargs)
 
-    def confirm_write(self, write_str: t.Any, expect_str: str, timeout: int = 1, retry_times: int = 3):
+    def confirm_write(
+        self,
+        write_str: t.Any,
+        *,
+        expect_pattern: t.Any = None,
+        expect_str: t.Any = None,
+        timeout: int = 1,
+        retry_times: int = 3,
+    ):
+        if not ((expect_pattern is None) ^ (expect_str is None)):
+            raise ValueError('should provide expect_pattern= or expect_str=, but not both nor none')
+
         err = None
         for _ in range(retry_times):
             try:
                 self.write(str(write_str))
-                res = self.expect(expect_str, timeout=timeout)
+                if expect_pattern is not None:
+                    res = self.expect(expect_pattern, timeout=timeout)
+                else:
+                    res = self.expect_exact(expect_str, timeout=timeout)
             except pexpect.TIMEOUT as e:
                 err = e
             else:
                 break
         else:
             raise err
 
@@ -105,15 +116,15 @@
                      This will be directly passed to `pexpect.expect()`.
             trigger: Keys to trigger device to print test menu by UART.
 
         Returns:
             A `list` of `UnittestMenuCase`, which includes info for each test case.
         """
         self.expect_exact(ready_line)
-        res = self.confirm_write(trigger, pattern)
+        res = self.confirm_write(trigger, expect_pattern=pattern)
         return self._parse_unity_menu_from_str(res.group(1).decode('utf8'))
 
     def parse_test_menu(
         self,
         ready_line: str = 'Press ENTER to see the list of tests',
         pattern="Here's the test menu, pick your combo:(.+)Enter test for running.",
         trigger: str = '',
@@ -221,15 +232,15 @@
 
         return self._test_menu
 
     def _record_single_unity_test_case(func):
         """
         The first argument of the function that is using this decorator must be `case`. passing with args.
 
-        Notes:
+        Note:
             This function is better than `dut.expect_unity_output()` since it will record the test case even it core
                 dumped during running the test case or other reasons that cause the final result block is uncaught.
         """
 
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             _start_at = time.perf_counter()  # declare here in case hard reset failed
@@ -313,40 +324,40 @@
         case: UnittestMenuCase,
         reset: bool = False,
         timeout: float = 30,
     ) -> None:
         """
         Run a specific normal case
 
-        Notes:
+        Note:
             Will skip with a warning if the case type is not "normal"
 
         Args:
             case: the specific case that parsed in test menu
             reset: whether to perform a hardware reset before running a case
             timeout: timeout. (Default: 30 seconds)
         """
         if case.type != 'normal':
             logging.warning('case %s is not a normal case', case.name)
             return
 
         self.expect_exact(READY_PATTERN_LIST, timeout=timeout)
-        self.confirm_write(case.index, f'Running {case.name}...')
+        self.confirm_write(case.index, expect_str=f'Running {case.name}...')
 
     @_record_single_unity_test_case
     def _run_multi_stage_case(
         self,
         case: UnittestMenuCase,
         reset: bool = False,
         timeout: float = 30,
     ) -> None:
         """
         Run a specific multi_stage case
 
-        Notes:
+        Note:
             Will skip with a warning if the case type is not "multi_stage"
 
         Args:
             case: the specific case that parsed in test menu
             reset: whether to perform a hardware reset before running a case
             timeout: timeout. (Default: 30 seconds)
         """
@@ -358,18 +369,17 @@
         _timestamp = _start_at
         for sub_case in case.subcases:
             _timeout = timeout - _timestamp + _start_at
             if _timeout < 0:  # pexpect process would expect 30s if < 0
                 _timeout = 0
 
             self.expect_exact(READY_PATTERN_LIST, timeout=_timeout)
-            self.confirm_write(case.index, f'Running {case.name}...')
+            self.confirm_write(case.index, expect_str=f'Running {case.name}...')
 
-            # here we can't use confirm_write becuase the sub cases won't print anything
-            time.sleep(1)
+            # here we can't use confirm_write because the sub cases won't print anything
             self.write(str(sub_case['index']))
 
             _timestamp = time.perf_counter()
 
     def run_single_board_case(self, name: str, reset: bool = False, timeout: float = 30) -> None:
         for case in self.test_menu:
             if case.name == name and case.type == 'normal':
@@ -385,15 +395,15 @@
         self,
         group: t.Optional[str] = None,
         reset: bool = False,
         timeout: float = 30,
         run_ignore_cases: bool = False,
     ) -> None:
         """
-        Run all multi_stage cases
+        Run all single board cases, including multi_stage cases, and normal cases
 
         Args:
             group: test case group
             reset: whether to perform a hardware reset before running a case
             timeout: timeout. (Default: 30 seconds)
             run_ignore_cases: run ignored test cases or not
         """
@@ -579,15 +589,15 @@
         reset: bool = False,
         timeout: float = DEFAULT_TIMEOUT,
         start_retry: int = DEFAULT_START_RETRY,
     ) -> None:
         """
         Run a specific multi_device case
 
-        Notes:
+        Note:
             Will skip with a warning if the case type is not multi_device
 
         Args:
             case: the specific case that parsed in test menu
             reset: whether to perform a hardware reset before running a case
             timeout: timeout in second
             start_retry (int): number of retries for a single case when it is failed to start
```

### Comparing `pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/PKG-INFO` & `pytest-embedded-idf-1.3.1/pytest_embedded_idf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for esp-idf project
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
-Description: ### pytest-embedded-idf
-        
-        pytest embedded service for esp-idf project
-        
-        Extra Functionalities:
-        
-        === "`pytest-embedded-serial-esp` activated"
-        
-            - `app`: parse the built binary by idf rules and gather more information.
-            - `serial`: auto flash the built binary into the target board at the beginning when running test cases.
-        
-        === "`pytest-embedded-serial-esp` NOT activated"
-        
-            - `app`: parse the built binary by idf rules and gather more information.
-        
-        Used CLI Options:
-        
-        - `part-tool`
-        
-Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: serial
+
+### pytest-embedded-idf
+
+pytest embedded service for esp-idf project
+
+Extra Functionalities:
+
+```{eval-rst}
+.. tabs::
+
+   .. group-tab:: `pytest-embedded-serial-esp` activated
+
+        - `app`: parse the built binary by idf rules and gather more information.
+        - `serial`: auto flash the built binary into the target board at the beginning when running test cases.
+
+   .. group-tab:: `pytest-embedded-serial-esp` NOT activated
+
+        - `app`: parse the built binary by idf rules and gather more information.
+```
```

### Comparing `pytest-embedded-idf-1.3.0/setup.py` & `pytest-embedded-idf-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,24 @@
     version=VERSION,
     author=AUTHOR,
     author_email=EMAIL,
     license=LICENSE,
     url=URL,
     description=SHORT_DESCRIPTION,
     long_description=read('README.md'),
+    long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude='tests'),
     python_requires='>=3.7',
     install_requires=REQUIRES,
     extras_require=EXTRAS_REQUIRE,
     classifiers=[
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
+        'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

