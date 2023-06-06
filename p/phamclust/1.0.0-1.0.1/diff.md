# Comparing `tmp/phamclust-1.0.0.tar.gz` & `tmp/phamclust-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phamclust-1.0.0.tar", last modified: Thu May  4 20:55:41 2023, max compression
+gzip compressed data, was "phamclust-1.0.1.tar", last modified: Tue Jun  6 18:27:09 2023, max compression
```

## Comparing `phamclust-1.0.0.tar` & `phamclust-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.780450 phamclust-1.0.0/
--rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2023-05-04 20:48:38.000000 phamclust-1.0.0/LICENSE
--rw-r--r--   0 cgauthier   (501) staff       (20)     1051 2023-05-04 20:55:41.780557 phamclust-1.0.0/PKG-INFO
--rw-r--r--   0 cgauthier   (501) staff       (20)       41 2023-05-04 20:48:38.000000 phamclust-1.0.0/README.md
--rw-r--r--   0 cgauthier   (501) staff       (20)       89 2023-05-04 20:48:38.000000 phamclust-1.0.0/pyproject.toml
--rw-r--r--   0 cgauthier   (501) staff       (20)     1178 2023-05-04 20:55:41.781096 phamclust-1.0.0/setup.cfg
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.774297 phamclust-1.0.0/src/
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.778957 phamclust-1.0.0/src/phamclust/
--rw-r--r--   0 cgauthier   (501) staff       (20)       69 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/__init__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)    16864 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/__main__.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     3888 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/blastn.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     5805 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/cli.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     1900 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/clustering.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2409 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/fasta.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     6745 2023-05-04 20:51:42.000000 phamclust-1.0.0/src/phamclust/genome.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2130 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/heatmap.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)    22884 2023-05-04 20:50:58.000000 phamclust-1.0.0/src/phamclust/matrix.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     8292 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/metrics.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     2168 2023-05-04 20:48:38.000000 phamclust-1.0.0/src/phamclust/multiprocess.py
--rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/parallel_process.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     2496 2023-05-04 20:48:38.000000 phamclust-1.0.0/src/phamclust/similarity.py
--rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2023-05-04 20:49:55.000000 phamclust-1.0.0/src/phamclust/statistics.py
-drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-05-04 20:55:41.780259 phamclust-1.0.0/src/phamclust.egg-info/
--rw-r--r--   0 cgauthier   (501) staff       (20)     1051 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/PKG-INFO
--rw-r--r--   0 cgauthier   (501) staff       (20)      596 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/SOURCES.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)        1 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/dependency_links.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)       54 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/entry_points.txt
--rw-r--r--   0 cgauthier   (501) staff       (20)       10 2023-05-04 20:55:41.000000 phamclust-1.0.0/src/phamclust.egg-info/top_level.txt
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-06-06 18:27:09.728974 phamclust-1.0.1/
+-rw-r--r--   0 cgauthier   (501) staff       (20)    35148 2023-05-04 20:48:38.000000 phamclust-1.0.1/LICENSE
+-rw-r--r--   0 cgauthier   (501) staff       (20)     6530 2023-06-06 18:27:09.729139 phamclust-1.0.1/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)     5520 2023-05-05 13:53:50.000000 phamclust-1.0.1/README.md
+-rw-r--r--   0 cgauthier   (501) staff       (20)       89 2023-05-04 20:48:38.000000 phamclust-1.0.1/pyproject.toml
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1178 2023-06-06 18:27:09.730090 phamclust-1.0.1/setup.cfg
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-06-06 18:27:09.716777 phamclust-1.0.1/src/
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-06-06 18:27:09.726561 phamclust-1.0.1/src/phamclust/
+-rw-r--r--   0 cgauthier   (501) staff       (20)       69 2023-05-04 22:50:47.000000 phamclust-1.0.1/src/phamclust/__init__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)    16719 2023-06-06 18:26:19.000000 phamclust-1.0.1/src/phamclust/__main__.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     3888 2023-05-04 22:50:47.000000 phamclust-1.0.1/src/phamclust/blastn.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     5852 2023-05-23 15:23:35.000000 phamclust-1.0.1/src/phamclust/cli.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     1897 2023-05-23 14:48:37.000000 phamclust-1.0.1/src/phamclust/clustering.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2408 2023-05-23 14:48:43.000000 phamclust-1.0.1/src/phamclust/fasta.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     6744 2023-05-23 14:48:50.000000 phamclust-1.0.1/src/phamclust/genome.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2130 2023-05-04 22:50:47.000000 phamclust-1.0.1/src/phamclust/heatmap.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)    23872 2023-05-23 14:49:22.000000 phamclust-1.0.1/src/phamclust/matrix.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     8460 2023-05-23 14:50:26.000000 phamclust-1.0.1/src/phamclust/metrics.py
+-rwxr-xr-x   0 cgauthier   (501) staff       (20)     2630 2023-05-04 22:50:47.000000 phamclust-1.0.1/src/phamclust/parallel_process.py
+-rw-r--r--   0 cgauthier   (501) staff       (20)     2831 2023-05-04 22:50:47.000000 phamclust-1.0.1/src/phamclust/statistics.py
+drwxr-xr-x   0 cgauthier   (501) staff       (20)        0 2023-06-06 18:27:09.728633 phamclust-1.0.1/src/phamclust.egg-info/
+-rw-r--r--   0 cgauthier   (501) staff       (20)     6530 2023-06-06 18:27:09.000000 phamclust-1.0.1/src/phamclust.egg-info/PKG-INFO
+-rw-r--r--   0 cgauthier   (501) staff       (20)      538 2023-06-06 18:27:09.000000 phamclust-1.0.1/src/phamclust.egg-info/SOURCES.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)        1 2023-06-06 18:27:09.000000 phamclust-1.0.1/src/phamclust.egg-info/dependency_links.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)       54 2023-06-06 18:27:09.000000 phamclust-1.0.1/src/phamclust.egg-info/entry_points.txt
+-rw-r--r--   0 cgauthier   (501) staff       (20)       10 2023-06-06 18:27:09.000000 phamclust-1.0.1/src/phamclust.egg-info/top_level.txt
```

### Comparing `phamclust-1.0.0/LICENSE` & `phamclust-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phamclust-1.0.0/setup.cfg` & `phamclust-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_files = LICENSE
 name = phamclust
-version = 1.0.0
+version = 1.0.1
 author = Christian Gauthier
 author_email = chg60@pitt.edu
 description = Cluster genomes based on gene phamily data
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/chg60/phamclust
 project_urls =
```

### Comparing `phamclust-1.0.0/src/phamclust/__main__.py` & `phamclust-1.0.1/src/phamclust/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             row = row.rstrip().split()
 
             if len(row) == 3:
                 name, pham, translation = row
             elif len(row) == 2:
                 (name, pham), translation = row, "M"
             else:
-                raise ValueError(f"input file must either 2 or 3 columns")
+                raise ValueError("input file must either 2 or 3 columns")
 
             if name not in genomes:
                 genomes[name] = Genome(name)
 
             genomes[name].add(pham, translation)
 
     return genomes
@@ -168,33 +168,31 @@
     nr_dist:    float = round(1.0 - args.nr_thresh, 6)      # cast to distance
     sub_linkage:  str = args.sub_linkage
     clu_linkage:  str = args.clu_linkage
     nr_linkage:   str = args.nr_linkage
     k_min:        int = max([1, args.k_min])
     metric:       str = args.metric
     cpus:         int = args.threads
-    # TODO: add argument to handle subcluster strategy ('all', 'core', 'cloud')
-    sub_strategy: str = "all"
 
     # Sanity check - if nr_dist not lower than clu_dist, use 0.0
     if nr_dist >= clu_dist:
         nr_dist = 0.0
 
     # Set logging context and log runtime parameters
     logfile = outdir.joinpath("phamclust.log")
     log_level = logging.INFO
     if debug:
         log_level = logging.DEBUG
     logging.basicConfig(filename=logfile, filemode="w", level=log_level,
                         format=LOG_STR_FMT, datefmt=LOG_TIME_FMT)
     logging.getLogger().addHandler(logging.StreamHandler(sys.stdout))
 
-    logging.info(f"=======================")
-    logging.info(f" 0: runtime parameters ")
-    logging.info(f"=======================")
+    logging.info("=======================")
+    logging.info(" 0: runtime parameters ")
+    logging.info("=======================")
     logging.info(f"infile:     {infile}")
     logging.info(f"outdir:     {outdir}")
     logging.info(f"debug:      {debug}")
     logging.info(f"subcluster: {not no_sub}")
     logging.info(f"remove tmp: {rm_tmp}")
     logging.info(f"sub dist:   {sub_dist}")
     logging.info(f"sub link:   {sub_linkage}")
@@ -202,17 +200,17 @@
     logging.info(f"clu link:   {clu_linkage}")
     logging.info(f"nr dist:    {nr_dist}")
     logging.info(f"nr link:    {nr_linkage}")
     logging.info(f"metric:     {metric}")
     logging.info(f"cpus:       {cpus}")
 
     # Parse genomes from TSV-formatted infile
-    logging.info(f"====================")
-    logging.info(f" 1: parsing genomes ")
-    logging.info(f"====================")
+    logging.info("====================")
+    logging.info(" 1: parsing genomes ")
+    logging.info("====================")
     if expect_dir:
         genomes = load_genomes_from_fasta_dir(infile)
         logging.info(f"loaded {len(genomes)} genomes from input directory")
     else:
         genomes = load_genomes_from_tsv(infile)
         logging.info(f"loaded {len(genomes)} genomes from input TSV")
     hashsum = hash_genomes(genomes)
@@ -221,79 +219,79 @@
     # Create temporary directory (or re-use) from genome hashsum
     tmpdir = outdir.joinpath(f"{hashsum}.tmp")
     if not tmpdir.is_dir():
         tmpdir.mkdir()
     logging.info(f"using temp directory {tmpdir.name}")
 
     # Write genomes to temporary directory as FASTA
-    tmp_genomes = tmpdir.joinpath(f"01_genomes")
+    tmp_genomes = tmpdir.joinpath("01_genomes")
     if not tmp_genomes.is_dir():
         tmp_genomes.mkdir()
 
     for name, genome in genomes.items():
         genome_fasta = tmp_genomes.joinpath(f"{name}.fasta")
         if not genome_fasta.is_file():
             genome.save(genome_fasta)
 
     logging.info(f"genomes stashed in {tmpdir.name}/{tmp_genomes.name}")
 
     # Always recycle pairwise matrices if available
-    logging.info(f"==========================")
-    logging.info(f" 2: build distance matrix ")
-    logging.info(f"==========================")
+    logging.info("==========================")
+    logging.info(" 2: build distance matrix ")
+    logging.info("==========================")
     logging.info(f"selected metric: {metric}")
 
     # Write distance matrix to temporary directory as FASTA
-    tmp_distmats = tmpdir.joinpath(f"02_distmats")
+    tmp_distmats = tmpdir.joinpath("02_distmats")
     if not tmp_distmats.is_dir():
         tmp_distmats.mkdir()
 
     dist_mat_file = tmp_distmats.joinpath(f"{metric}_distance_matrix.tsv")
     if not dist_mat_file.is_file():
-        logging.info(f"cached distance matrix not found - computing de novo")
+        logging.info("cached distance matrix not found - computing de novo")
         _start = datetime.datetime.now()
         dist_mat = matrix_de_novo(genomes, METRICS[metric], cpus)
         _elapsed = datetime.datetime.now() - _start
         logging.info(f"computed distance matrix in {str(_elapsed)}")
-        logging.info(f"caching distance matrix so it can be re-used")
+        logging.info("caching distance matrix so it can be re-used")
         matrix_to_squareform(dist_mat, dist_mat_file, lower_triangle=True)
     else:
-        logging.info(f"found cached distance matrix - importing it")
+        logging.info("found cached distance matrix - importing it")
         _start = datetime.datetime.now()
         dist_mat = matrix_from_squareform(dist_mat_file)
         _elapsed = datetime.datetime.now() - _start
         logging.info(f"loaded distance matrix in {str(_elapsed)}")
 
     # Make sure the matrix is a distance matrix
     if not dist_mat.is_distance:
-        logging.info(f"matrix is not a distance matrix - flipping it")
+        logging.info("matrix is not a distance matrix - flipping it")
         dist_mat.invert()
 
     # Check matrix integrity
     status = check_matrix_integrity(dist_mat)
     if not any(status):
-        logging.info(f"matrix passed all integrity checks")
+        logging.info("matrix passed all integrity checks")
     else:
-        logging.error(f"matrix failed the following integrity check(s):")
+        logging.error("matrix failed the following integrity check(s):")
         if status[0] > 0:
             logging.error(f"found {status[0]} too many edges")
         elif status[0] < 0:
             logging.error(f"found {0 - status[0]} too few edges")
         if status[1] != 0:
             logging.error(f"diagonal sum {status[0]} is wrong")
         if status[2] != 0:
             logging.error(f"found {status[2]} unfilled edges")
 
         print(f"matrix validation failed - check '{logfile}' for details")
         sys.exit(1)
 
     # If we got here, matrix is OK - begin clustering
-    logging.info(f"====================")
-    logging.info(f" 3: cluster genomes ")
-    logging.info(f"====================")
+    logging.info("====================")
+    logging.info(" 3: cluster genomes ")
+    logging.info("====================")
     logging.info(f"grouping highly redundant genomes with distance <= "
                  f"{nr_dist} by {nr_linkage} linkage")
     # Seed clusters with groups of phages that have low levels of divergence
     clu_mats = hierarchical(dist_mat, eps=nr_dist, linkage=nr_linkage)
 
     # Map the seed cluster representatives to their clusters
     seed_map = {x.medoid[0]: x for x in clu_mats}
@@ -312,22 +310,22 @@
 
     single_mats = [clu_mat for clu_mat in clu_mats if len(clu_mat) == 1]
     clu_mats = [clu_mat for clu_mat in clu_mats if len(clu_mat) > 1]
     logging.info(f"found {len(clu_mats)} clusters and {len(single_mats)} "
                  f"singletons")
 
     # Write genomes to temporary directory as FASTA
-    tmp_clusters = tmpdir.joinpath(f"03_clusters")
+    tmp_clusters = tmpdir.joinpath("03_clusters")
     if not tmp_clusters.is_dir():
         tmp_clusters.mkdir()
 
     # Begin sub-clustering
-    logging.info(f"========================")
-    logging.info(f" 4: sub-cluster genomes ")
-    logging.info(f"========================")
+    logging.info("========================")
+    logging.info(" 4: sub-cluster genomes ")
+    logging.info("========================")
     for i, clu_mat in enumerate(sorted(clu_mats, reverse=True)):
         logging.info(f"cluster {i + 1} has {len(clu_mat)} nodes")
 
         # Make a toplevel directory for this cluster
         cluster_dir = tmp_clusters.joinpath(f"cluster_{i+1}")
         if cluster_dir.is_dir():
             logging.debug(f"removing old cluster directory {cluster_dir}")
@@ -339,15 +337,15 @@
         cluster_nodes = sorted(clu_mat.nodes)
         cluster_genomes = [genomes[name] for name in cluster_nodes]
         cluster_matfile = cluster_dir.joinpath(f"{metric}_similarity.tsv")
         cluster_heatmap = cluster_dir.joinpath(f"{metric}_heatmap.pdf")
         cluster_heatmap2 = cluster_dir.joinpath(f"{metric}_heatmap.html")
 
         # Make a genome directory for this cluster, move genome files here
-        genome_dir = cluster_dir.joinpath(f"genomes")
+        genome_dir = cluster_dir.joinpath("genomes")
         genome_dir.mkdir()
         for genome in cluster_genomes:
             genome_file = genome_dir.joinpath(f"{genome.name}.faa")
             genome.save(genome_file)
             logging.debug(f"wrote genome to {genome_file}")
 
         if no_sub or len(clu_mat) < k_min:
@@ -367,29 +365,29 @@
             sub_mats = hierarchical(clu_mat, eps=sub_dist, linkage=sub_linkage)
             sub_mats = sorted(sub_mats, reverse=True)
             order = list()
             for j, sub_mat in enumerate(sub_mats):
                 sub_matfile = cluster_dir.joinpath(
                     f"subcluster_{j+1}_similarity.tsv")
                 _ord = [sub_mat.medoid[0]]
-                _ord.extend(sub_mat.nearest_neighbors(_ord[0], threshold=0.0))
+                _ord.extend(sub_mat.nearest_neighbors(_ord[0], threshold=1.0))
                 order.extend(_ord)
                 sub_mat.reorder(_ord)
                 sub_mat.invert()
                 matrix_to_squareform(sub_mat, sub_matfile)
             clu_mat.reorder(order)
             clu_mat.invert()
             matrix_to_squareform(clu_mat, cluster_matfile)
             draw_heatmap(clu_mat, midpoint=0.5, filename=cluster_heatmap)
             draw_heatmap(clu_mat, midpoint=0.5, filename=cluster_heatmap2)
             continue
 
     # Make a toplevel directory for singletons, with nested genome dir
     if single_mats:
-        single_dir = tmp_clusters.joinpath(f"singletons")
+        single_dir = tmp_clusters.joinpath("singletons")
         if single_dir.is_dir():
             logging.debug(f"removing old singleton directory {single_dir}")
             shutil.rmtree(single_dir)
 
         logging.debug(f"creating new singleton directory {single_dir}")
         single_dir.mkdir()
         genome_dir = single_dir.joinpath("genomes")
@@ -400,37 +398,37 @@
             genome = genomes[node]
 
             genome_file = genome_dir.joinpath(f"{genome.name}.faa")
             genome.save(genome_file)
             logging.debug(f"wrote genome to {genome_file}")
 
     # Write full dataset heatmap
-    logging.info(f"========================")
-    logging.info(f" 5: draw dataset heatmap")
-    logging.info(f"========================")
-    logging.info(f"putting matrix in cluster order")
+    logging.info("========================")
+    logging.info(" 5: draw dataset heatmap")
+    logging.info("========================")
+    logging.info("putting matrix in cluster order")
     dataset_order = list()
     for clu_mat in sorted(clu_mats, reverse=True):
         dataset_order.extend(clu_mat.nodes)
     for single_mat in single_mats:
         dataset_order.extend(single_mat.nodes)
 
     dataset_heatmap = tmp_clusters.joinpath(f"{metric}_heatmap.html")
     dist_mat.reorder(dataset_order)
 
-    logging.info(f"convert to similarity matrix for easier visualization")
+    logging.info("convert to similarity matrix for easier visualization")
     dist_mat.invert()
 
     logging.info(f"drawing heatmap and saving to {dataset_heatmap.name}")
     draw_heatmap(dist_mat, midpoint=0.5, filename=dataset_heatmap)
 
     # Copy output files to output directory
-    logging.info(f"========================")
-    logging.info(f" 6: move output files   ")
-    logging.info(f"========================")
+    logging.info("========================")
+    logging.info(" 6: move output files   ")
+    logging.info("========================")
     # if outdir.is_dir():
     #     logging.info(f"removing existing output directory {outdir}")
     #     shutil.rmtree(outdir)
 
     logging.info(f"moving output files from temporary directory to {outdir}")
     shutil.copytree(tmp_clusters, outdir, dirs_exist_ok=True)
```

### Comparing `phamclust-1.0.0/src/phamclust/blastn.py` & `phamclust-1.0.1/src/phamclust/blastn.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.0.0/src/phamclust/cli.py` & `phamclust-1.0.1/src/phamclust/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Cluster phage genomes using gene content similarity-based metrics."""
 
 import argparse
 import pathlib
 from psutil import virtual_memory, cpu_count
 
-from phamclust.metrics import *
+from phamclust import metrics
 
 
 def recommended_cpus(main=4.0, per_core=1.0):
     """Calculate how many cores can be safely used without straining
     the system.
 
     Defaults are calibrated against a large matrix.
 
-    A system with 8 cores and 12 GB available memory will recommend
-    using 8 cores.
+    A system with 8 cores and at least 12 GB available memory will
+    recommend using 8 cores.
 
     :param main: assumed memory needed for the main process
     :type main: float
     :param per_core: assumed memory needed for each child process
     :type per_core: float
     :return: cpus
     """
@@ -47,20 +47,20 @@
 https://doi.org/10.1093/nar/gkv657
 (5) aai         average aminoacid identity          \
 https://doi.org/10.1073/pnas.0409727102
 (6) peq         proteomic equivalence quotient      \
 Gauthier & Hatfull, 2023
 """
 LINKAGES = {"single", "average", "complete"}
-METRICS = {"gcs": gene_content_similarity,
-           "jc": jaccard_coefficient,
-           "pocp": percentage_of_conserved_proteins,
-           "af": alignment_fraction,
-           "aai": average_aminoacid_identity,
-           "peq": proteomic_equivalence_quotient}
+METRICS = {"gcs": metrics.gene_content_similarity,
+           "jc": metrics.jaccard_coefficient,
+           "pocp": metrics.percentage_of_conserved_proteins,
+           "af": metrics.alignment_fraction,
+           "aai": metrics.average_aminoacid_identity,
+           "peq": metrics.proteomic_equivalence_quotient}
 K_MIN = 6                       # Minimum size of cluster to sub-cluster
 METRIC = "peq"                  # Default metric
 NR_THRESH = 0.75                # Default 1st iteration cluster threshold
 NR_LINKAGE = "complete"         # Default 1st iteration cluster linkage
 CLU_THRESH = 0.25               # Default 2nd iteration cluster threshold
 CLU_LINKAGE = "average"         # Default 2nd iteration cluster linkage
 SUB_THRESH = 0.6                # Default subclustering threshold
@@ -70,21 +70,21 @@
 def parse_args():
     """Parse commandline arguments."""
     p = argparse.ArgumentParser(prog="phamclust",
                                 description=__doc__, epilog=EPILOG,
                                 formatter_class=argparse.RawTextHelpFormatter)
 
     p.add_argument("infile", type=pathlib.Path,
-                   help=f"path to a TSV file mapping genomes to phams and "
-                        f"translations")
+                   help="path to a TSV file mapping genomes to phams and "
+                        "translations")
     p.add_argument("outdir", type=pathlib.Path,
-                   help=f"path to which output files should be written")
+                   help="path to which output files should be written")
     p.add_argument("-g", "--genome-dir", action="store_true",
-                   help=f"interpret `infile` as a directory of genome FASTA "
-                        f"files instead of TSV")
+                   help="interpret `infile` as a directory of genome FASTA "
+                        "files instead of TSV")
 
     c = p.add_argument_group("clustering arguments:")
     c.add_argument("-k", "--k-min",
                    type=int, default=K_MIN, metavar="",
                    help=f"minimum cluster size to perform subclustering "
                         f"[default: {K_MIN}]")
     c.add_argument("-s", "--sub-thresh",
@@ -113,18 +113,18 @@
                    help=f"linkage type to use for pre-grouping very similar "
                         f"genomes [default: {NR_LINKAGE}]")
     c.add_argument("-m", "--metric",
                    type=str, choices=METRICS, default=METRIC, metavar="",
                    help=f"relatedness index to use for pairwise genome "
                         f"comparisons [default: {METRIC}]")
     p.add_argument("-d", "--debug", action="store_true",
-                   help=f"increase verbosity of logging for debug purposes")
+                   help="increase verbosity of logging for debug purposes")
     p.add_argument("-n", "--no-sub", action="store_true",
                    help="do not perform sub-clustering")
     p.add_argument("-r", "--remove-tmp", action="store_true",
-                   help=f"remove temporary files (not recommended if repeated "
-                        f"runs are planned on the same dataset)")
+                   help="remove temporary files (not recommended if repeated "
+                        "runs are planned on the same dataset)")
     p.add_argument("-t", "--threads",
                    type=int, default=CPUS, metavar="",
                    help=f"number of CPU cores to use [default: {CPUS}]")
 
     return p.parse_args()
```

### Comparing `phamclust-1.0.0/src/phamclust/clustering.py` & `phamclust-1.0.1/src/phamclust/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     :return: clusters
     """
     if len(matrix) == 1:
         return [matrix]
 
     # Export distance matrix
     if not matrix.is_distance:
-        raise ValueError(f"matrix must be a distance matrix")
+        raise ValueError("matrix must be a distance matrix")
     dist_mat = matrix.to_ndarray()
 
     if eps is None and not n_clusters:
-        raise ValueError(f"need either threshold or n_clusters to proceed")
+        raise ValueError("need either threshold or n_clusters to proceed")
     elif eps and n_clusters:
-        raise ValueError(f"threshold and n_clusters are mutually exclusive")
+        raise ValueError("threshold and n_clusters are mutually exclusive")
 
     # Build the clustering object using indicated eps/n_clusters
     c = AgglomerativeClustering(metric="precomputed", linkage=linkage,
                                 distance_threshold=eps, n_clusters=n_clusters)
 
     temp_clusters = dict()
     for node_name, label in zip(matrix.nodes, c.fit_predict(dist_mat)):
```

### Comparing `phamclust-1.0.0/src/phamclust/fasta.py` & `phamclust-1.0.1/src/phamclust/fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         # Read the first line
         line = next(fasta_reader)
 
         # Iterate until EOF
         while True:
             # Parse the header
             if line[0] != ">":
-                raise ValueError(f"records in FASTA files must start with '>'")
+                raise ValueError("records in FASTA files must start with '>'")
             header = line[1:].rstrip()
 
             # Parse the sequence
             sequence = list()
             for line in fasta_reader:
                 if line[0] == ">":
                     break   # ">" tells us we are moving to the next record
```

### Comparing `phamclust-1.0.0/src/phamclust/genome.py` & `phamclust-1.0.1/src/phamclust/genome.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             for field in header.split("|"):
                 key, value = field.split("=")
                 if key == "pham":
                     pham = value
                     break
 
             if pham is None:
-                raise GenomeLoadError(f"unable to get pham from FASTA header")
+                raise GenomeLoadError("unable to get pham from FASTA header")
 
             self.add(pham, translation)
 
     def pop(self, pham):
         """Remove and return a pham from this genome.
 
         :param pham: name of the pham to remove
```

### Comparing `phamclust-1.0.0/src/phamclust/heatmap.py` & `phamclust-1.0.1/src/phamclust/heatmap.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.0.0/src/phamclust/matrix.py` & `phamclust-1.0.1/src/phamclust/matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def diameter(self):
         """Return the cluster diameter (the longest edge weight).
 
         Because diameter is inherently a measure of distance, a
         ValueError will be raised if invoked for a similarity matrix.
         """
         if not self.is_distance:
-            raise ValueError(f"cannot compute diameter for similarity matrix")
+            raise ValueError("cannot compute diameter for similarity matrix")
 
         diameter = 0.0
 
         for source, target, weight in self:
             if source != target and weight > diameter:
                 diameter = weight
 
@@ -390,15 +390,15 @@
 
 # SymMatrix de novo
 def _calculate_batch_adjacency(genomes, pairs, func, as_distance=True):
     """Calculate the similarity between source and target genomes using
     `func`.
 
     :param genomes: all genomes in the dataset
-    :type genomes: dict[str, phamclust.Genome.Genome]
+    :type genomes: dict[str, phamclust.genome.Genome]
     :param pairs: list of (source, target) pairs to compute
     :type pairs: list[tuple[str, str]]
     :param func: similarity function to use for genome comparisons
     :type func: function
     :param as_distance: calculate distances rather than similarities
     :type as_distance: bool
     """
@@ -412,100 +412,123 @@
             weight = func(source, target, as_distance)
 
         adjacency.append((source_name, target_name, weight))
 
     return adjacency
 
 
-def _calculate_adjacency(genomes, func, as_distance=True):
+def _calculate_adjacency(pair, func, as_distance=True):
     """Calculate the similarity between source and target genomes using
     `func`.
 
-    :param genomes: all genomes in the dataset
-    :type genomes: dict[str, phamclust.Genome.Genome]
+    :param pair: genome pair to be evaluated using `func`
+    :type pair: tuple[phamclust.genome.Genome, phamclust.genome.Genome]]
     :param func: similarity function to use for genome comparisons
     :type func: function
     :param as_distance: calculate distances rather than similarities
     :type as_distance: bool
     """
-    adjacency = list()
-    nodes, jobs = list(genomes.keys()), list()
-    for i, source_name in enumerate(nodes):
-        source = genomes[source_name]
-        for target_name in nodes[i:]:
-            target = genomes[target_name]
-            weight = func(source, target, as_distance)
-
-            adjacency.append((source_name, target_name, weight))
-
-    return adjacency
-
+    source, target = pair
+    return source.name, target.name, func(source, target, as_distance)
 
-def matrix_de_novo(genomes, func, cpus, as_distance=True):
-    """Create a symmetric matrix from scratch using `func` to measure
-    the similarity between genomes.
-
-    Developer note: this list[Genome]-based implementation has similar
-    memory footprint to the previous dict[str, Genome]-based approach,
-    but is ~25-30% faster.
-
-    :param genomes: the genomes to build a matrix from
-    :type genomes: dict[str, phamclust.Genome.Genome]
-    :param func: similarity function to use for genome comparisons
-    :type func: function
-    :param cpus: number of CPU cores to use for matrix-building
-    :type cpus: int
-    :param as_distance: populate matrix with distance, not similarity
-    :type as_distance: bool
-    :return: matrix
-    """
-    # >>> Begin sanity checks >>>
-    if len(genomes) == 0:
-        raise ValueError(f"need at least 1 genome to construct matrix de novo")
 
+def calc_adjacency_scheme_1(genomes, func, cpus, as_distance=True):
     # Calculate the number of unique genome pairs
     n_pairs = int((len(genomes) * (len(genomes) - 1) / 2) + len(genomes))
     logging.debug(f"{len(genomes)} genomes -> {n_pairs} edges including "
                   f"diagonal")
 
     # If fewer genome pairs than CPUs, set CPU count to number of genome pairs
     if n_pairs < cpus:
         logging.info(f"small dataset - reducing # CPUs to {n_pairs}")
         cpus = n_pairs
 
     n_batches = min((1, n_pairs // cpus))
     while n_batches % cpus != 0:
         n_batches += 1
 
-    # <<< End sanity checks <<<
-
-    # >>> Begin creating & running jobs >>>
     jobs = list()
     for _ in range(n_batches):
         jobs.append(list())
 
     nodes = sorted(genomes.keys())
     for i, pair in enumerate(combinations_with_replacement(nodes, 2)):
         job_idx = i % n_batches
         jobs[job_idx].append(pair)
 
     for i in range(n_batches):
         jobs[i] = (genomes, jobs[i], func, as_distance)
 
-    adjacency_data = parallelize(_calculate_batch_adjacency, jobs, cpus)
+    return parallelize(_calculate_batch_adjacency, jobs, cpus)
+
+
+def calc_adjacency_scheme_2(genomes, func, cpus, as_distance=True):
+    # Calculate the number of unique genome pairs
+    n_pairs = int((len(genomes) * (len(genomes) - 1) / 2) + len(genomes))
+    logging.debug(f"{len(genomes)} genomes -> {n_pairs} edges including "
+                  f"diagonal")
+
+    # If fewer genome pairs than CPUs, set CPU count to number of genome pairs
+    if n_pairs < cpus:
+        logging.info(f"tiny dataset - reducing # CPUs to {n_pairs}")
+        cpus = n_pairs
+
+    jobs, adjacency = list(), list()
+    genome_list = [y for x, y in sorted(genomes.items(), key=lambda x: x[0])]
+    for i, pair in enumerate(combinations_with_replacement(genome_list, 2)):
+        # Dispatch jobs in batches of len(genomes)
+        if i != 0 and i % len(genomes) == 0:
+            adjacency.extend(parallelize(_calculate_adjacency, jobs, cpus))
+            jobs = [(pair, func, as_distance)]
+        else:
+            jobs.append((pair, func, as_distance))
+
+    # Dispatch any remaining jobs
+    if len(jobs) > 0:
+        adjacency.extend(parallelize(_calculate_adjacency, jobs, cpus))
+
+    return adjacency
+
+
+def matrix_de_novo(genomes, func, cpus, as_distance=True):
+    """Create a symmetric matrix from scratch using `func` to measure
+    the similarity between genomes.
+
+    Developer note: this list[Genome]-based implementation has similar
+    memory footprint to the previous dict[str, Genome]-based approach,
+    but is ~25-30% faster.
+
+    :param genomes: the genomes to build a matrix from
+    :type genomes: dict[str, phamclust.Genome.Genome]
+    :param func: similarity function to use for genome comparisons
+    :type func: function
+    :param cpus: number of CPU cores to use for matrix-building
+    :type cpus: int
+    :param as_distance: populate matrix with distance, not similarity
+    :type as_distance: bool
+    :return: matrix
+    """
+    # >>> Begin sanity checks >>>
+    if len(genomes) == 0:
+        raise ValueError("need at least 1 genome to construct matrix de novo")
+
+    # <<< End sanity checks <<<
+
+    adjacency_data = calc_adjacency_scheme_2(genomes, func, cpus, as_distance)
     # adjacency_data = _calculate_adjacency(genomes, func, as_distance)
     # <<< End creating & running jobs <<<
 
     # <<< Initialize the matrix >>>
+    nodes = sorted(genomes.keys())
     matrix = SymMatrix(nodes=nodes, is_distance=as_distance)
 
     # >>> Begin populating the matrix from adjacency data >>>
-    for adjacency_batch in adjacency_data:
-        for source, target, weight in adjacency_batch:
-            matrix.set_weight(source, target, weight)
+    # for adjacency_batch in adjacency_data:
+    for source, target, weight in adjacency_data:
+        matrix.set_weight(source, target, weight)
 
     # <<< End populating the matrix from adjacency data <<<
 
     return matrix
 
 
 # Adjacency matrix I/O
@@ -537,23 +560,23 @@
 
         names[target] = None
 
     names = list(names.keys())
 
     # Analyze diagonal: all values should be the same
     if len(diagonal) > 1:
-        raise ValueError(f"values on matrix diagonal should be identical")
+        raise ValueError("values on matrix diagonal should be identical")
 
     # Analyze diagonal: should be either 0.0 (distance) or 1.0 (similarity)
     if sum(diagonal) == 0.0:
         is_distance = True
     elif sum(diagonal) == 1.0:
         is_distance = False
     else:
-        raise ValueError(f"values on matrix diagonal can only be 0.0 or 1.0")
+        raise ValueError("values on matrix diagonal can only be 0.0 or 1.0")
 
     # Create the matrix
     matrix = SymMatrix(names, is_distance=is_distance)
     for source, target, weight in read_adjacency(filepath):
         matrix.set_weight(source, target, weight)
 
     return matrix
@@ -609,23 +632,23 @@
     names, diagonal = list(), set()
     for i, (target, row) in enumerate(read_squareform(filepath)):
         names.append(target)
         diagonal.add(row[i])
 
     # Analyze diagonal: all values should be the same
     if len(diagonal) > 1:
-        raise ValueError(f"values on matrix diagonal should be identical")
+        raise ValueError("values on matrix diagonal should be identical")
 
     # Analyze diagonal: should be either 0.0 (distance) or 1.0 (similarity)
     if sum(diagonal) == 0.0:
         is_distance = True
     elif sum(diagonal) == 1.0:
         is_distance = False
     else:
-        raise ValueError(f"values on matrix diagonal can only be 0.0 or 1.0")
+        raise ValueError("values on matrix diagonal can only be 0.0 or 1.0")
 
     # Create the matrix
     matrix = SymMatrix(names, is_distance=is_distance)
     for i, (target, row) in enumerate(read_squareform(filepath)):
         for (source, weight) in zip(names[:i + 1], row[:i + 1]):
             matrix.set_weight(source, target, weight)
```

### Comparing `phamclust-1.0.0/src/phamclust/metrics.py` & `phamclust-1.0.1/src/phamclust/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 
 All metrics can be optionally returned as distances rather than
 similarities.
 """
 
 from parasail import blosum62, nw_trace_diag_16
 
-from phamclust.genome import Genome
 from phamclust.statistics import average
 
 
 def gene_content_similarity(source, target, as_distance=False):
     """Calculate the gene content similarity between the given source
     and target genomes, as described in Mavrich and Hatfull (2017).
 
     DOI: https://doi.org/10.1038/nmicrobiol.2017.112.
 
     :param source: the source genome to be compared
-    :type source: Genome
+    :type source: phamclust.genome.Genome
     :param target: the target genome to be compared
-    :type target: Genome
+    :type target: phamclust.genome.Genome
     :param as_distance: return distance instead of similarity
     :type as_distance: bool
     :return: similarity
     """
     shared_phams = source.intersection(target)
 
     if not shared_phams:
@@ -56,17 +55,17 @@
 def jaccard_coefficient(source, target, as_distance=False):
     """Calculate the jaccard similarity coefficient between the given
     source and target genomes, as described in Jaccard (1912).
 
     DOI: https://doi.org/10.1111/j.1469-8137.1912.tb05611.x.
 
     :param source: the source genome to be compared
-    :type source: Genome
+    :type source: phamclust.genome.Genome
     :param target: the target genome to be compared
-    :type target: Genome
+    :type target: phamclust.genome.Genome
     :param as_distance: return distance instead of similarity
     :type as_distance: bool
     :return: similarity
     """
     shared_phams = source.intersection(target)
 
     if not shared_phams:
@@ -83,17 +82,17 @@
 def percentage_of_conserved_proteins(source, target, as_distance=False):
     """Calculate the percentage of conserved proteins between the
     given source and target genomes, as described in Qin et al. (2014).
 
     DOI: https://doi.org/10.1128/JB.01688-14.
 
     :param source: the source genome to be compared
-    :type source: Genome
+    :type source: phamclust.genome.Genome
     :param target: the target genome to be compared
-    :type target: Genome
+    :type target: phamclust.genome.Genome
     :param as_distance: return distance instead of similarity
     :type as_distance: bool
     :return: similarity
     """
     shared_phams = source.intersection(target)
 
     if not shared_phams:
@@ -116,17 +115,17 @@
 
 
 def alignment_fraction(source, target, as_distance=False):
     """Calculate the percentage of conserved proteins between the given
     source and target genomes, weighted by gene size.
 
     :param source: the source genome to be compared
-    :type source: Genome
+    :type source: phamclust.genome.Genome
     :param target: the target genome to be compared
-    :type target: Genome
+    :type target: phamclust.genome.Genome
     :param as_distance: return distance instead of similarity
     :type as_distance: bool
     :return: similarity
     """
     shared_phams = source.intersection(target)
 
     if not shared_phams:
@@ -180,17 +179,17 @@
     genomes by computing the length-weighted amino acid identity
     between genes in phams shared by the genomes.
 
     Use `positive=True` to return the average amino acid similarity
     instead of identity.
 
     :param source: the source genome to be compared
-    :type source: Genome
+    :type source: phamclust.genome.Genome
     :param target: the target genome to be compared
-    :type target: Genome
+    :type target: phamclust.genome.Genome
     :param as_distance: return distance instead of similarity
     :type as_distance: bool
     :param ppos: calculate percent positive instead of identical
     :type ppos: bool
     :return: similarity
     """
     shared_phams = source.intersection(target)
@@ -233,17 +232,17 @@
 
 
 def proteomic_equivalence_quotient(source, target, as_distance=False):
     """Compute the proteomic equivalence quotient between a pair of
     genomes.
 
     :param source: the source genome to be compared
-    :type source: Genome
+    :type source: phamclust.genome.Genome
     :param target: the target genome to be compared
-    :type target: Genome
+    :type target: phamclust.genome.Genome
     :param as_distance: return distance instead of similarity
     :type as_distance: bool
     :return: similarity
     """
     similarity = alignment_fraction(source, target)
     similarity *= average_aminoacid_identity(source, target)
```

### Comparing `phamclust-1.0.0/src/phamclust/multiprocess.py` & `phamclust-1.0.1/src/phamclust/parallel_process.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,81 +3,91 @@
 the caller."""
 
 import multiprocessing
 
 CPUS = multiprocessing.cpu_count()
 
 
-def parallelize(inputs, cpus, func):
+def parallelize(task, inputs, cpus):
     """Parallelize some task on an input list across the specified
     number of CPU cores.
 
-    :param inputs: arguments to call `func` with
-    :type inputs: list
-    :param cpus: number of CPU cores to use
+    :param task: name of the function to run
+    :type task: function
+    :param inputs: arguments to call `task` with
+    :type inputs: list or list[tuple]
+    :param cpus: number of processor cores to use
     :type cpus: int
-    :param func: function to call in parallel
-    :type func: function
-    :return: results
     """
-    # Return early if called with no inputs
+    results = []
+
+    # Don't do any work if there are no inputs
     if len(inputs) == 0:
-        return list()
+        return results
 
-    # User requested some number of cores - make sure it's sane
-    if cpus < 1 or cpus > CPUS:
-        cpus = min([CPUS, len(inputs)])
+    # User requested some number of CPUS - ensure it is sane.
+    # Then, reduce to match len(inputs) if fewer than CPUS.
+    if not 1 <= cpus <= CPUS:
+        cpus = CPUS
+    cpus = min([cpus, len(inputs)])
 
     tasks = []
     for item in inputs:
         if not isinstance(item, tuple):
             item = (item,)
-        tasks.append((func, item))
+        tasks.append((task, item))
 
-    return start_processes(tasks, cpus)
+    # Start working on the jobs
+    results = start_processes(tasks, cpus)
+
+    return results
 
 
 def worker(input_queue, output_queue):
     """Worker function to run jobs from the input queue until a stop
     signal is reached.
 
-    :param input_queue: thread-safe queue to pull jobs from
-    :type input_queue: multiprocessing.Queue
-    :param output_queue: thread-safe queue to add results to
+    :param input_queue: the tasks to run
+    :type input_queue: multiprocessing.Queue[tuple[function, tuple]]
+    :param output_queue: where to put results returned by each task
     :type output_queue: multiprocessing.Queue
     """
-    for func, args in iter(input_queue.get, "STOP"):
-        result = func(*args)
-        if result:
-            output_queue.put(result)
+    for func, args in iter(input_queue.get, 'STOP'):
+        output_queue.put(func(*args))
 
 
 def start_processes(inputs, cpus):
-    """Spool up processes and use them to run the jobs.
+    """Spool processes and use them to run jobs.
 
-    :param inputs:
-    :type inputs:
-    :param cpus:
-    :type cpus:
+    :param inputs: the functions and arguments to run in parallel
+    :type inputs: list[tuple[func, tuple]]
+    :param cpus: the number of CPU cores to use
+    :type cpus: int
     :return: results
     """
     job_q = multiprocessing.Queue()
-    done_q = multiprocessing.Queue()
+    result_q = multiprocessing.Queue()
 
+    # Populate the job_queue
     [job_q.put(job) for job in inputs]
 
+    # Set up workers and put a 'STOP' signal at the end of job_q for each
     worker_pool = list()
     for i in range(cpus):
         worker_pool.append(
-            multiprocessing.Process(target=worker, args=(job_q, done_q)))
-        job_q.put("STOP")
+            multiprocessing.Process(target=worker, args=(job_q, result_q)))
+        job_q.put('STOP')
 
+    # Ready... set... go!
     [w.start() for w in worker_pool]
 
-    # Grab results
+    # Grab results from result_q
     results = []
     for _ in range(len(inputs)):
-        results.append(done_q.get())
+        result = result_q.get()
+        if result is not None:
+            results.append(result)
 
+    # Make workers join the main process
     [w.join() for w in worker_pool]
 
     return results
```

### Comparing `phamclust-1.0.0/src/phamclust/statistics.py` & `phamclust-1.0.1/src/phamclust/statistics.py`

 * *Files identical despite different names*

### Comparing `phamclust-1.0.0/src/phamclust.egg-info/SOURCES.txt` & `phamclust-1.0.1/src/phamclust.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 src/phamclust/cli.py
 src/phamclust/clustering.py
 src/phamclust/fasta.py
 src/phamclust/genome.py
 src/phamclust/heatmap.py
 src/phamclust/matrix.py
 src/phamclust/metrics.py
-src/phamclust/multiprocess.py
 src/phamclust/parallel_process.py
-src/phamclust/similarity.py
 src/phamclust/statistics.py
 src/phamclust.egg-info/PKG-INFO
 src/phamclust.egg-info/SOURCES.txt
 src/phamclust.egg-info/dependency_links.txt
 src/phamclust.egg-info/entry_points.txt
 src/phamclust.egg-info/top_level.txt
```

