# Comparing `tmp/DNASpiderWeb-1.0-py3-none-any.whl.zip` & `tmp/DNASpiderWeb-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 40433 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat      810 b- defN 22-Feb-18 12:48 dsw/__init__.py
--rw-rw-rw-  2.0 fat     6649 b- defN 22-Feb-23 09:42 dsw/biofilter.py
--rw-rw-rw-  2.0 fat    39865 b- defN 22-Apr-03 13:49 dsw/graphized.py
--rw-rw-rw-  2.0 fat    13601 b- defN 22-Mar-12 07:17 dsw/operation.py
--rw-rw-rw-  2.0 fat    34242 b- defN 22-Apr-06 08:38 dsw/spiderweb.py
+Zip file size: 541996 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat      901 b- defN 22-Jul-12 13:26 dsw/__init__.py
+-rw-rw-rw-  2.0 fat     6689 b- defN 23-Feb-24 05:33 dsw/biofilter.py
+-rw-rw-rw-  2.0 fat    36014 b- defN 23-Feb-24 05:36 dsw/graphized.py
+-rw-rw-rw-  2.0 fat    13764 b- defN 23-Feb-24 05:37 dsw/operation.py
+-rw-rw-rw-  2.0 fat    36995 b- defN 23-Feb-24 05:41 dsw/spiderweb.py
 -rw-rw-rw-  2.0 fat      718 b- defN 21-Dec-31 06:38 tests/test_accessor_vs_latter_map.py
 -rw-rw-rw-  2.0 fat     5409 b- defN 21-Dec-31 06:38 tests/test_accessor_vs_matrix.py
--rw-rw-rw-  2.0 fat     4637 b- defN 21-Dec-31 06:38 tests/test_bio_filters.py
--rw-rw-rw-  2.0 fat    18281 b- defN 21-Dec-31 06:38 tests/test_capacities.py
--rw-rw-rw-  2.0 fat     3632 b- defN 22-Feb-20 13:12 tests/test_coding.py
--rw-rw-rw-  2.0 fat     2192 b- defN 22-Jan-09 10:38 tests/test_generating.py
--rw-rw-rw-  2.0 fat     2583 b- defN 21-Dec-31 06:38 tests/test_number_vs_binary_message.py
--rw-rw-rw-  2.0 fat     2192 b- defN 21-Dec-31 06:38 tests/test_number_vs_dna_string.py
+-rw-rw-rw-  2.0 fat     4828 b- defN 23-Feb-24 05:40 tests/test_bio_filters.py
+-rw-rw-rw-  2.0 fat    18689 b- defN 23-Feb-24 05:45 tests/test_capacities.py
+-rw-rw-rw-  2.0 fat     4447 b- defN 23-Feb-24 05:32 tests/test_coding.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-Feb-24 05:45 tests/test_generating.py
+-rw-rw-rw-  2.0 fat     2577 b- defN 23-Feb-24 05:49 tests/test_number_vs_binary_message.py
+-rw-rw-rw-  2.0 fat     2250 b- defN 23-Feb-24 05:51 tests/test_number_vs_dna_sequence.py
 -rw-rw-rw-  2.0 fat     1864 b- defN 21-Dec-31 06:38 tests/test_operations.py
--rw-rw-rw-  2.0 fat     1411 b- defN 21-Dec-31 06:38 tests/test_shuffling.py
--rw-rw-rw-  2.0 fat     3632 b- defN 22-Feb-20 13:12 tests/test_transcoding.py
--rw-rw-rw-  2.0 fat    35817 b- defN 22-Apr-07 15:14 DNASpiderWeb-1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1700 b- defN 22-Apr-07 15:14 DNASpiderWeb-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 22-Apr-07 15:14 DNASpiderWeb-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 22-Apr-07 15:14 DNASpiderWeb-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1700 b- defN 22-Apr-07 15:14 DNASpiderWeb-1.0.dist-info/RECORD
-21 files, 181042 bytes uncompressed, 37699 bytes compressed:  79.2%
+-rw-rw-rw-  2.0 fat     1623 b- defN 23-Feb-24 05:52 tests/test_repair.py
+-rw-rw-rw-  2.0 fat     1413 b- defN 23-Mar-06 13:58 tests/test_shuffling.py
+-rw-rw-rw-  2.0 fat   541985 b- defN 23-Jun-06 09:02 DNASpiderWeb-1.1.dist-info/LICENSE.pdf
+-rw-rw-rw-  2.0 fat     1602 b- defN 23-Jun-06 09:02 DNASpiderWeb-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-06 09:02 DNASpiderWeb-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-06 09:02 DNASpiderWeb-1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1702 b- defN 23-Jun-06 09:02 DNASpiderWeb-1.1.dist-info/RECORD
+21 files, 685791 bytes uncompressed, 539260 bytes compressed:  21.4%
```

## zipnote {}

```diff
@@ -30,35 +30,35 @@
 
 Filename: tests/test_generating.py
 Comment: 
 
 Filename: tests/test_number_vs_binary_message.py
 Comment: 
 
-Filename: tests/test_number_vs_dna_string.py
+Filename: tests/test_number_vs_dna_sequence.py
 Comment: 
 
 Filename: tests/test_operations.py
 Comment: 
 
-Filename: tests/test_shuffling.py
+Filename: tests/test_repair.py
 Comment: 
 
-Filename: tests/test_transcoding.py
+Filename: tests/test_shuffling.py
 Comment: 
 
-Filename: DNASpiderWeb-1.0.dist-info/LICENSE
+Filename: DNASpiderWeb-1.1.dist-info/LICENSE.pdf
 Comment: 
 
-Filename: DNASpiderWeb-1.0.dist-info/METADATA
+Filename: DNASpiderWeb-1.1.dist-info/METADATA
 Comment: 
 
-Filename: DNASpiderWeb-1.0.dist-info/WHEEL
+Filename: DNASpiderWeb-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: DNASpiderWeb-1.0.dist-info/top_level.txt
+Filename: DNASpiderWeb-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: DNASpiderWeb-1.0.dist-info/RECORD
+Filename: DNASpiderWeb-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dsw/__init__.py

```diff
@@ -1,13 +1,14 @@
 from dsw.biofilter import DefaultBioFilter, LocalBioFilter
 
-from dsw.spiderweb import encode, decode, set_vt, repair_dna
-from dsw.spiderweb import find_vertices, connect_valid_graph, connect_coding_graph, create_random_shuffles
+from dsw.spiderweb import encode, decode
+from dsw.spiderweb import find_vertices, connect_valid_graph, connect_coding_graph
+from dsw.spiderweb import set_vt, repair_dna, remove_nasty_arc
+from dsw.spiderweb import create_random_shuffles
 
 from dsw.graphized import accessor_to_adjacency_matrix, adjacency_matrix_to_accessor
-from dsw.graphized import accessor_to_latter_map, latter_map_to_accessor, remove_useless
-from dsw.graphized import obtain_leaf_vertices, obtain_formers, obtain_latters, get_complete_accessor
-from dsw.graphized import approximate_capacity, path_matching
+from dsw.graphized import accessor_to_latter_map, latter_map_to_accessor
+from dsw.graphized import obtain_vertices, obtain_leaf_vertices, obtain_formers, obtain_latters, get_complete_accessor
+from dsw.graphized import approximate_capacity, path_matching, remove_useless, calculate_intersection_score
 
-from dsw.operation import Monitor
 from dsw.operation import calculus_addition, calculus_subtraction, calculus_multiplication, calculus_division
-from dsw.operation import dna_to_number, number_to_dna, bit_to_number, number_to_bit
+from dsw.operation import Monitor, dna_to_number, number_to_dna, bit_to_number, number_to_bit
```

## dsw/biofilter.py

```diff
@@ -26,15 +26,15 @@
 
 class LocalBioFilter(DefaultBioFilter):
 
     def __init__(self, observed_length, max_homopolymer_runs=None, gc_range=None, undesired_motifs=None):
         """
         Initialize the screen of local biochemical constraints.
 
-        :param observed_length: length of the DNA string observed in the window.
+        :param observed_length: length of the DNA sequence observed in the window.
         :type observed_length: int
 
         :param max_homopolymer_runs: maximum homopolymer runs.
         :type max_homopolymer_runs: int
 
         :param gc_range: range of GC content.
         :type gc_range: list
@@ -42,114 +42,114 @@
         :param undesired_motifs: undesired DNA motifs.
         :type undesired_motifs: list
 
         Example
             >>> from dsw import LocalBioFilter
             >>> bio_filter = LocalBioFilter(observed_length=8, \
                                             max_homopolymer_runs=2, gc_range=[0.4, 0.6], undesired_motifs=["GC"])
-            >>> bio_filter.valid(dna_string="ACGTACGT")
+            >>> bio_filter.valid(dna_sequence="ACGTACGT")
             True
-            >>> bio_filter.valid(dna_string="GCATGCAT")
+            >>> bio_filter.valid(dna_sequence="GCATGCAT")
             False
-            >>> bio_filter.valid(dna_string="AAACCGGA")
+            >>> bio_filter.valid(dna_sequence="AAACCGGA")
             False
 
         .. notes::
             Reference [1] Nick Goldman et al. (2013) Nature
 
             Reference [2] Yaniv Erlich and Dina Zielinski (2017) Science
 
             Reference [3] William H. Press et al. (2020) Proceedings of the National Academy of Sciences
 
-            Reference [4] Hannah F Löchel et al. (2021) Nucleic Acids Research
+            Reference [4] Hannah F Lochel et al. (2021) Nucleic Acids Research
 
             If the maximum homopolymer runs (max_homopolymer_runs) is 1,
-            "AA", "CC", "GG", "TT" cannot be included in tue valid DNA strings.
+            "AA", "CC", "GG", "TT" cannot be included in tue valid DNA sequences.
 
             If the range of GC content (gc_range) is [0.4, 0.6],
-            the GC content of valid DNA strings must between 40% and 60%.
+            the GC content of valid DNA sequences must between 40% and 60%.
 
-            If "GC" in the undesired DNA motifs (undesired_motifs), "GC" cannot be included in tue valid DNA strings.
+            If "GC" in the undesired DNA motifs (undesired_motifs), "GC" cannot be included in tue valid DNA sequences.
             This parameter could contain the restriction enzyme sites or some low compatibility DNA patterns.
         """
         super().__init__(screen_name="Local")
         if max_homopolymer_runs is not None:
             if observed_length < max_homopolymer_runs:
                 raise ValueError("The parameter \"observed_length\" must "
                                  + "longer than the parameter \"max_homopolymer_runs\"!")
         if undesired_motifs is not None:
             for index, undesired_motif in enumerate(undesired_motifs):
                 if len(undesired_motif) > observed_length:
                     raise ValueError("The parameter \"observed_length\" must "
                                      + "longer than the length of any motif in the parameter \"undesired_motifs\"!")
 
-        self._observed_length = observed_length
-        self._max_homopolymer_runs = max_homopolymer_runs
-        self._gc_range = gc_range
-        self._undesired_motifs = undesired_motifs
+        self.observed_length = observed_length
+        self.max_homopolymer_runs = max_homopolymer_runs
+        self.gc_range = gc_range
+        self.undesired_motifs = undesired_motifs
 
-    def valid(self, dna_string, only_last=True):
+    def valid(self, dna_sequence, only_last=True):
         """
-        Judge whether the DNA string meets the local biochemical constraints.
+        Judge whether the DNA sequence meets the local biochemical constraints.
 
-        :param dna_string: DNA string to be judged.
-        :type dna_string: str
+        :param dna_sequence: DNA sequence to be judged.
+        :type dna_sequence: str
 
-        :param only_last: only check the DNA string of the last observed window.
+        :param only_last: only check the DNA sequence of the last observed window.
         :type only_last: bool
 
         :return: judgement.
         :rtype: bool
 
         .. note::
             "only_last" parameter is used to save time.
             For most tree-based coding algorithms,
-            it is not necessary to detect the sub DNA strings observed in each window from scratch every time.
+            it is not necessary to detect the sub DNA sequences observed in each window from scratch every time.
         """
         if only_last:
-            observed_dna_string = dna_string[-self._observed_length:]
+            observed_dna_sequence = dna_sequence[-self.observed_length:]
         else:
-            observed_dna_string = dna_string
+            observed_dna_sequence = dna_sequence
 
-        for nucleotide in observed_dna_string:
+        for nucleotide in observed_dna_sequence:
             if nucleotide not in "ACGT":
                 return False
 
-        if self._max_homopolymer_runs is not None:
+        if self.max_homopolymer_runs is not None:
             for nucleotide in "ACGT":
-                if nucleotide * (1 + self._max_homopolymer_runs) in observed_dna_string:
+                if nucleotide * (1 + self.max_homopolymer_runs) in observed_dna_sequence:
                     return False
 
-        if self._undesired_motifs is not None:
-            for special in self._undesired_motifs:
-                if special in observed_dna_string:
+        if self.undesired_motifs is not None:
+            for special in self.undesired_motifs:
+                if special in observed_dna_sequence:
                     return False
                 reverse_complement = special.replace("A", "t").replace("C", "g").replace("G", "c").replace("T", "a")
                 reverse_complement = reverse_complement[::-1].upper()
-                if reverse_complement in observed_dna_string:
+                if reverse_complement in observed_dna_sequence:
                     return False
 
-        if self._gc_range is not None:
-            if len(observed_dna_string) >= self._observed_length:
-                for index in range(len(observed_dna_string) - self._observed_length + 1):
-                    sub_dna_string = observed_dna_string[index: index + self._observed_length]
-                    gc_count = sub_dna_string.count("C") + sub_dna_string.count("G")
-                    if gc_count > self._gc_range[1] * self._observed_length:
+        if self.gc_range is not None:
+            if len(observed_dna_sequence) >= self.observed_length:
+                for index in range(len(observed_dna_sequence) - self.observed_length + 1):
+                    sub_dna_sequence = observed_dna_sequence[index: index + self.observed_length]
+                    gc_count = sub_dna_sequence.count("C") + sub_dna_sequence.count("G")
+                    if gc_count > self.gc_range[1] * self.observed_length:
                         return False
-                    if gc_count < self._gc_range[0] * self._observed_length:
+                    if gc_count < self.gc_range[0] * self.observed_length:
                         return False
             else:
-                gc_count = observed_dna_string.count("C") + observed_dna_string.count("G")
-                if gc_count > self._gc_range[1] * self._observed_length:
+                gc_count = observed_dna_sequence.count("C") + observed_dna_sequence.count("G")
+                if gc_count > self.gc_range[1] * self.observed_length:
                     return False
-                at_count = observed_dna_string.count("A") + observed_dna_string.count("T")
-                if at_count > (1 - self._gc_range[0]) * self._observed_length:
+                at_count = observed_dna_sequence.count("A") + observed_dna_sequence.count("T")
+                if at_count > (1 - self.gc_range[0]) * self.observed_length:
                     return False
 
         return True
 
     def __str__(self):
         info = self.screen_name + "\n"
-        info += "maximum homopolymer runs : " + str(self._max_homopolymer_runs) + "\n"
-        info += "local GC content range   : " + str(self._gc_range[0]) + "<= GC <=" + str(self._gc_range[1]) + "\n"
-        info += "undesired DNA motifs     : " + str(self._undesired_motifs).replace("\"", "") + "\n"
+        info += "maximum homopolymer runs : " + str(self.max_homopolymer_runs) + "\n"
+        info += "local GC content range   : " + str(self.gc_range[0]) + " <= GC <= " + str(self.gc_range[1]) + "\n"
+        info += "undesired DNA motifs     : " + str(self.undesired_motifs).replace("\"", "") + "\n"
         return info
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## dsw/graphized.py

```diff
@@ -1,17 +1,18 @@
-from numpy import zeros, ones, zeros_like, array, min, median, max, random, log, log2, sum, abs, all, where
+from itertools import combinations
+from numpy import zeros, ones, zeros_like, array, union1d, min, median, max, random, log, log2, sum, abs, all, where
 
 from dsw.operation import Monitor
 
 
 def get_complete_accessor(observed_length, verbose=False):
     """
     Get a complete accessor with the required observed length.
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: complete accessor.
     :rtype: numpy.ndarray
@@ -43,32 +44,28 @@
 
     for vertex_index in range(int(4 ** observed_length)):
         latters = obtain_latters(current=vertex_index, observed_length=observed_length)
         for position, latter_vertex_index in enumerate(latters):
             accessor[vertex_index][position] = latter_vertex_index
 
         if verbose:
-            monitor.output(vertex_index + 1, int(4 ** observed_length))
+            monitor(vertex_index + 1, int(4 ** observed_length))
 
     return accessor
 
 
-def accessor_to_adjacency_matrix(accessor, maximum_length=8, nucleotides=None, verbose=False):
+def accessor_to_adjacency_matrix(accessor, maximum_length=8, verbose=False):
     """
     Convert the accessor (compressed matrix) to its equivalent adjacency matrix.
 
     :param accessor: accessor (compressed matrix).
     :type: numpy.ndarray
 
     :param maximum_length: maximum vertex length (like 8 in general) of the adjacency matrix.
     :type maximum_length: int
-
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list or None
-
     :param verbose: need to print log.
     :type verbose: bool
 
     :raise MemoryError: when you generate a large adjacency matrix that your memory cannot allocate.
     :raise ValueError: when you input a graph of DNA Spider-Web with wrong format.
 
     :return: adjacency matrix of the uncompressed graph.
@@ -97,42 +94,38 @@
                [0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0],
                [0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0],
                [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1]])
 
     .. note::
         The size of accessor is 4 ^ l * 4 and that of corresponding adjacency matrix is 4 ^ l * 4 ^ l.
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     if len(accessor) >= 4 ** maximum_length:
-        raise MemoryError("Unable to allocate adjacency matrix when length of DNA string (vertex) is more than 7.")
+        raise MemoryError("Unable to allocate adjacency matrix when length of DNA sequence (vertex) is more than 7.")
     if accessor.shape[1] != len(nucleotides) or min(accessor) < -1 or max(accessor) > len(accessor) - 1:
         raise ValueError("Wrong format in the accessor")
 
     matrix, monitor = zeros(shape=(len(accessor), len(accessor)), dtype=int), Monitor()
     for vertex_index, vertex in enumerate(accessor):
         matrix[vertex_index][vertex[vertex >= 0]] = 1
 
         if verbose:
-            monitor.output(vertex_index + 1, len(accessor))
+            monitor(vertex_index + 1, len(accessor))
 
     return matrix
 
 
-def adjacency_matrix_to_accessor(matrix, nucleotides=None, verbose=False):
+def adjacency_matrix_to_accessor(matrix, verbose=False):
     """
     Convert the adjacency matrix to the equivalent accessor (compressed matrix).
 
     :param matrix: adjacency matrix.
     :type matrix: numpy.ndarray
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list or None
-
     :param verbose: need to print log.
     :type verbose: bool
 
     :raise ValueError: when you input an adjacency matrix with wrong format.
 
     :return: equivalent compressed matrix (accessor), compress rate = len(n_system) / len(matrix).
     :rtype: numpy.ndarray
@@ -172,46 +165,45 @@
                [ 4,  5,  6,  7],
                [ 8,  9, 10, 11],
                [12, 13, 14, 15]])
 
     .. note::
         The size of accessor is 4 ^ l * 4 and that of corresponding adjacency matrix is 4 ^ l * 4 ^ l.
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     accessor, monitor = -ones(shape=(len(matrix), len(nucleotides)), dtype=int), Monitor()
     observed_length = int(log(len(accessor)) / log(len(nucleotides)))
 
     for vertex_index, vertex in enumerate(matrix):
         next_indices = where(vertex == 1)[0].tolist()
         reference_latters = obtain_latters(current=vertex_index, observed_length=observed_length)
         if list(set(next_indices) | set(reference_latters)) != reference_latters:
             raise ValueError("Wrong format in the adjacency matrix, "
                              + "which cannot be converted to equivalent compressed accessor!")
         saved_information = [index if index in next_indices else -1 for index in reference_latters]
         accessor[vertex_index] = saved_information
 
         if verbose:
-            monitor.output(vertex_index + 1, len(matrix))
+            monitor(vertex_index + 1, len(matrix))
 
     return accessor
 
 
 def accessor_to_latter_map(accessor, verbose=False):
     """
     Convert the accessor to its equivalent latter map.
 
     :param accessor: accessor of graph.
     :type accessor: numpy.ndarray
 
     :param verbose: need to print log.
     :type verbose: bool
 
-    :return: latter vertices map of graph.
+    :return: latter vertex map of graph.
     :rtype: dict
 
     Example
         >>> from numpy import array
         >>> from dsw import get_complete_accessor, accessor_to_latter_map
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
@@ -225,42 +217,39 @@
         The size of accessor is 4 ^ l * 4.
 
         The size of corresponding latter map is further reduced,
         which only retains available information of follow-up vertices.
         However, latter map is not suitable for matrix calculation.
     """
     latter_map, monitor, total = {}, Monitor(), len(accessor)
-    for current, vertex in enumerate(accessor):
-        if not all(vertex == -1):
-            latters = vertex[vertex >= 0].tolist()
-            if len(latters) > 0:
-                latter_map[current] = latters
+
+    locations = where(sum(((accessor + 1).astype(bool)), axis=1).astype(int) > 0)[0]
+    for index, location in enumerate(locations):
+        vertex = accessor[location]
+        latter_map[location] = vertex[vertex >= 0].tolist()
 
         if verbose:
-            monitor.output(current_state=current + 1, total_state=total)
+            monitor(current_state=index + 1, total_state=len(locations))
 
     return latter_map
 
 
-def latter_map_to_accessor(latter_map, observed_length, threshold=None, nucleotides=None, verbose=False):
+def latter_map_to_accessor(latter_map, observed_length, threshold=None, verbose=False):
     """
     Convert the latter map to the equivalent accessor.
 
-    :param latter_map: latter vertices map of graph.
+    :param latter_map: latter vertex map of graph.
     :type latter_map: dict
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
     :param threshold: minimum out-degree threshold.
     :type threshold: int or None
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list or None
-
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: equivalent accessor.
     :rtype: numpy.ndarray
 
     Example
@@ -288,16 +277,15 @@
     .. note::
         The size of accessor is 4 ^ l * 4.
 
         The size of corresponding latter map is further reduced,
         which only retains available information of follow-up vertices.
         However, latter map is not suitable for matrix calculation.
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     monitor = Monitor()
 
     if threshold is not None:
         latter_map = remove_useless(latter_map, threshold=threshold, verbose=verbose)
 
     accessor = -ones(shape=(len(nucleotides) ** observed_length, len(nucleotides)), dtype=int)
@@ -307,24 +295,24 @@
 
         total = len(latter_map.items())
         for current, (former_vertex, latter_vertices) in enumerate(latter_map.items()):
             for latter_vertex in latter_vertices:
                 accessor[former_vertex, latter_vertex % len(nucleotides)] = latter_vertex
 
             if verbose:
-                monitor.output(current + 1, total)
+                monitor(current + 1, total)
 
     return accessor
 
 
 def remove_useless(latter_map, threshold, verbose=False):
     """
     Remove useless vertices (the out-degree of witch less than threshold) in the latter map.
 
-    :param latter_map: latter vertices map of graph.
+    :param latter_map: latter vertex map of graph.
     :type latter_map: dict
 
     :param threshold: minimum out-degree threshold.
     :type threshold: int
 
     :param verbose: need to print log.
     :type verbose: bool
@@ -356,15 +344,15 @@
         for current, (former_vertex, latter_vertices) in enumerate(latter_map.items()):
             if len(latter_vertices) < threshold:
                 remove_vertices.append(former_vertex)
             else:
                 saved_vertices.append(former_vertex)
 
             if verbose:
-                monitor.output(current + 1, total, extra={"round": round_number})
+                monitor(current + 1, total, extra={"round": round_number})
 
         if verbose:
             print("Remove vertices " + str(remove_vertices) + " and load a novel latter map.")
 
         new_latter_map, remove_flag = {}, False
         for current, (former_vertex, latter_vertices) in enumerate(latter_map.items()):
             if former_vertex not in remove_vertices:
@@ -373,40 +361,37 @@
                     if (latter_vertex not in remove_vertices) and (latter_vertex in saved_vertices):
                         available_latter_vertices.append(latter_vertex)
                     else:
                         remove_flag = True
                 new_latter_map[former_vertex] = available_latter_vertices
 
             if verbose:
-                monitor.output(current + 1, total, extra={"round": round_number})
+                monitor(current + 1, total, extra={"round": round_number})
 
         latter_map = new_latter_map
 
         round_number += 1
 
         if not remove_flag:
             break
 
     return latter_map
 
 
-def obtain_formers(current, observed_length, nucleotides=None):
+def obtain_formers(current, observed_length):
     """
-    Obtain former vertex indices based on the current vertex index.
+    Obtain former vertex given_amino_acids based on the current vertex index.
 
     :param current: current vertex index.
     :type current: int
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
-    :return: former vertex indices.
+    :return: former vertex given_amino_acids.
     :rtype: list
 
     Example
         >>> from dsw import obtain_formers
         >>> current = 0
         >>> obtain_formers(current=current, observed_length=2)
         [0, 4, 8, 12]
@@ -421,39 +406,35 @@
         >>> obtain_formers(current=current, observed_length=7)
         [0, 4096, 8192, 12288]
         >>> obtain_formers(current=current, observed_length=8)
         [0, 16384, 32768, 49152]
         >>> obtain_formers(current=current, observed_length=9)
         [0, 65536, 131072, 196608]
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     formers = []
     for former_value in range(len(nucleotides)):
         former = current // len(nucleotides) + former_value * int(len(nucleotides) ** (observed_length - 1))
         formers.append(former)
 
     return formers
 
 
-def obtain_latters(current, observed_length, nucleotides=None):
+def obtain_latters(current, observed_length):
     """
-    Obtain latter vertex indices based on the current vertex index.
+    Obtain latter vertex given_amino_acids based on the current vertex index.
 
     :param current: current vertex index.
     :type current: int
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
-    :return: latter vertex indices.
+    :return: latter vertex given_amino_acids.
     :rtype: list
 
     Example
         >>> from dsw import obtain_latters
         >>> current = 0
         >>> obtain_latters(current=current, observed_length=2)
         [0, 1, 2, 3]
@@ -468,42 +449,65 @@
         >>> obtain_latters(current=current, observed_length=7)
         [0, 1, 2, 3]
         >>> obtain_latters(current=current, observed_length=8)
         [0, 1, 2, 3]
         >>> obtain_latters(current=current, observed_length=9)
         [0, 1, 2, 3]
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     latters = []
     for latter_value in range(len(nucleotides)):
         latter = int((current * len(nucleotides) + latter_value) % (len(nucleotides) ** observed_length))
         latters.append(latter)
 
     return latters
 
 
+def obtain_vertices(accessor):
+    """
+    Obtain available vertices from the established graph.
+
+    :param accessor: accessor of graph.
+    :type accessor: numpy.ndarray
+
+    :return: vertex list.
+    :rtype: numpy.ndarray
+
+    Example
+        >>> from numpy import array
+        >>> from dsw import obtain_vertices
+        >>> # accessor with GC-balanced
+        >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
+                              [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
+                              [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
+                              [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
+        >>> obtain_vertices(accessor=accessor)
+        array([ 1,  2,  4,  7,  8, 11, 13, 14])
+    """
+    return where(sum(((accessor + 1).astype(bool)), axis=1).astype(bool) == 1)[0].astype(int)
+
+
 def obtain_leaf_vertices(vertex_index, depth, accessor=None, latter_map=None):
     """
     Obtain leaf vertices in required depth of the tree with the rooted vertex.
 
     :param vertex_index: vertex index in the graph.
     :type vertex_index: int
 
     :param depth: stride of the breadth-first search.
     :type depth: int
 
     :param accessor: accessor of graph.
     :type accessor: numpy.ndarray
 
-    :param latter_map: latter vertices map of graph.
+    :param latter_map: latter vertex map of graph.
     :type latter_map: dict
 
-    :return: indices of required leaf vertex.
+    :return: given_amino_acids of required leaf vertex.
     :rtype: numpy.ndarray
 
     Example
         >>> from numpy import array
         >>> from dsw import obtain_leaf_vertices
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
@@ -550,16 +554,16 @@
 
     else:
         raise ValueError("We need to select a data type (accessor and latter map) input for the graph!")
 
     return array(branch)
 
 
-def approximate_capacity(accessor, tolerance_level=-10, repeats=1, maximum_iteration=500,
-                         need_process=False, verbose=False):
+# noinspection PyUnresolvedReferences
+def approximate_capacity(accessor, tolerance_level=-10, repeats=1, maximum_iteration=500, process=False, verbose=False):
     """
     Approximate the capacity of the specific graph through Perron–Frobenius theorem.
 
     :param accessor: accessor of graph.
     :type accessor: numpy.ndarray
 
     :param tolerance_level: error tolerance of power iteration.
@@ -567,16 +571,16 @@
 
     :param repeats: random repeats for approximating the capacity.
     :type repeats: int
 
     :param maximum_iteration: maximum iteration in the power method.
     :type maximum_iteration: int
 
-    :param need_process: need eigenvalue in the process.
-    :type need_process: bool
+    :param process: need eigenvalue in the process.
+    :type process: bool
 
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: capacity of this graph (accessor) and process values if required.
     :rtype: float or (float, list)
 
@@ -584,19 +588,18 @@
         >>> from numpy import array, random
         >>> from dsw import approximate_capacity
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
-        >>> approximate_capacity(accessor=accessor, tolerance_level=-10, repeats=10)
+        >>> approximate_capacity(accessor=accessor, tolerance_level=-10, repeats=2, process=False)
         1.0
         >>> random.seed(0)
-        >>> capacity, processes = approximate_capacity(accessor=accessor, tolerance_level=-10, repeats=2, \
-                                                       need_process=True)
+        >>> capacity, processes = approximate_capacity(accessor=accessor, tolerance_level=-10, repeats=2, process=True)
         >>> capacity
         1.0
         >>> ["%.5f" % _ for _ in processes[0]]
         ['0.57779', '0.91175', '1.00000', '1.00000']
         >>> ["%.5f" % _ for _ in processes[1]]
         ['0.81488', '0.68189', '1.00000', '1.00000']
 
@@ -608,296 +611,242 @@
         Reference [3] Brian H. Marcus et al. (2001) Lecture notes
 
         Reference [4] Nabil Kahale (1995) Journal of the ACM
 
         Reference [5] William Ford (2014) Academic Press
     """
     if all(accessor == -1):
-        if need_process:
+        if process:
             return (0.0, [0.0]) if repeats == 1 else (0.0, [[0.0] for _ in range(repeats)])
         else:
             return 0.0
 
     ignore_positions = where(sum(accessor, axis=1) == -len(accessor[0]))[0]
 
-    results, process = [], []
+    results, record = [], []
     for repeat in range(repeats):
         if verbose and repeats > 1:
             print("Approximate capacity in " + str(repeat + 1) + " (" + str(repeats) + ") times.")
 
-        process.append([])
+        record.append([])
         if repeats > 1:
             last_eigenvector = abs(random.random(size=(len(accessor),)))  # Random initialization for a faster fitness.
         else:
             last_eigenvector = ones(shape=(len(accessor),), dtype=float)
 
         last_eigenvector[ignore_positions] = 0.0  # refers to the vertex without follow-up vertices.
 
         monitor, queue, last_eigenvalue, current = Monitor(), [], None, 0
         while True:
             eigenvector = zeros_like(last_eigenvector)
             for positions in accessor.T:
                 available = where(positions >= 0)
                 eigenvector[available] += last_eigenvector[positions[available]]
             eigenvalue = max(eigenvector)
-            eigenvector = eigenvector / eigenvalue
-            process[-1].append(log2(eigenvalue))
+            if eigenvalue > 0:
+                eigenvector = eigenvector / eigenvalue
+            else:
+                eigenvector = eigenvector * 0.0
+            record[-1].append(log2(eigenvalue) if eigenvalue > 10 ** tolerance_level else 0.0)
 
             if last_eigenvalue is not None:
-                relative_error = abs(eigenvalue - last_eigenvalue) / last_eigenvalue
+                if last_eigenvalue > 0.0:
+                    relative_error = abs(eigenvalue - last_eigenvalue) / last_eigenvalue
+                else:
+                    relative_error = 0.0
                 queue.append(eigenvalue)
 
                 if verbose and current + 1 < maximum_iteration:
-                    monitor.output(current + 1, maximum_iteration,
-                                   extra={"largest eigenvalue": "%.5f" % eigenvalue,
-                                          "relative error": "%.5f" % relative_error})
+                    monitor(current + 1, maximum_iteration,
+                            extra={"largest eigenvalue": "%.5f" % eigenvalue, "error": "%.5f" % relative_error})
 
                 is_finished = False
                 if relative_error < 10 ** tolerance_level:
-                    if eigenvalue < 1.0:
-                        eigenvalue = 1.0
-                    results.append(log2(eigenvalue))
+                    results.append(log2(eigenvalue) if eigenvalue > 10 ** tolerance_level else 0.0)
                     is_finished = True
 
                 if len(queue) > maximum_iteration:
                     eigenvalue = median(queue)
-                    if eigenvalue < 1.0:  # meaningless result.
-                        eigenvalue = 1.0
-                    results.append(log2(eigenvalue))
+                    results.append(log2(eigenvalue) if eigenvalue > 10 ** tolerance_level else 0.0)
                     is_finished = True
 
                 if is_finished:
                     if verbose:
-                        monitor.output(maximum_iteration, maximum_iteration,
-                                       extra={"capacity": "%.5f" % results[-1]})
+                        monitor(maximum_iteration, maximum_iteration, extra={"capacity": "%.5f" % results[-1]})
                     break
 
             last_eigenvalue, last_eigenvector, current = eigenvalue, eigenvector, current + 1
 
-    if need_process:
-        return (median(results), process[0]) if repeats == 1 else (median(results), process)
+    if process:
+        return (median(results), record[0]) if repeats == 1 else (median(results), record)
     else:
         return median(results)
 
 
-def path_matching(dna_string, accessor, index_queue, occur_location, nucleotides=None,
-                  has_insertion=False, has_deletion=False, verbose=False):
+def path_matching(dna_sequence, accessor, previous_index, occur_location, has_indel=False, nucleotides=None):
     """
-    Perform saturation repair at the selected position and obtain the DNA strings matching the path of accessor.
+    Perform saturation repair at the selected position and obtain the DNA sequences matching the path of accessor.
 
-    :param dna_string: DNA string waiting for saturation substitution in the specific location.
-    :type dna_string: str
+    :param dna_sequence: DNA sequence waiting for saturation substitution in the specific location.
+    :type dna_sequence: str
 
     :param accessor: accessor.
     :type accessor: numpy.ndarray
 
-    :param index_queue: queue of vertex indices (transcoding path in the graph).
-    :type index_queue: list
+    :param previous_index: previous vertex index before the occurred error location.
+    :type previous_index: int
 
     :param occur_location: the location that may occurring substitution (or specific location).
     :type occur_location: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
-    :param has_insertion: consider insertion error.
-    :type has_insertion: bool
-
-    :param has_deletion: consider deletion error.
-    :type has_deletion: bool
+    :param has_indel: consider insertion and/or deletion error.
+    :type has_indel: bool
 
-    :param verbose: need to print log.
-    :type verbose: bool
+    :param nucleotides: usage of nucleotides.
+    :type nucleotides: str or None
 
-    :return: repaired DNA strings (may contain multiple repair results).
-    :rtype: list
+    :return: repaired DNA sequences (may contain multiple repair show) and visited count.
+    :rtype: list, int
 
     Example
         >>> from numpy import array
         >>> from dsw import path_matching
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
-        >>> dna_string = "TCTCTATCTCT"  # "TCTCTCTCTCT" is original DNA string
-        >>> path_matching(dna_string=dna_string, accessor=accessor, index_queue=[1, 7, 13, 7, 13, 7], \
-                          occur_location=4, has_insertion=True, has_deletion=True)
-        [('D', 4, 'T', 'TCTCATCTCT')]
+        >>> dna_sequence = "TCTCTATCTCT"  # "TCTCTCTCTCT" is original DNA sequence
+        >>> path_matching(dna_sequence=dna_sequence, accessor=accessor, previous_index=7, occur_location=5, \
+                          has_indel=True)
+        ([(('S', 5, 'C'), 'TCTCTCTCTCT'), (('S', 5, 'G'), 'TCTCTGTCTCT')], 12)
     """
     if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
-
-    repair_info, observed_length = [], int(log(len(accessor)) / log(len(nucleotides)))
-    original = dna_string[occur_location]
+        nucleotides = "ACGT"
 
-    if occur_location + observed_length < len(dna_string):
-        check_segment = dna_string[occur_location: occur_location + observed_length]
-    else:
-        check_segment = dna_string[occur_location:]
+    repair_info, visited_count = [], 0
+    original, used_indices = dna_sequence[occur_location], where(accessor[previous_index] >= 0)[0]
 
-    if verbose:
-        print("Original = [" + dna_string + "]")
-        if occur_location + observed_length < len(dna_string):
-            remain = len(dna_string) - (occur_location + observed_length)
-            print("Checking = [" + "-" * occur_location + check_segment + "-" * remain + "]")
-        else:
-            print("Checking = [" + "-" * occur_location + check_segment + "]")
-
-    # find substitution error.
-    used_indices = where(accessor[index_queue[occur_location]] >= 0)[0]
-    o_options = [nucleotides[used_index] for used_index in used_indices]
-    b_options = accessor[index_queue[occur_location]][~(accessor[index_queue[occur_location]] == -1)]
-    for replace_nucleotide in list(filter(lambda n: n != original, o_options)):
-        try:
-            segment = "".join([replace_nucleotide] + list(check_segment)[1:])
-
-            if verbose:
-                print("Replace " + original + " to " + replace_nucleotide)
-                if occur_location + observed_length < len(dna_string):
-                    remain = len(dna_string) - (occur_location + observed_length)
-                    print("         = [" + "-" * occur_location + segment + "-" * remain + "]"
-                          + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                else:
-                    print("         = [" + "-" * occur_location + segment + "]"
-                          + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-
-            vertex_index, reliable = index_queue[occur_location], True
+    for r_nucleotide in list(filter(lambda n: n != original, [nucleotides[index] for index in used_indices])):
+        vertex_index, reliable = accessor[previous_index][nucleotides.index(r_nucleotide)], True
+        for index, nucleotide in enumerate(dna_sequence[occur_location + 1:]):
+            used_nucleotides = [nucleotides[used_index] for used_index in where(accessor[vertex_index] >= 0)[0]]
+            if nucleotide in used_nucleotides:
+                vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+                visited_count += 1
+            else:
+                reliable = False
+                break
 
-            for index, nucleotide in enumerate(segment):
-                inner_used_indices = where(accessor[vertex_index] >= 0)[0]
-                used_nucleotides = [nucleotides[used_index] for used_index in inner_used_indices]
+        if reliable:  # "S" refers to repair by substation.
+            obtained_dna_sequence = list(dna_sequence)
+            obtained_dna_sequence[occur_location] = r_nucleotide
+            repair_info.append((("S", occur_location, r_nucleotide), "".join(obtained_dna_sequence)))
+
+    if has_indel:
+        for a_nucleotide in [nucleotides[used_index] for used_index in used_indices]:
+            vertex_index, reliable = accessor[previous_index][nucleotides.index(a_nucleotide)], True
+            for nucleotide in dna_sequence[occur_location:]:
+                used_nucleotides = [nucleotides[used_index] for used_index in where(accessor[vertex_index] >= 0)[0]]
                 if nucleotide in used_nucleotides:
-                    if verbose:
-                        show_used_indices = where(accessor[vertex_index] >= 0)[0]
-                        o_options = [nucleotides[used_index] for used_index in show_used_indices]
-                        b_options = accessor[vertex_index][~(accessor[vertex_index] == -1)]
-                        if occur_location + observed_length < len(dna_string):
-                            remain = len(dna_string) - (occur_location + observed_length)
-                            print("           [" + "-" * (occur_location + index) + segment[index]
-                                  + "-" * (remain + len(segment) - index - 1) + "]"
-                                  + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                        else:
-                            print("           [" + "-" * (occur_location + index) + segment[index] + "]"
-                                  + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-
                     vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+                    visited_count += 1
                 else:
                     reliable = False
                     break
-        except IndexError:
-            reliable = False
 
-        if reliable:
-            if verbose:
-                print("Reliable: True")
-            obtained_dna_string = list(dna_string)
-            obtained_dna_string[occur_location] = replace_nucleotide
-            obtained_dna_string = "".join(obtained_dna_string)
-            # "S" refers to repair by substation.
-            repair_info.append(("S", occur_location, replace_nucleotide, obtained_dna_string))
-
-    if has_insertion:  # find insertion error if required.
-        used_indices = where(accessor[index_queue[occur_location]] >= 0)[0]
-        o_options = [nucleotides[used_index] for used_index in used_indices]
-        b_options = accessor[index_queue[occur_location]][~(accessor[index_queue[occur_location]] == -1)]
-        for add_nucleotide in o_options:
-            try:
-                segment = "".join([add_nucleotide] + list(check_segment))
-                if verbose:
-                    print("Insert " + add_nucleotide + " in location " + str(occur_location))
-                    if occur_location + observed_length < len(dna_string):
-                        remain = len(dna_string) - (occur_location + observed_length)
-                        print("         = [" + "-" * occur_location + segment + "-" * remain + "]"
-                              + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                    else:
-                        print("         = [" + "-" * occur_location + segment + "]"
-                              + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
+            if reliable:  # "I" refers to repair by insertion.
+                obtained_dna_sequence = list(dna_sequence)
+                obtained_dna_sequence.insert(occur_location, a_nucleotide)
+                repair_info.append((("I", occur_location, a_nucleotide), "".join(obtained_dna_sequence)))
+
+        d_nucleotide, vertex_index, reliable = original, previous_index, True
+        for index, nucleotide in enumerate(dna_sequence[occur_location + 1:]):
+            used_nucleotides = [nucleotides[used_index] for used_index in where(accessor[vertex_index] >= 0)[0]]
+            if nucleotide in used_nucleotides:
+                vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+                visited_count += 1
+            else:
+                reliable = False
+                break
 
-                vertex_index, reliable = index_queue[occur_location], True
-                for index, nucleotide in enumerate(segment):
-                    inner_used_indices = where(accessor[vertex_index] >= 0)[0]
-                    used_nucleotides = [nucleotides[used_index] for used_index in inner_used_indices]
-                    if nucleotide in used_nucleotides:
-                        if verbose:
-                            show_used_indices = where(accessor[vertex_index] >= 0)[0]
-                            o_options = [nucleotides[used_index] for used_index in show_used_indices]
-                            b_options = accessor[vertex_index][~(accessor[vertex_index] == -1)]
-                            if occur_location + observed_length < len(dna_string):
-                                remain = len(dna_string) - (occur_location + observed_length)
-                                print("           [" + "-" * (occur_location + index) + segment[index]
-                                      + "-" * (remain + len(segment) - index - 1) + "]"
-                                      + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                            else:
-                                print("           [" + "-" * (occur_location + index) + segment[index] + "]"
-                                      + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
+        if reliable:   # "D" refers to repair by deletion.
+            obtained_dna_sequence = list(dna_sequence)
+            del obtained_dna_sequence[occur_location]
+            repair_info.append((("D", occur_location, d_nucleotide), "".join(obtained_dna_sequence)))
 
-                        vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
-                    else:
-                        reliable = False
-                        break
-            except IndexError:
-                reliable = False
+    return repair_info, visited_count
 
-            if reliable:
-                if verbose:
-                    print("Reliable: True")
-                obtained_dna_string = list(dna_string)
-                obtained_dna_string.insert(occur_location, add_nucleotide)
-                obtained_dna_string = "".join(obtained_dna_string)
-                # "I" refers to repair by insertion.
-                repair_info.append(("I", occur_location, add_nucleotide, obtained_dna_string))
-
-    if has_deletion:  # find deletion error if required.
-        delete_nucleotide = None
-        try:
-            used_indices = where(accessor[index_queue[occur_location]] >= 0)[0]
-            o_options = [nucleotides[used_index] for used_index in used_indices]
-            b_options = accessor[index_queue[occur_location]][~(accessor[index_queue[occur_location]] == -1)]
 
-            delete_nucleotide = check_segment[0]
-            segment = "".join(list(check_segment)[1:])
-            if verbose:
-                print("Delete " + check_segment[0] + " in location " + str(occur_location))
-                if occur_location + observed_length < len(dna_string):
-                    remain = len(dna_string) - (occur_location + observed_length)
-                    print("         = [" + "-" * occur_location + segment + "-" * remain + "]"
-                          + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                else:
-                    print("         = [" + "-" * occur_location + segment + "]"
-                          + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
+def calculate_intersection_score(latter_map, observed_length=10, has_insertion=True, has_deletion=True, verbose=False):
+    """
+    Calculate the intersection score based on the breach-first search.
 
-            vertex_index, reliable = index_queue[occur_location], True
-            for index, nucleotide in enumerate(segment):
-                inner_used_indices = where(accessor[vertex_index] >= 0)[0]
-                used_nucleotides = [nucleotides[used_index] for used_index in inner_used_indices]
-                if nucleotide in used_nucleotides:
-                    if verbose:
-                        show_used_indices = where(accessor[vertex_index] >= 0)[0]
-                        o_options = [nucleotides[used_index] for used_index in show_used_indices]
-                        b_options = accessor[vertex_index][~(accessor[vertex_index] == -1)]
-                        if occur_location + observed_length < len(dna_string):
-                            remain = len(dna_string) - (occur_location + observed_length)
-                            print("           [" + "-" * (occur_location + index) + segment[index]
-                                  + "-" * (remain + len(segment) - index - 1) + "]"
-                                  + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                        else:
-                            print("           [" + "-" * (occur_location + index) + segment[index] + "]"
-                                  + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
+    :param latter_map: latter vertex map of graph.
+    :type latter_map: dict
 
-                    vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
-                else:
-                    reliable = False
-                    break
-        except IndexError:
-            reliable = False
+    :param observed_length: length of the DNA sequence in a vertex.
+    :type observed_length: int
 
-        if reliable:
-            if verbose:
-                print("Reliable: True")
-            obtained_dna_string = list(dna_string)
-            del obtained_dna_string[occur_location]
-            obtained_dna_string = "".join(obtained_dna_string)
-            # "D" refers to repair by deletion.
-            repair_info.append(("D", occur_location, delete_nucleotide, obtained_dna_string))
+    :param has_insertion: consider to repair insertion errors.
+    :type has_insertion: bool
+
+    :param has_deletion: consider to repair deletion errors.
+    :type has_deletion: bool
+
+    :param verbose: need to print log.
+    :type verbose: bool
+
+    :return: intersection scores for each arc in the coding graph (consistent with the shape of accessor).
+    :rtype: numpy.ndarray
+
+    Example
+        >>> from dsw import calculate_intersection_score
+        >>> # latter_map with GC-balanced
+        >>> latter_map = {1: [4, 7], 2: [8, 11], 4: [1, 2], 7: [13, 14], \
+                          8: [1, 2], 11: [13, 14], 13: [4, 7], 14: [8, 11]}
+        >>> calculate_intersection_score(latter_map, observed_length=10, \
+                                         has_insertion=True, has_deletion=True, verbose=False)
+        array([[ 0,  0,  0,  0],
+               [28,  0,  0, 28],
+               [28,  0,  0, 28],
+               ...,
+               [ 0,  0,  0,  0],
+               [ 0,  0,  0,  0],
+               [ 0,  0,  0,  0]])
+
+    .. note::
+        It is a gift for the follow-up investigation.
+        That is, removing arc to improve the capability of the probabilistic error correction.
+    """
+    nucleotides = "ACGT"
+
+    currents, depth, monitor = list(latter_map.keys()), observed_length - 1, Monitor()
+    scores = zeros(shape=(len(nucleotides) ** observed_length, len(nucleotides)), dtype=int)
+    for current, current_index in enumerate(currents):
+        mutate_branches = []  # substitution
+        for latter_index in latter_map[current_index]:
+            mutate_branches.append(obtain_leaf_vertices(latter_index, depth, latter_map=latter_map))
+        for one, two in combinations(range(len(mutate_branches)), 2):
+            score = len(union1d(mutate_branches[one], mutate_branches[two]))
+            scores[current_index, latter_map[current_index][one] % len(nucleotides)] += score
+            scores[current_index, latter_map[current_index][two] % len(nucleotides)] += score
+
+        if has_insertion:
+            for index, former_index in enumerate(latter_map[current_index]):  # insertion
+                if former_index in latter_map:
+                    for latter_index in latter_map[former_index]:
+                        insert_branch = obtain_leaf_vertices(latter_index, depth, latter_map=latter_map)
+                        score = len(union1d(mutate_branches[index], insert_branch))
+                        scores[current_index, latter_map[current_index][index] % len(nucleotides)] += score
+
+        if has_deletion:
+            delete_branch = [obtain_leaf_vertices(current_index, depth, latter_map=latter_map)]  # deletion
+            for index in range(len(mutate_branches)):
+                score = len(union1d(mutate_branches[index], delete_branch))
+                scores[current_index, latter_map[current_index][index] % len(nucleotides)] += score
+            del delete_branch
+
+        if verbose:
+            monitor(current + 1, len(currents))
 
-    return repair_info
+    return scores
```

## dsw/operation.py

```diff
@@ -6,24 +6,24 @@
     def __init__(self):
         """
         Initialize the monitor to identify the task progress.
 
         Example
             >>> from dsw import Monitor
             >>> monitor = Monitor()
-            >>> monitor.output(current_state=1, total_state=10)
+            >>> monitor(current_state=1, total_state=10)
             \r|███                 | 10% ( 1/10) wait 0000:00:00.
-            >>> monitor.output(current_state=5, total_state=10)
+            >>> monitor(current_state=5, total_state=10)
             \r|███████████         | 50% ( 5/10) wait 0000:00:00.
-            >>> monitor.output(current_state=10, total_state=10)
+            >>> monitor(current_state=10, total_state=10)
             \r|████████████████████|100% (10/10) used 0000:00:00.
         """
         self.last_time = None
 
-    def output(self, current_state, total_state, extra=None):
+    def __call__(self, current_state, total_state, extra=None):
         """
         Output the current state of process.
 
         :param current_state: current state of process.
         :type current_state: int
 
         :param total_state: total state of process.
@@ -258,47 +258,56 @@
     for index in range(len(quotient)):
         if quotient[index] != "0":
             return quotient[index:], str(remainder)
 
     return "0", str(remainder)
 
 
-def bit_to_number(bit_array, is_string=True):
+def bit_to_number(bit_array, is_string=True, verbose=False):
     """
     Transform a bit array to the equivalent decimal number.
 
     :param bit_array: bit array.
     :type bit_array: list
 
     :param is_string: type of equivalent decimal number is str.
     :type: is_string: bool
 
     :return: equivalent decimal number (may huge) of the inputted bit array.
     :rtype: str or int
 
+    :param verbose: need to print log.
+    :type verbose: bool
+
     Example
         >>> from dsw import bit_to_number
         >>> bit_to_number(bit_array=[1, 1, 1, 1, 1, 0, 0, 1, 1, 1], is_string=True)
         '999'
         >>> bit_to_number(bit_array=[1, 1, 1, 1, 1, 0, 0, 1, 1, 1], is_string=False)
         999
     """
+    monitor = Monitor()
     if is_string:
         decimal_number = "0"
 
-        for a_bit in bit_array:
+        for index, a_bit in enumerate(bit_array):
             # multiply by 2
             decimal_number = calculus_multiplication(number=decimal_number, base="2")
             # add current bit
             decimal_number = calculus_addition(number=decimal_number, base=str(a_bit))
+
+            if verbose:
+                monitor(index + 1, len(bit_array))
     else:
         decimal_number = 0
 
-        for a_bit in bit_array:
+        for index, a_bit in enumerate(bit_array):
             decimal_number = decimal_number * 2 + a_bit
+            if verbose:
+                monitor(index + 1, len(bit_array))
 
     return decimal_number
 
 
 def number_to_bit(decimal_number, bit_length):
     """
     Transform a decimal number to the equivalent bit array with specific length.
@@ -327,44 +336,45 @@
     elif type(decimal_number) == int:
         while decimal_number > 0:
             decimal_number, remainder = divmod(decimal_number, 2)
             one_array.insert(0, remainder)
     else:
         raise ValueError("No such type of decimal number (" + str(type(decimal_number)) + ")!")
 
-    return [0] * (bit_length - len(one_array)) + one_array
+    if len(one_array) == bit_length:
+        return one_array
+    elif len(one_array) < bit_length:
+        return [0] * (bit_length - len(one_array)) + one_array
+    else:
+        return one_array[:bit_length]
 
 
-def dna_to_number(dna_string, nucleotides=None, is_string=True):
+def dna_to_number(dna_sequence, is_string=True):
     """
     Transform a DNA string to the equivalent decimal number.
 
-    :param dna_string: required DNA string.
-    :type dna_string: str
-
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
+    :param dna_sequence: required DNA string.
+    :type dna_sequence: str
 
     :param is_string: type of equivalent decimal number is str.
     :type: is_string: bool
 
     :return: equivalent decimal number (may huge) of the inputted DNA string.
     :rtype: str or int
 
     Example
         >>> from dsw import dna_to_number
-        >>> dna_to_number(dna_string="ACGTACGT", is_string=True)
+        >>> dna_to_number(dna_sequence="ACGTACGT", is_string=True)
         '6939'
-        >>> dna_to_number(dna_string="ACGTACGT", is_string=False)
+        >>> dna_to_number(dna_sequence="ACGTACGT", is_string=False)
         6939
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
-    nucleotide_values = list(map(nucleotides.index, dna_string))
+    nucleotide_values = list(map(nucleotides.index, dna_sequence))
 
     if is_string:
         decimal_number = "0"
         for nucleotide_value in nucleotide_values:
             # multiply by length of usage of nucleotides.
             decimal_number = calculus_multiplication(number=decimal_number, base=str(len(nucleotides)))
             # add current nucleotide value.
@@ -373,39 +383,35 @@
         decimal_number = 0
         for nucleotide_value in nucleotide_values:
             decimal_number = decimal_number * 4 + nucleotide_value
 
     return decimal_number
 
 
-def number_to_dna(decimal_number, dna_length, nucleotides=None):
+def number_to_dna(decimal_number, dna_length):
     """
     Transform a decimal number to the equivalent DNA string with specific length.
 
     :param decimal_number: decimal number (may huge) of the DNA string.
     :type decimal_number: str or int
 
     :param dna_length: default length of the DNA string.
     :type dna_length: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
     :return: equivalent DNA string of the decimal number.
     :rtype: str
 
     Example
         >>> from dsw import number_to_dna
         >>> number_to_dna(decimal_number=6939, dna_length=8)
         'ACGTACGT'
         >>> number_to_dna(decimal_number="6939", dna_length=8)
         'ACGTACGT'
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     one_array = []
 
     if type(decimal_number) == str:
         while decimal_number != "0":  # decimal number > 0
             decimal_number, remainder = calculus_division(number=decimal_number, base=str(len(nucleotides)))
             one_array.insert(0, nucleotides[int(remainder)])
```

## dsw/spiderweb.py

```diff
@@ -1,487 +1,463 @@
-from copy import deepcopy
-from numpy import zeros, ones, array, random, sum, argsort, where
+from collections import Counter
+from itertools import product
+from networkx import DiGraph, find_cycle
+from numpy import zeros, ones, array, random, log, sum, max, argmax, argsort, unique, intersect1d, where
 
 from dsw.operation import Monitor, calculus_addition, calculus_multiplication, calculus_division
-from dsw.operation import bit_to_number, number_to_bit, number_to_dna
-from dsw.graphized import obtain_latters, path_matching
+from dsw.operation import bit_to_number, number_to_bit, number_to_dna, dna_to_number
+from dsw.graphized import obtain_vertices, obtain_formers, obtain_latters, path_matching, calculate_intersection_score
 
 
-def encode(binary_message, accessor, start_index, nucleotides=None,
-           vt_length=0, shuffles=None, verbose=False):
+def encode(binary_message, accessor, start_index,
+           is_faster=False, vt_length=0, shuffles=None, need_path=False, verbose=False):
     """
     Encode a bit array by the specific accessor.
 
     :param binary_message: binary message.
     :type binary_message: numpy.ndarray
 
     :param accessor: accessor of the coding algorithm.
     :type accessor: numpy.ndarray
 
     :param start_index: virtual vertex to start encoding.
     :type start_index: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list or None
+    :param is_faster: encode in a faster way.
+    :type is_faster: bool
 
     :param vt_length: length of Varshamov-Tenengolts code for error-correction.
     :type vt_length: int or None
 
     :param shuffles: shuffle relationships for bit-nucleotide mapping.
     :type: numpy.ndarray
 
+    :param need_path: need to record the restricted state transition path.
+    :type need_path: bool
+
     :param verbose: need to print log.
     :type verbose: bool
 
-    :return: DNA string encoded by this graph (and VT check string if required).
+    :return: DNA sequence encoded by this graph (and VT check sequence if required).
     :rtype: str or (str, str)
 
+    .. note::
+        If the parameter "is_faster" is set as True, the out-degree of coding digraph cannot contains 3.
+
+
     Example
         >>> from numpy import array
         >>> from dsw import encode
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
         >>> binary_message = array([0, 1, 0, 1, 0, 1, 0, 1])
         >>> encode(accessor=accessor, binary_message=binary_message, start_index=1)
         'TCTCTCT'
         >>> encode(accessor=accessor, binary_message=binary_message, start_index=1, vt_length=5)
-        ('TCTCTCT', 'TAATA')
+        ('TCTCTCT', 'TAAGC')
         >>> shuffles = array([[3, 2, 1, 0], [2, 3, 1, 0], [3, 1, 0, 2], [0, 3, 1, 2], \
                               [3, 2, 0, 1], [1, 0, 3, 2], [0, 3, 1, 2], [2, 0, 1, 3], \
                               [2, 3, 0, 1], [1, 0, 3, 2], [2, 0, 1, 3], [0, 1, 3, 2], \
                               [2, 3, 1, 0], [2, 0, 3, 1], [0, 1, 3, 2], [0, 3, 2, 1]])
         >>> encode(accessor=accessor, binary_message=binary_message, shuffles=shuffles, start_index=1)
         'AGAGAGA'
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    monitor, record_path, vertex_index, dna_sequence, nucleotides = Monitor(), [], start_index, "", "ACGT"
 
-    quotient, dna_string, vertex_index, monitor = bit_to_number(binary_message), "", start_index, Monitor()
-    total_state = len(quotient)  # number of symbol.
+    if not is_faster:
+        quotient = bit_to_number(binary_message, verbose=verbose)
+        total_state = len(quotient)  # number of symbol.
 
-    while quotient != "0":
-        used_indices = where(accessor[vertex_index] >= 0)[0]
+        while quotient != "0":
+            used_indices = where(accessor[vertex_index] >= 0)[0]
 
-        if len(used_indices) > 1:  # current vertex contains information.
-            quotient, remainder = calculus_division(number=quotient, base=str(len(used_indices)))
-            remainder = int(remainder)
+            if len(used_indices) > 1:  # current vertex contains information.
+                quotient, remainder = calculus_division(number=quotient, base=str(len(used_indices)))
+                remainder = int(remainder)
 
-            if shuffles is not None:  # shuffle remainder based on the inputted shuffles.
-                remainder = argsort(shuffles[vertex_index, used_indices])[remainder]
+                if shuffles is not None:  # shuffle remainder based on the inputted shuffles.
+                    remainder = argsort(shuffles[vertex_index, used_indices])[remainder]
 
-            value = used_indices[remainder]
+                value = used_indices[remainder]
 
-        elif len(used_indices) == 1:  # current vertex does not contain information.
-            value = used_indices[0]
+                if need_path:
+                    record_path.append([vertex_index, 1])
 
-        else:  # current vertex is wrong.
-            raise ValueError("Current vertex doesn't have an out-degree, the accessor or the start vertex is wrong!")
+            elif len(used_indices) == 1:  # current vertex does not contain information.
+                value = used_indices[0]
 
-        nucleotide, vertex_index = nucleotides[value], accessor[vertex_index][value]
+                if need_path:
+                    record_path.append([vertex_index, 0])
 
-        dna_string += nucleotide
+            else:  # current vertex is wrong.
+                raise ValueError("Current vertex doesn't have an out-degree, "
+                                 + "the accessor or the start vertex is wrong!")
 
-        if verbose:
-            if quotient != "0":
-                monitor.output(total_state - len(quotient), total_state)
-            else:
-                monitor.output(total_state, total_state)
+            nucleotide, vertex_index = nucleotides[value], accessor[vertex_index][value]
+
+            dna_sequence += nucleotide
+
+            if verbose:
+                if quotient != "0":
+                    monitor(total_state - len(quotient), total_state)
+                else:
+                    monitor(total_state, total_state)
+
+    else:
+        location = 0
+        while location < len(binary_message):
+            used_indices = where(accessor[vertex_index] >= 0)[0]
+            radix = len(used_indices)
+
+            if radix == 4:  # current vertex contains information.
+                remainder = binary_message[location] * 2 + binary_message[location + 1]
+
+                if shuffles is not None:  # shuffle remainder based on the inputted shuffles.
+                    remainder = argsort(shuffles[vertex_index, used_indices])[remainder]
+
+                value = used_indices[remainder]
+                location += 2
+            elif radix == 2:
+                remainder = binary_message[location]
+
+                if shuffles is not None:  # shuffle remainder based on the inputted shuffles.
+                    remainder = argsort(shuffles[vertex_index, used_indices])[remainder]
+
+                value = used_indices[remainder]
+                location += 1
+            elif radix == 1:  # current vertex does not contain information.
+                value = used_indices[0]
+            elif radix == 3:
+                raise ValueError("Not implementation!")
+            else:  # current vertex is wrong.
+                raise ValueError("Current vertex doesn't have an out-degree, "
+                                 + "the accessor or the start vertex is wrong!")
+
+            nucleotide, vertex_index = nucleotides[value], accessor[vertex_index][value]
+            dna_sequence += nucleotides[value]
+
+            if need_path:
+                record_path.append([vertex_index, int(radix > 1)])
+
+            if verbose:
+                monitor(location + 1, len(binary_message))
+
+    if need_path:
+        record_path = array(record_path)
 
     if vt_length > 0:
-        vt_check = set_vt(dna_string=dna_string, vt_length=vt_length, nucleotides=nucleotides)
-        return dna_string, vt_check
+        vt_check = set_vt(dna_sequence=dna_sequence, vt_length=vt_length)
+        if need_path:
+            return dna_sequence, set_vt(dna_sequence=dna_sequence, vt_length=vt_length), record_path
+        else:
+            return dna_sequence, vt_check
     else:
-        return dna_string
+        if need_path:
+            return dna_sequence, record_path
+        else:
+            return dna_sequence
 
 
-def decode(dna_string, bit_length, accessor, start_index, nucleotides=None,
-           vt_check=None, shuffles=None, verbose=False):
+def decode(dna_sequence, bit_length, accessor, start_index,
+           is_faster=False, vt_check=None, shuffles=None, verbose=False):
     """
-    Decode a DNA string by the specific accessor.
+    Decode a DNA sequence by the specific accessor.
 
-    :param dna_string: DNA string encoded by this graph.
-    :type dna_string: str
+    :param dna_sequence: DNA sequence encoded by this graph.
+    :type dna_sequence: str
 
     :param bit_length: length of the bit array.
     :type bit_length: int
 
     :param accessor: accessor of the coding algorithm (consistent with the encoding process).
     :type accessor: numpy.ndarray
 
     :param start_index: virtual vertex to start decoding (consistent with the encoding process).
     :type start_index: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list or None
+    :param is_faster: encode in a faster way.
+    :type is_faster: bool
 
-    :param vt_check: check string of Varshamov-Tenengolts code.
+    :param vt_check: check sequence of Varshamov-Tenengolts code.
     :type vt_check: str or None
 
     :param shuffles: shuffle relationships for bit-nucleotide mapping.
     :type shuffles: numpy.ndarray
 
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: binary message decoded by this graph.
     :rtype: numpy.ndarray
 
     :raise ValueError: if one or more errors are found.
 
+    .. note::
+        If the parameter "is_faster" is set as True, the out-degree of coding digraph cannot contains 3.
+
     Example
         >>> from numpy import array
         >>> from dsw import decode
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
-        >>> dna_string = "TCTCTCT"
-        >>> decode(accessor=accessor, dna_string=dna_string, start_index=1, bit_length=8)
+        >>> dna_sequence = "TCTCTCT"
+        >>> decode(accessor=accessor, dna_sequence=dna_sequence, start_index=1, bit_length=8)
         array([0, 1, 0, 1, 0, 1, 0, 1])
-        >>> vt_check = "TAATA"
-        >>> decode(accessor=accessor, dna_string=dna_string, start_index=1, vt_check=vt_check, bit_length=8)
+        >>> vt_check = "TAAGC"
+        >>> decode(accessor=accessor, dna_sequence=dna_sequence, start_index=1, vt_check=vt_check, bit_length=8)
         array([0, 1, 0, 1, 0, 1, 0, 1])
         >>> shuffles = array([[3, 2, 1, 0], [2, 3, 1, 0], [3, 1, 0, 2], [0, 3, 1, 2], \
                               [3, 2, 0, 1], [1, 0, 3, 2], [0, 3, 1, 2], [2, 0, 1, 3], \
                               [2, 3, 0, 1], [1, 0, 3, 2], [2, 0, 1, 3], [0, 1, 3, 2], \
                               [2, 3, 1, 0], [2, 0, 3, 1], [0, 1, 3, 2], [0, 3, 2, 1]])
-        >>> decode(accessor=accessor, dna_string="TCTCTCT", start_index=1, shuffles=shuffles, bit_length=8)
+        >>> decode(accessor=accessor, dna_sequence="TCTCTCT", start_index=1, shuffles=shuffles, bit_length=8)
         array([0, 0, 0, 0, 0, 0, 0, 0])
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    vertex_index, nucleotides, monitor = start_index, "ACGT", Monitor()
+
+    if vt_check is not None:
+        if vt_check != set_vt(dna_sequence=dna_sequence, vt_length=len(vt_check)):
+            raise ValueError("At least one error is found in this DNA sequence!")
 
-    quotient, saved_values, vertex_index, monitor = "0", [], start_index, Monitor()
+    if not is_faster:
+        quotient, saved_values = "0", []
 
-    for location, nucleotide in enumerate(dna_string):
-        used_indices = where(accessor[vertex_index] >= 0)[0]
+        for location, nucleotide in enumerate(dna_sequence):
+            used_indices = where(accessor[vertex_index] >= 0)[0]
 
-        if len(used_indices) > 1:  # current vertex contains information.
-            used_nucleotides = [nucleotides[used_index] for used_index in used_indices]
+            if len(used_indices) > 1:  # current vertex contains information.
+                used_nucleotides = [nucleotides[used_index] for used_index in used_indices]
+
+                if nucleotide in used_nucleotides:  # check whether the DNA sequence is right currently.
+                    remainder = used_nucleotides.index(nucleotide)
+                else:
+                    raise ValueError("At least one error is found in this DNA sequence!")
+
+                if shuffles is not None:  # shuffle remainder based on the inputted shuffles.
+                    remainder = where(argsort(shuffles[vertex_index, used_indices]) == remainder)[0][0]
+
+                saved_values.append((len(used_indices), remainder))
+                vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+
+            elif len(used_indices) == 1:  # current vertex does not contain information.
+                used_nucleotide = nucleotides[used_indices[0]]
+                if nucleotide == used_nucleotide:
+                    vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+                else:
+                    raise ValueError("At least one error is found in this DNA sequence!")
 
-            if nucleotide in used_nucleotides:  # check whether the DNA string is right currently.
+            else:  # current vertex is wrong.
+                raise ValueError("Current vertex doesn't have an out-degree, "
+                                 + "the accessor, the start vertex, or DNA sequence is wrong!")
+
+            if verbose:
+                monitor(location + 1, len(dna_sequence))
+
+        for location, (out_degree, number) in enumerate(saved_values[::-1]):
+            quotient = calculus_multiplication(number=quotient, base=str(out_degree))
+            quotient = calculus_addition(number=quotient, base=str(number))
+
+        binary_message = array(number_to_bit(decimal_number=quotient, bit_length=bit_length), dtype=int)
+
+    else:
+        message_location, binary_message = 0, zeros(shape=(bit_length,), dtype=int)
+
+        for location, nucleotide in enumerate(dna_sequence):
+            used_indices = where(accessor[vertex_index] >= 0)[0]
+            radix = len(used_indices)
+
+            used_nucleotides = [nucleotides[used_index] for used_index in used_indices]
+            if nucleotide in used_nucleotides:  # check whether the DNA sequence is right currently.
                 remainder = used_nucleotides.index(nucleotide)
             else:
-                raise ValueError("At least one error is found in this DNA string!")
+                raise ValueError("At least one error is found in this DNA sequence!")
 
             if shuffles is not None:  # shuffle remainder based on the inputted shuffles.
                 remainder = where(argsort(shuffles[vertex_index, used_indices]) == remainder)[0][0]
 
-            saved_values.append((len(used_indices), remainder))
             vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
 
-        elif len(used_indices) == 1:  # current vertex does not contain information.
-            used_nucleotide = nucleotides[used_indices[0]]
-            if nucleotide == used_nucleotide:
-                vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+            if radix == 4:
+                binary_message[message_location] = remainder // 2
+                binary_message[message_location + 1] = remainder % 2
+                message_location += 2
+            elif radix == 2:
+                binary_message[message_location] = remainder % 2
+                message_location += 1
+            elif radix == 1:
+                pass  # do nothing.
+            elif radix == 3:
+                raise ValueError("Not implementation!")
             else:
-                raise ValueError("At least one error is found in this DNA string!")
-
-        else:  # current vertex is wrong.
-            raise ValueError("Current vertex doesn't have an out-degree, "
-                             + "the accessor, the start vertex, or DNA string is wrong!")
-
-        if verbose:
-            monitor.output(location + 1, len(dna_string))
+                raise ValueError("Current vertex doesn't have an out-degree, "
+                                 + "the accessor, the start vertex, or DNA sequence is wrong!")
 
-    if vt_check is not None:
-        if vt_check != set_vt(dna_string=dna_string, vt_length=len(vt_check), nucleotides=nucleotides):
-            raise ValueError("At least one error is found in this DNA string!")
-
-    for location, (out_degree, number) in enumerate(saved_values[::-1]):
-        quotient = calculus_multiplication(number=quotient, base=str(out_degree))
-        quotient = calculus_addition(number=quotient, base=str(number))
+    return binary_message
 
-    return array(number_to_bit(decimal_number=quotient, bit_length=bit_length), dtype=int)
 
-
-def set_vt(dna_string, vt_length, nucleotides=None):
+def set_vt(dna_sequence, vt_length):
     """
-    Set Varshamov-Tenengolts-based path check string ('salt-protected') from DNA (payload) string.
+    Set Varshamov-Tenengolts-based path check string ('salt-protected') from DNA (payload) sequence.
 
-    :param dna_string: DNA string encoded through SPIDER-WEB.
-    :type dna_string: str
+    :param dna_sequence: DNA sequence encoded through SPIDER-WEB.
+    :type dna_sequence: str
 
-    :param vt_length: length of DNA string (path check).
+    :param vt_length: length of DNA sequence (path check).
     :type vt_length: int or None
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list or None
-
-    :return: path check DNA string with required length.
+    :return: path check DNA sequence with required length.
 
     Example
         >>> from dsw import set_vt
-        >>> dna_string = "TCTCTCT"
+        >>> dna_sequence = "TCTCTCT"
         >>> vt_length = 5
-        >>> set_vt(dna_string=dna_string, vt_length=vt_length)
-        'TAATA'
+        >>> set_vt(dna_sequence=dna_sequence, vt_length=vt_length)
+        'TAAGC'
 
     .. note::
         Reference [1] Rom R. Varshamov and Grigory M. Tenengolts (1965) Avtomat. i Telemekh
 
         Reference [2] Grigory Tenengolts (1984) IEEE Transactions on Information Theory
 
         Reference [3] William H. Press et al. (2020) Proceedings of the National Academy of Sciences
 
         Reference [4] A. Xavier Kohll et al. (2020) Chemical Communications
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
-    vt_flag, vt_value = 0, 0
-    for location, nucleotide in enumerate(dna_string):
-        value = nucleotides.index(nucleotide)
-        if location > 0 and value >= nucleotides.index(dna_string[location - 1]):
-            vt_value += location
-        vt_flag += value
-    vt_value %= 4 ** (vt_length - 1)
-    vt_flag %= 4
+    values = array([nucleotides.index(nucleotide) for nucleotide in dna_sequence])
+    vt_value = sum(where((values[1:] - values[:-1]) > 0)[0]) % (len(nucleotides) ** (vt_length - 1))
+    vt_flag = sum(values) % len(nucleotides)
 
-    former = nucleotides[vt_flag % len(nucleotides)]
-    latter = number_to_dna(decimal_number=vt_value % len(nucleotides) ** (vt_length - 1), dna_length=vt_length - 1)
+    return nucleotides[vt_flag] + number_to_dna(decimal_number=int(vt_value), dna_length=vt_length - 1)
 
-    return former + latter
 
-
-def repair_dna(dna_string, accessor, start_index, observed_length, check_iterations=1, heap_size=1e6, vt_check=None,
-               has_insertion=False, has_deletion=False, nucleotides=None, verbose=False):
+def repair_dna(dna_sequence, accessor, start_index, observed_length, vt_check=None, has_indel=False, heap_size=1e3):
     """
-    Repair the DNA string containing one (or more) errors.
+    Repair the DNA sequence containing one (or more) errors.
 
-    :param dna_string: DNA string waiting for recovery.
-    :type dna_string: str
+    :param dna_sequence: DNA sequence waiting for recovery.
+    :type dna_sequence: str
 
     :param accessor: accessor of the coding algorithm.
     :type accessor: numpy.ndarray
 
     :param start_index: virtual vertex to start encoding.
     :type start_index: int
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
-    :param check_iterations: repair check iterations, which greater than or equal to the estimated number of errors.
-    :type check_iterations: int
-
-    :param heap_size: available set size of repaired DNA strings.
-    :type heap_size: int or None
-
-    :param vt_check: check string of Varshamov-Tenengolts code.
+    :param vt_check: check sequence of Varshamov-Tenengolts code.
     :type vt_check: str or None
 
-    :param has_insertion: consider insertion error.
-    :type has_insertion: bool
-
-    :param has_deletion: consider deletion error.
-    :type has_deletion: bool
-
-    :param verbose: need to print log.
-    :type verbose: bool
+    :param has_indel: consider insertion and/or deletion error.
+    :type has_indel: bool
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
+    :param heap_size: maximum heap size.
+    :type heap_size: int
 
-    :return: repaired DNA string set and additional information (includes detect flags and initial repaired strings).
+    :return: repaired DNA sequence set and additional information.
     :rtype: (list, (bool, bool, int))
 
     Example
         >>> from numpy import array
         >>> from dsw import repair_dna
         >>> # accessor with GC-balanced
         >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
                               [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
-        >>> dna_string = "TCTCTATCTCTC"  # "TCTCTCTCTCTC" is original DNA string
-        >>> repair_dna(dna_string=dna_string, accessor=accessor, start_index=1, observed_length=2, \
-                       check_iterations=1, has_insertion=True, has_deletion=True, verbose=False)
-        (['TCTCTCTCTCTC', 'TCTCTGTCTCTC'], (True, False, 2))
-        >>> vt_check = "AACTG"  # check list of Varshamov-Tenengolts code.
-        >>> repair_dna(dna_string=dna_string, accessor=accessor, start_index=1, observed_length=2, \
-                       check_iterations=1, vt_check=vt_check, has_insertion=True, has_deletion=True, verbose=False)
-        (['TCTCTCTCTCTC'], (True, True, 2))
-    """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
-
-    original_dna_string = deepcopy(dna_string)
-    dna_strings, repaired_dna_strings, detected_flag_1, detected_flag_2 = [dna_string], [], False, False
-    for _ in range(check_iterations + 1):
-        new_dna_strings = []
-        for detected_dna_string in dna_strings:
-            found_wrong, vertex_index, index_queue = False, start_index, [start_index]
-            for location, nucleotide in enumerate(detected_dna_string):
-                used_indices = where(accessor[vertex_index] >= 0)[0]
-                if nucleotide in [nucleotides[used_index] for used_index in used_indices]:
-                    vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
-                    index_queue.append(vertex_index)
-                else:
-                    if verbose:
-                        used_indices = where(accessor[index_queue[-1]] >= 0)[0]
-                        o_options = [nucleotides[used_index] for used_index in used_indices]
-                        b_options = [accessor[index_queue[-1]][used_index] for used_index in used_indices]
-                        print("error occur in location " + str(location) + ", found " + detected_dna_string[location]
-                              + " | " + str(o_options).replace("\'", "") + ", " + str(b_options))
-                        print("-" * 50)
-                        print("Search error in current location.")
-                        print("Check location = " + detected_dna_string[location] + " | " + str(location) + ", found "
-                              + detected_dna_string[location] + " | "
-                              + str(o_options).replace("\'", "") + ", " + str(b_options))
-
-                    found_wrong, detected_flag_1 = True, True
-                    for _, _, _, dna_string in path_matching(dna_string=detected_dna_string,
-                                                             accessor=accessor, index_queue=index_queue,
-                                                             occur_location=location,
-                                                             has_insertion=has_insertion,
-                                                             has_deletion=has_deletion,
-                                                             verbose=verbose):
-                        if dna_string not in new_dna_strings:
-                            new_dna_strings.append(dna_string)
-
-                    recall_queue = index_queue[::-1][:observed_length - 1]
-                    for recall_index, original_vertex_index in enumerate(recall_queue):
-                        error_index = location - recall_index - 1
-                        if verbose:
-                            print("-" * 50)
-                            print("Search the error in the previous (" + str((recall_index + 1)) + ") location.")
-                            print("Check location = " + detected_dna_string[error_index] + " | " + str(error_index))
-
-                        for _, _, _, dna_string in path_matching(dna_string=detected_dna_string,
-                                                                 accessor=accessor, index_queue=index_queue,
-                                                                 occur_location=error_index,
-                                                                 has_insertion=has_insertion,
-                                                                 has_deletion=has_deletion,
-                                                                 verbose=verbose):
-                            if dna_string not in new_dna_strings:
-                                new_dna_strings.append(dna_string)
-                    break
-
-            if (not found_wrong) and (detected_dna_string not in repaired_dna_strings):
-                repaired_dna_strings.append(detected_dna_string)
-
-        if 0 <= len(new_dna_strings) <= heap_size:
-            dna_strings = new_dna_strings
+        >>> dna_sequence = "TCTCTATCTCTC"  # "TCTCTCTCTCTC" is original DNA sequence
+        >>> repair_dna(dna_sequence=dna_sequence, accessor=accessor, start_index=1, observed_length=2, has_indel=True)
+        (['TCTCTCTCTCTC', 'TCTCTGTCTCTC'], (1, False, 2, 14))
+        >>> vt_check = "AACGC"  # check list of Varshamov-Tenengolts code.
+        >>> repair_dna(dna_sequence=dna_sequence, accessor=accessor, start_index=1, observed_length=2, \
+                       vt_check=vt_check, has_indel=True)
+        (['TCTCTCTCTCTC'], (1, True, 2, 14))
+    """
+    nucleotides = "ACGT"
+
+    location, vertex_index, index_queue = 0, start_index, -ones(shape=(len(dna_sequence),), dtype=int)
+    split_sequences, chuck_sequences, index_markers = [""], [], []
+    detected_count, chuck_flag, visited_times = 0, False, 0
+
+    while location < len(dna_sequence):
+        used_indices, nucleotide = where(accessor[vertex_index] >= 0)[0], dna_sequence[location]
+        if dna_sequence[location] in [nucleotides[used_index] for used_index in used_indices]:
+            split_sequences[-1] += nucleotide
+            vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
+            index_queue[location] = vertex_index
+            visited_times += 1
+            location += 1
+        elif len(split_sequences[-1]) > 0:
+            detected_count += 1
+            split_sequences[-1] = split_sequences[-1][: - observed_length + 1]
+            vertex_index = dna_to_number(dna_sequence[location + 1: location + observed_length + 1], is_string=False)
+            split_sequences.append(nucleotides[vertex_index % 4])
+            index_markers.append(index_queue[location - observed_length: location])
+            chuck_sequences.append(dna_sequence[location - observed_length + 1: location + observed_length])
+            location += observed_length + 1
+
+    repaired_fragment_set = [set() for _ in range(len(index_markers))]
+    for index, (chuck_sequence, index_marker) in enumerate(zip(chuck_sequences, index_markers)):
+        for recall, vertex_index in enumerate(index_marker[::-1]):
+            record, times = path_matching(dna_sequence=chuck_sequence, accessor=accessor, has_indel=has_indel,
+                                          previous_index=vertex_index, occur_location=observed_length - recall - 1)
+            visited_times += times
+            for _, fragment in record:
+                if dna_sequence not in repaired_fragment_set[index]:
+                    repaired_fragment_set[index].add(fragment)
+        repaired_fragment_set[index] = list(repaired_fragment_set[index])
+
+    repaired_results, count = set(), 1
+    for fragments in repaired_fragment_set:
+        count *= len(fragments)
+
+    if count == 0 or count > heap_size:
+        if vt_check is not None:
+            if vt_check == set_vt(dna_sequence=dna_sequence, vt_length=len(vt_check)):
+                return [dna_sequence], (0, False, 0, visited_times)
+            else:
+                return [], (0, True, 0, visited_times)
         else:
-            break
+            return [dna_sequence], (0, False, 0, visited_times)
 
-    repaired_results = []
-    if len(repaired_dna_strings) > 0:
-        for repaired_dna_string in repaired_dna_strings:
-            if vt_check is not None:
-                if vt_check == set_vt(dna_string=repaired_dna_string, vt_length=len(vt_check), nucleotides=nucleotides):
-                    repaired_results.append(repaired_dna_string)
-                else:
-                    detected_flag_2 = True
+    for fragments in product(*repaired_fragment_set):
+        repaired_dna_sequence = ""
+        for index in range(len(split_sequences) - 1):
+            repaired_dna_sequence += split_sequences[index] + fragments[index]
+        repaired_dna_sequence += split_sequences[-1]
+        if vt_check is not None:
+            if vt_check == set_vt(dna_sequence=repaired_dna_sequence, vt_length=len(vt_check)):
+                repaired_results.add(repaired_dna_sequence)
             else:
-                repaired_results.append(repaired_dna_string)
-
-    if len(repaired_results) == 0:  # use original Varshamov-Tenengolts repair (only one error).
-        if verbose:
-            print()
-            print("No result check, we use original Varshamov-Tenengolts repair.")
-            print()
-
-        # no mathematical method, using saturated attempt (substitute nucleotide in each location).
-        for assume_location in range(len(original_dna_string)):
-            for assume_nucleotide in list(filter(lambda n: n != original_dna_string[assume_location], nucleotides)):
-                if verbose:
-                    print("-" * 50)
-                    print("Find the substitution error (" + str(assume_location) + ") location.")
-                    print(original_dna_string[assume_location] + " needs to be substituted by "
-                          + assume_nucleotide + ".")
-
-                # substitution error checking through Varshamov-Tenengolts principle.
-                repaired_dna_string = list(original_dna_string)
-                repaired_dna_string[assume_location] = assume_nucleotide
-                repaired_dna_string = "".join(repaired_dna_string)
-
-                if vt_check == set_vt(dna_string=repaired_dna_string, vt_length=len(vt_check), nucleotides=nucleotides):
-                    found_wrong, vertex_index = False, start_index
-                    for location, nucleotide in enumerate(repaired_dna_string):
-                        used_indices = where(accessor[vertex_index] >= 0)[0]
-                        if nucleotide in [nucleotides[used_index] for used_index in used_indices]:
-                            vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
-                        else:
-                            found_wrong = True
-                            break
-                    if not found_wrong:
-                        repaired_results.append(repaired_dna_string)
-
-        if has_insertion:
-            # insertion error checking through Varshamov-Tenengolts principle.
-            for assume_location in range(len(original_dna_string)):
-                if verbose:
-                    nucleotide = original_dna_string[assume_location]
-                    print("-" * 50)
-                    print("Find the insertion error (" + str(assume_location) + ") location.")
-                    print(nucleotide + " needs to be deleted.")
-
-                repaired_dna_string = list(original_dna_string)
-                del repaired_dna_string[assume_location]
-                repaired_dna_string = "".join(repaired_dna_string)
-
-                if vt_check == set_vt(dna_string=repaired_dna_string, vt_length=len(vt_check), nucleotides=nucleotides):
-                    found_wrong, vertex_index = False, start_index
-                    for location, nucleotide in enumerate(repaired_dna_string):
-                        used_indices = where(accessor[vertex_index] >= 0)[0]
-                        if nucleotide in [nucleotides[used_index] for used_index in used_indices]:
-                            vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
-                        else:
-                            found_wrong = True
-                            break
-                    if not found_wrong:
-                        repaired_results.append(repaired_dna_string)
-
-        if has_deletion:
-            # deletion error checking through Varshamov-Tenengolts principle.
-            for assume_location in range(len(original_dna_string) + 1):
-                for assume_nucleotide in nucleotides:
-                    if verbose:
-                        print("-" * 50)
-                        print("Find the deletion error (" + str(assume_location) + ") location.")
-                        print(assume_nucleotide + " need to be inserted.")
-
-                    repaired_dna_string = list(original_dna_string)
-                    repaired_dna_string.insert(assume_location, assume_nucleotide)
-                    repaired_dna_string = "".join(repaired_dna_string)
-
-                    if vt_check == set_vt(dna_string=repaired_dna_string, vt_length=len(vt_check),
-                                          nucleotides=nucleotides):
-                        found_wrong, vertex_index = False, start_index
-                        for location, nucleotide in enumerate(repaired_dna_string):
-                            used_indices = where(accessor[vertex_index] >= 0)[0]
-                            if nucleotide in [nucleotides[used_index] for used_index in used_indices]:
-                                vertex_index = accessor[vertex_index][nucleotides.index(nucleotide)]
-                            else:
-                                found_wrong = True
-                                break
-                        if not found_wrong:
-                            repaired_results.append(repaired_dna_string)
+                chuck_flag = True
+        else:
+            repaired_results.add(repaired_dna_sequence)
 
-    return repaired_results, (detected_flag_1, detected_flag_2, len(repaired_dna_strings))
+    return sorted(list(repaired_results)), (detected_count, chuck_flag, count, visited_times)
 
 
-def find_vertices(observed_length, bio_filter, nucleotides=None, verbose=False):
+def find_vertices(observed_length, bio_filter, verbose=False):
     """
     Find valid vertices based on the given the biochemical constraints.
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
-    :param bio_filter: screening operation for identifying the valid DNA string (required the given constraints).
+    :param bio_filter: screening operation for identifying the valid DNA sequence (required the given constraints).
     :type bio_filter: dsw.biofilter.DefaultBioFilter
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: available vertices.
     :rtype: numpy.ndarray
 
     :raise ValueError: if no valid vertices are available under the required biochemical constraints.
@@ -492,53 +468,49 @@
         >>> # "1" refers to the available index of vertex, otherwise "0" refers to unavailable index of vertex.
         >>> find_vertices(observed_length=2, bio_filter=bio_filter).astype(int)
         array([0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0])
 
     .. note::
         Reference [1] Florent Capelli and Yann Strozecki (2019) Discrete Applied Mathematics
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     vertices, monitor = zeros(shape=(int(len(nucleotides) ** observed_length),), dtype=bool), Monitor()
 
     if verbose:
-        print("Find valid vertices in this observed length of DNA string.")
+        print("Find valid vertices in this observed length of DNA sequence.")
 
     for vertex_index in range(len(vertices)):
-        dna_string = number_to_dna(decimal_number=vertex_index, dna_length=observed_length)
-        vertices[vertex_index] = bio_filter.valid(dna_string=dna_string)
+        dna_sequence = number_to_dna(decimal_number=vertex_index, dna_length=observed_length)
+        vertices[vertex_index] = bio_filter.valid(dna_sequence=dna_sequence)
 
         if verbose:
-            monitor.output(vertex_index + 1, len(vertices))
+            monitor(vertex_index + 1, len(vertices), extra={"valid": sum(vertices[: vertex_index + 1])})
 
     valid_rate = sum(vertices) / len(vertices)
 
     if valid_rate == 0:
         raise ValueError("No vertex is collected!")
 
     if verbose:
         print(str(round(valid_rate * 100, 2)) + "% (" + str(sum(vertices)) + ") valid vertices are collected.")
 
     return vertices
 
 
-def connect_valid_graph(observed_length, vertices, nucleotides=None, verbose=False):
+def connect_valid_graph(observed_length, vertices, verbose=False):
     """
     Connect a valid graph by valid vertices.
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
     :param vertices: vertex accessor, in each cell, True is valid vertex and False is invalid vertex.
     :type vertices: numpy.ndarray
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: accessor of the valid graph.
     :rtype: numpy.ndarray
 
     :raise ValueError: if no valid vertices are available.
@@ -564,16 +536,15 @@
                [ 4, -1, -1,  7],
                [ 8, -1, -1, 11],
                [-1, -1, -1, -1]])
 
     .. note::
         Reference [1] Nicolaas Govert de Bruijn (1946) Indagationes Mathematicae
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     if vertices is None:
         raise ValueError("No collected vertex!")
 
     if verbose:
         print("Connect valid graph with valid vertices.")
 
@@ -586,40 +557,37 @@
             if vertices[vertex_index]:
                 latters = obtain_latters(current=vertex_index, observed_length=observed_length)
                 for position, latter_vertex_index in enumerate(latters):
                     if vertices[latter_vertex_index]:
                         accessor[vertex_index][position] = latter_vertex_index
 
             if verbose:
-                monitor.output(vertex_index + 1, len(vertices))
+                monitor(vertex_index + 1, len(vertices))
 
         if verbose:
             print("Valid graph is created.")
 
         return accessor
     else:
         raise ValueError("No collected vertex!")
 
 
-def connect_coding_graph(observed_length, vertices, threshold, nucleotides=None, verbose=False):
+def connect_coding_graph(observed_length, vertices, threshold, verbose=False):
     """
     Connect a coding algorithm by valid vertices and the threshold for minimum out-degree.
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
     :param vertices: vertex accessor, in each cell, True is valid vertex and False is invalid vertex.
     :type vertices: numpy.ndarray
 
     :param threshold: threshold for minimum out-degree.
     :type threshold: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: coding vertices and coding accessor.
     :rtype: (numpy.ndarray, numpy.ndarray)
 
     :raise ValueError: if no coding graph are created because of the vertex set and/or the trimming requirement.
@@ -648,31 +616,28 @@
                [-1, -1, -1, -1]])
         >>> vertices.astype(int)
         array([0, 1, 1, 0, 1, 0, 0, 1, 1, 0, 0, 1, 0, 1, 1, 0])
 
     .. note::
         Reference [1] Nicolaas Govert de Bruijn (1946) Indagationes Mathematicae
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
-
-    times = 1
+    times, nucleotides = 1, "ACGT"
 
     while True:
         if verbose:
             print("Check the vertex collection requirement in round " + str(times) + ".")
 
         new_vertices, monitor = zeros(shape=(int(len(nucleotides) ** observed_length),), dtype=bool), Monitor()
         saved_indices = where(vertices != 0)[0]
         for current, vertex_index in enumerate(saved_indices):
             latter_indices = obtain_latters(current=vertex_index, observed_length=observed_length)
             new_vertices[vertex_index] = sum(vertices[latter_indices]) >= threshold
 
             if verbose:
-                monitor.output(current + 1, len(saved_indices))
+                monitor(current + 1, len(saved_indices))
 
         changed = sum(vertices) - sum(new_vertices)
 
         if verbose:
             print(str(round(sum(new_vertices) / len(vertices) * 100, 2)) + "% (" + str(sum(new_vertices)) + ") "
                   + "valid vertices are saved.")
 
@@ -692,34 +657,164 @@
             if vertices[vertex_index]:
                 latters = obtain_latters(current=vertex_index, observed_length=observed_length)
                 for position, latter_vertex_index in enumerate(latters):
                     if vertices[latter_vertex_index]:
                         accessor[vertex_index][position] = latter_vertex_index
 
             if verbose:
-                monitor.output(vertex_index + 1, len(vertices))
+                monitor(vertex_index + 1, len(vertices))
+
+        if threshold == 1:
+            while True:
+                vertices = obtain_vertices(accessor)
+                graph = DiGraph()
+                for former_index, latter_indices in enumerate(accessor):
+                    for latter_index in latter_indices:
+                        if latter_index >= 0:
+                            graph.add_edge(u_of_edge=former_index, v_of_edge=latter_index)
+                useless_vertices, cycle = [], find_cycle(graph)
+                for former_index, latter_index in cycle:
+                    if len(where(accessor[former_index] >= 0)[0]) == 1:
+                        useless_vertices.append(former_index)
+                if len(useless_vertices) == len(cycle):
+                    for useless_vertex in useless_vertices:
+                        accessor[useless_vertex] = -1
+                        pairs = [(i, useless_vertex) for i in obtain_formers(useless_vertex, 10)]
+                        while len(pairs) > 0:
+                            new_pairs = []
+                            for former_index, latter_index in pairs:
+                                previous = len(where(accessor[former_index] >= 0)[0])
+                                accessor[former_index, latter_index % 4] = -1
+                                current = len(where(accessor[former_index] >= 0)[0])
+                                if previous > current == 0:
+                                    new_pairs += [(i, former_index) for i in obtain_formers(former_index, 10)]
+                            pairs = new_pairs
+                else:
+                    break
 
         if verbose:
             print("The coding graph is created.")
 
         return vertices, accessor
     else:
         raise ValueError("The coding graph cannot be created!")
 
 
-def create_random_shuffles(observed_length, nucleotides=None, random_seed=None, verbose=False):
+def remove_nasty_arc(accessor, latter_map, iteration=0, has_insertion=True, has_deletion=True, verbose=False):
+    """
+    Remove the nasty arc.
+
+    :param accessor: accessor of the coding algorithm.
+    :type accessor: numpy.ndarray
+
+    :param latter_map: latter map of the coding algorithm.
+    :type latter_map: dict
+
+    :param iteration: current round if required.
+    :type iteration: int
+
+    :param has_insertion: need to repair insertion error.
+    :type has_insertion: bool
+
+    :param has_deletion: need to repair deletion error.
+    :type has_deletion: bool
+
+    :param verbose: need to print log.
+    :type verbose: bool
+
+    :return: adjusted accessor, adjusted latter map, removed arc, and maximum intersection score.
+    :rtype: (numpy.ndarray, dict, tuple, int)
+
+    Example
+        >>> from numpy import array
+        >>> from dsw import accessor_to_latter_map, remove_nasty_arc
+        >>> # accessor with GC-balanced
+        >>> accessor = array([[-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1], \
+                              [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
+                              [-1,  1,  2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1], \
+                              [-1, -1, -1, -1], [ 4, -1, -1,  7], [ 8, -1, -1, 11], [-1, -1, -1, -1]])
+        >>> latter_map = accessor_to_latter_map(accessor)
+        >>> result = remove_nasty_arc(accessor=accessor, latter_map=latter_map, iteration=0, verbose=False, \
+                                      has_insertion=True, has_deletion=True)
+        >>> result[0]
+        array([[-1, -1, -1, -1],
+               [-1, -1, -1,  7],
+               [ 8, -1, -1, 11],
+               [-1, -1, -1, -1],
+               [-1,  1,  2, -1],
+               [-1, -1, -1, -1],
+               [-1, -1, -1, -1],
+               [-1, 13, 14, -1],
+               [-1,  1,  2, -1],
+               [-1, -1, -1, -1],
+               [-1, -1, -1, -1],
+               [-1, 13, 14, -1],
+               [-1, -1, -1, -1],
+               [ 4, -1, -1,  7],
+               [ 8, -1, -1, 11],
+               [-1, -1, -1, -1]])
+        >>> result[1]
+        {1: [7], 2: [8, 11], 4: [1, 2], 7: [13, 14], 8: [1, 2], 11: [13, 14], 13: [4, 7], 14: [8, 11]}
+        >>> result[2]
+        (1, 4)
+        >>> result[3]
+        [16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16, 16]
+
+    .. note::
+        The graph information contained in "accessor" and "latter_map" is consistent.
+
+        It is a gift for the follow-up investigation.
+        That is, removing arc to improve the capability of the probabilistic error correction.
+    """
+    nucleotides = "ACGT"
+
+    observed_length = int(log(len(accessor)) / log(len(nucleotides)))
+
+    if verbose:
+        if iteration > 0:
+            print("Calculate the intersection score for each remained arc in " + str(iteration) + " round(s).")
+        else:
+            print("Calculate the intersection score for each remained arc.")
+
+    scores = calculate_intersection_score(latter_map=latter_map, has_insertion=has_insertion, has_deletion=has_deletion,
+                                          observed_length=observed_length, verbose=verbose)
+
+    vertex_indices = unique(where(scores == max(scores))[0])
+
+    former = intersect1d(obtain_vertices(accessor=accessor), vertex_indices)[0]
+    former_value, latter_value = former % len(nucleotides), argmax(scores[former])
+    latter = int((former * len(nucleotides) + latter_value) % (len(nucleotides) ** observed_length))
+
+    accessor[former, latter_value] = -1
+    del latter_map[former][latter_map[former].index(latter)]
+    if len(latter_map[former]) == 0:
+        del latter_map[former]
+
+    scores = scores.reshape(-1)
+    scores = scores[scores > 0].tolist()
+    score_record = array(list(Counter(scores).items())).T
+    score_record = score_record[:, argsort(score_record[0])[::-1]]
+
+    if verbose:
+        print("Current scores are:")
+        print(score_record)
+        print("Remove arc " + number_to_dna(int(former), dna_length=observed_length) + " -> "
+              + number_to_dna(int(latter), dna_length=observed_length)
+              + " with the maximum intersection score " + str(max(scores)) + ".")
+
+    return accessor, latter_map, (former, latter), scores
+
+
+def create_random_shuffles(observed_length, random_seed=None, verbose=False):
     """
     Create the shuffles for accessor through the random mechanism.
 
-    :param observed_length: length of the DNA string in a vertex.
+    :param observed_length: length of the DNA sequence in a vertex.
     :type observed_length: int
 
-    :param nucleotides: usage of nucleotides.
-    :type nucleotides: list
-
     :param random_seed: random seed for creating shuffles.
     :type random_seed: int
 
     :param verbose: need to print log.
     :type verbose: bool
 
     :return: shuffles for accessor.
@@ -752,16 +847,15 @@
         Value 0 ~ 3 in each line shuffle only describes the relationship between progressive order and position.
         The original position is [0, 1, 2, 3].
         If the follow-up nucleotides in a vertex are ["A", "G"] when the line shuffle is [3, 2, 1, 0],
         This line shuffle can be regarded as [1, -, 0, -] for ["A", -, "G", -].
 
         Ths shuffle will not disclose the topology information of accessor.
     """
-    if nucleotides is None:
-        nucleotides = ["A", "C", "G", "T"]
+    nucleotides = "ACGT"
 
     shuffles = zeros(shape=(4 ** observed_length, len(nucleotides)), dtype=int)
     shuffles[:, 1] = 1
     shuffles[:, 2] = 2
     shuffles[:, 3] = 3
 
     random.seed(random_seed)
@@ -769,12 +863,12 @@
     monitor = Monitor()
     for index in range(4 ** observed_length):
         card = shuffles[index]
         random.shuffle(card)
         shuffles[index] = card
 
         if verbose:
-            monitor.output(index + 1, 4 ** observed_length)
+            monitor(index + 1, 4 ** observed_length)
 
     random.seed(None)
 
     return shuffles
```

## tests/test_bio_filters.py

```diff
@@ -11,87 +11,90 @@
         self.single_repeats = 1000
         self.dna_length = 80
         self.observed_length = 10
         self.reference = "ACGT" * (self.dna_length // 4)
         self.bio_filters = [LocalBioFilter(observed_length=self.observed_length, max_homopolymer_runs=2),
                             LocalBioFilter(observed_length=self.observed_length, gc_range=[0.5, 0.5]),
                             LocalBioFilter(observed_length=self.observed_length, undesired_motifs=["GCC"])]
-        self.dna_string_group = [[], [], []]
+        self.dna_sequence_group = [[], [], []]
 
         random.seed(self.random_seed)
 
-        # for normal DNA strings.
+        # for normal DNA sequences.
         for _ in range(self.single_repeats):
             nucleotides = random.choice(["AAA", "CCC", "GGG", "TTT"])
             location = random.randint(0, self.dna_length - 2)
-            dna_string = list(self.reference)
-            dna_string[int(location)], dna_string[int(location) + 1], dna_string[int(location) + 2] = nucleotides
-            self.dna_string_group[0].append((False, "".join(dna_string)))
+            dna_sequence = list(self.reference)
+            dna_sequence[int(location)], dna_sequence[int(location) + 1], dna_sequence[int(location) + 2] = nucleotides
+            self.dna_sequence_group[0].append((False, "".join(dna_sequence)))
 
             location = random.randint(0, self.dna_length)
             mapping = {"A": "C", "C": "A", "G": "T", "T": "G"}
-            dna_string = list(self.reference)
-            dna_string[location] = mapping[dna_string[location]]
-            self.dna_string_group[1].append((False, "".join(dna_string)))
+            dna_sequence = list(self.reference)
+            dna_sequence[location] = mapping[dna_sequence[location]]
+            self.dna_sequence_group[1].append((False, "".join(dna_sequence)))
 
             location = random.randint(0, self.dna_length - 2)
-            dna_string = list(self.reference)
-            dna_string[int(location)], dna_string[int(location) + 1], dna_string[int(location) + 2] = ["G", "C", "C"]
-            self.dna_string_group[2].append((False, "".join(dna_string)))
+            dna_sequence = list(self.reference)
+            dna_sequence[int(location)], dna_sequence[int(location) + 1], dna_sequence[int(location) + 2] = ["G", "C", "C"]
+            self.dna_sequence_group[2].append((False, "".join(dna_sequence)))
 
     def test(self):
-        for dna_strings, bio_filter in zip(self.dna_string_group, self.bio_filters):
-            for flag, dna_string in dna_strings:
-                self.assertEqual(flag, bio_filter.valid(dna_string=dna_string, only_last=False))
+        for dna_sequences, bio_filter in zip(self.dna_sequence_group, self.bio_filters):
+            for flag, dna_sequence in dna_sequences:
+                self.assertEqual(flag, bio_filter.valid(dna_sequence=dna_sequence, only_last=False))
 
 
 class TestLocalBioFilterOnlyLast(TestCase):
 
+    # noinspection PyUnresolvedReferences
     def setUp(self):
         self.random_seed = 2021
         self.single_repeats = 1000
         self.dna_length = 80
         self.observed_length = 10
         self.reference = "ACGT" * (self.dna_length // 4)
         self.bio_filters = [LocalBioFilter(observed_length=self.observed_length, max_homopolymer_runs=2),
                             LocalBioFilter(observed_length=self.observed_length, gc_range=[0.5, 0.5]),
                             LocalBioFilter(observed_length=self.observed_length, undesired_motifs=["GCC"])]
-        self.dna_string_group = [[], [], []]
+        self.dna_sequence_group = [[], [], []]
 
         random.seed(self.random_seed)
 
-        # for normal DNA strings.
+        # for normal DNA sequences.
         for _ in range(self.single_repeats):
             nucleotides = random.choice(["AAA", "CCC", "GGG", "TTT"])
             location = random.randint(0, self.dna_length - 2)
-            dna_string = list(self.reference)
-            dna_string[int(location)], dna_string[int(location) + 1], dna_string[int(location) + 2] = nucleotides
-            dna_string = "".join(dna_string)
+            dna_sequence = list(self.reference)
+            dna_sequence[int(location)], dna_sequence[int(location) + 1], dna_sequence[int(location) + 2] = nucleotides
+            dna_sequence = "".join(dna_sequence)
 
             flag = True
             for pattern in ["AAA", "CCC", "GGG", "TTT"]:
-                if pattern in dna_string[-self.observed_length:]:
+                if pattern in dna_sequence[-self.observed_length:]:
                     flag = False
-            self.dna_string_group[0].append((flag, dna_string))
+            self.dna_sequence_group[0].append((flag, dna_sequence))
 
             location = random.randint(0, self.dna_length)
             mapping = {"A": "C", "C": "A", "G": "T", "T": "G"}
-            dna_string = list(self.reference)
-            dna_string[location] = mapping[dna_string[location]]
-            dna_string = "".join(dna_string)
+            dna_sequence = list(self.reference)
+            dna_sequence[location] = mapping[dna_sequence[location]]
+            dna_sequence = "".join(dna_sequence)
 
-            gc_count = dna_string[-self.observed_length:].count("C") + dna_string[-self.observed_length:].count("G")
+            gc_count = dna_sequence[-self.observed_length:].count("C") + dna_sequence[-self.observed_length:].count("G")
             flag = gc_count == (self.observed_length // 2)
-            self.dna_string_group[1].append((flag, dna_string))
+            self.dna_sequence_group[1].append((flag, dna_sequence))
 
             location = random.randint(0, self.dna_length - 2)
-            dna_string = list(self.reference)
-            dna_string[int(location)], dna_string[int(location) + 1], dna_string[int(location) + 2] = ["G", "C", "C"]
-            dna_string = "".join(dna_string)
+            dna_sequence = list(self.reference)
+            dna_sequence[int(location) + 0] = "G"
+            dna_sequence[int(location) + 1] = "C"
+            dna_sequence[int(location) + 2] = "C"
+            dna_sequence = "".join(dna_sequence)
 
-            flag = "GCC" not in dna_string[-self.observed_length:]
-            self.dna_string_group[2].append((flag, dna_string))
+            flag = "GCC" not in dna_sequence[-self.observed_length:]
+            self.dna_sequence_group[2].append((flag, dna_sequence))
 
     def test(self):
-        for dna_strings, bio_filter in zip(self.dna_string_group, self.bio_filters):
-            for flag, dna_string in dna_strings:
-                self.assertEqual(flag, bio_filter.valid(dna_string=dna_string, only_last=True))
+        for dna_sequences, bio_filter in zip(self.dna_sequence_group, self.bio_filters):
+            for flag, dna_sequence in dna_sequences:
+                self.assertEqual(flag, bio_filter.valid(dna_sequence=dna_sequence, only_last=True))
```

## tests/test_capacities.py

```diff
@@ -27,17 +27,19 @@
         self.empty_graph = zeros(shape=(16, 16), dtype=int)
 
     def test(self):
         freed_maximum_eigenvalue = real(max(linalg.eig(self.freed_graph)[0]))
         empty_maximum_eigenvalue = real(max(linalg.eig(self.empty_graph)[0]))
         freed_value = log2(freed_maximum_eigenvalue) if freed_maximum_eigenvalue > 0.0 else 0.0
         empty_value = log2(empty_maximum_eigenvalue) if empty_maximum_eigenvalue > 0.0 else 0.0
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.freed_graph), repeats=10) - freed_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.freed_graph),
+                                                  repeats=10) - freed_value)
         self.assertEqual(relative_error <= 1e-4, True)
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.empty_graph), repeats=10) - empty_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.empty_graph),
+                                                  repeats=10) - empty_value)
         self.assertEqual(relative_error <= 1e-4, True)
         self.assertEqual(abs(2.0 - freed_value) <= 1e-4, True)
         self.assertEqual(abs(0.0 - empty_value) <= 1e-4, True)
 
 
 class TestBiochemicals(TestCase):
 
@@ -78,17 +80,19 @@
                                         [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]])
 
     def test(self):
         h_maximum_eigenvalue = real(max(linalg.eig(self.homopolymer_graph)[0]))
         g_maximum_eigenvalue = real(max(linalg.eig(self.gc_balanced_graph)[0]))
         h_value = log2(h_maximum_eigenvalue) if h_maximum_eigenvalue > 0.0 else 0.0
         g_value = log2(g_maximum_eigenvalue) if g_maximum_eigenvalue > 0.0 else 0.0
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.homopolymer_graph), repeats=10) - h_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.homopolymer_graph),
+                                                  repeats=10) - h_value)
         self.assertEqual(relative_error <= 1e-4, True)
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.gc_balanced_graph), repeats=10) - g_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.gc_balanced_graph),
+                                                  repeats=10) - g_value)
         self.assertEqual(relative_error <= 1e-4, True)
         self.assertEqual(abs(log2(3.0) - h_value) <= 1e-4, True)
         self.assertEqual(abs(log2(2.0) - g_value) <= 1e-4, True)
 
 
 class TestCycles(TestCase):
 
@@ -167,21 +171,25 @@
         c_3_maximum_eigenvalue = real(max(linalg.eig(self.cycle_3_graph)[0]))
         c_4_maximum_eigenvalue = real(max(linalg.eig(self.cycle_4_graph)[0]))
         c_5_maximum_eigenvalue = real(max(linalg.eig(self.cycle_5_graph)[0]))
         c_2_value = log2(c_2_maximum_eigenvalue) if c_2_maximum_eigenvalue > 0.0 else 0.0
         c_3_value = log2(c_3_maximum_eigenvalue) if c_3_maximum_eigenvalue > 0.0 else 0.0
         c_4_value = log2(c_4_maximum_eigenvalue) if c_4_maximum_eigenvalue > 0.0 else 0.0
         c_5_value = log2(c_5_maximum_eigenvalue) if c_5_maximum_eigenvalue > 0.0 else 0.0
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_2_graph), repeats=10) - c_2_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_2_graph),
+                                                  repeats=10) - c_2_value)
         self.assertEqual(relative_error <= 1e-4, True)
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_3_graph), repeats=10) - c_3_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_3_graph),
+                                                  repeats=10) - c_3_value)
         self.assertEqual(relative_error <= 1e-4, True)
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_4_graph), repeats=10) - c_4_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_4_graph),
+                                                  repeats=10) - c_4_value)
         self.assertEqual(relative_error <= 1e-4, True)
-        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_5_graph), repeats=10) - c_5_value)
+        relative_error = abs(approximate_capacity(accessor=adjacency_matrix_to_accessor(self.cycle_5_graph),
+                                                  repeats=10) - c_5_value)
         self.assertEqual(relative_error <= 1e-4, True)
         self.assertEqual(abs(c_2_value - 0.0) <= 1e-4, True)
         self.assertEqual(abs(c_3_value - 0.0) <= 1e-4, True)
         self.assertEqual(abs(c_4_value - 0.0) <= 1e-4, True)
         self.assertEqual(abs(c_5_value - 0.0) <= 1e-4, True)
```

## tests/test_coding.py

```diff
@@ -1,66 +1,88 @@
 from numpy import array, all
 from unittest import TestCase
 
-from dsw import encode, decode, repair_dna
+from dsw import encode, decode
 
 
-class TestEncode(TestCase):
+class TestNormalEncode(TestCase):
 
     def setUp(self):
         self.accessor = array([[-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1],
                                [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                [-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1]])
         self.start_index = 1
         self.vt_length = 4
         self.binary_message = array([0, 1, 0, 1, 0, 1, 0, 1])
 
     def test(self):
-        dna_string = encode(accessor=self.accessor, binary_message=self.binary_message, start_index=self.start_index)
-        self.assertEqual("TCTCTCT", dna_string)
-        dna_string, vt_list = encode(accessor=self.accessor, binary_message=self.binary_message,
-                                     start_index=self.start_index, vt_length=self.vt_length)
-        self.assertEqual("TCTCTCT", dna_string)
-        self.assertEqual("TATA", vt_list)
+        dna_sequence = encode(accessor=self.accessor, binary_message=self.binary_message, start_index=self.start_index)
+        self.assertEqual("TCTCTCT", dna_sequence)
+        dna_sequence, vt_list = encode(accessor=self.accessor, binary_message=self.binary_message,
+                                       start_index=self.start_index, vt_length=self.vt_length)
+        self.assertEqual("TCTCTCT", dna_sequence)
+        self.assertEqual("TAGC", vt_list)
 
 
-class TestDecode(TestCase):
+class TestNormalDecode(TestCase):
 
     def setUp(self):
         self.accessor = array([[-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1],
                                [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                [-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1]])
         self.start_index = 1
         self.vt_length = 4
-        self.dna_string = "TCTCTCT"
+        self.dna_sequence = "TCTCTCT"
 
     def test(self):
-        binary_message = decode(accessor=self.accessor, dna_string=self.dna_string, start_index=1, bit_length=8)
+        binary_message = decode(accessor=self.accessor, dna_sequence=self.dna_sequence, start_index=1, bit_length=8)
         self.assertEqual(all(binary_message == array([0, 1, 0, 1, 0, 1, 0, 1])), True)
 
 
-class TestRepair(TestCase):
+class TestNormalMap(TestCase):
 
     def setUp(self):
         self.accessor = array([[-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1],
                                [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                [-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1]])
-        self.dna_string = "TCTCTATCTCTC"  # "TCTCTCTCTCTC" is original DNA string
-        self.vt_check = "ACTG"  # check list of Varshamov-Tenengolts code.
+        self.seed = 2021
+
+
+class TestFasterEncode(TestCase):
+
+    def setUp(self):
+        self.accessor = array([[-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1],
+                               [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
+                               [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
+                               [-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1]])
+        self.start_index = 1
+        self.vt_length = 4
+        self.binary_message = array([0, 1, 0, 1, 0, 1, 0, 1])
+
+    def test(self):
+        dna_sequence = encode(accessor=self.accessor, binary_message=self.binary_message, start_index=self.start_index,
+                              is_faster=True)
+        self.assertEqual("AGAGAGAG", dna_sequence)
+        dna_sequence, vt_list = encode(accessor=self.accessor, binary_message=self.binary_message,
+                                       start_index=self.start_index, vt_length=self.vt_length, is_faster=True)
+        self.assertEqual("AGAGAGAG", dna_sequence)
+        self.assertEqual("AATA", vt_list)
+
+
+class TestFasterDecode(TestCase):
+
+    def setUp(self):
+        self.accessor = array([[-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1],
+                               [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
+                               [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
+                               [-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1]])
+        self.start_index = 1
+        self.vt_length = 4
+        self.dna_sequence = "AGAGAGAG"
 
     def test(self):
-        repaired_dna_strings, additions = repair_dna(dna_string=self.dna_string,
-                                                     accessor=self.accessor, start_index=1,
-                                                     observed_length=2, check_iterations=1,
-                                                     has_insertion=True, has_deletion=True, verbose=False)
-        self.assertEqual(repaired_dna_strings, ["TCTCTCTCTCTC", "TCTCTGTCTCTC"])
-        self.assertEqual(additions, (True, False, 2))
-
-        repaired_dna_strings, additions = repair_dna(dna_string=self.dna_string, vt_check=self.vt_check,
-                                                     accessor=self.accessor, start_index=1,
-                                                     observed_length=2, check_iterations=1,
-                                                     has_insertion=True, has_deletion=True, verbose=False)
-        self.assertEqual(repaired_dna_strings, ["TCTCTCTCTCTC"])
-        self.assertEqual(additions, (True, True, 2))
+        binary_message = decode(accessor=self.accessor, dna_sequence=self.dna_sequence, start_index=1, bit_length=8,
+                                is_faster=True)
+        self.assertEqual(all(binary_message == array([0, 1, 0, 1, 0, 1, 0, 1])), True)
```

## tests/test_generating.py

```diff
@@ -1,8 +1,8 @@
-from numpy import array, all
+from numpy import array, all, where
 from unittest import TestCase
 
 from dsw import LocalBioFilter, find_vertices, connect_valid_graph, connect_coding_graph
 
 
 class TestFindVertices(TestCase):
 
@@ -36,9 +36,9 @@
         self.coding_graph = array([[-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1],
                                    [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                    [-1, 1, 2, -1], [-1, -1, -1, -1], [-1, -1, -1, -1], [-1, 13, 14, -1],
                                    [-1, -1, -1, -1], [4, -1, -1, 7], [8, -1, -1, 11], [-1, -1, -1, -1]])
 
     def test(self):
         vertices, graph = connect_coding_graph(observed_length=2, vertices=self.vertices, threshold=1)
-        self.assertEqual(all(self.vertices == vertices.astype(int)), True)
+        self.assertEqual(all(where(self.vertices == 1)[0] == vertices.astype(int)), True)
         self.assertEqual(all(self.coding_graph == graph), True)
```

## tests/test_number_vs_binary_message.py

```diff
@@ -46,13 +46,13 @@
 
 class TestTransform(TestCase):
 
     def setUp(self):
         self.bit_length = 8
 
     def test(self):
-        for requested in range(2 ** (self.bit_length * 2)):
+        for requested in range(2 ** self.bit_length):
             bits = number_to_bit(decimal_number=str(requested), bit_length=self.bit_length)
             predicted_1 = int(bit_to_number(bit_array=bits))
             predicted_2 = bit_to_number(bit_array=bits, is_string=False)
             self.assertEqual(requested, predicted_1)
             self.assertEqual(requested, predicted_2)
```

## tests/test_shuffling.py

```diff
@@ -22,10 +22,10 @@
 
     def test(self):
         for source in self.bit_matrix:
             for shuffles in self.shuffle_group:
                 for start_index in self.start_indices:
                     oligo = encode(binary_message=source, accessor=self.accessor,
                                    shuffles=shuffles, start_index=start_index)
-                    target = decode(dna_string=oligo, accessor=self.accessor, bit_length=self.bit_length,
+                    target = decode(dna_sequence=oligo, accessor=self.accessor, bit_length=self.bit_length,
                                     shuffles=shuffles, start_index=start_index)
                     self.assertEqual(all(source == target), True)
```

## Comparing `tests/test_number_vs_dna_string.py` & `tests/test_number_vs_dna_sequence.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 
 
 class TestNumber(TestCase):
 
     def setUp(self):
         seed(2021)
         self.dna_length = 10
-        self.test_dna_strings = ["".join(["ACGT"[randint(0, 3)] for _ in range(self.dna_length)])
-                                 for _ in range(10)]
+        self.test_dna_sequences = ["".join(["ACGT"[randint(0, 3)] for _ in range(self.dna_length)])
+                                   for _ in range(10)]
         self.verify_numbers = [937770, 807052, 502551, 991128, 88040, 531838, 908835, 656257, 889866, 144398]
 
     def test(self):
-        results = [int(dna_to_number(dna_string=dna_string)) for dna_string in self.test_dna_strings]
+        results = [int(dna_to_number(dna_sequence=dna_sequence)) for dna_sequence in self.test_dna_sequences]
         self.assertEqual(results, self.verify_numbers)
-        results = [dna_to_number(dna_string=dna_string, is_string=False) for dna_string in self.test_dna_strings]
+        results = [dna_to_number(dna_sequence=dna_sequence, is_string=False)
+                   for dna_sequence in self.test_dna_sequences]
         self.assertEqual(results, self.verify_numbers)
 
 
 class TestOligo(TestCase):
 
     def setUp(self):
         seed(2021)
         self.dna_length = 10
         self.test_numbers = [randint(0, 4 ** self.dna_length) for _ in range(10)]
-        self.verify_dna_strings = ["TATGTTCAAA", "GATCGGTCAC", "CTTGGGAGCC", "ACACGTTTAG", "TGATAATTGG",
-                                   "TTAGGCCAGT", "AGAAGGAGGG", "GGAAATAAAA", "GAGGATCGAG", "GCCTGCGACG"]
+        self.verify_dna_sequences = ["TATGTTCAAA", "GATCGGTCAC", "CTTGGGAGCC", "ACACGTTTAG", "TGATAATTGG",
+                                     "TTAGGCCAGT", "AGAAGGAGGG", "GGAAATAAAA", "GAGGATCGAG", "GCCTGCGACG"]
 
     def test(self):
         results = [number_to_dna(decimal_number=str(number), dna_length=self.dna_length)
                    for number in self.test_numbers]
-        self.assertEqual(results, self.verify_dna_strings)
+        self.assertEqual(results, self.verify_dna_sequences)
         results = [number_to_dna(decimal_number=number, dna_length=self.dna_length)
                    for number in self.test_numbers]
-        self.assertEqual(results, self.verify_dna_strings)
+        self.assertEqual(results, self.verify_dna_sequences)
 
 
 class TestTransform(TestCase):
 
     def setUp(self):
         self.oligo_length = 8
 
     def test(self):
         for requested in range(4 ** self.oligo_length):
-            dna_string = number_to_dna(decimal_number=str(requested), dna_length=self.oligo_length)
-            predicted_1 = int(dna_to_number(dna_string=dna_string))
-            predicted_2 = dna_to_number(dna_string=dna_string, is_string=False)
+            dna_sequence = number_to_dna(decimal_number=str(requested), dna_length=self.oligo_length)
+            predicted_1 = int(dna_to_number(dna_sequence=dna_sequence))
+            predicted_2 = dna_to_number(dna_sequence=dna_sequence, is_string=False)
             self.assertEqual(requested, predicted_1)
             self.assertEqual(requested, predicted_2)
```

## Comparing `DNASpiderWeb-1.0.dist-info/METADATA` & `DNASpiderWeb-1.1.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: DNASpiderWeb
-Version: 1.0
-Summary: package for Spider-Web
+Version: 1.1
+Summary: SPIDER-WEB generates coding algorithms with superior error tolerance and real-time information retrieval capacity
 Home-page: https://github.com/HaolingZHANG/DNASpiderWeb
 Author: Haoling ZHANG
 Author-email: zhanghaoling@genomics.cn
-License: GPL
-Keywords: DNA-based Storage,Coding Algorithm,Automatic Algorithm Generator,Probabilistic Error-Correction
+License: BGI-Research
+Keywords: DNA-based data storage,coding algorithm,automatic algorithm generator,probabilistic error correction
 Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
+License-File: LICENSE.pdf
 Requires-Dist: numpy
-Requires-Dist: scipy
+Requires-Dist: networkx
 
-As a genetic material, DNA has become an attractive medium for storing digital information gradually. Besides the biochemical progress on DNA synthesis and sequencing, novel coding algorithms need to be constructed catering to the specific constraints in DNA storage. In recent years, a growing number of functional biochemical operations and storage environments were introduced, bringing in various biochemical constraints including but not confined to long single-nucleotide repeats and abnormal GC content. Given several local biochemical constraints and their combinations, the code rate capacity and capacity-achieving coding algorithms require in-depth investigation. In this work, we design an automatic generator, named SPIDER-WEB, to create corresponding graph-based algorithms which could be used directly or served as a benchmark for the construction of coding algorithms. The main advantage of SPIDER-WEB is that it provides an efficient way to applicable coding algorithms for arbitrary local biochemical constraints in an automatic way and support for probabilistic error correction and one-time pad encryption.
+DNA has been considered a promising medium for storing digital information. Previously, functions including bit-to-base transcoding and error correction are implemented by independent algorithms. It would result in either increased computational complexity or compromised error tolerance when attempting to correct various types of errors, especially for insertions/deletions (indels). To address this issue, we report a graph-based architecture, named SPIDER-WEB, providing an all-in-one coding solution by generating customized algorithms with an efficient built-in error correction function. SPIDER-WEB is able to correct a maximum of 4% edit errors in the DNA sequences including substitution and indel, with only 5.5% logical redundancy. In addition, SPIDER-WEB enables real-time retrieval of megabyte-level data with a 100x execution speed improvement over conventional methods and hold the potential of practicability for large-scale data storage applications at the exabyte-level.
```

## Comparing `DNASpiderWeb-1.0.dist-info/RECORD` & `DNASpiderWeb-1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-dsw/__init__.py,sha256=2lw4NQ1Rt2H3Uy4d_sWEySf2wohqns7LoiEe3txQzS0,810
-dsw/biofilter.py,sha256=IWmZ9i8znoimtg-Zm09UUTCSffHhcs4E3jq4yxM7pkg,6649
-dsw/graphized.py,sha256=-DXtMYWxYG4zZ9dbpQ0HjFKG6t7esez0fhATRlNL42k,39865
-dsw/operation.py,sha256=wakulyL6dItTvMZ13B0uS5UM9SskUzrurSmOzF7bGps,13601
-dsw/spiderweb.py,sha256=Hv1iLZ8qyILgR_wraCb5bKQw9UMtZ2HLNuiAi5xsd40,34242
+dsw/__init__.py,sha256=xTcN_WSWHsZkCjbg6DCEwz3DhRYCknIs_Twu6FV3fbI,901
+dsw/biofilter.py,sha256=iuLezgTrxRZWiGkM3kaL2vUwiGt3u7BV8XZsUOlgkQU,6689
+dsw/graphized.py,sha256=IPd-uZsHqIgso6LFaP_4y8cLFhBL95_PYAebbrzqKHA,36014
+dsw/operation.py,sha256=CcQ7SRH9K-8Tya_t-lsP7L5MpzeAGJpSFmD813duJ80,13764
+dsw/spiderweb.py,sha256=Mbu93tqGkBLblTyXvwRTsxb7WGfcnMX8DuTDbTM9mYI,36995
 tests/test_accessor_vs_latter_map.py,sha256=xOWmgGdvIgIjhlWSBtFsOpohrgtHINzQmEDOnYWuEw0,718
 tests/test_accessor_vs_matrix.py,sha256=QdMofYFGjMvDTs7pgNq_-9NODIfA6Vquy_s-_JyDbnE,5409
-tests/test_bio_filters.py,sha256=mLvVkv0Nc3OMDgIsMN7tulKt_lkgPdQLBrE4QG34GFk,4637
-tests/test_capacities.py,sha256=RbS2pGZy5h3Vd_tl2h3U6A9nyr-rijpo4kDIMErI7xM,18281
-tests/test_coding.py,sha256=Xjv90plXbMtZjSfpR0g4asoVSwPMQUTFZeBlRQ9vcKI,3632
-tests/test_generating.py,sha256=mwFXlv1qWST4rym79wagBIl1zrhp_A6NNJBePL9KUak,2192
-tests/test_number_vs_binary_message.py,sha256=Ybizmn6FCuxFGvL_TfQquUG0Ifwdb9WbiVrIMLO8iLA,2583
-tests/test_number_vs_dna_string.py,sha256=6-tG7F-hsQAdb12vZzVrBcZcjh9biP1d4vVB6Thapa0,2192
+tests/test_bio_filters.py,sha256=amYDMVd-3juYdUT72z180dfg1vquXiThsRd6iDB1lrY,4828
+tests/test_capacities.py,sha256=8D1c2OuSeRfIXVrOzFnACYHMF2uRfGQn2SrYF1jRIdo,18689
+tests/test_coding.py,sha256=R3K4evcmSGZqXSHD5Rzm2Zchrhsk4R3xdvhH8cm2xNE,4447
+tests/test_generating.py,sha256=v6GQUut7qyLZQWeontgbLA80-JjIn8_sVPlAyQnhW8Y,2214
+tests/test_number_vs_binary_message.py,sha256=joMhAFHANaJBOrg-e2x_4latWf4uHavVjWiOorignxQ,2577
+tests/test_number_vs_dna_sequence.py,sha256=1p3Y2XxRUneoRSWVK7XhZ63iPhBc4gYuVHEEUXSRcQ8,2250
 tests/test_operations.py,sha256=83knvpnNeFwg4edGHQ80LEzKo5l40OxK_9t-ds7h4yU,1864
-tests/test_shuffling.py,sha256=OVSIiaAlvTkgl8lii2RXUTOAuSSo9A_Hxaf5RQ6fjzw,1411
-tests/test_transcoding.py,sha256=Xjv90plXbMtZjSfpR0g4asoVSwPMQUTFZeBlRQ9vcKI,3632
-DNASpiderWeb-1.0.dist-info/LICENSE,sha256=21yJWJR87d4sfXnvyiivkUN1Kf9Y96UpYiaq9ahdKOk,35817
-DNASpiderWeb-1.0.dist-info/METADATA,sha256=81SFO1qalZBrSF33lSFwqiFfi8q-xLjvU_ZYhl9ya08,1700
-DNASpiderWeb-1.0.dist-info/WHEEL,sha256=v8slff5hmCpvciQ3G55d2d1CnOBupjDFJHDE2dUb1Ao,97
-DNASpiderWeb-1.0.dist-info/top_level.txt,sha256=aA1yvxnsQHsXhlfJP05LoJam3n_FKcofzSGcMKz0hYU,10
-DNASpiderWeb-1.0.dist-info/RECORD,,
+tests/test_repair.py,sha256=0kpW9S1nNuAeJQ8UxskQKgkoG6LWxztzmxaWUipkaAk,1623
+tests/test_shuffling.py,sha256=Bu-u0-VyeNYDp9jyoiK7vHauDzPLwbq6sGynAg4OGHA,1413
+DNASpiderWeb-1.1.dist-info/LICENSE.pdf,sha256=sGKjXvlYW_trNeZgzKeW1utWlytsSoYMrAJ06x1qv_Y,541985
+DNASpiderWeb-1.1.dist-info/METADATA,sha256=j9hxz2md5pi9je550jdJpSj2TmjWWMbVPO10OUxgIP4,1602
+DNASpiderWeb-1.1.dist-info/WHEEL,sha256=v8slff5hmCpvciQ3G55d2d1CnOBupjDFJHDE2dUb1Ao,97
+DNASpiderWeb-1.1.dist-info/top_level.txt,sha256=aA1yvxnsQHsXhlfJP05LoJam3n_FKcofzSGcMKz0hYU,10
+DNASpiderWeb-1.1.dist-info/RECORD,,
```

