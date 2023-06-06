# Comparing `tmp/typst_sympy_calculator-0.4.8-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33323 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     7111 b- defN 23-May-31 13:00 DefaultTypstCalculator.py
--rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
--rw-rw-rw-  2.0 fat    11376 b- defN 23-Jun-06 08:20 TypstCalculatorServer.py
--rw-rw-rw-  2.0 fat    21135 b- defN 23-May-31 13:01 TypstConverter.py
+Zip file size: 35063 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     7926 b- defN 23-Jun-06 12:27 DefaultTypstCalculator.py
+-rw-rw-rw-  2.0 fat     7683 b- defN 23-Jun-06 12:37 TypstCalculator.py
+-rw-rw-rw-  2.0 fat    11039 b- defN 23-Jun-06 12:49 TypstCalculatorServer.py
+-rw-rw-rw-  2.0 fat    25676 b- defN 23-Jun-06 12:41 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
--rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
--rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
--rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
+-rw-rw-rw-  2.0 fat    17703 b- defN 23-Jun-06 08:35 gen/TypstGrammarLexer.py
+-rw-rw-rw-  2.0 fat    10476 b- defN 23-Jun-06 08:35 gen/TypstGrammarListener.py
+-rw-rw-rw-  2.0 fat    94820 b- defN 23-Jun-06 08:35 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    12770 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 08:21 typst_sympy_calculator-0.4.8.dist-info/RECORD
-14 files, 187208 bytes uncompressed, 31383 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 12:50 typst_sympy_calculator-0.5.0.dist-info/RECORD
+14 files, 196920 bytes uncompressed, 33123 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.8.dist-info/METADATA
+Filename: typst_sympy_calculator-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.8.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.8.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.8.dist-info/RECORD
+Filename: typst_sympy_calculator-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DefaultTypstCalculator.py

```diff
@@ -58,14 +58,19 @@
 
     # complex_number
     if complex_number:
         calculator.set_variance('i', sympy.I)
         calculator.set_variance('I', sympy.I)
         calculator.set_variance('j', sympy.I)
 
+    # Cases
+    @func()
+    def convert_cases(*args):
+        return args
+
     # Relation Operators
     @relation_op()
     def convert_eq(a, b):
         return sympy.Eq(a, b)
 
     @relation_op()
     def convert_eq_dot_not(a, b):
@@ -105,26 +110,40 @@
     def convert_div(a, b):
         return a / b
 
     # Postfix Operators
     @postfix_op()
     def convert_degree(expr):
         return expr / 180 * sympy.pi
+        
 
     # Matrix
     @func_mat()
     def convert_mat(mat):
         return sympy.Matrix(mat)
 
     @func()
     def convert_vec(*vec):
         return sympy.Matrix(vec)
+    
+    # Reduces
+    @reduce_op()
+    def convert_sum(expr, args):
+        return sympy.Sum(expr, args)
+
+    @reduce_op()
+    def convert_product(expr, args):
+        return sympy.Product(expr, args)
 
     # Functions
     @func()
+    def convert_derivative(expr, var):
+        return sympy.Derivative(expr, var)
+
+    @func()
     def convert_binom(n, k):
         return sympy.binomial(n, k)
 
     @func()
     def convert_frac(n, d):
         return sympy.Rational(n, d)
 
@@ -290,7 +309,22 @@
 
     calculator.define_function('f')
     expr = calculator.simplify('f(1) + f(1) - f(1)')
     assert expr == 'f(1)'
 
     expr = calculator.simplify('lim_(x -> oo) 1/x')
     assert expr == '0'
+
+    expr = calculator.simplify('sum_(k = 1)^n k')
+    assert expr == '1/2 n (n + 1)'
+
+    expr = calculator.simplify('product_(k = 1)^3 k')
+    assert expr == '6'
+
+    expr = calculator.simplify('integral_0^1 x^2 dif x')
+    assert expr == '1/3'
+
+    expr = calculator.simplify('derivative(x^2, x)')
+    assert expr == '2 x'
+
+    expr = calculator.simplify('x^2 bar_1^(2+1)')
+    assert expr == '8'
```

## TypstCalculator.py

```diff
@@ -1,18 +1,21 @@
+import itertools
+from typing import Iterable
 import sympy
 from TypstConverter import TypstMathConverter
 
 
 class TypstCalculator:
 
     def __init__(self, precision: int = 15, return_text=False, enable_subs=True):
         self.converter = TypstMathConverter()
         self.precision = precision
         self.return_text = return_text
         self.enable_subs = enable_subs
+        self.max_sub_count = 5
         self.var = {}
 
     def define(self, name: str, type: str, value: str):
         self.converter.define(name, type, value)
 
     def undefine(self, name: str):
         self.converter.undefine(name)
@@ -23,23 +26,38 @@
     def define_symbol_base(self, symbol_base_name: str):
         self.converter.define_symbol_base(symbol_base_name)
 
     def define_function(self, func_name: str):
         self.converter.define_function(func_name)
 
     def set_variance(self, name: str, value, simplify=True):
+        if name.startswith('#'):
+            name = name[1:]
+        if not isinstance(value, str):
+            self.var[name] = value
+            return
+        if simplify:
+            self.var[name] = self.converter.sympy(value).simplify()
+        else:
+            self.var[name] = self.converter.sympy(value)
+        name = '#' + name
         if not isinstance(value, str):
             self.var[name] = value
             return
         if simplify:
             self.var[name] = self.converter.sympy(value).simplify()
         else:
             self.var[name] = self.converter.sympy(value)
 
     def unset_variance(self, name: str):
+        if name.startswith('#'):
+            name = name[1:]
+        if name in self.var:
+            del self.var[name]
+        name = '#' + name
         if name in self.var:
             del self.var[name]
 
     def clear_variance(self):
         self.var.clear()
 
     @property
@@ -60,38 +78,115 @@
             return sympy_expr
         last = None
         while last != sympy_expr:
             last = sympy_expr
             sympy_expr = sympy_expr.doit()
         return sympy_expr
 
+    def _subs(self, expr):
+        sub_count = 0
+        last = None
+        while last != expr and sub_count < self.max_sub_count:
+            last = expr
+            expr = expr.subs(self.variances, simultaneous=True)
+            sub_count += 1
+        return expr
+
     def subs(self, typst_math: str):
         expr = self.sympy(typst_math)
-        result = expr.subs(self.variances, simultaneous=True)
+        expr = self._subs(expr)
         if self.return_text:
-            return self.typst(result)
+            return self.typst(expr)
         else:
-            return result
+            return expr
 
-    def simplify(self, typst_math: str):
-        expr = self.sympy(typst_math)
+    def _simplify(self, expr):
         if self.enable_subs:
-            expr = expr.subs(self.variances, simultaneous=True)
+            expr = self._subs(expr)
         result = sympy.simplify(self.doit(expr))
+        return result
+
+    def simplify(self, typst_math: str):
+        expr = self.sympy(typst_math)
+        result = self._simplify(expr)
         if self.return_text:
             return self.typst(result)
         else:
             return result
 
-    def evalf(self, typst_math: str, n: int = None):
-        expr = self.sympy(typst_math)
+    def _evalf(self, expr, n: int = None):
         if self.enable_subs:
-            expr = expr.subs(self.variances, simultaneous=True)
+            expr = self._subs(expr)
         result = sympy.N(sympy.simplify(self.doit(expr)),
                          n=n if n else self.precision)
+        return result
+
+    def evalf(self, typst_math: str, n: int = None):
+        expr = self.sympy(typst_math)
+        result = self._evalf(expr, n)
+        if self.return_text:
+            return self.typst(result)
+        else:
+            return result
+
+    def _solve(self, expr):
+        if self.enable_subs:
+            sub_count = 0
+            last = None
+            while last != expr and sub_count < self.max_sub_count:
+                last = expr
+                if isinstance(expr, list):
+                    expr = [e.subs(self.variances, simultaneous=True)
+                            for e in expr]
+                if isinstance(expr, tuple):
+                    expr = tuple(e.subs(self.variances, simultaneous=True)
+                                 for e in expr)
+                elif isinstance(expr, dict):
+                    expr = {k: v.subs(self.variances, simultaneous=True)
+                            for k, v in expr.items()}
+                else:
+                    expr = expr.subs(self.variances, simultaneous=True)
+                sub_count += 1
+        if isinstance(expr, Iterable):
+            # is all equations
+            is_all_equations = True
+            for e in expr:
+                if not isinstance(e, sympy.Eq):
+                    is_all_equations = False
+                    break
+            if is_all_equations:
+                result = []
+                free_symbols = set()
+                for e in expr:
+                    free_symbols.update(e.free_symbols)
+                # subsets of free_symbols
+                subsets = []
+                for i in range(1, len(free_symbols) + 1):
+                    subsets.extend(itertools.combinations(free_symbols, i))
+                for subset in subsets:
+                    result.extend(sympy.solve(expr, subset, dict=True))
+            else:
+                result = sympy.solve(expr, dict=True)
+        else:
+            if isinstance(expr, sympy.Eq):
+                result = []
+                free_symbols = expr.free_symbols
+                # subsets of free_symbols
+                subsets = []
+                for i in range(1, len(free_symbols) + 1):
+                    subsets.extend(itertools.combinations(free_symbols, i))
+                for subset in subsets:
+                    result.extend(sympy.solve(expr, subset, dict=True))
+            else:
+                result = sympy.solve(expr, dict=True)
+        return result
+
+    def solve(self, typst_math: str):
+        expr = self.sympy(typst_math)
+        result = self._solve(expr)
         if self.return_text:
             return self.typst(result)
         else:
             return result
 
     @property
     def id2type(self):
@@ -133,10 +228,10 @@
     calculator.unset_variance('a')
     expr = calculator.simplify('a + 1')
     assert expr == 'a + 1' or expr == '1 + a'
 
     @constant()
     def convert_pi():
         return sympy.pi
-    
+
     expr = calculator.simplify('pi')
-    assert expr == 'pi'
+    assert expr == 'pi'
```

## TypstCalculatorServer.py

```diff
@@ -1,24 +1,25 @@
+import itertools
+from typing import Iterable
 import sympy
 import math
 import re
 import os
 from TypstCalculator import TypstCalculator
 from DefaultTypstCalculator import get_default_calculator
 
-VERSION = '0.4.2'
+VERSION = '0.5.0'
 
 
 class TypstCalculatorServer:
 
-    def __init__(self, calculator: TypstCalculator = None, precision=15) -> None:
+    def __init__(self, calculator: TypstCalculator = None) -> None:
         if calculator is None:
             calculator = get_default_calculator()
         self.calculator = calculator
-        self.precision = precision
         self.cache_variance_names = []
         self.cache_mode = True
 
     @property
     def var(self):
         return self.calculator.var
 
@@ -89,54 +90,39 @@
         return self.calculator.typst(sympy_expr)
 
     def doit(self, sympy_expr):
         return self.calculator.doit(sympy_expr)
 
     def subs(self, typst_math: str, typst_file: str = None):
         expr = self.sympy(typst_math, typst_file)
-        max_sub_count = 5
-        sub_count = 0
-        last = None
-        while last != expr and sub_count < max_sub_count:
-            last = expr
-            expr = expr.subs(self.variances, simultaneous=True)
-            sub_count += 1
+        result = self.calculator._subs(expr)
         if self.return_text:
-            return self.typst(expr)
+            return self.typst(result)
         else:
-            return expr
+            return result
 
     def simplify(self, typst_math: str, typst_file: str = None):
         expr = self.sympy(typst_math, typst_file)
-        if self.enable_subs:
-            max_sub_count = 5
-            sub_count = 0
-            last = None
-            while last != expr and sub_count < max_sub_count:
-                last = expr
-                expr = expr.subs(self.variances, simultaneous=True)
-                sub_count += 1
-        result = sympy.simplify(self.doit(expr))
+        result = self.calculator._simplify(expr)
         if self.return_text:
             return self.typst(result)
         else:
             return result
 
     def evalf(self, typst_math: str, typst_file: str = None, n: int = None):
         expr = self.sympy(typst_math, typst_file)
-        if self.enable_subs:
-            max_sub_count = 5
-            sub_count = 0
-            last = None
-            while last != expr and sub_count < max_sub_count:
-                last = expr
-                expr = expr.subs(self.variances, simultaneous=True)
-                sub_count += 1
-        result = sympy.N(sympy.simplify(self.doit(expr)),
-                         n=n if n else self.precision)
+        result = self.calculator._evalf(expr, n)
+        if self.return_text:
+            return self.typst(result)
+        else:
+            return result
+
+    def solve(self, typst_math: str, typst_file: str = None):
+        expr = self.sympy(typst_math, typst_file)
+        result = self.calculator._solve(expr)
         if self.return_text:
             return self.typst(result)
         else:
             return result
 
     def clear_cache(self):
         for name in self.cache_variance_names:
@@ -259,15 +245,15 @@
         pattern2 = r'#include[\t ]+"(.+?)"'
         paths = []
         for match in re.finditer(pattern1, typst_content):
             paths.append(match.group(1))
         for match in re.finditer(pattern2, typst_content):
             paths.append(match.group(1))
         return paths
-    
+
     def remove_comments(self, typst_content: str) -> str:
         '''
         // #let var = 2.0
         /* #let var = 2.0 */
         '''
         pattern1 = r'\/\/.*?\n'
         pattern2 = r'\/\*[\d\D]*?\*\/'
@@ -278,20 +264,28 @@
     server = TypstCalculatorServer()
     typst_file = os.path.abspath(r'./tests/test.typ')
     server.init(typst_file)
     server.return_text = True
     expr = server.simplify('1 + 1', typst_file)
     print(expr)
     server.enable_subs = False
-    expr = server.simplify('a + 1', typst_file)
+    expr = server.simplify('#a + 1', typst_file)
     print(expr)
     server.enable_subs = True
-    expr = server.simplify('a + 1', typst_file)
+    expr = server.simplify('#a + 1', typst_file)
     print(expr)
     expr = server.simplify('b + 1', typst_file)
     print(expr)
-    expr = server.simplify('cmat(1, 2)', typst_file)
+    expr = server.simplify('#cmat(1, 2)', typst_file)
     print(expr)
     expr = server.simplify('f(1) + f(1)', typst_file)
     print(expr)
     expr = server.simplify('xy + mail + mail.stamped', typst_file)
     print(expr)
+    expr = server.solve('x + y + z = 1')
+    print(expr)
+    expr = server.solve('cases(x + y + z = 1, x = 2)')
+    print(expr)
+    expr = server.solve('cases(x^2 + y = 4, y = 2)')
+    print(expr)
+    expr = server.solve('cases(x < 2, x > 1)')
+    print(expr)
```

## TypstConverter.py

```diff
@@ -6,16 +6,39 @@
 
 
 class TypstMathPrinter(StrPrinter):
 
     def paren(self, expr):
         return '(' + self.doprint(expr) + ')' if expr.is_Add else self.doprint(expr)
 
+    def _print_list(self, lst):
+        lst = list(set([self.doprint(item) for item in lst]))
+        # lst = [self.doprint(item) for item in lst]
+        return ', '.join(lst)
+
+    def _print_tuple(self, tup):
+        return ', '.join([self.doprint(item) for item in tup])
+    
+    def _print_dict(self, dic):
+        if len(dic) == 0:
+            return 'nothing'
+        elif len(dic) == 1:
+            k, v = dic.popitem()
+            return self.doprint(k) + ' = ' + self.doprint(v)
+        else:
+            return 'cases(' + ', '.join([self.doprint(k) + ' = ' + self.doprint(v) for k, v in dic.items()]) + ')'
+
     def _print_Mul(self, expr):
-        return reduce(lambda x, y: x + ' ' + y, map(self.paren, expr.args))
+        def mul(x, y):
+            if x == '1':
+                return y
+            if x == '-1':
+                return '-' + y
+            return x + ' ' + y
+        return reduce(mul, map(self.paren, expr.args))
     
     # matrix form: mat(1, 2; 3, 4)
     def _print_MatrixBase(self, expr):
         n, m, mat_flattern = expr.args
         res = 'mat('
         rows = [mat_flattern[i:i+m] for i in range(0, n*m, m)]
         res += '; '.join(map(lambda row: ', '.join(map(self.doprint, row)), rows))
@@ -65,31 +88,53 @@
             return "1 / sqrt(%s)" % self.doprint(b)
         if e is -sympy.S.One:
             return "1 / %s" % base
         if e.is_Atom or e.is_Pow:
             return base + '^' + self.doprint(e)
         else:
             return base + '^' + '(' + self.doprint(e) + ')'
+    
+    def _print_And(self, expr):
+        return ' and '.join([self.doprint(item) for item in expr.args])
+
+    def _print_Or(self, expr):
+        return ' or '.join([self.doprint(item) for item in expr.args])
+
+    def _print_Not(self, expr):
+        return 'not ' + self.doprint(expr.args[0])
 
 
 class TypstMathConverter(object):
 
     id2type = {}
     id2func = {}
 
     def __init__(self) -> None:
         self.parser = TypstMathParser()
         self.printer = TypstMathPrinter()
 
     def define(self, name: str, type: str, func: Callable = None):
+        if name.startswith('#'):
+            name = name[1:]
+        self.id2type[name.split('_')[0]] = type
+        if isinstance(func, Callable):
+            self.id2func[name] = func
+        name = '#' + name
         self.id2type[name.split('_')[0]] = type
         if isinstance(func, Callable):
             self.id2func[name] = func
 
     def undefine(self, name: str):
+        if name.startswith('#'):
+            name = name[1:]
+        if name in self.id2type:
+            del self.id2type[name]
+        if name in self.id2func:
+            del self.id2func[name]
+        name = '#' + name
         if name in self.id2type:
             del self.id2type[name]
         if name in self.id2func:
             del self.id2func[name]
 
     def define_accent(self, accent_name: str):
         self.define(accent_name, 'ACCENT_OP')
@@ -120,15 +165,15 @@
             relations = relation.relation()
             assert len(relations) == 2
             op = relation_op.getText()
 
             def rel(i):
                 return self.convert_relation(relations[i])
             if op == '=':
-                raise NotImplementedError('equal')
+                return sympy.Eq(rel(0), rel(1))
             elif op == '==':
                 return sympy.Eq(rel(0), rel(1))
             elif op == '!=':
                 return sympy.Ne(rel(0), rel(1))
             elif op == '<':
                 return sympy.Lt(rel(0), rel(1))
             elif op == '>':
@@ -209,23 +254,35 @@
         else:
             postfixes = [self.convert_postfix(pos) for pos in unary.postfix()]
             assert len(postfixes) >= 1
             if len(postfixes) == 1:
                 return postfixes[0]
             else:
                 return reduce(lambda x, y: x * y, postfixes)
+    
+    def convert_eval_at(self, expr, eval_at):
+        # eval_at: EVAL_BAR subsupassign;
+        symbol, sub, sup = self.convert_subsupassign(eval_at.subsupassign())
+        if symbol is None:
+            symbol = expr.free_symbols.pop()
+        assert sub or sup
+        if sub is None or sup is None:
+            val = sub or sup
+            return expr.subs(symbol, val)
+        else:
+            return expr.subs(symbol, sup) - expr.subs(symbol, sub)
 
     def convert_postfix(self, postfix):
         exp = postfix.exp()
         assert exp
         result = self.convert_exp(exp)
         postfix_ops = postfix.postfix_op()
         for postfix_op in postfix_ops:
             if postfix_op.eval_at():
-                raise NotImplementedError('eval_at')
+                result = self.convert_eval_at(result, postfix_op.eval_at())
             elif postfix_op.transpose():
                 result = sympy.transpose(result)
             elif postfix_op.POSTFIX_OP():
                 op = postfix_op.POSTFIX_OP().getText()
                 if op == '!':
                     result = sympy.factorial(result)
                 elif op == '%':
@@ -316,17 +373,62 @@
     def convert_matrix(self, matrix):
         func_name = matrix.FUNC_MAT().getText()
         if func_name in self.id2type and self.id2type[func_name] == 'FUNC_MAT':
             assert func_name in self.id2func, f'function for {func_name} not found'
             return self.id2func[func_name](matrix)
         else:
             raise Exception(f'unknown matrix function {func_name}')
+        
+    def convert_subassign(self, subassign):
+        if subassign.atom():
+            return None, self.convert_atom(subassign.atom())
+        elif subassign.expr():
+            return None, self.convert_expr(subassign.expr())
+        elif subassign.relation():
+            # assert relation is `symbol = expr`
+            rel = self.convert_relation(subassign.relation())
+            assert isinstance(rel, sympy.Equality)
+            return rel.lhs, rel.rhs
+        
+    def convert_supassign(self, supassign):
+        if supassign.exp():
+            return None, self.convert_exp(supassign.exp())
+        elif supassign.expr():
+            return None, self.convert_expr(supassign.expr())
+        elif supassign.relation():
+            rel = self.convert_relation(supassign.relation())
+            assert isinstance(rel, sympy.Equality)
+            assert isinstance(rel.lhs, sympy.Symbol), f'lhs of {supassign.relation().getText()} is not a symbol'
+            return rel.lhs, rel.rhs
+    
+    def convert_subsupassign(self, subsupassign):
+        symbol = None
+        sub = None
+        sup = None
+        # process sub
+        if subsupassign.subassign():
+            sym, sub = self.convert_subassign(subsupassign.subassign())
+            if sym:
+                symbol = sym
+        # process sup
+        if subsupassign.supexpr():
+            sup = self.convert_supexpr(subsupassign.supexpr())
+        elif subsupassign.supassign():
+            sym, sup = self.convert_supassign(subsupassign.supassign())
+            if sym:
+                symbol = sym
+        return (symbol, sub, sup)
 
     def convert_reduceit(self, reduceit):
-        raise NotImplementedError('reduceit')
+        reduce_name = reduceit.REDUCE_OP().getText()
+        if reduce_name in self.id2type and self.id2type[reduce_name] == 'REDUCE_OP':
+            assert reduce_name in self.id2func, f'function for {reduce_name} not found'
+            return self.id2func[reduce_name](reduceit)
+        else:
+            raise Exception(f'unknown reduce function {reduce_name}')
 
     def convert_lim(self, lim):
         symbol = self.convert_symbol(lim.symbol())
         expr = self.convert_expr(lim.expr())
         additive = self.convert_additive(lim.additive())
         return sympy.Limit(additive, symbol, expr)
 
@@ -453,15 +555,24 @@
                 def convert_ast(result):
                     return [result], {}
                 super().__init__('POSTFIX_OP', convert_ast, name, ast)
 
         class reduce_op(operator):
 
             def __init__(self, name: str = None, ast=False):
-                raise NotImplementedError('reduce_op')
+                def convert_ast(reduceit):
+                    # reduceit: REDUCE_OP subsupassign mp;
+                    symbol, sub, sup = self.env.convert_subsupassign(reduceit.subsupassign())
+                    assert sub is not None and sup is not None
+                    mp = self.env.convert_mp(reduceit.mp())
+                    if symbol is None:
+                        # get the first symbol in mp
+                        symbol = mp.free_symbols.pop()
+                    return [mp, (symbol, sub, sup)], {}
+                super().__init__('REDUCE_OP', convert_ast, name, ast)
 
         class func(operator):
 
             def __init__(self, name: str = None, ast=False):
                 def convert_ast(func):
                     func_args = func.args()
                     if func_args:
```

## gen/TypstGrammarLexer.py

```diff
@@ -5,183 +5,187 @@
 import sys
 
 
 
 def serializedATN():
     with StringIO() as buf:
         buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\2)")
-        buf.write("\u0197\b\1\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7")
+        buf.write("\u019f\b\1\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7")
         buf.write("\t\7\4\b\t\b\4\t\t\t\4\n\t\n\4\13\t\13\4\f\t\f\4\r\t\r")
         buf.write("\4\16\t\16\4\17\t\17\4\20\t\20\4\21\t\21\4\22\t\22\4\23")
         buf.write("\t\23\4\24\t\24\4\25\t\25\4\26\t\26\4\27\t\27\4\30\t\30")
         buf.write("\4\31\t\31\4\32\t\32\4\33\t\33\4\34\t\34\4\35\t\35\4\36")
         buf.write("\t\36\4\37\t\37\4 \t \4!\t!\4\"\t\"\4#\t#\4$\t$\4%\t%")
-        buf.write("\4&\t&\4\'\t\'\4(\t(\4)\t)\4*\t*\4+\t+\3\2\3\2\3\2\3\3")
-        buf.write("\3\3\3\3\3\3\3\3\3\4\3\4\3\4\3\4\3\4\3\5\3\5\3\5\3\5\3")
-        buf.write("\5\3\5\3\5\3\6\3\6\3\7\3\7\3\b\3\b\3\t\3\t\3\t\3\t\3\t")
-        buf.write("\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3\t\3")
-        buf.write("\t\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n")
-        buf.write("\3\n\3\n\3\n\3\n\3\13\6\13\u0097\n\13\r\13\16\13\u0098")
-        buf.write("\3\13\3\13\3\f\3\f\3\f\3\f\3\r\3\r\3\16\3\16\3\17\3\17")
-        buf.write("\3\20\3\20\3\21\3\21\3\22\3\22\3\23\3\23\3\24\3\24\3\24")
-        buf.write("\3\24\3\24\3\24\5\24\u00b5\n\24\3\25\3\25\3\26\3\26\3")
-        buf.write("\27\3\27\3\30\3\30\3\31\3\31\3\32\3\32\3\33\3\33\3\33")
-        buf.write("\3\34\3\34\3\34\3\34\3\34\3\34\3\34\3\34\3\34\3\34\5\34")
-        buf.write("\u00d0\n\34\3\35\3\35\3\36\3\36\3\36\5\36\u00d7\n\36\3")
-        buf.write("\37\3\37\3 \3 \3 \3 \3 \3 \3 \3 \3 \3 \3 \3 \3 \3 \3 ")
-        buf.write("\3 \3 \3 \3 \3 \3!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3")
-        buf.write("!\3!\3!\3!\3!\3!\3!\3!\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"")
-        buf.write("\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3#\3#\3#\3#\3")
-        buf.write("#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3$\3$\3$\3$\3%\3")
-        buf.write("%\3%\3%\3&\3&\3&\3&\3&\3&\3&\3&\3&\3\'\3\'\3\'\3\'\3(")
-        buf.write("\3(\3(\3(\3(\3)\3)\3)\3)\3)\3)\3)\3)\3)\3)\3)\3)\3)\3")
-        buf.write(")\3)\3)\3)\3)\3)\3)\3)\3)\3)\3)\3)\3*\6*\u015a\n*\r*\16")
-        buf.write("*\u015b\3*\3*\3*\3*\3*\7*\u0163\n*\f*\16*\u0166\13*\3")
-        buf.write("*\7*\u0169\n*\f*\16*\u016c\13*\3*\3*\3*\3*\3*\7*\u0173")
-        buf.write("\n*\f*\16*\u0176\13*\3*\3*\6*\u017a\n*\r*\16*\u017b\5")
-        buf.write("*\u017e\n*\3+\3+\3+\7+\u0183\n+\f+\16+\u0186\13+\3+\3")
-        buf.write("+\3+\3+\7+\u018c\n+\f+\16+\u018f\13+\7+\u0191\n+\f+\16")
-        buf.write("+\u0194\13+\3+\3+\2\2,\3\3\5\4\7\5\t\6\13\2\r\2\17\2\21")
-        buf.write("\7\23\b\25\t\27\n\31\13\33\f\35\r\37\16!\17#\20%\21\'")
-        buf.write("\22)\23+\24-\25/\26\61\27\63\30\65\31\67\329\33;\34=\35")
-        buf.write("?\36A\37C E!G\"I#K$M%O&Q\'S(U)\3\2\n\5\2\13\f\17\17\"")
-        buf.write("\"\3\2\62;\4\2C\\c|\4\2((^^\4\2>>@@\4\2--//\4\2,,\61\61")
-        buf.write("\4\2##\'\'\2\u01a6\2\3\3\2\2\2\2\5\3\2\2\2\2\7\3\2\2\2")
-        buf.write("\2\t\3\2\2\2\2\21\3\2\2\2\2\23\3\2\2\2\2\25\3\2\2\2\2")
-        buf.write("\27\3\2\2\2\2\31\3\2\2\2\2\33\3\2\2\2\2\35\3\2\2\2\2\37")
-        buf.write("\3\2\2\2\2!\3\2\2\2\2#\3\2\2\2\2%\3\2\2\2\2\'\3\2\2\2")
-        buf.write("\2)\3\2\2\2\2+\3\2\2\2\2-\3\2\2\2\2/\3\2\2\2\2\61\3\2")
-        buf.write("\2\2\2\63\3\2\2\2\2\65\3\2\2\2\2\67\3\2\2\2\29\3\2\2\2")
-        buf.write("\2;\3\2\2\2\2=\3\2\2\2\2?\3\2\2\2\2A\3\2\2\2\2C\3\2\2")
-        buf.write("\2\2E\3\2\2\2\2G\3\2\2\2\2I\3\2\2\2\2K\3\2\2\2\2M\3\2")
-        buf.write("\2\2\2O\3\2\2\2\2Q\3\2\2\2\2S\3\2\2\2\2U\3\2\2\2\3W\3")
-        buf.write("\2\2\2\5Z\3\2\2\2\7_\3\2\2\2\td\3\2\2\2\13k\3\2\2\2\r")
-        buf.write("m\3\2\2\2\17o\3\2\2\2\21q\3\2\2\2\23\u0084\3\2\2\2\25")
-        buf.write("\u0096\3\2\2\2\27\u009c\3\2\2\2\31\u00a0\3\2\2\2\33\u00a2")
-        buf.write("\3\2\2\2\35\u00a4\3\2\2\2\37\u00a6\3\2\2\2!\u00a8\3\2")
-        buf.write("\2\2#\u00aa\3\2\2\2%\u00ac\3\2\2\2\'\u00b4\3\2\2\2)\u00b6")
-        buf.write("\3\2\2\2+\u00b8\3\2\2\2-\u00ba\3\2\2\2/\u00bc\3\2\2\2")
-        buf.write("\61\u00be\3\2\2\2\63\u00c0\3\2\2\2\65\u00c2\3\2\2\2\67")
-        buf.write("\u00cf\3\2\2\29\u00d1\3\2\2\2;\u00d6\3\2\2\2=\u00d8\3")
-        buf.write("\2\2\2?\u00da\3\2\2\2A\u00ee\3\2\2\2C\u0102\3\2\2\2E\u0114")
-        buf.write("\3\2\2\2G\u0125\3\2\2\2I\u0129\3\2\2\2K\u012d\3\2\2\2")
-        buf.write("M\u0136\3\2\2\2O\u013a\3\2\2\2Q\u013f\3\2\2\2S\u017d\3")
-        buf.write("\2\2\2U\u017f\3\2\2\2WX\7`\2\2XY\7V\2\2Y\4\3\2\2\2Z[\7")
-        buf.write("`\2\2[\\\7v\2\2\\]\7q\2\2]^\7r\2\2^\6\3\2\2\2_`\7`\2\2")
-        buf.write("`a\7*\2\2ab\7V\2\2bc\7+\2\2c\b\3\2\2\2de\7`\2\2ef\7*\2")
-        buf.write("\2fg\7v\2\2gh\7q\2\2hi\7r\2\2ij\7+\2\2j\n\3\2\2\2kl\t")
-        buf.write("\2\2\2l\f\3\2\2\2mn\t\3\2\2n\16\3\2\2\2op\t\4\2\2p\20")
-        buf.write("\3\2\2\2qr\7>\2\2rs\7v\2\2st\7{\2\2tu\7r\2\2uv\7u\2\2")
-        buf.write("vw\7v\2\2wx\7a\2\2xy\7o\2\2yz\7c\2\2z{\7v\2\2{|\7j\2\2")
-        buf.write("|}\7a\2\2}~\7u\2\2~\177\7v\2\2\177\u0080\7c\2\2\u0080")
-        buf.write("\u0081\7t\2\2\u0081\u0082\7v\2\2\u0082\u0083\7@\2\2\u0083")
-        buf.write("\22\3\2\2\2\u0084\u0085\7>\2\2\u0085\u0086\7v\2\2\u0086")
-        buf.write("\u0087\7{\2\2\u0087\u0088\7r\2\2\u0088\u0089\7u\2\2\u0089")
-        buf.write("\u008a\7v\2\2\u008a\u008b\7a\2\2\u008b\u008c\7o\2\2\u008c")
-        buf.write("\u008d\7c\2\2\u008d\u008e\7v\2\2\u008e\u008f\7j\2\2\u008f")
-        buf.write("\u0090\7a\2\2\u0090\u0091\7g\2\2\u0091\u0092\7p\2\2\u0092")
-        buf.write("\u0093\7f\2\2\u0093\u0094\7@\2\2\u0094\24\3\2\2\2\u0095")
-        buf.write("\u0097\5\13\6\2\u0096\u0095\3\2\2\2\u0097\u0098\3\2\2")
-        buf.write("\2\u0098\u0096\3\2\2\2\u0098\u0099\3\2\2\2\u0099\u009a")
-        buf.write("\3\2\2\2\u009a\u009b\b\13\2\2\u009b\26\3\2\2\2\u009c\u009d")
-        buf.write("\t\5\2\2\u009d\u009e\3\2\2\2\u009e\u009f\b\f\2\2\u009f")
-        buf.write("\30\3\2\2\2\u00a0\u00a1\7*\2\2\u00a1\32\3\2\2\2\u00a2")
-        buf.write("\u00a3\7+\2\2\u00a3\34\3\2\2\2\u00a4\u00a5\7}\2\2\u00a5")
-        buf.write("\36\3\2\2\2\u00a6\u00a7\7\177\2\2\u00a7 \3\2\2\2\u00a8")
-        buf.write("\u00a9\7]\2\2\u00a9\"\3\2\2\2\u00aa\u00ab\7_\2\2\u00ab")
-        buf.write("$\3\2\2\2\u00ac\u00ad\7~\2\2\u00ad&\3\2\2\2\u00ae\u00af")
-        buf.write("\7$\2\2\u00af\u00b0\7~\2\2\u00b0\u00b5\7$\2\2\u00b1\u00b2")
-        buf.write("\7d\2\2\u00b2\u00b3\7c\2\2\u00b3\u00b5\7t\2\2\u00b4\u00ae")
-        buf.write("\3\2\2\2\u00b4\u00b1\3\2\2\2\u00b5(\3\2\2\2\u00b6\u00b7")
-        buf.write("\7$\2\2\u00b7*\3\2\2\2\u00b8\u00b9\7a\2\2\u00b9,\3\2\2")
-        buf.write("\2\u00ba\u00bb\7`\2\2\u00bb.\3\2\2\2\u00bc\u00bd\7=\2")
-        buf.write("\2\u00bd\60\3\2\2\2\u00be\u00bf\7.\2\2\u00bf\62\3\2\2")
-        buf.write("\2\u00c0\u00c1\7\60\2\2\u00c1\64\3\2\2\2\u00c2\u00c3\7")
-        buf.write("/\2\2\u00c3\u00c4\7@\2\2\u00c4\66\3\2\2\2\u00c5\u00d0")
-        buf.write("\7?\2\2\u00c6\u00c7\7?\2\2\u00c7\u00d0\7?\2\2\u00c8\u00c9")
-        buf.write("\7#\2\2\u00c9\u00d0\7?\2\2\u00ca\u00d0\t\6\2\2\u00cb\u00cc")
-        buf.write("\7>\2\2\u00cc\u00d0\7?\2\2\u00cd\u00ce\7@\2\2\u00ce\u00d0")
-        buf.write("\7?\2\2\u00cf\u00c5\3\2\2\2\u00cf\u00c6\3\2\2\2\u00cf")
-        buf.write("\u00c8\3\2\2\2\u00cf\u00ca\3\2\2\2\u00cf\u00cb\3\2\2\2")
-        buf.write("\u00cf\u00cd\3\2\2\2\u00d08\3\2\2\2\u00d1\u00d2\t\7\2")
-        buf.write("\2\u00d2:\3\2\2\2\u00d3\u00d7\t\b\2\2\u00d4\u00d5\7^\2")
-        buf.write("\2\u00d5\u00d7\7\61\2\2\u00d6\u00d3\3\2\2\2\u00d6\u00d4")
-        buf.write("\3\2\2\2\u00d7<\3\2\2\2\u00d8\u00d9\t\t\2\2\u00d9>\3\2")
-        buf.write("\2\2\u00da\u00db\7>\2\2\u00db\u00dc\7v\2\2\u00dc\u00dd")
-        buf.write("\7{\2\2\u00dd\u00de\7r\2\2\u00de\u00df\7u\2\2\u00df\u00e0")
-        buf.write("\7v\2\2\u00e0\u00e1\7a\2\2\u00e1\u00e2\7o\2\2\u00e2\u00e3")
-        buf.write("\7c\2\2\u00e3\u00e4\7v\2\2\u00e4\u00e5\7j\2\2\u00e5\u00e6")
-        buf.write("\7a\2\2\u00e6\u00e7\7c\2\2\u00e7\u00e8\7e\2\2\u00e8\u00e9")
-        buf.write("\7e\2\2\u00e9\u00ea\7g\2\2\u00ea\u00eb\7p\2\2\u00eb\u00ec")
-        buf.write("\7v\2\2\u00ec\u00ed\7@\2\2\u00ed@\3\2\2\2\u00ee\u00ef")
-        buf.write("\7>\2\2\u00ef\u00f0\7v\2\2\u00f0\u00f1\7{\2\2\u00f1\u00f2")
-        buf.write("\7r\2\2\u00f2\u00f3\7u\2\2\u00f3\u00f4\7v\2\2\u00f4\u00f5")
-        buf.write("\7a\2\2\u00f5\u00f6\7o\2\2\u00f6\u00f7\7c\2\2\u00f7\u00f8")
-        buf.write("\7v\2\2\u00f8\u00f9\7j\2\2\u00f9\u00fa\7a\2\2\u00fa\u00fb")
-        buf.write("\7t\2\2\u00fb\u00fc\7g\2\2\u00fc\u00fd\7f\2\2\u00fd\u00fe")
-        buf.write("\7w\2\2\u00fe\u00ff\7e\2\2\u00ff\u0100\7g\2\2\u0100\u0101")
-        buf.write("\7@\2\2\u0101B\3\2\2\2\u0102\u0103\7>\2\2\u0103\u0104")
-        buf.write("\7v\2\2\u0104\u0105\7{\2\2\u0105\u0106\7r\2\2\u0106\u0107")
-        buf.write("\7u\2\2\u0107\u0108\7v\2\2\u0108\u0109\7a\2\2\u0109\u010a")
-        buf.write("\7o\2\2\u010a\u010b\7c\2\2\u010b\u010c\7v\2\2\u010c\u010d")
-        buf.write("\7j\2\2\u010d\u010e\7a\2\2\u010e\u010f\7h\2\2\u010f\u0110")
-        buf.write("\7w\2\2\u0110\u0111\7p\2\2\u0111\u0112\7e\2\2\u0112\u0113")
-        buf.write("\7@\2\2\u0113D\3\2\2\2\u0114\u0115\7>\2\2\u0115\u0116")
-        buf.write("\7v\2\2\u0116\u0117\7{\2\2\u0117\u0118\7r\2\2\u0118\u0119")
-        buf.write("\7u\2\2\u0119\u011a\7v\2\2\u011a\u011b\7a\2\2\u011b\u011c")
-        buf.write("\7o\2\2\u011c\u011d\7c\2\2\u011d\u011e\7v\2\2\u011e\u011f")
-        buf.write("\7j\2\2\u011f\u0120\7a\2\2\u0120\u0121\7o\2\2\u0121\u0122")
-        buf.write("\7c\2\2\u0122\u0123\7v\2\2\u0123\u0124\7@\2\2\u0124F\3")
-        buf.write("\2\2\2\u0125\u0126\7n\2\2\u0126\u0127\7k\2\2\u0127\u0128")
-        buf.write("\7o\2\2\u0128H\3\2\2\2\u0129\u012a\7n\2\2\u012a\u012b")
-        buf.write("\7q\2\2\u012b\u012c\7i\2\2\u012cJ\3\2\2\2\u012d\u012e")
-        buf.write("\7k\2\2\u012e\u012f\7p\2\2\u012f\u0130\7v\2\2\u0130\u0131")
-        buf.write("\7g\2\2\u0131\u0132\7i\2\2\u0132\u0133\7t\2\2\u0133\u0134")
-        buf.write("\7c\2\2\u0134\u0135\7n\2\2\u0135L\3\2\2\2\u0136\u0137")
-        buf.write("\7f\2\2\u0137\u0138\7k\2\2\u0138\u0139\7h\2\2\u0139N\3")
+        buf.write("\4&\t&\4\'\t\'\4(\t(\4)\t)\4*\t*\4+\t+\4,\t,\3\2\3\2\3")
+        buf.write("\2\3\3\3\3\3\3\3\3\3\3\3\4\3\4\3\4\3\4\3\4\3\5\3\5\3\5")
+        buf.write("\3\5\3\5\3\5\3\5\3\6\3\6\3\7\3\7\3\b\3\b\3\t\3\t\3\n\3")
+        buf.write("\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n\3\n")
+        buf.write("\3\n\3\n\3\n\3\n\3\13\3\13\3\13\3\13\3\13\3\13\3\13\3")
+        buf.write("\13\3\13\3\13\3\13\3\13\3\13\3\13\3\13\3\13\3\13\3\f\6")
+        buf.write("\f\u009b\n\f\r\f\16\f\u009c\3\f\3\f\3\r\3\r\3\r\3\r\3")
+        buf.write("\16\3\16\3\17\3\17\3\20\3\20\3\21\3\21\3\22\3\22\3\23")
+        buf.write("\3\23\3\24\3\24\3\25\3\25\3\25\3\25\3\25\3\25\5\25\u00b9")
+        buf.write("\n\25\3\26\3\26\3\27\3\27\3\30\3\30\3\31\3\31\3\32\3\32")
+        buf.write("\3\33\3\33\3\34\3\34\3\34\3\35\3\35\3\35\3\35\3\35\3\35")
+        buf.write("\3\35\3\35\3\35\3\35\5\35\u00d4\n\35\3\36\3\36\3\37\3")
+        buf.write("\37\3\37\5\37\u00db\n\37\3 \3 \3!\3!\3!\3!\3!\3!\3!\3")
+        buf.write("!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3!\3\"\3\"\3\"\3\"")
+        buf.write("\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3\"\3")
+        buf.write("\"\3\"\3\"\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3")
+        buf.write("#\3#\3#\3#\3$\3$\3$\3$\3$\3$\3$\3$\3$\3$\3$\3$\3$\3$\3")
+        buf.write("$\3$\3$\3%\3%\3%\3%\3&\3&\3&\3&\3\'\3\'\3\'\3\'\3\'\3")
+        buf.write("\'\3\'\3\'\3\'\3(\3(\3(\3(\3)\3)\3)\3)\3)\3*\3*\3*\3*")
+        buf.write("\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3*\3")
+        buf.write("*\3*\3*\3*\3+\6+\u015e\n+\r+\16+\u015f\3+\3+\3+\3+\3+")
+        buf.write("\7+\u0167\n+\f+\16+\u016a\13+\3+\7+\u016d\n+\f+\16+\u0170")
+        buf.write("\13+\3+\3+\3+\3+\3+\7+\u0177\n+\f+\16+\u017a\13+\3+\3")
+        buf.write("+\7+\u017e\n+\f+\16+\u0181\13+\5+\u0183\n+\3,\5,\u0186")
+        buf.write("\n,\3,\3,\3,\7,\u018b\n,\f,\16,\u018e\13,\3,\3,\3,\3,")
+        buf.write("\7,\u0194\n,\f,\16,\u0197\13,\7,\u0199\n,\f,\16,\u019c")
+        buf.write("\13,\3,\3,\2\2-\3\3\5\4\7\5\t\6\13\2\r\2\17\2\21\2\23")
+        buf.write("\7\25\b\27\t\31\n\33\13\35\f\37\r!\16#\17%\20\'\21)\22")
+        buf.write("+\23-\24/\25\61\26\63\27\65\30\67\319\32;\33=\34?\35A")
+        buf.write("\36C\37E G!I\"K#M$O%Q&S\'U(W)\3\2\n\5\2\13\f\17\17\"\"")
+        buf.write("\3\2\62;\4\2C\\c|\4\2((^^\4\2>>@@\4\2--//\4\2,,\61\61")
+        buf.write("\4\2##\'\'\2\u01ae\2\3\3\2\2\2\2\5\3\2\2\2\2\7\3\2\2\2")
+        buf.write("\2\t\3\2\2\2\2\23\3\2\2\2\2\25\3\2\2\2\2\27\3\2\2\2\2")
+        buf.write("\31\3\2\2\2\2\33\3\2\2\2\2\35\3\2\2\2\2\37\3\2\2\2\2!")
+        buf.write("\3\2\2\2\2#\3\2\2\2\2%\3\2\2\2\2\'\3\2\2\2\2)\3\2\2\2")
+        buf.write("\2+\3\2\2\2\2-\3\2\2\2\2/\3\2\2\2\2\61\3\2\2\2\2\63\3")
+        buf.write("\2\2\2\2\65\3\2\2\2\2\67\3\2\2\2\29\3\2\2\2\2;\3\2\2\2")
+        buf.write("\2=\3\2\2\2\2?\3\2\2\2\2A\3\2\2\2\2C\3\2\2\2\2E\3\2\2")
+        buf.write("\2\2G\3\2\2\2\2I\3\2\2\2\2K\3\2\2\2\2M\3\2\2\2\2O\3\2")
+        buf.write("\2\2\2Q\3\2\2\2\2S\3\2\2\2\2U\3\2\2\2\2W\3\2\2\2\3Y\3")
+        buf.write("\2\2\2\5\\\3\2\2\2\7a\3\2\2\2\tf\3\2\2\2\13m\3\2\2\2\r")
+        buf.write("o\3\2\2\2\17q\3\2\2\2\21s\3\2\2\2\23u\3\2\2\2\25\u0088")
+        buf.write("\3\2\2\2\27\u009a\3\2\2\2\31\u00a0\3\2\2\2\33\u00a4\3")
+        buf.write("\2\2\2\35\u00a6\3\2\2\2\37\u00a8\3\2\2\2!\u00aa\3\2\2")
+        buf.write("\2#\u00ac\3\2\2\2%\u00ae\3\2\2\2\'\u00b0\3\2\2\2)\u00b8")
+        buf.write("\3\2\2\2+\u00ba\3\2\2\2-\u00bc\3\2\2\2/\u00be\3\2\2\2")
+        buf.write("\61\u00c0\3\2\2\2\63\u00c2\3\2\2\2\65\u00c4\3\2\2\2\67")
+        buf.write("\u00c6\3\2\2\29\u00d3\3\2\2\2;\u00d5\3\2\2\2=\u00da\3")
+        buf.write("\2\2\2?\u00dc\3\2\2\2A\u00de\3\2\2\2C\u00f2\3\2\2\2E\u0106")
+        buf.write("\3\2\2\2G\u0118\3\2\2\2I\u0129\3\2\2\2K\u012d\3\2\2\2")
+        buf.write("M\u0131\3\2\2\2O\u013a\3\2\2\2Q\u013e\3\2\2\2S\u0143\3")
+        buf.write("\2\2\2U\u0182\3\2\2\2W\u0185\3\2\2\2YZ\7`\2\2Z[\7V\2\2")
+        buf.write("[\4\3\2\2\2\\]\7`\2\2]^\7v\2\2^_\7q\2\2_`\7r\2\2`\6\3")
+        buf.write("\2\2\2ab\7`\2\2bc\7*\2\2cd\7V\2\2de\7+\2\2e\b\3\2\2\2")
+        buf.write("fg\7`\2\2gh\7*\2\2hi\7v\2\2ij\7q\2\2jk\7r\2\2kl\7+\2\2")
+        buf.write("l\n\3\2\2\2mn\t\2\2\2n\f\3\2\2\2op\t\3\2\2p\16\3\2\2\2")
+        buf.write("qr\t\4\2\2r\20\3\2\2\2st\7%\2\2t\22\3\2\2\2uv\7>\2\2v")
+        buf.write("w\7v\2\2wx\7{\2\2xy\7r\2\2yz\7u\2\2z{\7v\2\2{|\7a\2\2")
+        buf.write("|}\7o\2\2}~\7c\2\2~\177\7v\2\2\177\u0080\7j\2\2\u0080")
+        buf.write("\u0081\7a\2\2\u0081\u0082\7u\2\2\u0082\u0083\7v\2\2\u0083")
+        buf.write("\u0084\7c\2\2\u0084\u0085\7t\2\2\u0085\u0086\7v\2\2\u0086")
+        buf.write("\u0087\7@\2\2\u0087\24\3\2\2\2\u0088\u0089\7>\2\2\u0089")
+        buf.write("\u008a\7v\2\2\u008a\u008b\7{\2\2\u008b\u008c\7r\2\2\u008c")
+        buf.write("\u008d\7u\2\2\u008d\u008e\7v\2\2\u008e\u008f\7a\2\2\u008f")
+        buf.write("\u0090\7o\2\2\u0090\u0091\7c\2\2\u0091\u0092\7v\2\2\u0092")
+        buf.write("\u0093\7j\2\2\u0093\u0094\7a\2\2\u0094\u0095\7g\2\2\u0095")
+        buf.write("\u0096\7p\2\2\u0096\u0097\7f\2\2\u0097\u0098\7@\2\2\u0098")
+        buf.write("\26\3\2\2\2\u0099\u009b\5\13\6\2\u009a\u0099\3\2\2\2\u009b")
+        buf.write("\u009c\3\2\2\2\u009c\u009a\3\2\2\2\u009c\u009d\3\2\2\2")
+        buf.write("\u009d\u009e\3\2\2\2\u009e\u009f\b\f\2\2\u009f\30\3\2")
+        buf.write("\2\2\u00a0\u00a1\t\5\2\2\u00a1\u00a2\3\2\2\2\u00a2\u00a3")
+        buf.write("\b\r\2\2\u00a3\32\3\2\2\2\u00a4\u00a5\7*\2\2\u00a5\34")
+        buf.write("\3\2\2\2\u00a6\u00a7\7+\2\2\u00a7\36\3\2\2\2\u00a8\u00a9")
+        buf.write("\7}\2\2\u00a9 \3\2\2\2\u00aa\u00ab\7\177\2\2\u00ab\"\3")
+        buf.write("\2\2\2\u00ac\u00ad\7]\2\2\u00ad$\3\2\2\2\u00ae\u00af\7")
+        buf.write("_\2\2\u00af&\3\2\2\2\u00b0\u00b1\7~\2\2\u00b1(\3\2\2\2")
+        buf.write("\u00b2\u00b3\7$\2\2\u00b3\u00b4\7~\2\2\u00b4\u00b9\7$")
+        buf.write("\2\2\u00b5\u00b6\7d\2\2\u00b6\u00b7\7c\2\2\u00b7\u00b9")
+        buf.write("\7t\2\2\u00b8\u00b2\3\2\2\2\u00b8\u00b5\3\2\2\2\u00b9")
+        buf.write("*\3\2\2\2\u00ba\u00bb\7$\2\2\u00bb,\3\2\2\2\u00bc\u00bd")
+        buf.write("\7a\2\2\u00bd.\3\2\2\2\u00be\u00bf\7`\2\2\u00bf\60\3\2")
+        buf.write("\2\2\u00c0\u00c1\7=\2\2\u00c1\62\3\2\2\2\u00c2\u00c3\7")
+        buf.write(".\2\2\u00c3\64\3\2\2\2\u00c4\u00c5\7\60\2\2\u00c5\66\3")
+        buf.write("\2\2\2\u00c6\u00c7\7/\2\2\u00c7\u00c8\7@\2\2\u00c88\3")
+        buf.write("\2\2\2\u00c9\u00d4\7?\2\2\u00ca\u00cb\7?\2\2\u00cb\u00d4")
+        buf.write("\7?\2\2\u00cc\u00cd\7#\2\2\u00cd\u00d4\7?\2\2\u00ce\u00d4")
+        buf.write("\t\6\2\2\u00cf\u00d0\7>\2\2\u00d0\u00d4\7?\2\2\u00d1\u00d2")
+        buf.write("\7@\2\2\u00d2\u00d4\7?\2\2\u00d3\u00c9\3\2\2\2\u00d3\u00ca")
+        buf.write("\3\2\2\2\u00d3\u00cc\3\2\2\2\u00d3\u00ce\3\2\2\2\u00d3")
+        buf.write("\u00cf\3\2\2\2\u00d3\u00d1\3\2\2\2\u00d4:\3\2\2\2\u00d5")
+        buf.write("\u00d6\t\7\2\2\u00d6<\3\2\2\2\u00d7\u00db\t\b\2\2\u00d8")
+        buf.write("\u00d9\7^\2\2\u00d9\u00db\7\61\2\2\u00da\u00d7\3\2\2\2")
+        buf.write("\u00da\u00d8\3\2\2\2\u00db>\3\2\2\2\u00dc\u00dd\t\t\2")
+        buf.write("\2\u00dd@\3\2\2\2\u00de\u00df\7>\2\2\u00df\u00e0\7v\2")
+        buf.write("\2\u00e0\u00e1\7{\2\2\u00e1\u00e2\7r\2\2\u00e2\u00e3\7")
+        buf.write("u\2\2\u00e3\u00e4\7v\2\2\u00e4\u00e5\7a\2\2\u00e5\u00e6")
+        buf.write("\7o\2\2\u00e6\u00e7\7c\2\2\u00e7\u00e8\7v\2\2\u00e8\u00e9")
+        buf.write("\7j\2\2\u00e9\u00ea\7a\2\2\u00ea\u00eb\7c\2\2\u00eb\u00ec")
+        buf.write("\7e\2\2\u00ec\u00ed\7e\2\2\u00ed\u00ee\7g\2\2\u00ee\u00ef")
+        buf.write("\7p\2\2\u00ef\u00f0\7v\2\2\u00f0\u00f1\7@\2\2\u00f1B\3")
+        buf.write("\2\2\2\u00f2\u00f3\7>\2\2\u00f3\u00f4\7v\2\2\u00f4\u00f5")
+        buf.write("\7{\2\2\u00f5\u00f6\7r\2\2\u00f6\u00f7\7u\2\2\u00f7\u00f8")
+        buf.write("\7v\2\2\u00f8\u00f9\7a\2\2\u00f9\u00fa\7o\2\2\u00fa\u00fb")
+        buf.write("\7c\2\2\u00fb\u00fc\7v\2\2\u00fc\u00fd\7j\2\2\u00fd\u00fe")
+        buf.write("\7a\2\2\u00fe\u00ff\7t\2\2\u00ff\u0100\7g\2\2\u0100\u0101")
+        buf.write("\7f\2\2\u0101\u0102\7w\2\2\u0102\u0103\7e\2\2\u0103\u0104")
+        buf.write("\7g\2\2\u0104\u0105\7@\2\2\u0105D\3\2\2\2\u0106\u0107")
+        buf.write("\7>\2\2\u0107\u0108\7v\2\2\u0108\u0109\7{\2\2\u0109\u010a")
+        buf.write("\7r\2\2\u010a\u010b\7u\2\2\u010b\u010c\7v\2\2\u010c\u010d")
+        buf.write("\7a\2\2\u010d\u010e\7o\2\2\u010e\u010f\7c\2\2\u010f\u0110")
+        buf.write("\7v\2\2\u0110\u0111\7j\2\2\u0111\u0112\7a\2\2\u0112\u0113")
+        buf.write("\7h\2\2\u0113\u0114\7w\2\2\u0114\u0115\7p\2\2\u0115\u0116")
+        buf.write("\7e\2\2\u0116\u0117\7@\2\2\u0117F\3\2\2\2\u0118\u0119")
+        buf.write("\7>\2\2\u0119\u011a\7v\2\2\u011a\u011b\7{\2\2\u011b\u011c")
+        buf.write("\7r\2\2\u011c\u011d\7u\2\2\u011d\u011e\7v\2\2\u011e\u011f")
+        buf.write("\7a\2\2\u011f\u0120\7o\2\2\u0120\u0121\7c\2\2\u0121\u0122")
+        buf.write("\7v\2\2\u0122\u0123\7j\2\2\u0123\u0124\7a\2\2\u0124\u0125")
+        buf.write("\7o\2\2\u0125\u0126\7c\2\2\u0126\u0127\7v\2\2\u0127\u0128")
+        buf.write("\7@\2\2\u0128H\3\2\2\2\u0129\u012a\7n\2\2\u012a\u012b")
+        buf.write("\7k\2\2\u012b\u012c\7o\2\2\u012cJ\3\2\2\2\u012d\u012e")
+        buf.write("\7n\2\2\u012e\u012f\7q\2\2\u012f\u0130\7i\2\2\u0130L\3")
+        buf.write("\2\2\2\u0131\u0132\7k\2\2\u0132\u0133\7p\2\2\u0133\u0134")
+        buf.write("\7v\2\2\u0134\u0135\7g\2\2\u0135\u0136\7i\2\2\u0136\u0137")
+        buf.write("\7t\2\2\u0137\u0138\7c\2\2\u0138\u0139\7n\2\2\u0139N\3")
         buf.write("\2\2\2\u013a\u013b\7f\2\2\u013b\u013c\7k\2\2\u013c\u013d")
-        buf.write("\7h\2\2\u013d\u013e\7h\2\2\u013eP\3\2\2\2\u013f\u0140")
-        buf.write("\7>\2\2\u0140\u0141\7v\2\2\u0141\u0142\7{\2\2\u0142\u0143")
-        buf.write("\7r\2\2\u0143\u0144\7u\2\2\u0144\u0145\7v\2\2\u0145\u0146")
-        buf.write("\7a\2\2\u0146\u0147\7o\2\2\u0147\u0148\7c\2\2\u0148\u0149")
-        buf.write("\7v\2\2\u0149\u014a\7j\2\2\u014a\u014b\7a\2\2\u014b\u014c")
-        buf.write("\7u\2\2\u014c\u014d\7{\2\2\u014d\u014e\7o\2\2\u014e\u014f")
-        buf.write("\7d\2\2\u014f\u0150\7q\2\2\u0150\u0151\7n\2\2\u0151\u0152")
-        buf.write("\7a\2\2\u0152\u0153\7d\2\2\u0153\u0154\7c\2\2\u0154\u0155")
-        buf.write("\7u\2\2\u0155\u0156\7g\2\2\u0156\u0157\7@\2\2\u0157R\3")
-        buf.write("\2\2\2\u0158\u015a\5\r\7\2\u0159\u0158\3\2\2\2\u015a\u015b")
-        buf.write("\3\2\2\2\u015b\u0159\3\2\2\2\u015b\u015c\3\2\2\2\u015c")
-        buf.write("\u0164\3\2\2\2\u015d\u015e\5\61\31\2\u015e\u015f\5\r\7")
-        buf.write("\2\u015f\u0160\5\r\7\2\u0160\u0161\5\r\7\2\u0161\u0163")
-        buf.write("\3\2\2\2\u0162\u015d\3\2\2\2\u0163\u0166\3\2\2\2\u0164")
-        buf.write("\u0162\3\2\2\2\u0164\u0165\3\2\2\2\u0165\u017e\3\2\2\2")
-        buf.write("\u0166\u0164\3\2\2\2\u0167\u0169\5\r\7\2\u0168\u0167\3")
-        buf.write("\2\2\2\u0169\u016c\3\2\2\2\u016a\u0168\3\2\2\2\u016a\u016b")
-        buf.write("\3\2\2\2\u016b\u0174\3\2\2\2\u016c\u016a\3\2\2\2\u016d")
-        buf.write("\u016e\5\61\31\2\u016e\u016f\5\r\7\2\u016f\u0170\5\r\7")
-        buf.write("\2\u0170\u0171\5\r\7\2\u0171\u0173\3\2\2\2\u0172\u016d")
-        buf.write("\3\2\2\2\u0173\u0176\3\2\2\2\u0174\u0172\3\2\2\2\u0174")
-        buf.write("\u0175\3\2\2\2\u0175\u0177\3\2\2\2\u0176\u0174\3\2\2\2")
-        buf.write("\u0177\u0179\5\63\32\2\u0178\u017a\5\r\7\2\u0179\u0178")
-        buf.write("\3\2\2\2\u017a\u017b\3\2\2\2\u017b\u0179\3\2\2\2\u017b")
-        buf.write("\u017c\3\2\2\2\u017c\u017e\3\2\2\2\u017d\u0159\3\2\2\2")
-        buf.write("\u017d\u016a\3\2\2\2\u017eT\3\2\2\2\u017f\u0184\5\17\b")
-        buf.write("\2\u0180\u0183\5\17\b\2\u0181\u0183\5\r\7\2\u0182\u0180")
-        buf.write("\3\2\2\2\u0182\u0181\3\2\2\2\u0183\u0186\3\2\2\2\u0184")
-        buf.write("\u0182\3\2\2\2\u0184\u0185\3\2\2\2\u0185\u0192\3\2\2\2")
-        buf.write("\u0186\u0184\3\2\2\2\u0187\u0188\5\63\32\2\u0188\u018d")
-        buf.write("\5\17\b\2\u0189\u018c\5\17\b\2\u018a\u018c\5\r\7\2\u018b")
-        buf.write("\u0189\3\2\2\2\u018b\u018a\3\2\2\2\u018c\u018f\3\2\2\2")
-        buf.write("\u018d\u018b\3\2\2\2\u018d\u018e\3\2\2\2\u018e\u0191\3")
-        buf.write("\2\2\2\u018f\u018d\3\2\2\2\u0190\u0187\3\2\2\2\u0191\u0194")
-        buf.write("\3\2\2\2\u0192\u0190\3\2\2\2\u0192\u0193\3\2\2\2\u0193")
-        buf.write("\u0195\3\2\2\2\u0194\u0192\3\2\2\2\u0195\u0196\b+\3\2")
-        buf.write("\u0196V\3\2\2\2\22\2\u0098\u00b4\u00cf\u00d6\u015b\u0164")
-        buf.write("\u016a\u0174\u017b\u017d\u0182\u0184\u018b\u018d\u0192")
-        buf.write("\4\b\2\2\3+\2")
+        buf.write("\7h\2\2\u013dP\3\2\2\2\u013e\u013f\7f\2\2\u013f\u0140")
+        buf.write("\7k\2\2\u0140\u0141\7h\2\2\u0141\u0142\7h\2\2\u0142R\3")
+        buf.write("\2\2\2\u0143\u0144\7>\2\2\u0144\u0145\7v\2\2\u0145\u0146")
+        buf.write("\7{\2\2\u0146\u0147\7r\2\2\u0147\u0148\7u\2\2\u0148\u0149")
+        buf.write("\7v\2\2\u0149\u014a\7a\2\2\u014a\u014b\7o\2\2\u014b\u014c")
+        buf.write("\7c\2\2\u014c\u014d\7v\2\2\u014d\u014e\7j\2\2\u014e\u014f")
+        buf.write("\7a\2\2\u014f\u0150\7u\2\2\u0150\u0151\7{\2\2\u0151\u0152")
+        buf.write("\7o\2\2\u0152\u0153\7d\2\2\u0153\u0154\7q\2\2\u0154\u0155")
+        buf.write("\7n\2\2\u0155\u0156\7a\2\2\u0156\u0157\7d\2\2\u0157\u0158")
+        buf.write("\7c\2\2\u0158\u0159\7u\2\2\u0159\u015a\7g\2\2\u015a\u015b")
+        buf.write("\7@\2\2\u015bT\3\2\2\2\u015c\u015e\5\r\7\2\u015d\u015c")
+        buf.write("\3\2\2\2\u015e\u015f\3\2\2\2\u015f\u015d\3\2\2\2\u015f")
+        buf.write("\u0160\3\2\2\2\u0160\u0168\3\2\2\2\u0161\u0162\5\63\32")
+        buf.write("\2\u0162\u0163\5\r\7\2\u0163\u0164\5\r\7\2\u0164\u0165")
+        buf.write("\5\r\7\2\u0165\u0167\3\2\2\2\u0166\u0161\3\2\2\2\u0167")
+        buf.write("\u016a\3\2\2\2\u0168\u0166\3\2\2\2\u0168\u0169\3\2\2\2")
+        buf.write("\u0169\u0183\3\2\2\2\u016a\u0168\3\2\2\2\u016b\u016d\5")
+        buf.write("\r\7\2\u016c\u016b\3\2\2\2\u016d\u0170\3\2\2\2\u016e\u016c")
+        buf.write("\3\2\2\2\u016e\u016f\3\2\2\2\u016f\u0178\3\2\2\2\u0170")
+        buf.write("\u016e\3\2\2\2\u0171\u0172\5\63\32\2\u0172\u0173\5\r\7")
+        buf.write("\2\u0173\u0174\5\r\7\2\u0174\u0175\5\r\7\2\u0175\u0177")
+        buf.write("\3\2\2\2\u0176\u0171\3\2\2\2\u0177\u017a\3\2\2\2\u0178")
+        buf.write("\u0176\3\2\2\2\u0178\u0179\3\2\2\2\u0179\u017b\3\2\2\2")
+        buf.write("\u017a\u0178\3\2\2\2\u017b\u017f\5\65\33\2\u017c\u017e")
+        buf.write("\5\r\7\2\u017d\u017c\3\2\2\2\u017e\u0181\3\2\2\2\u017f")
+        buf.write("\u017d\3\2\2\2\u017f\u0180\3\2\2\2\u0180\u0183\3\2\2\2")
+        buf.write("\u0181\u017f\3\2\2\2\u0182\u015d\3\2\2\2\u0182\u016e\3")
+        buf.write("\2\2\2\u0183V\3\2\2\2\u0184\u0186\5\21\t\2\u0185\u0184")
+        buf.write("\3\2\2\2\u0185\u0186\3\2\2\2\u0186\u0187\3\2\2\2\u0187")
+        buf.write("\u018c\5\17\b\2\u0188\u018b\5\17\b\2\u0189\u018b\5\r\7")
+        buf.write("\2\u018a\u0188\3\2\2\2\u018a\u0189\3\2\2\2\u018b\u018e")
+        buf.write("\3\2\2\2\u018c\u018a\3\2\2\2\u018c\u018d\3\2\2\2\u018d")
+        buf.write("\u019a\3\2\2\2\u018e\u018c\3\2\2\2\u018f\u0190\5\65\33")
+        buf.write("\2\u0190\u0195\5\17\b\2\u0191\u0194\5\17\b\2\u0192\u0194")
+        buf.write("\5\r\7\2\u0193\u0191\3\2\2\2\u0193\u0192\3\2\2\2\u0194")
+        buf.write("\u0197\3\2\2\2\u0195\u0193\3\2\2\2\u0195\u0196\3\2\2\2")
+        buf.write("\u0196\u0199\3\2\2\2\u0197\u0195\3\2\2\2\u0198\u018f\3")
+        buf.write("\2\2\2\u0199\u019c\3\2\2\2\u019a\u0198\3\2\2\2\u019a\u019b")
+        buf.write("\3\2\2\2\u019b\u019d\3\2\2\2\u019c\u019a\3\2\2\2\u019d")
+        buf.write("\u019e\b,\3\2\u019eX\3\2\2\2\23\2\u009c\u00b8\u00d3\u00da")
+        buf.write("\u015f\u0168\u016e\u0178\u017f\u0182\u0185\u018a\u018c")
+        buf.write("\u0193\u0195\u019a\4\b\2\2\3,\2")
         return buf.getvalue()
 
 
 class TypstGrammarLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
@@ -243,21 +247,22 @@
             "L_BRACE", "R_BRACE", "L_BRACKET", "R_BRACKET", "BAR", "EVAL_BAR", 
             "QUOTE", "UNDERSCORE", "CARET", "SEMICOLON", "COMMA", "PERIOD", 
             "LIM_APPROACH_SYM", "RELATION_OP", "ADDITIVE_OP", "MP_OP", "POSTFIX_OP", 
             "ACCENT_OP", "REDUCE_OP", "FUNC", "FUNC_MAT", "FUNC_LIM", "FUNC_LOG", 
             "FUNC_INTEGRAL", "DIF", "DIFF", "SYMBOL_BASE", "NUMBER", "ID" ]
 
     ruleNames = [ "T__0", "T__1", "T__2", "T__3", "WS_CHAR", "DIGIT", "LETTER", 
-                  "MATH_START", "MATH_END", "WS", "USELESS_SIGN", "L_PAREN", 
-                  "R_PAREN", "L_BRACE", "R_BRACE", "L_BRACKET", "R_BRACKET", 
-                  "BAR", "EVAL_BAR", "QUOTE", "UNDERSCORE", "CARET", "SEMICOLON", 
-                  "COMMA", "PERIOD", "LIM_APPROACH_SYM", "RELATION_OP", 
-                  "ADDITIVE_OP", "MP_OP", "POSTFIX_OP", "ACCENT_OP", "REDUCE_OP", 
-                  "FUNC", "FUNC_MAT", "FUNC_LIM", "FUNC_LOG", "FUNC_INTEGRAL", 
-                  "DIF", "DIFF", "SYMBOL_BASE", "NUMBER", "ID" ]
+                  "HASHTAG", "MATH_START", "MATH_END", "WS", "USELESS_SIGN", 
+                  "L_PAREN", "R_PAREN", "L_BRACE", "R_BRACE", "L_BRACKET", 
+                  "R_BRACKET", "BAR", "EVAL_BAR", "QUOTE", "UNDERSCORE", 
+                  "CARET", "SEMICOLON", "COMMA", "PERIOD", "LIM_APPROACH_SYM", 
+                  "RELATION_OP", "ADDITIVE_OP", "MP_OP", "POSTFIX_OP", "ACCENT_OP", 
+                  "REDUCE_OP", "FUNC", "FUNC_MAT", "FUNC_LIM", "FUNC_LOG", 
+                  "FUNC_INTEGRAL", "DIF", "DIFF", "SYMBOL_BASE", "NUMBER", 
+                  "ID" ]
 
     grammarFileName = "TypstGrammar.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.7.2")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
@@ -276,15 +281,15 @@
         else:
             raise Exception("Unknown ID: " + self.text)
 
 
     def action(self, localctx:RuleContext, ruleIndex:int, actionIndex:int):
         if self._actions is None:
             actions = dict()
-            actions[41] = self.ID_action 
+            actions[42] = self.ID_action 
             self._actions = actions
         action = self._actions.get(ruleIndex, None)
         if action is not None:
             action(localctx, actionIndex)
         else:
             raise Exception("No registered action for:" + str(ruleIndex))
```

## Comparing `typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.8.dist-info/METADATA` & `typst_sympy_calculator-0.5.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.8
+Version: 0.5.0
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -70,23 +70,29 @@
 
     - [x] **Common Functions:** `gcd`, `lcm`, `floor`, `ceil`, `max`, `min`, `log`, `ln`, `exp`, `sin`, `cos`, `tan`, `csc`, `sec`, `cot`, `arcsin`, `sinh`, `arsinh`, etc...
 
     - [x] **Funcion Symbol:** `f(x)`, `f(x-1,)`, `g(x,y)`, etc...
 
     - [x] **Calculous:** Limit `lim_(x -> oo) 1/x`, Integration `integral_1^2 x dif x`, etc...
 
-    - [ ] **Calculous:** Derivation (`dif/(dif x) (x^2 + 1)`), etc...
+    - [x] **Calculous:** Derivation (`dif/(dif x) (x^2 + 1)` is not supported, but you can use `derivative(expr, var)` instead), etc...
 
-    - [ ] **Reduce:** Sum `sum_(k=1)^oo (1/2)^k`, Product `product_(k=1)^oo (1/2)^k`
+    - [x] **Reduce:** Sum `sum_(k=1)^oo (1/2)^k`, Product `product_(k=1)^oo (1/2)^k`, etc...
+
+    - [x] **Eval At:** Evalat `x^2 bar_(x = 2)`, `x^2 "|"_(x = 2)`, etc...
 
     - [x] **Linear Algebra:** Matrix to raw echelon form `rref`, Determinant `det`, Transpose `^T`, Inverse `^(-1)`, etc...
 
     - [x] **Relations:** `==`, `>`, `>=`, `<`, `<=`, etc...
 
-    - [ ] **Solve Equation:** Single Equation `x + 1 = 2`, Multiple Equations `cases(x + y = 1, x - y = 2)`, etc...
+    - [x] **Solve Equation:** Single Equation `x + 1 = 2`, Multiple Equations `cases(x + y = 1, x - y = 2)`, etc...
+
+    - [ ] **Logical:** `and`, `or`, `not`, etc...
+
+    - [ ] **Set Theory:** `in`, `sect`, `union`, `subset`, etc...
 
     - [x] **Other:** Binomial `binom(n, k)` ...
 
 - **Custom Math (in typst file):**
 
     - [x] **Define Accents:** `#let acc(x) = math.accent(x, math.grave)`
 
@@ -302,14 +308,30 @@
 
 print(expr)  # 2 f(1)
 
 expr = server.simplify('xy + mail + mail.stamped', typst_file)
 
 print(expr)  # mail + mail.stamped + xy
 
+expr = server.solve('x + y + z = 1')
+
+print(expr)  # y = -x - z + 1, z = -x - y + 1, x = -y - z + 1
+
+expr = server.solve('cases(x + y + z = 1, x = 2)')
+
+print(expr)  # cases(x = 2, z = -y - 1), cases(y = -z - 1, x = 2), y = -x - z + 1, z = -x - y + 1
+
+expr = server.solve('cases(x^2 + y = 4, y = 2)')
+
+print(expr)  # x = sqrt(4 - y), cases(y = 2, x = sqrt(2)), cases(y = 2, x = -sqrt(2)), x = -sqrt(4 - y)
+
+expr = server.solve('cases(x < 2, x > 1)')
+
+print(expr)  # 1 < x and x < 2
+
 ```
 
 
 
 and the typst files `tests/test.typ`
 
 
@@ -638,28 +660,48 @@
 
 - `@additive_op()`: Define a additive operator, receive args `a` and `b`;
 
 - `@mp_op()`: Define a multiplicative operator, receive args `a` and `b`;
 
 - `@postfix_op()`: Define a postfix operator, receive args `a`;
 
-- `@reduce_op()`: Define a reduce operator, NOT IMPLEMENTED YET;
+- `@reduce_op()`: Define a reduce operator, receive args `expr` and `args = (symbol, sub, sup)`;
 
 
 
 It is important that the function name MUST be `def convert_{operator_name}`, or you can use decorator arg `@func(name='operator_name')`, and the substring `_dot_` will be replaced by `.`.
 
 
 
 There are some examples (from [DefaultTypstCalculator.py](https://github.com/OrangeX4/typst-sympy-calculator/blob/main/DefaultTypstCalculator.py)):
 
 
 
 ```python
 
+# Functions
+
+@func()
+
+def convert_binom(n, k):
+
+    return sympy.binomial(n, k)
+
+
+
+# Matrix
+
+@func_mat()
+
+def convert_mat(mat):
+
+    return sympy.Matrix(mat)
+
+
+
 # Constants
 
 @constant()
 
 def convert_oo():
 
     return sympy.oo
@@ -702,31 +744,23 @@
 
 def convert_degree(expr):
 
     return expr / 180 * sympy.pi
 
 
 
-# Matrix
-
-@func_mat()
-
-def convert_mat(mat):
-
-    return sympy.Matrix(mat)
+# Reduces
 
+@reduce_op()
 
+def convert_sum(expr, args):
 
-# Functions
+    # symbol, sub, sup = args
 
-@func()
-
-def convert_binom(n, k):
-
-    return sympy.binomial(n, k)
+    return sympy.Sum(expr, args)
 
 ```
```

## Comparing `typst_sympy_calculator-0.4.8.dist-info/RECORD` & `typst_sympy_calculator-0.5.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-DefaultTypstCalculator.py,sha256=SpwQmZJ3SCXlFTFbXdD1e3nPywwzVztrlYCFEhzxd34,7111
-TypstCalculator.py,sha256=bfCf1g_vPkTDBp3gi8uVwmuybG3HJEspF226CcqVhiI,4242
-TypstCalculatorServer.py,sha256=3AQJaTIKi3c6CfdUBSzJYjAmo3fhbujByMrHHPI0B-c,11376
-TypstConverter.py,sha256=fPh9d66rUDSspOKVvvdi5ZO0GYr74T2v2gLIKXfqMcI,21135
+DefaultTypstCalculator.py,sha256=BAjiYxf7-_xaMjQxakZD2hEpRTIs8bR39g9eJdgdwKA,7926
+TypstCalculator.py,sha256=4AjhzjT4rx421NYshEa-smQJ-FmRVCsDuNUUh_ly9sA,7683
+TypstCalculatorServer.py,sha256=pMa-igBftbG7LFxa5-BWAU1IyXl6LfHTa1-86Vkch4o,11039
+TypstConverter.py,sha256=wkHDHU4WAaaPf0ieXS8_IrcLQSvvd1PtgDY129nlZIU,25676
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
-gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
+gen/TypstGrammarLexer.py,sha256=GVL1rcChdiQif2X-Fd7qnooKPUWtMCjInIOkJ8rzf7M,17703
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.8.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.8.dist-info/METADATA,sha256=vdhm4AOU-y4ZG-Bf7RDbVNgyXlWpf2LFlYYQycx6K4w,12770
-typst_sympy_calculator-0.4.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.8.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.8.dist-info/RECORD,,
+typst_sympy_calculator-0.5.0.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.5.0.dist-info/METADATA,sha256=0a7opBKKMtc1_buFe5l_4FDRDH3mYS60NtsUdrbqp-8,13675
+typst_sympy_calculator-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.5.0.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.5.0.dist-info/RECORD,,
```

