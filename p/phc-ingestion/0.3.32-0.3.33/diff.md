# Comparing `tmp/phc-ingestion-0.3.32.tar.gz` & `tmp/phc-ingestion-0.3.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.32.tar", last modified: Mon Jun  5 13:26:09 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.33.tar", last modified: Tue Jun  6 11:22:39 2023, max compression
```

## Comparing `phc-ingestion-0.3.32.tar` & `phc-ingestion-0.3.33.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3030 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2214 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     7359 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3652 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5664 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2222 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-05 13:25:42.546540 phc-ingestion-0.3.32/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-05 13:25:42.550540 phc-ingestion-0.3.32/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-05 13:25:42.550540 phc-ingestion-0.3.32/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-05 13:25:42.550540 phc-ingestion-0.3.32/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-05 13:25:42.550540 phc-ingestion-0.3.32/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-05 13:25:42.550540 phc-ingestion-0.3.32/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.32/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-06 11:22:09.263869 phc-ingestion-0.3.33/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2222 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     7409 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3761 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5664 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     1913 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-06 11:22:09.267869 phc-ingestion-0.3.33/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-06 11:22:09.271869 phc-ingestion-0.3.33/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.33/PKG-INFO
```

### Comparing `phc-ingestion-0.3.32/ingestion/caris/process.py` & `phc-ingestion-0.3.33/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.33/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.33/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.33/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.33/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/json.py` & `phc-ingestion-0.3.33/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.33/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.33/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.33/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.33/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/foundation/process.py` & `phc-ingestion-0.3.33/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.33/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.33/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.33/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.33/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/nextgen/process.py` & `phc-ingestion-0.3.33/ingestion/nextgen/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,34 +23,34 @@
         "projectId": project_id,
         "archiveFileId": source_file_id,
         "caseId": prefix,
         "ingestion_id": ingestion_id,
     }
     with scoped_logger(__name__, log_context) as log:
         cnv_path_name = process_cnv(
-            pdf_in_file=vendor_files["pdfFile"],
+            xml_in_file=vendor_files["xmlFile"],
             cnv_in_file=vendor_files["somaticCnvTxtFile"],
             root_path=local_output_dir,
             prefix=prefix,
             log=log,
         )
-
+        structural_path_name, structural_status = process_structural(
+            xml_in_file=vendor_files["xmlFile"],
+            sv_in_file=vendor_files["somaticSvVcfFile"],
+            root_path=local_output_dir,
+            prefix=prefix,
+            log=log,
+        )
         xml_pdf_prefix = vendor_files["pdfFile"].split("/")[-1].split(".")[0]
         manifest = process_manifest(
             xml_in_file=vendor_files["xmlFile"],
             source_file_id=source_file_id,
             prefix=prefix,
             xml_pdf_prefix=xml_pdf_prefix,
-            log=log,
-        )
-        structural_path_name = process_structural(
-            pdf_in_file=vendor_files["pdfFile"],
-            sv_in_file=vendor_files["somaticSvVcfFile"],
-            root_path=local_output_dir,
-            prefix=prefix,
+            structural_status=structural_status,
             log=log,
         )
         somatic_vcf_meta_data = process_vcf(
             vcf_in_file=vendor_files["somaticVcfFile"],
             root_path=local_output_dir,
             prefix=prefix,
             sequence_type="somatic",
```

### Comparing `phc-ingestion-0.3.32/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.33/ingestion/nextgen/util/process_cnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pandas as pd
 from logging import Logger
 
 from ingestion.nextgen.util.variant_table import extract_variant_table
 from ingestion.nextgen.util.interpretation import map_interpretation
 
 
-def process_cnv(pdf_in_file: str, cnv_in_file: str, root_path: str, prefix: str, log: Logger):
+def process_cnv(xml_in_file: str, cnv_in_file: str, root_path: str, prefix: str, log: Logger):
     copy_number_path_name = f"{root_path}/{prefix}.copynumber.csv"
     sample_id = prefix
 
     copy_number_variant_rows = []
     copy_number_variant_table = extract_variant_table(
-        pdf=pdf_in_file, variant_type="copy number", log=log
+        xml_in_file=xml_in_file, variant_type="copy number", log=log
     )
 
     with open(cnv_in_file, "r") as f:
         cnv_rows = f.readlines()
 
     for row in cnv_rows[1:]:
         working = row.strip().split("\t")
```

### Comparing `phc-ingestion-0.3.32/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.33/ingestion/nextgen/util/process_manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 from ruamel.yaml import YAML
 from logging import Logger
-from pdfminer.high_level import extract_pages
-from pdfminer.layout import LTTextBoxHorizontal
 
 
 def transform_date(date: str):
     """mm/dd/yyyy -> yyyy-mm-dd"""
     date_list = date.split("/")
     new_date = f"{date_list[2]}-{date_list[0]}-{date_list[1]}"
     return new_date
@@ -140,15 +138,20 @@
             manifest["bodySite"] = f"{body_site_one} {body_site_two}"
             manifest["bodySiteDisplay"] = f"{body_site_one} {body_site_two}"
 
     return manifest
 
 
 def process_manifest(
-    xml_in_file: str, source_file_id: str, prefix: str, xml_pdf_prefix: str, log: Logger
+    xml_in_file: str,
+    source_file_id: str,
+    prefix: str,
+    xml_pdf_prefix: str,
+    structural_status: bool,
+    log: Logger,
 ):
     xml_text = extract_xml_text(xml_in_file)
     manifest = extract_test_data(xml_text)
     manifest.update(extract_patient_data(xml_text))
 
     manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{xml_pdf_prefix}.pdf"
     manifest["sourceFileId"] = source_file_id
@@ -159,19 +162,14 @@
     manifest["files"] = [
         {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.copynumber.csv",
             "sequenceType": "somatic",
             "type": "copyNumberVariant",
         },
         {
-            "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.structural.csv",
-            "sequenceType": "somatic",
-            "type": "structuralVariant",
-        },
-        {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.modified.somatic.nrm.filtered.vcf.gz",
             "sequenceType": "somatic",
             "type": "shortVariant",
         },
         {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.modified.germline.nrm.filtered.vcf.gz",
             "sequenceType": "germline",
@@ -184,9 +182,17 @@
         },
         {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.germline.updated.bam",
             "sequenceType": "germline",
             "type": "read",
         },
     ]
+    if structural_status == True:
+        manifest["files"].append(
+            {
+                "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.structural.csv",
+                "sequenceType": "somatic",
+                "type": "structuralVariant",
+            },
+        )
 
     return manifest
```

### Comparing `phc-ingestion-0.3.32/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.33/ingestion/nextgen/util/process_structural.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 from logging import Logger
 
 from ingestion.shared_util.coords_to_genes import coords_to_genes
 from ingestion.nextgen.util.variant_table import extract_variant_table
 from ingestion.nextgen.util.interpretation import map_interpretation
 
 
-def process_structural(sv_in_file: str, pdf_in_file, root_path: str, prefix: str, log: Logger):
+def process_structural(sv_in_file: str, xml_in_file, root_path: str, prefix: str, log: Logger):
     structural_variant_table = extract_variant_table(
-        pdf=pdf_in_file, variant_type="structural", log=log
+        xml_in_file=xml_in_file, variant_type="structural", log=log
     )
 
     structural_variant_path_name = f"{root_path}/{prefix}.structural.csv"
     sample_id = prefix
 
     with open(sv_in_file, "r") as f:
         variants = [line for line in f.readlines() if not line.startswith("#")]
 
     if not variants:
         log.info(f"No structural variants found in {sv_in_file}")
-        return None
+        structural_status = False
+        return None, structural_status
 
     structural_variant_rows = []
+    structural_status = True
     for variant in variants:
         working_variant = variant.strip().split("\t")
 
         chromosome1 = f"chr{working_variant[0]}"
         start_position1 = working_variant[1]
 
         if working_variant[4] in ["<DEL>", "<DUP:TANDEM>"]:
@@ -84,8 +86,8 @@
     with open(structural_variant_path_name, "w+") as f:
         f.write(
             "sample_id,gene1,gene2,effect,chromosome1,start_position1,end_position1,chromosome2,start_position2,end_position2,interpretation,sequence_type,in-frame,attributes\n"
         )
         for sv_text_row in structural_variant_rows:
             f.write(sv_text_row)
 
-    return structural_variant_path_name
+    return structural_variant_path_name, structural_status
```

### Comparing `phc-ingestion-0.3.32/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.33/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.33/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.33/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.33/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.33/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.32/pyproject.toml` & `phc-ingestion-0.3.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.32"
+version = "0.3.33"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

