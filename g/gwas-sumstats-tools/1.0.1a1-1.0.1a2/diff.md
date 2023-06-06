# Comparing `tmp/gwas_sumstats_tools-1.0.1a1.tar.gz` & `tmp/gwas_sumstats_tools-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas_sumstats_tools-1.0.1a1.tar", max compression
+gzip compressed data, was "gwas_sumstats_tools-1.0.1a2.tar", max compression
```

## Comparing `gwas_sumstats_tools-1.0.1a1.tar` & `gwas_sumstats_tools-1.0.1a2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-03-09 11:15:51.784497 gwas_sumstats_tools-1.0.1a1/LICENSE
--rw-r--r--   0        0        0     4846 2023-03-27 10:55:38.752210 gwas_sumstats_tools-1.0.1a1/README.md
--rw-r--r--   0        0        0    11560 2023-04-05 16:37:33.320361 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/cli.py
--rw-r--r--   0        0        0     1387 2023-03-14 16:16:38.921210 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/config.py
--rw-r--r--   0        0        0     5701 2023-05-12 13:51:17.072439 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/format.py
--rw-r--r--   0        0        0    10291 2023-04-05 16:37:33.320361 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/interfaces/data_table.py
--rw-r--r--   0        0        0     7516 2023-05-12 13:51:17.072439 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/interfaces/metadata.py
--rw-r--r--   0        0        0     3913 2023-03-09 11:15:51.785498 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/read.py
--rw-r--r--   0        0        0     5754 2023-03-14 16:16:38.921210 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/schema/data_table.py
--rw-r--r--   0        0        0     1816 2023-05-12 16:09:09.068864 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/schema/metadata.py
--rw-r--r--   0        0        0     4773 2023-05-12 13:51:17.072439 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/utils.py
--rw-r--r--   0        0        0     8337 2023-04-05 16:37:33.320361 gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/validate.py
--rw-r--r--   0        0        0      679 2023-05-12 16:09:09.068864 gwas_sumstats_tools-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.1a2/LICENSE
+-rw-r--r--   0        0        0     4846 2023-04-11 15:51:21.526207 gwas_sumstats_tools-1.0.1a2/README.md
+-rw-r--r--   0        0        0    11560 2023-04-11 15:51:21.557208 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/cli.py
+-rw-r--r--   0        0        0     1387 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/config.py
+-rw-r--r--   0        0        0     5817 2023-05-16 16:41:20.816328 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/format.py
+-rw-r--r--   0        0        0    10291 2023-04-11 15:51:21.558208 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/data_table.py
+-rw-r--r--   0        0        0     7574 2023-05-16 16:41:20.816328 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/metadata.py
+-rw-r--r--   0        0        0     3913 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/read.py
+-rw-r--r--   0        0        0     5754 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/data_table.py
+-rw-r--r--   0        0        0     1816 2023-05-12 16:09:12.400946 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/metadata.py
+-rw-r--r--   0        0        0     4773 2023-05-12 13:51:16.163417 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/utils.py
+-rw-r--r--   0        0        0     8337 2023-04-11 15:51:21.558208 gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/validate.py
+-rw-r--r--   0        0        0      679 2023-05-16 16:41:20.824328 gwas_sumstats_tools-1.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.1a2/PKG-INFO
```

### Comparing `gwas_sumstats_tools-1.0.1a1/LICENSE` & `gwas_sumstats_tools-1.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/README.md` & `gwas_sumstats_tools-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/cli.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/cli.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/config.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/config.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/format.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,27 @@
                      from_gwas_cat: bool = False,
                      custom_metadata: dict = None) -> MetadataClient:
         """Set metadata.
         The hierarchy of where metadata is set is as follows:
         1. custom_metadata map (overwrites anything below)
         2. metadata from the GWAS Catalog
         3. metadata from the original input file
+        4. metadata inferred from the datafile
 
         Keyword Arguments:
             from_gwas_cat -- update with data from GWAS catalog (default: {False})
             custom_metadata -- Update with this map (default: {None})
 
         Returns:
             metadata object
         """
         self.meta.from_file()
         meta_dict = get_file_metadata(in_file=self.data_infile,
-                                      out_file=self.data_outfile)
+                                      out_file=self.data_outfile,
+                                      meta_dict=self.meta.as_dict())
         if from_gwas_cat:
             accession_id = parse_accession_id(filename=self.data_infile)
             meta_dict.update(metadata_dict_from_gwas_cat(accession_id=accession_id))
         if custom_metadata:
             meta_dict.update(custom_metadata)
         self.meta.update_metadata(meta_dict)
         return self.meta
```

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/interfaces/data_table.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/interfaces/metadata.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/interfaces/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         self._meta_dict = meta_dict
         self._in_file = in_file
         self._out_file = out_file
 
     def from_file(self) -> None:
         """Create metadata from YAML file
         """
+        if self._in_file is None:
+            return None
         with open(self._in_file, "r") as fh:
             self._meta_dict = yaml.safe_load(fh)
             self.update_metadata(self._meta_dict)
 
     def to_file(self) -> None:
         """Write metadata to YAML file
         """
```

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/read.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/read.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/schema/data_table.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/schema/metadata.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/utils.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/utils.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/gwas_sumstats_tools/validate.py` & `gwas_sumstats_tools-1.0.1a2/gwas_sumstats_tools/validate.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.1a1/pyproject.toml` & `gwas_sumstats_tools-1.0.1a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwas-sumstats-tools"
-version = "1.0.1a1"
+version = "1.0.1a2"
 description = ""
 authors = ["jdhayhurst <jhayhurst@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "gwas_sumstats_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gwas_sumstats_tools-1.0.1a1/PKG-INFO` & `gwas_sumstats_tools-1.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas-sumstats-tools
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: 
 Author: jdhayhurst
 Author-email: jhayhurst@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

