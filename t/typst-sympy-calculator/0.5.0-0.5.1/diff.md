# Comparing `tmp/typst_sympy_calculator-0.5.0-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 35063 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     7926 b- defN 23-Jun-06 12:27 DefaultTypstCalculator.py
--rw-rw-rw-  2.0 fat     7683 b- defN 23-Jun-06 12:37 TypstCalculator.py
+Zip file size: 35165 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     8110 b- defN 23-Jun-06 14:16 DefaultTypstCalculator.py
+-rw-rw-rw-  2.0 fat     7712 b- defN 23-Jun-06 14:17 TypstCalculator.py
 -rw-rw-rw-  2.0 fat    11039 b- defN 23-Jun-06 12:49 TypstCalculatorServer.py
--rw-rw-rw-  2.0 fat    25676 b- defN 23-Jun-06 12:41 TypstConverter.py
+-rw-rw-rw-  2.0 fat    25952 b- defN 23-Jun-06 14:16 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17703 b- defN 23-Jun-06 08:35 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-Jun-06 08:35 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-Jun-06 08:35 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/RECORD
-14 files, 196920 bytes uncompressed, 33123 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/RECORD
+14 files, 197409 bytes uncompressed, 33225 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.0.dist-info/METADATA
+Filename: typst_sympy_calculator-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.0.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.0.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.0.dist-info/RECORD
+Filename: typst_sympy_calculator-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DefaultTypstCalculator.py

```diff
@@ -324,7 +324,13 @@
     assert expr == '1/3'
 
     expr = calculator.simplify('derivative(x^2, x)')
     assert expr == '2 x'
 
     expr = calculator.simplify('x^2 bar_1^(2+1)')
     assert expr == '8'
+
+    expr = calculator.simplify('(x - 1) / (x + 1)^2')
+    assert expr == '(x - 1) / (x + 1)^2'
+
+    expr = calculator.simplify('-1 / (x + 1)')
+    assert expr == '-1 / (x + 1)'
```

## TypstCalculator.py

```diff
@@ -2,20 +2,20 @@
 from typing import Iterable
 import sympy
 from TypstConverter import TypstMathConverter
 
 
 class TypstCalculator:
 
-    def __init__(self, precision: int = 15, return_text=False, enable_subs=True):
+    def __init__(self, precision: int = 15, return_text=False, enable_subs=True, max_sub_count=1):
         self.converter = TypstMathConverter()
         self.precision = precision
         self.return_text = return_text
         self.enable_subs = enable_subs
-        self.max_sub_count = 5
+        self.max_sub_count = max_sub_count
         self.var = {}
 
     def define(self, name: str, type: str, value: str):
         self.converter.define(name, type, value)
 
     def undefine(self, name: str):
         self.converter.undefine(name)
```

## TypstConverter.py

```diff
@@ -30,15 +30,19 @@
     def _print_Mul(self, expr):
         def mul(x, y):
             if x == '1':
                 return y
             if x == '-1':
                 return '-' + y
             return x + ' ' + y
-        return reduce(mul, map(self.paren, expr.args))
+        x = expr.args[0]
+        if x.is_Pow and x.args[1].is_Number and x.args[1] < 0:
+            return (reduce(mul, [self.paren(arg) for arg in expr.args[1:]]) if len(expr.args) > 1 else '1') + ' / ' + self.paren(sympy.simplify(x ** -1))
+        else:
+            return reduce(mul, [self.paren(arg) for arg in expr.args])
     
     # matrix form: mat(1, 2; 3, 4)
     def _print_MatrixBase(self, expr):
         n, m, mat_flattern = expr.args
         res = 'mat('
         rows = [mat_flattern[i:i+m] for i in range(0, n*m, m)]
         res += '; '.join(map(lambda row: ', '.join(map(self.doprint, row)), rows))
```

## Comparing `typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.5.0.dist-info/METADATA` & `typst_sympy_calculator-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `typst_sympy_calculator-0.5.0.dist-info/RECORD` & `typst_sympy_calculator-0.5.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-DefaultTypstCalculator.py,sha256=BAjiYxf7-_xaMjQxakZD2hEpRTIs8bR39g9eJdgdwKA,7926
-TypstCalculator.py,sha256=4AjhzjT4rx421NYshEa-smQJ-FmRVCsDuNUUh_ly9sA,7683
+DefaultTypstCalculator.py,sha256=2hvQfvtzwC13K_BSAjjCWB6G-wbWxW4-m1f6ms46dMA,8110
+TypstCalculator.py,sha256=TtYmz7A66vUBGJrkkCJ0aKkb35TBoohAcpY5wTSa5Xs,7712
 TypstCalculatorServer.py,sha256=pMa-igBftbG7LFxa5-BWAU1IyXl6LfHTa1-86Vkch4o,11039
-TypstConverter.py,sha256=wkHDHU4WAaaPf0ieXS8_IrcLQSvvd1PtgDY129nlZIU,25676
+TypstConverter.py,sha256=0t7M-irkUo4eHlv18adxABEhsR9CkvWrbhGH7TZ7XiM,25952
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=GVL1rcChdiQif2X-Fd7qnooKPUWtMCjInIOkJ8rzf7M,17703
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.5.0.dist-info/METADATA,sha256=0a7opBKKMtc1_buFe5l_4FDRDH3mYS60NtsUdrbqp-8,13675
-typst_sympy_calculator-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.5.0.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.5.0.dist-info/RECORD,,
+typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.5.1.dist-info/METADATA,sha256=vkfPfTi5mYXIYMsqokeGKx0-ZS12MfLVZwJT6nV_by8,13675
+typst_sympy_calculator-0.5.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.5.1.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.5.1.dist-info/RECORD,,
```

