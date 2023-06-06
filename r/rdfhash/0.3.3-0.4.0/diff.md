# Comparing `tmp/rdfhash-0.3.3.tar.gz` & `tmp/rdfhash-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfhash-0.3.3.tar", last modified: Wed Dec 14 06:42:16 2022, max compression
+gzip compressed data, was "rdfhash-0.4.0.tar", last modified: Tue Jun  6 08:30:57 2023, max compression
```

## Comparing `rdfhash-0.3.3.tar` & `rdfhash-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-12-14 06:42:16.087814 rdfhash-0.3.3/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     5582 2022-12-14 06:42:16.087814 rdfhash-0.3.3/PKG-INFO
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     5080 2022-12-08 20:57:24.000000 rdfhash-0.3.3/README.md
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-12-14 06:42:16.087814 rdfhash-0.3.3/package/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      154 2022-12-14 05:41:39.000000 rdfhash-0.3.3/package/__init__.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     4041 2022-12-14 06:28:55.000000 rdfhash-0.3.3/package/cli.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     9206 2022-12-14 04:41:19.000000 rdfhash-0.3.3/package/hash.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     2766 2022-12-14 04:27:47.000000 rdfhash-0.3.3/package/helper.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     1026 2022-12-08 20:57:24.000000 rdfhash-0.3.3/package/logger.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      273 2022-12-08 20:57:24.000000 rdfhash-0.3.3/pyproject.toml
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-12-14 06:42:16.087814 rdfhash-0.3.3/rdfhash.egg-info/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     5582 2022-12-14 06:42:16.000000 rdfhash-0.3.3/rdfhash.egg-info/PKG-INFO
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      330 2022-12-14 06:42:16.000000 rdfhash-0.3.3/rdfhash.egg-info/SOURCES.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)        1 2022-12-14 06:42:16.000000 rdfhash-0.3.3/rdfhash.egg-info/dependency_links.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       45 2022-12-14 06:42:16.000000 rdfhash-0.3.3/rdfhash.egg-info/entry_points.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       28 2022-12-14 06:42:16.000000 rdfhash-0.3.3/rdfhash.egg-info/requires.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)        8 2022-12-14 06:42:16.000000 rdfhash-0.3.3/rdfhash.egg-info/top_level.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       38 2022-12-14 06:42:16.087814 rdfhash-0.3.3/setup.cfg
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      981 2022-12-14 06:42:03.000000 rdfhash-0.3.3/setup.py
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-12-14 06:42:16.087814 rdfhash-0.3.3/test/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     4072 2022-12-08 20:57:24.000000 rdfhash-0.3.3/test/test_examples.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.568454 rdfhash-0.4.0/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 08:30:57.568303 rdfhash-0.4.0/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5080 2022-12-16 20:21:13.000000 rdfhash-0.4.0/README.md
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.567270 rdfhash-0.4.0/package/
+-rw-r--r--   0 grahamneil   (501) staff       (20)      140 2023-06-06 08:26:03.000000 rdfhash-0.4.0/package/__init__.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     4108 2023-06-06 08:26:03.000000 rdfhash-0.4.0/package/cli.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1026 2022-12-16 20:21:13.000000 rdfhash-0.4.0/package/logger.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)     9876 2023-06-06 08:26:03.000000 rdfhash-0.4.0/package/main.py
+-rw-r--r--   0 grahamneil   (501) staff       (20)      273 2022-12-16 20:21:13.000000 rdfhash-0.4.0/pyproject.toml
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.567912 rdfhash-0.4.0/rdfhash.egg-info/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     5598 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/PKG-INFO
+-rw-r--r--   0 grahamneil   (501) staff       (20)      312 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/SOURCES.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        1 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/dependency_links.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       45 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/entry_points.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       62 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/requires.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)        8 2023-06-06 08:30:57.000000 rdfhash-0.4.0/rdfhash.egg-info/top_level.txt
+-rw-r--r--   0 grahamneil   (501) staff       (20)       38 2023-06-06 08:30:57.568503 rdfhash-0.4.0/setup.cfg
+-rw-r--r--   0 grahamneil   (501) staff       (20)     1041 2023-06-06 08:26:03.000000 rdfhash-0.4.0/setup.py
+drwxr-xr-x   0 grahamneil   (501) staff       (20)        0 2023-06-06 08:30:57.568064 rdfhash-0.4.0/test/
+-rw-r--r--   0 grahamneil   (501) staff       (20)     3869 2023-06-06 08:26:03.000000 rdfhash-0.4.0/test/test_examples.py
```

### Comparing `rdfhash-0.3.3/PKG-INFO` & `rdfhash-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rdfhash
-Version: 0.3.3
-Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}.
+Version: 0.4.0
+Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}. ' pairs sorted.
 Home-page: https://github.com/NeilGraham/rdfhash
 Author: Neil Graham
 Author-email: grahamneiln@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `rdfhash-0.3.3/README.md` & `rdfhash-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rdfhash-0.3.3/package/hash.py` & `rdfhash-0.4.0/package/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from string import Template
-
-from rdflib.term import URIRef, BNode
-
-from .helper import hash_string, convert_data_to_graph, rdf_term_to_id, hashlib_methods
+from .utils.hash import hash_string, hashlib_methods
+from .utils.graph import get_graph
+from .utils import validate_uri
 from .logger import logger
 
 
 def hash_subjects(
     data,
-    format = None,
-    method = "sha256",
-    template = "${method}:${value}",
-    sparql_select_subjects=(
-        "SELECT DISTINCT ?s { ?s ?p ?o . FILTER (isBlank(?s)) }"
-    ),
+    format=None,
+    method="sha256",
+    template="{method}:{value}",
+    sparql_select_subjects=("SELECT DISTINCT ?s { ?s ?p ?o . FILTER (isBlank(?s)) }"),
+    graph_type="oxrdflib",
+    length=None,
 ):
     """Hash subjects by the sum of their triples.
 
     Subject hash result is calculated by sorting each triple by
     `{subject} {predicate}.` then joining with `\n`.
 
     Example:
@@ -35,115 +33,145 @@
         data (str|rdflib.Graph): Data representing RDF triples.
         format (str, optional): Format of data. Defaults to None.
         method (str, optional): Hashing method to use. Defaults to "sha256".
         template (str, optional): Template string for hash URI.
             Defaults to "{method}:{value}".
         sparql_select_subject (str, optional): SPARQL SELECT query to return
             list of subjects which will have their triples hashed.
+        graph_type (str, optional): Graph type to use. Defaults to "oxrdflib".
+        length (int, optional): Length of hash result. Required for some hash methods,
+            optional for all.
 
     Returns:
         rdflib.Graph: Updated 'data' graph.
     """
-    # Convert template string to 'Template' class.
-    if type(template) != Template:
-        template = Template(template)
 
     # Convert data provided to rdflib.Graph.
-    graph = convert_data_to_graph(data, format)
+    graph = get_graph(data, format, graph_type)
     len_before = len(graph)
 
     # Use SPARQL query 'sparql_select_subject' to get list of subjects to hash.
-    select_subjects = set([r[0] for r in graph.query(sparql_select_subjects)])
+    select_subjects = set()
+    for row in graph.query(sparql_select_subjects):
+        for item in row:
+            select_subjects.add(item)
 
     logger.info(
         f"\n({len(select_subjects)}) Hashing subject triples:\n-- "
-        + "\n-- ".join([s.n3() for s in select_subjects])
+        + "\n-- ".join([graph.term_to_string(s) for s in select_subjects])
     )
 
     hashed_values = {}  # Dictionary of subjects and resolved hash values.
 
+    spec_length = None
+    if ":" in method:
+        method, spec_length = method.split(":")
+        spec_length = int(spec_length)
+
     for s in select_subjects:
+        if s in hashed_values:
+            continue
+
         # Continue if subject is already replaced or N/A.
         if (s, None, None) not in graph:
-            logger.debug("Subject was already replaced or is N/A: " + s.n3())
+            logger.warning(
+                "Selected subject not found in graph: " + graph.term_to_string(s)
+            )
             continue
 
-        hashed_values.update(hash_subject(graph, s, method, template, select_subjects))
+        hashed_values.update(
+            hash_subject(
+                graph,
+                s,
+                method,
+                template,
+                select_subjects,
+                length=length or spec_length,
+            )
+        )
 
     logger.info(
         f"\n({len(hashed_values)}) Hashed subjects:\n-- "
-        + "\n-- ".join(f"{k.n3()} -> {v.n3()}" for k, v in hashed_values.items())
+        + "\n-- ".join(
+            f"{graph.term_to_string(k)} -> {graph.term_to_string(v)}"
+            for k, v in hashed_values.items()
+        )
     )
 
     len_after = len(graph)
     if len_before == len_after:
         logger.info(f"(=) Graph size did not change: {len_before}")
     else:
         logger.info(
             f"(-{len_before-len_after}) Graph size reduced from {len_before} to {len_after}."
         )
 
-    return graph
+    return graph, hashed_values
 
 
 def hash_subject(
     graph,
     subject,
     method="sha256",
-    template = "${method}:${value}",
-    also_subjects = None,
-    circ_deps = None,
+    template="{method}:{value}",
+    also_subjects=None,
+    circ_deps=None,
+    length=None,
 ):
     """Replaces subject in graph with hash of it's triples.
 
     If encounters a blank node in the object position, recursively hashes it.
-    
+
     Updates 'graph' rdflib.Graph but does not return anything.
 
     Args:
         graph (rdflib.Graph): rdflib.Graph.
         subject (_type_): rdflib.term representing a subject.
         method (str, optional): Hashing method to use. Defaults to "sha256".
         template (str, optional): Template string for hash URI.
             Defaults to "{method}:{value}".
         also_subjects (set, optional) If encounters any of these terms in triples,
-            recursively resolves them. Throws error if circular dependency found. 
+            recursively resolves them. Throws error if circular dependency found.
             Defaults to None.
         circ_deps (set, optional): Set of values which 'subject' cannot be.
             Defaults to None.
+        length (int, optional): Length of hash result. Required for some hash methods,
+            optional for all.
 
     Raises:
         ValueError: If blank node in predicate position of any triples.
         ValueError: If subject does not have triples associated with it.
         ValueError: If circular dependency is detected. Unable to resolve
             current hash.
     """
     hashed_values = {}  # Return dictionary.
 
-    if type(template) != Template:
-        template = Template(template)
+    # if type(template) != Template:
+    #     template = Template(template)
 
     if also_subjects == None:
         also_subjects = set()
 
     if circ_deps == None:
         circ_deps = set()
 
     # Add current subject to circular dependencies.
     circ_deps.add(subject)
 
-    hash_value_list = []  # List of values to hash. (`${predicate} ${object}.`)
+    hash_input_list = []  # List of values to hash. (`${predicate} ${object}.`)
     triples_add = []  # List of triples to replace with hashed subject.
 
     # Get all triples containing subject.
     triples = [*graph.triples((subject, None, None))]
 
     # Return if no triples found on subject specified.
     if len(triples) == 0:
-        logger.warning("Could not find any triples for subject: " + subject.n3())
+        logger.warning(
+            "Could not find any triples for subject: " + graph.term_to_string(subject)
+        )
         return hashed_values
 
     # Generate list of `${predicate} ${object}.` for each triple on subject.
     # ----------------------------------------------------------------------
 
     for triple in triples:
         graph.remove(triple)  # Remove triple from graph.
@@ -154,53 +182,54 @@
         for i in range(1, 3):
             term = triple[i]
             if term in also_subjects:
                 # If object in circular dependencies, throw error.
                 if term in circ_deps:
                     raise ValueError(
                         "Unable to resolve hash. Circular dependency "
-                        f"detected: {subject.n3()} <--> {term.n3()}"
+                        f"detected: {graph.term_to_string(subject)} <--> {graph.term_to_string(term)}"
                     )
 
                 # Recursive Call.
                 # ---------------
                 # Resolve hash value of nested triples first.
                 hashed_values.update(
                     hash_subject(
-                        graph, term, method, template, also_subjects, circ_deps
+                        graph, term, method, template, also_subjects, circ_deps, length
                     )
                 )
                 triple_new.append(hashed_values[term])
             else:
                 triple_new.append(term)
 
         # Append predicate and object to list to be added later with hashed subject.
         triples_add.append(triple_new)
 
         # Append `{predicate} {object}.\n` to list of values to hash.
-        hash_value_list.append(
-            f"{rdf_term_to_id(triple_new[0])} {rdf_term_to_id(triple_new[1])}.\n"
+        hash_input_list.append(
+            f"{graph.term_to_string(triple_new[0], expand_xsd_string=True)} {graph.term_to_string(triple_new[1], expand_xsd_string=True)}.\n"
         )
 
     # Sort and concatenate list, hash value, then add to graph.
     # ---------------------------------------------------------
 
     # Sort list of strings: `{predicate} {object}.\n`
-    hash_value_list.sort()
+    hash_input_list.sort()
 
     # Join list of strings to be hashed.
-    hash_value = "".join(hash_value_list)
+    hash_input = "".join(hash_input_list)
+    print(f"'{hash_input}'")
 
-    logger.debug(f'({len(hash_value_list)}) Hashing triple set: """{hash_value}"""')
+    logger.debug(f'({len(hash_input_list)}) Hashing triple set: """{hash_input}"""')
 
     # Concatenate sorted list, hash with method, then add to a URIRef.
-    hash_dict = {"method": method, "value": hash_string(hash_value, method)}
-    hash_subj = URIRef(template.substitute(**hash_dict))
+    hash_dict = {"method": method, "value": hash_string(hash_input, method, length)}
+    hash_subj = graph.NamedNode(template.format(**hash_dict))
 
-    logger.debug(f"Result of hashed triples: {hash_subj.n3()}")
+    logger.debug(f"Result of hashed triples: {graph.term_to_string(hash_subj)}")
 
     # Add triples to graph with hashed subject.
     for pred_obj in triples_add:
         graph.add((hash_subj, *pred_obj))
 
     # Replace instances of current subject in the object position.
     for triple in graph.triples((None, None, subject)):
@@ -208,51 +237,46 @@
         graph.add((triple[0], triple[1], hash_subj))
 
     # Add hashed subject to 'hashed_values' and return.
     hashed_values[subject] = hash_subj
     return hashed_values
 
 
-def reverse_hash_subjects(data, format = None):
+def reverse_hash_subjects(
+    data, format=None, template="{method}:{value}", graph_type="oxrdflib"
+):
     """Convert hashed URIs to blank nodes.
 
     Args:
         data (_type_): Data representing RDF triples.
         format (str, optional): Format of data. Defaults to None.
 
     Returns:
         rdflib.Graph: Updated 'data' graph.
     """
     bnode_int = 0
     bnode_dict = {}
 
-    # Convert data provided to rdflib.Graph.
-    graph = convert_data_to_graph(data, format)
+    graph = get_graph(data, format, graph_type)
 
     # Check every term in graph.
-    for triple in graph:
+    for triple in graph.triples():
         new_triple = []  # Replaces 'triple'.
         updated = False  # Tracks whether 'new_triple' is different to 'triple'.
 
         for term in triple:
-            # Skip update if starts with 'http' (most common case).
-            # No hash method is expected to start with this string.
-            if term.startswith("http"):
-                new_triple.append(term)
-            # If URI is already replaced, use replacement.
-            elif term in bnode_dict:
+            if term in bnode_dict:
                 updated = True
                 new_triple.append(bnode_dict[term])
-            # Check to see if term starts with any of the possible hash methods.
-            elif any(
-                term.startswith(hash_string + ":")
-                for hash_string in hashlib_methods.keys()
+            # If term matches 'template' regex, replace with blank node.
+            elif graph.is_uri(term) and validate_uri(
+                graph.term_to_string(term)[1:-1], template
             ):
                 updated = True
-                bnode = BNode(bnode_int)
+                bnode = graph.BlankNode(bnode_int)
                 bnode_int += 1
                 bnode_dict[term] = bnode
                 new_triple.append(bnode)
             # If does not start with hash method, do not update.
             else:
                 new_triple.append(term)
```

### Comparing `rdfhash-0.3.3/package/logger.py` & `rdfhash-0.4.0/package/logger.py`

 * *Files identical despite different names*

### Comparing `rdfhash-0.3.3/rdfhash.egg-info/PKG-INFO` & `rdfhash-0.4.0/rdfhash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rdfhash
-Version: 0.3.3
-Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}.
+Version: 0.4.0
+Summary: De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}. ' pairs sorted.
 Home-page: https://github.com/NeilGraham/rdfhash
 Author: Neil Graham
 Author-email: grahamneiln@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `rdfhash-0.3.3/setup.py` & `rdfhash-0.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path, getcwd
 
 setup(
     name="rdfhash",
-    version="0.3.3",
+    version="0.4.0",
     author="Neil Graham",
     author_email="grahamneiln@gmail.com",
     url="https://github.com/NeilGraham/rdfhash",
     license_files="LICENSE.txt",
     description="De-duplicate RDF triples w/ a SPARQL query. Subjects taken from SELECT are replaced by the hash of their triples '{predicate} {object}.\n' pairs sorted.",
     long_description=open(path.join(getcwd(), "README.md")).read()
     # Replace local links to 'docs/' to Github page 'docs/'.
@@ -19,9 +19,11 @@
     packages=["rdfhash"],
     package_dir={"rdfhash": "package"},
     entry_points={"console_scripts": ["rdfhash = rdfhash.cli:cli"]},
     python_requires=">=3.6",
     install_requires=[
         "pytest >= 7.1.2",
         "rdflib >= 6.1.1",
+        "oxrdflib >= 0.3.4",
+        "pyoxigraph >= 0.8.0",
     ],
 )
```

