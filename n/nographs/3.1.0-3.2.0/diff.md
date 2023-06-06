# Comparing `tmp/nographs-3.1.0.tar.gz` & `tmp/nographs-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nographs-3.1.0.tar", last modified: Sun May  7 17:44:16 2023, max compression
+gzip compressed data, was "nographs-3.2.0.tar", last modified: Tue Jun  6 07:00:21 2023, max compression
```

## Comparing `nographs-3.1.0.tar` & `nographs-3.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.787736 nographs-3.1.0/
--rw-rw-rw-   0        0        0     9118 2023-05-07 17:44:16.786736 nographs-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7807 2023-05-07 17:05:23.000000 nographs-3.1.0/README.rst
--rw-rw-rw-   0        0        0      162 2022-11-27 13:28:03.000000 nographs-3.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 17:44:16.787736 nographs-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1876 2023-05-07 17:05:23.000000 nographs-3.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.729657 nographs-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.759736 nographs-3.1.0/src/nographs/
--rw-rw-rw-   0        0        0     7644 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/__init__.py
--rw-rw-rw-   0        0        0    41849 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_bidir_search.py
--rw-rw-rw-   0        0        0      761 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_compatibility.py
--rw-rw-rw-   0        0        0     8188 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_edge_gadgets.py
--rw-rw-rw-   0        0        0    42642 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_gear_collections.py
--rw-rw-rw-   0        0        0    35184 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_gears.py
--rw-rw-rw-   0        0        0    13918 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_matrix_gadgets.py
--rw-rw-rw-   0        0        0     9679 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_path.py
--rw-rw-rw-   0        0        0    19478 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_paths.py
--rw-rw-rw-   0        0        0    13949 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_strategies.py
--rw-rw-rw-   0        0        0   147991 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_traversals.py
--rw-rw-rw-   0        0        0     3232 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_types.py
--rw-rw-rw-   0        0        0        0 2022-11-27 13:28:03.000000 nographs-3.1.0/src/nographs/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.765735 nographs-3.1.0/src/nographs.egg-info/
--rw-rw-rw-   0        0        0     9118 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      834 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.784735 nographs-3.1.0/tests/
--rw-rw-rw-   0        0        0     5033 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_docs_examples.py
--rw-rw-rw-   0        0        0     5963 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_edge_gadgets.py
--rw-rw-rw-   0        0        0    11625 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_gear_collections.py
--rw-rw-rw-   0        0        0     2065 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_gears.py
--rw-rw-rw-   0        0        0     1923 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_matrix_gadgets.py
--rw-rw-rw-   0        0        0     2138 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_nographs.py
--rw-rw-rw-   0        0        0      510 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_path.py
--rw-rw-rw-   0        0        0     5828 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_paths.py
--rw-rw-rw-   0        0        0     2783 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_strategies.py
--rw-rw-rw-   0        0        0   155814 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_traversals_and_searches.py
--rw-rw-rw-   0        0        0     1419 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_types.py
--rw-rw-rw-   0        0        0     3389 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_unit_typed.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.798009 nographs-3.2.0/
+-rw-rw-rw-   0        0        0     9657 2023-06-06 07:00:21.797011 nographs-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8142 2023-06-06 06:52:14.000000 nographs-3.2.0/README.rst
+-rw-rw-rw-   0        0        0      162 2022-11-27 13:28:03.000000 nographs-3.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 07:00:21.798009 nographs-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2100 2023-06-06 06:52:14.000000 nographs-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.646988 nographs-3.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.718495 nographs-3.2.0/src/nographs/
+-rw-rw-rw-   0        0        0     7660 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/__init__.py
+-rw-rw-rw-   0        0        0    41869 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_bidir_search.py
+-rw-rw-rw-   0        0        0      953 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_compatibility.py
+-rw-rw-rw-   0        0        0     8188 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_edge_gadgets.py
+-rw-rw-rw-   0        0        0    42642 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_gear_collections.py
+-rw-rw-rw-   0        0        0    35184 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_gears.py
+-rw-rw-rw-   0        0        0    13918 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_matrix_gadgets.py
+-rw-rw-rw-   0        0        0     9679 2023-05-09 07:48:46.000000 nographs-3.2.0/src/nographs/_path.py
+-rw-rw-rw-   0        0        0    19478 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_paths.py
+-rw-rw-rw-   0        0        0    16057 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_strategies.py
+-rw-rw-rw-   0        0        0   148710 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_traversals.py
+-rw-rw-rw-   0        0        0     3232 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_types.py
+-rw-rw-rw-   0        0        0        0 2022-11-27 13:28:03.000000 nographs-3.2.0/src/nographs/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.724497 nographs-3.2.0/src/nographs.egg-info/
+-rw-rw-rw-   0        0        0     9657 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      834 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.796010 nographs-3.2.0/tests/
+-rw-rw-rw-   0        0        0     5033 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_docs_examples.py
+-rw-rw-rw-   0        0        0     5963 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_edge_gadgets.py
+-rw-rw-rw-   0        0        0    11625 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_gear_collections.py
+-rw-rw-rw-   0        0        0     2065 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_gears.py
+-rw-rw-rw-   0        0        0     1923 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_matrix_gadgets.py
+-rw-rw-rw-   0        0        0     2171 2023-06-06 06:52:14.000000 nographs-3.2.0/tests/test_nographs.py
+-rw-rw-rw-   0        0        0      510 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_path.py
+-rw-rw-rw-   0        0        0     5828 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_paths.py
+-rw-rw-rw-   0        0        0     2783 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_strategies.py
+-rw-rw-rw-   0        0        0   157579 2023-06-06 06:52:14.000000 nographs-3.2.0/tests/test_traversals_and_searches.py
+-rw-rw-rw-   0        0        0     1419 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_types.py
+-rw-rw-rw-   0        0        0     3389 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_unit_typed.py
```

### Comparing `nographs-3.1.0/PKG-INFO` & `nographs-3.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nographs
-Version: 3.1.0
+Version: 3.2.0
 Summary: Graph analysis – the lazy (evaluation) way: Analysis on the fly, for graphs, that are computed and/or adapted on the fly.
 Home-page: https://github.com/HeWeMel/nographs
 Author: Dr. Helmut Melcher
 Author-email: HeWeMel@web.de
 Project-URL: Documentation, https://nographs.readthedocs.io/
 Project-URL: Source, https://github.com/hewemel/nographs/
 Project-URL: Bug Reports, https://github.com/hewemel/nographs/issues
-Keywords: graph,search,traverse,analysis,lazy,infinite,large,adapt
+Keywords: graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,depth,DFS,breadth,BFS,Dijkstra,topological,MST
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
@@ -32,14 +34,17 @@
 
 .. |PyPI status| image:: https://img.shields.io/pypi/status/nographs.svg
    :target: https://pypi.python.org/pypi/nographs/
 
 .. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/nographs.svg
    :target: https://pypi.python.org/pypi/nographs/
 
+.. |PyPy versions| image:: https://img.shields.io/badge/PyPy-3.11-blue
+   :target: https://pypi.python.org/pypi/nographs/
+
 .. |PyPI license| image:: https://img.shields.io/pypi/l/nographs.svg
    :target: https://github.com/HeWeMel/nographs/blob/main/LICENSE
 
 .. |CI| image:: https://github.com/hewemel/nographs/workflows/CI%20(tests,%20flake8,%20mypy)/badge.svg?branch=main
    :target: https://github.com/hewemel/nographs/actions?query=workflow%3ACI%20(pip)
 
 .. |CodeCov| image:: https://img.shields.io/codecov/c/gh/HeWeMel/NoGraphs/main
@@ -74,59 +79,62 @@
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
 **Feature overview**
 
 - Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
 - Bidirectional search algorithms: BFS and Dijkstra.
+- Results: Reachability, depth, distance, paths and trees.
+  Paths can be
+  calculated with vertices, edges, or attributed edges,
+  and can be iterated in both directions.
 - Flexible graph notion:
 
   - Infinite directed multigraphs with loops and
     attributes (this includes
     multiple adjacency, cycles, self-loops,
     directed edges,
     weighted edges and edges with application specific attributes).
   - Infinite graphs are supported, but need to be
     locally finite (i.e., a vertex has only finitely many outgoing edges).
 
-- Generic API. The application can define the following:
+- Generic API:
 
   - Vertices: Can be anything except for None. Hashable vertices can be
     used directly, unhashable vertices can be used together with
     hashable identifiers.
   - Edge weights and distances: Wide range of data types
     supported (float, int, Decimal, mpmath.mpf and others), e.g.,
     for high precision computations.
   - Edge attributes: Any object, e.g, a container
     with further data.
-  - Identity and equivalence of vertices.
+  - Identity and equivalence of vertices can be chosen / defined.
   - Bookkeeping: Several sets of bookkeeping data structures
     are predefined, optimized for different situations (data types used by the
     application, hashing vs. indexing, collections for *Python* objects or *C* native
     data types,...); Adaptable and extendable, e.g., specialized
     collections of 3rd party libraries can be integrated easily and runtime
     efficiently
 
-- Results: Reachability, depth, distance, paths and trees.
-  Paths can be
-  calculated with vertices or edges or attributed edges
-  and can be iterated in both directions.
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
   allows for an API that eases
   operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
   computation of search-aware graphs, and
   traversals of vertex equivalence classes on the fly.
   Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
-- Runtime and memory performance: Have been goals. In its domain, it
-  often even outperforms Rust- and C-based libraries.
+- CI tests: For all supported versions of Python and both supported interpreters
+  CPython and PyPy, both code and docs, 100% code coverage.
+- Runtime and memory performance: Have been goals (CPython). In its domain, it often
+  even outperforms Rust- and C-based libraries.
+  If you need an even higher performance, using PyPy could be an option.
 
 **Documentation**
 
 - `Homepage of the documentation <https://nographs.readthedocs.io>`__
 - `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
 - `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
   (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
```

### Comparing `nographs-3.1.0/README.rst` & `nographs-3.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 .. |PyPI status| image:: https://img.shields.io/pypi/status/nographs.svg
    :target: https://pypi.python.org/pypi/nographs/
 
 .. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/nographs.svg
    :target: https://pypi.python.org/pypi/nographs/
 
+.. |PyPy versions| image:: https://img.shields.io/badge/PyPy-3.11-blue
+   :target: https://pypi.python.org/pypi/nographs/
+
 .. |PyPI license| image:: https://img.shields.io/pypi/l/nographs.svg
    :target: https://github.com/HeWeMel/nographs/blob/main/LICENSE
 
 .. |CI| image:: https://github.com/hewemel/nographs/workflows/CI%20(tests,%20flake8,%20mypy)/badge.svg?branch=main
    :target: https://github.com/hewemel/nographs/actions?query=workflow%3ACI%20(pip)
 
 .. |CodeCov| image:: https://img.shields.io/codecov/c/gh/HeWeMel/NoGraphs/main
@@ -47,59 +50,62 @@
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
 **Feature overview**
 
 - Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
 - Bidirectional search algorithms: BFS and Dijkstra.
+- Results: Reachability, depth, distance, paths and trees.
+  Paths can be
+  calculated with vertices, edges, or attributed edges,
+  and can be iterated in both directions.
 - Flexible graph notion:
 
   - Infinite directed multigraphs with loops and
     attributes (this includes
     multiple adjacency, cycles, self-loops,
     directed edges,
     weighted edges and edges with application specific attributes).
   - Infinite graphs are supported, but need to be
     locally finite (i.e., a vertex has only finitely many outgoing edges).
 
-- Generic API. The application can define the following:
+- Generic API:
 
   - Vertices: Can be anything except for None. Hashable vertices can be
     used directly, unhashable vertices can be used together with
     hashable identifiers.
   - Edge weights and distances: Wide range of data types
     supported (float, int, Decimal, mpmath.mpf and others), e.g.,
     for high precision computations.
   - Edge attributes: Any object, e.g, a container
     with further data.
-  - Identity and equivalence of vertices.
+  - Identity and equivalence of vertices can be chosen / defined.
   - Bookkeeping: Several sets of bookkeeping data structures
     are predefined, optimized for different situations (data types used by the
     application, hashing vs. indexing, collections for *Python* objects or *C* native
     data types,...); Adaptable and extendable, e.g., specialized
     collections of 3rd party libraries can be integrated easily and runtime
     efficiently
 
-- Results: Reachability, depth, distance, paths and trees.
-  Paths can be
-  calculated with vertices or edges or attributed edges
-  and can be iterated in both directions.
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
   allows for an API that eases
   operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
   computation of search-aware graphs, and
   traversals of vertex equivalence classes on the fly.
   Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
-- Runtime and memory performance: Have been goals. In its domain, it
-  often even outperforms Rust- and C-based libraries.
+- CI tests: For all supported versions of Python and both supported interpreters
+  CPython and PyPy, both code and docs, 100% code coverage.
+- Runtime and memory performance: Have been goals (CPython). In its domain, it often
+  even outperforms Rust- and C-based libraries.
+  If you need an even higher performance, using PyPy could be an option.
 
 **Documentation**
 
 - `Homepage of the documentation <https://nographs.readthedocs.io>`__
 - `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
 - `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
   (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
```

### Comparing `nographs-3.1.0/setup.py` & `nographs-3.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.rst').read_text(encoding='utf-8')
 
 setup(
     name="nographs",
-    version="3.1.0",
+    version="3.2.0",
     description=("Graph analysis – the lazy (evaluation) way: Analysis on the fly, "
                  + "for graphs, that are computed and/or adapted on the fly."),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/HeWeMel/nographs",
     author="Dr. Helmut Melcher",
     author_email='HeWeMel@web.de',
@@ -22,23 +22,26 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Typing :: Typed",
     ],
-    keywords='graph,search,traverse,analysis,lazy,infinite,large,adapt',
+    keywords=('graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,'
+              + 'depth,DFS,breadth,BFS,Dijkstra,topological,MST'),
     python_requires='>=3.9, <4',
     project_urls={
         'Documentation': 'https://nographs.readthedocs.io/',
         'Source': 'https://github.com/hewemel/nographs/',
         'Bug Reports': 'https://github.com/hewemel/nographs/issues',
         # 'Say Thanks!': 'http://saythanks.io/to/HeWeMel',
     },
```

### Comparing `nographs-3.1.0/src/nographs/__init__.py` & `nographs-3.2.0/src/nographs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     Paths,
     # PathsOfUnlabeledEdges,
     # PathsOfLabeledEdges,
     # PathsDummy,
     # DummyPredecessorOrAttributesMapping,
 )
 from ._strategies import (
+    # StrRepr,
     Strategy,
     T_strategy,
     NextVertices,  # Usable, in rare cases, for typing application-defined functions
     NextEdges,
     NextLabeledEdges,
     NextWeightedEdges,
     NextWeightedLabeledEdges,
```

### Comparing `nographs-3.1.0/src/nographs/_bidir_search.py` & `nographs-3.2.0/src/nographs/_bidir_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,18 +512,18 @@
 
     **Properties:** In both directions, vertices are visited by increasing distance
     (minimally necessary sum of edge weights) from a start (resp. a goal) vertex,
     till a shortest path (minimal sum of edge weights) from a start to a goal vertex
     is found. Each vertex is visited only once.
 
     **Input:** Weighted directed graph. One or more start vertices, and one or more
-    goal vertices. Weights need to be non-negative. NextVertices (resp. NextEdges)
-    functions both for the outgoing edges from a vertex and the incoming edges to a
-    vertex have to be provided, and they need to describe the same graph. Optional
-    calculation limit.
+    goal vertices. Weights need to be non-negative. NextWeightedEdges (resp.
+    NextWeightedLabeledEdges) functions both for the outgoing edges from a vertex
+    and the incoming edges to a vertex have to be provided, and they need to describe
+    the same graph. Optional calculation limit.
 
     Note: A shortest path from a vertex *v* to itself always exists, has length 0,
     and will be found by the class, whilst TraversalShortestPaths does not report
     start vertices and thus,
     TraversalShortestPaths(<something>).start_at(v).go_to(v) fails.
     """
```

### Comparing `nographs-3.1.0/src/nographs/_compatibility.py` & `nographs-3.2.0/src/nographs/_compatibility.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 
 
 # --- Solve 3.9 compatibility issue
 
 
 def _pairwise(iterable: Iterable[T]) -> Iterator[tuple[T, T]]:
     """Returns an iterator of paired items, overlapping, from the original.
-    On Python 3.10 and above, this is an alias for :func:`itertools.pairwise`.
+    On Python 3.10 and above, this is replaced by an alias for
+    :func:`itertools.pairwise`.
+
+    >>> list(_pairwise("abc"))
+    [('a', 'b'), ('b', 'c')]
     """
     a, b = itertools.tee(iterable)
     next(b, None)
     yield from zip(a, b)
 
 
 try:
     from itertools import pairwise as itertools_pairwise  # type: ignore[attr-defined]
-except ImportError:
+except ImportError:  # pragma: no cover  # not executed under Python >=3.10
     pairwise = _pairwise
-else:
+else:  # pragma: no cover  # not executed under Python <3.10
 
     def pairwise(iterable: Iterable[T]) -> Iterator[tuple[T, T]]:
         yield from itertools_pairwise(iterable)
 
     pairwise.__doc__ = _pairwise.__doc__
```

### Comparing `nographs-3.1.0/src/nographs/_edge_gadgets.py` & `nographs-3.2.0/src/nographs/_edge_gadgets.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs/_gear_collections.py` & `nographs-3.2.0/src/nographs/_gear_collections.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs/_gears.py` & `nographs-3.2.0/src/nographs/_gears.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs/_matrix_gadgets.py` & `nographs-3.2.0/src/nographs/_matrix_gadgets.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs/_path.py` & `nographs-3.2.0/src/nographs/_path.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs/_paths.py` & `nographs-3.2.0/src/nographs/_paths.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs/_strategies.py` & `nographs-3.2.0/src/nographs/_strategies.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,37 +41,91 @@
     WeightedLabeledOutEdge,
     UnweightedLabeledOutEdge,
     LabeledOutEdge,
     OutEdge,
 )
 
 
-# -- Base class for all traversals and searches --
+# --------------- classes -------------
+
+
+class StrRepr:
+    """Provides a specifically "normalized" string representation of data."""
+
+    def __init__(self, s: str) -> None:
+        self.s = s
+
+    @classmethod
+    def from_iterable(cls, i: Iterable[tuple[Any, Any]]) -> StrRepr:
+        """
+        Provides a string representation of an iterable of key/value tuples,
+        that look like the output from a dict with these items.
+
+        (The 'keys' do not need to be hashable.)
+        """
+        return cls("{" + ", ".join(repr(k) + ": " + repr(v) for k, v in i) + "}")
+
+    @classmethod
+    def from_set(cls, c: MutableSet[Any]) -> StrRepr:
+        """
+        Provides a string representation of a *MutableSet*,
+        that looks like the string representation of a *Set* with these items,
+        but the elements are lexicographically sorted.
+
+        The result is independent of the methods repr() and str() of the
+        *MutableSet*. (The elements do not need to be hashable.)
+        """
+        return cls("{" + ", ".join(sorted(repr(k) for k in c)) + "}")
+
+    def __repr__(self) -> str:
+        return self.s
 
 
 class Strategy(ABC, Generic[T_vertex, T_vertex_id, T_labels]):
     """Base class of the traversal strategies and search strategies of NoGraphs."""
 
-    def _state_and_more_to_str(self, less: Iterable[str], more: dict[str, Any]) -> str:
-        """Return a description of the public state of the strategy as a string.
-        If the strategy has a paths container, this container is ignored."""
-        a = dict((k, v) for k, v in self.__dict__.items() if k[0] != "_")
-        for key_string in less:
-            if key_string in a:
-                del a[key_string]
-        a.update(more)
-        return str(a)
+    def _improve_state(
+        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
+    ) -> None:
+        """Improve the state description
+
+        :param state: State in current form
+        :param vertices: If the strategy can provide additional state data w.r.t. these
+            vertices, it will do so.
+        """
+        pass
 
     def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
-        """Return a description of the public state of the strategy as a string.
+        """Return a human-readable description of the public state of the strategy as
+        a string.
+
+        Implementation details, not covered by the semantic versioning:
+
+        Currently, the method aims at providing a uniform behaviour over different
+        platforms (*CPython* and *PyPy*) and collection types (Gears with different
+        *MutableSet* and *MutableMapping* implementations). It behaves roughly as
+        follows:
+
+        - A *MutableSet*, e.g. attribute *visited*, is described similar to a *set*,
+          but items are sorted lexicographically in their string representations
+          (this bridges differences between *CPython* and *PyPy*).
+
+        - Attribute *Paths* is described similar to a *dict* (although keys can contain
+          unhashable values, and only paths for the given *vertices* are described).
+
+        - A *MutableMapping*, e.g. attribute *distance*, is described similarly to a
+          *dict*, also in cases, where it is not a *dict*, and although the items
+          for only the given *vertices* are described.
 
         :param vertices: If the strategy can provide additional state data w.r.t. these
             vertices, it will do so.
         """
-        return self._state_and_more_to_str(less=(), more=dict())
+        state = dict((k, v) for k, v in self.__dict__.items() if k[0] != "_")
+        self._improve_state(state, vertices)
+        return str(state)
 
 
 # --------------- exported types -------------
 
 # todo: Warning: The following types are manually documented in api.rst
 
 # next vertices and next edges functions for traversals
```

### Comparing `nographs-3.1.0/src/nographs/_traversals.py` & `nographs-3.2.0/src/nographs/_traversals.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 )
 from ._paths import (
     Paths,
     DummyPredecessorOrAttributesMapping,
     PathsDummy,
 )
 from ._strategies import (
+    StrRepr,
     Strategy,
     T_strategy,
     NextVertices,
     NextEdges,
     NextLabeledEdges,
     NextWeightedEdges,
     NextWeightedLabeledEdges,
@@ -360,20 +361,31 @@
     def _start(self) -> None:
         self._generator = self._traverse()
 
     @abstractmethod
     def _traverse(self) -> Iterator[T_vertex]:
         """Has to be implemented in subclass"""
 
-    def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
-        more = dict()
-        if vertices is not None and self._build_paths:
-            for vertex in vertices:
-                more[f"paths[{vertex}]"] = self.paths[vertex]
-        return self._state_and_more_to_str(less=["paths"], more=more)
+    def _improve_state(
+        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
+    ) -> None:
+        # Convert a Paths object to an object that can be converted to a str.
+        # Paths in the paths object are only valid for reported vertices,
+        # and these do not need to be hashable. So, we cannot convert them
+        # to a dict and from there to a string.
+        del state["paths"]
+        if vertices is not None:
+            state["paths"] = (
+                StrRepr.from_iterable(
+                    (vertex, self.paths[vertex]) for vertex in vertices
+                )
+                if self._build_paths
+                else dict()
+            )
+        super()._improve_state(state, vertices)
 
 
 # -------------- Traversal strategies for unweighted edges -----------------
 
 
 class _TraversalWithoutWeights(Traversal[T_vertex, T_vertex_id, T_labels], ABC):
     """Internal: A traversal without weight type and distances collection, but
@@ -416,14 +428,24 @@
             self._gear,
             already_visited,
             iter_start_ids(self._start_vertices, self._vertex_to_id),
             self._is_tree,
         )
         super()._start()
 
+    def _improve_state(
+        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
+    ) -> None:
+        # Visited, a MutableSet, is typically not ordered. str(self.visited)
+        # results in different strings for different interpreters (PyPy) and
+        # the keys are not sorted. Here, we create a normalized description.
+        del state["visited"]
+        state["visited"] = StrRepr.from_set(self.visited)
+        super()._improve_state(state, vertices)
+
 
 class _TraversalWithoutWeightsBasic(
     _TraversalWithoutWeights[T_vertex, T_vertex_id, T_labels], ABC
 ):
     @abstractmethod
     def start_from(
         self,
@@ -2547,31 +2569,27 @@
             for v in self._generator:
                 if self.distance >= stop:
                     break
                 yield v
 
         return my_generator()
 
-    def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
-        more = dict[str, Any]()
+    def _improve_state(
+        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
+    ) -> None:
+        # Assignments in distances are only valid for reported vertices. Thus,
+        # we need to convert only keys/values for requested vertices to a string,
+        # not the whole MutableMapping. So, we special case this attribute here.
+        del state["distances"]
         if vertices is not None:
-            if self._build_paths:
-                for vertex in vertices:
-                    more[f"paths[{vertex}]"] = self.paths[vertex]
-            if self._vertex_to_id is vertex_as_id:
-                for vertex in vertices:
-                    more[f"distances[{vertex}]"] = self.distances[
-                        self._vertex_to_id(vertex)
-                    ]
-            else:
-                for vertex in vertices:
-                    more[f"distances[vertex_to_id({vertex})]"] = self.distances[
-                        self._vertex_to_id(vertex)
-                    ]
-        return self._state_and_more_to_str(less=["paths", "distances"], more=more)
+            vertex_to_id, distances = self._vertex_to_id, self.distances
+            state["distances"] = StrRepr.from_iterable(
+                (v_id := vertex_to_id(vertex), distances[v_id]) for vertex in vertices
+            )
+        super()._improve_state(state, vertices)
 
 
 class TraversalShortestPaths(
     Generic[T_vertex, T_weight, T_labels],
     TraversalShortestPathsFlex[T_vertex, T_vertex, Union[T_weight, float], T_labels],
 ):
     """
@@ -3003,31 +3021,27 @@
                     except IndexError:
                         path_length_guesses_wrapper.extend_and_set(n_id, n_guess)
                 heappush(
                     to_visit,
                     (n_guess, next(unique_no), neighbor, n_path_edge_count),
                 )
 
-    def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
-        more = dict[str, Any]()
+    def _improve_state(
+        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
+    ) -> None:
+        # Assignments in distances are only valid for reported vertices. Thus,
+        # we need to convert only keys/values for requested vertices to a string,
+        # not the whole MutableMapping. So, we special case this attribute here.
+        del state["distances"]
         if vertices is not None:
-            if self._build_paths:
-                for vertex in vertices:
-                    more[f"paths[{vertex}]"] = self.paths[vertex]
-            if self._vertex_to_id is vertex_as_id:
-                for vertex in vertices:
-                    more[f"distances[{vertex}]"] = self.distances[
-                        self._vertex_to_id(vertex)
-                    ]
-            else:
-                for vertex in vertices:
-                    more[f"distances[vertex_to_id({vertex})]"] = self.distances[
-                        self._vertex_to_id(vertex)
-                    ]
-        return self._state_and_more_to_str(less=["paths", "distances"], more=more)
+            vertex_to_id, distances = self._vertex_to_id, self.distances
+            state["distances"] = StrRepr.from_iterable(
+                (v_id := vertex_to_id(vertex), distances[v_id]) for vertex in vertices
+            )
+        super()._improve_state(state, vertices)
 
 
 class TraversalAStar(
     Generic[T_vertex, T_weight, T_labels],
     TraversalAStarFlex[T_vertex, T_vertex, Union[T_weight, float], T_labels],
 ):
     """
```

### Comparing `nographs-3.1.0/src/nographs/_types.py` & `nographs-3.2.0/src/nographs/_types.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/src/nographs.egg-info/PKG-INFO` & `nographs-3.2.0/src/nographs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nographs
-Version: 3.1.0
+Version: 3.2.0
 Summary: Graph analysis – the lazy (evaluation) way: Analysis on the fly, for graphs, that are computed and/or adapted on the fly.
 Home-page: https://github.com/HeWeMel/nographs
 Author: Dr. Helmut Melcher
 Author-email: HeWeMel@web.de
 Project-URL: Documentation, https://nographs.readthedocs.io/
 Project-URL: Source, https://github.com/hewemel/nographs/
 Project-URL: Bug Reports, https://github.com/hewemel/nographs/issues
-Keywords: graph,search,traverse,analysis,lazy,infinite,large,adapt
+Keywords: graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,depth,DFS,breadth,BFS,Dijkstra,topological,MST
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
@@ -32,14 +34,17 @@
 
 .. |PyPI status| image:: https://img.shields.io/pypi/status/nographs.svg
    :target: https://pypi.python.org/pypi/nographs/
 
 .. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/nographs.svg
    :target: https://pypi.python.org/pypi/nographs/
 
+.. |PyPy versions| image:: https://img.shields.io/badge/PyPy-3.11-blue
+   :target: https://pypi.python.org/pypi/nographs/
+
 .. |PyPI license| image:: https://img.shields.io/pypi/l/nographs.svg
    :target: https://github.com/HeWeMel/nographs/blob/main/LICENSE
 
 .. |CI| image:: https://github.com/hewemel/nographs/workflows/CI%20(tests,%20flake8,%20mypy)/badge.svg?branch=main
    :target: https://github.com/hewemel/nographs/actions?query=workflow%3ACI%20(pip)
 
 .. |CodeCov| image:: https://img.shields.io/codecov/c/gh/HeWeMel/NoGraphs/main
@@ -74,59 +79,62 @@
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
 **Feature overview**
 
 - Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
 - Bidirectional search algorithms: BFS and Dijkstra.
+- Results: Reachability, depth, distance, paths and trees.
+  Paths can be
+  calculated with vertices, edges, or attributed edges,
+  and can be iterated in both directions.
 - Flexible graph notion:
 
   - Infinite directed multigraphs with loops and
     attributes (this includes
     multiple adjacency, cycles, self-loops,
     directed edges,
     weighted edges and edges with application specific attributes).
   - Infinite graphs are supported, but need to be
     locally finite (i.e., a vertex has only finitely many outgoing edges).
 
-- Generic API. The application can define the following:
+- Generic API:
 
   - Vertices: Can be anything except for None. Hashable vertices can be
     used directly, unhashable vertices can be used together with
     hashable identifiers.
   - Edge weights and distances: Wide range of data types
     supported (float, int, Decimal, mpmath.mpf and others), e.g.,
     for high precision computations.
   - Edge attributes: Any object, e.g, a container
     with further data.
-  - Identity and equivalence of vertices.
+  - Identity and equivalence of vertices can be chosen / defined.
   - Bookkeeping: Several sets of bookkeeping data structures
     are predefined, optimized for different situations (data types used by the
     application, hashing vs. indexing, collections for *Python* objects or *C* native
     data types,...); Adaptable and extendable, e.g., specialized
     collections of 3rd party libraries can be integrated easily and runtime
     efficiently
 
-- Results: Reachability, depth, distance, paths and trees.
-  Paths can be
-  calculated with vertices or edges or attributed edges
-  and can be iterated in both directions.
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
   allows for an API that eases
   operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
   computation of search-aware graphs, and
   traversals of vertex equivalence classes on the fly.
   Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
-- Runtime and memory performance: Have been goals. In its domain, it
-  often even outperforms Rust- and C-based libraries.
+- CI tests: For all supported versions of Python and both supported interpreters
+  CPython and PyPy, both code and docs, 100% code coverage.
+- Runtime and memory performance: Have been goals (CPython). In its domain, it often
+  even outperforms Rust- and C-based libraries.
+  If you need an even higher performance, using PyPy could be an option.
 
 **Documentation**
 
 - `Homepage of the documentation <https://nographs.readthedocs.io>`__
 - `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
 - `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
   (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
```

### Comparing `nographs-3.1.0/src/nographs.egg-info/SOURCES.txt` & `nographs-3.2.0/src/nographs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_docs_examples.py` & `nographs-3.2.0/tests/test_docs_examples.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_edge_gadgets.py` & `nographs-3.2.0/tests/test_edge_gadgets.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_gear_collections.py` & `nographs-3.2.0/tests/test_gear_collections.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_gears.py` & `nographs-3.2.0/tests/test_gears.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_matrix_gadgets.py` & `nographs-3.2.0/tests/test_matrix_gadgets.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_nographs.py` & `nographs-3.2.0/tests/test_nographs.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         test_suite.addTests(doctest.DocTestSuite(name))
 
     # Unittests from unit test classes in some unit test files in tests folder
     new_suite = unittest.defaultTestLoader.discover("tests", pattern="test_unit*.py")
     test_suite.addTests(new_suite)
 
     # Unittests from doc tests in modules of package
-    modules = ("types", "strategies", "matrix_gadgets", "edge_gadgets", "paths")
+    modules = ("types", "strategies", "matrix_gadgets", "edge_gadgets", "paths",
+               "compatibility")
     for f in modules:
         temp_module = importlib.import_module("._" + f, "nographs")
         test_suite.addTests(doctest.DocTestSuite(temp_module))
 
     # Unittests from doc tests in documentation
     p = pathlib.Path("./docs/source")
     for file_path in p.glob("*.rst"):
```

### Comparing `nographs-3.1.0/tests/test_paths.py` & `nographs-3.2.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_strategies.py` & `nographs-3.2.0/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_traversals_and_searches.py` & `nographs-3.2.0/tests/test_traversals_and_searches.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import abstractmethod, ABC
 from collections.abc import Callable, Hashable, Iterator
 from typing import Any, Iterable, Union, TypeVar, Optional, Protocol, Generic
 
 import nographs as nog
 from nographs import T, Strategy, T_vertex, T_vertex_id, T_labels, T_weight
 from nographs._compatibility import pairwise
+from nographs._strategies import StrRepr  # NOQA F401 (import needed by doc tests)
 
 # ----- Utilities: Printing test results -----
 
 
 def eprint(*args: Any, **kwargs: Any) -> None:
     """Print to stderr. For typing see print.
     Untyped, because type is overly complex."""
@@ -89,15 +90,17 @@
     that path container remains the same object, print all paths.
     Additionally, print visited container and check that it remained the same object
     during traversal.
     """
     org_dict = _results_of_traversal(traversal, start_vertices)
     if org_dict["visited"] is not traversal.visited:
         print("traversal.visited before and while traversal differ!")
-    print("All visited:", list(traversal.visited))
+    visited = list(traversal.visited)
+    visited.sort()
+    print("All visited:", visited)
 
 
 def results_with_distances(
     traversal: nog.TraversalShortestPathsFlex[
         T_sortable_vertex, T_vertex_id, T_weight, T_labels
     ],
     start_vertices: Iterable[T_sortable_vertex],
@@ -615,69 +618,69 @@
 class GraphWithoutEdges:
     """-- Graph without edges --
     -- 1) No vertices are reported. Exceptions: topological sorting reports it,
     and BidirectionalSearchShortestPath finds a path from v to v in empty paths.
     >>> f = FNoEdgesGoalIsStart()
 
     >>> list(nog.TraversalBreadthFirst(f.next_vertices).start_from(f.start))
-    ? 0: {'visited': {0}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0}, 'paths': {}}
     []
     >>> list(nog.TraversalDepthFirst(f.next_vertices).start_from(f.start,
     ...     compute_depth=True))
-    ? 0: {'visited': {0}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0}, 'paths': {}}
     []
     >>> list(nog.TraversalNeighborsThenDepth(f.next_vertices).start_from(f.start,
     ...     compute_depth=True))
-    ? 0: {'visited': {0}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0}, 'paths': {}}
     []
     >>> list(nog.TraversalTopologicalSort(f.next_vertices).start_from(f.start))
-    ? 0: {'visited': {0}, 'depth': 0, 'cycle_from_start': []}
+    ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {}}
     [0]
     >>> list(nog.TraversalShortestPaths(f.next_edges).start_from(f.start))
-    ? 0: {'distance': 0, 'depth': 0, 'distances[0]': 0}
+    ? 0: {'distance': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {}}
     []
     >>> list(nog.TraversalMinimumSpanningTree(f.next_edges).start_from(f.start))
-    ? 0: {'edge': None}
+    ? 0: {'edge': None, 'paths': {}}
     []
     >>> list(nog.TraversalAStar(f.next_edges).start_from(f.heuristic, f.start))
-    ? 0: {'path_length': 0, 'depth': 0, 'distances[0]': 0}
+    ? 0: {'path_length': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {}}
     []
     >>> d, p = nog.BSearchBreadthFirst(f.next_vertices_bi).start_from(f.start_bi)
     >>> print(d, list(p))
     0 [0]
     >>> l, p = nog.BSearchShortestPath(f.next_edges_bi).start_from(f.start_bi)
     >>> print(l, list(p))
     0 [0]
 
     -- 2a) go_to and go_for_vertices_in find nothing and correctly report this
     >>> f = FNoEdgesGoalUnreachable()
 
     >>> traversal = nog.TraversalBreadthFirst(f.next_vertices)
     >>> traversal.start_from(f.start).go_to(f.goal, fail_silently=True) is None
-    ? 0: {'visited': {0}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0}, 'paths': {}}
     True
     >>> traversal.start_from(f.start).go_to(f.goal)
     Traceback (most recent call last):
     KeyError: 'Vertex not found, graph exhausted.'
     >>> list(traversal.start_from(f.start).go_for_vertices_in(
     ...    (f.goal,), fail_silently=True)
     ... )
-    ? 0: {'visited': {0}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0}, 'paths': {}}
     []
     >>> list(traversal.start_from(f.start).go_for_vertices_in((f.goal,)))
     Traceback (most recent call last):
     KeyError: 'Not all of the given vertices have been found'
 
     -- 2b) start_at of bidirectional searches find nothing and correctly report this
     >>> search = nog.BSearchBreadthFirst(next_edges=f.next_vertices_bi)
     >>> _ = search.start_from(f.start_bi)
     Traceback (most recent call last):
     KeyError: 'No path to (a) goal vertex found'
     >>> length, path = search.start_from(f.start_bi, fail_silently=True)
-    ? 0: {'visited': {0}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0}, 'paths': {}}
     >>> print(length, type(path))
     -1 <class 'nographs._path.PathOfUnlabeledEdges'>
 
     >>> search = nog.BSearchShortestPath(f.next_edges_bi)
     >>> _ = search.start_from(f.start_bi)
     Traceback (most recent call last):
     KeyError: 'No path to (a) goal vertex found'
@@ -1052,40 +1055,40 @@
     >>> traversal = nog.TraversalBreadthFirstFlex(
     ...     first_of, nog.GearDefault(), f.next_vertices)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': 1, 'paths[[1]]': ([0], [1])}
+    {'depth': 1, 'visited': {0, 1}, 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalDepthFirstFlex(
     ...    first_of, nog.GearDefault(), f.next_vertices)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': -1, 'paths[[1]]': ([0], [1])}
+    {'depth': -1, 'visited': {0, 1}, 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalNeighborsThenDepthFlex(
     ...    first_of, nog.GearDefault(), f.next_vertices)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': -1, 'paths[[1]]': ([0], [1])}
+    {'depth': -1, 'visited': {0, 1}, 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalTopologicalSortFlex(
     ...    first_of, nog.GearDefault(), f.next_vertices)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1], [0]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': 1, 'cycle_from_start': [], 'paths[[1]]': ([0],
-      [1])}
+    {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1}, 'paths': {[1]: ([0],
+      [1])}}
     >>> search = nog.BSearchBreadthFirstFlex(
     ...     first_of, nog.GearDefault(), f.next_vertices_bi)
     >>> test_bidirectional(search, f.start, f.goal, labeled_paths=False)
     1 True
     1 [[0], [1]]
 
 
@@ -1093,150 +1096,148 @@
     >>> traversal = nog.TraversalBreadthFirstFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': 1, 'paths[[1]]': ([0], [1])}
+    {'depth': 1, 'visited': {0, 1}, 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalBreadthFirstFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True)
     [[1]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'visited': {0, 1}, 'depth': 1, 'paths[[1]]': (([0], [1], 2),)}
+    {'depth': 1, 'visited': {0, 1}, 'paths': {[1]: (([0], [1], 2),)}}
 
     >>> traversal = nog.TraversalDepthFirstFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': -1, 'paths[[1]]': ([0], [1])}
+    {'depth': -1, 'visited': {0, 1}, 'paths': {[1]: ([0], [1])}}
 
     >>> traversal = nog.TraversalDepthFirstFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True)
     [[1]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'visited': {0, 1}, 'depth': -1, 'paths[[1]]': (([0], [1], 2),)}
+    {'depth': -1, 'visited': {0, 1}, 'paths': {[1]: (([0], [1], 2),)}}
 
     >>> traversal = nog.TraversalNeighborsThenDepthFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': -1, 'paths[[1]]': ([0], [1])}
+    {'depth': -1, 'visited': {0, 1}, 'paths': {[1]: ([0], [1])}}
 
     >>> traversal = nog.TraversalNeighborsThenDepthFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True)
     [[1]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'visited': {0, 1}, 'depth': -1, 'paths[[1]]': (([0], [1], 2),)}
+    {'depth': -1, 'visited': {0, 1}, 'paths': {[1]: (([0], [1], 2),)}}
 
     >>> traversal = nog.TraversalShortestPathsFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'distance': 1, 'depth': 1, 'paths[[1]]': ([0], [1]),
-      'distances[vertex_to_id([1])]': 0}
+    {'distance': 1, 'depth': 1, 'distances': {1: 0}, 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalShortestPathsFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True)
     [[1]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'distance': 1, 'depth': 1, 'paths[[1]]': (([0], [1], 2),),
-      'distances[vertex_to_id([1])]': 0}
+    {'distance': 1, 'depth': 1, 'distances': {1: 0}, 'paths': {[1]: (([0], [1],
+      2),)}}
 
     >>> traversal = nog.TraversalMinimumSpanningTreeFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'edge': ([0], [1], 1, 2), 'paths[[1]]': ([0], [1])}
+    {'edge': ([0], [1], 1, 2), 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalMinimumSpanningTreeFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True)
     [[1]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'edge': ([0], [1], 1, 2), 'paths[[1]]': (([0], [1], 2),)}
+    {'edge': ([0], [1], 1, 2), 'paths': {[1]: (([0], [1], 2),)}}
 
     >>> traversal = nog.TraversalTopologicalSortFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False)
     [[1], [0]]
     True
     [1]
     ([0], [1])
-    {'visited': {0, 1}, 'depth': 1, 'cycle_from_start': [], 'paths[[1]]': ([0],
-      [1])}
+    {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1}, 'paths': {[1]: ([0],
+      [1])}}
     >>> traversal = nog.TraversalTopologicalSortFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True)
     [[1], [0]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'visited': {0, 1}, 'depth': 1, 'cycle_from_start': [], 'paths[[1]]': (([0],
-      [1], 2),)}
+    {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1}, 'paths': {[1]: (([0],
+      [1], 2),)}}
 
     >>> traversal = nog.TraversalAStarFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=False,
     ...     heuristic=f.heuristic)
     [[1]]
     True
     [1]
     ([0], [1])
-    {'path_length': 1, 'depth': 1, 'paths[[1]]': ([0], [1]),
-      'distances[vertex_to_id([1])]': 1}
+    {'path_length': 1, 'depth': 1, 'distances': {1: 1}, 'paths': {[1]: ([0], [1])}}
     >>> traversal = nog.TraversalAStarFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges)
     >>> test(traversal, f.start, f.goal, labeled_paths=True,
     ...     heuristic=f.heuristic)
     [[1]]
     True
     [1]
     ([0], [1])
     (([0], [1], 2),)
-    {'path_length': 1, 'depth': 1, 'paths[[1]]': (([0], [1], 2),),
-      'distances[vertex_to_id([1])]': 1}
+    {'path_length': 1, 'depth': 1, 'distances': {1: 1}, 'paths': {[1]: (([0], [1],
+      2),)}}
 
     >>> search = nog.BSearchBreadthFirstFlex(
     ...     first_of, nog.GearDefault(),
     ...     next_labeled_edges=f.next_edges_bi)
     >>> test_bidirectional(search, f.start, f.goal, labeled_paths=True)
     1 True
     1 [([0], [1], 2)]
@@ -1269,60 +1270,60 @@
 
     >>> test_traversal(nog.TraversalBreadthFirstFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges))
     [[1], [2], [3], [4]]
     [[1], [3]]
     [3]
     ([0], [1], [2], [3])
-    {'visited': {0, 1, 2, 3}, 'depth': 3, 'paths[[3]]': ([0], [1], [2], [3])}
+    {'depth': 3, 'visited': {0, 1, 2, 3}, 'paths': {[3]: ([0], [1], [2], [3])}}
     >>> test_traversal(nog.TraversalDepthFirstFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges))
     [[1], [2], [3], [4]]
     [[1], [3]]
     [3]
     ([0], [1], [2], [3])
-    {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[[3]]': ([0], [1], [2], [3])}
+    {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {[3]: ([0], [1], [2], [3])}}
     >>> test_traversal(nog.TraversalNeighborsThenDepthFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges))
     [[1], [2], [3], [4]]
     [[1], [3]]
     [3]
     ([0], [1], [2], [3])
-    {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[[3]]': ([0], [1], [2], [3])}
+    {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {[3]: ([0], [1], [2], [3])}}
     >>> test_traversal(nog.TraversalShortestPathsFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges))
     [[1], [2], [3], [4]]
     [[1], [3]]
     [3]
     ([0], [1], [2], [3])
-    {'distance': 3, 'depth': 3, 'paths[[3]]': ([0], [1], [2], [3]),
-      'distances[vertex_to_id([3])]': 0}
+    {'distance': 3, 'depth': 3, 'distances': {3: 0}, 'paths': {[3]: ([0], [1], [2],
+      [3])}}
     >>> test_traversal(nog.TraversalMinimumSpanningTreeFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges))
     [[1], [2], [3], [4]]
     [[1], [3]]
     [3]
     ([0], [1], [2], [3])
-    {'edge': ([2], [3], 1, 3), 'paths[[3]]': ([0], [1], [2], [3])}
+    {'edge': ([2], [3], 1, 3), 'paths': {[3]: ([0], [1], [2], [3])}}
     >>> test_traversal(nog.TraversalTopologicalSortFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges))
     [[4], [3], [2], [1], [0]]
     [[3], [1]]
     [3]
     ([0], [1], [2], [3])
-    {'visited': {0, 1, 2, 3, 4}, 'depth': 3, 'cycle_from_start': [], 'paths[[3]]':
-      ([0], [1], [2], [3])}
+    {'depth': 3, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4}, 'paths': {[3]:
+      ([0], [1], [2], [3])}}
     >>> test_traversal(nog.TraversalAStarFlex(
     ...     first_of, nog.GearDefault(), next_edges=f.next_edges), f.heuristic)
     [[1], [2], [3], [4]]
     [[1], [3]]
     [3]
     ([0], [1], [2], [3])
-    {'path_length': 3, 'depth': 3, 'paths[[3]]': ([0], [1], [2], [3]),
-      'distances[vertex_to_id([3])]': 3}
+    {'path_length': 3, 'depth': 3, 'distances': {3: 3}, 'paths': {[3]: ([0], [1],
+      [2], [3])}}
     >>> test_bsearch(nog.BSearchBreadthFirstFlex(
     ...     first_of, nog.GearDefault(), next_labeled_edges=f.next_edges_bi))
     3 []
     3 [([0], [1], 1), ([1], [2], 2), ([2], [3], 3)]
     >>> test_bsearch(nog.BSearchShortestPathFlex(
     ...     first_of, nog.GearDefault(), next_labeled_edges=f.next_edges_bi))
     3 []
@@ -1380,109 +1381,110 @@
     @staticmethod
     def unattributed_edges() -> None:
         """
         >>> f = FDiamond()
         >>> traversal = nog.TraversalBreadthFirst(f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 1: {'visited': {0, 1, 2}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 1, 3)}
-        ? 2: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 1, 3)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': 1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {1: (0, 1)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 1, 3)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {2: (0, 2)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 1, 3)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 1, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalDepthFirst(f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        -> 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalDepthFirst(f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': -1, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[1]': (0, 1)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': -1, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 2: {'depth': -1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': -1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': -1, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': -1, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        -> 1: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
+        ? 1: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalNeighborsThenDepth(f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': 1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalNeighborsThenDepth(f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': -1, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': -1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': -1, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': -1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': -1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': -1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 1: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalTopologicalSort(f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'cycle_from_start': [], 'paths[0]': (0,)}
-        ? 2: {'visited': {0, 2}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0, 2)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]': (0,
-          2, 3)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]': (0,
-          2, 3)}
-        -> 2: {'visited': {0, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0,
-          2)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[1]':
-          (0, 1)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[1]':
-          (0, 1)}
-        -> 0: {'visited': {0, 1, 2, 3}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
+        After start: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {0:
+          (0,)}}
+        ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {0: (0,)}}
+        ? 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 2}, 'paths': {2: (0,
+          2)}}
+        ? 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {3: (0,
+          2, 3)}}
+        -> 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {3:
+          (0, 2, 3)}}
+        -> 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {2:
+          (0, 2)}}
+        ? 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {1:
+          (0, 1)}}
+        -> 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {1:
+          (0, 1)}}
+        -> 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {0:
+          (0,)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> search = nog.BSearchBreadthFirst(f.next_vertices_bi)
         >>> l, p = search.start_from(f.start_bi, build_path=True)
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ?<3: {'visited': {3}, 'depth': 0, 'paths[3]': (3,)}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ?<3: {'depth': 0, 'visited': {3}, 'paths': {3: (3,)}}
         >>> print(l, list(p))
         2 [0, 1, 3]
         """
         pass
 
     @staticmethod
     def unattributed_edges_and_int_id_gear() -> None:
@@ -1490,115 +1492,116 @@
         >>> f = FDiamond()
         >>> gear = nog.GearForIntVertexIDsAndCFloats()
 
         >>> traversal = nog.TraversalBreadthFirstFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 1: {'visited': {0, 1, 2}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 1, 3)}
-        ? 2: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 1, 3)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': 1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {1: (0, 1)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 1, 3)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {2: (0, 2)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 1, 3)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 1, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalDepthFirstFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        -> 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalDepthFirstFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': -1, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[1]': (0, 1)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': -1, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 2: {'depth': -1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': -1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': -1, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': -1, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        -> 1: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
+        ? 1: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalNeighborsThenDepthFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': 1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalNeighborsThenDepthFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': -1, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': -1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': -1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[3]': (0, 2, 3)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': -1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': -1, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': -1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': -1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': -1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 1: {'depth': -1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalTopologicalSortFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'cycle_from_start': [], 'paths[0]': (0,)}
-        ? 2: {'visited': {0, 2}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0, 2)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]': (0,
-          2, 3)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]': (0,
-          2, 3)}
-        -> 2: {'visited': {0, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0,
-          2)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[1]':
-          (0, 1)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[1]':
-          (0, 1)}
-        -> 0: {'visited': {0, 1, 2, 3}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
+        After start: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {0:
+          (0,)}}
+        ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {0: (0,)}}
+        ? 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 2}, 'paths': {2: (0,
+          2)}}
+        ? 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {3: (0,
+          2, 3)}}
+        -> 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {3:
+          (0, 2, 3)}}
+        -> 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {2:
+          (0, 2)}}
+        ? 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {1:
+          (0, 1)}}
+        -> 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {1:
+          (0, 1)}}
+        -> 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {0:
+          (0,)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> search = nog.BSearchBreadthFirstFlex(
         ...     nog.vertex_as_id, gear, f.next_vertices_bi)
         >>> l, p = search.start_from(f.start_bi, build_path=True)
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ?<3: {'visited': {3}, 'depth': 0, 'paths[3]': (3,)}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ?<3: {'depth': 0, 'visited': {3}, 'paths': {3: (3,)}}
         >>> print(l, list(p))
         2 [0, 1, 3]
         """
         pass
 
     @staticmethod
     def unlabeled_edges_and_already_visited() -> None:
@@ -1607,89 +1610,89 @@
         >>> f = FDiamond()
 
         >>> traversal = nog.TraversalBreadthFirst(f.next_vertices)
         >>> already_visited={f.vertex_for_already_visited}
         >>> traversal = traversal.start_from(
         ...     f.start, build_paths=True, already_visited=already_visited)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
+        After start: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
         All paths: [(0,), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
-        >>> print("Already visited:", already_visited)
+        >>> print("Already visited:", StrRepr.from_set(already_visited))
         Already visited: {0, 1, 2, 3}
         >>> traversal.paths[f.vertex_for_already_visited]
         Traceback (most recent call last):
         RuntimeError: Paths: No path for given vertex.
 
         >>> traversal = nog.TraversalDepthFirst(f.next_vertices)
         >>> already_visited={f.vertex_for_already_visited}
         >>> traversal = traversal.start_from(
         ...     f.start, build_paths=True, compute_depth=True,
         ...     already_visited=already_visited)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
+        After start: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
         All paths: [(0,), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
-        >>> print("Already visited:", already_visited)
+        >>> print("Already visited:", StrRepr.from_set(already_visited))
         Already visited: {0, 1, 2, 3}
         >>> traversal.paths[f.vertex_for_already_visited]
         Traceback (most recent call last):
         RuntimeError: Paths: No path for given vertex.
 
         >>> traversal = nog.TraversalNeighborsThenDepth(f.next_vertices)
         >>> already_visited={f.vertex_for_already_visited}
         >>> traversal = traversal.start_from(
         ...     f.start, build_paths=True, compute_depth=True,
         ...     already_visited=already_visited)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
+        After start: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
         All paths: [(0,), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
-        >>> print("Already visited:", already_visited)
+        >>> print("Already visited:", StrRepr.from_set(already_visited))
         Already visited: {0, 1, 2, 3}
         >>> traversal.paths[f.vertex_for_already_visited]
         Traceback (most recent call last):
         RuntimeError: Paths: No path for given vertex.
 
         >>> traversal = nog.TraversalTopologicalSort(f.next_vertices)
         >>> already_visited={f.vertex_for_already_visited}
         >>> traversal = traversal.start_from(
         ...     f.start, build_paths=True, already_visited=already_visited)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0, 1}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
-        ? 0: {'visited': {0, 1}, 'depth': 0, 'cycle_from_start': [], 'paths[0]': (0,)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0,
-          2)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]':
-          (0, 2, 3)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]':
-          (0, 2, 3)}
-        -> 2: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[2]':
-          (0, 2)}
-        -> 0: {'visited': {0, 1, 2, 3}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
+        After start: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1}, 'paths':
+          {0: (0,)}}
+        ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1}, 'paths': {0: (0,)}}
+        ? 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2}, 'paths': {2: (0,
+          2)}}
+        ? 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {3:
+          (0, 2, 3)}}
+        -> 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {3:
+          (0, 2, 3)}}
+        -> 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {2:
+          (0, 2)}}
+        -> 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {0:
+          (0,)}}
         All paths: [(0,), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
-        >>> print("Already visited:", already_visited)
+        >>> print("Already visited:", StrRepr.from_set(already_visited))
         Already visited: {0, 1, 2, 3}
         >>> traversal.paths[f.vertex_for_already_visited]
         Traceback (most recent call last):
         RuntimeError: Paths: No path for given vertex.
         """
         pass
 
@@ -1700,20 +1703,20 @@
         >>> traversal = nog.TraversalBreadthFirst(f.next_vertices)
         >>> already_visited = nog.GearForIntVertexIDsAndCFloats().vertex_id_set(())
         >>> already_visited.add(f.vertex_for_already_visited)
         >>> traversal = traversal.start_from(
         ...     f.start, build_paths=True, already_visited=already_visited)
 
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0, 1}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
+        After start: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0, 1}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
         All paths: [(0,), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
         >>> print("Already visited:", already_visited)
         Already visited: {0, 1, 2, 3}
         >>> traversal.paths[f.vertex_for_already_visited]
         Traceback (most recent call last):
         RuntimeError: Paths: No path for given vertex.
@@ -1724,182 +1727,183 @@
     def labeled_edges() -> None:
         """
         >>> f = FDiamond()
         >>> traversal = nog.TraversalBreadthFirst(
         ...     next_edges=f.next_edges)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 1: {'visited': {0, 1, 2}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 1, 3)}
-        ? 2: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 1, 3)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': 1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {1: (0, 1)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 1, 3)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {2: (0, 2)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 1, 3)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 1, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalDepthFirst(
         ...     next_edges=f.next_edges)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 2: {'visited': {0, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 2: {'depth': 1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        -> 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalNeighborsThenDepth(
         ...     next_edges=f.next_edges)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        -> 1: {'visited': {0, 1}, 'depth': 1, 'paths[1]': (0, 1)}
-        -> 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        ? 2: {'visited': {0, 1, 2}, 'depth': 1, 'paths[2]': (0, 2)}
-        -> 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 3: {'visited': {0, 1, 2, 3}, 'depth': 2, 'paths[3]': (0, 2, 3)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'paths[1]': (0, 1)}
+        After start: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        -> 1: {'depth': 1, 'visited': {0, 1}, 'paths': {1: (0, 1)}}
+        -> 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        ? 2: {'depth': 1, 'visited': {0, 1, 2}, 'paths': {2: (0, 2)}}
+        -> 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 3: {'depth': 2, 'visited': {0, 1, 2, 3}, 'paths': {3: (0, 2, 3)}}
+        ? 1: {'depth': 1, 'visited': {0, 1, 2, 3}, 'paths': {1: (0, 1)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> traversal = nog.TraversalTopologicalSort(
         ...     next_edges=f.next_edges)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': {0}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
-        ? 0: {'visited': {0}, 'depth': 0, 'cycle_from_start': [], 'paths[0]': (0,)}
-        ? 2: {'visited': {0, 2}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0, 2)}
-        ? 3: {'visited': {0, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]': (0,
-          2, 3)}
-        -> 3: {'visited': {0, 2, 3}, 'depth': 2, 'cycle_from_start': [], 'paths[3]': (0,
-          2, 3)}
-        -> 2: {'visited': {0, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[2]': (0,
-          2)}
-        ? 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[1]':
-          (0, 1)}
-        -> 1: {'visited': {0, 1, 2, 3}, 'depth': 1, 'cycle_from_start': [], 'paths[1]':
-          (0, 1)}
-        -> 0: {'visited': {0, 1, 2, 3}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-          (0,)}
+        After start: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {0:
+          (0,)}}
+        ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {0: (0,)}}
+        ? 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 2}, 'paths': {2: (0,
+          2)}}
+        ? 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {3: (0,
+          2, 3)}}
+        -> 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {3:
+          (0, 2, 3)}}
+        -> 2: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 2, 3}, 'paths': {2:
+          (0, 2)}}
+        ? 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {1:
+          (0, 1)}}
+        -> 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {1:
+          (0, 1)}}
+        -> 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1, 2, 3}, 'paths': {0:
+          (0,)}}
         All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
         All visited: [0, 1, 2, 3]
 
         >>> search = nog.BSearchBreadthFirst(next_edges=f.next_edges_bi)
         >>> l, p = search.start_from(f.start_bi, build_path=True)
-        ? 0: {'visited': {0}, 'depth': 0, 'paths[0]': (0,)}
-        ?<3: {'visited': {3}, 'depth': 0, 'paths[3]': (3,)}
+        ? 0: {'depth': 0, 'visited': {0}, 'paths': {0: (0,)}}
+        ?<3: {'depth': 0, 'visited': {3}, 'paths': {3: (3,)}}
         >>> print(l, list(p))
         2 [0, 1, 3]
         """
         pass
 
     @staticmethod
     def is_tree() -> None:
         """
         >>> f = FSmallBinaryTree()
         >>> traversal = nog.TraversalBreadthFirst(f.next_vertices,is_tree=True)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': set(), 'depth': 0, 'paths[1]': (1,)}
-        ? 1: {'visited': set(), 'depth': 0, 'paths[1]': (1,)}
-        -> 2: {'visited': set(), 'depth': 1, 'paths[2]': (1, 2)}
-        -> 3: {'visited': set(), 'depth': 1, 'paths[3]': (1, 3)}
-        ? 2: {'visited': set(), 'depth': 1, 'paths[2]': (1, 2)}
-        -> 4: {'visited': set(), 'depth': 2, 'paths[4]': (1, 2, 4)}
-        -> 5: {'visited': set(), 'depth': 2, 'paths[5]': (1, 2, 5)}
-        ? 3: {'visited': set(), 'depth': 1, 'paths[3]': (1, 3)}
-        -> 6: {'visited': set(), 'depth': 2, 'paths[6]': (1, 3, 6)}
-        -> 7: {'visited': set(), 'depth': 2, 'paths[7]': (1, 3, 7)}
-        ? 4: {'visited': set(), 'depth': 2, 'paths[4]': (1, 2, 4)}
-        ? 5: {'visited': set(), 'depth': 2, 'paths[5]': (1, 2, 5)}
-        ? 6: {'visited': set(), 'depth': 2, 'paths[6]': (1, 3, 6)}
-        ? 7: {'visited': set(), 'depth': 2, 'paths[7]': (1, 3, 7)}
+        After start: {'depth': 0, 'visited': {}, 'paths': {1: (1,)}}
+        ? 1: {'depth': 0, 'visited': {}, 'paths': {1: (1,)}}
+        -> 2: {'depth': 1, 'visited': {}, 'paths': {2: (1, 2)}}
+        -> 3: {'depth': 1, 'visited': {}, 'paths': {3: (1, 3)}}
+        ? 2: {'depth': 1, 'visited': {}, 'paths': {2: (1, 2)}}
+        -> 4: {'depth': 2, 'visited': {}, 'paths': {4: (1, 2, 4)}}
+        -> 5: {'depth': 2, 'visited': {}, 'paths': {5: (1, 2, 5)}}
+        ? 3: {'depth': 1, 'visited': {}, 'paths': {3: (1, 3)}}
+        -> 6: {'depth': 2, 'visited': {}, 'paths': {6: (1, 3, 6)}}
+        -> 7: {'depth': 2, 'visited': {}, 'paths': {7: (1, 3, 7)}}
+        ? 4: {'depth': 2, 'visited': {}, 'paths': {4: (1, 2, 4)}}
+        ? 5: {'depth': 2, 'visited': {}, 'paths': {5: (1, 2, 5)}}
+        ? 6: {'depth': 2, 'visited': {}, 'paths': {6: (1, 3, 6)}}
+        ? 7: {'depth': 2, 'visited': {}, 'paths': {7: (1, 3, 7)}}
         All paths: [(1,), (1, 2), (1, 3), (1, 2, 4), (1, 2, 5), (1, 3, 6), (1, 3, 7)]
         All visited: []
 
         >>> traversal = nog.TraversalDepthFirst(f.next_vertices, is_tree=True)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': set(), 'depth': 0, 'paths[1]': (1,)}
-        ? 1: {'visited': set(), 'depth': 0, 'paths[1]': (1,)}
-        -> 3: {'visited': set(), 'depth': 1, 'paths[3]': (1, 3)}
-        ? 3: {'visited': set(), 'depth': 1, 'paths[3]': (1, 3)}
-        -> 7: {'visited': set(), 'depth': 2, 'paths[7]': (1, 3, 7)}
-        ? 7: {'visited': set(), 'depth': 2, 'paths[7]': (1, 3, 7)}
-        -> 6: {'visited': set(), 'depth': 2, 'paths[6]': (1, 3, 6)}
-        ? 6: {'visited': set(), 'depth': 2, 'paths[6]': (1, 3, 6)}
-        -> 2: {'visited': set(), 'depth': 1, 'paths[2]': (1, 2)}
-        ? 2: {'visited': set(), 'depth': 1, 'paths[2]': (1, 2)}
-        -> 5: {'visited': set(), 'depth': 2, 'paths[5]': (1, 2, 5)}
-        ? 5: {'visited': set(), 'depth': 2, 'paths[5]': (1, 2, 5)}
-        -> 4: {'visited': set(), 'depth': 2, 'paths[4]': (1, 2, 4)}
-        ? 4: {'visited': set(), 'depth': 2, 'paths[4]': (1, 2, 4)}
+        After start: {'depth': 0, 'visited': {}, 'paths': {1: (1,)}}
+        ? 1: {'depth': 0, 'visited': {}, 'paths': {1: (1,)}}
+        -> 3: {'depth': 1, 'visited': {}, 'paths': {3: (1, 3)}}
+        ? 3: {'depth': 1, 'visited': {}, 'paths': {3: (1, 3)}}
+        -> 7: {'depth': 2, 'visited': {}, 'paths': {7: (1, 3, 7)}}
+        ? 7: {'depth': 2, 'visited': {}, 'paths': {7: (1, 3, 7)}}
+        -> 6: {'depth': 2, 'visited': {}, 'paths': {6: (1, 3, 6)}}
+        ? 6: {'depth': 2, 'visited': {}, 'paths': {6: (1, 3, 6)}}
+        -> 2: {'depth': 1, 'visited': {}, 'paths': {2: (1, 2)}}
+        ? 2: {'depth': 1, 'visited': {}, 'paths': {2: (1, 2)}}
+        -> 5: {'depth': 2, 'visited': {}, 'paths': {5: (1, 2, 5)}}
+        ? 5: {'depth': 2, 'visited': {}, 'paths': {5: (1, 2, 5)}}
+        -> 4: {'depth': 2, 'visited': {}, 'paths': {4: (1, 2, 4)}}
+        ? 4: {'depth': 2, 'visited': {}, 'paths': {4: (1, 2, 4)}}
         All paths: [(1,), (1, 2), (1, 3), (1, 2, 4), (1, 2, 5), (1, 3, 6), (1, 3, 7)]
         All visited: []
 
         >>> traversal = nog.TraversalNeighborsThenDepth(f.next_vertices, is_tree=True)
         >>> traversal = traversal.start_from(f.start, build_paths=True,
         ...                                  compute_depth=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': set(), 'depth': 0, 'paths[1]': (1,)}
-        ? 1: {'visited': set(), 'depth': 0, 'paths[1]': (1,)}
-        -> 2: {'visited': set(), 'depth': 1, 'paths[2]': (1, 2)}
-        -> 3: {'visited': set(), 'depth': 1, 'paths[3]': (1, 3)}
-        ? 3: {'visited': set(), 'depth': 1, 'paths[3]': (1, 3)}
-        -> 6: {'visited': set(), 'depth': 2, 'paths[6]': (1, 3, 6)}
-        -> 7: {'visited': set(), 'depth': 2, 'paths[7]': (1, 3, 7)}
-        ? 7: {'visited': set(), 'depth': 2, 'paths[7]': (1, 3, 7)}
-        ? 6: {'visited': set(), 'depth': 2, 'paths[6]': (1, 3, 6)}
-        ? 2: {'visited': set(), 'depth': 1, 'paths[2]': (1, 2)}
-        -> 4: {'visited': set(), 'depth': 2, 'paths[4]': (1, 2, 4)}
-        -> 5: {'visited': set(), 'depth': 2, 'paths[5]': (1, 2, 5)}
-        ? 5: {'visited': set(), 'depth': 2, 'paths[5]': (1, 2, 5)}
-        ? 4: {'visited': set(), 'depth': 2, 'paths[4]': (1, 2, 4)}
+        After start: {'depth': 0, 'visited': {}, 'paths': {1: (1,)}}
+        ? 1: {'depth': 0, 'visited': {}, 'paths': {1: (1,)}}
+        -> 2: {'depth': 1, 'visited': {}, 'paths': {2: (1, 2)}}
+        -> 3: {'depth': 1, 'visited': {}, 'paths': {3: (1, 3)}}
+        ? 3: {'depth': 1, 'visited': {}, 'paths': {3: (1, 3)}}
+        -> 6: {'depth': 2, 'visited': {}, 'paths': {6: (1, 3, 6)}}
+        -> 7: {'depth': 2, 'visited': {}, 'paths': {7: (1, 3, 7)}}
+        ? 7: {'depth': 2, 'visited': {}, 'paths': {7: (1, 3, 7)}}
+        ? 6: {'depth': 2, 'visited': {}, 'paths': {6: (1, 3, 6)}}
+        ? 2: {'depth': 1, 'visited': {}, 'paths': {2: (1, 2)}}
+        -> 4: {'depth': 2, 'visited': {}, 'paths': {4: (1, 2, 4)}}
+        -> 5: {'depth': 2, 'visited': {}, 'paths': {5: (1, 2, 5)}}
+        ? 5: {'depth': 2, 'visited': {}, 'paths': {5: (1, 2, 5)}}
+        ? 4: {'depth': 2, 'visited': {}, 'paths': {4: (1, 2, 4)}}
         All paths: [(1,), (1, 2), (1, 3), (1, 2, 4), (1, 2, 5), (1, 3, 6), (1, 3, 7)]
         All visited: []
 
         >>> traversal = nog.TraversalTopologicalSort(f.next_vertices, is_tree=True)
         >>> traversal = traversal.start_from(f.start, build_paths=True)
         >>> results_with_visited(traversal, {f.start})
-        After start: {'visited': set(), 'depth': 0, 'cycle_from_start': [], 'paths[1]':
-          (1,)}
-        ? 1: {'visited': set(), 'depth': 0, 'cycle_from_start': [], 'paths[1]': (1,)}
-        ? 3: {'visited': set(), 'depth': 1, 'cycle_from_start': [], 'paths[3]': (1, 3)}
-        ? 7: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[7]': (1, 3,
-          7)}
-        -> 7: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[7]': (1, 3,
-          7)}
-        ? 6: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[6]': (1, 3,
-          6)}
-        -> 6: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[6]': (1, 3,
-          6)}
-        -> 3: {'visited': set(), 'depth': 1, 'cycle_from_start': [], 'paths[3]': (1, 3)}
-        ? 2: {'visited': set(), 'depth': 1, 'cycle_from_start': [], 'paths[2]': (1, 2)}
-        ? 5: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[5]': (1, 2,
-          5)}
-        -> 5: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[5]': (1, 2,
-          5)}
-        ? 4: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[4]': (1, 2,
-          4)}
-        -> 4: {'visited': set(), 'depth': 2, 'cycle_from_start': [], 'paths[4]': (1, 2,
-          4)}
-        -> 2: {'visited': set(), 'depth': 1, 'cycle_from_start': [], 'paths[2]': (1, 2)}
-        -> 1: {'visited': set(), 'depth': 0, 'cycle_from_start': [], 'paths[1]': (1,)}
+        After start: {'depth': 0, 'cycle_from_start': [], 'visited': {}, 'paths': {1:
+          (1,)}}
+        ? 1: {'depth': 0, 'cycle_from_start': [], 'visited': {}, 'paths': {1: (1,)}}
+        ? 3: {'depth': 1, 'cycle_from_start': [], 'visited': {}, 'paths': {3: (1, 3)}}
+        ? 7: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {7: (1, 3,
+          7)}}
+        -> 7: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {7: (1, 3,
+          7)}}
+        ? 6: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {6: (1, 3,
+          6)}}
+        -> 6: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {6: (1, 3,
+          6)}}
+        -> 3: {'depth': 1, 'cycle_from_start': [], 'visited': {}, 'paths': {3: (1, 3)}}
+        ? 2: {'depth': 1, 'cycle_from_start': [], 'visited': {}, 'paths': {2: (1, 2)}}
+        ? 5: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {5: (1, 2,
+          5)}}
+        -> 5: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {5: (1, 2,
+          5)}}
+        ? 4: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {4: (1, 2,
+          4)}}
+        -> 4: {'depth': 2, 'cycle_from_start': [], 'visited': {}, 'paths': {4: (1, 2,
+          4)}}
+        -> 2: {'depth': 1, 'cycle_from_start': [], 'visited': {}, 'paths': {2: (1, 2)}}
+        -> 1: {'depth': 0, 'cycle_from_start': [], 'visited': {}, 'paths': {1: (1,)}}
         All paths: [(1,), (1, 2), (1, 3), (1, 2, 4), (1, 2, 5), (1, 3, 6), (1, 3, 7)]
         All visited: []
         """
         pass
 
 
 class NormalGraphTraversalsWithWeights:
@@ -1910,22 +1914,23 @@
     First we test without know_distances, and with option keep_distances.
     We also check here, whether distances and paths stay the same from
     start_from till traversal.
     >>> f = FDiamond()
     >>> traversal = nog.TraversalShortestPaths(next_edges=f.next_edges)
     >>> traversal = traversal.start_from(f.start, build_paths=True, keep_distances=True)
     >>> results_with_distances(traversal, {f.start})
-    After start: {'distance': inf, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    ? 0: {'distance': 0, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    -> 2: {'distance': 1, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 1}
-    ? 2: {'distance': 1, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 1}
-    -> 1: {'distance': 2, 'depth': 1, 'paths[1]': (0, 1), 'distances[1]': 2}
-    ? 1: {'distance': 2, 'depth': 1, 'paths[1]': (0, 1), 'distances[1]': 2}
-    -> 3: {'distance': 3, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 3}
-    ? 3: {'distance': 3, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 3}
+    After start: {'distance': inf, 'depth': 0, 'distances': {0: 0}, 'paths': {0:
+      (0,)}}
+    ? 0: {'distance': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 2: {'distance': 1, 'depth': 1, 'distances': {2: 1}, 'paths': {2: (0, 2)}}
+    ? 2: {'distance': 1, 'depth': 1, 'distances': {2: 1}, 'paths': {2: (0, 2)}}
+    -> 1: {'distance': 2, 'depth': 1, 'distances': {1: 2}, 'paths': {1: (0, 1)}}
+    ? 1: {'distance': 2, 'depth': 1, 'distances': {1: 2}, 'paths': {1: (0, 1)}}
+    -> 3: {'distance': 3, 'depth': 2, 'distances': {3: 3}, 'paths': {3: (0, 2, 3)}}
+    ? 3: {'distance': 3, 'depth': 2, 'distances': {3: 3}, 'paths': {3: (0, 2, 3)}}
     All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
     All distances: {0: 0, 1: 2, 2: 1, 3: 3}
 
 
     Now we test with known_distances, but without option keep_distances.
     Start vertex starts with distance 2, and we pretend to have a path to 1 with
     distance 0. Effect: All reported distances are 2 higher than in the test before,
@@ -1933,101 +1938,107 @@
     reported at all, because no path can be found that beats this "already found" low
     distance. Due to keep_distances==False, the distances to 2 and 3 are deleted.
     >>> known_distances = collections.defaultdict(
     ...     lambda: infinity, f.values_for_known_distances)
     >>> traversal = traversal.start_from(
     ...     f.start, build_paths=True, known_distances=known_distances)
     >>> results_with_distances(traversal, {f.start})
-    After start: {'distance': inf, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 2}
-    ? 0: {'distance': 2, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    -> 2: {'distance': 3, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 0}
-    ? 2: {'distance': 3, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 0}
-    -> 3: {'distance': 5, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 0}
-    ? 3: {'distance': 5, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 0}
+    After start: {'distance': inf, 'depth': 0, 'distances': {0: 2}, 'paths': {0:
+      (0,)}}
+    ? 0: {'distance': 2, 'depth': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 2: {'distance': 3, 'depth': 1, 'distances': {2: 0}, 'paths': {2: (0, 2)}}
+    ? 2: {'distance': 3, 'depth': 1, 'distances': {2: 0}, 'paths': {2: (0, 2)}}
+    -> 3: {'distance': 5, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (0, 2, 3)}}
+    ? 3: {'distance': 5, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (0, 2, 3)}}
     All paths: [(0,), (0, 2), (0, 2, 3)]
     All distances: {0: 0, 1: 0, 2: 0, 3: 0}
     >>> traversal.distances is known_distances
     True
 
     The same again, but with a sequence-based known_distances
     >>> gear = nog.GearForIntVertexIDsAndIntsMaybeFloats()
     >>> known_distances = gear.vertex_id_to_distance_mapping(())
     >>> known_distances.update(f.values_for_known_distances)
     >>> traversal = traversal.start_from(
     ...     f.start, build_paths=True, known_distances=known_distances)
     >>> results_with_distances(traversal, {f.start})
-    After start: {'distance': inf, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 2}
-    ? 0: {'distance': 2, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    -> 2: {'distance': 3, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 0}
-    ? 2: {'distance': 3, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 0}
-    -> 3: {'distance': 5, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 0}
-    ? 3: {'distance': 5, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 0}
+    After start: {'distance': inf, 'depth': 0, 'distances': {0: 2}, 'paths': {0:
+      (0,)}}
+    ? 0: {'distance': 2, 'depth': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 2: {'distance': 3, 'depth': 1, 'distances': {2: 0}, 'paths': {2: (0, 2)}}
+    ? 2: {'distance': 3, 'depth': 1, 'distances': {2: 0}, 'paths': {2: (0, 2)}}
+    -> 3: {'distance': 5, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (0, 2, 3)}}
+    ? 3: {'distance': 5, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (0, 2, 3)}}
     All paths: [(0,), (0, 2), (0, 2, 3)]
     All distances: {0: 0, 1: 0, 2: 0, 3: 0}
     >>> traversal.distances is known_distances
     True
 
 
     -- TraversalMinimumSpanningTree --
     >>> fmst = FDiamond2()
     >>> traversal = nog.TraversalMinimumSpanningTree(next_edges=fmst.next_edges)
     >>> traversal = traversal.start_from(fmst.start, build_paths=True)
     >>> results_standard(traversal, {fmst.start})
-    After start: {'edge': None, 'paths[0]': (0,)}
-    ? 0: {'edge': None, 'paths[0]': (0,)}
-    -> 2: {'edge': (0, 2, 1), 'paths[2]': (0, 2)}
-    ? 2: {'edge': (0, 2, 1), 'paths[2]': (0, 2)}
-    -> 1: {'edge': (0, 1, 2), 'paths[1]': (0, 1)}
-    ? 1: {'edge': (0, 1, 2), 'paths[1]': (0, 1)}
-    -> 3: {'edge': (2, 3, 3), 'paths[3]': (0, 2, 3)}
-    ? 3: {'edge': (2, 3, 3), 'paths[3]': (0, 2, 3)}
+    After start: {'edge': None, 'paths': {0: (0,)}}
+    ? 0: {'edge': None, 'paths': {0: (0,)}}
+    -> 2: {'edge': (0, 2, 1), 'paths': {2: (0, 2)}}
+    ? 2: {'edge': (0, 2, 1), 'paths': {2: (0, 2)}}
+    -> 1: {'edge': (0, 1, 2), 'paths': {1: (0, 1)}}
+    ? 1: {'edge': (0, 1, 2), 'paths': {1: (0, 1)}}
+    -> 3: {'edge': (2, 3, 3), 'paths': {3: (0, 2, 3)}}
+    ? 3: {'edge': (2, 3, 3), 'paths': {3: (0, 2, 3)}}
     All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
 
 
     -- TraversaAStar --
     Typically, one would use go_to(3) for our goal vertex 3, but for
     the test purposes we continue to iterate the rest of the graph.
     >>> fa = FAStar()
     >>> traversal = nog.TraversalAStar(next_edges=fa.next_edges)
     >>> traversal = traversal.start_from(fa.heuristic, fa.start, build_paths=True)
     >>> results_standard(traversal, {fa.start})
-    After start: {'path_length': inf, 'depth': 0, 'paths[0]': (0,), 'distances[0]':
-      0}
-    ? 0: {'path_length': 0, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    -> 1: {'path_length': 3, 'depth': 1, 'paths[1]': (0, 1), 'distances[1]': 3}
-    ? 1: {'path_length': 3, 'depth': 1, 'paths[1]': (0, 1), 'distances[1]': 3}
-    -> 2: {'path_length': 3, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 3}
-    ? 2: {'path_length': 3, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 3}
-    -> 3: {'path_length': 5, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 5}
-    ? 3: {'path_length': 5, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 5}
-    -> 4: {'path_length': 1, 'depth': 1, 'paths[4]': (0, 4), 'distances[4]': 1}
-    ? 4: {'path_length': 1, 'depth': 1, 'paths[4]': (0, 4), 'distances[4]': 1}
+    After start: {'path_length': inf, 'depth': 0, 'distances': {0: 0}, 'paths': {0:
+      (0,)}}
+    ? 0: {'path_length': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 1: {'path_length': 3, 'depth': 1, 'distances': {1: 3}, 'paths': {1: (0, 1)}}
+    ? 1: {'path_length': 3, 'depth': 1, 'distances': {1: 3}, 'paths': {1: (0, 1)}}
+    -> 2: {'path_length': 3, 'depth': 1, 'distances': {2: 3}, 'paths': {2: (0, 2)}}
+    ? 2: {'path_length': 3, 'depth': 1, 'distances': {2: 3}, 'paths': {2: (0, 2)}}
+    -> 3: {'path_length': 5, 'depth': 2, 'distances': {3: 5}, 'paths': {3: (0, 2,
+      3)}}
+    ? 3: {'path_length': 5, 'depth': 2, 'distances': {3: 5}, 'paths': {3: (0, 2,
+      3)}}
+    -> 4: {'path_length': 1, 'depth': 1, 'distances': {4: 1}, 'paths': {4: (0, 4)}}
+    ? 4: {'path_length': 1, 'depth': 1, 'distances': {4: 1}, 'paths': {4: (0, 4)}}
     All paths: [(0,), (0, 1), (0, 2), (0, 2, 3), (0, 4)]
 
 
     Variant of the test with option known_distances.
     For the start vertex, we define a start distance. Effect: All distances are now 2
     higher. For vertex 1, we define an artificial and low distance of 0. Effect: it is
     not visited.
     >>> known_distances = collections.defaultdict(
     ...     lambda: infinity, fa.values_for_known_distances)
     >>> known_path_length_guesses = collections.defaultdict(lambda: infinity)
     >>> traversal = traversal.start_from(fa.heuristic, fa.start, build_paths=True,
     ...     known_distances=known_distances,
     ...     known_path_length_guesses=known_path_length_guesses)
     >>> results_standard(traversal, {fa.start})
-    After start: {'path_length': inf, 'depth': 0, 'paths[0]': (0,), 'distances[0]':
-      2}
-    ? 0: {'path_length': 2, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 2}
-    -> 2: {'path_length': 5, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 5}
-    ? 2: {'path_length': 5, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 5}
-    -> 3: {'path_length': 7, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 7}
-    ? 3: {'path_length': 7, 'depth': 2, 'paths[3]': (0, 2, 3), 'distances[3]': 7}
-    -> 4: {'path_length': 3, 'depth': 1, 'paths[4]': (0, 4), 'distances[4]': 3}
-    ? 4: {'path_length': 3, 'depth': 1, 'paths[4]': (0, 4), 'distances[4]': 3}
+    After start: {'path_length': inf, 'depth': 0, 'distances': {0: 2}, 'paths': {0:
+      (0,)}}
+    ? 0: {'path_length': 2, 'depth': 0, 'distances': {0: 2}, 'paths': {0: (0,)}}
+    -> 2: {'path_length': 5, 'depth': 1, 'distances': {2: 5}, 'paths': {2: (0, 2)}}
+    ? 2: {'path_length': 5, 'depth': 1, 'distances': {2: 5}, 'paths': {2: (0, 2)}}
+    -> 3: {'path_length': 7, 'depth': 2, 'distances': {3: 7}, 'paths': {3: (0, 2,
+      3)}}
+    ? 3: {'path_length': 7, 'depth': 2, 'distances': {3: 7}, 'paths': {3: (0, 2,
+      3)}}
+    -> 4: {'path_length': 3, 'depth': 1, 'distances': {4: 3}, 'paths': {4: (0, 4)}}
+    ? 4: {'path_length': 3, 'depth': 1, 'distances': {4: 3}, 'paths': {4: (0, 4)}}
     All paths: [(0,), (0, 2), (0, 2, 3), (0, 4)]
     >>> print("Distance at goal:", known_distances[fa.goal])
     Distance at goal: 7
     >>> print("Best distances found so far:", dict(known_distances))
     Best distances found so far: {0: 2, 1: 0, 2: 5, 4: 3, 3: 7}
     >>> print("Best path len guesses found so far):", dict(known_path_length_guesses))
     Best path len guesses found so far): {0: 8, 2: 7, 4: inf, 3: 7}
@@ -2058,51 +2069,65 @@
 
     All traversals, with option is_tree (except for MST and BSearchShortestPath,
     they do not have the option):
     >>> fsb = FSmallBinaryTree()
     >>> traversal = nog.TraversalShortestPaths(fsb.next_edges, is_tree=True)
     >>> traversal = traversal.start_from(fsb.start, build_paths=True)
     >>> results_with_distances(traversal, {fsb.start})
-    After start: {'distance': inf, 'depth': 0, 'paths[1]': (1,), 'distances[1]': 0}
-    ? 1: {'distance': 0, 'depth': 0, 'paths[1]': (1,), 'distances[1]': 0}
-    -> 2: {'distance': 2, 'depth': 1, 'paths[2]': (1, 2), 'distances[2]': inf}
-    ? 2: {'distance': 2, 'depth': 1, 'paths[2]': (1, 2), 'distances[2]': inf}
-    -> 3: {'distance': 3, 'depth': 1, 'paths[3]': (1, 3), 'distances[3]': inf}
-    ? 3: {'distance': 3, 'depth': 1, 'paths[3]': (1, 3), 'distances[3]': inf}
-    -> 4: {'distance': 6, 'depth': 2, 'paths[4]': (1, 2, 4), 'distances[4]': inf}
-    ? 4: {'distance': 6, 'depth': 2, 'paths[4]': (1, 2, 4), 'distances[4]': inf}
-    -> 5: {'distance': 7, 'depth': 2, 'paths[5]': (1, 2, 5), 'distances[5]': inf}
-    ? 5: {'distance': 7, 'depth': 2, 'paths[5]': (1, 2, 5), 'distances[5]': inf}
-    -> 6: {'distance': 9, 'depth': 2, 'paths[6]': (1, 3, 6), 'distances[6]': inf}
-    ? 6: {'distance': 9, 'depth': 2, 'paths[6]': (1, 3, 6), 'distances[6]': inf}
-    -> 7: {'distance': 10, 'depth': 2, 'paths[7]': (1, 3, 7), 'distances[7]': inf}
-    ? 7: {'distance': 10, 'depth': 2, 'paths[7]': (1, 3, 7), 'distances[7]': inf}
+    After start: {'distance': inf, 'depth': 0, 'distances': {1: 0}, 'paths': {1:
+      (1,)}}
+    ? 1: {'distance': 0, 'depth': 0, 'distances': {1: 0}, 'paths': {1: (1,)}}
+    -> 2: {'distance': 2, 'depth': 1, 'distances': {2: inf}, 'paths': {2: (1, 2)}}
+    ? 2: {'distance': 2, 'depth': 1, 'distances': {2: inf}, 'paths': {2: (1, 2)}}
+    -> 3: {'distance': 3, 'depth': 1, 'distances': {3: inf}, 'paths': {3: (1, 3)}}
+    ? 3: {'distance': 3, 'depth': 1, 'distances': {3: inf}, 'paths': {3: (1, 3)}}
+    -> 4: {'distance': 6, 'depth': 2, 'distances': {4: inf}, 'paths': {4: (1, 2,
+      4)}}
+    ? 4: {'distance': 6, 'depth': 2, 'distances': {4: inf}, 'paths': {4: (1, 2, 4)}}
+    -> 5: {'distance': 7, 'depth': 2, 'distances': {5: inf}, 'paths': {5: (1, 2,
+      5)}}
+    ? 5: {'distance': 7, 'depth': 2, 'distances': {5: inf}, 'paths': {5: (1, 2, 5)}}
+    -> 6: {'distance': 9, 'depth': 2, 'distances': {6: inf}, 'paths': {6: (1, 3,
+      6)}}
+    ? 6: {'distance': 9, 'depth': 2, 'distances': {6: inf}, 'paths': {6: (1, 3, 6)}}
+    -> 7: {'distance': 10, 'depth': 2, 'distances': {7: inf}, 'paths': {7: (1, 3,
+      7)}}
+    ? 7: {'distance': 10, 'depth': 2, 'distances': {7: inf}, 'paths': {7: (1, 3,
+      7)}}
     All paths: [(1,), (1, 2), (1, 3), (1, 2, 4), (1, 2, 5), (1, 3, 6), (1, 3, 7)]
     All distances: {1: 0, 2: inf, 3: inf, 4: inf, 5: inf, 6: inf, 7: inf}
 
     Test TraversaAStar. Typically, one would use go_to(6) for our goal vertex 6, but for
     the test purposes we continue to iterate the rest of the graph.
     >>> traversal = nog.TraversalAStar(next_edges=fsb.next_edges)
     >>> traversal = traversal.start_from(fsb.heuristic, fsb.start, build_paths=True)
     >>> results_standard(traversal, {fsb.start})
-    After start: {'path_length': inf, 'depth': 0, 'paths[1]': (1,), 'distances[1]':
-      0}
-    ? 1: {'path_length': 0, 'depth': 0, 'paths[1]': (1,), 'distances[1]': 0}
-    -> 3: {'path_length': 3, 'depth': 1, 'paths[3]': (1, 3), 'distances[3]': 3}
-    ? 3: {'path_length': 3, 'depth': 1, 'paths[3]': (1, 3), 'distances[3]': 3}
-    -> 6: {'path_length': 9, 'depth': 2, 'paths[6]': (1, 3, 6), 'distances[6]': 9}
-    ? 6: {'path_length': 9, 'depth': 2, 'paths[6]': (1, 3, 6), 'distances[6]': 9}
-    -> 2: {'path_length': 2, 'depth': 1, 'paths[2]': (1, 2), 'distances[2]': 2}
-    ? 2: {'path_length': 2, 'depth': 1, 'paths[2]': (1, 2), 'distances[2]': 2}
-    -> 4: {'path_length': 6, 'depth': 2, 'paths[4]': (1, 2, 4), 'distances[4]': 6}
-    ? 4: {'path_length': 6, 'depth': 2, 'paths[4]': (1, 2, 4), 'distances[4]': 6}
-    -> 5: {'path_length': 7, 'depth': 2, 'paths[5]': (1, 2, 5), 'distances[5]': 7}
-    ? 5: {'path_length': 7, 'depth': 2, 'paths[5]': (1, 2, 5), 'distances[5]': 7}
-    -> 7: {'path_length': 10, 'depth': 2, 'paths[7]': (1, 3, 7), 'distances[7]': 10}
-    ? 7: {'path_length': 10, 'depth': 2, 'paths[7]': (1, 3, 7), 'distances[7]': 10}
+    After start: {'path_length': inf, 'depth': 0, 'distances': {1: 0}, 'paths': {1:
+      (1,)}}
+    ? 1: {'path_length': 0, 'depth': 0, 'distances': {1: 0}, 'paths': {1: (1,)}}
+    -> 3: {'path_length': 3, 'depth': 1, 'distances': {3: 3}, 'paths': {3: (1, 3)}}
+    ? 3: {'path_length': 3, 'depth': 1, 'distances': {3: 3}, 'paths': {3: (1, 3)}}
+    -> 6: {'path_length': 9, 'depth': 2, 'distances': {6: 9}, 'paths': {6: (1, 3,
+      6)}}
+    ? 6: {'path_length': 9, 'depth': 2, 'distances': {6: 9}, 'paths': {6: (1, 3,
+      6)}}
+    -> 2: {'path_length': 2, 'depth': 1, 'distances': {2: 2}, 'paths': {2: (1, 2)}}
+    ? 2: {'path_length': 2, 'depth': 1, 'distances': {2: 2}, 'paths': {2: (1, 2)}}
+    -> 4: {'path_length': 6, 'depth': 2, 'distances': {4: 6}, 'paths': {4: (1, 2,
+      4)}}
+    ? 4: {'path_length': 6, 'depth': 2, 'distances': {4: 6}, 'paths': {4: (1, 2,
+      4)}}
+    -> 5: {'path_length': 7, 'depth': 2, 'distances': {5: 7}, 'paths': {5: (1, 2,
+      5)}}
+    ? 5: {'path_length': 7, 'depth': 2, 'distances': {5: 7}, 'paths': {5: (1, 2,
+      5)}}
+    -> 7: {'path_length': 10, 'depth': 2, 'distances': {7: 10}, 'paths': {7: (1, 3,
+      7)}}
+    ? 7: {'path_length': 10, 'depth': 2, 'distances': {7: 10}, 'paths': {7: (1, 3,
+      7)}}
     All paths: [(1,), (1, 2), (1, 3), (1, 2, 4), (1, 2, 5), (1, 3, 6), (1, 3, 7)]
     """
 
 
 class MultipleOrNoneStartVerticesTraversalsWithOrWithoutLabels:
     """-- Traversal with none or multiple start vertices, first 3 traversal strategies
     Checks: Correct traversal of TraversalBreadthFirst, TraversalDepthFirst,
@@ -2117,173 +2142,173 @@
     1. Unlabeled edges
     >>> f = FMultiStart()
     >>> fb = FMultiStartB()
 
     >>> t = nog.TraversalBreadthFirst(f.next_vertices).start_from(
     ...      start_vertices=f.start_vertices, build_paths=True)
     >>> results_with_visited(t, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 0: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,)}
-    -> 1: {'visited': {0, 1, 5}, 'depth': 1, 'paths[1]': (0, 1)}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0, 'paths[5]': (5,)}
-    -> 6: {'visited': {0, 1, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    ? 1: {'visited': {0, 1, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    -> 2: {'visited': {0, 1, 2, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    ? 6: {'visited': {0, 1, 2, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    -> 3: {'visited': {0, 1, 2, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 2: {'visited': {0, 1, 2, 3, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    -> 4: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (0, 1, 2, 4)}
-    ? 3: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 4: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (0, 1, 2, 4)}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,), 5: (5,)}}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,)}}
+    -> 1: {'depth': 1, 'visited': {0, 1, 5}, 'paths': {1: (0, 1)}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
+    -> 6: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {6: (5, 6)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {1: (0, 1)}}
+    -> 2: {'depth': 2, 'visited': {0, 1, 2, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    ? 6: {'depth': 1, 'visited': {0, 1, 2, 5, 6}, 'paths': {6: (5, 6)}}
+    -> 3: {'depth': 2, 'visited': {0, 1, 2, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 2: {'depth': 2, 'visited': {0, 1, 2, 3, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    -> 4: {'depth': 3, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {4: (0, 1, 2, 4)}}
+    ? 3: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 4: {'depth': 3, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {4: (0, 1, 2, 4)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (0, 1, 2, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
     >>> list(t.start_from(start_vertices=(), build_paths=True))
     []
     >>> list(t.start_from(start_vertices=f.start_vertices, build_paths=True
     ...     ).go_for_vertices_in([]))
     []
 
     For TraversalDepthFirst, we need to specify compute_depth to get depth.
     And we need to check the extra execution path for the case without depth and paths.
     >>> t = nog.TraversalDepthFirst(f.next_vertices).start_from(
     ...      start_vertices=f.start_vertices, build_paths=True, compute_depth=True)
     >>> results_with_visited(t, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 5: {'visited': {0, 5}, 'depth': 0, 'paths[5]': (5,)}
-    -> 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    ? 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    -> 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'paths[0]': (0,)}
-    -> 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,), 5: (5,)}}
+    ? 5: {'depth': 0, 'visited': {0, 5}, 'paths': {5: (5,)}}
+    -> 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    ? 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    -> 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    -> 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 0: {'depth': 0, 'visited': {0, 3, 4, 5, 6}, 'paths': {0: (0,)}}
+    -> 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    -> 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    ? 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
     >>> _ = t.start_from(start_vertices=f.start_vertices)
     >>> results_with_visited(t, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0}
-    ? 5: {'visited': {0, 5}, 'depth': -1}
-    -> 6: {'visited': {0, 5, 6}, 'depth': -1}
-    ? 6: {'visited': {0, 5, 6}, 'depth': -1}
-    -> 3: {'visited': {0, 3, 5, 6}, 'depth': -1}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': -1}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': -1}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': -1}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': -1}
-    -> 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': -1}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': -1}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': -1}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': -1}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {}}
+    ? 5: {'depth': -1, 'visited': {0, 5}, 'paths': {}}
+    -> 6: {'depth': -1, 'visited': {0, 5, 6}, 'paths': {}}
+    ? 6: {'depth': -1, 'visited': {0, 5, 6}, 'paths': {}}
+    -> 3: {'depth': -1, 'visited': {0, 3, 5, 6}, 'paths': {}}
+    ? 3: {'depth': -1, 'visited': {0, 3, 5, 6}, 'paths': {}}
+    -> 4: {'depth': -1, 'visited': {0, 3, 4, 5, 6}, 'paths': {}}
+    ? 4: {'depth': -1, 'visited': {0, 3, 4, 5, 6}, 'paths': {}}
+    ? 0: {'depth': -1, 'visited': {0, 3, 4, 5, 6}, 'paths': {}}
+    -> 1: {'depth': -1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {}}
+    ? 1: {'depth': -1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {}}
+    -> 2: {'depth': -1, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {}}
+    ? 2: {'depth': -1, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {}}
     All visited: [0, 1, 2, 3, 4, 5, 6]
     >>> list(t.start_from(start_vertices=(), build_paths=True))
     []
     >>> list(t.start_from(start_vertices=f.start_vertices, build_paths=True
     ...     ).go_for_vertices_in([]))
     []
 
     For TraversalNeighborsThenDepth, we need to specify compute_depth to get depth.
     And we need to check the extra execution path for the case without depth and paths.
     >>> t = nog.TraversalNeighborsThenDepth(f.next_vertices).start_from(
     ...      start_vertices=f.start_vertices, build_paths=True, compute_depth=True)
     >>> results_with_visited(t, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 5: {'visited': {0, 5}, 'depth': 0, 'paths[5]': (5,)}
-    -> 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    ? 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    -> 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'paths[0]': (0,)}
-    -> 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,), 5: (5,)}}
+    ? 5: {'depth': 0, 'visited': {0, 5}, 'paths': {5: (5,)}}
+    -> 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    ? 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    -> 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    -> 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 0: {'depth': 0, 'visited': {0, 3, 4, 5, 6}, 'paths': {0: (0,)}}
+    -> 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    -> 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    ? 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
     >>> _ = t.start_from(start_vertices=f.start_vertices)
     >>> results_with_visited(t, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0}
-    ? 5: {'visited': {0, 5}, 'depth': -1}
-    -> 6: {'visited': {0, 5, 6}, 'depth': -1}
-    ? 6: {'visited': {0, 5, 6}, 'depth': -1}
-    -> 3: {'visited': {0, 3, 5, 6}, 'depth': -1}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': -1}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': -1}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': -1}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': -1}
-    -> 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': -1}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': -1}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': -1}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': -1}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {}}
+    ? 5: {'depth': -1, 'visited': {0, 5}, 'paths': {}}
+    -> 6: {'depth': -1, 'visited': {0, 5, 6}, 'paths': {}}
+    ? 6: {'depth': -1, 'visited': {0, 5, 6}, 'paths': {}}
+    -> 3: {'depth': -1, 'visited': {0, 3, 5, 6}, 'paths': {}}
+    ? 3: {'depth': -1, 'visited': {0, 3, 5, 6}, 'paths': {}}
+    -> 4: {'depth': -1, 'visited': {0, 3, 4, 5, 6}, 'paths': {}}
+    ? 4: {'depth': -1, 'visited': {0, 3, 4, 5, 6}, 'paths': {}}
+    ? 0: {'depth': -1, 'visited': {0, 3, 4, 5, 6}, 'paths': {}}
+    -> 1: {'depth': -1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {}}
+    ? 1: {'depth': -1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {}}
+    -> 2: {'depth': -1, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {}}
+    ? 2: {'depth': -1, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {}}
     All visited: [0, 1, 2, 3, 4, 5, 6]
     >>> list(t.start_from(start_vertices=(), build_paths=True))
     []
     >>> list(t.start_from(start_vertices=f.start_vertices, build_paths=True
     ...     ).go_for_vertices_in([]))
     []
 
     >>> t = nog.TraversalTopologicalSort(f.next_vertices).start_from(
     ...      start_vertices=f.start_vertices, build_paths=True)
     >>> results_with_visited(t, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-      (0,), 'paths[5]': (5,)}
-    ? 5: {'visited': {0, 5}, 'depth': 0, 'cycle_from_start': [], 'paths[5]': (5,)}
-    ? 6: {'visited': {0, 5, 6}, 'depth': 1, 'cycle_from_start': [], 'paths[6]': (5,
-      6)}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'cycle_from_start': [], 'paths[3]':
-      (5, 6, 3)}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'cycle_from_start': [],
-      'paths[4]': (5, 6, 3, 4)}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'cycle_from_start': [],
-      'paths[4]': (5, 6, 3, 4)}
-    -> 3: {'visited': {0, 3, 4, 5, 6}, 'depth': 2, 'cycle_from_start': [],
-      'paths[3]': (5, 6, 3)}
-    -> 6: {'visited': {0, 3, 4, 5, 6}, 'depth': 1, 'cycle_from_start': [],
-      'paths[6]': (5, 6)}
-    -> 5: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'cycle_from_start': [],
-      'paths[5]': (5,)}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'cycle_from_start': [],
-      'paths[0]': (0,)}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'cycle_from_start': [],
-      'paths[1]': (0, 1)}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'cycle_from_start': [],
-      'paths[2]': (0, 1, 2)}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'cycle_from_start': [],
-      'paths[2]': (0, 1, 2)}
-    -> 1: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 1, 'cycle_from_start': [],
-      'paths[1]': (0, 1)}
-    -> 0: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 0, 'cycle_from_start': [],
-      'paths[0]': (0,)}
+    After start: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 5}, 'paths':
+      {0: (0,), 5: (5,)}}
+    ? 5: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 5}, 'paths': {5: (5,)}}
+    ? 6: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 5, 6}, 'paths': {6: (5,
+      6)}}
+    ? 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 3, 5, 6}, 'paths': {3:
+      (5, 6, 3)}}
+    ? 4: {'depth': 3, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {4: (5, 6, 3, 4)}}
+    -> 4: {'depth': 3, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {4: (5, 6, 3, 4)}}
+    -> 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {3: (5, 6, 3)}}
+    -> 6: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {6: (5, 6)}}
+    -> 5: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {5: (5,)}}
+    ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {0: (0,)}}
+    ? 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 3, 4, 5, 6},
+      'paths': {1: (0, 1)}}
+    ? 2: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {2: (0, 1, 2)}}
+    -> 2: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {2: (0, 1, 2)}}
+    -> 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {1: (0, 1)}}
+    -> 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {0: (0,)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
     >>> list(t.start_from(start_vertices=(), build_paths=True))
     []
     >>> list(t.start_from(start_vertices=f.start_vertices, build_paths=True
     ...     ).go_for_vertices_in([]))
     []
 
     >>> l, p = nog.BSearchBreadthFirst(fb.next_vertices_bi
     ...     ).start_from(start_and_goal_vertices=fb.start_vertices_bi)
-    ? 0: {'visited': {0, 5}, 'depth': 0}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0}
-    ?<4: {'visited': {4}, 'depth': 0}
-    ? 1: {'visited': {0, 1, 5, 6}, 'depth': 1}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {}}
+    ?<4: {'depth': 0, 'visited': {4}, 'paths': {}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {}}
     >>> print(l, f.goal not in p)
     3 True
     >>> l, p = nog.BSearchBreadthFirst(fb.next_vertices_bi
     ...     ).start_from(start_and_goal_vertices=fb.start_vertices_bi, build_path=True)
-    ? 0: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,)}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0, 'paths[5]': (5,)}
-    ?<4: {'visited': {4}, 'depth': 0, 'paths[4]': (4,)}
-    ? 1: {'visited': {0, 1, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,)}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
+    ?<4: {'depth': 0, 'visited': {4}, 'paths': {4: (4,)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {1: (0, 1)}}
     >>> print(l, list(p))
     3 [0, 1, 2, 4]
 
     >>> l, p = nog.BSearchBreadthFirst(fb.next_vertices_bi
     ...     ).start_from(start_and_goal_vertices=((), ()))
     Traceback (most recent call last):
     KeyError: 'No path to (a) goal vertex found'
@@ -2299,117 +2324,117 @@
     Search in graph with reversed edges and with exchanged start and goal vertices.
     Since we exchange the adjacency functions instead of defining new ones with
     correct reporting, the edge directions reported below are to be interpreted in
     reversed directions.
     >>> l, p = nog.BSearchBreadthFirst(tuple(reversed(fb.next_vertices_bi))
     ...     ).start_from(start_and_goal_vertices=tuple(reversed(fb.start_vertices_bi)),
     ...                  build_path=True)
-    ?<4: {'visited': {4}, 'depth': 0, 'paths[4]': (4,)}
-    ? 0: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,)}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0, 'paths[5]': (5,)}
-    ?<2: {'visited': {2, 3, 4}, 'depth': 1, 'paths[2]': (4, 2)}
+    ?<4: {'depth': 0, 'visited': {4}, 'paths': {4: (4,)}}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,)}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
+    ?<2: {'depth': 1, 'visited': {2, 3, 4}, 'paths': {2: (4, 2)}}
     >>> print(l, list(p))
     3 [4, 2, 1, 0]
 
     2. Labeled edges
     >>> traversal = nog.TraversalBreadthFirst(
     ...     next_edges=f.next_edges
     ... ).start_from(start_vertices=f.start_vertices, build_paths=True)
     >>> results_with_visited(traversal, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 0: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,)}
-    -> 1: {'visited': {0, 1, 5}, 'depth': 1, 'paths[1]': (0, 1)}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0, 'paths[5]': (5,)}
-    -> 6: {'visited': {0, 1, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    ? 1: {'visited': {0, 1, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    -> 2: {'visited': {0, 1, 2, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    ? 6: {'visited': {0, 1, 2, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    -> 3: {'visited': {0, 1, 2, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 2: {'visited': {0, 1, 2, 3, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    -> 4: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (0, 1, 2, 4)}
-    ? 3: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 4: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (0, 1, 2, 4)}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,), 5: (5,)}}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,)}}
+    -> 1: {'depth': 1, 'visited': {0, 1, 5}, 'paths': {1: (0, 1)}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
+    -> 6: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {6: (5, 6)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {1: (0, 1)}}
+    -> 2: {'depth': 2, 'visited': {0, 1, 2, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    ? 6: {'depth': 1, 'visited': {0, 1, 2, 5, 6}, 'paths': {6: (5, 6)}}
+    -> 3: {'depth': 2, 'visited': {0, 1, 2, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 2: {'depth': 2, 'visited': {0, 1, 2, 3, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    -> 4: {'depth': 3, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {4: (0, 1, 2, 4)}}
+    ? 3: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 4: {'depth': 3, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {4: (0, 1, 2, 4)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (0, 1, 2, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
 
     >>> traversal = nog.TraversalDepthFirst(
     ...     next_edges=f.next_edges
     ... ).start_from(
     ...     start_vertices=f.start_vertices, build_paths=True, compute_depth=True)
     >>> results_with_visited(traversal, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 5: {'visited': {0, 5}, 'depth': 0, 'paths[5]': (5,)}
-    -> 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    ? 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    -> 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'paths[0]': (0,)}
-    -> 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,), 5: (5,)}}
+    ? 5: {'depth': 0, 'visited': {0, 5}, 'paths': {5: (5,)}}
+    -> 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    ? 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    -> 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    -> 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 0: {'depth': 0, 'visited': {0, 3, 4, 5, 6}, 'paths': {0: (0,)}}
+    -> 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    -> 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    ? 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
 
     >>> traversal = nog.TraversalNeighborsThenDepth(
     ...     next_edges=f.next_edges
     ... ).start_from(
     ...     start_vertices=f.start_vertices, build_paths=True, compute_depth=True)
     >>> results_with_visited(traversal, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 5: {'visited': {0, 5}, 'depth': 0, 'paths[5]': (5,)}
-    -> 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    ? 6: {'visited': {0, 5, 6}, 'depth': 1, 'paths[6]': (5, 6)}
-    -> 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'paths[3]': (5, 6, 3)}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'paths[4]': (5, 6, 3, 4)}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'paths[0]': (0,)}
-    -> 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'paths[2]': (0, 1, 2)}
+    After start: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,), 5: (5,)}}
+    ? 5: {'depth': 0, 'visited': {0, 5}, 'paths': {5: (5,)}}
+    -> 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    ? 6: {'depth': 1, 'visited': {0, 5, 6}, 'paths': {6: (5, 6)}}
+    -> 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    ? 3: {'depth': 2, 'visited': {0, 3, 5, 6}, 'paths': {3: (5, 6, 3)}}
+    -> 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 4: {'depth': 3, 'visited': {0, 3, 4, 5, 6}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 0: {'depth': 0, 'visited': {0, 3, 4, 5, 6}, 'paths': {0: (0,)}}
+    -> 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 3, 4, 5, 6}, 'paths': {1: (0, 1)}}
+    -> 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
+    ? 2: {'depth': 2, 'visited': {0, 1, 2, 3, 4, 5, 6}, 'paths': {2: (0, 1, 2)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
 
     >>> traversal = nog.TraversalTopologicalSort(
     ...     next_edges=f.next_edges
     ... ).start_from(start_vertices=f.start_vertices, build_paths=True)
     >>> results_with_visited(traversal, f.start_vertices)
-    After start: {'visited': {0, 5}, 'depth': 0, 'cycle_from_start': [], 'paths[0]':
-      (0,), 'paths[5]': (5,)}
-    ? 5: {'visited': {0, 5}, 'depth': 0, 'cycle_from_start': [], 'paths[5]': (5,)}
-    ? 6: {'visited': {0, 5, 6}, 'depth': 1, 'cycle_from_start': [], 'paths[6]': (5,
-      6)}
-    ? 3: {'visited': {0, 3, 5, 6}, 'depth': 2, 'cycle_from_start': [], 'paths[3]':
-      (5, 6, 3)}
-    ? 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'cycle_from_start': [],
-      'paths[4]': (5, 6, 3, 4)}
-    -> 4: {'visited': {0, 3, 4, 5, 6}, 'depth': 3, 'cycle_from_start': [],
-      'paths[4]': (5, 6, 3, 4)}
-    -> 3: {'visited': {0, 3, 4, 5, 6}, 'depth': 2, 'cycle_from_start': [],
-      'paths[3]': (5, 6, 3)}
-    -> 6: {'visited': {0, 3, 4, 5, 6}, 'depth': 1, 'cycle_from_start': [],
-      'paths[6]': (5, 6)}
-    -> 5: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'cycle_from_start': [],
-      'paths[5]': (5,)}
-    ? 0: {'visited': {0, 3, 4, 5, 6}, 'depth': 0, 'cycle_from_start': [],
-      'paths[0]': (0,)}
-    ? 1: {'visited': {0, 1, 3, 4, 5, 6}, 'depth': 1, 'cycle_from_start': [],
-      'paths[1]': (0, 1)}
-    ? 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'cycle_from_start': [],
-      'paths[2]': (0, 1, 2)}
-    -> 2: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 2, 'cycle_from_start': [],
-      'paths[2]': (0, 1, 2)}
-    -> 1: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 1, 'cycle_from_start': [],
-      'paths[1]': (0, 1)}
-    -> 0: {'visited': {0, 1, 2, 3, 4, 5, 6}, 'depth': 0, 'cycle_from_start': [],
-      'paths[0]': (0,)}
+    After start: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 5}, 'paths':
+      {0: (0,), 5: (5,)}}
+    ? 5: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 5}, 'paths': {5: (5,)}}
+    ? 6: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 5, 6}, 'paths': {6: (5,
+      6)}}
+    ? 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 3, 5, 6}, 'paths': {3:
+      (5, 6, 3)}}
+    ? 4: {'depth': 3, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {4: (5, 6, 3, 4)}}
+    -> 4: {'depth': 3, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {4: (5, 6, 3, 4)}}
+    -> 3: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {3: (5, 6, 3)}}
+    -> 6: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {6: (5, 6)}}
+    -> 5: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {5: (5,)}}
+    ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 3, 4, 5, 6}, 'paths':
+      {0: (0,)}}
+    ? 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 3, 4, 5, 6},
+      'paths': {1: (0, 1)}}
+    ? 2: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {2: (0, 1, 2)}}
+    -> 2: {'depth': 2, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {2: (0, 1, 2)}}
+    -> 1: {'depth': 1, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {1: (0, 1)}}
+    -> 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0, 1, 2, 3, 4, 5, 6},
+      'paths': {0: (0,)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All visited: [0, 1, 2, 3, 4, 5, 6]
 
     >>> search =  nog.BSearchBreadthFirst(next_edges=fb.next_edges_bi)
     >>> l, p = search.start_from(start_and_goal_vertices=((), fb.goal_vertices))
     Traceback (most recent call last):
     KeyError: 'No path to (a) goal vertex found'
@@ -2418,46 +2443,46 @@
     KeyError: 'No path to (a) goal vertex found'
     >>> l, p = search.start_from(start_and_goal_vertices=((), fb.goal_vertices),
     ...                          fail_silently=True)
     >>> print(l, type(p))
     -1 <class 'nographs._path.PathOfUnlabeledEdges'>
     >>> l, p = search.start_from(start_and_goal_vertices=(fb.start_vertices, ()),
     ...                          fail_silently=True)
-    ? 0: {'visited': {0, 5}, 'depth': 0}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {}}
     >>> print(l, type(p))
     -1 <class 'nographs._path.PathOfUnlabeledEdges'>
 
     >>> l, p = search.start_from(start_and_goal_vertices=fb.start_vertices_bi)
-    ? 0: {'visited': {0, 5}, 'depth': 0}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0}
-    ?<4: {'visited': {4}, 'depth': 0}
-    ? 1: {'visited': {0, 1, 5, 6}, 'depth': 1}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {}}
+    ?<4: {'depth': 0, 'visited': {4}, 'paths': {}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {}}
     >>> print(l, f.goal not in p)
     3 True
     >>> l, p = search.start_from(start_and_goal_vertices=fb.start_vertices_bi,
     ...                          build_path=True)
-    ? 0: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,)}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0, 'paths[5]': (5,)}
-    ?<4: {'visited': {4}, 'depth': 0, 'paths[4]': (4,)}
-    ? 1: {'visited': {0, 1, 5, 6}, 'depth': 1, 'paths[1]': (0, 1)}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,)}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
+    ?<4: {'depth': 0, 'visited': {4}, 'paths': {4: (4,)}}
+    ? 1: {'depth': 1, 'visited': {0, 1, 5, 6}, 'paths': {1: (0, 1)}}
     >>> print(l, list(p))
     3 [0, 1, 2, 4]
 
     Search in graph with reversed edges and with exchanged start and goal vertices.
     Since we exchange the adjacency functions instead of defining new ones with
     correct reporting, the edge directions reported below are to be interpreted in
     reversed directions.
     >>> l, p = nog.BSearchBreadthFirst(next_edges=tuple(reversed(fb.next_edges_bi))
     ...     ).start_from(start_and_goal_vertices=tuple(reversed(fb.start_vertices_bi)),
     ...                  build_path=True)
-    ?<4: {'visited': {4}, 'depth': 0, 'paths[4]': (4,)}
-    ? 0: {'visited': {0, 5}, 'depth': 0, 'paths[0]': (0,)}
-    ? 5: {'visited': {0, 1, 5}, 'depth': 0, 'paths[5]': (5,)}
-    ?<2: {'visited': {2, 3, 4}, 'depth': 1, 'paths[2]': (4, 2)}
+    ?<4: {'depth': 0, 'visited': {4}, 'paths': {4: (4,)}}
+    ? 0: {'depth': 0, 'visited': {0, 5}, 'paths': {0: (0,)}}
+    ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
+    ?<2: {'depth': 1, 'visited': {2, 3, 4}, 'paths': {2: (4, 2)}}
     >>> print(l, list(p))
     3 [4, 2, 1, 0]
     """
 
 
 class MultipleStartVerticesTraversalsWithLabels:
     """-- Traversal with multiple start vertex, last 3 traversal strategies --
@@ -2468,75 +2493,79 @@
     >>> fb = FMultiStartB()
 
     >>> traversal = nog.TraversalShortestPaths(
     ...     next_edges=f.next_edges)
     >>> traversal = traversal.start_from(
     ...     start_vertices=f.start_vertices, build_paths=True)
     >>> results_with_distances(traversal, f.start_vertices)
-    After start: {'distance': inf, 'depth': 0, 'paths[0]': (0,), 'paths[5]': (5,),
-      'distances[0]': 0, 'distances[5]': 0}
-    ? 5: {'distance': 0, 'depth': 0, 'paths[5]': (5,), 'distances[5]': 0}
-    ? 0: {'distance': 0, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    -> 1: {'distance': 1, 'depth': 1, 'paths[1]': (0, 1), 'distances[1]': 0}
-    ? 1: {'distance': 1, 'depth': 1, 'paths[1]': (0, 1), 'distances[1]': 0}
-    -> 6: {'distance': 1, 'depth': 1, 'paths[6]': (5, 6), 'distances[6]': 0}
-    ? 6: {'distance': 1, 'depth': 1, 'paths[6]': (5, 6), 'distances[6]': 0}
-    -> 3: {'distance': 2, 'depth': 2, 'paths[3]': (5, 6, 3), 'distances[3]': 0}
-    ? 3: {'distance': 2, 'depth': 2, 'paths[3]': (5, 6, 3), 'distances[3]': 0}
-    -> 2: {'distance': 2, 'depth': 2, 'paths[2]': (0, 1, 2), 'distances[2]': 0}
-    ? 2: {'distance': 2, 'depth': 2, 'paths[2]': (0, 1, 2), 'distances[2]': 0}
-    -> 4: {'distance': 3, 'depth': 3, 'paths[4]': (5, 6, 3, 4), 'distances[4]': 0}
-    ? 4: {'distance': 3, 'depth': 3, 'paths[4]': (5, 6, 3, 4), 'distances[4]': 0}
+    After start: {'distance': inf, 'depth': 0, 'distances': {0: 0, 5: 0}, 'paths':
+      {0: (0,), 5: (5,)}}
+    ? 5: {'distance': 0, 'depth': 0, 'distances': {5: 0}, 'paths': {5: (5,)}}
+    ? 0: {'distance': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 1: {'distance': 1, 'depth': 1, 'distances': {1: 0}, 'paths': {1: (0, 1)}}
+    ? 1: {'distance': 1, 'depth': 1, 'distances': {1: 0}, 'paths': {1: (0, 1)}}
+    -> 6: {'distance': 1, 'depth': 1, 'distances': {6: 0}, 'paths': {6: (5, 6)}}
+    ? 6: {'distance': 1, 'depth': 1, 'distances': {6: 0}, 'paths': {6: (5, 6)}}
+    -> 3: {'distance': 2, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (5, 6, 3)}}
+    ? 3: {'distance': 2, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (5, 6, 3)}}
+    -> 2: {'distance': 2, 'depth': 2, 'distances': {2: 0}, 'paths': {2: (0, 1, 2)}}
+    ? 2: {'distance': 2, 'depth': 2, 'distances': {2: 0}, 'paths': {2: (0, 1, 2)}}
+    -> 4: {'distance': 3, 'depth': 3, 'distances': {4: 0}, 'paths': {4: (5, 6, 3,
+      4)}}
+    ? 4: {'distance': 3, 'depth': 3, 'distances': {4: 0}, 'paths': {4: (5, 6, 3,
+      4)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All distances: {0: 0, 5: 0, 6: 0, 1: 0, 2: 0, 3: 0, 4: 0}
     >>> traversal = traversal.start_from(start_vertices=(), build_paths=True)
     >>> list(traversal)
     []
 
     >>> traversal = nog.TraversalMinimumSpanningTree(
     ...     next_edges=f.next_edges)
     >>> traversal = traversal.start_from(
     ...     start_vertices=f.start_vertices, build_paths=True)
     >>> results_standard(traversal, f.start_vertices)
-    After start: {'edge': None, 'paths[0]': (0,), 'paths[5]': (5,)}
-    ? 0: {'edge': None, 'paths[0]': (0,)}
-    ? 5: {'edge': None, 'paths[5]': (5,)}
-    -> 1: {'edge': (0, 1, 1), 'paths[1]': (0, 1)}
-    ? 1: {'edge': (0, 1, 1), 'paths[1]': (0, 1)}
-    -> 6: {'edge': (5, 6, 1), 'paths[6]': (5, 6)}
-    ? 6: {'edge': (5, 6, 1), 'paths[6]': (5, 6)}
-    -> 2: {'edge': (1, 2, 1), 'paths[2]': (0, 1, 2)}
-    ? 2: {'edge': (1, 2, 1), 'paths[2]': (0, 1, 2)}
-    -> 3: {'edge': (6, 3, 1), 'paths[3]': (5, 6, 3)}
-    ? 3: {'edge': (6, 3, 1), 'paths[3]': (5, 6, 3)}
-    -> 4: {'edge': (2, 4, 1), 'paths[4]': (0, 1, 2, 4)}
-    ? 4: {'edge': (2, 4, 1), 'paths[4]': (0, 1, 2, 4)}
+    After start: {'edge': None, 'paths': {0: (0,), 5: (5,)}}
+    ? 0: {'edge': None, 'paths': {0: (0,)}}
+    ? 5: {'edge': None, 'paths': {5: (5,)}}
+    -> 1: {'edge': (0, 1, 1), 'paths': {1: (0, 1)}}
+    ? 1: {'edge': (0, 1, 1), 'paths': {1: (0, 1)}}
+    -> 6: {'edge': (5, 6, 1), 'paths': {6: (5, 6)}}
+    ? 6: {'edge': (5, 6, 1), 'paths': {6: (5, 6)}}
+    -> 2: {'edge': (1, 2, 1), 'paths': {2: (0, 1, 2)}}
+    ? 2: {'edge': (1, 2, 1), 'paths': {2: (0, 1, 2)}}
+    -> 3: {'edge': (6, 3, 1), 'paths': {3: (5, 6, 3)}}
+    ? 3: {'edge': (6, 3, 1), 'paths': {3: (5, 6, 3)}}
+    -> 4: {'edge': (2, 4, 1), 'paths': {4: (0, 1, 2, 4)}}
+    ? 4: {'edge': (2, 4, 1), 'paths': {4: (0, 1, 2, 4)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (0, 1, 2, 4), (5,), (5, 6)]
     >>> traversal = traversal.start_from(start_vertices=(), build_paths=True)
     >>> list(traversal)
     []
 
 
     >>> fa = FMultiStartAStar()
     >>> traversal = nog.TraversalAStar(next_edges=fa.next_edges)
     >>> traversal = traversal.start_from(
     ...     fa.heuristic, start_vertices=fa.start_vertices, build_paths=True)
     >>> results_standard(traversal, fa.start_vertices)
-    After start: {'path_length': inf, 'depth': 0, 'paths[0]': (0,), 'paths[1]':
-      (1,), 'distances[0]': 0, 'distances[1]': 0}
-    ? 1: {'path_length': 0, 'depth': 0, 'paths[1]': (1,), 'distances[1]': 0}
-    -> 3: {'path_length': 1, 'depth': 1, 'paths[3]': (1, 3), 'distances[3]': 1}
-    ? 3: {'path_length': 1, 'depth': 1, 'paths[3]': (1, 3), 'distances[3]': 1}
-    -> 5: {'path_length': 2, 'depth': 2, 'paths[5]': (1, 3, 5), 'distances[5]': 2}
-    ? 5: {'path_length': 2, 'depth': 2, 'paths[5]': (1, 3, 5), 'distances[5]': 2}
-    ? 0: {'path_length': 0, 'depth': 0, 'paths[0]': (0,), 'distances[0]': 0}
-    -> 2: {'path_length': 1, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 1}
-    ? 2: {'path_length': 1, 'depth': 1, 'paths[2]': (0, 2), 'distances[2]': 1}
-    -> 4: {'path_length': 1, 'depth': 1, 'paths[4]': (1, 4), 'distances[4]': 1}
-    ? 4: {'path_length': 1, 'depth': 1, 'paths[4]': (1, 4), 'distances[4]': 1}
+    After start: {'path_length': inf, 'depth': 0, 'distances': {0: 0, 1: 0},
+      'paths': {0: (0,), 1: (1,)}}
+    ? 1: {'path_length': 0, 'depth': 0, 'distances': {1: 0}, 'paths': {1: (1,)}}
+    -> 3: {'path_length': 1, 'depth': 1, 'distances': {3: 1}, 'paths': {3: (1, 3)}}
+    ? 3: {'path_length': 1, 'depth': 1, 'distances': {3: 1}, 'paths': {3: (1, 3)}}
+    -> 5: {'path_length': 2, 'depth': 2, 'distances': {5: 2}, 'paths': {5: (1, 3,
+      5)}}
+    ? 5: {'path_length': 2, 'depth': 2, 'distances': {5: 2}, 'paths': {5: (1, 3,
+      5)}}
+    ? 0: {'path_length': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 2: {'path_length': 1, 'depth': 1, 'distances': {2: 1}, 'paths': {2: (0, 2)}}
+    ? 2: {'path_length': 1, 'depth': 1, 'distances': {2: 1}, 'paths': {2: (0, 2)}}
+    -> 4: {'path_length': 1, 'depth': 1, 'distances': {4: 1}, 'paths': {4: (1, 4)}}
+    ? 4: {'path_length': 1, 'depth': 1, 'distances': {4: 1}, 'paths': {4: (1, 4)}}
     All paths: [(0,), (1,), (0, 2), (1, 3), (1, 4), (1, 3, 5)]
     >>> traversal = traversal.start_from(
     ...     fa.heuristic, start_vertices=(), build_paths=True)
     >>> list(traversal)
     []
 
     >>> search = nog.BSearchShortestPath(fb.next_edges_bi)
```

### Comparing `nographs-3.1.0/tests/test_types.py` & `nographs-3.2.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `nographs-3.1.0/tests/test_unit_typed.py` & `nographs-3.2.0/tests/test_unit_typed.py`

 * *Files identical despite different names*

