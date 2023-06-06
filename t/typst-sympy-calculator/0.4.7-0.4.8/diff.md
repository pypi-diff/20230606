# Comparing `tmp/typst_sympy_calculator-0.4.7-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33138 bytes, number of entries: 14
+Zip file size: 33323 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     7111 b- defN 23-May-31 13:00 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
--rw-rw-rw-  2.0 fat     9984 b- defN 23-May-30 15:34 TypstCalculatorServer.py
+-rw-rw-rw-  2.0 fat    11376 b- defN 23-Jun-06 08:20 TypstCalculatorServer.py
 -rw-rw-rw-  2.0 fat    21135 b- defN 23-May-31 13:01 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    12770 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1169 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/RECORD
-14 files, 185815 bytes uncompressed, 31198 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    12770 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/RECORD
+14 files, 187208 bytes uncompressed, 31383 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.7.dist-info/METADATA
+Filename: typst_sympy_calculator-0.4.8.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.7.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.7.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.7.dist-info/RECORD
+Filename: typst_sympy_calculator-0.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstCalculatorServer.py

```diff
@@ -89,34 +89,52 @@
         return self.calculator.typst(sympy_expr)
 
     def doit(self, sympy_expr):
         return self.calculator.doit(sympy_expr)
 
     def subs(self, typst_math: str, typst_file: str = None):
         expr = self.sympy(typst_math, typst_file)
-        result = expr.subs(self.variances, simultaneous=True)
+        max_sub_count = 5
+        sub_count = 0
+        last = None
+        while last != expr and sub_count < max_sub_count:
+            last = expr
+            expr = expr.subs(self.variances, simultaneous=True)
+            sub_count += 1
         if self.return_text:
-            return self.typst(result)
+            return self.typst(expr)
         else:
-            return result
+            return expr
 
     def simplify(self, typst_math: str, typst_file: str = None):
         expr = self.sympy(typst_math, typst_file)
         if self.enable_subs:
-            expr = expr.subs(self.variances, simultaneous=True)
+            max_sub_count = 5
+            sub_count = 0
+            last = None
+            while last != expr and sub_count < max_sub_count:
+                last = expr
+                expr = expr.subs(self.variances, simultaneous=True)
+                sub_count += 1
         result = sympy.simplify(self.doit(expr))
         if self.return_text:
             return self.typst(result)
         else:
             return result
 
     def evalf(self, typst_math: str, typst_file: str = None, n: int = None):
         expr = self.sympy(typst_math, typst_file)
         if self.enable_subs:
-            expr = expr.subs(self.variances, simultaneous=True)
+            max_sub_count = 5
+            sub_count = 0
+            last = None
+            while last != expr and sub_count < max_sub_count:
+                last = expr
+                expr = expr.subs(self.variances, simultaneous=True)
+                sub_count += 1
         result = sympy.N(sympy.simplify(self.doit(expr)),
                          n=n if n else self.precision)
         if self.return_text:
             return self.typst(result)
         else:
             return result
 
@@ -158,54 +176,58 @@
         test()
         ```
 
         ```typst-calculator
         test()
         ```
         '''
-        pattern1 = r'\s*```python\s*\n\s*# typst-calculator\s*\n([\d\D]*?)```'
-        pattern2 = r'\s*```py\s*\n\s*# typst-calculator\s*\n([\d\D]*?)```'
-        pattern3 = r'\s*```typst-calculator\s*\n([\d\D]*?)```'
-        pattern4 = r'\s*```typst-sympy-calculator\s*\n([\d\D]*?)```'
+        typst_content = self.remove_comments(typst_content)
+        pattern1 = r'[\t ]*```python[\t ]*\n[\t ]*# typst-calculator[\t ]*\n([\d\D]*?)```'
+        pattern2 = r'[\t ]*```py[\t ]*\n[\t ]*# typst-calculator[\t ]*\n([\d\D]*?)```'
+        pattern3 = r'[\t ]*```typst-calculator[\t ]*\n([\d\D]*?)```'
+        pattern4 = r'[\t ]*```typst-sympy-calculator[\t ]*\n([\d\D]*?)```'
         for match in re.finditer(pattern1, typst_content):
             self.exec(match.group(1))
         for match in re.finditer(pattern2, typst_content):
             self.exec(match.group(1))
         for match in re.finditer(pattern3, typst_content):
             self.exec(match.group(1))
         for match in re.finditer(pattern4, typst_content):
             self.exec(match.group(1))
 
     def find_and_define_accent(self, typst_content: str):
         '''
         #let acc(x) = math.accent(x, math.grave)
         '''
-        pattern = r'#let\s+([a-zA-z][a-zA-z0-9]*)\(\s*([_a-zA-z][_\-a-zA-z0-9]*)\s*\)\s*=\s*math\.accent'
+        typst_content = self.remove_comments(typst_content)
+        pattern = r'#let[\t ]+([a-zA-z][a-zA-z0-9]*)\([\t ]*([_a-zA-z][_\-a-zA-z0-9]*)[\t ]*\)[\t ]*=[\t ]*math\.accent'
         for match in re.finditer(pattern, typst_content):
             accent_name = match.group(1)
             accent_arg = match.group(2)
             self.calculator.define_accent(accent_name)
 
     def find_and_define_func(self, typst_content: str):
         '''
         #let fn = math.op("fn")
         '''
-        pattern = r'#let\s+([a-zA-z][a-zA-z0-9]*)\s*=\s*math\.op'
+        typst_content = self.remove_comments(typst_content)
+        pattern = r'#let[\t ]+([a-zA-z][a-zA-z0-9]*)[\t ]*=[\t ]*math\.op'
         for match in re.finditer(pattern, typst_content):
             func_name = match.group(1)
             self.calculator.define_function(func_name)
 
     def find_and_define_symbol(self, typst_content: str):
         '''
         #let xy = math.italic("xy")
         #let xy = symbol("🖂", ("stamped", "🖃"),)
         '''
-        pattern1 = r'#let\s+([a-zA-z][a-zA-z0-9]*)\s*=\s*math\.(?!op)'
-        pattern2 = r'#let\s+([a-zA-z][a-zA-z0-9]*)\s*=\s*symbol(\(.+\))\s*\n'
-        pattern3 = r'\("(.+?)"\s*,\s*"(.+?)"\)'
+        typst_content = self.remove_comments(typst_content)
+        pattern1 = r'#let[\t ]+([a-zA-z][a-zA-z0-9]*)[\t ]*=[\t ]*math\.(?!op)'
+        pattern2 = r'#let[\t ]+([a-zA-z][a-zA-z0-9]*)[\t ]*=[\t ]*symbol(\(.+\))[\t ]*\n'
+        pattern3 = r'\("(.+?)"[\t ]*,[\t ]*"(.+?)"\)'
         for match in re.finditer(pattern1, typst_content):
             symbol_name = match.group(1)
             self.calculator.define_symbol_base(symbol_name)
         for match in re.finditer(pattern2, typst_content):
             symbol_name = match.group(1)
             self.calculator.define_symbol_base(symbol_name)
             for m in re.finditer(pattern3, match.group(2)[1:-1]):
@@ -213,36 +235,47 @@
                 self.calculator.define_symbol_base(symbol_name + '.' + modify)
 
     def find_and_set_variance(self, typst_content: str):
         '''
         #let var = 2.0
         #let var = $x + y$
         '''
-        pattern1 = r'#let\s+([a-zA-z][._a-zA-z0-9]*)\s*=\s*([0-9]+(\.[0-9]*)?\%?)\s*\n'
-        pattern2 = r'#let\s+([a-zA-z][._a-zA-z0-9]*)\s*=\s*\$(.+?)\$\s*\n'
+        typst_content = self.remove_comments(typst_content)
+        pattern1 = r'#let[\t ]+([a-zA-z][._a-zA-z0-9]*)[\t ]*=[\t ]*([-+]?[\t ]*[0-9]+(\.[0-9]*)?\%?)[\t ]*\n'
+        pattern2 = r'#let[\t ]+([a-zA-z][._a-zA-z0-9]*)[\t ]*=[\t ]*\$(.+?)\$[\t ]*\n'
         for match in re.finditer(pattern1, typst_content):
             symbol_name = match.group(1)
             self.set_variance(symbol_name, match.group(2))
         for match in re.finditer(pattern2, typst_content):
             symbol_name = match.group(1)
             self.set_variance(symbol_name, match.group(2))
 
     def find_import_and_include(self, typst_content: str) -> list:
         '''
         #import "../../../Typst/report-template.typ"
         #include "../../../Typst/report-template.typ"
         '''
-        pattern1 = r'#import\s+"(.+?)"'
-        pattern2 = r'#include\s+"(.+?)"'
+        typst_content = self.remove_comments(typst_content)
+        pattern1 = r'#import[\t ]+"(.+?)"'
+        pattern2 = r'#include[\t ]+"(.+?)"'
         paths = []
         for match in re.finditer(pattern1, typst_content):
             paths.append(match.group(1))
         for match in re.finditer(pattern2, typst_content):
             paths.append(match.group(1))
         return paths
+    
+    def remove_comments(self, typst_content: str) -> str:
+        '''
+        // #let var = 2.0
+        /* #let var = 2.0 */
+        '''
+        pattern1 = r'\/\/.*?\n'
+        pattern2 = r'\/\*[\d\D]*?\*\/'
+        return re.sub(pattern2, '', re.sub(pattern1, '', typst_content))
 
 
 if __name__ == '__main__':
     server = TypstCalculatorServer()
     typst_file = os.path.abspath(r'./tests/test.typ')
     server.init(typst_file)
     server.return_text = True
```

## Comparing `typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.7.dist-info/METADATA` & `typst_sympy_calculator-0.4.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.7
+Version: 0.4.8
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `typst_sympy_calculator-0.4.7.dist-info/RECORD` & `typst_sympy_calculator-0.4.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DefaultTypstCalculator.py,sha256=SpwQmZJ3SCXlFTFbXdD1e3nPywwzVztrlYCFEhzxd34,7111
 TypstCalculator.py,sha256=bfCf1g_vPkTDBp3gi8uVwmuybG3HJEspF226CcqVhiI,4242
-TypstCalculatorServer.py,sha256=NvFNnZeP2MbP-ICsIHX1dPOOVYlSn40q2FfulWWrAJg,9984
+TypstCalculatorServer.py,sha256=3AQJaTIKi3c6CfdUBSzJYjAmo3fhbujByMrHHPI0B-c,11376
 TypstConverter.py,sha256=fPh9d66rUDSspOKVvvdi5ZO0GYr74T2v2gLIKXfqMcI,21135
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.7.dist-info/METADATA,sha256=220qBFsx_Pu1-I8kV0H9u4YiTeTcjfdnjWOtTx77eyM,12770
-typst_sympy_calculator-0.4.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.7.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.7.dist-info/RECORD,,
+typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.4.8.dist-info/METADATA,sha256=vdhm4AOU-y4ZG-Bf7RDbVNgyXlWpf2LFlYYQycx6K4w,12770
+typst_sympy_calculator-0.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.4.8.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.4.8.dist-info/RECORD,,
```

