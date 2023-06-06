# Comparing `tmp/school_grader-2.0.5.tar.gz` & `tmp/school_grader-3.0.0.tar.gz`

## Comparing `school_grader-2.0.5.tar` & `school_grader-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 school_grader-2.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    19534 2020-02-02 00:00:00.000000 school_grader-2.0.5/assets/extension1.PNG
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 school_grader-2.0.5/assets/extension2.PNG
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 school_grader-2.0.5/assets/html_report1.PNG
--rw-r--r--   0        0        0    29356 2020-02-02 00:00:00.000000 school_grader-2.0.5/assets/html_report2.PNG
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 school_grader-2.0.5/src/school_grader/__init__.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 school_grader-2.0.5/src/school_grader/html_test_result.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 school_grader-2.0.5/src/school_grader/json_test_result.py
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 school_grader-2.0.5/src/school_grader/test_case.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 school_grader-2.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 school_grader-2.0.5/LICENSE
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 school_grader-2.0.5/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 school_grader-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 school_grader-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 school_grader-3.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    19534 2020-02-02 00:00:00.000000 school_grader-3.0.0/assets/extension1.PNG
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 school_grader-3.0.0/assets/extension2.PNG
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 school_grader-3.0.0/assets/html_report1.PNG
+-rw-r--r--   0        0        0    24394 2020-02-02 00:00:00.000000 school_grader-3.0.0/assets/html_report2.PNG
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 school_grader-3.0.0/src/school_grader/__init__.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 school_grader-3.0.0/src/school_grader/equality.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 school_grader-3.0.0/src/school_grader/html_test_result.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 school_grader-3.0.0/src/school_grader/json_test_result.py
+-rw-r--r--   0        0        0     8414 2020-02-02 00:00:00.000000 school_grader-3.0.0/src/school_grader/test_case.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 school_grader-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 school_grader-3.0.0/LICENSE
+-rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 school_grader-3.0.0/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 school_grader-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 school_grader-3.0.0/PKG-INFO
```

### Comparing `school_grader-2.0.5/.github/workflows/python-publish.yml` & `school_grader-3.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `school_grader-2.0.5/assets/extension1.PNG` & `school_grader-3.0.0/assets/extension1.PNG`

 * *Files identical despite different names*

### Comparing `school_grader-2.0.5/assets/extension2.PNG` & `school_grader-3.0.0/assets/extension2.PNG`

 * *Files identical despite different names*

### Comparing `school_grader-2.0.5/src/school_grader/html_test_result.py` & `school_grader-3.0.0/src/school_grader/html_test_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,92 +3,93 @@
 
 from abc import ABC, abstractmethod
 from typing import List
 import unittest
 import webbrowser
 
 
-HTML_BEGIN = """<html>
-    <head>
-        <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
-        <style>
-            table {
-                border-radius: 10px;
-                width: 100%;
-                margin: 40px auto;
-                box-shadow: 0 2px 15px rgba(0, 0, 0, 0.1);
-                text-align: center;
-                border-spacing: 0;
-            }
-            table tr:first-child td {
-                border-top: 0;
-            }
-
-            table tr td:first-child {
-                border-left: 0;
-            }
-
-            table tr:last-child td {
-                border-bottom: 0;
-            }
-
-            table tr td:last-child {
-                border-right: 0;
-            }
-            th, td {
-                border: solid 1px #68706a29;
-                padding: 20px;
-                font-size: 16px;
-                font-weight: 500;
-                color: #333;
-                text-align: center;
-                vertical-align: middle;
-            }
-            th {
-                background-color: #ddd;
-                font-weight: bold;
-            }
-            pre {
-                background-color: #f6f8fa;
-                border-radius: 10px;
-                font-size: 85%;
-                line-height: 1.45;
-                overflow: auto;
-                padding: 16px;
-                text-align: left;
-                margin: 20px 0;
-            }
-            body {
-                padding: 20px;
-                background-color: #f2f2f2;
-                font-family: 'Roboto', sans-serif;
-            }
-            .error {
-                background-color: #FFE844;
-            }
-            .pass {
-                background-color: #A6FB88;
-            }
-            .fail {
-                background-color: #FF4444;
-            }
-        </style>
-    </head>
-    <body>
-        <table>
-            <tr>
-                <th>Test name</th>
-                <th>Directory</th>
-                <th>Result</th>
-                <th>Stack trace</th>
-            </tr>"""
-
-HTML_END = """</table>
-    </body>
-</html>"""
+HTML_BEGIN = (
+    "<html>"
+    "<head>"
+    '<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">'
+    "<style>"
+    "table {"
+    "border-radius: 10px;"
+    "width: 100%;"
+    "margin: 40px auto;"
+    "box-shadow: 0 2px 15px rgba(0, 0, 0, 0.1);"
+    "text-align: center;"
+    "border-spacing: 0;"
+    "}"
+    "table tr:first-child td {"
+    "border-top: 0;"
+    "}"
+    "table tr td:first-child {"
+    "border-left: 0;"
+    "}"
+    "table tr:last-child td {"
+    "border-bottom: 0;"
+    "}"
+    "table tr td:last-child {"
+    "border-right: 0;"
+    "}"
+    "th, td {"
+    "border: solid 1px #68706a29;"
+    "padding: 20px;"
+    "font-size: 16px;"
+    "font-weight: 500;"
+    "color: #333;"
+    "text-align: center;"
+    "vertical-align: middle;"
+    "}"
+    "th {"
+    "background-color: #ddd;"
+    "font-weight: bold;"
+    "}"
+    "pre {"
+    "background-color: #f6f8fa;"
+    "border-radius: 10px;"
+    "font-size: 85%;"
+    "line-height: 1.45;"
+    "overflow: auto;"
+    "padding: 16px;"
+    "text-align: left;"
+    "margin: 20px 0;"
+    "}"
+    "body {"
+    "padding: 20px;"
+    "background-color: #f2f2f2;"
+    "font-family: 'Roboto', sans-serif;"
+    "}"
+    ".error {"
+    "background-color: #FFE844;"
+    "}"
+    ".pass {"
+    "background-color: #A6FB88;"
+    "}"
+    ".fail {"
+    "background-color: #FF4444;"
+    "}"
+    "</style>"
+    "</head>"
+    "<body>"
+    "<table>"
+    "<tr>"
+    "<th>Test name</th>"
+    "<th>Directory</th>"
+    "<th>Result</th>"
+    "<th>Stack trace</th>"
+    "</tr>"
+)
+
+HTML_END = (
+    "</table>"
+    "</body>"
+    "</html>"
+)
 
 
 def sanitize_html(html_string: str):
     return html_string.replace("<", "&lt;").replace(">", "&gt;")
 
 
 class HTMLResult(ABC):
@@ -96,51 +97,51 @@
 
     def __init__(self, test):
         self._test = test
 
     @abstractmethod
     def generate_html(self):
         """Generates the HTML result of a test."""
-        return f"""
-        <tr>
-            <td><b>{sanitize_html(self._test.shortDescription())}</b></td>
-            <td><b>{sanitize_html(self._test._dirname)}</b></td>"""
-
+        return (
+            "<tr>"
+            f"<td><b>{sanitize_html(self._test.shortDescription())}</b></td>"
+            f"<td><b>{sanitize_html(self._test._dirname)}</b></td>"
+        )
 
 class HTMLSuccessResult(HTMLResult):
     """A class for the HTML result of a successful test."""
 
     def __init__(self, test):
         super().__init__(test)
 
     def generate_html(self):
         """Generates the HTML result of a successful test."""
-        return f"""
-        {super().generate_html()}
-            <td class="pass"><b>PASS</b></td>
-            <td></td>
-        </tr>
-        """
+        return (
+            super().generate_html() +
+            "<td class=\"pass\"><b>PASS</b></td>"
+            "<td></td>"
+            "</tr>"
+        )
 
 
 class HTMLFailureResult(HTMLResult):
     """A class for the HTML result of a failed test."""
 
     def __init__(self, test, stack_trace: str):
         super().__init__(test)
         self._stack_trace = stack_trace
 
     def generate_html(self):
         """Generates the HTML result of a failed test."""
-        return f"""
-        {super().generate_html()}
-            <td class="fail"><b>FAIL</b></td>
-            <td><pre>{sanitize_html(self._stack_trace)}</pre></td>
-        </tr>
-        """
+        return (
+            super().generate_html() +
+            "<td class=\"fail\"><b>FAIL</b></td>"
+            f"<td><pre>{sanitize_html(self._stack_trace)}</pre></td>"
+            "</tr>"
+        )
 
 
 class HTMLErrorResult(HTMLResult):
     """A class for the HTML result of a failed test."""
 
     def __init__(self, test, stack_trace: str):
         super().__init__(test)
@@ -165,24 +166,22 @@
 
     def addSuccess(self, test):
         """Adds a successful test to the HTML result."""
         self._test_result.append(HTMLSuccessResult(test))
 
     def addFailure(self, test, err):
         """Adds a failed test to the HTML result."""
-        self._test_result.append(HTMLFailureResult(
-            test, self._exc_info_to_string(err, test)))
+        self._test_result.append(HTMLFailureResult(test, self._exc_info_to_string(err, test)))
 
     def addError(self, test, err):
         """Adds an error test to the HTML result."""
-        self._test_result.append(HTMLErrorResult(
-            test, self._exc_info_to_string(err, test)))
+        self._test_result.append(HTMLErrorResult(test, self._exc_info_to_string(err, test)))
 
     def generate(self):
         """Generates the HTML result of a test."""
         html_content = HTML_BEGIN
         for result in self._test_result:
             html_content += result.generate_html()
         html_content += HTML_END
         with open("results.html", "w") as f:
             f.write(html_content)
-        webbrowser.open("results.html", new=2)
+        webbrowser.open("results.html", new=2)
```

### Comparing `school_grader-2.0.5/src/school_grader/json_test_result.py` & `school_grader-3.0.0/src/school_grader/json_test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 __author__ = "Marc-Olivier Derouin"
 __email__ = "marcolivier.derouin@poulet-frit.com"
 
 import unittest
 import json
 from dataclasses import dataclass
 
-
-
-
 @dataclass
 class Result:
     """A class for the result of a test."""
     description: int
     status: str
     message: str
```

### Comparing `school_grader-2.0.5/src/school_grader/test_case.py` & `school_grader-3.0.0/src/school_grader/test_case.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,92 +2,37 @@
 __email__ = "marcolivier.derouin@poulet-frit.com"
 
 import threading
 import _thread
 import unittest
 from unittest.mock import patch
 from abc import ABC, abstractmethod
-from typing import List, Callable, Union
+from typing import List, Callable, Optional, Union
 from io import StringIO
 from collections import deque
 import sys
 import importlib.util
-import re
 import os
-from school_grader import HTMLTestResult
-from school_grader.json_test_result import JSONTestResult
 import inspect
 import argparse
+from school_grader.html_test_result import HTMLTestResult
+from school_grader.json_test_result import JSONTestResult
+from school_grader.equality import Equality
 
 
-class Equality(ABC):
-    """Abstract base class for equality validation."""
-
-    @abstractmethod
-    def validate(self, unittest: unittest.TestCase, value_to_test: str, fail_message: str):
-        """Validate equality between `value_to_test` and the expected value.
-
-        Args:
-            unittest: Instance of `unittest.TestCase` to run the equality check.
-            value_to_test: The value to test for equality.
-            fail_message: The message to display if the equality check fails.
-        """
-        pass
-
-
-class AlmostEqualNumber(Equality):
-    """Class for almost equal numerical validation."""
-
-    def __init__(self, expected: str, precisions: List[int]):
-        """Initialize the class with the expected value and the precision values.
-
-        Args:
-            expected: The expected value as a string.
-            precisions: List of precisions, where each precision specifies the maximum difference
-                between the expected number and the result number that will be considered equal.
-        """
-        self.expected = expected
-        self.precisions = precisions
-
-    def validate(self, unittest: unittest.TestCase, value_to_test: str, fail_message: str):
-        """Validate almost equal numerical equality between `value_to_test` and the expected value.
-
-        Args:
-            unittest: Instance of `unittest.TestCase` to run the equality check.
-            value_to_test: The value to test for equality.
-            fail_message: The message to display if the equality check fails.
-        """
-        expected_numbers = list(
-            map(float, re.findall(r'[-+]?\d*\.\d+|\d+', self.expected)))
-        result_numbers = list(
-            map(float, re.findall(r'[-+]?\d*\.\d+|\d+', value_to_test)))
-
-        if len(self.precisions) != len(expected_numbers):
-            raise AssertionError(
-                "Number of precisions does not match the number of expected numbers")
-
-        if len(expected_numbers) != len(result_numbers):
-            raise AssertionError(
-                f"Expected {len(expected_numbers)} numbers, but got {len(result_numbers)}")
-
-        for expected_number, result_number, precision in zip(expected_numbers, result_numbers, self.precisions):
-            unittest.assertAlmostEqual(float(expected_number), float(
-                result_number), precision, fail_message)
-
-
-def timeout(timeout_time):
+def timeout(timeout_time: Optional[int]):
     """
     Decorator that sets a timer for a function execution.
     If the function execution takes longer than `timeout_time` seconds,
     the main thread of the program will be interrupted.
 
     :param timeout_time: The number of seconds after which to interrupt the main thread.
     :return: The decorated function.
     """
-    def decorator(function):
+    def decorator(function: Callable):
         """
         The actual decorator function that sets the timer and raises an exception
         if the function execution takes longer than `timeout_time` seconds.
 
         :param function: The function to be decorated.
         :return: The decorated function `inner`.
         """
@@ -98,23 +43,21 @@
 
             :param *args: The positional arguments passed to the decorated function.
             :param **kwargs: The keyword arguments passed to the decorated function.
             """
             timer = None
             try:
                 if timeout_time is not None:
-                    timer = threading.Timer(
-                        timeout_time, lambda: _thread.interrupt_main())
+                    timer = threading.Timer(timeout_time, lambda: _thread.interrupt_main())
                     timer.start()
                 function(*args, **kwargs)
             except KeyboardInterrupt:
-                raise TimeoutError(
-                    f'Program execution did not finish within the allotted time of {timeout_time} seconds. You may be in an infinite loop.')
+                raise TimeoutError(f'Program execution did not finish within the allotted time of {timeout_time} seconds. You may be in an infinite loop.')
             finally:
-                if timer:
+                if timer is not None:
                     timer.cancel()
         return inner
     return decorator
 
 
 class TestCase(unittest.TestCase, ABC):
     """Abstract base class for test cases."""
@@ -126,74 +69,71 @@
         self.shortDescription = lambda: test_name
         self._timeout = timeout
         self._fail_message = fail_message
         self._dirname = os.getcwd()
         self.line_number = inspect.currentframe().f_back.f_back.f_lineno
 
     @abstractmethod
-    def runTest(self):
+    def runTest(self) -> None:
         """Run the test case."""
         pass
 
 
 class FileTestCase(TestCase):
     """Custom test case class for testing python code"""
 
-    def __init__(self, test_name: str, file_name: str, expected_output: List[Union[str, Equality]], mock_input: List[str] = None, timeout: float = 1, fail_message: str = None):
+    def __init__(self, test_name: str, file_name: str, expected_output: List[Union[str, Equality]], mock_input: List[str] = [], timeout: float = 1, fail_message: str = None):
         """
         Initializes the test case with the given test name, file name, mock input, expected output, timeout and fail message
 
         :param test_name: name of the test
         :param file_name: name of the python file to be tested
         :param expected_output: list of str or Equality objects to be used as expected outputs
         :param mock_input: list of strings to be used as inputs
         :param timeout: maximum time in seconds that the test can run
         :param fail_message: message to be displayed in case of failure
         """
         super().__init__(test_name, timeout, fail_message)
         self._file_name = file_name
-        self._mock_input = mock_input or []
+        self._mock_input = mock_input
         self._expected_output = expected_output
 
-    def run_whole_file(self):
+    def run_whole_file(self) -> None:
         try:
-            spec = importlib.util.spec_from_file_location(
-                self._file_name, os.path.join(self._dirname, f'{self._file_name}.py'))
+            spec = importlib.util.spec_from_file_location(self._file_name, os.path.join(self._dirname, f'{self._file_name}.py'))
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
-        except FileNotFoundError:
-            raise FileNotFoundError(
-                f'File {self._file_name}.py not found. Your current working directory is {self._dirname}.')
+        except FileNotFoundError as e:
+            raise FileNotFoundError(f'File {self._file_name}.py not found. Your current working directory is {self._dirname}.') from e
 
-    def override_input(self):
+    def override_input(self) -> Callable[[], str]:
         queue = deque(self._mock_input)
-
-        def fake_input(*_):
+        def fake_input(*_, **__) -> str:
             if not queue:
                 raise AssertionError("Too many input calls. Check your code")
             return queue.popleft()
         return fake_input
 
     def runTest(self):
         @timeout(self._timeout)
         def exec_test():
             with patch('builtins.input', self.override_input()), patch('sys.stdout', new=StringIO()) as fake_out:
                 try:
                     self.run_whole_file()
                     output = fake_out.getvalue().strip().splitlines()
 
                     if (len(output) != len(self._expected_output)):
-                        raise AssertionError(
-                            f'The output of your program contains {len(output)} lines. You should have {len(self._expected_output)} lines')
+                        raise AssertionError(f'The output of your program contains {len(output)} lines. You should have {len(self._expected_output)} lines')
                     for result, expected in zip(output, self._expected_output):
                         if isinstance(expected, str):
-                            self.assertEqual(result, expected,
-                                             self._fail_message)
-                        else:
+                            self.assertEqual(result, expected,self._fail_message)
+                        elif isinstance(expected, Equality):
                             expected.validate(self, result, self._fail_message)
+                        else:
+                            raise TypeError(f'Expected output should be a string or an Equality object. Got {type(expected)} instead.')
                 finally:
                     sys.stdout = sys.__stdout__
         exec_test()
 
 
 class FunctionTestCase(TestCase):
     """A basic test case class for running unit tests.
@@ -205,60 +145,56 @@
         timeout (float): The maximum time in seconds allowed for the test to complete.
         fail_message (str, optional): A custom message to display on test failure. Default is None.
     """
 
     def __init__(self, test_name: str, result_func: Callable, expected_result, timeout: float = 1, fail_message: str = None):
         """Initialize the test case with the required attributes.
 
-        Args:
-            test_name (str): The name of the test case.
-            result_func (Callable): A function that returns the result to be tested.
-            expected_result: The expected result from the result_func.
-            timeout (float): The maximum time in seconds allowed for the test to complete.
-            fail_message (str, optional): A custom message to display on test failure. Default is None.
+        :param test_name: The name of the test case.
+        :param result_func: A function that returns the result to be tested.
+        :param expected_result: The expected result from the result_func.
+        :param timeout: The maximum time in seconds allowed for the test to complete.
+        :param fail_message: A custom message to display on test failure. Default is None.
         """
         super().__init__(test_name, timeout, fail_message)
         self._result_func = result_func
         self._expected_result = expected_result
 
     def runTest(self):
         """Execute the test case and check the result against the expected result."""
         @timeout(self._timeout)
         def exec_test():
             """Execute the test within a time limit defined by the timeout attribute."""
-            self.assertEqual(self._expected_result,
-                             self._result_func(), self._fail_message)
+            self.assertEqual(self._expected_result, self._result_func(), self._fail_message)
         exec_test()
 
 
 def run_tests(generate_html: bool = True):
     """
     Run all the tests in the BasicTestCase and FunctionTestCase classes.
 
     :param generate_html: Whether to generate an HTML report of the test results. Default is True.
     """
     if not TestCase.tests_case:
         raise ValueError("No test cases were added to the test suite.")
-    
+
     suite = unittest.TestSuite()
     suite.addTests(TestCase.tests_case)
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--extension', action='store_true')
     args = parser.parse_args()
 
     if args.extension:
         runner = unittest.TextTestRunner(resultclass=JSONTestResult)
-        with patch('sys.stdout', new=StringIO()) as _:
-            result = runner.run(unittest.TestSuite(TestCase.tests_case))
-        result.print_report()
-        return
+        with patch('sys.stdout', new=StringIO()):
+            result: JSONTestResult = runner.run(unittest.TestSuite(TestCase.tests_case))
+            result.print_report()
+            return
 
     if generate_html:
         runner = unittest.TextTestRunner(resultclass=HTMLTestResult)
-        result = runner.run(suite)
+        result: HTMLTestResult = runner.run(suite)
         result.generate()
     else:
         runner = unittest.TextTestRunner()
         runner.run(suite)
-    
-
```

### Comparing `school_grader-2.0.5/.gitignore` & `school_grader-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `school_grader-2.0.5/LICENSE` & `school_grader-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `school_grader-2.0.5/pyproject.toml` & `school_grader-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "school_grader"
-version = "2.0.5"
+version = "3.0.0"
 authors = [
   { name="Marc-Olivier Derouin", email="marcolivier.derouin@poulet-frit.com" },
 ]
 description = "Testing framework for Python students code."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-keywords = ["testing", "test", "students", "school", "education", "framework", "python", "python3", "python3.7", "python3.8", "python3.9", "python3.10"]
+keywords = ["testing", "test", "students", "school", "education", "framework", "python", "python3", "python3.7", "python3.8", "python3.9", "python3.10", "python3.11"]
 
 [project.urls]
 "Homepage" = "https://github.com/school-grader/school-grader"
 "Bug Tracker" = "https://github.com/school-grader/school-grader/issues"
```

