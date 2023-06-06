# Comparing `tmp/wgd-2.0.15.tar.gz` & `tmp/wgd-2.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.15.tar", last modified: Sat May 20 13:46:37 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.16.tar", last modified: Tue Jun  6 13:41:28 2023, max compression
```

## Comparing `wgd-2.0.15.tar` & `wgd-2.0.16.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.969748 wgd-2.0.15/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.15/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    39373 2023-05-20 13:46:37.969748 wgd-2.0.15/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    39135 2023-05-20 13:42:49.000000 wgd-2.0.15/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    50452 2023-05-20 10:15:19.000000 wgd-2.0.15/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-20 13:46:37.969748 wgd-2.0.15/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-05-20 13:46:11.000000 wgd-2.0.15/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.912264 wgd-2.0.15/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.15/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.945640 wgd-2.0.15/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.15/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.15/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.15/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.15/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   134238 2023-05-19 10:45:47.000000 wgd-2.0.15/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.15/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.15/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103472 2023-05-20 07:48:15.000000 wgd-2.0.15/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.15/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.15/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   113236 2023-05-20 10:17:11.000000 wgd-2.0.15/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-20 13:46:37.968331 wgd-2.0.15/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    39373 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-20 13:46:37.000000 wgd-2.0.15/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.610749 wgd-2.0.16/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.16/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    44508 2023-06-06 13:41:28.610749 wgd-2.0.16/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    39901 2023-06-02 15:36:16.000000 wgd-2.0.16/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    50452 2023-05-30 15:36:15.000000 wgd-2.0.16/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-06-06 13:41:28.610749 wgd-2.0.16/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-06-06 13:40:10.000000 wgd-2.0.16/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.580312 wgd-2.0.16/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.16/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.600718 wgd-2.0.16/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.16/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.16/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.16/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.16/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   134238 2023-05-19 10:45:47.000000 wgd-2.0.16/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.16/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.16/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103616 2023-06-05 09:26:29.000000 wgd-2.0.16/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8792 2023-06-03 13:38:23.000000 wgd-2.0.16/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.16/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   113240 2023-05-28 17:34:16.000000 wgd-2.0.16/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-06 13:41:28.602237 wgd-2.0.16/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    44508 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       51 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-06-06 13:41:28.000000 wgd-2.0.16/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.15/LICENSE` & `wgd-2.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/PKG-INFO` & `wgd-2.0.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: wgd
-Version: 2.0.15
-Summary: wgd
-Home-page: http://github.com/heche-psb/wgd
-Author: Hengchi Chen
-Author-email: heche@psb.vib-ugent.be
-License: GPL
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
 **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
@@ -298,14 +287,16 @@
 Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
 
 **The collinear coalescence inference of phylogeny**
 ```
 wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
 ```
 
+Note that there should be no duplicated gene IDs in the sequence file.
+
 ### wgd focus
 
 **The concatenation-based/coalescence-based phylogenetic inference**
 ```
 wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
 ```
 
@@ -502,14 +493,22 @@
 wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
 ```
 
 ![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
 
 As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
 
+Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
+```
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
+
 An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
 
 ```
 wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
 ```
 
 Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
```

### Comparing `wgd-2.0.15/README.md` & `wgd-2.0.16/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,535 +1,556 @@
-<div align="center">
-
-# `wgd v2` : a suite tool of WGD inference and timing
-
-**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-
-[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-
-[**Introduction**](#Introduction) | 
-[**Installation**](#Installation) | 
-[**Parameters**](#Parameters) | 
-[**Usage**](#Usage) | 
-[**Illustration**](#Illustration) |
-[**Citation**](#Citation)
-
-</div>
-
-`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-
-## Introduction
-
-Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-
-The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-
-## Installation
-
-The easiest way to install `wgd v2` is using PYPI
-
-```
-pip install wgd
-```
-
-To install `wgd v2` in a virtual environment, the following command lines could be used.
-
-```
-git clone <wgd repo>
-cd wgd
-virtualenv -p=python3 ENV (or python3 -m venv ENV)
-source ENV/bin/activate
-pip install -r requirements.txt
-pip install .
-```
-
-When met with permission problem in installation, please try the following command line.
-
-```
-pip install -e .
-```
-
-If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-
-```
-export PATH="$PATH:~/.local/bin/wgd"
-```
-
-Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
-
-## Parameters
-
-There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-
-The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-```
-wgd dmd sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_dmd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
--I, --inflation, the inflation factor for MCL program, default 2.0
--e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
--f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
--ap, --anchorpoints, the anchor points data file, default None
--coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
--sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
--le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
--gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
--kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
--kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
--gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
--n, --nthreads, the number of threads to use, default 4
--oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
--oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
--gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
--mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
--ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
--am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
--sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
--fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
--cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
--te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
--bs, --bins, the number of bins divided in gene length normalization, default 100
--np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
--nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
--bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
--bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
--bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-```
-
-The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-```
-wgd focus families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_focus
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--a, --aligner, which alignment program to use, default mafft
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
---concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
---coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
--sp, --speciestree, species tree darafile for dating, default None
--d, --dating, which molecular dating program to use, default none
--ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
--ns, --nsites, the nsites information for r8s dating, default None
--ot, --outgroup, the outgroup information for r8s dating, default None
--pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
--am, --aamodel, which protein model to be used in mcmctree, default poisson
--ks, flag option, whether to initiate Ks analysis
---annotation, which annotation program to use, default none
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
--ed, --eggnogdata, the eggnog annotation datafile, default None
---pfam, which option to use for pfam annotation, default none
---dmnb, the diamond database for annotation, default None
---hmm, the HMM profile for annotation, default None
---evalue, the e-value cut-off for annotation, default 1e-10
---exepath, the path to the interproscan executable, default None
--f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
- -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
--cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
---beastlgjar, the path to beastLG.jar, default None
---beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
---protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-```
-
-The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-```
-wgd ksd families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_ksd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-```
-
-The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-```
-wgd mix ks_datafile (option)
---------------------------------------------------------------------------------
--f, --filters, the cutoff alignment length, default 300
--r, --ks_range, the Ks range to be considered, default (0.005, 3)
--b, --bins, the number of bins in Ks distribution, default 50
--o, --outdir, the output directory, default wgd_mix
---method, which mixture model to use, default gmm
--n, --components, the range of the number of components to fit, default (1, 4)
--g, --gamma, the gamma parameter for bgmm models, default 0.001
--ni, --n_init, the number of k-means initializations, default 200
--mi, --max_iter, the maximum number of iterations, default 1000
-```
-
-The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-```
-wgd peak ks_datafile (option)
---------------------------------------------------------------------------------
--ap, --anchorpoints, the anchor points datafile, default None
--sm, --segments, the segments datafile, default None
--le, --listelements, the listsegments datafile, default None 
--mp, --multipliconpairs, the multipliconpairs datafile, default None
--o, --outdir, the output directory, default wgd_peak
--af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
--r, --ksrange, range of Ks to be analyzed, default (0, 5)
--bw, --bin_width, bandwidth of Ks distribution, default 0.1
--ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
--m, --method, which mixture model to use, default gmm
---seed, random seed given to initialization, default 2352890
--ei, --em_iter, the number of EM iterations to perform, default 200
--ni, --n_init, the number of k-means initializations, default 200
--n, --components, the range of the number of components to fit, default (1, 4)
---boots, the number of bootstrap replicates of kde, default 200
---weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
--p, --plot, the plotting method to be used, default identical
--bm, --bw_method, the bandwidth method to be used, default silverman
---n_medoids, the number of medoids to fit, default 2
--km, --kdemethod, the kde method to be used, default scipy
---n_clusters, the number of clusters to plot Elbow loss function, default 5
---kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
--gd, --guide, the regime residing anchors, default: segment
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
--f, --family, the family to filter Ks upon, default None
---manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
---ci, the confidence level of log-normal distribution to date, default 95
---hdr, the highest densidy region (HDR) in a given distribution to date, default 95
---heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
--kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-```
-
-The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-```
-wgd syn families gffs (option)
---------------------------------------------------------------------------------
--ks, --ks_distribution, ks distribution datafile, default None
--o, --outdir, the output directory, default wgd_syn
--f, --feature, the feature for parsing gene IDs from GFF files, default gene
--a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--r, --ks_range, the Ks range in colored dotplot, default (0, 5)
---iadhore_options, the parameter setting in iadhore, default 
--ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-```
-wgd viz (option)
---------------------------------------------------------------------------------
--d, --datafile, the Ks datafile, default None
--o, --outdir, the output directory, default wgd_viz
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--gs, --gsmap, the gene name-species name map, default None
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
--iter, --em_iterations, the maximum EM iterations, default 200
--init, --em_initializations, the maximum EM initializations, default 200
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--sm, --segments, the segments data file, default None
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--ap, --anchorpoints, the anchor points datafile, default None
--mt, --multiplicon, the multiplicons datafile, default None
--gt, --genetable, the gene table datafile, default None
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-## Usage
-
-Here we provided the basic usage for each program.
-
-### wgd dmd
-
-**The delineation of whole paranome**
-```
-wgd dmd sequence
-``` 
-
-**The delineation of RBHs**
-```
-wgd dmd sequence1 sequence2
-```
-
-**The delineation of local MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -f sequence1
-```
-
-**The delineation of global MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -gm
-```
-
-**The delineation of orthogroups**
-```
-wgd dmd sequence1 sequence2 sequence3 -oi (option)
-```
-Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-
-**The collinear coalescence inference of phylogeny**
-```
-wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-```
-
-### wgd focus
-
-**The concatenation-based/coalescence-based phylogenetic inference**
-```
-wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-```
-
-**The functional annotation of gene families**
-```
-wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-```
-
-**The phylogenetic dating of WGDs**
-```
-wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-```
-
-### wgd ksd
-
-**The construction of whole paranome *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence
-```
-
-**The construction of orthologous *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence1 sequence2
-```
-
-**The construction of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-```
-
-### wgd mix
-
-**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-```
-wgd mix ksdata
-```
-
-### wgd peak
-
-**The search of crediable *K*<sub>S</sub> range used in WGD dating**
-```
-wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-```
-Note that users can add the flag --heuristic to implement the heuristic search analysis
-
-### wgd syn
-
-**The intra-specific synteny inference**
-```
-wgd syn families gff
-```
-
-**The inter-specific synteny inference**
-```
-wgd syn families gff1 gff2
-```
-
-### wgd viz
-
-**The visualization of *K*<sub>S</sub> age distribution**
-```
-wgd viz -d ksdata
-```
-
-**The visualization of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-```
-
-**The visualization of synteny**
-```
-wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-```
-
-## Illustration
-
-We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-
-The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-
-First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-
-```
-wgd dmd Aquilegia_coerulea
-wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-```
-
-The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
-
-![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
-
-We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
-
-```
-wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-```
-
-As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
-
-![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
-
-The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
-
-![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
-
-The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
-
-![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
-
-A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
-
-![](data/Syndepth.svg)
-
-We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
-
-```
-wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-```
-
-The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
-
-![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
-
-Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
-
-```
-wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
-```
-
-The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
-
-![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
-
-Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
-
-```
-wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
-```
-
-In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
-
-```
-wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-```
-
-The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
-
-```
-(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
-```
-
-![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
-
-As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
-
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
-```
-
-Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
-```
-
-![](data/Raw_Orthologues_Compare_rate.ksd.svg)
-
-As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
-
-Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
-
-```
-Aqcoe6G057800.1 Aquilegia_coerulea
-Vvi_VIT_201s0011g01530.1 Vitis_vinifera
-Pcy_Procy01g08510 Protea_cynaroides
-Aam_Acora.04G142900.1 Acorus_americanus
-```
-
-A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
-```
-
-![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
-
-From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
-
-Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
-```
-
-![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
-
-As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
-
-An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
-
-```
-wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
-```
-
-Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
-
-```
-wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-```
-
-![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
-
-As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
-
-If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
-```
-
-We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
-![](data/Raw_Orthologues.ksd.svg)
-
-## Citation
- 
-Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-
-```
-Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-
-Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-```
-
-For citation of the tools used in wgd, please consult the documentation at
-https://wgd.readthedocs.io/en/latest/index.html#citation.
-
+Metadata-Version: 2.1
+Name: wgd
+Version: 2.0.16
+Summary: wgd
+Home-page: http://github.com/heche-psb/wgd
+Author: Hengchi Chen
+Author-email: heche@psb.vib-ugent.be
+License: GPL
+Description: <div align="center">
+        
+        # `wgd v2` : a suite tool of WGD inference and timing
+        
+        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+        
+        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+        
+        [**Introduction**](#Introduction) | 
+        [**Installation**](#Installation) | 
+        [**Parameters**](#Parameters) | 
+        [**Usage**](#Usage) | 
+        [**Illustration**](#Illustration) |
+        [**Citation**](#Citation)
+        
+        </div>
+        
+        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+        
+        ## Introduction
+        
+        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+        
+        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+        
+        ## Installation
+        
+        The easiest way to install `wgd v2` is using PYPI
+        
+        ```
+        pip install wgd
+        ```
+        
+        To install `wgd v2` in a virtual environment, the following command lines could be used.
+        
+        ```
+        git clone <wgd repo>
+        cd wgd
+        virtualenv -p=python3 ENV (or python3 -m venv ENV)
+        source ENV/bin/activate
+        pip install -r requirements.txt
+        pip install .
+        ```
+        
+        When met with permission problem in installation, please try the following command line.
+        
+        ```
+        pip install -e .
+        ```
+        
+        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+        
+        ```
+        export PATH="$PATH:~/.local/bin/wgd"
+        ```
+        
+        Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+        
+        ## Parameters
+        
+        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+        
+        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+        ```
+        wgd dmd sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_dmd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+        -I, --inflation, the inflation factor for MCL program, default 2.0
+        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+        -ap, --anchorpoints, the anchor points data file, default None
+        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+        -n, --nthreads, the number of threads to use, default 4
+        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+        -bs, --bins, the number of bins divided in gene length normalization, default 100
+        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+        ```
+        
+        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+        ```
+        wgd focus families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_focus
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -a, --aligner, which alignment program to use, default mafft
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+        -sp, --speciestree, species tree darafile for dating, default None
+        -d, --dating, which molecular dating program to use, default none
+        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+        -ns, --nsites, the nsites information for r8s dating, default None
+        -ot, --outgroup, the outgroup information for r8s dating, default None
+        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+        -am, --aamodel, which protein model to be used in mcmctree, default poisson
+        -ks, flag option, whether to initiate Ks analysis
+        --annotation, which annotation program to use, default none
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        -ed, --eggnogdata, the eggnog annotation datafile, default None
+        --pfam, which option to use for pfam annotation, default none
+        --dmnb, the diamond database for annotation, default None
+        --hmm, the HMM profile for annotation, default None
+        --evalue, the e-value cut-off for annotation, default 1e-10
+        --exepath, the path to the interproscan executable, default None
+        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+        --beastlgjar, the path to beastLG.jar, default None
+        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+        ```
+        
+        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+        ```
+        wgd ksd families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_ksd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        ```
+        
+        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+        ```
+        wgd mix ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -f, --filters, the cutoff alignment length, default 300
+        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
+        -b, --bins, the number of bins in Ks distribution, default 50
+        -o, --outdir, the output directory, default wgd_mix
+        --method, which mixture model to use, default gmm
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        -g, --gamma, the gamma parameter for bgmm models, default 0.001
+        -ni, --n_init, the number of k-means initializations, default 200
+        -mi, --max_iter, the maximum number of iterations, default 1000
+        ```
+        
+        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+        ```
+        wgd peak ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -sm, --segments, the segments datafile, default None
+        -le, --listelements, the listsegments datafile, default None 
+        -mp, --multipliconpairs, the multipliconpairs datafile, default None
+        -o, --outdir, the output directory, default wgd_peak
+        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
+        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
+        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+        -m, --method, which mixture model to use, default gmm
+        --seed, random seed given to initialization, default 2352890
+        -ei, --em_iter, the number of EM iterations to perform, default 200
+        -ni, --n_init, the number of k-means initializations, default 200
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        --boots, the number of bootstrap replicates of kde, default 200
+        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+        -p, --plot, the plotting method to be used, default identical
+        -bm, --bw_method, the bandwidth method to be used, default silverman
+        --n_medoids, the number of medoids to fit, default 2
+        -km, --kdemethod, the kde method to be used, default scipy
+        --n_clusters, the number of clusters to plot Elbow loss function, default 5
+        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+        -gd, --guide, the regime residing anchors, default: segment
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+        -f, --family, the family to filter Ks upon, default None
+        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        --ci, the confidence level of log-normal distribution to date, default 95
+        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+        ```
+        
+        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+        ```
+        wgd syn families gffs (option)
+        --------------------------------------------------------------------------------
+        -ks, --ks_distribution, ks distribution datafile, default None
+        -o, --outdir, the output directory, default wgd_syn
+        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
+        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+        --iadhore_options, the parameter setting in iadhore, default 
+        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+        ```
+        wgd viz (option)
+        --------------------------------------------------------------------------------
+        -d, --datafile, the Ks datafile, default None
+        -o, --outdir, the output directory, default wgd_viz
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -gs, --gsmap, the gene name-species name map, default None
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        -iter, --em_iterations, the maximum EM iterations, default 200
+        -init, --em_initializations, the maximum EM initializations, default 200
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -sm, --segments, the segments data file, default None
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -mt, --multiplicon, the multiplicons datafile, default None
+        -gt, --genetable, the gene table datafile, default None
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        ## Usage
+        
+        Here we provided the basic usage for each program.
+        
+        ### wgd dmd
+        
+        **The delineation of whole paranome**
+        ```
+        wgd dmd sequence
+        ``` 
+        
+        **The delineation of RBHs**
+        ```
+        wgd dmd sequence1 sequence2
+        ```
+        
+        **The delineation of local MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -f sequence1
+        ```
+        
+        **The delineation of global MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -gm
+        ```
+        
+        **The delineation of orthogroups**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -oi (option)
+        ```
+        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+        
+        **The collinear coalescence inference of phylogeny**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+        ```
+        
+        Note that there should be no duplicated gene IDs in the sequence file.
+        
+        ### wgd focus
+        
+        **The concatenation-based/coalescence-based phylogenetic inference**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+        ```
+        
+        **The functional annotation of gene families**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+        ```
+        
+        **The phylogenetic dating of WGDs**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+        ```
+        
+        ### wgd ksd
+        
+        **The construction of whole paranome *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence
+        ```
+        
+        **The construction of orthologous *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence1 sequence2
+        ```
+        
+        **The construction of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+        ```
+        
+        ### wgd mix
+        
+        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+        ```
+        wgd mix ksdata
+        ```
+        
+        ### wgd peak
+        
+        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
+        ```
+        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+        ```
+        Note that users can add the flag --heuristic to implement the heuristic search analysis
+        
+        ### wgd syn
+        
+        **The intra-specific synteny inference**
+        ```
+        wgd syn families gff
+        ```
+        
+        **The inter-specific synteny inference**
+        ```
+        wgd syn families gff1 gff2
+        ```
+        
+        ### wgd viz
+        
+        **The visualization of *K*<sub>S</sub> age distribution**
+        ```
+        wgd viz -d ksdata
+        ```
+        
+        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+        ```
+        
+        **The visualization of synteny**
+        ```
+        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+        ```
+        
+        ## Illustration
+        
+        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+        
+        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+        
+        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+        
+        ```
+        wgd dmd Aquilegia_coerulea
+        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+        ```
+        
+        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+        
+        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+        
+        ```
+        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+        
+        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+        
+        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+        
+        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+        
+        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+        
+        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+        
+        ![](data/Syndepth.svg)
+        
+        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+        
+        ```
+        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+        
+        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+        
+        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+        
+        ```
+        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+        ```
+        
+        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+        
+        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+        
+        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+        
+        ```
+        wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+        ```
+        
+        In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+        
+        ```
+        wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+        ```
+        
+        The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+        
+        ```
+        (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+        
+        As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+        
+        If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+        ```
+        
+        Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
+        ```
+        
+        ![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+        
+        As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+        
+        Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+        
+        ```
+        Aqcoe6G057800.1 Aquilegia_coerulea
+        Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+        Pcy_Procy01g08510 Protea_cynaroides
+        Aam_Acora.04G142900.1 Acorus_americanus
+        ```
+        
+        A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+        
+        From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+        
+        Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+        
+        As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+        
+        Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
+        
+        An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+        
+        ```
+        wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+        ```
+        
+        Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+        
+        ```
+        wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+        ```
+        
+        ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+        
+        As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+        
+        If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
+        ```
+        
+        We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+        ![](data/Raw_Orthologues.ksd.svg)
+        
+        ## Citation
+         
+        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+        
+        ```
+        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+        
+        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+        ```
+        
+        For citation of the tools used in wgd, please consult the documentation at
+        https://wgd.readthedocs.io/en/latest/index.html#citation.
+        
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `wgd-2.0.15/cli.py` & `wgd-2.0.16/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
 @click.option('--speciestree', '-sp', default=None, show_default=True,help='species tree to perform rate correction')
 @click.option('--reweight', '-rw', is_flag=True, help='recalculate the weight per species pair')
 @click.option('--onlyrootout', '-or', is_flag=True, help='only consider the outgroup at root')
 @click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
 @click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
 @click.option('--plotkde', '-pk', is_flag=True, help='plot kde curve over histogram')
 @click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
-@click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
+@click.option('--components', '-c', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
 def ksd(**kwargs):
     """
     Paranome and one-to-one ortholog Ks distribution inference pipeline.
 
     Example 1 - whole-paranome:
 
         wgd ksd families.mcl cds.fasta
```

### Comparing `wgd-2.0.15/setup.py` & `wgd-2.0.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.15',
+    version='2.0.16',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.15/test/test_core.py` & `wgd-2.0.16/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/__init__.py` & `wgd-2.0.16/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/beast.py` & `wgd-2.0.16/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/cluster.py` & `wgd-2.0.16/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/codeml.py` & `wgd-2.0.16/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/core.py` & `wgd-2.0.16/wgd/core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/mcmctree.py` & `wgd-2.0.16/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/mix.py` & `wgd-2.0.16/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/peak.py` & `wgd-2.0.16/wgd/peak.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,30 +293,31 @@
             w = w[np.isfinite(x)]
             if len(y) < 2:
                 logging.info("Detected one component with less than 2 elements, will skip it")
                 continue
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
-            ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num+1,np.exp(mean - std**2)))
+            ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num,np.exp(mean - std**2)))
     else:
         for num,color in zip(range(nums),colors):
             mean,std,weight = means[num][0],np.sqrt(stds[num][0][0]),weights[num]
             if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
             else: df_comp = df[df['AnchorKs_GMM_Component']==num].drop_duplicates(subset=['family','node'])
             x = np.array(list(df_comp['node_averaged_dS_outlierexcluded']))
             y = x[np.isfinite(x)]
             if len(y) < 2:
                 logging.info("Detected one component with less than 2 elements, will skip it")
                 continue
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
-            ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num+1,np.exp(mean - std**2)))
-    ax.legend(loc='upper right', fontsize='small',frameon=False)
+            ax.plot(kde_x,scaling*weight*stats.lognorm.pdf(kde_x, scale=np.exp(mean),s=std), c=color, ls='-', lw=1.5, alpha=0.8, label='component {} mode {:.2f}'.format(num,np.exp(mean - std**2)))
+    #ax.legend(loc='upper right', fontsize='small',frameon=False)
+    ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ GMM modeling')
     elif regime=='segment': plt.title('Segment-guided Syntelog $K_\mathrm{S}$ GMM modeling')
     elif regime== 'original': plt.title('Original Anchor $K_\mathrm{S}$ GMM modeling')
@@ -387,15 +388,16 @@
             safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
             ax.set_ylim(0, safe_max)
             ax.axvline(x = mode, color = color, alpha = 0.8, ls = ':', lw = 1)
             upper_HPD,lower_HPD = calculateHPD(y,hdr)
             ax.axvline(x = upper_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
             ax.axvline(x = lower_HPD, color = color, alpha = 0.8, ls = '-.', lw = 1)
             HDRs[num] = (lower_HPD,upper_HPD)
-    ax.legend(loc='upper right', fontsize='small',frameon=False)
+    #ax.legend(loc='upper right', fontsize='small',frameon=False)
+    ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
     ax.set_xticks([0,1,2,3,4,5])
     sns.despine(offset=1)
     if regime=='multiplicon': plt.title('Multilplicon-guided Anchor $K_\mathrm{S}$ GMM modeling')
     elif regime=='segment': plt.title('Segment-guided Syntelog $K_\mathrm{S}$ GMM modeling')
     elif regime== 'original': plt.title('Original Anchor $K_\mathrm{S}$ GMM modeling')
```

### Comparing `wgd-2.0.15/wgd/syn.py` & `wgd-2.0.16/wgd/syn.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 def gff2table(gff, feature, attribute):
     """
     Read a GFF file to a pandas data frame, from a filename.
     """
     rows = []
     with open(gff, "r") as f:
         for l in f.readlines():
-            if l.startswith("#") or l.strip()=='':
+            if l.startswith("#") or l.strip("\n").strip()=='':
                 continue
-            x = l.split("\t")
+            x = l.strip("\n").strip("\t").split("\t")
             #Note here the empty lines from input will make error
             if x[2] == feature:
                 a = getattr(x[-1], attribute)
                 rows.append({"gene": a, "scaffold": x[0], "start": int(x[3]), "or": x[6]})
     df = pd.DataFrame.from_dict(rows).set_index("gene")
     return df
 
@@ -99,14 +99,17 @@
         if not os.path.exists(gdir):
             os.mkdir(gdir)
         lists = {}
         for scaffold, sdf in df.groupby("scaffold"):
             if len(sdf.index) <= 2: continue
             fname = os.path.join(gdir, scaffold)
             with open(fname, "w") as o:
+                if len(list(sdf.sort_values(by=["start"]).index)) != len(set(sdf.sort_values(by=["start"]).index)):
+                    logging.error("There are duplicated gene IDs for given feature and attribute")
+                    exit(1)
                 for g in sdf.sort_values(by=["start"]).index:
                     o.write(g + sdf.loc[g,"or"] + "\n")
             lists[scaffold] = os.path.abspath(fname)
         genomes[sp] = lists
     return genomes
 
 def write_config_adhore(
```

### Comparing `wgd-2.0.15/wgd/utils.py` & `wgd-2.0.16/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.15/wgd/viz.py` & `wgd-2.0.16/wgd/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,16 +524,16 @@
                 logging.info('The corrected mode of species pair {} is {:.2f}'.format(pair,corrected_ks_spair[pair]))
         if pair not in paralog_pair:
             kde = stats.gaussian_kde(y,weights=w,bw_method=0.1)
             kde_y = kde(kde_x)
             mode, maxim = kde_mode(kde_x, kde_y)
             logging.info('The mode of species pair {} is {:.2f}'.format(pair,mode))
             CHF = get_totalH(Hs)
-            scale = CHF*0.1
-            if plotkde: ax.plot(kde_x, kde_y*scale, color=cs[i],alpha=0.4, ls = '--')
+            scaling = CHF*0.1
+            if plotkde: ax.plot(kde_x, kde_y*scaling, color=cs[i],alpha=0.4, ls = '--')
             ax.axvline(x = mode, color = cs[i], alpha = 0.8, ls = ':', lw = 1,label = 'Original mode {:.2f} of {}'.format(mode,pair))
             if corrected_ks_spair != None:
                 if pair in corrected_ks_spair.keys():
                     ax.quiver(mode,maxim*scale, corrected_ks_spair[pair]-mode, 0, angles='xy', scale_units='xy', scale=1,color=cs[i],width=0.005,headwidth=2,headlength=2,headaxislength=2)
     if ap != None:
         df_ap = pd.read_csv(ap,header=0,index_col=0,sep='\t')
         df_ap.loc[:,"pair"] = df_ap[["gene_x", "gene_y"]].apply(lambda x: "__".join(sorted([x[0], x[1]])), axis=1)
```

### Comparing `wgd-2.0.15/wgd.egg-info/PKG-INFO` & `wgd-2.0.16/wgd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,546 +1,556 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.15
+Version: 2.0.16
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
+Description: <div align="center">
+        
+        # `wgd v2` : a suite tool of WGD inference and timing
+        
+        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+        
+        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+        
+        [**Introduction**](#Introduction) | 
+        [**Installation**](#Installation) | 
+        [**Parameters**](#Parameters) | 
+        [**Usage**](#Usage) | 
+        [**Illustration**](#Illustration) |
+        [**Citation**](#Citation)
+        
+        </div>
+        
+        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+        
+        ## Introduction
+        
+        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+        
+        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+        
+        ## Installation
+        
+        The easiest way to install `wgd v2` is using PYPI
+        
+        ```
+        pip install wgd
+        ```
+        
+        To install `wgd v2` in a virtual environment, the following command lines could be used.
+        
+        ```
+        git clone <wgd repo>
+        cd wgd
+        virtualenv -p=python3 ENV (or python3 -m venv ENV)
+        source ENV/bin/activate
+        pip install -r requirements.txt
+        pip install .
+        ```
+        
+        When met with permission problem in installation, please try the following command line.
+        
+        ```
+        pip install -e .
+        ```
+        
+        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+        
+        ```
+        export PATH="$PATH:~/.local/bin/wgd"
+        ```
+        
+        Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+        
+        ## Parameters
+        
+        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+        
+        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+        ```
+        wgd dmd sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_dmd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+        -I, --inflation, the inflation factor for MCL program, default 2.0
+        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+        -ap, --anchorpoints, the anchor points data file, default None
+        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+        -n, --nthreads, the number of threads to use, default 4
+        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+        -bs, --bins, the number of bins divided in gene length normalization, default 100
+        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+        ```
+        
+        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+        ```
+        wgd focus families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_focus
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -a, --aligner, which alignment program to use, default mafft
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+        -sp, --speciestree, species tree darafile for dating, default None
+        -d, --dating, which molecular dating program to use, default none
+        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+        -ns, --nsites, the nsites information for r8s dating, default None
+        -ot, --outgroup, the outgroup information for r8s dating, default None
+        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+        -am, --aamodel, which protein model to be used in mcmctree, default poisson
+        -ks, flag option, whether to initiate Ks analysis
+        --annotation, which annotation program to use, default none
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        -ed, --eggnogdata, the eggnog annotation datafile, default None
+        --pfam, which option to use for pfam annotation, default none
+        --dmnb, the diamond database for annotation, default None
+        --hmm, the HMM profile for annotation, default None
+        --evalue, the e-value cut-off for annotation, default 1e-10
+        --exepath, the path to the interproscan executable, default None
+        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+        --beastlgjar, the path to beastLG.jar, default None
+        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+        ```
+        
+        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+        ```
+        wgd ksd families sequences (option)
+        --------------------------------------------------------------------------------
+        -o, --outdir, the output directory, default wgd_ksd
+        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+        -n, --nthreads, the number of threads to use, default 4
+        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        ```
+        
+        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+        ```
+        wgd mix ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -f, --filters, the cutoff alignment length, default 300
+        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
+        -b, --bins, the number of bins in Ks distribution, default 50
+        -o, --outdir, the output directory, default wgd_mix
+        --method, which mixture model to use, default gmm
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        -g, --gamma, the gamma parameter for bgmm models, default 0.001
+        -ni, --n_init, the number of k-means initializations, default 200
+        -mi, --max_iter, the maximum number of iterations, default 1000
+        ```
+        
+        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+        ```
+        wgd peak ks_datafile (option)
+        --------------------------------------------------------------------------------
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -sm, --segments, the segments datafile, default None
+        -le, --listelements, the listsegments datafile, default None 
+        -mp, --multipliconpairs, the multipliconpairs datafile, default None
+        -o, --outdir, the output directory, default wgd_peak
+        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
+        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
+        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+        -m, --method, which mixture model to use, default gmm
+        --seed, random seed given to initialization, default 2352890
+        -ei, --em_iter, the number of EM iterations to perform, default 200
+        -ni, --n_init, the number of k-means initializations, default 200
+        -n, --components, the range of the number of components to fit, default (1, 4)
+        --boots, the number of bootstrap replicates of kde, default 200
+        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+        -p, --plot, the plotting method to be used, default identical
+        -bm, --bw_method, the bandwidth method to be used, default silverman
+        --n_medoids, the number of medoids to fit, default 2
+        -km, --kdemethod, the kde method to be used, default scipy
+        --n_clusters, the number of clusters to plot Elbow loss function, default 5
+        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+        -gd, --guide, the regime residing anchors, default: segment
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+        -f, --family, the family to filter Ks upon, default None
+        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        --ci, the confidence level of log-normal distribution to date, default 95
+        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+        ```
+        
+        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+        ```
+        wgd syn families gffs (option)
+        --------------------------------------------------------------------------------
+        -ks, --ks_distribution, ks distribution datafile, default None
+        -o, --outdir, the output directory, default wgd_syn
+        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
+        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+        --iadhore_options, the parameter setting in iadhore, default 
+        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+        ```
+        wgd viz (option)
+        --------------------------------------------------------------------------------
+        -d, --datafile, the Ks datafile, default None
+        -o, --outdir, the output directory, default wgd_viz
+        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+        -gs, --gsmap, the gene name-species name map, default None
+        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+        -iter, --em_iterations, the maximum EM iterations, default 200
+        -init, --em_initializations, the maximum EM initializations, default 200
+        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+        -sm, --segments, the segments data file, default None
+        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+        -ms, --maxsize, the maximum family size to include, default 200
+        -ap, --anchorpoints, the anchor points datafile, default None
+        -mt, --multiplicon, the multiplicons datafile, default None
+        -gt, --genetable, the gene table datafile, default None
+        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+        ```
+        
+        ## Usage
+        
+        Here we provided the basic usage for each program.
+        
+        ### wgd dmd
+        
+        **The delineation of whole paranome**
+        ```
+        wgd dmd sequence
+        ``` 
+        
+        **The delineation of RBHs**
+        ```
+        wgd dmd sequence1 sequence2
+        ```
+        
+        **The delineation of local MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -f sequence1
+        ```
+        
+        **The delineation of global MRBHs**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -gm
+        ```
+        
+        **The delineation of orthogroups**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -oi (option)
+        ```
+        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+        
+        **The collinear coalescence inference of phylogeny**
+        ```
+        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+        ```
+        
+        Note that there should be no duplicated gene IDs in the sequence file.
+        
+        ### wgd focus
+        
+        **The concatenation-based/coalescence-based phylogenetic inference**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+        ```
+        
+        **The functional annotation of gene families**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+        ```
+        
+        **The phylogenetic dating of WGDs**
+        ```
+        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+        ```
+        
+        ### wgd ksd
+        
+        **The construction of whole paranome *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence
+        ```
+        
+        **The construction of orthologous *K*<sub>S</sub> age distribution**
+        ```
+        wgd ksd families sequence1 sequence2
+        ```
+        
+        **The construction of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+        ```
+        
+        ### wgd mix
+        
+        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+        ```
+        wgd mix ksdata
+        ```
+        
+        ### wgd peak
+        
+        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
+        ```
+        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+        ```
+        Note that users can add the flag --heuristic to implement the heuristic search analysis
+        
+        ### wgd syn
+        
+        **The intra-specific synteny inference**
+        ```
+        wgd syn families gff
+        ```
+        
+        **The inter-specific synteny inference**
+        ```
+        wgd syn families gff1 gff2
+        ```
+        
+        ### wgd viz
+        
+        **The visualization of *K*<sub>S</sub> age distribution**
+        ```
+        wgd viz -d ksdata
+        ```
+        
+        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
+        ```
+        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+        ```
+        
+        **The visualization of synteny**
+        ```
+        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+        ```
+        
+        ## Illustration
+        
+        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+        
+        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+        
+        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+        
+        ```
+        wgd dmd Aquilegia_coerulea
+        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+        ```
+        
+        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+        
+        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+        
+        ```
+        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+        
+        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+        
+        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+        
+        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+        
+        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+        
+        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+        
+        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+        
+        ![](data/Syndepth.svg)
+        
+        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+        
+        ```
+        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+        ```
+        
+        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+        
+        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+        
+        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+        
+        ```
+        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+        ```
+        
+        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+        
+        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+        
+        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+        
+        ```
+        wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+        ```
+        
+        In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+        
+        ```
+        wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+        ```
+        
+        The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+        
+        ```
+        (((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+        
+        As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+        
+        If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+        ```
+        
+        Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
+        ```
+        
+        ![](data/Raw_Orthologues_Compare_rate.ksd.svg)
+        
+        As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
+        
+        Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+        
+        ```
+        Aqcoe6G057800.1 Aquilegia_coerulea
+        Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+        Pcy_Procy01g08510 Protea_cynaroides
+        Aam_Acora.04G142900.1 Acorus_americanus
+        ```
+        
+        A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
+        
+        From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
+        
+        Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
+        
+        As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
+        
+        Adding both ELMM result for paranome and GMM result for anchor *K*<sub>S</sub> can be achieved just by add the two flags mentioned above, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm --plotapgmmm
+        ```
+        
+        ![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Apgmm_Corrected.ksd.svg)
+        
+        An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+        
+        ```
+        wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+        ```
+        
+        Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+        
+        ```
+        wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+        ```
+        
+        ![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+        
+        As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+        
+        If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+        
+        ```
+        wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
+        ```
+        
+        We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+        ![](data/Raw_Orthologues.ksd.svg)
+        
+        ## Citation
+         
+        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+        
+        ```
+        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+        
+        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+        ```
+        
+        For citation of the tools used in wgd, please consult the documentation at
+        https://wgd.readthedocs.io/en/latest/index.html#citation.
+        
+        
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-# `wgd v2` : a suite tool of WGD inference and timing
-
-**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-
-[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-
-[**Introduction**](#Introduction) | 
-[**Installation**](#Installation) | 
-[**Parameters**](#Parameters) | 
-[**Usage**](#Usage) | 
-[**Illustration**](#Illustration) |
-[**Citation**](#Citation)
-
-</div>
-
-`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-
-## Introduction
-
-Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-
-The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-
-## Installation
-
-The easiest way to install `wgd v2` is using PYPI
-
-```
-pip install wgd
-```
-
-To install `wgd v2` in a virtual environment, the following command lines could be used.
-
-```
-git clone <wgd repo>
-cd wgd
-virtualenv -p=python3 ENV (or python3 -m venv ENV)
-source ENV/bin/activate
-pip install -r requirements.txt
-pip install .
-```
-
-When met with permission problem in installation, please try the following command line.
-
-```
-pip install -e .
-```
-
-If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-
-```
-export PATH="$PATH:~/.local/bin/wgd"
-```
-
-Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
-
-## Parameters
-
-There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-
-The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-```
-wgd dmd sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_dmd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
--I, --inflation, the inflation factor for MCL program, default 2.0
--e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
--f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
--ap, --anchorpoints, the anchor points data file, default None
--coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
--sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
--le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
--gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
--kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
--kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
--gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
--n, --nthreads, the number of threads to use, default 4
--oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
--oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
--gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
--mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
--ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
--am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
--sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
--fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
--cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
--te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
--bs, --bins, the number of bins divided in gene length normalization, default 100
--np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
--nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
--bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
--bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
--bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-```
-
-The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-```
-wgd focus families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_focus
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--a, --aligner, which alignment program to use, default mafft
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
---concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
---coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
--sp, --speciestree, species tree darafile for dating, default None
--d, --dating, which molecular dating program to use, default none
--ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
--ns, --nsites, the nsites information for r8s dating, default None
--ot, --outgroup, the outgroup information for r8s dating, default None
--pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
--am, --aamodel, which protein model to be used in mcmctree, default poisson
--ks, flag option, whether to initiate Ks analysis
---annotation, which annotation program to use, default none
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
--ed, --eggnogdata, the eggnog annotation datafile, default None
---pfam, which option to use for pfam annotation, default none
---dmnb, the diamond database for annotation, default None
---hmm, the HMM profile for annotation, default None
---evalue, the e-value cut-off for annotation, default 1e-10
---exepath, the path to the interproscan executable, default None
--f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
- -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
--cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
---beastlgjar, the path to beastLG.jar, default None
---beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
---protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-```
-
-The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-```
-wgd ksd families sequences (option)
---------------------------------------------------------------------------------
--o, --outdir, the output directory, default wgd_ksd
--t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
--n, --nthreads, the number of threads to use, default 4
---to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
---cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
---pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
---strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
--tree, --tree_method, which gene tree inference program to invoke, default fasttree
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-```
-
-The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-```
-wgd mix ks_datafile (option)
---------------------------------------------------------------------------------
--f, --filters, the cutoff alignment length, default 300
--r, --ks_range, the Ks range to be considered, default (0.005, 3)
--b, --bins, the number of bins in Ks distribution, default 50
--o, --outdir, the output directory, default wgd_mix
---method, which mixture model to use, default gmm
--n, --components, the range of the number of components to fit, default (1, 4)
--g, --gamma, the gamma parameter for bgmm models, default 0.001
--ni, --n_init, the number of k-means initializations, default 200
--mi, --max_iter, the maximum number of iterations, default 1000
-```
-
-The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-```
-wgd peak ks_datafile (option)
---------------------------------------------------------------------------------
--ap, --anchorpoints, the anchor points datafile, default None
--sm, --segments, the segments datafile, default None
--le, --listelements, the listsegments datafile, default None 
--mp, --multipliconpairs, the multipliconpairs datafile, default None
--o, --outdir, the output directory, default wgd_peak
--af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
--r, --ksrange, range of Ks to be analyzed, default (0, 5)
--bw, --bin_width, bandwidth of Ks distribution, default 0.1
--ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
--m, --method, which mixture model to use, default gmm
---seed, random seed given to initialization, default 2352890
--ei, --em_iter, the number of EM iterations to perform, default 200
--ni, --n_init, the number of k-means initializations, default 200
--n, --components, the range of the number of components to fit, default (1, 4)
---boots, the number of bootstrap replicates of kde, default 200
---weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
--p, --plot, the plotting method to be used, default identical
--bm, --bw_method, the bandwidth method to be used, default silverman
---n_medoids, the number of medoids to fit, default 2
--km, --kdemethod, the kde method to be used, default scipy
---n_clusters, the number of clusters to plot Elbow loss function, default 5
---kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
--gd, --guide, the regime residing anchors, default: segment
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
--f, --family, the family to filter Ks upon, default None
---manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
---ci, the confidence level of log-normal distribution to date, default 95
---hdr, the highest densidy region (HDR) in a given distribution to date, default 95
---heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
--kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-```
-
-The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-```
-wgd syn families gffs (option)
---------------------------------------------------------------------------------
--ks, --ks_distribution, ks distribution datafile, default None
--o, --outdir, the output directory, default wgd_syn
--f, --feature, the feature for parsing gene IDs from GFF files, default gene
--a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--r, --ks_range, the Ks range in colored dotplot, default (0, 5)
---iadhore_options, the parameter setting in iadhore, default 
--ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-```
-wgd viz (option)
---------------------------------------------------------------------------------
--d, --datafile, the Ks datafile, default None
--o, --outdir, the output directory, default wgd_viz
--sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
--gs, --gsmap, the gene name-species name map, default None
--sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
--pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
--rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
--or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
--iter, --em_iterations, the maximum EM iterations, default 200
--init, --em_initializations, the maximum EM initializations, default 200
--prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
--sm, --segments, the segments data file, default None
--ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
--ms, --maxsize, the maximum family size to include, default 200
--ap, --anchorpoints, the anchor points datafile, default None
--mt, --multiplicon, the multiplicons datafile, default None
--gt, --genetable, the gene table datafile, default None
--rh, --rel_height, the relative height at which the peak width is measured, default 0.4
--mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
--kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-```
-
-## Usage
-
-Here we provided the basic usage for each program.
-
-### wgd dmd
-
-**The delineation of whole paranome**
-```
-wgd dmd sequence
-``` 
-
-**The delineation of RBHs**
-```
-wgd dmd sequence1 sequence2
-```
-
-**The delineation of local MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -f sequence1
-```
-
-**The delineation of global MRBHs**
-```
-wgd dmd sequence1 sequence2 sequence3 -gm
-```
-
-**The delineation of orthogroups**
-```
-wgd dmd sequence1 sequence2 sequence3 -oi (option)
-```
-Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-
-**The collinear coalescence inference of phylogeny**
-```
-wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-```
-
-### wgd focus
-
-**The concatenation-based/coalescence-based phylogenetic inference**
-```
-wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-```
-
-**The functional annotation of gene families**
-```
-wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-```
-
-**The phylogenetic dating of WGDs**
-```
-wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-```
-
-### wgd ksd
-
-**The construction of whole paranome *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence
-```
-
-**The construction of orthologous *K*<sub>S</sub> age distribution**
-```
-wgd ksd families sequence1 sequence2
-```
-
-**The construction of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-```
-
-### wgd mix
-
-**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-```
-wgd mix ksdata
-```
-
-### wgd peak
-
-**The search of crediable *K*<sub>S</sub> range used in WGD dating**
-```
-wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-```
-Note that users can add the flag --heuristic to implement the heuristic search analysis
-
-### wgd syn
-
-**The intra-specific synteny inference**
-```
-wgd syn families gff
-```
-
-**The inter-specific synteny inference**
-```
-wgd syn families gff1 gff2
-```
-
-### wgd viz
-
-**The visualization of *K*<sub>S</sub> age distribution**
-```
-wgd viz -d ksdata
-```
-
-**The visualization of *K*<sub>S</sub> age distribution with rate correction**
-```
-wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-```
-
-**The visualization of synteny**
-```
-wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-```
-
-## Illustration
-
-We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-
-The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-
-First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-
-```
-wgd dmd Aquilegia_coerulea
-wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-```
-
-The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
-
-![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
-
-We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
-
-```
-wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-```
-
-As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
-
-![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
-
-The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
-
-![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
-
-The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
-
-![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
-
-A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
-
-![](data/Syndepth.svg)
-
-We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
-
-```
-wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-```
-
-The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
-
-![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
-
-Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
-
-```
-wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
-```
-
-The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
-
-![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
-
-Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
-
-```
-wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
-```
-
-In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
-
-```
-wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-```
-
-The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
-
-```
-(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
-```
-
-![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
-
-As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
-
-If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
-```
-
-Note that we can easily show that *Aquilegia coerulea* has higher substitution rate than *Protea cynaroides* and *Vitis vinifera* by comparing their substitution distance in regard to the same divergence event with outgroup species *Acorus_americanus*, using command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_viz_Compare_rate --spair "Acorus_americanus;Protea_cynaroides" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Vitis_vinifera;Acorus_americanus" --gsmap gene_species.map --plotkde
-```
-
-![](data/Raw_Orthologues_Compare_rate.ksd.svg)
-
-As displayed above, the orthologous *K*<sub>S</sub> values bewteen *Aquilegia coerulea* and *Acorus americanus* has the highest mode, indicatingthe faster substitution rate of *Aquilegia coerulea* compared to *Protea cynaroides* and *Vitis vinifera*.
-
-Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
-
-```
-Aqcoe6G057800.1 Aquilegia_coerulea
-Vvi_VIT_201s0011g01530.1 Vitis_vinifera
-Pcy_Procy01g08510 Protea_cynaroides
-Aam_Acora.04G142900.1 Acorus_americanus
-```
-
-A more complex plot can be made by add the flag `--plotelmm` such that the ELMM mixture modeling of provided paranome *K*<sub>S</sub> can be superimposed, using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotelmm
-```
-
-![](data/Aquilegia_coerulea_GlobalmrbhKs_Elmm_Corrected.ksd.svg)
-
-From the mixed *K*<sub>S</sub> plot above, we can see that the optimized lognormal component b with mode 1.2 is younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera* (1.39 and 1.47, respectively).
-
-Besides, we can also add the GMM mixture modeling of anchor *K*<sub>S</sub> values with the flag `--plotapgmm`, using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks_elmm --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde --plotapgmmm
-```
-
-![](data/Aquilegia_coerulea_GlobalmrbhKs_Apgmm_Corrected.ksd.svg)
-
-As manifested above, the anchor *K*<sub>S</sub> component 2 with mode 1.28 is also younger than the corrected orthologous *K*<sub>S</sub> mode with *Protea cynaroides* and *Vitis vinifera*. But we need to be of course cautious that such distinction comes with the uncertainties introduced from the applied mixture modeling methodology in terms of for instance different initialization points and the issue of overfitting and the sister speciess adopted in that there might be species with more disparate substitution rates than the one we chose.
-
-An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
-
-```
-wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
-```
-
-Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
-
-```
-wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
-```
-
-![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
-
-As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
-
-If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, as we have already shown above, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
-
-```
-wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --gsmap gene_species.map
-```
-
-We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
-![](data/Raw_Orthologues.ksd.svg)
-
-## Citation
- 
-Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-
-```
-Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-
-Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-```
-
-For citation of the tools used in wgd, please consult the documentation at
-https://wgd.readthedocs.io/en/latest/index.html#citation.
-
```

### Comparing `wgd-2.0.15/wgd.egg-info/requires.txt` & `wgd-2.0.16/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

