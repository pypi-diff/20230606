# Comparing `tmp/SBILoops-0.2.1.tar.gz` & `tmp/SBILoops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILoops-0.2.1.tar", last modified: Mon Jun  5 22:16:39 2023, max compression
+gzip compressed data, was "SBILoops-0.2.2.tar", last modified: Mon Jun  5 22:41:12 2023, max compression
```

## Comparing `SBILoops-0.2.1.tar` & `SBILoops-0.2.2.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.885929 SBILoops-0.2.1/
--rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-05 22:16:39.886373 SBILoops-0.2.1/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.1/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.631650 SBILoops-0.2.1/SBILoops/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.641968 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     4327 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)       60 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/top_level.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.662660 SBILoops-0.2.1/SBILoops/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.1/SBILoops/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.676958 SBILoops-0.2.1/SBILoops/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.708099 SBILoops-0.2.1/SBILoops/databases/
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.714383 SBILoops-0.2.1/SBILoops/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.722651 SBILoops-0.2.1/SBILoops/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.724872 SBILoops-0.2.1/SBILoops/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.735945 SBILoops-0.2.1/SBILoops/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.741458 SBILoops-0.2.1/SBILoops/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.751666 SBILoops-0.2.1/SBILoops/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/blast_parser.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.755321 SBILoops-0.2.1/SBILoops/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.766072 SBILoops-0.2.1/SBILoops/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.775360 SBILoops-0.2.1/SBILoops/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.784823 SBILoops-0.2.1/SBILoops/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    20850 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.794752 SBILoops-0.2.1/SBILoops/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.805440 SBILoops-0.2.1/SBILoops/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.811117 SBILoops-0.2.1/SBILoops/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.821833 SBILoops-0.2.1/SBILoops/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.829660 SBILoops-0.2.1/SBILoops/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.840507 SBILoops-0.2.1/SBILoops/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.862271 SBILoops-0.2.1/SBILoops/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.874709 SBILoops-0.2.1/SBILoops/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.884158 SBILoops-0.2.1/SBILoops/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/residue/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-05 22:16:39.887630 SBILoops-0.2.1/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      593 2023-06-05 22:16:16.000000 SBILoops-0.2.1/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.421498 SBILoops-0.2.2/
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-05 22:41:12.421886 SBILoops-0.2.2/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.2/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-05 22:41:12.423092 SBILoops-0.2.2/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      589 2023-06-05 22:40:15.000000 SBILoops-0.2.2/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.143442 SBILoops-0.2.2/src/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.157087 SBILoops-0.2.2/src/SBILoops/
+-rw-r--r--   0 patrick    (501) staff       (20)    12913 2023-06-05 22:40:40.000000 SBILoops-0.2.2/src/SBILoops/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.182460 SBILoops-0.2.2/src/SBILoops/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.2/src/SBILoops/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.198025 SBILoops-0.2.2/src/SBILoops/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.229920 SBILoops-0.2.2/src/SBILoops/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.236477 SBILoops-0.2.2/src/SBILoops/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.244974 SBILoops-0.2.2/src/SBILoops/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.248105 SBILoops-0.2.2/src/SBILoops/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.261922 SBILoops-0.2.2/src/SBILoops/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.268490 SBILoops-0.2.2/src/SBILoops/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.279725 SBILoops-0.2.2/src/SBILoops/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/external/blast/blast_parser.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.283844 SBILoops-0.2.2/src/SBILoops/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.294390 SBILoops-0.2.2/src/SBILoops/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.303528 SBILoops-0.2.2/src/SBILoops/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.314657 SBILoops-0.2.2/src/SBILoops/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    20850 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.323120 SBILoops-0.2.2/src/SBILoops/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.335419 SBILoops-0.2.2/src/SBILoops/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.341367 SBILoops-0.2.2/src/SBILoops/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.354043 SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.361192 SBILoops-0.2.2/src/SBILoops/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.373777 SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.397559 SBILoops-0.2.2/src/SBILoops/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.409431 SBILoops-0.2.2/src/SBILoops/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.418104 SBILoops-0.2.2/src/SBILoops/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.2/src/SBILoops/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.2/src/SBILoops/structure/residue/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:41:12.162288 SBILoops-0.2.2/src/SBILoops.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-05 22:41:12.000000 SBILoops-0.2.2/src/SBILoops.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4775 2023-06-05 22:41:12.000000 SBILoops-0.2.2/src/SBILoops.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-05 22:41:12.000000 SBILoops-0.2.2/src/SBILoops.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-05 22:41:12.000000 SBILoops-0.2.2/src/SBILoops.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-06-05 22:41:12.000000 SBILoops-0.2.2/src/SBILoops.egg-info/top_level.txt
```

### Comparing `SBILoops-0.2.1/PKG-INFO` & `SBILoops-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBILoops
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
```

### Comparing `SBILoops-0.2.1/README.md` & `SBILoops-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/SBILoops.egg-info/PKG-INFO` & `SBILoops-0.2.2/src/SBILoops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBILoops
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
```

### Comparing `SBILoops-0.2.1/SBILoops/SBILoops.egg-info/SOURCES.txt` & `SBILoops-0.2.2/src/SBILoops.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,121 @@
 README.md
 setup.cfg
 setup.py
-SBILoops/SBILoops.egg-info/PKG-INFO
-SBILoops/SBILoops.egg-info/SOURCES.txt
-SBILoops/SBILoops.egg-info/dependency_links.txt
-SBILoops/SBILoops.egg-info/requires.txt
-SBILoops/SBILoops.egg-info/top_level.txt
-SBILoops/beans/Executable.py
-SBILoops/beans/File.py
-SBILoops/beans/IndexedNum.py
-SBILoops/beans/JSONer.py
-SBILoops/beans/Path.py
-SBILoops/beans/StorableObject.py
-SBILoops/beans/__init__.py
-SBILoops/beans/butler.py
-SBILoops/beans/singleton.py
-SBILoops/data/Alphabet.py
-SBILoops/data/AminoAcids.py
-SBILoops/data/AtomVariants.py
-SBILoops/data/Element.py
-SBILoops/data/Properties.py
-SBILoops/data/SetDict.py
-SBILoops/data/__init__.py
-SBILoops/databases/CATHlink.py
-SBILoops/databases/DrugBanklink.py
-SBILoops/databases/Enzymelink.py
-SBILoops/databases/GOlink.py
-SBILoops/databases/PDBTMlink.py
-SBILoops/databases/PDBeChemConnect.py
-SBILoops/databases/PDBeChemlink.py
-SBILoops/databases/PDBlink.py
-SBILoops/databases/SCOPlink.py
-SBILoops/databases/TaxIDlink.py
-SBILoops/databases/Uniprotlink.py
-SBILoops/databases/__Uniprotlink.py
-SBILoops/databases/__init__.py
-SBILoops/databases/dblink.py
-SBILoops/databases/uniprot/__init__.py
-SBILoops/databases/uniprot/connect.py
-SBILoops/databases/uniprot/uniprot.py
-SBILoops/error/BlastError.py
-SBILoops/error/FileError.py
-SBILoops/error/SeqAliError.py
-SBILoops/error/__init__.py
-SBILoops/external/__init__.py
-SBILoops/external/CDhit/CDhit.py
-SBILoops/external/CDhit/CDhitExe.py
-SBILoops/external/CDhit/CDhitHomolog.py
-SBILoops/external/CDhit/CDhitList.py
-SBILoops/external/CDhit/__init__.py
-SBILoops/external/DSSP/DSSP.py
-SBILoops/external/DSSP/DSSPExe.py
-SBILoops/external/DSSP/__init__.py
-SBILoops/external/blast/BlastExe.py
-SBILoops/external/blast/BlastHit.py
-SBILoops/external/blast/BlastResult.py
-SBILoops/external/blast/__init__.py
-SBILoops/external/blast/blast_parser.py
-SBILoops/math/__init__.py
-SBILoops/math/stats.py
-SBILoops/sequence/Fasta.py
-SBILoops/sequence/IndexedSeqAli.py
-SBILoops/sequence/SeqAli.py
-SBILoops/sequence/Sequence.py
-SBILoops/sequence/__init__.py
-SBILoops/sequence/alignment/Needleman_Wunsch.py
-SBILoops/sequence/alignment/SeqAli.py
-SBILoops/sequence/alignment/SimilarityMatrix.py
-SBILoops/sequence/alignment/__init__.py
-SBILoops/structure/PDB.py
-SBILoops/structure/__init__.py
-SBILoops/structure/parse_mmCIF.py
-SBILoops/structure/parse_pdb.py
-SBILoops/structure/atom/Atom.py
-SBILoops/structure/atom/AtomOfAminoAcid.py
-SBILoops/structure/atom/AtomOfNucleotide.py
-SBILoops/structure/atom/AtomSeries.py
-SBILoops/structure/atom/__init__.py
-SBILoops/structure/chain/Chain.py
-SBILoops/structure/chain/ChainFrame.py
-SBILoops/structure/chain/ChainOfNucleotide.py
-SBILoops/structure/chain/ChainOfProtein.py
-SBILoops/structure/chain/ProteinChainFrame.py
-SBILoops/structure/chain/__init__.py
-SBILoops/structure/contacts/Complex.py
-SBILoops/structure/contacts/InnerContacts.py
-SBILoops/structure/contacts/__init__.py
-SBILoops/structure/contacts/contact/Contact.py
-SBILoops/structure/contacts/contact/ContactAA.py
-SBILoops/structure/contacts/contact/ContactAH.py
-SBILoops/structure/contacts/contact/ContactAN.py
-SBILoops/structure/contacts/contact/__init__.py
-SBILoops/structure/contacts/inner/PHInnerContact.py
-SBILoops/structure/contacts/inner/PPInnerContact.py
-SBILoops/structure/contacts/inner/__init__.py
-SBILoops/structure/contacts/interface/Interface.py
-SBILoops/structure/contacts/interface/PHInterface.py
-SBILoops/structure/contacts/interface/PNInterface.py
-SBILoops/structure/contacts/interface/PPInterface.py
-SBILoops/structure/contacts/interface/__init__.py
-SBILoops/structure/header/BioMolecule.py
-SBILoops/structure/header/DBreference.py
-SBILoops/structure/header/Experiment.py
-SBILoops/structure/header/Header.py
-SBILoops/structure/header/HeteroAtom.py
-SBILoops/structure/header/MiniRes.py
-SBILoops/structure/header/Molecule.py
-SBILoops/structure/header/SecondaryStructure.py
-SBILoops/structure/header/Site.py
-SBILoops/structure/header/__init__.py
-SBILoops/structure/protein/Arch.py
-SBILoops/structure/protein/SShelper.py
-SBILoops/structure/protein/SecondaryStructure.py
-SBILoops/structure/protein/Sequencer.py
-SBILoops/structure/protein/__init__.py
-SBILoops/structure/residue/Residue.py
-SBILoops/structure/residue/ResidueOfAminoAcid.py
-SBILoops/structure/residue/ResidueOfNucleotide.py
-SBILoops/structure/residue/__init__.py
+src/SBILoops/__init__.py
+src/SBILoops.egg-info/PKG-INFO
+src/SBILoops.egg-info/SOURCES.txt
+src/SBILoops.egg-info/dependency_links.txt
+src/SBILoops.egg-info/requires.txt
+src/SBILoops.egg-info/top_level.txt
+src/SBILoops/beans/Executable.py
+src/SBILoops/beans/File.py
+src/SBILoops/beans/IndexedNum.py
+src/SBILoops/beans/JSONer.py
+src/SBILoops/beans/Path.py
+src/SBILoops/beans/StorableObject.py
+src/SBILoops/beans/__init__.py
+src/SBILoops/beans/butler.py
+src/SBILoops/beans/singleton.py
+src/SBILoops/data/Alphabet.py
+src/SBILoops/data/AminoAcids.py
+src/SBILoops/data/AtomVariants.py
+src/SBILoops/data/Element.py
+src/SBILoops/data/Properties.py
+src/SBILoops/data/SetDict.py
+src/SBILoops/data/__init__.py
+src/SBILoops/databases/CATHlink.py
+src/SBILoops/databases/DrugBanklink.py
+src/SBILoops/databases/Enzymelink.py
+src/SBILoops/databases/GOlink.py
+src/SBILoops/databases/PDBTMlink.py
+src/SBILoops/databases/PDBeChemConnect.py
+src/SBILoops/databases/PDBeChemlink.py
+src/SBILoops/databases/PDBlink.py
+src/SBILoops/databases/SCOPlink.py
+src/SBILoops/databases/TaxIDlink.py
+src/SBILoops/databases/Uniprotlink.py
+src/SBILoops/databases/__Uniprotlink.py
+src/SBILoops/databases/__init__.py
+src/SBILoops/databases/dblink.py
+src/SBILoops/databases/uniprot/__init__.py
+src/SBILoops/databases/uniprot/connect.py
+src/SBILoops/databases/uniprot/uniprot.py
+src/SBILoops/error/BlastError.py
+src/SBILoops/error/FileError.py
+src/SBILoops/error/SeqAliError.py
+src/SBILoops/error/__init__.py
+src/SBILoops/external/__init__.py
+src/SBILoops/external/CDhit/CDhit.py
+src/SBILoops/external/CDhit/CDhitExe.py
+src/SBILoops/external/CDhit/CDhitHomolog.py
+src/SBILoops/external/CDhit/CDhitList.py
+src/SBILoops/external/CDhit/__init__.py
+src/SBILoops/external/DSSP/DSSP.py
+src/SBILoops/external/DSSP/DSSPExe.py
+src/SBILoops/external/DSSP/__init__.py
+src/SBILoops/external/blast/BlastExe.py
+src/SBILoops/external/blast/BlastHit.py
+src/SBILoops/external/blast/BlastResult.py
+src/SBILoops/external/blast/__init__.py
+src/SBILoops/external/blast/blast_parser.py
+src/SBILoops/math/__init__.py
+src/SBILoops/math/stats.py
+src/SBILoops/sequence/Fasta.py
+src/SBILoops/sequence/IndexedSeqAli.py
+src/SBILoops/sequence/SeqAli.py
+src/SBILoops/sequence/Sequence.py
+src/SBILoops/sequence/__init__.py
+src/SBILoops/sequence/alignment/Needleman_Wunsch.py
+src/SBILoops/sequence/alignment/SeqAli.py
+src/SBILoops/sequence/alignment/SimilarityMatrix.py
+src/SBILoops/sequence/alignment/__init__.py
+src/SBILoops/structure/PDB.py
+src/SBILoops/structure/__init__.py
+src/SBILoops/structure/parse_mmCIF.py
+src/SBILoops/structure/parse_pdb.py
+src/SBILoops/structure/atom/Atom.py
+src/SBILoops/structure/atom/AtomOfAminoAcid.py
+src/SBILoops/structure/atom/AtomOfNucleotide.py
+src/SBILoops/structure/atom/AtomSeries.py
+src/SBILoops/structure/atom/__init__.py
+src/SBILoops/structure/chain/Chain.py
+src/SBILoops/structure/chain/ChainFrame.py
+src/SBILoops/structure/chain/ChainOfNucleotide.py
+src/SBILoops/structure/chain/ChainOfProtein.py
+src/SBILoops/structure/chain/ProteinChainFrame.py
+src/SBILoops/structure/chain/__init__.py
+src/SBILoops/structure/contacts/Complex.py
+src/SBILoops/structure/contacts/InnerContacts.py
+src/SBILoops/structure/contacts/__init__.py
+src/SBILoops/structure/contacts/contact/Contact.py
+src/SBILoops/structure/contacts/contact/ContactAA.py
+src/SBILoops/structure/contacts/contact/ContactAH.py
+src/SBILoops/structure/contacts/contact/ContactAN.py
+src/SBILoops/structure/contacts/contact/__init__.py
+src/SBILoops/structure/contacts/inner/PHInnerContact.py
+src/SBILoops/structure/contacts/inner/PPInnerContact.py
+src/SBILoops/structure/contacts/inner/__init__.py
+src/SBILoops/structure/contacts/interface/Interface.py
+src/SBILoops/structure/contacts/interface/PHInterface.py
+src/SBILoops/structure/contacts/interface/PNInterface.py
+src/SBILoops/structure/contacts/interface/PPInterface.py
+src/SBILoops/structure/contacts/interface/__init__.py
+src/SBILoops/structure/header/BioMolecule.py
+src/SBILoops/structure/header/DBreference.py
+src/SBILoops/structure/header/Experiment.py
+src/SBILoops/structure/header/Header.py
+src/SBILoops/structure/header/HeteroAtom.py
+src/SBILoops/structure/header/MiniRes.py
+src/SBILoops/structure/header/Molecule.py
+src/SBILoops/structure/header/SecondaryStructure.py
+src/SBILoops/structure/header/Site.py
+src/SBILoops/structure/header/__init__.py
+src/SBILoops/structure/protein/Arch.py
+src/SBILoops/structure/protein/SShelper.py
+src/SBILoops/structure/protein/SecondaryStructure.py
+src/SBILoops/structure/protein/Sequencer.py
+src/SBILoops/structure/protein/__init__.py
+src/SBILoops/structure/residue/Residue.py
+src/SBILoops/structure/residue/ResidueOfAminoAcid.py
+src/SBILoops/structure/residue/ResidueOfNucleotide.py
+src/SBILoops/structure/residue/__init__.py
```

### Comparing `SBILoops-0.2.1/SBILoops/beans/Executable.py` & `SBILoops-0.2.2/src/SBILoops/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/beans/File.py` & `SBILoops-0.2.2/src/SBILoops/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/beans/IndexedNum.py` & `SBILoops-0.2.2/src/SBILoops/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/beans/Path.py` & `SBILoops-0.2.2/src/SBILoops/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/beans/StorableObject.py` & `SBILoops-0.2.2/src/SBILoops/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/beans/butler.py` & `SBILoops-0.2.2/src/SBILoops/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/beans/singleton.py` & `SBILoops-0.2.2/src/SBILoops/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/Alphabet.py` & `SBILoops-0.2.2/src/SBILoops/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/AminoAcids.py` & `SBILoops-0.2.2/src/SBILoops/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/AtomVariants.py` & `SBILoops-0.2.2/src/SBILoops/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/Element.py` & `SBILoops-0.2.2/src/SBILoops/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/Properties.py` & `SBILoops-0.2.2/src/SBILoops/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/SetDict.py` & `SBILoops-0.2.2/src/SBILoops/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/data/__init__.py` & `SBILoops-0.2.2/src/SBILoops/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/CATHlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/DrugBanklink.py` & `SBILoops-0.2.2/src/SBILoops/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/Enzymelink.py` & `SBILoops-0.2.2/src/SBILoops/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/GOlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/PDBTMlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/PDBeChemlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/PDBlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/SCOPlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/TaxIDlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/Uniprotlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/__Uniprotlink.py` & `SBILoops-0.2.2/src/SBILoops/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/__init__.py` & `SBILoops-0.2.2/src/SBILoops/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/dblink.py` & `SBILoops-0.2.2/src/SBILoops/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/uniprot/connect.py` & `SBILoops-0.2.2/src/SBILoops/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/databases/uniprot/uniprot.py` & `SBILoops-0.2.2/src/SBILoops/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/error/BlastError.py` & `SBILoops-0.2.2/src/SBILoops/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/error/FileError.py` & `SBILoops-0.2.2/src/SBILoops/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/error/SeqAliError.py` & `SBILoops-0.2.2/src/SBILoops/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/CDhit/CDhit.py` & `SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/CDhit/CDhitExe.py` & `SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/CDhit/CDhitHomolog.py` & `SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/CDhit/CDhitList.py` & `SBILoops-0.2.2/src/SBILoops/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/DSSP/DSSP.py` & `SBILoops-0.2.2/src/SBILoops/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/DSSP/DSSPExe.py` & `SBILoops-0.2.2/src/SBILoops/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/blast/BlastExe.py` & `SBILoops-0.2.2/src/SBILoops/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/blast/BlastHit.py` & `SBILoops-0.2.2/src/SBILoops/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/blast/BlastResult.py` & `SBILoops-0.2.2/src/SBILoops/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/external/blast/blast_parser.py` & `SBILoops-0.2.2/src/SBILoops/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/math/stats.py` & `SBILoops-0.2.2/src/SBILoops/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/Fasta.py` & `SBILoops-0.2.2/src/SBILoops/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/IndexedSeqAli.py` & `SBILoops-0.2.2/src/SBILoops/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/SeqAli.py` & `SBILoops-0.2.2/src/SBILoops/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/Sequence.py` & `SBILoops-0.2.2/src/SBILoops/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/alignment/Needleman_Wunsch.py` & `SBILoops-0.2.2/src/SBILoops/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/alignment/SeqAli.py` & `SBILoops-0.2.2/src/SBILoops/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/sequence/alignment/SimilarityMatrix.py` & `SBILoops-0.2.2/src/SBILoops/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/PDB.py` & `SBILoops-0.2.2/src/SBILoops/structure/PDB.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/atom/Atom.py` & `SBILoops-0.2.2/src/SBILoops/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/atom/AtomOfAminoAcid.py` & `SBILoops-0.2.2/src/SBILoops/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/atom/AtomOfNucleotide.py` & `SBILoops-0.2.2/src/SBILoops/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/atom/AtomSeries.py` & `SBILoops-0.2.2/src/SBILoops/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/chain/Chain.py` & `SBILoops-0.2.2/src/SBILoops/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/chain/ChainFrame.py` & `SBILoops-0.2.2/src/SBILoops/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/chain/ChainOfNucleotide.py` & `SBILoops-0.2.2/src/SBILoops/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/chain/ChainOfProtein.py` & `SBILoops-0.2.2/src/SBILoops/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/chain/ProteinChainFrame.py` & `SBILoops-0.2.2/src/SBILoops/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/Complex.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/InnerContacts.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/contact/Contact.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAA.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAH.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAN.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/inner/PHInnerContact.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/inner/PPInnerContact.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/interface/Interface.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/interface/PHInterface.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/interface/PNInterface.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/contacts/interface/PPInterface.py` & `SBILoops-0.2.2/src/SBILoops/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/BioMolecule.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/DBreference.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/Experiment.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/Header.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/HeteroAtom.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/MiniRes.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/Molecule.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/SecondaryStructure.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/Site.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/header/__init__.py` & `SBILoops-0.2.2/src/SBILoops/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/parse_mmCIF.py` & `SBILoops-0.2.2/src/SBILoops/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/parse_pdb.py` & `SBILoops-0.2.2/src/SBILoops/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/protein/Arch.py` & `SBILoops-0.2.2/src/SBILoops/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/protein/SShelper.py` & `SBILoops-0.2.2/src/SBILoops/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/protein/SecondaryStructure.py` & `SBILoops-0.2.2/src/SBILoops/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/protein/Sequencer.py` & `SBILoops-0.2.2/src/SBILoops/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/residue/Residue.py` & `SBILoops-0.2.2/src/SBILoops/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfAminoAcid.py` & `SBILoops-0.2.2/src/SBILoops/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfNucleotide.py` & `SBILoops-0.2.2/src/SBILoops/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.1/setup.py` & `SBILoops-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 
 setup(
     name='SBILoops',
-    version='0.2.1',
+    version='0.2.2',
     license='MIT',
     author="Patrick Gohl",
     author_email='patrick.gohl@upf.edu',
-    packages=find_packages('SBILoops'),
-    package_dir={'': 'SBILoops'},
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     long_description=readme,
     long_description_content_type="text/markdown",
     url='https://github.com/structuralbioinformatics/SBI',
     keywords='Structural Bioinformatics, Loops',
     install_requires=[
           'numpy','pandas','pynion','Requests','scipy','six'
       ],
```

