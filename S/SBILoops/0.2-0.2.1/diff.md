# Comparing `tmp/SBILoops-0.2.tar.gz` & `tmp/SBILoops-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILoops-0.2.tar", last modified: Mon Jun  5 20:35:16 2023, max compression
+gzip compressed data, was "SBILoops-0.2.1.tar", last modified: Mon Jun  5 22:16:39 2023, max compression
```

## Comparing `SBILoops-0.2.tar` & `SBILoops-0.2.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.447921 SBILoops-0.2/
--rw-r--r--   0 patrick    (501) staff       (20)      220 2023-06-05 20:35:16.448207 SBILoops-0.2/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 17:30:37.000000 SBILoops-0.2/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.321856 SBILoops-0.2/SBI/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.333814 SBILoops-0.2/SBI/SBILoops.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)      220 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     3742 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)       60 2023-06-05 20:35:16.000000 SBILoops-0.2/SBI/SBILoops.egg-info/top_level.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.342584 SBILoops-0.2/SBI/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4497 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11690 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14924 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2923 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2/SBI/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.349709 SBILoops-0.2/SBI/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.366255 SBILoops-0.2/SBI/databases/
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8403 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13608 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5564 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5346 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6698 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9105 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1786 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5721 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7083 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7048 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7140 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.368631 SBILoops-0.2/SBI/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4768 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8163 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.373000 SBILoops-0.2/SBI/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.373987 SBILoops-0.2/SBI/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.379007 SBILoops-0.2/SBI/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2246 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2217 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.381204 SBILoops-0.2/SBI/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3321 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3603 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.385593 SBILoops-0.2/SBI/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9086 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12567 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23479 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8066 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/external/blast/blast_parser.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.387319 SBILoops-0.2/SBI/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.393825 SBILoops-0.2/SBI/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6322 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4862 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15039 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.397600 SBILoops-0.2/SBI/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43520 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.401806 SBILoops-0.2/SBI/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    20840 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.406555 SBILoops-0.2/SBI/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3749 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.412100 SBILoops-0.2/SBI/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19958 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13255 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2760 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6874 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4982 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.414934 SBILoops-0.2/SBI/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9007 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3405 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.420532 SBILoops-0.2/SBI/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3803 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3272 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.423590 SBILoops-0.2/SBI/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.428324 SBILoops-0.2/SBI/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11112 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.436707 SBILoops-0.2/SBI/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2279 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3821 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2005 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14751 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1196 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      938 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7642 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8524 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2418 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18690 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14365 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8538 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.443766 SBILoops-0.2/SBI/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19059 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19197 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 20:35:16.447172 SBILoops-0.2/SBI/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10768 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10715 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5354 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2/SBI/structure/residue/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-05 20:35:16.449450 SBILoops-0.2/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      449 2023-06-05 20:34:54.000000 SBILoops-0.2/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.885929 SBILoops-0.2.1/
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-05 22:16:39.886373 SBILoops-0.2.1/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.1/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.631650 SBILoops-0.2.1/SBILoops/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.641968 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4327 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       60 2023-06-05 22:16:39.000000 SBILoops-0.2.1/SBILoops/SBILoops.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.662660 SBILoops-0.2.1/SBILoops/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.1/SBILoops/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.676958 SBILoops-0.2.1/SBILoops/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.708099 SBILoops-0.2.1/SBILoops/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.714383 SBILoops-0.2.1/SBILoops/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.722651 SBILoops-0.2.1/SBILoops/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.724872 SBILoops-0.2.1/SBILoops/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.735945 SBILoops-0.2.1/SBILoops/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.741458 SBILoops-0.2.1/SBILoops/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.751666 SBILoops-0.2.1/SBILoops/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/external/blast/blast_parser.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.755321 SBILoops-0.2.1/SBILoops/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.766072 SBILoops-0.2.1/SBILoops/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.775360 SBILoops-0.2.1/SBILoops/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.784823 SBILoops-0.2.1/SBILoops/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    20850 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.794752 SBILoops-0.2.1/SBILoops/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.805440 SBILoops-0.2.1/SBILoops/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.811117 SBILoops-0.2.1/SBILoops/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.821833 SBILoops-0.2.1/SBILoops/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.829660 SBILoops-0.2.1/SBILoops/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.840507 SBILoops-0.2.1/SBILoops/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.862271 SBILoops-0.2.1/SBILoops/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.874709 SBILoops-0.2.1/SBILoops/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-05 22:16:39.884158 SBILoops-0.2.1/SBILoops/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.1/SBILoops/structure/residue/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-05 22:16:39.887630 SBILoops-0.2.1/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      593 2023-06-05 22:16:16.000000 SBILoops-0.2.1/setup.py
```

### Comparing `SBILoops-0.2/README.md` & `SBILoops-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/beans/Executable.py` & `SBILoops-0.2.1/SBILoops/beans/Executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 date:   03/2013
 
 @oliva's lab
 """
 
 import os
 import subprocess
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 
 class Executable(object):
     """
     Checks the integrity of an executable program
     """
     def __init__(self, executable, path=None, variable_path=None):
```

### Comparing `SBILoops-0.2/SBI/beans/File.py` & `SBILoops-0.2.1/SBILoops/beans/File.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import math
 import gzip
 import warnings
 
 """
 Dependences in SBI library
 """
-from SBI.error import FileError
-from SBI       import SBIglobals
+from SBILoops.error import FileError
+from SBILoops       import SBIglobals
 
 
 class File(object):
     """The File class manages certain aspects of the IO process
 
         File allows to seamless control some aspects about working with files.
         Namely, it will allow to:
@@ -80,15 +80,15 @@
 
         Requirements:
             * os, sys, math, gzip, warnings
             < SBI.error.FileError
             < SBI.SBIglobals
 
         Usage:
-            from SBI.beans.File import File
+            from SBILoops.beans.File import File
             newReadFile = File(file_name = 'test.txt', action = 'r')
             for line in newReadFile.descriptor:
                 //DO STUFF
             newReadFile.close()
             newWriteFile = File(file_name = 'test.txt', action = 'w', overwrite = True)
             newWriteFile.write(//STUFF)
             newWriteFile.close()
```

### Comparing `SBILoops-0.2/SBI/beans/IndexedNum.py` & `SBILoops-0.2.1/SBILoops/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/beans/Path.py` & `SBILoops-0.2.1/SBILoops/beans/Path.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import os
 import fnmatch
 import shutil
 
 """
 Dependences in SBI library
 """
-from SBI.error import FileError
+from SBILoops.error import FileError
 from .             import File
-from SBI           import SBIglobals
+from SBILoops           import SBIglobals
 
 class Path(object):
     """Path
 
         Path is a collection of @staticmethod (can be called without declaring an instance of the class) to 
         help in file and directory management.
```

### Comparing `SBILoops-0.2/SBI/beans/StorableObject.py` & `SBILoops-0.2.1/SBILoops/beans/StorableObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 except:  import pickle
 import sys
 
 """
 Dependences in SBI library
 """
 from .   import File
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 class StorableObject(object, metaclass=ABCMeta):
     """StorableObject is an abstract "dumping" class.
 
         This means that it is basically usefull for those who would like to extend this library.
         Basically, it gives the object the hability to be "dumped" on disk and be recovered afterwards.
```

### Comparing `SBILoops-0.2/SBI/beans/butler.py` & `SBILoops-0.2.1/SBILoops/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/beans/singleton.py` & `SBILoops-0.2.1/SBILoops/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/Alphabet.py` & `SBILoops-0.2.1/SBILoops/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/AminoAcids.py` & `SBILoops-0.2.1/SBILoops/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/AtomVariants.py` & `SBILoops-0.2.1/SBILoops/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/Element.py` & `SBILoops-0.2.1/SBILoops/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/Properties.py` & `SBILoops-0.2.1/SBILoops/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/SetDict.py` & `SBILoops-0.2.1/SBILoops/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/data/__init__.py` & `SBILoops-0.2.1/SBILoops/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/databases/CATHlink.py` & `SBILoops-0.2.1/SBILoops/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/databases/DrugBanklink.py` & `SBILoops-0.2.1/SBILoops/databases/DrugBanklink.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 """
 import os, re
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI.databases import drugBankftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
+from SBILoops.databases import drugBankftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
 
 class DrugBanklink(object):
     def __init__(self, local = None):
         self._local    = os.path.abspath(local)
         self._tagets   = None
         self._main     = None
         self._drugfile = None
```

### Comparing `SBILoops-0.2/SBI/databases/Enzymelink.py` & `SBILoops-0.2.1/SBILoops/databases/Enzymelink.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 """
 import os, re
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI.databases import Enzymeftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
+from SBILoops.databases import Enzymeftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
 
 class Enzymelink(object):
     """The Enzymelink class controls the download and parsing of Enzyme database
 
     """
     def __init__(self, local = None):
         self._local   = os.path.abspath(local)
```

### Comparing `SBILoops-0.2/SBI/databases/GOlink.py` & `SBILoops-0.2.1/SBILoops/databases/GOlink.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 """
 import os, re
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI.databases import GOftp, GOnamespace
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
+from SBILoops.databases import GOftp, GOnamespace
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
 
 class GOlink(object):
     """The GOlink class controls the download and parsing of GO database
 
     """
     def __init__(self, local = None):
         self._local   = os.path.abspath(local)
```

### Comparing `SBILoops-0.2/SBI/databases/PDBTMlink.py` & `SBILoops-0.2.1/SBILoops/databases/PDBTMlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 """
 import os, re
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI.databases import PDBTMftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
+from SBILoops.databases import PDBTMftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
 
 class PDBTMlink(object):
 
     def __init__(self, local = None):
         self._local     = os.path.abspath(local)
         self._main      = None
         self._pdbtmfile = None
```

### Comparing `SBILoops-0.2/SBI/databases/PDBeChemlink.py` & `SBILoops-0.2.1/SBILoops/databases/PDBeChemlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import subprocess
 import warnings
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI               import SBIglobals
-from SBI.databases import PDBeChemftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
-from SBI.data      import element_dic
+from SBILoops               import SBIglobals
+from SBILoops.databases import PDBeChemftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
+from SBILoops.data      import element_dic
 
 class PDBeChemlink(object):
     """The PDBeChemlink class controls the download and parsing of PDBeChem database
 
     """
     def __init__(self, local = None):
         self._local   = os.path.abspath(local)
```

### Comparing `SBILoops-0.2/SBI/databases/PDBlink.py` & `SBILoops-0.2.1/SBILoops/databases/PDBlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import warnings
 import urllib.request, urllib.parse, urllib.error
 import ftplib
 
 """
 Dependences in SBI library
 """
-from SBI               import SBIglobals
-from SBI.structure import PDB
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
-from SBI.databases import PDBftp, PDBrsync
-from SBI.sequence  import Fasta
+from SBILoops               import SBIglobals
+from SBILoops.structure import PDB
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
+from SBILoops.databases import PDBftp, PDBrsync
+from SBILoops.sequence  import Fasta
 
 
 class PDBlink(object):
     """The PBDlink class controls the management of PDB on database level
 
         For some functionalities, it requires rsync (in the path). Thus, it might be limited to unix-derived OS.
```

### Comparing `SBILoops-0.2/SBI/databases/SCOPlink.py` & `SBILoops-0.2.1/SBILoops/databases/SCOPlink.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 """
 import os, re
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI.databases import SCOPftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
+from SBILoops.databases import SCOPftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
 
 class SCOPlink(object):
     def __init__(self, local = None):
         self._local     = os.path.abspath(local)
         self._desc      = None
         self._rel       = None
         if local is not None:
```

### Comparing `SBILoops-0.2/SBI/databases/TaxIDlink.py` & `SBILoops-0.2.1/SBILoops/databases/TaxIDlink.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 import subprocess
 import warnings
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI               import SBIglobals
-from SBI.databases import taxIDftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
+from SBILoops               import SBIglobals
+from SBILoops.databases import taxIDftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
 
 class TaxIDlink(object):
     """The TaxIDlink class controls the download and parsing of TaxID database
 
     """
     def __init__(self, local = None):
         self._local   = os.path.abspath(local)
```

### Comparing `SBILoops-0.2/SBI/databases/Uniprotlink.py` & `SBILoops-0.2.1/SBILoops/databases/Uniprotlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import subprocess
 import warnings
 import urllib.request, urllib.parse, urllib.error
 
 """
 Dependences in SBI library
 """
-from SBI               import SBIglobals
-from SBI.databases import Uniprotftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
-from SBI.beans.StorableObject     import StorableObject
+from SBILoops               import SBIglobals
+from SBILoops.databases import Uniprotftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
+from SBILoops.beans.StorableObject     import StorableObject
 
 class Uniprotlink(object):
     """The Uniprotlink class controls the download and parsing of Uniprot database
 
     """
     def __init__(self, local = None):
         self._local   = os.path.abspath(local)
```

### Comparing `SBILoops-0.2/SBI/databases/__Uniprotlink.py` & `SBILoops-0.2.1/SBILoops/databases/__Uniprotlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import subprocess
 import warnings
 import urllib
 
 """
 Dependences in SBI library
 """
-from SBI               import SBIglobals
-from SBI.databases import Uniprotftp
-from SBI.beans.Path     import Path
-from SBI.beans.File     import File
-from SBI.beans.StorableObject     import StorableObject
+from SBILoops               import SBIglobals
+from SBILoops.databases import Uniprotftp
+from SBILoops.beans.Path     import Path
+from SBILoops.beans.File     import File
+from SBILoops.beans.StorableObject     import StorableObject
 
 
 class Uniprotlink(object):
     """The Uniprotlink class controls the download and parsing of Uniprot database
 
     """
     def __init__(self, local = None):
```

### Comparing `SBILoops-0.2/SBI/databases/__init__.py` & `SBILoops-0.2.1/SBILoops/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/databases/dblink.py` & `SBILoops-0.2.1/SBILoops/databases/dblink.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from datetime import date
 # import time
 import urllib
 
 import os
 import json
 
-from SBI.beans import Path
-from SBI.beans import File
-from SBI       import SBIglobals as SBIg
+from SBILoops.beans import Path
+from SBILoops.beans import File
+from SBILoops       import SBIglobals as SBIg
 
 
 class DBlink(object):
     '''
     Manages the connection to databases.
     It creates a local copy of the DB that can be queried a posteriori.
     '''
```

### Comparing `SBILoops-0.2/SBI/databases/uniprot/connect.py` & `SBILoops-0.2.1/SBILoops/databases/uniprot/connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 
-from SBI.databases import DBlink
+from SBILoops.databases import DBlink
 from uniprot       import Uniprot
-from SBI.beans     import File
-from SBI           import SBIglobals as SBIg
+from SBILoops.beans     import File
+from SBILoops           import SBIglobals as SBIg
 
 
 class Connect(DBlink):
     '''
     Manages the connection to the [Uniprot](http://www.uniprot.org/) database.
     '''
     _FTP = 'ftp://ftp.uniprot.org/pub/databases/uniprot/current_release/knowledgebase/complete/'
```

### Comparing `SBILoops-0.2/SBI/databases/uniprot/uniprot.py` & `SBILoops-0.2.1/SBILoops/databases/uniprot/uniprot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from SBI.beans    import JSONer
-from SBI.sequence import Sequence
+from SBILoops.beans    import JSONer
+from SBILoops.sequence import Sequence
 
 
 class Uniprot(JSONer):
 
     def __init__(self, entry_name, status):
         '''
         @param:    entry_name
```

### Comparing `SBILoops-0.2/SBI/error/BlastError.py` & `SBILoops-0.2.1/SBILoops/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/error/FileError.py` & `SBILoops-0.2.1/SBILoops/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/error/SeqAliError.py` & `SBILoops-0.2.1/SBILoops/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/external/CDhit/CDhit.py` & `SBILoops-0.2.1/SBILoops/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/external/CDhit/CDhitExe.py` & `SBILoops-0.2.1/SBILoops/external/CDhit/CDhitExe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 jbonet @ boliva's lab 2013
 '''
 
 import os, sys, time, copy, re, configparser
 
-from SBI.beans.Executable import Executable
-from SBI.beans.File       import File
-from SBI.external.CDhit   import CDhitList  as CHL
+from SBILoops.beans.Executable import Executable
+from SBILoops.beans.File       import File
+from SBILoops.external.CDhit   import CDhitList  as CHL
 
 global default_configuration_file
 default_configuration_file = os.path.join(os.path.normpath(os.path.join(os.path.dirname(__file__),'..')),'configSBI.txt')
 
 class CDhitExe(object):
 
     def __init__(self, fasta, threshold, output_dir = None, execute = True):
```

### Comparing `SBILoops-0.2/SBI/external/CDhit/CDhitHomolog.py` & `SBILoops-0.2.1/SBILoops/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/external/CDhit/CDhitList.py` & `SBILoops-0.2.1/SBILoops/external/CDhit/CDhitList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from SBI.beans.StorableObject import StorableObject
-from SBI.beans.File           import File
+from SBILoops.beans.StorableObject import StorableObject
+from SBILoops.beans.File           import File
 from .CDhit         import CDhit
 from .CDhitHomolog  import CDhitHomolog
 
 class CDhitList(StorableObject):
     def __init__(self, cdhitfile):
         self._clusters  = []
         self._allseqids = {}
```

### Comparing `SBILoops-0.2/SBI/external/DSSP/DSSP.py` & `SBILoops-0.2.1/SBILoops/external/DSSP/DSSP.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @oliva's lab
 """
 
 global exposed_threshold
 exposed_threshold = 2.5 #Why? DSSP exposition refers only to secondary chain (aprox.) see PMID: 15768403
 
-from SBI.data import aminoacids3to1, aminoacids_surface
+from SBILoops.data import aminoacids3to1, aminoacids_surface
 
 class DSSP(object):
     """
     The {DSSP} stores the dssp prediction
     """
     def __init__(self, secondary_structure, accessibility, AAtype):
```

### Comparing `SBILoops-0.2/SBI/external/DSSP/DSSPExe.py` & `SBILoops-0.2.1/SBILoops/external/DSSP/DSSPExe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 jbonet @ boliva's lab 2013
 '''
 
 import os
 import sys
 import configparser
 
-from SBI.beans.Executable import Executable
+from SBILoops.beans.Executable import Executable
 from .DSSP                 import DSSP       as DSSP
 
 
 class DSSPExe(object):
     
     default_config_file = os.path.join(
         os.path.normpath(
```

### Comparing `SBILoops-0.2/SBI/external/blast/BlastExe.py` & `SBILoops-0.2.1/SBILoops/external/blast/BlastExe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 '''
 Check BLAST user's guide at: http://www.ncbi.nlm.nih.gov/books/NBK1763/
 
 jbonet @ boliva's lab 2013
 '''
 import os, sys, time, copy, re, configparser
 
-from SBI.beans.Executable    import Executable
-from SBI.beans.File     import File
-from SBI.sequence  import Fasta      as Fasta
-from SBI.error     import BlastError as BE
-from SBI           import SBIglobals
+from SBILoops.beans.Executable    import Executable
+from SBILoops.beans.File     import File
+from SBILoops.sequence  import Fasta      as Fasta
+from SBILoops.error     import BlastError as BE
+from SBILoops           import SBIglobals
 
-from SBI.external.blast import BlastResult as BR
-from SBI.external.blast import BlastHit    as BH
+from SBILoops.external.blast import BlastResult as BR
+from SBILoops.external.blast import BlastHit    as BH
 
 global default_configuration_file
 default_configuration_file = os.path.join(os.path.normpath(os.path.join(os.path.dirname(__file__),'..')),'configSBI.txt')
 
 class BlastExe(object):
 
     def __init__(self, database, search_type = 'prot'):
```

### Comparing `SBILoops-0.2/SBI/external/blast/BlastHit.py` & `SBILoops-0.2.1/SBILoops/external/blast/BlastHit.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
           with xml.dom.minidom parsing capabilities.
 
                                    ############################################ 
                                         jbonet @ boliva's lab        2011
 """
 import re
 
-from SBI.sequence import IndexedSeqAli as IndexedSeqAli
+from SBILoops.sequence import IndexedSeqAli as IndexedSeqAli
 from collections      import Counter
 class BlastHit(IndexedSeqAli):    
     """
     The BlastHit object stores all the data related to a blast XML output hit.
     
     That means the data inside each <Hit> tag of the blast XML file which corresponds to a single blast match to the query.
```

### Comparing `SBILoops-0.2/SBI/external/blast/BlastResult.py` & `SBILoops-0.2.1/SBILoops/external/blast/BlastResult.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
                                         jbonet @ boliva's lab        2011
 """
 
 '''
     Supporting Modules
 '''
 import os, sys, pydoc, warnings, gzip
-from SBI.error import BlastError as BE
-from SBI.beans.StorableObject import StorableObject
-from SBI           import SBIglobals
+from SBILoops.error import BlastError as BE
+from SBILoops.beans.StorableObject import StorableObject
+from SBILoops           import SBIglobals
 
 try:
     import pickle as pickle
 except:
     import pickle
 
 class BlastResult(StorableObject):
```

### Comparing `SBILoops-0.2/SBI/external/blast/blast_parser.py` & `SBILoops-0.2.1/SBILoops/external/blast/blast_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from . import BlastResult as BR
 from . import BlastHit    as BH
-from SBI.error          import BlastError  as BE
-from SBI                    import SBIglobals
+from SBILoops.error          import BlastError  as BE
+from SBILoops                    import SBIglobals
 
 
 from xml.dom.minidom import parseString
 import sys
 
 def parse_blast(query_sequence, blast_output_file, selfHit, hitIDformat):
     '''
```

### Comparing `SBILoops-0.2/SBI/math/stats.py` & `SBILoops-0.2.1/SBILoops/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/sequence/Fasta.py` & `SBILoops-0.2.1/SBILoops/sequence/Fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 @oliva's lab
 """
 
 import subprocess, sys
 
-from SBI.beans.File    import File
-from SBI.sequence import Sequence
-from SBI              import SBIglobals
+from SBILoops.beans.File    import File
+from SBILoops.sequence import Sequence
+from SBILoops              import SBIglobals
 
 class Fasta(object):
 
     def __init__(self, fasta_file):
 
         if isinstance(fasta_file, str):
             self._file = File(file_name = fasta_file, action = 'r')
```

### Comparing `SBILoops-0.2/SBI/sequence/IndexedSeqAli.py` & `SBILoops-0.2.1/SBILoops/sequence/IndexedSeqAli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 jbonet @ oliva's lab 2013
 '''
 import re
 
-from SBI.error    import SeqAliError as SAE
-from SBI.sequence import SeqAli      as SeqAli
-from SBI.beans.IndexedNum    import IndexedNum
+from SBILoops.error    import SeqAliError as SAE
+from SBILoops.sequence import SeqAli      as SeqAli
+from SBILoops.beans.IndexedNum    import IndexedNum
 
 class IndexedSeqAli(SeqAli):
 
 	def __init__(self, sequences, sequenceInits, identities = None, positives = None, gaps = None):
 
 		super(IndexedSeqAli, self).__init__(sequences, sequenceInits, identities, positives, gaps)
```

### Comparing `SBILoops-0.2/SBI/sequence/SeqAli.py` & `SBILoops-0.2.1/SBILoops/sequence/SeqAli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Iterables of SeqAli refer to the alignment
 
 jbonet @ oliva's lab 2013
 '''
 import re
 from collections import Counter
 
-from SBI.error    import SeqAliError as SAE
-from SBI.sequence import Sequence    as Sequence
+from SBILoops.error    import SeqAliError as SAE
+from SBILoops.sequence import Sequence    as Sequence
 
 class SeqAli(object):
 
 	def __init__(self, sequences, sequenceInits, identities = None, positives = None, gaps = None):
 
 		if not isinstance(sequences, list): 	 raise AttributeError('Sequences must be added in a list\n')
 		if not isinstance(sequenceInits, list):	 raise AttributeError('Sequence inits must be added in a list\n')
```

### Comparing `SBILoops-0.2/SBI/sequence/Sequence.py` & `SBILoops-0.2.1/SBILoops/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/sequence/alignment/Needleman_Wunsch.py` & `SBILoops-0.2.1/SBILoops/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/sequence/alignment/SeqAli.py` & `SBILoops-0.2.1/SBILoops/sequence/alignment/SeqAli.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 @class: Rost
 @class: SeqAliError
 '''
 import re
 import decimal
 import math
 
-from SBI.sequence import Sequence
-from SBI.beans    import IndexedNum
+from SBILoops.sequence import Sequence
+from SBILoops.beans    import IndexedNum
 
 
 class SeqAli(object):
     '''
     Sequence alignment container.
     Capacity for multiple sequence alignment.
     Iterable. Iteration refers to the *alignment position*, which starts in *1*
```

### Comparing `SBILoops-0.2/SBI/sequence/alignment/SimilarityMatrix.py` & `SBILoops-0.2.1/SBILoops/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/PDB.py` & `SBILoops-0.2.1/SBILoops/structure/PDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 @oliva's lab
 """
 
 import numpy
 
 from .chain import ChainOfProtein, ChainOfNucleotide
 
-from SBI.beans.StorableObject import StorableObject
-from SBI.beans.File           import File
+from SBILoops.beans.StorableObject import StorableObject
+from SBILoops.beans.File           import File
 
 
 class PDB(StorableObject):
 
     """
     A {PDB} is a collection of {Chain}
     """
```

### Comparing `SBILoops-0.2/SBI/structure/atom/Atom.py` & `SBILoops-0.2.1/SBILoops/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/atom/AtomOfAminoAcid.py` & `SBILoops-0.2.1/SBILoops/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/atom/AtomOfNucleotide.py` & `SBILoops-0.2.1/SBILoops/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/atom/AtomSeries.py` & `SBILoops-0.2.1/SBILoops/structure/atom/AtomSeries.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 # External Libraries
 import numpy as np
 from numpy.linalg import norm
 import pandas as pd
 
 # This Library
-from SBI.structure.io import mmNone
-from SBI.structure.Frame3D import mandatory_fields, frame3D_classify
+from SBILoops.structure.io import mmNone
+from SBILoops.structure.Frame3D import mandatory_fields, frame3D_classify
 
 __all__ = ['AtomSeries', 'VirtualAtom']
 
 
 class AtomSeries( pd.Series ):
     """A single Atom data.
     """
@@ -101,15 +101,15 @@
                 return frame3D_classify(AtomSeries(*args, **kwargs))
             except AtomSeriesCreationError:
                 return frame3D_classify(pd.Series(*args, **kwargs))
         return f
 
     @property
     def _constructor_expanddim( self ):
-        from SBI.structure import Frame3D
+        from SBILoops.structure import Frame3D
 
         def f(*args, **kwargs):
             return frame3D_classify(Frame3D(*args, **kwargs))
         return f
 
 
 class VirtualAtom( AtomSeries ):
```

### Comparing `SBILoops-0.2/SBI/structure/chain/Chain.py` & `SBILoops-0.2.1/SBILoops/structure/chain/Chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import warnings
 import copy
 import numpy
 import re
 
 from ..atom       import Atom
 from ..residue    import Residue, ResidueOfAminoAcid, ResidueOfNucleotide
-from SBI.data     import aminoacids_main1
-from SBI          import SBIglobals
+from SBILoops.data     import aminoacids_main1
+from SBILoops          import SBIglobals
 
 
 class Chain(object):
     """
     A {Chain} represents a collection of {Residue}s
     """
     chaintype   = 'O'
```

### Comparing `SBILoops-0.2/SBI/structure/chain/ChainFrame.py` & `SBILoops-0.2.1/SBILoops/structure/chain/ChainFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 # External Libraries
 import pandas as pd
 import numpy as np
 
 # This Library
 from ..Frame3D import Frame3D
-from SBI.core import core
-from SBI.data import alphabet
+from SBILoops.core import core
+from SBILoops.data import alphabet
 
 __all__ = ['ChainFrame', 'ProteinChainFrame', 'NucleotideChainFrame']
 
 CF = TypeVar('CF', bound='ChainFrame')
 
 
 class ChainFrame( Frame3D ):
@@ -335,15 +335,15 @@
         :param bool minimize: If :data:`True`, ignore data from DSSP output that is not secondary structure
             assignation or accessibility.
         :param str simplify: Secondary structure codes to simplify. ``H``, ``E`` and ``L`` are ignored if provided,
             as they cannot be simplified. The default represents the maximum possible simplification.
 
         :return: :class:`.DSSPFrame`
         """
-        from SBI.external import DSSPExe
+        from SBILoops.external import DSSPExe
 
         tmppdb = tmppdb if tmppdb is not None else os.path.join(gettempdir(), '{}.pdb'.format(os.getpid()))
         tmpdssp = tmpdssp if tmpdssp is not None else os.path.join(gettempdir(), '{}.dssp'.format(os.getpid()))
         if not os.path.isfile(tmppdb):
             self.dehydrate(False).remove_heteroatoms(False).write(tmppdb, format='pdb', force=False, clean=False)
         dssp = DSSPExe(pdb=tmppdb, dssp=tmpdssp, cleanpdb=cleanfiles, cleandssp=cleanfiles, minimize=minimize).dsspdata.simplify(simplify)
```

### Comparing `SBILoops-0.2/SBI/structure/chain/ChainOfNucleotide.py` & `SBILoops-0.2.1/SBILoops/structure/chain/ChainOfNucleotide.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @oliva's lab
 """
 
 from ..atom       import Atom,    AtomOfNucleotide
 from ..residue    import Residue, ResidueOfNucleotide
 from .            import Chain
-from SBI.data import nucleic3to1
+from SBILoops.data import nucleic3to1
 
 class ChainOfNucleotide(Chain):
     """
     A {NucleotideChain} represents a collection of {AminoAcids}s
     """
     chaintype   = 'N'
     atomtype    = AtomOfNucleotide
```

### Comparing `SBILoops-0.2/SBI/structure/chain/ChainOfProtein.py` & `SBILoops-0.2.1/SBILoops/structure/chain/ChainOfProtein.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from ..atom     import AtomOfAminoAcid
 from ..residue  import ResidueOfAminoAcid
 from .          import Chain
 from ..protein  import SShelper
 from ..protein  import Sequencer
-from SBI.data   import aminoacids3to1
+from SBILoops.data   import aminoacids3to1
 
 import numpy         as np
 
 
 class ChainOfProtein(Chain):
     """
     A {ProteinChain} represents a collection of {AminoAcids}s
```

### Comparing `SBILoops-0.2/SBI/structure/chain/ProteinChainFrame.py` & `SBILoops-0.2.1/SBILoops/structure/chain/ProteinChainFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Standard Libraries
 import warnings
 
 # External Libraries
 import pandas as pd
 
 # This Library
-from SBI.data import aminoacids_main3, nucleic_main
+from SBILoops.data import aminoacids_main3, nucleic_main
 from ..Frame3D import Frame3D
 from ..residue import ResidueFrame
 
 __all__ = ['ChainFrame', 'ProteinChainFrame', 'NucleotideChainFrame']
 
 
 class ChainFrame( Frame3D ):
@@ -88,15 +88,15 @@
             if (self[self._current_comp].isin(aminoacids_main3) == True).any():
                 return ProteinChainFrame(self).__finalize__(other, 'inherit')
             if (self[self._current_comp].isin(nucleic_main) == True).any():
                 return NucleotideChainFrame(self).__finalize__(other, 'inherit')
             return self._inheritance(other)
         if method == 'concat':
             if len(self._current_model[self._current_asym].unique()) > 1:
-                from SBI.structure import PDBFrame
+                from SBILoops.structure import PDBFrame
                 return PDBFrame(self)
         return self
 
 
 class ProteinChainFrame( ChainFrame ):
     _subtyp = 'protein_chain_frame'
```

### Comparing `SBILoops-0.2/SBI/structure/contacts/Complex.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/Complex.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 author: jbonet
 date:   02/2014
 
 @oliva's lab
 """
 from .   import PPInterface, PNInterface, PHInterface
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 class Complex(object):
     def __init__(self, pdb, biomolecule = False, PPI = True, PPI_type = "cb",  PPI_distance = 12,
                                                  PNI = True, PNI_type = "min", PNI_distance = 8,
                                                  PHI = True, PHI_type = "min", PHI_distance = 6):
         self._pdb          = pdb
         self._biomolecule  = biomolecule
```

### Comparing `SBILoops-0.2/SBI/structure/contacts/InnerContacts.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/InnerContacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 author: jbonet
 date:   02/2014
 
 @oliva's lab
 """
 from .   import PPInnerContact, PHInnerContact
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 class InnerContacts(object):
     def __init__(self, pdb, AA = False, AA_type = "cb",  AA_distance = 12,
                             NC = False, NC_type = "min", NC_distance = 8,
                             HT = True,  HT_type = "min", HT_distance = 6):
         self._pdb          = pdb
```

### Comparing `SBILoops-0.2/SBI/structure/contacts/contact/Contact.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/contacts/contact/ContactAA.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAA.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author: jbonet
 date:   02/2014
 
 @oliva's lab
 """
 
 from .   import Contact
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 class ContactAA(Contact):
 
     available_distance_types = set(["min","ca","cb","geometric","backbone"])
     atomic_types             = set(["min","ca","cb","backbone"])
     description              = 'AminoAmino'
```

### Comparing `SBILoops-0.2/SBI/structure/contacts/contact/ContactAH.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/contacts/contact/ContactAN.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/contact/ContactAN.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 author: jbonet
 date:   02/2014
 
 @oliva's lab
 """
 from .   import Contact
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 class ContactAN(Contact):
 
     available_distance_types = set(["min","geometric","cbbackbone"])
     atomic_types             = set(["min","cbbackbone"])
     description              = 'AminoNucleo'
```

### Comparing `SBILoops-0.2/SBI/structure/contacts/inner/PHInnerContact.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/contacts/inner/PPInnerContact.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/contacts/interface/Interface.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/contacts/interface/PHInterface.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/contacts/interface/PNInterface.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/interface/PNInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author: jbonet
 date:   03/2013
 
 @oliva's lab
 """
 from .         import Interface
 from ..contact import ContactAN
-from SBI       import SBIglobals
+from SBILoops       import SBIglobals
 
 class PNInterface(Interface):
     """
     {Interface} between two protein chains
     """
     def __init__(self, protein         = None,  nucleotide         = None, 
                        threshold_type  = "min", threshold_distance = 8,
```

### Comparing `SBILoops-0.2/SBI/structure/contacts/interface/PPInterface.py` & `SBILoops-0.2.1/SBILoops/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/header/BioMolecule.py` & `SBILoops-0.2.1/SBILoops/structure/header/BioMolecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from SBI.beans.JSONer import JSONer
+from SBILoops.beans.JSONer import JSONer
 
 
 class BioMolecule(JSONer):
     def __init__(self, identifier):
         self._identifier = identifier
         self._matrices   = []
         self._chains     = set()
```

### Comparing `SBILoops-0.2/SBI/structure/header/DBreference.py` & `SBILoops-0.2.1/SBILoops/structure/header/DBreference.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from SBI              import SBIglobals
+from SBILoops              import SBIglobals
 from .                import process_DBREF_line
-from SBI.beans.JSONer import JSONer
+from SBILoops.beans.JSONer import JSONer
 
 
 class DBref(JSONer):
 
     '''
     {DBRef} includes the reference data to the PDB-CHAIN from:
     Known database-references include:
```

### Comparing `SBILoops-0.2/SBI/structure/header/Experiment.py` & `SBILoops-0.2.1/SBILoops/structure/header/Experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from SBI.data import crystal_method_has_resolution
+from SBILoops.data import crystal_method_has_resolution
 from . import process_EXPERIMENT_line, process_RESOLUTION_line
 from . import process_RFACTOR_line, process_FREER_line
-from SBI.beans.JSONer import JSONer
+from SBILoops.beans.JSONer import JSONer
 
 
 class Experiment(JSONer):
     def __init__(self, line):
         self._xpdta      = process_EXPERIMENT_line(line)
         self._res        = None
         self._rfactor    = None
```

### Comparing `SBILoops-0.2/SBI/structure/header/Header.py` & `SBILoops-0.2.1/SBILoops/structure/header/Header.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .DBreference        import DBref
 from .Site               import Site
 from .HeteroAtom         import Hetero
 from .SecondaryStructure import HelixInfo
 from .SecondaryStructure import SheetInfo
 from .SecondaryStructure import TurnInfo
 from .BioMolecule        import BioMolecule
-from SBI.beans.JSONer    import JSONer
+from SBILoops.beans.JSONer    import JSONer
 
 
 class PDBHeader(JSONer):
 
     def __init__(self):
 
         self._pdb        = None     # PDB ID
```

### Comparing `SBILoops-0.2/SBI/structure/header/HeteroAtom.py` & `SBILoops-0.2.1/SBILoops/structure/header/HeteroAtom.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .MiniRes         import MiniResidue
-from SBI.beans.JSONer import JSONer
+from SBILoops.beans.JSONer import JSONer
 
 
 class Hetero(MiniResidue, JSONer):
     '''
     {Hetero} includes all the data related to a heteroatom in the PDB.
     This does not include modified AminoAcids or Nucleotides in the main chain.
     '''
```

### Comparing `SBILoops-0.2/SBI/structure/header/MiniRes.py` & `SBILoops-0.2.1/SBILoops/structure/header/MiniRes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from SBI.beans.IndexedNum import IndexedNum
-from SBI.beans.JSONer     import JSONer
+from SBILoops.beans.IndexedNum import IndexedNum
+from SBILoops.beans.JSONer     import JSONer
 
 
 class MiniResidue(JSONer):
     def __init__(self, restype, position):
         self._type  = restype
         self._chain = None
         self._pos   = None
```

### Comparing `SBILoops-0.2/SBI/structure/header/Molecule.py` & `SBILoops-0.2.1/SBILoops/structure/header/Molecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import process_COMPND_line
 from . import process_SOURCE_line
-from SBI.beans.JSONer     import JSONer
+from SBILoops.beans.JSONer     import JSONer
 import re
 
 
 class Molecule(JSONer):
 
     '''
     Includes the data from COMPND and SOURCE.
```

### Comparing `SBILoops-0.2/SBI/structure/header/SecondaryStructure.py` & `SBILoops-0.2.1/SBILoops/structure/header/SecondaryStructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from SBI.beans.IndexedNum import IndexedNum
-from SBI.beans.JSONer     import JSONer
+from SBILoops.beans.IndexedNum import IndexedNum
+from SBILoops.beans.JSONer     import JSONer
 
 class SecondaryStructureInfo(JSONer):
     # http://www.wwpdb.org/documentation/format32/sect5.html
 
     _sstype = '-'
 
     def __init__(self, line):
```

### Comparing `SBILoops-0.2/SBI/structure/header/Site.py` & `SBILoops-0.2.1/SBILoops/structure/header/Site.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from .MiniRes import MiniResidue
-from SBI.beans.JSONer import JSONer
+from SBILoops.beans.JSONer import JSONer
 
 class Site(JSONer):
 
     def __init__(self, identifier):
         self._id    = identifier
         self._desc  = ''
         self._evid  = ''
```

### Comparing `SBILoops-0.2/SBI/structure/header/__init__.py` & `SBILoops-0.2.1/SBILoops/structure/header/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SBI.beans.IndexedNum import IndexedNum
+from SBILoops.beans.IndexedNum import IndexedNum
 import time
 import re
 
 
 def process_HEADER_line(line):
     '''
     COLUMNS  DATA TYPE    FIELD           DEFINITION
```

### Comparing `SBILoops-0.2/SBI/structure/parse_mmCIF.py` & `SBILoops-0.2.1/SBILoops/structure/parse_mmCIF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from SBI.data       import aminoacids3to1, nucleic3to1
+from SBILoops.data       import aminoacids3to1, nucleic3to1
 from .chain         import Chain, ChainOfProtein, ChainOfNucleotide
 import gzip
 import re
 
 columns_order = [
     "group_PDB",
     "id",
```

### Comparing `SBILoops-0.2/SBI/structure/parse_pdb.py` & `SBILoops-0.2.1/SBILoops/structure/parse_pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SBI.data       import aminoacids3to1, nucleic3to1
+from SBILoops.data       import aminoacids3to1, nucleic3to1
 from .chain         import Chain, ChainOfProtein, ChainOfNucleotide
 from .header.Header import PDBHeader
 import re
 
 
 def read_PDB_header(pdbobject):
```

### Comparing `SBILoops-0.2/SBI/structure/protein/Arch.py` & `SBILoops-0.2.1/SBILoops/structure/protein/Arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 jbonet @ boliva's lab 2013
 """
-from SBI.beans.StorableObject import StorableObject
-from SBI.beans.JSONer         import JSONer
-from SBI.beans.File           import File
+from SBILoops.beans.StorableObject import StorableObject
+from SBILoops.beans.JSONer         import JSONer
+from SBILoops.beans.File           import File
 
 import numpy as np
 from collections import Counter
 
 
 class Arch(StorableObject, JSONer):
```

### Comparing `SBILoops-0.2/SBI/structure/protein/SShelper.py` & `SBILoops-0.2.1/SBILoops/structure/protein/SShelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from collections        import Counter
 from random             import randint
 from ..atom             import AtomOfAminoAcid
-from SBI.external.DSSP  import DSSPExe
+from SBILoops.external.DSSP  import DSSPExe
 from .Arch               import Arch
 from .SecondaryStructure import SecondaryStructure
 
 
 def calculate_dssp(pdb, tmppdb=None, tmpdssp=None, cleanfiles=True):
 
     prefix     = ".".join([pdb.globalID, str(randint(0, 100))])
```

### Comparing `SBILoops-0.2/SBI/structure/protein/SecondaryStructure.py` & `SBILoops-0.2.1/SBILoops/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/protein/Sequencer.py` & `SBILoops-0.2.1/SBILoops/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2/SBI/structure/residue/Residue.py` & `SBILoops-0.2.1/SBILoops/structure/residue/Residue.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @oliva's lab
 """
 
 import numpy         as np
 import scipy.spatial as sp
 
-from SBI import SBIglobals
+from SBILoops import SBIglobals
 
 class Residue(object):
     """
     A {Residue} collects a series of {Atom}
     """
 
     def __init__(self, number, version, Rtype, mode):
```

### Comparing `SBILoops-0.2/SBI/structure/residue/ResidueOfAminoAcid.py` & `SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfAminoAcid.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 author: jbonet
 date:   02/2013
 
 @oliva's lab
 """
 
 from .          import Residue,        ResidueOfNucleotide
-from SBI.data   import aminoacids3to1, aminoacids1to3, aminoacids_polarity_boolean, aminoacids_surface
-from SBI        import SBIglobals
+from SBILoops.data   import aminoacids3to1, aminoacids1to3, aminoacids_polarity_boolean, aminoacids_surface
+from SBILoops        import SBIglobals
 
 import numpy         as np
 import scipy.spatial as sp
 
 class ResidueOfAminoAcid(Residue):
     """
     A {AminoAcid} collects a series of {AminoAtoms}
```

### Comparing `SBILoops-0.2/SBI/structure/residue/ResidueOfNucleotide.py` & `SBILoops-0.2.1/SBILoops/structure/residue/ResidueOfNucleotide.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author: jbonet
 date:   02/2013
 
 @oliva's lab
 """
 
 from .          import Residue
-from SBI.data   import nucleic3to1, nucleic1to3
+from SBILoops.data   import nucleic3to1, nucleic1to3
 import numpy    as np
 
 class ResidueOfNucleotide(Residue):
     """
     A {Nucleotide} collects a series of {NucleotideAtom}s
     """
     def __init__(self, number, version, Rtype, mode):
```

