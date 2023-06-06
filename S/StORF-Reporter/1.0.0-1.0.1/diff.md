# Comparing `tmp/StORF-Reporter-1.0.0.tar.gz` & `tmp/StORF-Reporter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StORF-Reporter-1.0.0.tar", last modified: Sun May 28 20:53:55 2023, max compression
+gzip compressed data, was "StORF-Reporter-1.0.1.tar", last modified: Tue Jun  6 02:48:35 2023, max compression
```

## Comparing `StORF-Reporter-1.0.0.tar` & `StORF-Reporter-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:53:55.186365 StORF-Reporter-1.0.0/
--rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-23 17:28:19.000000 StORF-Reporter-1.0.0/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-05-28 20:53:55.186365 StORF-Reporter-1.0.0/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-05-28 20:46:50.000000 StORF-Reporter-1.0.0/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-23 17:28:19.000000 StORF-Reporter-1.0.0/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-05-28 20:53:55.186365 StORF-Reporter-1.0.0/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:53:55.182365 StORF-Reporter-1.0.0/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:53:55.182365 StORF-Reporter-1.0.0/src/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-05-28 20:28:06.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/Constants.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16596 2023-05-28 20:30:57.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Extractor.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-05-28 20:30:57.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Finder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5306 2023-05-28 20:30:57.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Remover.py
--rw-r--r--   0 nick      (1000) nick      (1000)    52243 2023-05-28 20:43:07.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Reporter.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:53:55.186365 StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/
--rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-05-28 20:30:57.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/StORF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-23 17:28:19.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/UR_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-23 17:28:19.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/Un_StORFed.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:28:19.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/__init__.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    15208 2023-05-28 20:36:27.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/UR_Extractor.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-07 16:36:44.000000 StORF-Reporter-1.0.0/src/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:53:55.186365 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-05-28 20:53:55.000000 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-05-28 20:53:55.000000 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-28 20:53:55.000000 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-05-28 20:53:55.000000 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-05-28 20:53:55.000000 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-05-28 20:53:55.000000 StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/
+-rw-r--r--   0 nick      (1000) nick      (1000)    35149 2021-12-28 14:08:10.000000 StORF-Reporter-1.0.1/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-06-06 02:48:16.000000 StORF-Reporter-1.0.1/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-16 17:48:19.000000 StORF-Reporter-1.0.1/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.303331 StORF-Reporter-1.0.1/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.303331 StORF-Reporter-1.0.1/src/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-06-06 02:48:16.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Constants.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16596 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Extractor.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Finder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5220 2023-05-14 21:36:54.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Remover.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    51993 2023-06-06 02:42:40.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Reporter.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/StORF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-09-29 20:25:03.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/UR_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-09-29 20:25:03.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/Un_StORFed.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-09-29 20:25:03.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/__init__.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    15208 2023-06-06 02:45:48.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/UR_Extractor.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 11:38:05.000000 StORF-Reporter-1.0.1/src/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-06 02:48:35.307331 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-06-06 02:48:35.000000 StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/top_level.txt
```

### Comparing `StORF-Reporter-1.0.0/LICENSE` & `StORF-Reporter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/PKG-INFO` & `StORF-Reporter-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 1.0.0
+Version: 1.0.1
 Summary: StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 Home-page: https://github.com/NickJD/StORF-Reporter
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/StORF-Reporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -73,15 +73,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.1: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -183,15 +183,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -221,15 +221,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.1: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -285,15 +285,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.1: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -318,15 +318,15 @@
 StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
 ```
 
 ```python
 usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
                         [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.0/README.md` & `StORF-Reporter-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.1: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -168,15 +168,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -206,15 +206,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.1: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -270,15 +270,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.1: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -303,15 +303,15 @@
 StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
 ```
 
 ```python
 usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
                         [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.0/setup.cfg` & `StORF-Reporter-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = StORF-Reporter
-version = v1.0.0
+version = v1.0.1
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/StORF-Reporter
 project_urls =
```

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Extractor.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Extractor.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Finder.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Finder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Remover.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Remover.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 
 try:
     from .Constants import *
 except (ModuleNotFoundError, ImportError, NameError, TypeError) as error:
     from Constants import *
 
 def gff_load_and_write(options,gff_in,blast_hits):
-    for line in gff_in:  # Get gene loci from GFF - ID=Gene will also classify Pseudogenes as genes
+    for line in gff_in: 
         line_data = line.split()
         if line.startswith('\n') or line.startswith('#'):  # Not to crash on empty lines in GFF
             options.gff_out.write(line)
         else:
-            if 'Single_Genome' in line:
+            if 'StORF-Reporter' in line:
                 StORF = line_data[8].split('ID=')[1].split(';')[0]
                 if StORF in blast_hits:
                     options.gff_out.write(line)
             else:
                 options.gff_out.write(line)
 
 
 def load_blast_6(options, blast_in):
     blast_hits = collections.OrderedDict()
     for line in blast_in:
         line_data = line.split('\t')
         if 'StORF' in line_data[0]:
             if int(line_data[11].split('.')[0]) >= options.minscore:
-                blast_hits.update({line_data[0].split(';')[0]:[]})
+                blast_hits.update({line_data[0]:[]})
 
     return blast_hits
 
 def remover(options):
     try:
         try:
             blast_in = gzip.open(options.blast,'rt')
@@ -50,15 +50,15 @@
             gff_load_and_write(options,gff_in,blast_hits)
     except AttributeError:
         sys.exit("Attribute Error")
 
 
 def main():
 
-    parser = argparse.ArgumentParser(description='Single_Genome ' + StORF_Reporter_Version + ': UR-Extractor Run Parameters.')
+    parser = argparse.ArgumentParser(description='StORF-Reporter ' + StORF_Reporter_Version + ': UR-Extractor Run Parameters.')
     parser._action_groups.pop()
 
     required = parser.add_argument_group('Required Arguments')
     required.add_argument('-gff', action='store', dest='gff', help='GFF annotation file for the FASTA',
                         required=False)
     required.add_argument('-blast', action='store', dest='blast', help='BLAST format 6 annotation file',
                         required=False)
@@ -86,15 +86,15 @@
     options = parser.parse_args()
     if options.gff == None or options.blast == None:
         if options.version:
             sys.exit(StORF_Reporter_Version)
         else:
             exit('StORF-Remover: error: the following arguments are required: -f, -gff, -blast')
 
-    print("Thank you for using Single_Genome -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
+    print("Thank you for using StORF-Reporter -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
           "Please report any issues to: https://github.com/NickJD/StORF-Reporter/issues\n#####")
 
     options.annotation_type = [None,None]
 
     #### Output Directory and Filename handling
     if options.o_dir == None and options.o_name == None:
         tmp_extension = options.gff.split('.')[-1]
```

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/StORF_Reporter.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/StORF_Reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
       'TGC':'C', 'TGT':'C', 'TGA':'*', 'TGG':'W'}
 
 def translate_frame(sequence):
     translate = ''.join([gencode.get(sequence[3 * i:3 * i + 3], 'X') for i in range(len(sequence) // 3)])
     return translate
 ############################
 
-def GFF_StoRF_write(Reporter_options, track_contig, gff_out, StORF, StORF_Num): # Consistency in outfile
+def GFF_StORF_write(Reporter_options, track_contig, gff_out, StORF, StORF_Num): # Consistency in outfile
     ID = track_contig + '_UR_' + StORF[0] + '_' + StORF[10] + '_'+ str(StORF[9])
     try:
         to_hash = gff_out.split('.')[0] + '_' + ID # create unique hash from outfile name and ID
     except AttributeError:
         to_hash = gff_out.name.split('.')[0] + '_' + ID  # create unique hash from outfile name and ID
     locus_tag = hashlib.shake_256(to_hash.encode()).hexdigest(8)
     ### Write out new GFF entry -
@@ -272,19 +272,19 @@
         elif os.path.isfile(fa):
             Reporter_options.fasta = fa
         else:
             sys.exit('No matching FASTA file found for ' + gff)
     URs = extractor(Reporter_options)
     return URs,Reporter_options
 
-def run_UR_Extractor_GFF(Reporter_options, fasta, gff): # When given a directory with multiple GFFs but without accompianing .fna
+def run_UR_Extractor_GFF(Reporter_options, gff): # When given a directory with multiple GFFs but without accompianing .fna
     if '_StORF-Reporter_Extended' not in gff: #Might fall over - put a break
         gff = gff
         Reporter_options.gff = gff
-    fasta = str(fasta)
+    fasta = str(gff)
     Reporter_options.fasta = fasta
     URs = extractor(Reporter_options)
     return URs,Reporter_options
 
 def find_prev_StORFs(StORF_options, Reporter_options, Contig_URs, track_current_start, track_prev_stop, track_contig):
     StORFs_to_del = []
     StORFs = []
@@ -408,18 +408,18 @@
                 fasta_outfile = open(Reporter_options.output_file + '.fasta', 'w', newline='\n', encoding='utf-8')
         elif Reporter_options.gz == True:
                 fasta_outfile = gzip.open(Reporter_options.output_file + '.fasta.gz', 'wt', newline='\n', encoding='utf-8')
         faa_infile = Reporter_options.gff.replace('.gff3', '.faa').replace('.gff','.faa')
         ffn_infile = Reporter_options.gff.replace('.gff3', '.ffn').replace('.gff','.ffn')
         Original_AA,Original_NT = FASTA_Load(faa_infile,ffn_infile)
     if Reporter_options.annotation_type[0] == 'Pyrodigal':
-        Reporter_options.gff_outfile.write('##Pyrodigal annotation and Single_Genome extended GFF annotation of ' + Reporter_options.fasta.split('/')[-1] + '\n')
+        Reporter_options.gff_outfile.write('##Pyrodigal annotation and StORF-Reporter extended GFF annotation of ' + Reporter_options.fasta.split('/')[-1] + '\n')
     else:
-        Reporter_options.gff_outfile.write('##Single_Genome extended annotation of ' + gff_name.split('/')[-1] + '\n')
-    Reporter_options.gff_outfile.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
+        Reporter_options.gff_outfile.write('##StORF-Reporter extended annotation of ' + gff_name.split('/')[-1] + '\n')
+    Reporter_options.gff_outfile.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
 
     first_region = True
     for line in gff_in.splitlines( ):
         if not line.startswith('#') and end == False:
             data = line.split('\t')
             track_current_start = int(data[3])
             track_current_stop = int(data[4])
@@ -429,15 +429,15 @@
                 first_region = False
                 continue
             if track_contig != track_prev_contig:  # End of current contig
                 # if track_prev_contig != '': # Get last StORF on Contig - If Present
                 #     StORFs = find_after_StORFs(StORF_options, Contig_URS, track_prev_start, track_prev_stop,track_prev_contig) # Changed to prev stop because we are switching from previous contig
                 #     if StORFs:
                 #         for StORF in StORFs:
-                #             GFF_StoRF_write( Reporter_options, track_prev_contig, outfile, StORF,
+                #             GFF_StORF_write( Reporter_options, track_prev_contig, outfile, StORF,
                 #                             StORF_Num)  # To keep consistency
                 #             if StORF_options.path == True:
                 #                 FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
                 #             StORF_Num += 1
                 track_prev_start, track_prev_stop = 0, 0
             track_prev_contig = track_contig
             if track_current_start == track_prev_start and track_current_stop == track_prev_stop:  # `duplicate' entry in GFF
@@ -468,40 +468,39 @@
                         wrapped = textwrap.wrap(Original_Seq, width=60)
                         for wrap in wrapped:
                             fasta_outfile.write(wrap + '\n')
                     else:
                         fasta_outfile.write(Original_Seq+'\n')
             if StORFs:
                 for StORF in StORFs:  # ([ur_pos,StORF_start, StORF_stop, StORF_Start_In_UR, StORF_Stop_In_UR, frame, ur_frame, strand, StORF_Length, StORF_UR_Num, StORF_Seq)]
-                    GFF_StoRF_write(Reporter_options, track_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
+                    GFF_StORF_write(Reporter_options, track_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
                     if Reporter_options.annotation_type[1] == 'Out_Dir':
                         FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
                     StORF_Num += 1
             if line != written_line:
                 Reporter_options.gff_outfile.write(line.strip()+'\n')
                 written_line = line
             StORFs = None
         elif line.startswith('##sequence-region') and first_region != True:
-            StORFs = find_after_StORFs(Reporter_options, Contig_URS, track_prev_start, track_prev_stop,
-                                       track_prev_contig)  # Changed to prev stop because we are switching from previous contig
+            StORFs = find_after_StORFs(Reporter_options, Contig_URS, track_prev_start, track_prev_stop, track_prev_contig)  # Changed to prev stop because we are switching from previous contig
             if StORFs:
                 for StORF in StORFs:
-                    GFF_StoRF_write(Reporter_options, track_prev_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
+                    GFF_StORF_write(Reporter_options, track_prev_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
                     if Reporter_options.annotation_type[1] == 'Out_Dir':
                         FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
                     StORF_Num += 1
             Reporter_options.gff_outfile.write(line.strip() + '\n')
 
         elif line.startswith('##FASTA'):
             Reporter_options.gff_outfile.write(line.strip() + '\n')
             end = True
             # StORFs = find_after_StORFs(StORF_options, Contig_URS, track_prev_start, track_prev_stop, track_prev_contig)  # Changed to prev stop because we are switching from previous contig
             # if StORFs:
             #     for StORF in StORFs:
-            #         GFF_StoRF_write(Reporter_options, track_prev_contig, outfile, StORF)  # To keep consistency
+            #         GFF_StORF_write(Reporter_options, track_prev_contig, outfile, StORF)  # To keep consistency
             #         if StORF_options.path == True:
             #             FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
             #         StORF_Num += 1
             # if line != written_line:
             #     outfile.write(line.strip()+'\n')
             #     written_line = line
 
@@ -509,15 +508,15 @@
             Reporter_options.gff_outfile.write(line.strip()+'\n')
             written_line = line
 ##############################################################
 
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Single_Genome ' + StORF_Reporter_Version + ': Single_Genome Run Parameters.', formatter_class=SmartFormatter)
+    parser = argparse.ArgumentParser(description='StORF-Reporter ' + StORF_Reporter_Version + ': StORF-Reporter Run Parameters.', formatter_class=SmartFormatter)
     parser._action_groups.pop()
 
     required = parser.add_argument_group('Required Options')
     required.add_argument('-anno', action='store', dest='annotation_type', required=False,
                         choices=['Prokka', 'Bakta', 'Out_Dir', 'Single_GFF', 'Multiple_GFFs', 'Ensembl', 'Feature_Types',
                                   'Single_Genome', 'Multiple_Genomes','Single_Combined_GFF', 'Multiple_Combined_GFFs',
                                  'Pyrodigal', 'Single_FASTA', 'Multiple_FASTA'], nargs='*',
@@ -544,15 +543,15 @@
                              '--- Complete Annotation Input Options: \n'
                              '\tSingle_FASTA = To provide a single FASTA file; \n'
                              '\tMultiple_FASTA = To provide a directory containing multiple FASTA files (will detect .fna,.fa,.fasta); \n\n')
 
     required.add_argument('-p', action='store', dest='path', default='', required=False,
                         help='Provide input file or directory path')
     ###
-    StORF_Reporter_args = parser.add_argument_group('Single_Genome Options')
+    StORF_Reporter_args = parser.add_argument_group('StORF-Reporter Options')
     ### Add options to redirect into new output directory and filename - and output StORFs on their own in their own GFF -
     StORF_Reporter_args.add_argument('-oname', action="store", dest='o_name', required=False,
                         help='Default - Appends \'_StORF-R\' to end of input FASTA filename - Multiple_* runs will be numbered')
     StORF_Reporter_args.add_argument('-odir', action="store", dest='o_dir', required=False,
                         help='Default -  Same directory as input FASTA')
     StORF_Reporter_args.add_argument('-sout', action="store", dest='storfs_out', default=False, type=eval, choices=[True, False],
                         help='Default - False: Print out StORF sequences separately from Prokka/Bakta annotations')
@@ -640,47 +639,46 @@
     #optional.add_argument('-comb', action='store', dest='combined_gffs', default='', required=False,
     #                    help='Provide directory containing GFFs with sequences combined into single file to be StORFed - Only produces modified GFFs')
 
     misc = parser.add_argument_group('Misc')
 
 
     misc.add_argument('-overwrite', action='store', dest='overwrite', default=False, type=eval, choices=[True, False],
-                        help='Default - False: Overwrite Single_Genome output if already present')
+                        help='Default - False: Overwrite StORF-Reporter output if already present')
     misc.add_argument('-verbose', action='store', dest='verbose', default=False, type=eval, choices=[True, False],
                         help='Default - False: Print out runtime messages')
     misc.add_argument('-v', action='store_true', dest='version',
-                        help='Default - False: Print out version number and exit')
+                        help='Print out version number and exit')
     misc.add_argument('-nout', action='store', dest='nout', default=True, type=eval, choices=[True, False],
                         help=argparse.SUPPRESS)
     misc.add_argument('-nout_pyrodigal', action='store', dest='nout_pyrodigal', default=True, type=eval, choices=[True, False],
                         help=argparse.SUPPRESS)
 
     Reporter_options = parser.parse_args()
     Reporter_options.gff_fasta = None # To be done
     Reporter_options.reporter = True
 
     if Reporter_options.annotation_type == None or Reporter_options.path == None:
         if Reporter_options.version:
             sys.exit(StORF_Reporter_Version)
         else:
-            exit('Single_Genome: error: the following arguments are required: -anno, -p')
-    print("Thank you for using Single_Genome -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
+            exit('StORF-Reporter: error: the following arguments are required: -anno, -p')
+    print("Thank you for using StORF-Reporter -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
           "Please report any issues to: https://github.com/NickJD/StORF-Reporter/issues\n#####")
 
     ##############
     ## Print out user chosen annotation options
 
     ##############
     ## Incompatible argument catching
     if len(Reporter_options.annotation_type) != 2:
         parser.error('Please select two compatible options for required argument -anno.')
     ##############
     #### Output Directory and Filename handling
     ### Add '/' to end of directory path
-    Reporter_options.path = os.path.abspath(Reporter_options.path) # If given relative path, convert to absolute path
     if Reporter_options.annotation_type[1] in ['Multiple_GFFs','Multiple_Genomes','Multiple_FASTA','Out_Dir','Comb_GFFs', 'Multiple_Combined_GFFs']:
         Reporter_options.path = Reporter_options.path + '/' if not Reporter_options.path.endswith('/') else Reporter_options.path
 
     if Reporter_options.o_dir == None and Reporter_options.o_name == None:
         if Reporter_options.annotation_type[1] == 'Out_Dir':
             output_file = Reporter_options.path#.split('.')[-1]
             output_file = output_file + output_file.split('/')[-2] + '_StORF-Reporter_Extended'
@@ -720,19 +718,19 @@
     ############## Setup for Prokka/Bakta output directory
     if Reporter_options.annotation_type[0] in ('Prokka','Bakta') and Reporter_options.annotation_type[1] == 'Out_Dir':
         Reporter_options.output_file = output_file
         #### Checking and cleaning
         for fname in os.listdir(Reporter_options.path):
             if '_StORF-Reporter_Extended' in fname and Reporter_options.overwrite == False:
                 parser.error(
-                    'Prokka/Bakta directory not clean and already contains a Single_Genome output. Please delete or use "-overwrite True" and try again.')
+                    'Prokka/Bakta directory not clean and already contains a StORF-Reporter output. Please delete or use "-overwrite True" and try again.')
             elif '_StORF-Reporter_Extended' in fname and Reporter_options.overwrite == True:
                 os.remove(Reporter_options.path + '/' + fname)
                 if Reporter_options.verbose == True:
-                    print('Single_Genome output ' + fname + ' will be overwritten.')
+                    print('StORF-Reporter output ' + fname + ' will be overwritten.')
         ####
         Reporter_options.gene_ident = "misc_RNA,gene,mRNA,CDS,rRNA,tRNA,tmRNA,CRISPR,ncRNA,regulatory_region,oriC,pseudo"
         Contigs, Reporter_options = run_UR_Extractor_Directory(Reporter_options)
         ################## Find StORFs in URs - Setup StORF_Reporter-Finder Run
         Reporter_StORFs = StORF_Reported(Reporter_options, Contigs)
         StORF_Filler(Reporter_options, Reporter_StORFs)
         if Reporter_options.verbose == True:
@@ -745,23 +743,23 @@
         elif Reporter_options.annotation_type[1]  == "Multiple_GFFs":
             gff_list = list(pathlib.Path(Reporter_options.path).glob('*.gff'))
             gff_list.extend(pathlib.Path(Reporter_options.path).glob('*.gff3'))
         #### Checking and cleaning
         gff_list = list(map(str, gff_list))
         gffs_to_filter = []
         for gff in gff_list:
-            if '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
+            if '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
                 gffs_to_filter.append(gff)
                 gffs_to_filter.append(gff.replace('_StORF-Reporter_Extended.gff','.gff'))
-                print('GFF has already been processed and a Single_Genome output exists for ' + gff.split('/')[-1] + '. Please delete or use "-overwrite True" and try again.')
-            elif '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
+                print('Prokka/Bakta GFF has already been processed and a StORF-Reporter output exists for ' + gff.split('/')[-1] + '. Please delete or use "-overwrite True" and try again.')
+            elif '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
                 os.remove(gff)
                 gffs_to_filter.append(gff)
                 if Reporter_options.verbose == True:
-                    print('Single_Genome output '  + gff.split('/')[-1] +  ' will be overwritten.')
+                    print('StORF-Reporter output '  + gff.split('/')[-1] +  ' will be overwritten.')
         gff_list = [x for x in gff_list if x not in gffs_to_filter]
         ####
         Reporter_options.gene_ident = "misc_RNA,gene,mRNA,CDS,rRNA,tRNA,tmRNA,CRISPR,ncRNA,regulatory_region,oriC,pseudo"
         file_counter = 0
         for gff in gff_list:
             # Finalising output_file name
             if Reporter_options.annotation_type[1]  == "Multiple_GFFs" and Reporter_options.o_name != None:
@@ -770,22 +768,22 @@
             elif Reporter_options.annotation_type[1]  == "Multiple_GFFs":
                 tmp_filename = gff.split('/')[-1].split('.gff')[0]  # could be .fa/.fasta etc
                 Reporter_options.output_file = output_file.replace('_StORF-Reporter',tmp_filename + '_StORF-Reporter')
             else:
                 Reporter_options.output_file = output_file
             if Reporter_options.verbose == True:
                 print("Starting: " + str(gff))
-            Contigs, Reporter_options = run_UR_Extractor_Matched(Reporter_options,gff) # used to be extended
+            Contigs, Reporter_options = run_UR_Extractor_GFF(Reporter_options,gff) # used to be extended
             ################## Find StORFs in URs - Setup StORF_Reporter-Finder Run
             Reporter_StORFs = StORF_Reported(Reporter_options, Contigs)
             StORF_Filler(Reporter_options, Reporter_StORFs)
             if Reporter_options.verbose == True:
                 print("Finished: " + gff.split('/')[-1]) # Will add number of additional StORFs here
 
-    ################ Run Single_Genome on standardGFFs
+    ################ Run StORF-Reporter on standardGFFs
     elif Reporter_options.annotation_type[0] in ('Ensembl', 'Feature_Types'):
         if Reporter_options.annotation_type[0] == 'Ensembl':
             Reporter_options.gene_ident = "ID=gene"
         elif Reporter_options.annotation_type[0] == 'Feature_Types':
             Reporter_options.gene_ident = Reporter_options.gene_ident.split(',')
         ####
         if Reporter_options.annotation_type[1] in ("Single_Genome", "Single_Combined_GFF"):
@@ -795,33 +793,33 @@
             gff_list.extend(pathlib.Path(Reporter_options.path).glob('*.gff3'))
         else:
             parser.error('Please select two compatible options for required argument -anno.')
         #### Checking and cleaning
         gff_list = list(map(str, gff_list))
         gffs_to_filter = []
         for gff in gff_list:
-            if '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
+            if '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
                 gffs_to_filter.append(gff)
                 gffs_to_filter.append(gff.replace('_StORF-Reporter_Extended.gff', '.gff'))
-                print('GFF has already been processed and a Single_Genome output exists for ' +
+                print('Prokka/Bakta GFF has already been processed and a StORF-Reporter output exists for ' +
                       gff.split('/')[-1] + '. Please delete or use "-overwrite True" and try again.')
-            elif '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
+            elif '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
                 os.remove(gff)
                 gffs_to_filter.append(gff)
                 if Reporter_options.verbose == True:
-                    print('Single_Genome output ' + gff.split('/')[-1] + ' will be overwritten.')
+                    print('StORF-Reporter output ' + gff.split('/')[-1] + ' will be overwritten.')
         gff_list = [x for x in gff_list if x not in gffs_to_filter]
         ####
         file_counter = 0
         for gff in gff_list:
             # Finalising output_file name
-            if (Reporter_options.annotation_type[1] == "Multiple_Combined_GFFs" or Reporter_options.annotation_type[1] == "Multiple_Genomes") and Reporter_options.o_name != None:
+            if Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs" and Reporter_options.o_name != None:
                 Reporter_options.output_file = output_file + '_' + str(file_counter)
                 file_counter += 1
-            elif Reporter_options.annotation_type[1] == "Multiple_Combined_GFFs" or Reporter_options.annotation_type[1] == "Multiple_Genomes":
+            elif Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs":
                 tmp_filename = gff.split('/')[-1].split('.gff')[0]  # could be .fa/.fasta etc
                 Reporter_options.output_file = output_file.replace('_StORF-Reporter',tmp_filename + '_StORF-Reporter')
             else:
                 Reporter_options.output_file = output_file
 
 
             if Reporter_options.verbose == True:
@@ -832,15 +830,15 @@
                 Contigs, Reporter_options = run_UR_Extractor_Matched(Reporter_options, gff)
             ################## Find StORFs in URs - Setup StORF_Reporter-Finder Run
             Reporter_StORFs = StORF_Reported(Reporter_options, Contigs)
             StORF_Filler(Reporter_options, Reporter_StORFs)
             if Reporter_options.verbose == True:
                 print("Finished: " + gff.split('/')[-1])  # Will add number of additional StORFs here`
 
-    ####### Run Pyrodigal and then Single_Genome on either a single or directory of FASTA files
+    ####### Run Pyrodigal and then StORF-Reporter on either a single or directory of FASTA files
     elif Reporter_options.annotation_type[0] == 'Pyrodigal' and Reporter_options.annotation_type[1] in ("Single_FASTA", "Multiple_FASTA"):  # needs cleaning
         Reporter_options.gene_ident = "gene"
         if os.path.isdir(Reporter_options.path) and Reporter_options.annotation_type[1]  == "Multiple_FASTA":
             fasta_list = list(pathlib.Path(Reporter_options.path).glob('*.fasta'))
             fasta_list.extend(list(pathlib.Path(Reporter_options.path).glob('*.fna')))
             fasta_list.extend(list(pathlib.Path(Reporter_options.path).glob('*.fa')))
             fasta_list = list(map(str, fasta_list))
```

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/StORF_Adder.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/StORF_Adder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/UR_Lenghts.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/UR_Lenghts.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/Tools/Un_StORFed.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/Tools/Un_StORFed.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter/UR_Extractor.py` & `StORF-Reporter-1.0.1/src/StORF_Reporter/UR_Extractor.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/PKG-INFO` & `StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 1.0.0
+Version: 1.0.1
 Summary: StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 Home-page: https://github.com/NickJD/StORF-Reporter
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/StORF-Reporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -73,15 +73,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.1: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -183,15 +183,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -221,15 +221,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.1: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -285,15 +285,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.1: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -318,15 +318,15 @@
 StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
 ```
 
 ```python
 usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
                         [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.1: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.0/src/StORF_Reporter.egg-info/SOURCES.txt` & `StORF-Reporter-1.0.1/src/StORF_Reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

