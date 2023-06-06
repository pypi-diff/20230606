# Comparing `tmp/yarrow_diagrams-0.0.2.1.tar.gz` & `tmp/yarrow_diagrams-0.0.2.2.tar.gz`

## Comparing `yarrow_diagrams-0.0.2.1.tar` & `yarrow_diagrams-0.0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/__init__.py
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/bipartite_multigraph.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/cupy.py
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/diagram.py
--rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/finite_function.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/array/__init__.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/array/cupy.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/array/numpy.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/decompose/frobenius.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/functor/functor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/segmented/__init__.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/segmented/finite_function.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/yarrow/segmented/operations.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/__init__.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/bipartite_multigraph.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/cupy.py
+-rw-r--r--   0        0        0    12819 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/diagram.py
+-rw-r--r--   0        0        0    13057 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/finite_function.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/array/__init__.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/array/cupy.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/array/numpy.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/decompose/frobenius.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/functor/functor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/segmented/__init__.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/segmented/finite_function.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/yarrow/segmented/operations.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 yarrow_diagrams-0.0.2.2/PKG-INFO
```

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/bipartite_multigraph.py` & `yarrow_diagrams-0.0.2.2/yarrow/bipartite_multigraph.py`

 * *Files 24% similar despite different names*

```diff
@@ -173,14 +173,39 @@
             po=f.po + g.po,
             xn=f.xn + g.xn,
         )
 
     def __matmul__(f, g):
         return f.coproduct(g)
 
+    @classmethod
+    def coproduct_list(cls, Gs: 'List[AbstractBipartiteMultigraph]', wn=None, xn=None):
+        """ Compute the coproduct of a list of bipartite multigraphs. O(n) in the size of the result.
+
+        .. warning::
+            Does not speed up to O(log n) in the parallel case.
+        """
+        if len(Gs) == 0:
+            assert wn is not None
+            assert xn is not None
+            return cls.empty(wn, xn)
+
+        # can't specify Σ if Gs is non-empty
+        assert wn is None
+        assert xn is None
+        return cls(
+            wi=cls._Fun.tensor_list([g.wi for g in Gs]),
+            wo=cls._Fun.tensor_list([g.wo for g in Gs]),
+            xi=cls._Fun.tensor_list([g.xi for g in Gs]),
+            xo=cls._Fun.tensor_list([g.xo for g in Gs]),
+            wn=cls._Fun.coproduct_list([g.wn for g in Gs]),
+            pi=cls._Fun.coproduct_list([g.pi for g in Gs]),
+            po=cls._Fun.coproduct_list([g.po for g in Gs]),
+            xn=cls._Fun.coproduct_list([g.xn for g in Gs]))
+
     # Apply a morphism α of bipartite multigraphs whose only
     # non-identity component is α_W = q.
     def coequalize_wires(self, q : AbstractFiniteFunction):
         """
         Apply a morphism α of bipartite multigraphs
         whose only non-identity component α_W = q
         for some coequalizer q.
```

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/cupy.py` & `yarrow_diagrams-0.0.2.2/yarrow/cupy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/diagram.py` & `yarrow_diagrams-0.0.2.2/yarrow/diagram.py`

 * *Files 3% similar despite different names*

```diff
@@ -304,27 +304,51 @@
             s = f.s.inject0(g.G.W) >> q,
             t = g.t.inject1(f.G.W) >> q,
             G = h.G.coequalize_wires(q))
 
     def __rshift__(f, g):
         return f.compose(g)
 
+    # TODO: IMPROVE THIS
+    @classmethod
+    def tensor_list(cls, ds: 'List[AbstractDiagram]', wn=None, xn=None):
+        """ Compute the tensor product of a list of diagrams. O(n) time in the size of the result.
+
+        .. warning::
+            Does not speed up to O(log n) in the parallel case
+        """
+        if len(ds) == 0:
+            assert wn is not None
+            assert xn is not None
+            return Diagram.empty(wn, xn)
+
+        assert wn is None
+        assert xn is None
+        s = cls._Fun.tensor_list([d.s for d in ds])
+        t = cls._Fun.tensor_list([d.t for d in ds])
+        G = cls._Graph.coproduct_list([d.G for d in ds])
+        return Diagram(s, t, G)
+
     @classmethod
     def tensor_operations(cls, ops: Operations):
         pass # hide the docstring for now
         """ Compute the X-fold tensoring of operations
 
+        .. code-block:: text
+
             xn : X → Σ₁
 
         whose typings are given by the segmented finite functions
 
+        .. code-block:: text
+
             s_type : sum_{i ∈ X} arity(xn(i))   → Σ₀
             t_type : sum_{i ∈ X} coarity(xn(i)) → Σ₀
 
-        (This is Proposition 4.13 in the paper)
+        See Proposition 4.13 in :cite:t:`dpafsd`.
         """
         Fun   = cls._Fun
         Array = Fun._Array
 
         xn, s_type, t_type = ops.xn, ops.s_type, ops.t_type
 
         r = Array.arange(0, xn.source)
```

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/finite_function.py` & `yarrow_diagrams-0.0.2.2/yarrow/finite_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,15 +148,15 @@
            and f._Array.all(f.table == g.table)
 
     ################################################################################
     # FiniteFunction has initial objects and coproducts
     @classmethod
     def initial(cls, b, dtype=DTYPE):
         """Compute the initial map ``? : 0 → b``"""
-        return cls(b, cls._Array.zeros(0, dtype=DTYPE))
+        return cls(b, cls._Array.zeros(0, dtype=dtype))
 
     @classmethod
     def inj0(cls, a, b):
         """Compute the injection ``ι₀ : a → a + b``"""
         table = cls._Array.arange(0, a, dtype=DTYPE)
         return cls(a + b, table)
 
@@ -269,27 +269,37 @@
         Return the *stable* sorting permutation     ``p : A → A``
         such that                                   ``p >> f``  is monotonic.
         """
         return type(f)(f.source, f._Array.argsort(f.table))
 
     ################################################################################
     # Sequential-only methods
+
     @classmethod
     def coproduct_list(cls, fs: List['AbstractFiniteFunction'], target=None):
-        """ Compute the coproduct of a list of finite functions with a common target """
+        """ Compute the coproduct of a list of finite functions. O(n) in size of the result.
+
+        .. warning::
+            Does not speed up to O(log n) in the parallel case.
+        """
         # NOTE: this function is not parallelized!
         if len(fs) == 0:
             return cls.initial(0 if target is None else target)
 
         # all targets must be equal
         assert all(f.target == g.target for f, g in zip(fs, fs[:1]))
         return cls(fs[0].target, cls._Array.concatenate([f.table for f in fs]))
 
     @classmethod
     def tensor_list(cls, fs: List['AbstractFiniteFunction']):
+        """ Compute the tensor product of a list of finite functions. O(n) in size of the result.
+
+        .. warning::
+            Does not speed up to O(log n) in the parallel case.
+        """
         if len(fs) == 0:
             return cls.initial(0)
 
         targets = cls._Array.array([f.target for f in fs])
         offsets = cls._Array.zeros(len(targets) + 1, dtype=type(fs[0].source))
         offsets[1:] = cls._Array.cumsum(targets) # exclusive scan
         table = cls._Array.concatenate([f.table + offset for f, offset in zip(fs, offsets[:-1])])
```

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/array/__init__.py` & `yarrow_diagrams-0.0.2.2/yarrow/array/__init__.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/array/cupy.py` & `yarrow_diagrams-0.0.2.2/yarrow/array/cupy.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/array/numpy.py` & `yarrow_diagrams-0.0.2.2/yarrow/array/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :meta hide-value:
 """
 # NOTE: we use :meta hide-value: above because numpy is mocked, so sphinx will
 # have the incorrect value in documentation.
 
 def array(*args, **kwargs):
     kwargs.setdefault('dtype', DEFAULT_DTYPE)
-    return np.array(*args, **kwargs)
+    return np.fromiter(*args, **kwargs)
 
 def max(*args, **kwargs):
     return np.max(*args, **kwargs)
 
 def arange(*args, **kwargs):
     return np.arange(*args, **kwargs)
```

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/decompose/frobenius.py` & `yarrow_diagrams-0.0.2.2/yarrow/decompose/frobenius.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/functor/functor.py` & `yarrow_diagrams-0.0.2.2/yarrow/functor/functor.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,20 +63,20 @@
     decomposition.  """
     # NOTE: it's *very* important that d is a frobenius decomposition, since we
     # directly use the maps d.G.wi and d.G.wo in the result.
     Fun = d._Fun
     Array = Fun._Array
     s_type = SegmentedFiniteFunction(
         sources = bincount(d.G.xi),
-        targets = Fun(None, Array.full(d.operations, d.G.xn.target)),
+        targets = Fun(None, Array.full(d.operations, d.G.xn.target, dtype=d.G.xn.table.dtype)),
         values  = d.G.wi >> d.G.wn)
 
     t_type = SegmentedFiniteFunction(
         sources = bincount(d.G.xo),
-        targets = Fun(None, Array.full(d.operations, d.G.xn.target)),
+        targets = Fun(None, Array.full(d.operations, d.G.xn.target, dtype=d.G.xn.table.dtype)),
         values  = d.G.wo >> d.G.wn)
     
     return Operations(d.G.xn, s_type, t_type)
 
 class FrobeniusFunctor(Functor):
     """ A functor defined in terms of Frobenius decompositions.
     Instead of specifying map_arrow, the implementor can specify map_operations,
@@ -92,22 +92,22 @@
 
         swn = self.map_objects(d.G.wn)
         h = self.map_operations(ops)
 
         Fun   = h._Fun
         Graph = h._Graph
 
-        xn = d._Fun.initial(h.G.xn.target)
+        xn = d._Fun.initial(h.G.xn.target, dtype=h.G.xn.table.dtype)
 
         # build the morphisms (s ; x) ; (id × h) ; (z ; t) from Proposition B.1
         i = Diagram.identity(swn.values, xn)
         # note: we use the source/target maps of i in constructing those of sx, yt
         # to avoid constructing another array with the same data.
-        sx = Diagram(d.s, i.t + map_half_spider(swn, d.G.wi), Graph.discrete(swn.values, xn))
-        yt = Diagram(i.s + map_half_spider(swn, d.G.wo), d.t, Graph.discrete(swn.values, xn))
+        sx = Diagram(map_half_spider(swn, d.s), i.t + map_half_spider(swn, d.G.wi), Graph.discrete(swn.values, xn))
+        yt = Diagram(i.s + map_half_spider(swn, d.G.wo), map_half_spider(swn, d.t), Graph.discrete(swn.values, xn))
         return (sx >> (i @ h) >> yt)
 
     @abstractmethod
     def map_operations(self, ops: Operations) -> Diagram:
         """Given an array of generating operations
 
             xn : X → Σ₁
```

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/segmented/finite_function.py` & `yarrow_diagrams-0.0.2.2/yarrow/segmented/finite_function.py`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/yarrow/segmented/operations.py` & `yarrow_diagrams-0.0.2.2/yarrow/segmented/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     The Operations type is therefore a 3-tuple:
 
     Operation labels
 
       xn         : N            → Σ₁
 
     Source types
-    
+
       s_type
           sources: N            → K₀
           values : sum(sources) → Σ₀      (= max(targets))
           targets: N            → Σ₀      (= const Σ₀+1)
 
     Target types
 
@@ -36,9 +36,10 @@
           targets: N            → Σ₀      (= const Σ₀+1)
 
     The "sources" arrays of s_type and t_type store
     """
     xn: AbstractFiniteFunction
     s_type: AbstractSegmentedFiniteFunction
     t_type: AbstractSegmentedFiniteFunction
+
     def __post_init__(self):
         assert _is_valid(self)
```

### Comparing `yarrow_diagrams-0.0.2.1/LICENSE` & `yarrow_diagrams-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/README.md` & `yarrow_diagrams-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yarrow_diagrams-0.0.2.1/pyproject.toml` & `yarrow_diagrams-0.0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yarrow-diagrams"
-version = "0.0.2.1"
+version = "0.0.2.2"
 authors = [
   { name="Paul Wilson", email="paul@statusfailed.com" }
 ]
 description = "yarrow diagrams"
 readme = "README.md"
 requires-python = ">= 3.7"
 classifiers = [
```

### Comparing `yarrow_diagrams-0.0.2.1/PKG-INFO` & `yarrow_diagrams-0.0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yarrow-diagrams
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: yarrow diagrams
 Project-URL: Homepage, https://yarrow.id
 Project-URL: Github, https://github.com/yarrow-id/diagrams/
 Project-URL: Documentation, https://yarrow-diagrams.readthedocs.io/
 Author-email: Paul Wilson <paul@statusfailed.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

