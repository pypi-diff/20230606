# Comparing `tmp/big_O-0.8.1.tar.gz` & `tmp/big_O-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/big_O-0.8.1.tar", last modified: Wed Jan 24 08:39:22 2018, max compression
+gzip compressed data, was "dist/big_O-0.9.tar", last modified: Mon Oct 29 19:24:53 2018, max compression
```

## Comparing `big_O-0.8.1.tar` & `big_O-0.9.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-01-24 08:39:22.000000 big_O-0.8.1/
--rw-r--r--   0 berkes   (735983909) 1116983699     5525 2018-01-24 08:39:22.000000 big_O-0.8.1/PKG-INFO
--rwxr-xr-x   0 berkes   (735983909) 1116983699      471 2018-01-24 08:39:16.000000 big_O-0.8.1/setup.py
-drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-01-24 08:39:22.000000 big_O-0.8.1/big_o/
--rwxr-xr-x   0 berkes   (735983909) 1116983699     4143 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/complexities.py
-drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-01-24 08:39:22.000000 big_O-0.8.1/big_o/test/
--rwxr-xr-x   0 berkes   (735983909) 1116983699     2944 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/test/test_big_o.py
--rw-r--r--   0 berkes   (735983909) 1116983699        0 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/test/__init__.py
--rw-r--r--   0 berkes   (735983909) 1116983699      528 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/test/test_complexities.py
--rwxr-xr-x   0 berkes   (735983909) 1116983699      211 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/__init__.py
--rwxr-xr-x   0 berkes   (735983909) 1116983699      798 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/datagen.py
--rwxr-xr-x   0 berkes   (735983909) 1116983699     5611 2018-01-23 16:20:43.000000 big_O-0.8.1/big_o/big_o.py
--rwxr-xr-x   0 berkes   (735983909) 1116983699     4317 2018-01-23 16:20:43.000000 big_O-0.8.1/README.rst
+drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-10-29 19:24:53.000000 big_O-0.9/
+-rw-r--r--   0 berkes   (735983909) 1116983699     7026 2018-10-29 19:24:53.000000 big_O-0.9/PKG-INFO
+-rw-r--r--   0 berkes   (735983909) 1116983699       19 2018-01-24 09:00:39.000000 big_O-0.9/MANIFEST.in
+-rwxr-xr-x   0 berkes   (735983909) 1116983699      496 2018-10-29 17:12:10.000000 big_O-0.9/setup.py
+drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-10-29 19:24:53.000000 big_O-0.9/big_o/
+-rwxr-xr-x   0 berkes   (735983909) 1116983699     4167 2018-10-29 17:11:56.000000 big_O-0.9/big_o/complexities.py
+drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-10-29 19:24:53.000000 big_O-0.9/big_o/test/
+-rwxr-xr-x   0 berkes   (735983909) 1116983699     2944 2018-01-23 16:20:43.000000 big_O-0.9/big_o/test/test_big_o.py
+-rw-r--r--   0 berkes   (735983909) 1116983699        0 2018-01-23 16:20:43.000000 big_O-0.9/big_o/test/__init__.py
+-rw-r--r--   0 berkes   (735983909) 1116983699      766 2018-10-29 17:11:56.000000 big_O-0.9/big_o/test/test_complexities.py
+-rwxr-xr-x   0 berkes   (735983909) 1116983699      211 2018-01-23 16:20:43.000000 big_O-0.9/big_o/__init__.py
+-rwxr-xr-x   0 berkes   (735983909) 1116983699      804 2018-10-29 18:27:19.000000 big_O-0.9/big_o/datagen.py
+-rwxr-xr-x   0 berkes   (735983909) 1116983699     5614 2018-10-29 17:11:56.000000 big_O-0.9/big_o/big_o.py
+-rw-r--r--   0 berkes   (735983909) 1116983699       38 2018-10-29 19:24:53.000000 big_O-0.9/setup.cfg
+-rwxr-xr-x   0 berkes   (735983909) 1116983699     5474 2018-10-29 18:27:19.000000 big_O-0.9/README.rst
+drwxr-xr-x   0 berkes   (735983909) 1116983699        0 2018-10-29 19:24:53.000000 big_O-0.9/big_O.egg-info/
+-rw-r--r--   0 berkes   (735983909) 1116983699     7026 2018-10-29 19:24:53.000000 big_O-0.9/big_O.egg-info/PKG-INFO
+-rw-r--r--   0 berkes   (735983909) 1116983699      327 2018-10-29 19:24:53.000000 big_O-0.9/big_O.egg-info/SOURCES.txt
+-rw-r--r--   0 berkes   (735983909) 1116983699        6 2018-10-29 19:24:53.000000 big_O-0.9/big_O.egg-info/requires.txt
+-rw-r--r--   0 berkes   (735983909) 1116983699        6 2018-10-29 19:24:53.000000 big_O-0.9/big_O.egg-info/top_level.txt
+-rw-r--r--   0 berkes   (735983909) 1116983699        1 2018-10-29 19:24:53.000000 big_O-0.9/big_O.egg-info/dependency_links.txt
```

### Comparing `big_O-0.8.1/PKG-INFO` & `big_O-0.9/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,155 @@
-Metadata-Version: 1.0
-Name: big_O
-Version: 0.8.1
-Summary: Empirical estimation of time complexity from execution time
-Home-page: https://github.com/pberkes/big_O
-Author: Pietro Berkes
-Author-email: pietro.berkes@googlemail.com
-License: LICENSE.txt
-Description: =====
-        big_O
-        =====
-        
-        big_O is a Python module to estimate the time complexity of Python code from
-        its execution time.  It can be used to analyze how functions scale with inputs
-        of increasing size.
-        
-        
-        big_O executes a Python function for input of increasing size `N`, and measures
-        its execution time. From the measurements, big_O fits a set of time complexity
-        classes and returns the best fitting class. This is an empirical way to
-        compute the asymptotic class of a function in `"Big-O"
-        <http://en.wikipedia.org/wiki/Big_oh>`_.  notation. (Strictly
-        speaking, we're empirically computing the Big Theta class.)
-        
-        Usage
-        -----
-        
-        For concreteness, let's say we would like to compute the asymptotic behavior
-        of a simple function that finds the maximum element in a list of positive
-        integers:
-        
-            >>> def find_max(x):
-            ...     """Find the maximum element in a list of positive integers."""
-            ...     max_ = 0
-            ...     for el in x:
-            ...         if el > max_:
-            ...             max_ = el
-            ...     return max_
-            ...
-        
-        To do this, we call `big_o.big_o` passing as argument the function and a
-        data generator that provides lists of random integers of length N:
-        
-            >>> import big_o
-            >>> positive_int_generator = lambda n: big_o.datagen.integers(n, 0, 10000)
-            >>> best, others = big_o.big_o(find_max, positive_int_generator, n_repeats=100)
-            >>> print(best)
-            Linear: time = -0.0021 + 4E-06*n
-        
-        `big_o` inferred that the asymptotic behavior of the `find_max` fuction is
-        linear, and returns an object containing the fitted coefficients for the
-        complexity class. The second return argument, `others`, contains a dictionary
-        of all fitted classes with the residuals from the fit as keys:
-        
-            >>> for class_, residuals in others.items():
-            ...     print('{:<60s}    (res: {:.2G})'.format(class_, residuals))
-            ...
-            Logarithmic: time = -0.3 + 0.05*log(n)                      (res: 0.072)
-            Cubic: time = 0.1 + 3.6E-16*n^3                             (res: 0.028)
-            Quadratic: time = 0.068 + 3.8E-11*n^2                       (res: 0.011)
-            Constant: time = 0.2                                        (res: 0.17)
-            Exponential: time = -4.2 * 4.1E-05^n                        (res: 9.6)
-            Linearithmic: time = 0.0077 + 3.5E-07*n*log(n)              (res: 0.00055)
-            Polynomial: time = -11 * x^0.84                             (res: 0.12)
-            Linear: time = -0.0021 + 4E-06*n                            (res: 0.00054)
-        
-        Submodules
-        ----------
-        
-        - `big_o.datagen`: this sub-module contains common data generators, including an identity generator that simply returns N (`datagen.n_`), and a data generator that returns a list of random integers of length N (`datagen.integers`).
-        - `big_o.complexities`: this sub-module defines the complexity classes to be fit to the execution times. Unless you want to define new classes, you don't need to worry about it.
-        
-        
-        Standard library examples
-        -------------------------
-        
-        Sorting a list in Python is O(n*log(n)) (a.k.a. 'linearithmic'):
-        
-            >>> big_o.big_o(sorted, lambda n: big_o.datagen.integers(n, -100, 100))
-            (<big_o.complexities.Linearithmic object at 0x031DA9D0>, ...)
-        
-        Inserting elements at the beginning of a list is O(n):
-        
-            >>> def insert_0(lst):
-            ...     lst.insert(0, 0)
-            ...
-            >>> print big_o.big_o(insert_0, big_o.datagen.range_n, n_repeats=100)[0]
-            Linear: time = 0.00035 + 7.5E-08*n
-        
-        Inserting elements at the beginning of a queue is O(1):
-        
-            >>> from collections import deque
-            >>> def insert_0_queue(queue):
-            ...     lst.insert(0, 0)
-            ...
-            >>> def queue_generator(n):
-            ...      return deque(xrange(n))
-            ...
-            >>> print big_o.big_o(insert_0_queue, queue_generator, n_repeats=100)[0]
-            Constant: time = 0.00012
-        
-        `numpy` examples
-        ----------------
-        
-        Creating an array:
-        
-        - `numpy.zeros` is O(n), since it needs to initialize every element to 0:
-        
-            >>> import numpy as np
-            >>> big_o.big_o(np.zeros, big_o.datagen.n_, max_n=100000, n_repeats=100)
-            (<class 'big_o.big_o.Linear'>, ...)
-        
-        - `numpy.empty` instead just allocates the memory, and is thus O(1):
-        
-            >>> big_o.big_o(np.empty, big_o.datagen.n_, max_n=100000, n_repeats=100)
-            (<class 'big_o.big_o.Constant'> ...)
-        
-        
-        License
-        -------
-        
-        big_O is released under the GPL v3. See LICENSE.txt .
-        
-        Copyright (c) 2011, Pietro Berkes. All rights reserved.
-        
-Platform: UNKNOWN
+=====
+big_O
+=====
+
+big_O is a Python module to estimate the time complexity of Python code from
+its execution time.  It can be used to analyze how functions scale with inputs
+of increasing size.
+
+big_O executes a Python function for input of increasing size `N`, and measures
+its execution time. From the measurements, big_O fits a set of time complexity
+classes and returns the best fitting class. This is an empirical way to
+compute the asymptotic class of a function in `"Big-O"
+<http://en.wikipedia.org/wiki/Big_oh>`_.  notation. (Strictly
+speaking, we're empirically computing the Big Theta class.)
+
+Usage
+-----
+
+For concreteness, let's say we would like to compute the asymptotic behavior
+of a simple function that finds the maximum element in a list of positive
+integers:
+
+    >>> def find_max(x):
+    ...     """Find the maximum element in a list of positive integers."""
+    ...     max_ = 0
+    ...     for el in x:
+    ...         if el > max_:
+    ...             max_ = el
+    ...     return max_
+    ...
+
+To do this, we call `big_o.big_o` passing as argument the function and a
+data generator that provides lists of random integers of length N:
+
+    >>> import big_o
+    >>> positive_int_generator = lambda n: big_o.datagen.integers(n, 0, 10000)
+    >>> best, others = big_o.big_o(find_max, positive_int_generator, n_repeats=100)
+    >>> print(best)
+    Linear: time = -0.00035 + 2.7E-06*n (sec)
+
+`big_o` inferred that the asymptotic behavior of the `find_max` function is
+linear, and returns an object containing the fitted coefficients for the
+complexity class. The second return argument, `others`, contains a dictionary
+of all fitted classes with the residuals from the fit as keys:
+
+    >>> for class_, residuals in others.items():
+    ...     print('{!s:<60s}    (res: {:.2G})'.format(class_, residuals))
+    ...
+    Exponential: time = -5 * 4.6E-05^n (sec)                        (res: 15)
+    Linear: time = -0.00035 + 2.7E-06*n (sec)                       (res: 6.3E-05)
+    Quadratic: time = 0.046 + 2.4E-11*n^2 (sec)                     (res: 0.0056)
+    Linearithmic: time = 0.0061 + 2.3E-07*n*log(n) (sec)            (res: 0.00016)
+    Cubic: time = 0.067 + 2.3E-16*n^3 (sec)                         (res: 0.013)
+    Logarithmic: time = -0.2 + 0.033*log(n) (sec)                   (res: 0.03)
+    Constant: time = 0.13 (sec)                                     (res: 0.071)
+    Polynomial: time = -13 * x^0.98 (sec)                           (res: 0.0056)
+
+Submodules
+----------
+
+- `big_o.datagen`: this sub-module contains common data generators, including
+  an identity generator that simply returns N (`datagen.n_`), and a data
+  generator that returns a list of random integers of length N
+  (`datagen.integers`).
+
+- `big_o.complexities`: this sub-module defines the complexity classes to be
+  fit to the execution times. Unless you want to define new classes, you don't
+  need to worry about it.
+
+
+Standard library examples
+-------------------------
+
+Sorting a list in Python is O(n*log(n)) (a.k.a. 'linearithmic'):
+
+    >>> big_o.big_o(sorted, lambda n: big_o.datagen.integers(n, 10000, 50000))
+    (<big_o.complexities.Linearithmic object at 0x031DA9D0>, ...)
+
+Inserting elements at the beginning of a list is O(n):
+
+    >>> def insert_0(lst):
+    ...     lst.insert(0, 0)
+    ...
+    >>> print(big_o.big_o(insert_0, big_o.datagen.range_n, n_measures=100)[0])
+    Linear: time = -4.2E-06 + 7.9E-10*n (sec)
+
+Inserting elements at the beginning of a queue is O(1):
+
+    >>> from collections import deque
+    >>> def insert_0_queue(queue):
+    ...     queue.insert(0, 0)
+    ...
+    >>> def queue_generator(n):
+    ...      return deque(range(n))
+    ...
+    >>> print(big_o.big_o(insert_0_queue, queue_generator, n_measures=100)[0])
+    Constant: time = 2.2E-06 (sec)
+
+`numpy` examples
+----------------
+
+Creating an array:
+
+- `numpy.zeros` is O(n), since it needs to initialize every element to 0:
+
+    >>> import numpy as np
+    >>> big_o.big_o(np.zeros, big_o.datagen.n_, max_n=100000, n_repeats=100)
+    (<class 'big_o.big_o.Linear'>, ...)
+
+- `numpy.empty` instead just allocates the memory, and is thus O(1):
+
+    >>> big_o.big_o(np.empty, big_o.datagen.n_, max_n=100000, n_repeats=100)
+    (<class 'big_o.big_o.Constant'> ...)
+
+Additional examples
+--------------
+
+We can compare the estimated time complexities of different Fibonacci number
+implementations. The naive implementation is exponential O(2^n). Since this
+implementation is very inefficient we'll reduce the maximum tested n:
+
+    >>> def fib_naive(n):
+    ...     if n < 0:
+    ...         return -1
+    ...     if n < 2:
+    ...         return n
+    ...     return fib_naive(n-1) + fib_naive(n-2)
+    ...
+    >>> print(big_o.big_o(fib_naive, big_o.datagen.n_, n_repeats=20, min_n=2, max_n=25)[0])
+    Exponential: time = -11 * 0.47^n (sec)
+
+A more efficient implementation to find Fibonacci numbers involves using
+dynamic programming and is linear O(n):
+
+    >>> def fib_dp(n):
+    ...     if n < 0:
+    ...         return -1
+    ...     if n < 2:
+    ...         return n
+    ...     a = 0
+    ...     b = 1
+    ...     for i in range(2, n+1):
+    ...         a, b = b, a+b
+    ...     return b
+    ...
+    >>> print(big_o.big_o(fib_dp, big_o.datagen.n_, n_repeats=100, min_n=200, max_n=1000)[0])
+    Linear: time = -1.8E-06 + 7.3E-06*n (sec)
+
+
+License
+-------
+
+big_O is released under BSD-3. See LICENSE.txt .
+
+Copyright (c) 2011-2018, Pietro Berkes. All rights reserved.
```

### Comparing `big_O-0.8.1/big_o/complexities.py` & `big_O-0.9/big_o/complexities.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
         """ Fit complexity class parameters to timing data.
 
         Input:
         ------
 
         n -- Array of values of N for which execution time has been measured.
 
-        t -- Array of execution times for each N in `ns`.
+        t -- Array of execution times for each N in seconds.
 
         Output:
         -------
 
         residuals -- Sum of square errors of fit
         """
         x = self._transform_n(n)
         y = self._transform_time(t)
-        coeff, residuals, rank, s = np.linalg.lstsq(x, y)
+        coeff, residuals, rank, s = np.linalg.lstsq(x, y, rcond=-1)
         self.coeff = coeff
         return residuals[0]
 
     def compute(self, n):
         """ Compute the value of the fitted function at `n`. """
         if self.coeff is None:
             raise NotFittedError()
@@ -51,15 +51,15 @@
         return tot
 
     def __str__(self):
         prefix = '{}: '.format(self.__class__.__name__)
 
         if self.coeff is None:
             return prefix + ': not yet fitted'
-        return prefix + self.format_str().format(*tuple(self.coeff))
+        return prefix + self.format_str().format(*tuple(self.coeff)) + ' (sec)'
 
     # --- abstract methods
 
     @classmethod
     def format_str(cls):
         """ Return a string describing the fitted function.
```

### Comparing `big_O-0.8.1/big_o/test/test_big_o.py` & `big_O-0.9/big_o/test/test_big_o.py`

 * *Files identical despite different names*

### Comparing `big_O-0.8.1/big_o/test/test_complexities.py` & `big_O-0.9/big_o/test/test_complexities.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,15 @@
         linear = complexities.Linear()
         linear.fit(x, y)
         assert_array_almost_equal(linear.compute(x), y, 10)
 
     def test_not_fitted(self):
         linear = complexities.Linear()
         self.assertRaises(complexities.NotFittedError, linear.compute, 100)
+
+    def test_str_includes_units(self):
+        x = np.linspace(10, 100, 100)
+        y = 3.0 * x + 2.0
+        linear = complexities.Linear()
+        linear.fit(x, y)
+        linear_str = str(linear)
+        assert '(sec)' in linear_str
```

### Comparing `big_O-0.8.1/big_o/datagen.py` & `big_O-0.9/big_o/datagen.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def n_(n):
     """ Return N. """
     return n
 
 
 def range_n(n, start=0):
     """ Return the sequence [start, start+1, ..., start+N-1]. """
-    return range(start, start+n)
+    return list(range(start, start+n))
 
 
 def integers(n, min_, max_):
     """ Return sequence of N random integers between min_ and max_ (included).
     """
     return [random.randint(min_, max_) for _ in range(n)]
```

### Comparing `big_O-0.8.1/big_o/big_o.py` & `big_O-0.9/big_o/big_o.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """Infer the complexity class from execution times.
 
     Input:
     ------
 
     ns -- Array of values of N for which execution time has been measured.
 
-    time -- Array of execution times for each N in `ns`.
+    time -- Array of execution times for each N in seconds.
 
     classes -- The complexity classes to consider. This is a list of subclasses
                of `big_o.complexities.ComplexityClass`.
                Default: all the classes in `big_o.complexities.ALL_CLASSES`
 
     verbose -- If True, print parameters and residuals of the fit for each
                complexity class
```

