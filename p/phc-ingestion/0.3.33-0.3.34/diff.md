# Comparing `tmp/phc-ingestion-0.3.33.tar.gz` & `tmp/phc-ingestion-0.3.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.33.tar", last modified: Tue Jun  6 11:22:39 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.34.tar", last modified: Tue Jun  6 16:50:14 2023, max compression
```

## Comparing `phc-ingestion-0.3.33.tar` & `phc-ingestion-0.3.34.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-06 11:22:09.263869 phc-ingestion-0.3.33/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2222 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     7409 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3761 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5664 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1913 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.33/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     7409 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5664 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     1913 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-06 16:49:46.547448 phc-ingestion-0.3.34/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.34/PKG-INFO
```

### Comparing `phc-ingestion-0.3.33/ingestion/caris/process.py` & `phc-ingestion-0.3.34/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.34/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.34/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.34/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.34/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/json.py` & `phc-ingestion-0.3.34/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.34/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.34/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.34/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.34/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/foundation/process.py` & `phc-ingestion-0.3.34/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.34/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.34/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.34/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.34/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/nextgen/process.py` & `phc-ingestion-0.3.34/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.34/ingestion/nextgen/util/process_cnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         gene = working[3]
         gene_id_only = gene.split("_")[0]
         if gene_id_only.endswith("CN"):
             gene_id_only = gene_id_only[:-2]
 
         copy_number = working[4]
         status = working[5]
+        if status == "normal":
+            status = "neutral"
 
         # Hard-code
         attributes = {}
 
         # Scrape interpretation
         interpretation = None
         if not copy_number_variant_table.empty:
```

### Comparing `phc-ingestion-0.3.33/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.34/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.34/ingestion/nextgen/util/process_structural.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     structural_status = True
     for variant in variants:
         working_variant = variant.strip().split("\t")
 
         chromosome1 = f"chr{working_variant[0]}"
         start_position1 = working_variant[1]
 
-        if working_variant[4] in ["<DEL>", "<DUP:TANDEM>"]:
+        if "MantaDEL" in working_variant[2] or "MantaDUP" in working_variant[2]:
             end_position1 = working_variant[7].split(";")[0].split("=")[1]
             chromosome2 = chromosome1
             start_position2 = start_position1
-            end_position2 = end_position2
-            effect = "deletion" if working_variant[4] == "<DEL>" else "duplication"
+            end_position2 = end_position1
+            effect = "deletion" if "MantaDEL" in working_variant[2] else "duplication"
 
             # Get genes from coordinates using center point of start and end positions
             gene1 = coords_to_genes(
                 "GRCh38", chromosome1, int((int(start_position1) + int(end_position1)) / 2), log
             )
             gene2 = "N/A"
```

### Comparing `phc-ingestion-0.3.33/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.34/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.34/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.34/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.34/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.34/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.34/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.33/pyproject.toml` & `phc-ingestion-0.3.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.33"
+version = "0.3.34"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

