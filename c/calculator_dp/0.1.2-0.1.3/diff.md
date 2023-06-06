# Comparing `tmp/calculator_dp-0.1.2.tar.gz` & `tmp/calculator_dp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator_dp-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "calculator_dp-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `calculator_dp-0.1.2.tar` & `calculator_dp-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1443 2023-06-03 07:55:59.769389 calculator_dp-0.1.2/.gitignore
--rw-r--r--   0        0        0      153 2023-06-03 09:34:24.389571 calculator_dp-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     7511 2023-06-01 10:49:00.812462 calculator_dp-0.1.2/115.ipynb
--rw-r--r--   0        0        0       62 2023-06-04 10:09:39.547818 calculator_dp-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1104 2023-06-03 08:47:22.877933 calculator_dp-0.1.2/LICENSE
--rw-r--r--   0        0        0     1345 2023-06-04 19:33:05.731343 calculator_dp-0.1.2/Makefile
--rw-r--r--   0        0        0     1844 2023-06-04 10:08:54.965074 calculator_dp-0.1.2/README.md
--rw-r--r--   0        0        0      889 2023-06-04 18:51:42.238729 calculator_dp-0.1.2/main.py
--rw-r--r--   0        0        0       52 2023-06-04 18:27:31.586779 calculator_dp-0.1.2/mycalculator/__init__.py
--rw-r--r--   0        0        0     4764 2023-06-04 12:25:07.733199 calculator_dp-0.1.2/mycalculator/calculator.py
--rw-r--r--   0        0        0      450 2023-06-04 11:45:17.468345 calculator_dp-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 08:43:04.120358 calculator_dp-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3499 2023-06-05 07:19:19.898765 calculator_dp-0.1.2/tests/test_calculator.py
--rw-r--r--   0        0        0      393 2023-06-04 12:26:00.171625 calculator_dp-0.1.2/tox.ini
--rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 calculator_dp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1443 2023-06-03 07:55:59.769389 calculator_dp-0.1.3/.gitignore
+-rw-r--r--   0        0        0      153 2023-06-03 09:34:24.389571 calculator_dp-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0     7511 2023-06-01 10:49:00.812462 calculator_dp-0.1.3/115.ipynb
+-rw-r--r--   0        0        0       62 2023-06-04 10:09:39.547818 calculator_dp-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1104 2023-06-03 08:47:22.877933 calculator_dp-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1345 2023-06-04 19:33:05.731343 calculator_dp-0.1.3/Makefile
+-rw-r--r--   0        0        0     1974 2023-06-06 11:03:44.045519 calculator_dp-0.1.3/README.md
+-rw-r--r--   0        0        0      938 2023-06-06 10:47:25.975369 calculator_dp-0.1.3/main.py
+-rw-r--r--   0        0        0       52 2023-06-06 11:01:58.396928 calculator_dp-0.1.3/mycalculator/__init__.py
+-rw-r--r--   0        0        0     5104 2023-06-06 11:01:07.059928 calculator_dp-0.1.3/mycalculator/calculator.py
+-rw-r--r--   0        0        0      450 2023-06-04 11:45:17.468345 calculator_dp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 08:43:04.120358 calculator_dp-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3615 2023-06-06 10:53:08.927614 calculator_dp-0.1.3/tests/test_calculator.py
+-rw-r--r--   0        0        0      393 2023-06-04 12:26:00.171625 calculator_dp-0.1.3/tox.ini
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 calculator_dp-0.1.3/PKG-INFO
```

### Comparing `calculator_dp-0.1.2/.gitignore` & `calculator_dp-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `calculator_dp-0.1.2/115.ipynb` & `calculator_dp-0.1.3/115.ipynb`

 * *Files identical despite different names*

### Comparing `calculator_dp-0.1.2/LICENSE` & `calculator_dp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calculator_dp-0.1.2/Makefile` & `calculator_dp-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `calculator_dp-0.1.2/README.md` & `calculator_dp-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 - addition;
 - subtraction;
 - multiplication;
 - division;
 - taking n-th root.
 
 
+Feel free to test this package on Colab:
+https://colab.research.google.com/drive/1uMqeByiKxSz4wNqJlSgiFFqrXeDLLWu8?usp=sharing
+
+
 ## Details
 
 Class attributes:
 
 - `.result` -- read-only attribute, returns a numeric value of current result `.__result`.
    Initial (default) value of `.__result` is 0.
 
@@ -23,14 +27,15 @@
 - `.add(value)` -- This method performs addition of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.subtract(value)` -- This method performs subtraction of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.multiply_by(value)` -- This method performs multiplication of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.divide_by(value)` -- This method performs division of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.root_by(value)` -- This method performs taking n-th root of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.reset()` -- This method resets the `.__result` to 0 (default).   
 
+
 ## Installation
 
 ```sh
 pip install calculator_dp
 ```
 
 ## Examples
```

### Comparing `calculator_dp-0.1.2/main.py` & `calculator_dp-0.1.3/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 if __name__ == "__main__":
     from mycalculator.calculator import Calculator
 
     calculator = Calculator()
     print(f"Initializing. Default result: {calculator.result}")
 
+    print(calculator)
+    # help(calculator)
+
     calculator.add(100)
     print(f"Calling: add 100. Result: {calculator.result}")
 
     calculator.subtract(50)
     print(f"Calling: subtract 50. Result: {calculator.result}")
 
     calculator.multiple_by(4)
```

### Comparing `calculator_dp-0.1.2/mycalculator/calculator.py` & `calculator_dp-0.1.3/mycalculator/calculator.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,20 +30,25 @@
     >>> print(calculator.result)
     0.0
     """
 
     @property
     # Property decorator - read-only attribute
     def result(self) -> float:
-        """Initializing class object"""
+        """Read-only attribute which returns the value of working
+        attribute `__result`.
+        """
         return self.__result
 
     def __init__(self) -> None:
         self.__result = 0.0
 
+    def __repr__(self) -> None:
+        return "This object performs simple math operations."
+
     def add(self, value: float) -> None:
         """Add `value` to a value of attribute `result` and save
         result to `result`
 
         Args
         ---------
         value (float): The value that will be added to `result`
@@ -124,14 +129,16 @@
         ---------
         >>> calculator = Calculator()
         >>> calculator.add(10)
         >>> calculator.divide_by(2)
         >>> print(calculator.result)
         5.0
         """
+        if value == 0:
+            raise ZeroDivisionError("Can't divide by zero.")
         self.__result = self.__result / value
 
     def root_by(self, value: float) -> None:
         """Take `value` root of the value of attribute `result` and save
         result to `result`
 
         Args
@@ -147,14 +154,16 @@
         ---------
         >>> calculator = Calculator()
         >>> calculator.add(100)
         >>> calculator.root_by(2)
         >>> print(calculator.result)
         10.0
         """
+        if value == 0:
+            raise ZeroDivisionError("Can't divide by zero.")
         self.__result = self.__result ** (1 / value)
 
     def reset(self) -> None:
         """Reset the value of attribute `result`.
 
         Returns
         ---------
```

### Comparing `calculator_dp-0.1.2/tests/test_calculator.py` & `calculator_dp-0.1.3/tests/test_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,17 @@
     calculator = Calculator()
     calculator.add(100)
     calculator.root_by(2)
     assert calculator.result == 10
     calculator.add(90)
     calculator.root_by(-2)
     assert calculator.result == 0.1
+    if calculator.result == 0:
+        with pytest.raises(ZeroDivisionError):
+            calculator.root_by(-2)
 
 
 def test_root_by_wrong_inputs():
     calculator = Calculator()
     calculator.add(100)
     # Input is str instead of float:
     with pytest.raises(TypeError):
```

### Comparing `calculator_dp-0.1.2/PKG-INFO` & `calculator_dp-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculator_dp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lets do simple math
 Author-email: Dainius Pakeltis <dainius.pakeltis@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 
 # Basic Calculator
 
@@ -15,14 +15,18 @@
 - addition;
 - subtraction;
 - multiplication;
 - division;
 - taking n-th root.
 
 
+Feel free to test this package on Colab:
+https://colab.research.google.com/drive/1uMqeByiKxSz4wNqJlSgiFFqrXeDLLWu8?usp=sharing
+
+
 ## Details
 
 Class attributes:
 
 - `.result` -- read-only attribute, returns a numeric value of current result `.__result`.
    Initial (default) value of `.__result` is 0.
 
@@ -31,14 +35,15 @@
 - `.add(value)` -- This method performs addition of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.subtract(value)` -- This method performs subtraction of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.multiply_by(value)` -- This method performs multiplication of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.divide_by(value)` -- This method performs division of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.root_by(value)` -- This method performs taking n-th root of numeric value of `.__result` (class attribute) and `value` (parameter) and saves the result as `.__result`.
 - `.reset()` -- This method resets the `.__result` to 0 (default).   
 
+
 ## Installation
 
 ```sh
 pip install calculator_dp
 ```
 
 ## Examples
```

