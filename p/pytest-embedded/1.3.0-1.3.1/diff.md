# Comparing `tmp/pytest-embedded-1.3.0.tar.gz` & `tmp/pytest-embedded-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-1.3.0.tar", last modified: Wed May 31 13:09:02 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-1.3.1.tar", last modified: Tue Jun  6 08:07:03 2023, max compression
```

## Comparing `pytest-embedded-1.3.0.tar` & `pytest-embedded-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    50776 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/unity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/pytest_embedded/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/pytest_embedded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:02.000000 pytest-embedded-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 13:08:52.000000 pytest-embedded-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50774 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/unity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/pytest_embedded/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/pytest_embedded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:03.000000 pytest-embedded-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-06 08:06:48.000000 pytest-embedded-1.3.1/setup.py
```

### Comparing `pytest-embedded-1.3.0/PKG-INFO` & `pytest-embedded-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 1.2
 Name: pytest-embedded
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded
         
         A pytest plugin for embedded systems. Could activate different services for extra functionalities.
         
-        Used CLI Options:
-        
-        - `app_path`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-1.3.0/pytest_embedded/app.py` & `pytest-embedded-1.3.1/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.3.0/pytest_embedded/dut.py` & `pytest-embedded-1.3.1/pytest_embedded/dut.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,72 +97,74 @@
             return res
 
         return wrapper
 
     @_pexpect_func  # noqa
     def expect(self, pattern, **kwargs) -> Match:  # noqa
         """
-        Expect the `pattern` from the internal buffer. All the arguments would pass to `pexpect.expect()`.
+        Expect the `pattern` from the internal buffer. All the arguments will be passed to `pexpect.expect()`.
 
         Args:
             pattern: string, or compiled regex, or a list of string and compiled regex.
 
         Keyword Args:
             timeout (float): would raise `pexpect.TIMEOUT` exception when pattern is not matched after timeout
             expect_all (bool): need to match all specified patterns if this flag is `True`.
                 Otherwise match any of them could pass
 
         Returns:
-            (AnyStr): if you're matching pexpect.EOF or pexpect.TIMEOUT to get all the current buffers.
+            `AnyStr` or `re.Match`
 
-            (re.Match): if matched given string.
+            - `AnyStr`: if you're matching `pexpect.EOF` or `pexpect.TIMEOUT` to get all the current buffers.
+            - `re.Match`: if matched given string.
         """
         return self.pexpect_proc.expect(pattern, **kwargs)
 
     @_pexpect_func  # noqa
     def expect_exact(self, pattern, **kwargs) -> Match:  # noqa
         """
-        Expect the `pattern` from the internal buffer. All the arguments would pass to `pexpect.expect_exact()`.
+        Expect the `pattern` from the internal buffer. All the arguments will be passed to `pexpect.expect_exact()`.
 
         Args:
             pattern: string, or a list of string
 
         Keyword Args:
             timeout (float): would raise `pexpect.TIMEOUT` exception when pattern is not matched after timeout
             expect_all (bool): need to match all specified patterns if this flag is `True`.
                 Otherwise match any of them could pass
 
         Returns:
-            (AnyStr): if you're matching pexpect.EOF or pexpect.TIMEOUT to get all the current buffers.
+            `AnyStr` or `re.Match`
 
-            (re.Match): if matched given string.
+            - `AnyStr`: if you're matching `pexpect.EOF` or `pexpect.TIMEOUT` to get all the current buffers.
+            - `re.Match`: if matched given string.
         """
         return self.pexpect_proc.expect_exact(pattern, **kwargs)
 
     def expect_unity_test_output(
         self,
         remove_asci_escape_code: bool = True,
         timeout: float = 60,
         extra_before: Optional[AnyStr] = None,
     ) -> None:
         """
         Expect a unity test summary block and parse the output into junit report.
 
-        Would combine the junit report into the main one if you use `pytest --junitxml` feature.
+        Would combine the junit report into the main one if you use ``pytest --junitxml`` feature.
 
         Args:
             remove_asci_escape_code: remove asci escape code in the message field. (default: True)
             timeout: timeout. (default: 60 seconds)
             extra_before: would append before the expected bytes.
                 Use this argument when need to run `expect` functions between one unity test call.
 
-        Notes:
+        Note:
             - Would raise AssertionError at the end of the test if any unity test case result is "FAIL"
-            - Would raise TIMEOUT exception at the end of the test if any unity test case execution took longer
-                than timeout value
+            - Would raise TIMEOUT exception at the end of the test \
+                if any unity test case execution took longer than timeout value
 
         Warning:
             - All unity test cases record would be missed if the final report block is uncaught.
         """
         self.expect(UNITY_SUMMARY_LINE_REGEX, timeout=timeout)
 
         if extra_before:
@@ -178,21 +180,21 @@
     @_InjectMixinCls.require_services('idf')
     def run_all_single_board_cases(
         self,
         group: Optional[str] = None,
         reset: bool = False,
         timeout: float = 30,
         run_ignore_cases: bool = False,
-    ):
+    ) -> None:
         """
         Run all multi_stage cases
 
         Args:
             group: test case group
             reset: whether to perform a hardware reset before running a case
             timeout: timeout. (Default: 30 seconds)
             run_ignore_cases: run ignored test cases or not
 
         Warning:
-            requires enable service `idf`
+            requires enable service ``idf``
         """
         pass
```

### Comparing `pytest-embedded-1.3.0/pytest_embedded/log.py` & `pytest-embedded-1.3.1/pytest_embedded/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,23 @@
     def buffer_debug_str(self):
         return textwrap.shorten(
             remove_asci_color_code(to_str(self.buffer)),
             width=200,
             placeholder=f'... (total {len(self.buffer)} bytes)',
         )
 
-    def read_nonblocking(self, size=1, timeout=-1) -> bytes:
+    def read_nonblocking(self, size: int = 1, timeout: int = -1) -> bytes:
         """
         Since we're using real file stream, here we only raise an EOF error when the file stream has been closed.
         This could solve the `os.read()` blocked issue.
 
-        :return: String containing the bytes read
-
         Args:
-            size (int): Read at most *size* bytes.
-            timeout (float): Wait timeout seconds for file descriptor to be
-                ready to read. When -1 (default), use self.timeout. When 0, poll.
+            size: Read at most *size* bytes.
+            timeout: Wait timeout seconds for file descriptor to be
+                ready to read. When -1 (default), use `self.timeout`. When 0, poll.
 
         Returns:
             String containing the bytes read
         """
         try:
             if os.name == 'posix':
                 if timeout == -1:
@@ -111,15 +109,15 @@
     """
     live print the `subprocess.Popen` process
 
     Args:
         msg_queue: `MessageQueue` instance, would redirect to message queue instead of sys.stdout if specified
         expect_returncode: expect return code. (Default 0). Would raise exception when return code is different
 
-    Notes:
+    Note:
         This function behaves the same as `subprocess.call()`, it would block your current process.
     """
     default_kwargs = {
         'stdout': subprocess.PIPE,
         'stderr': subprocess.STDOUT,
     }
     default_kwargs.update(kwargs)
@@ -206,19 +204,18 @@
 
     def terminate(self):
         self.close()
 
         super().terminate()
 
     def write(self, s: AnyStr) -> None:
-        """
+        r"""
         Write to `stdin` via `stdin.write`.
 
-        If the input is `str`, will encode to `bytes` and add a b'\\n' automatically in the end.
-
-        if the input is `bytes`, will pass this directly.
+        - If the input is `str`, will encode to `bytes` and add a b'\\n' automatically in the end.
+        - If the input is `bytes`, will pass this directly.
 
         Args:
             s: bytes or str
         """
         logging.debug(f'{self.SOURCE} ->: {to_str(s)}')
         self.stdin.write(to_bytes(s, '\n'))
```

### Comparing `pytest-embedded-1.3.0/pytest_embedded/plugin.py` & `pytest-embedded-1.3.1/pytest_embedded/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
     return wrapper
 
 
 def multi_dut_fixture(func) -> t.Callable[..., t.Union[t.Any, t.Tuple[t.Any]]]:
     """
     Apply the multi-dut arguments to each fixture.
 
-    Notes:
+    Note:
         Run the `func(*args, **kwargs)` for multiple times by iterating all `kwargs` via `itemgetter`
 
         For example:
 
         - input: `{key1: (v1, v2), key2: (v1, v2)}`
         - output: `(func(**{key1: v1, key2: v1}), func(**{key1: v2, key2: v2}))`
 
@@ -383,15 +383,15 @@
 
 def multi_dut_generator_fixture(
     func,
 ) -> t.Callable[..., t.Generator[t.Union[t.Any, t.Tuple[t.Any]], t.Any, None]]:
     """
     Apply the multi-dut arguments to each fixture.
 
-    Notes:
+    Note:
         Run the `func()` for multiple times by iterating all `kwargs` via `itemgetter`. Auto call `close()` or
         `terminate()` method of the object after it yield back.
 
     Yields:
         The return value, if `count` is 1.
         The tuple of return values, if `count` is greater than 1.
     """
```

### Comparing `pytest-embedded-1.3.0/pytest_embedded/unity.py` & `pytest-embedded-1.3.1/pytest_embedded/unity.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-1.3.0/pytest_embedded/utils.py` & `pytest-embedded-1.3.1/pytest_embedded/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+import functools
 import importlib
 import logging
 import os
 import re
 import typing as t
 
 if t.TYPE_CHECKING:
@@ -113,18 +114,19 @@
 
 def to_list(s: _T) -> t.List[_T]:
     """
     Args:
         s: Anything
 
     Returns:
-        List (list[_T]):
-            - `list(s)` (List. If `s` is a tuple or a set.
-            - itself. If `s` is a list.
-            - `[s]`. If `s` is other types.
+        List (list[_T])
+
+        - `list(s)` (List. If `s` is a tuple or a set.
+        - itself. If `s` is a list.
+        - `[s]`. If `s` is other types.
     """
     if not s:
         return s
 
     if isinstance(s, set) or isinstance(s, tuple):
         return list(s)
     elif isinstance(s, list):
@@ -227,30 +229,31 @@
         name_obj_dict (dict[str, any]): name, real object dict, used to store real objects,
             no need to add lazy-load objects
         obj_module_dict (dict[str, str]): dict of object name and module name
 
     Returns:
         __getattr__ function
 
-    Examples:
-        ```python
-        __getattr__ = lazy_load(
-            importlib.import_module(__name__),
-            {
-                'IdfApp': IdfApp,
-                'LinuxDut': LinuxDut,
-                'LinuxSerial': LinuxSerial,
-                'CaseTester': CaseTester,
-            },
-            {
-                'IdfSerial': '.serial',
-                'IdfDut': '.dut',
-            },
-        )
-        ```
+    Example:
+
+        ::
+
+            __getattr__ = lazy_load(
+                importlib.import_module(__name__),
+                {
+                    'IdfApp': IdfApp,
+                    'LinuxDut': LinuxDut,
+                    'LinuxSerial': LinuxSerial,
+                    'CaseTester': CaseTester,
+                },
+                {
+                    'IdfSerial': '.serial',
+                    'IdfDut': '.dut',
+                },
+            )
     """
 
     def __getattr__(object_name):
         if object_name in name_obj_dict:
             return name_obj_dict[object_name]
         elif object_name in obj_module_dict:
             module = importlib.import_module(obj_module_dict[object_name], base_module.__name__)
@@ -290,41 +293,44 @@
     This class provide a check function `require_services()` to check if the function is injected by
     enabling one of the required services.
 
     The benefits are:
     - provide the autocompletion for the functions provided by the mixins
     - check the requirement at runtime
 
-    Examples:
+    Example:
+
+        ::
 
-        class IdfUnityMixin:
-            def foo(self):
-                print('foo from MixinOne')
+            class IdfUnityMixin:
+                def foo(self):
+                    print('foo from MixinOne')
 
 
-        class Test(_InjectMixinCls):
-            def __init__(self, **kwargs):
-                for k, v in kwargs.items():
-                    setattr(self, k, v)
+            class Test(_InjectMixinCls):
+                def __init__(self, **kwargs):
+                    for k, v in kwargs.items():
+                        setattr(self, k, v)
 
-            @_InjectMixinCls.require_services('idf')
-            def foo(self):
-                pass
+                @_InjectMixinCls.require_services('idf')
+                def foo(self):
+                    pass
 
 
-        # mro(): TestWithIdfUnityMixin, IdfUnityMixin, Test, object
-        s1 = Test(mixins=IdfUnityMixin)
-        # mro(): Test, object
-        s2 = Test()
-        s1.foo()  # foo from IdfUnityMixin
-        s2.foo()  # function foo requires enabling one of the service(s) idf.
+            # mro(): TestWithIdfUnityMixin, IdfUnityMixin, Test, object
+            s1 = Test(mixins=IdfUnityMixin)
+            # mro(): Test, object
+            s2 = Test()
+            s1.foo()  # foo from IdfUnityMixin
+            s2.foo()  # function foo requires enabling one of the service(s) idf.
     """
 
     def require_services(*services):
         def decorator(func):
+            @functools.wraps(func)
             def wrapped(self, *args, **kwargs):
                 based = False
                 for service in services:
                     if hasattr(self, _MIXIN_REQUIRED_SERVICES_KEY) and service in getattr(
                         self, _MIXIN_REQUIRED_SERVICES_KEY
                     ):
                         based = True
```

### Comparing `pytest-embedded-1.3.0/pytest_embedded.egg-info/PKG-INFO` & `pytest-embedded-1.3.1/pytest_embedded.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 1.2
 Name: pytest-embedded
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded
         
         A pytest plugin for embedded systems. Could activate different services for extra functionalities.
         
-        Used CLI Options:
-        
-        - `app_path`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-1.3.0/setup.py` & `pytest-embedded-1.3.1/setup.py`

 * *Files identical despite different names*

