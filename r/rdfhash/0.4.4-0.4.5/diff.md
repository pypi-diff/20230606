# Comparing `tmp/rdfhash-0.4.4.tar.gz` & `tmp/rdfhash-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfhash-0.4.4.tar", last modified: Tue Jun  6 15:00:46 2023, max compression
+gzip compressed data, was "rdfhash-0.4.5.tar", last modified: Tue Jun  6 16:52:37 2023, max compression
```

## Comparing `rdfhash-0.4.4.tar` & `rdfhash-0.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 15:00:46.176340 rdfhash-0.4.4/
--rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 15:00:46.175563 rdfhash-0.4.4/PKG-INFO
--rw-r--r--   0 grahamneil   (501) staff       (20)     5080 2022-12-16 20:21:13.000000 rdfhash-0.4.4/README.md
--rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.4/pyproject.toml
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 15:00:46.173179 rdfhash-0.4.4/rdfhash/
--rw-r--r--   0 grahamneil   (501) staff       (20)      147 2023-06-06 14:58:14.000000 rdfhash-0.4.4/rdfhash/__init__.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     4136 2023-06-06 14:58:10.000000 rdfhash-0.4.4/rdfhash/cli.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2022-12-16 20:21:13.000000 rdfhash-0.4.4/rdfhash/logger.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     9904 2023-06-06 14:58:02.000000 rdfhash-0.4.4/rdfhash/main.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 15:00:46.174965 rdfhash-0.4.4/rdfhash/utils/
--rw-r--r--   0 grahamneil   (501) staff       (20)      592 2023-06-06 08:26:03.000000 rdfhash-0.4.4/rdfhash/utils/__init__.py
--rw-r--r--   0 grahamneil   (501) staff       (20)    10205 2023-06-06 14:58:29.000000 rdfhash-0.4.4/rdfhash/utils/graph.py
--rw-r--r--   0 grahamneil   (501) staff       (20)     2944 2023-06-06 08:26:03.000000 rdfhash-0.4.4/rdfhash/utils/hash.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 15:00:46.174342 rdfhash-0.4.4/rdfhash.egg-info/
--rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 15:00:46.000000 rdfhash-0.4.4/rdfhash.egg-info/PKG-INFO
--rw-r--r--   0 grahamneil   (501) staff       (20)      383 2023-06-06 15:00:46.000000 rdfhash-0.4.4/rdfhash.egg-info/SOURCES.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-06 15:00:46.000000 rdfhash-0.4.4/rdfhash.egg-info/dependency_links.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-06 15:00:46.000000 rdfhash-0.4.4/rdfhash.egg-info/entry_points.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       63 2023-06-06 15:00:46.000000 rdfhash-0.4.4/rdfhash.egg-info/requires.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-06 15:00:46.000000 rdfhash-0.4.4/rdfhash.egg-info/top_level.txt
--rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-06 15:00:46.176378 rdfhash-0.4.4/setup.cfg
--rw-r--r--   0 grahamneil   (501) staff       (20)     1006 2023-06-06 14:59:25.000000 rdfhash-0.4.4/setup.py
-drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 15:00:46.175239 rdfhash-0.4.4/test/
--rw-r--r--   0 grahamneil   (501) staff       (20)     3869 2023-06-06 08:26:03.000000 rdfhash-0.4.4/test/test_examples.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.990050 rdfhash-0.4.5/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 16:52:37.989918 rdfhash-0.4.5/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5080 2022-12-16 20:21:13.000000 rdfhash-0.4.5/README.md
+-rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.5/pyproject.toml
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.988065 rdfhash-0.4.5/rdfhash/
+-rw-r--r--   0 grahamneil   (501) staff       (20)      147 2023-06-06 14:58:14.000000 rdfhash-0.4.5/rdfhash/__init__.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     4136 2023-06-06 14:58:10.000000 rdfhash-0.4.5/rdfhash/cli.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2022-12-16 20:21:13.000000 rdfhash-0.4.5/rdfhash/logger.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     9839 2023-06-06 16:30:35.000000 rdfhash-0.4.5/rdfhash/main.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.989433 rdfhash-0.4.5/rdfhash/utils/
+-rw-r--r--   0 grahamneil   (501) staff       (20)      592 2023-06-06 08:26:03.000000 rdfhash-0.4.5/rdfhash/utils/__init__.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)    10765 2023-06-06 16:50:17.000000 rdfhash-0.4.5/rdfhash/utils/graph.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     2944 2023-06-06 08:26:03.000000 rdfhash-0.4.5/rdfhash/utils/hash.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.988866 rdfhash-0.4.5/rdfhash.egg-info/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)      383 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/SOURCES.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/dependency_links.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/entry_points.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       63 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/requires.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-06 16:52:37.000000 rdfhash-0.4.5/rdfhash.egg-info/top_level.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-06 16:52:37.990085 rdfhash-0.4.5/setup.cfg
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1006 2023-06-06 16:51:53.000000 rdfhash-0.4.5/setup.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 16:52:37.989646 rdfhash-0.4.5/test/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     3924 2023-06-06 16:44:42.000000 rdfhash-0.4.5/test/test_examples.py
```

### Comparing `rdfhash-0.4.4/PKG-INFO` & `rdfhash-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfhash
-Version: 0.4.4
+Version: 0.4.5
 Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}. ' pairs sorted.
 Home-page: https://github.com/NeilGraham/rdfhash
 Author: Neil Graham
 Author-email: grahamneiln@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `rdfhash-0.4.4/README.md` & `rdfhash-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.4/rdfhash/cli.py` & `rdfhash-0.4.5/rdfhash/cli.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.4/rdfhash/logger.py` & `rdfhash-0.4.5/rdfhash/logger.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.4/rdfhash/main.py` & `rdfhash-0.4.5/rdfhash/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,26 +202,25 @@
                 triple_new.append(term)
 
         # Append predicate and object to list to be added later with hashed subject.
         triples_add.append(triple_new)
 
         # Append `{predicate} {object}.\n` to list of values to hash.
         hash_input_list.append(
-            f"{graph.term_to_string(triple_new[0], expand_xsd_string=True)} {graph.term_to_string(triple_new[1], expand_xsd_string=True)}.\n"
+            f"{graph.term_to_string(triple_new[0], True)} {graph.term_to_string(triple_new[1], True)}.\n"
         )
 
     # Sort and concatenate list, hash value, then add to graph.
     # ---------------------------------------------------------
 
     # Sort list of strings: `{predicate} {object}.\n`
     hash_input_list.sort()
 
     # Join list of strings to be hashed.
     hash_input = "".join(hash_input_list)
-    print(f"'{hash_input}'")
 
     logger.debug(f'({len(hash_input_list)}) Hashing triple set: """{hash_input}"""')
 
     # Concatenate sorted list, hash with method, then add to a URIRef.
     hash_dict = {"method": method, "value": hash_string(hash_input, method, length)}
     hash_subj = graph.NamedNode(template.format(**hash_dict))
```

### Comparing `rdfhash-0.4.4/rdfhash/utils/__init__.py` & `rdfhash-0.4.5/rdfhash/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.4/rdfhash/utils/graph.py` & `rdfhash-0.4.5/rdfhash/utils/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,22 @@
     graph_class = rdflib.ConjunctiveGraph
 
     NamedNode = rdflib.URIRef
     BlankNode = rdflib.BNode
     Literal = rdflib.Literal
     Variable = rdflib.Variable
 
+    xsd_langstring = rdflib.URIRef(
+        "http://www.w3.org/1999/02/22-rdf-syntax-ns#langString"
+    )
+
+    xsd_string = rdflib.URIRef("http://www.w3.org/2001/XMLSchema#string")
+    
+    xsd_boolean = rdflib.URIRef("http://www.w3.org/2001/XMLSchema#boolean")
+
     default_format = mime["trig"]
 
     supports_named_graphs = True
 
     def __init__(self, data=None, format=None, max_path=2048):
         """Initialize graph object
 
@@ -169,19 +177,26 @@
                 self.is_uri(term),
                 self.is_literal(term),
                 self.is_bnode(term),
                 self.is_variable(term) if allow_variable else False,
             ]
         )
 
-    def term_to_string(self, term, expand_xsd_string=False):
-        if expand_xsd_string and type(term) == self.Literal and term.datatype == None:
+    def term_to_string(self, term, expand_literals=False):
+        if expand_literals and type(term) == self.Literal:
+            value, datatype, language = term.value, term.datatype, term.language
+            if datatype == None:
+                if language:
+                    datatype = self.xsd_langstring
+                else:
+                    datatype = self.xsd_string
             if term.language:
-                return f'"{term.value}"^^<http://www.w3.org/2001/XMLSchema#string>@{term.language}'
-            return f'"{term.value}"^^<http://www.w3.org/2001/XMLSchema#string>'
+                return f'"{value}"^^{datatype.n3()}@{language}'
+
+            return f'"{value}"^^{datatype.n3()}'
         return term.n3()
 
     def hash_triples(self, triples, method="sha256", triple_format="{p} {o}\n"):
         sorted_triples = sorted(
             triple_format.format(s=s, p=p, o=o) for s, p, o in triples
         )
         joined_triples = "".join(sorted_triples)
@@ -264,14 +279,15 @@
     NamedNode = pyoxigraph.NamedNode
     Literal = pyoxigraph.Literal
     Variable = pyoxigraph.Variable
 
     Quad = pyoxigraph.Quad
 
     xsd_string = pyoxigraph.NamedNode("http://www.w3.org/2001/XMLSchema#string")
+    xsd_boolean = pyoxigraph.NamedNode("http://www.w3.org/2001/XMLSchema#boolean")
 
     supports_named_graphs = True
 
     def __contains__(self, item):
         iter = self.quads(item)
         try:
             next(iter)
@@ -310,23 +326,22 @@
 
     def quads(self, quad):
         return self.graph.quads_for_pattern(*quad)
 
     def triples(self, triple):
         return self.quads(triple)
 
-    def term_to_string(self, term, expand_xsd_string=False):
-        if (
-            expand_xsd_string
-            and type(term) == self.Literal
-            and term.datatype == self.xsd_string
-        ):
-            if term.language != None:
-                return f'"{term.value}"^^{term.datatype}@{term.language}'
-            return f'"{term.value}"^^{term.datatype}'
+    def term_to_string(self, term, expand_literals=False):
+        if expand_literals and type(term) == self.Literal:
+            value, datatype, language = term.value, term.datatype, term.language
+            if datatype == self.xsd_boolean:
+                value = str(value.capitalize())
+            if language:
+                return f'"{value}"^^{datatype}@{language}'
+            return f'"{value}"^^{datatype}'
         return str(term)
 
     def add(self, quad):
         return self.graph.add(self.Quad(*quad))
 
     def remove(self, quad):
         return self.graph.remove(self.Quad(*quad))
```

### Comparing `rdfhash-0.4.4/rdfhash/utils/hash.py` & `rdfhash-0.4.5/rdfhash/utils/hash.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.4.4/rdfhash.egg-info/PKG-INFO` & `rdfhash-0.4.5/rdfhash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfhash
-Version: 0.4.4
+Version: 0.4.5
 Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}. ' pairs sorted.
 Home-page: https://github.com/NeilGraham/rdfhash
 Author: Neil Graham
 Author-email: grahamneiln@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `rdfhash-0.4.4/setup.py` & `rdfhash-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path, getcwd
 
 setup(
     name="rdfhash",
-    version="0.4.4",
+    version="0.4.5",
     author="Neil Graham",
     author_email="grahamneiln@gmail.com",
     url="https://github.com/NeilGraham/rdfhash",
     license_files="LICENSE.txt",
     description="De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}.\n' pairs sorted.",
     long_description=open(path.join(getcwd(), "README.md")).read()
     # Replace local links to 'docs/' to Github page 'docs/'.
```

### Comparing `rdfhash-0.4.4/test/test_examples.py` & `rdfhash-0.4.5/test/test_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from pathlib import Path
 from glob import glob
 
 from rdflib import Graph
 import pytest
 import oxrdflib
 
-from package import rdfhash, reverse_hash_subjects
-from package.logger import logger
-from package.utils.hash import (
+from rdfhash import rdfhash, reverse_hash_subjects
+from rdfhash.logger import logger
+from rdfhash.utils.hash import (
     hash_types,
     hash_types_requiring_length,
     hash_types_resolvable,
 )
-from package.utils.graph import graph_types
+from rdfhash.utils.graph import graph_types
 from utils import compare_graphs, graph_differences
 
 repo_dir = path.dirname(Path(__file__).parent.absolute())
 ttl_files = (
     path.relpath(file) for file in glob(path.join(repo_dir, "examples", "*.ttl"))
 )
 
@@ -27,14 +27,15 @@
         resolvable_hash_methods[i] = resolvable_hash_methods[i] + ":64"
 
 
 @pytest.mark.parametrize("file_path", ttl_files)
 # @pytest.mark.parametrize("hash_method", resolvable_hash_methods)
 @pytest.mark.parametrize("hash_method", ["sha256"])
 @pytest.mark.parametrize("graph_type", list(graph_types.keys()))
+# @pytest.mark.parametrize("graph_type", ["oxrdflib"])
 def test__hash_examples(file_path, hash_method, graph_type, force_write=False):
     """Hash file and compare against hash file.
 
     Args:
         graph_type (str): Graph type to use.
         force_write (bool, optional): If True, forces writing hash
             result to file './examples/hashed'. Defaults to True.
```

