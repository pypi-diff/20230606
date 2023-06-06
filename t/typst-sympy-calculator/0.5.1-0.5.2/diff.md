# Comparing `tmp/typst_sympy_calculator-0.5.1-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 35165 bytes, number of entries: 14
+Zip file size: 35169 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     8110 b- defN 23-Jun-06 14:16 DefaultTypstCalculator.py
--rw-rw-rw-  2.0 fat     7712 b- defN 23-Jun-06 14:17 TypstCalculator.py
--rw-rw-rw-  2.0 fat    11039 b- defN 23-Jun-06 12:49 TypstCalculatorServer.py
+-rw-rw-rw-  2.0 fat     7723 b- defN 23-Jun-06 16:15 TypstCalculator.py
+-rw-rw-rw-  2.0 fat    11040 b- defN 23-Jun-06 16:15 TypstCalculatorServer.py
 -rw-rw-rw-  2.0 fat    25952 b- defN 23-Jun-06 14:16 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17703 b- defN 23-Jun-06 08:35 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-Jun-06 08:35 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-Jun-06 08:35 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 14:18 typst_sympy_calculator-0.5.1.dist-info/RECORD
-14 files, 197409 bytes uncompressed, 33225 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/RECORD
+14 files, 197421 bytes uncompressed, 33229 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.1.dist-info/METADATA
+Filename: typst_sympy_calculator-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.1.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.1.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.1.dist-info/RECORD
+Filename: typst_sympy_calculator-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstCalculator.py

```diff
@@ -25,30 +25,30 @@
 
     def define_symbol_base(self, symbol_base_name: str):
         self.converter.define_symbol_base(symbol_base_name)
 
     def define_function(self, func_name: str):
         self.converter.define_function(func_name)
 
-    def set_variance(self, name: str, value, simplify=True):
+    def set_variance(self, name: str, value, simplify=False):
         if name.startswith('#'):
             name = name[1:]
         if not isinstance(value, str):
             self.var[name] = value
             return
         if simplify:
-            self.var[name] = self.converter.sympy(value).simplify()
+            self.var[name] = self._simplify(self.converter.sympy(value))
         else:
             self.var[name] = self.converter.sympy(value)
         name = '#' + name
         if not isinstance(value, str):
             self.var[name] = value
             return
         if simplify:
-            self.var[name] = self.converter.sympy(value).simplify()
+            self.var[name] = self._simplify(self.converter.sympy(value))
         else:
             self.var[name] = self.converter.sympy(value)
 
     def unset_variance(self, name: str):
         if name.startswith('#'):
             name = name[1:]
         if name in self.var:
```

## TypstCalculatorServer.py

```diff
@@ -125,15 +125,15 @@
             return result
 
     def clear_cache(self):
         for name in self.cache_variance_names:
             self.unset_variance(name)
         self.cache_variance_names = []
 
-    def set_variance(self, name: str, value, simplify=True):
+    def set_variance(self, name: str, value, simplify=False):
         if self.cache_mode:
             self.cache_variance_names.append(name)
         self.calculator.set_variance(name, value, simplify)
 
     def unset_variance(self, name: str):
         self.calculator.unset_variance(name)
```

## Comparing `typst_sympy_calculator-0.5.1.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.5.1.dist-info/METADATA` & `typst_sympy_calculator-0.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.5.1
+Version: 0.5.2
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

