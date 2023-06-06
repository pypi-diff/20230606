# Comparing `tmp/grape-0.1.9.tar.gz` & `tmp/grape-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grape-0.1.9.tar", last modified: Tue Jul  5 20:32:57 2022, max compression
+gzip compressed data, was "grape-0.2.0.tar", last modified: Tue Jun  6 08:45:20 2023, max compression
```

## Comparing `grape-0.1.9.tar` & `grape-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-07-05 20:32:57.000000 grape-0.1.9/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    15181 2022-07-05 20:32:57.000000 grape-0.1.9/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    12404 2022-06-15 19:23:22.000000 grape-0.1.9/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-07-05 20:32:57.000000 grape-0.1.9/grape/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1197 2022-06-14 09:43:15.000000 grape-0.1.9/grape/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       62 2022-07-05 20:30:11.000000 grape-0.1.9/grape/__version__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-07-05 20:32:57.000000 grape-0.1.9/grape.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    15181 2022-07-05 20:32:57.000000 grape-0.1.9/grape.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      202 2022-07-05 20:32:57.000000 grape-0.1.9/grape.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2022-07-05 20:32:57.000000 grape-0.1.9/grape.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       35 2022-07-05 20:32:57.000000 grape-0.1.9/grape.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        6 2022-07-05 20:32:57.000000 grape-0.1.9/grape.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2022-07-05 20:32:57.000000 grape-0.1.9/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1845 2022-07-05 20:30:19.000000 grape-0.1.9/setup.py
+drwxr-xr-x   0 luca      (1001) luca      (1003)        0 2023-06-06 08:45:20.095202 grape-0.2.0/
+-rw-r--r--   0 luca      (1001) luca      (1003)     1090 2023-05-14 14:45:38.000000 grape-0.2.0/LICENSE
+-rw-r--r--   0 luca      (1001) luca      (1003)    12754 2023-06-06 08:45:20.095202 grape-0.2.0/PKG-INFO
+-rw-r--r--   0 luca      (1001) luca      (1003)    12156 2023-05-21 21:27:34.000000 grape-0.2.0/README.rst
+drwxr-xr-x   0 luca      (1001) luca      (1003)        0 2023-06-06 08:45:20.095202 grape-0.2.0/grape/
+-rw-r--r--   0 luca      (1001) luca      (1003)     2538 2023-05-14 14:45:38.000000 grape-0.2.0/grape/__init__.py
+-rw-r--r--   0 luca      (1001) luca      (1003)       62 2023-06-06 08:44:21.000000 grape-0.2.0/grape/__version__.py
+drwxr-xr-x   0 luca      (1001) luca      (1003)        0 2023-06-06 08:45:20.095202 grape-0.2.0/grape.egg-info/
+-rw-r--r--   0 luca      (1001) luca      (1003)    12754 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1001) luca      (1003)      210 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1001) luca      (1003)        1 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1001) luca      (1003)       71 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/requires.txt
+-rw-r--r--   0 luca      (1001) luca      (1003)        6 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/top_level.txt
+-rw-r--r--   0 luca      (1001) luca      (1003)       38 2023-06-06 08:45:20.095202 grape-0.2.0/setup.cfg
+-rw-r--r--   0 luca      (1001) luca      (1003)     1924 2023-06-06 08:44:35.000000 grape-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grape-0.1.9/README.rst` & `grape-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,90 @@
-|logo|
+Metadata-Version: 2.1
+Name: grape
+Version: 0.2.0
+Summary: 🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.
+Home-page: https://github.com/AnacletoLAB/grape
+Author: Luca Cappelletti, Tommaso Fontana, Vida Ravanmehr, Peter Robinson
+Author-email: luca.cappelletti1@unimi.it, tommaso.fontana@mail.polimi.it, vida.ravanmehr@jax.org, peter.robinson@jax.org
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
 
-GraPE
+🍇 GRAPE
 ===================================
 |pip| |downloads| |tutorials| |documentation| |python_version| |DOI| |license| |telegram| |discord| |twitter|
 
-`GraPE`_ (*Graph Processing and Embedding*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
+`GRAPE`_ (*Graph Representation leArning, Predictions and Evaluation*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
 
-The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept.of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
+The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept. of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
 
-`GraPE`_ is composed of two main modules: `Ensmallen`_ (*ENabler  of  SMALL  runtimE  and  memory  Needs*) and `Embiggen`_ (*EMBeddInG  GENerator*), that run synergistically using parallel computation and efficient data structures.
+The library is composed of two main modules, `Ensmallen <https://github.com/AnacletoLAB/ensmallen>`_, which is the Rust/Python high-performance graph processing submodule, and `Embiggen <https://github.com/monarch-initiative/embiggen>`_, which is the Python Graph Representation learning, Prediction and Evaluation submodule.
 
-`Ensmallen`_ efficiently executes graph processing operations including large-scale first and second-order random walks, while
-`Embiggen`_ leverages the large amount of sampled random walks generated by `Ensmallen`_ by computing effective node and edge embeddings. 
-Beside being helpful for unsupervised exploratory analysis of graphs, the computed embeddings can be used for trainining any of the flexible neural models for edge and node label prediction, provided by `Embiggen`_ itself.
-
-The following figure shows the main relationships between `Ensmallen`_ and `Embiggen`_ modules:
-
-.. image:: images/link_prediction_model.png
-    :width:  900
-    :align: left
-
-
-Installation of `GraPE`_
+Installation of `GRAPE`_
 ----------------------------------------------
-
-For most computers you can just download it using pip:
+As usual, just install it from PyPi by running:
 
 .. code:: shell
 
     pip install grape
-    
-Since Ensmallen is written in Rust, on PyPi we distribute pre-compiled packages for :code:`Windows, Linux, MacOs` for the Python version :code:`3.6+` for :code:`x86_64` and :code:`Arm` cpus.
-
-For the Linux binaries we follow the `Python's ManyLinux2010 (PEP 571) <https://www.python.org/dev/peps/pep-0571/>`_ standard which requires libc version >= 2.12, this version was releasted in 03/08/2010 so any Linux System in the last ten years should be compatible. To check your current libc version you can run :code:`ldd --version`.
 
-These requirements were chosen to provide a good tradeoff between compatability and performance. 
-If your system is not compatible, you can `manually compile Ensmallen <https://github.com/AnacletoLAB/ensmallen/blob/master/bindings/python/README.md>`_ for any  Os, libc version, and CPU architecture (such as Arm, AArch64, RiscV, Mips) which are supported by Rust and LLVM. 
-Manually compiling Ensmallen might require around half an hour and 10GB of RAM, if you encounter any error during the installation and/or compilation feel free to open an Issue here on Github and we will help troubleshoot it.
+Generally, the installation does not take longer than a minute.
 
+It is possible to `manually compile Ensmallen <https://github.com/AnacletoLAB/ensmallen/blob/master/CONTRIBUTING.md>`_ for any OS, libc version, and CPU architecture (such as Arm, AArch64, RiscV, Mips) which are supported by Rust and LLVM. Just open an issue if you need some help.
 
 Main functionalities of the library
 ----------------------------------------------
 
-* Robust graph loading and automatic graph retrieval:
-
-     * More than 80000 graphs directly available from the library for benchmarking
-     * Support for multiple graph formats
-     * Automatic human readable reports of format errors
-     * Automatic human readable reports of the main graph characteristics
-
-* Random walks:
-
-     * Exact and approximated first and second order random walks
-     * Massive generation of sampled random walks for graph embedding
-     * Automatic dispatching of 8 optimized random walk algorithms depending on the parameters of the random walk and the type (weighted/unweighted) of the graph
-
-* Node embedding models:
-
-    * SkipGram
-    * CBOW
-    * GloVe
-    
-* Edge and node prediction models:
-
-    * Decision Trees
-    * Random Forest
-    * Perceptron
-    * Multi-Layer Perceptron
-    * Deep Neural Networks
-    * Interface for general models
-    * And more!
-
-* Preprocessing for node embedding and edge prediction:
-
-    * Lazy generation of skip-grams from random walks
-    * Lazy generation of balanced batches for edge prediction
-    * GloVe co-occurence matrix computation
-    
-* Graph processing operations:
-
-    * Optimized filtering by node, edge and components characteristics
-    * Optimized algebraic set operations on graphs
-    * Automatic generation of reports summarizing graph features in natural language
-    
-* Graph algorithms:
-
-    * Breadth and Depth-first search
-    * Dijkstra, Tarjan's strongly connected component
-    * Efficient Diameter computation, spanning arborescence and connected components
-    * Approximated vertex cover, triads counting, transitivity, clustering coefficient and triangles counting
-    * Betweenness and stress centrality, Closeness and harmonic centrality
-    
-* Graph visualization tools: visualization of node and edge properties
-        
+|features|
 
+* Robust graph loading and graph retrieval:
+    * `80K+ graphs <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Ensmallen_Automatic_graph_retrieval_utilities.ipynb>`_
+    * `Support for multiple graph formats <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Loading_a_Graph_in_Ensmallen.ipynb>`_
+    * `human readable reports of graph characteristics <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Create%20extensive%20knowledge%20graph%20reports%20using%20GRAPE.ipynb>`_
+* 60+ Node embedding models, with easy integration of third parties libraries.
+    * DeepWalk, Walklets and Node2Vec-based CBOW, SkipGram and GloVe, `also with degree normalization! <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20degree-normalization%20in%20random-walk-based%20embedding%20models.ipynb>`_
+    * `First <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_First-order_LINE_to_embed_Cora.ipynb>`_ and `second order LINE <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_Second-order_LINE_to_embed_Cora.ipynb>`_
+    * Unstructured, Structured Embedding, TransE
+    * All embedding models have an MMAPP-ed versions to allow for very large embeddings
+    * All embedding models have support for mixed precision, allowing embedding using 16 bits floats
+    * Integrated models from `Karate Club <https://github.com/benedekrozemberczki/karateclub>`_ and `PyKEEN <https://github.com/pykeen/pykeen>`_
+* 20+ Classifier models, with easy integration of third parties libraries.
+    * All sklearn models, adapted for edge prediction, edge-label prediction and node-label prediction
+    * GraphSAGE and Kipf GCN for `edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Multi-modal%20GCN%20for%20edge%20prediction.ipynb>`_, edge-label prediction and node-label prediction
+    * `Baseline Perceptron for edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Edge%20Predictions%20on%20STRING%20Homo%20Sapiens%20using%20a%20Perceptron.ipynb>`_
+    * `Integrated support to parallelize holdouts across a SLURM cluster <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20HPC%20SLURM%20in%20the%20GRAPE%20evaluation%20pipelines.ipynb>`_
+* Graph processing: if NetworkX has it, odds are good we have it and it is way faster!
+    * Resnik, Jaccard, Ancestors Jaccard similarities
+    * `Diameter <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Exact%20billion-scale%20graph%20diameter%20with%20GRAPE.ipynb>`_, `Vertex cover <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%202-approximated%20vertex%20cover%20with%20GRAPE.ipynb>`_, `connected components <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20connected%20components%20with%20GRAPE.ipynb>`_, `Triangles <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20triangles%20on%20multigraphs%20with%20GRAPE.ipynb>`_, `Squares <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20squares%20on%20multigraphs%20with%20GRAPE.ipynb>`__, `Betweenness Centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Betweenness%20Centrality%20with%20GRAPE.ipynb>`__, `HyperBall-based approximated Closeness and Harmonic centralities <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__, `Exact Closeness centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Weighted%20and%20Unweighted%20Closeness%20Centrality%20with%20GRAPE.ipynb>`__ and `Exact Harmonic centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__
+    * Filters on graph properties and `set operations on graph edges <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Graph%20set%20algebra.ipynb>`_
+* Graph visualization tools
+    * TSNE, UMAP, PCA of embeddings
+    * Edge properties
 
 Tutorials
 ----------------------------------------------
-You can find tutorials covering various aspects of the GraPE library `here <https://github.com/AnacletoLAB/grape/tree/main/tutorials>`_. All tutorials are as self-contained as possible and can be immediately executed on COLAB.
-
-If you want to get quickly started, after having installed `GraPE`_ from Pypi as described above, you can try running the following example using the SkipGram embedding model on the Cora-graph:
-
-.. code:: python
-
-    from grape.datasets.linqs import Cora, get_words_data
-    from grape.embedders import SkipGramEnsmallen
-    from graph.edge_prediction import RandomForestEdgePrediction
-    from grape import GraphVisualizer
-
-    # Dowload, load up the graph and its node features
-    graph, _ = get_words_data(Cora())
-    
-    # Create the model
-    model = SkipGramEnsmallen()
-    node_embedding = model.fit_transform(graph).get_node_embedding_from_index(0)
-
-    # Visualize the obtained node embeddings
-    visualizer = GraphVisualizer(graph, node_embedding_method_name="SkipGram")
-    visualizer.fit_and_plot_all(node_embedding)
-    plt.show()
-
-
-You can `see a tutorial detailing the above script here <https://github.com/AnacletoLAB/grape/blob/main/tutorials/SkipGram_to_embed_Cora.ipynb>`_, and you `can run it on COLAB from here <https://colab.research.google.com/github/AnacletoLAB/grape/blob/main/tutorials/SkipGram_to_embed_Cora.ipynb>`_.
+You can find tutorials covering various aspects of the GRAPE library `here <https://github.com/AnacletoLAB/grape/tree/main/tutorials>`_.
+All tutorials are as self-contained as possible and can be immediately executed on COLAB.
 
 If you believe that any example may be of help, do feel free to `open a GitHub issue describing what we are missing in this tutorial <https://github.com/AnacletoLAB/grape/issues/new>`_.
 
 Documentation
 ----------------------------------------------
-On line documentation
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+On line documentation (currently being updated)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 The on line documentation of the library is available `here <https://anacletolab.github.io/grape/index.html>`__.
 Since Ensmallen is written in Rust, and PyO3 (the crate we use for the Python bindings), `doesn't support typing <https://github.com/PyO3/pyo3/issues/510>`_, the documentation is obtained generating an empty skeleton package. This allows to have a proper documentation but you won't be able to see the source-code in it. 
 
 Using the automatic method suggestions utility
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-To aid working with the library, Grape provides an integrated recommender system meant to help you either to find a method or, if a method has been renamed for any reason, find its new name.
+To aid working with the library, GRAPE provides an integrated recommender system meant to help you either to find a method or, if a method has been renamed for any reason, find its new name.
 
 As an example, after having loaded the `STRING Homo Sapiens graph <https://string-db.org/cgi/organisms>`_, the function for computing the connected components can be retrieved by simply typing components as follows: 
 
 .. code:: python
 
     from grape.datasets.string import HomoSapiens
 
@@ -199,36 +145,37 @@
     -------
     ValueError
         If the given graph is directed.
     ValueError
         If the system configuration does not allow for the creation of the thread pool.
 
 
-You can try `to run the code described above on COLAB <https://colab.research.google.com/github/AnacletoLAB/grape/blob/main/tutorials/Method_recommender_system.ipynb>`_.
-
-
-Cite GraPE
+Cite GRAPE
 ----------------------------------------------
 Please cite the following paper if it was useful for your research:
 
 .. code:: bib
 
     @misc{cappelletti2021grape,
-      title={GraPE: fast and scalable Graph Processing and Embedding}, 
+      title={GRAPE: fast and scalable Graph Processing and Embedding}, 
       author={Luca Cappelletti and Tommaso Fontana and Elena Casiraghi and Vida Ravanmehr and Tiffany J. Callahan and Marcin P. Joachimiak and Christopher J. Mungall and Peter N. Robinson and Justin Reese and Giorgio Valentini},
       year={2021},
       eprint={2110.06196},
       archivePrefix={arXiv},
       primaryClass={cs.LG}
     }
     
 
 .. |pip| image:: https://badge.fury.io/py/grape.svg
     :target: https://badge.fury.io/py/grape
     :alt: Pypi project
+    
+.. |features| image:: https://github.com/AnacletoLAB/grape/blob/main/images/sequence_diagram.png?raw=true
+    :target: https://github.com/AnacletoLAB/grape
+    :alt: Features
 
 .. |downloads| image:: https://pepy.tech/badge/grape
     :target: https://pepy.tech/badge/grape
     :alt: Pypi total project downloads 
 
 .. _Grape: https://github.com/AnacletoLAB/grape
 .. _Ensmallen: https://github.com/AnacletoLAB/ensmallen
@@ -251,15 +198,15 @@
     :target: https://anacletolab.github.io/grape/index.html
     :alt: Documentation
 
 .. |DOI| image:: https://img.shields.io/badge/DOI-10.48550/arXiv.2110.06196-blue.svg
     :target: https://doi.org/10.48550/arXiv.2110.06196
     :alt: DOI
 
-.. |python_version| image:: https://img.shields.io/badge/Python-3.6+-blue.svg
+.. |python_version| image:: https://img.shields.io/badge/Python-3.7+-blue.svg
     :target: https://pypi.org/project/embiggen/#history
     :alt: Supported Python versions
 
 .. |twitter| image:: https://badges.aleen42.com/src/twitter.svg
     :target: https://twitter.com/grapelib
     :alt: Twitter
 
@@ -269,8 +216,10 @@
 
 .. |discord| image:: https://badges.aleen42.com/src/discord.svg
     :target: https://discord.gg/Nda2cqYvTN
     :alt: Discord Server
 
 .. |logo| image:: images/grape_logo.png
     :target: https://github.com/AnacletoLAB/grape
-    :width:  80
+    :width:  80
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grape-0.1.9/setup.py` & `grape-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "Peter Robinson": "peter.robinson@jax.org",
 }
 
 
 setup(
     name='grape',
     version=__version__,
-    description="🍇 GraPE is a Rust/Python library for high-performance Graph Processing and Embedding.",
+    description="🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.",
     long_description=long_description,
     url="https://github.com/AnacletoLAB/grape",
     author=", ".join(list(authors.keys())),
     author_email=", ".join(list(authors.values())),
     # Choose your license
     license='MIT',
     include_package_data=True,
@@ -56,11 +56,14 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     tests_require=test_deps,
     install_requires=[
-        "ensmallen>=0.8.6",
-        "embiggen>=0.11.13",
+        "downloaders",
+        "bioregistry",
+        "py-cpuinfo",
+        "ensmallen>=0.8.60",
+        "embiggen>=0.11.54",
     ]
 )
```

