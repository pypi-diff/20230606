# Comparing `tmp/adsorption_file_parser-0.2.5.tar.gz` & `tmp/adsorption_file_parser-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsorption_file_parser-0.2.5.tar", last modified: Wed May 24 23:08:28 2023, max compression
+gzip compressed data, was "adsorption_file_parser-0.2.6.tar", last modified: Tue Jun  6 00:09:00 2023, max compression
```

## Comparing `adsorption_file_parser-0.2.5.tar` & `adsorption_file_parser-0.2.6.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.113256 adsorption_file_parser-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.093256 adsorption_file_parser-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.093256 adsorption_file_parser-0.2.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.093256 adsorption_file_parser-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.github/workflows/CI-CD.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-24 23:08:28.113256 adsorption_file_parser-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-24 23:08:28.113256 adsorption_file_parser-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.093256 adsorption_file_parser-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.093256 adsorption_file_parser-0.2.5/src/adsorption_file_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 23:08:28.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/mic_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/qnt_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/smsdvs_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/trp_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.097256 adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/unit_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.097256 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-24 23:08:28.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-24 23:08:28.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:08:28.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 23:08:28.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 23:08:28.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:08:17.000000 adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.097256 adsorption_file_parser-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.093256 adsorption_file_parser-0.2.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.101256 adsorption_file_parser-0.2.5/tests/data/3p/
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json
--rw-r--r--   0 runner    (1001) docker     (123)  1637702 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/3p/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.105256 adsorption_file_parser-0.2.5/tests/data/bel/
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/1.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/200819-2_jis.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/200819-2_jis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/CEP 3xx-2-B 120529.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/CEP 3xx-2-B 120529.json
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-13-CH4-190K.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-13-CH4-190K.json
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K.json
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K_run2.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K_run2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-32-N2_77K(BelMax).csv
--rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-32-N2_77K(BelMax).json
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_Ar_87K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_Ar_87K.json
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_N2_77K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_N2_77K.json
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_273K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_273K.json
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67-N2_77K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67-N2_77K.json
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_DCM_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_DCM_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_EtOH_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_EtOH_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_H2O_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_H2O_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_MeOH_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_MeOH_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_acetone_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_acetone_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_hexane_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_hexane_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_isopropanol_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_isopropanol_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_toluol_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_toluol_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_wasser_298K.DAT
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_wasser_298K.json
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-8_zn_etoh_298k.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/DUT-8_zn_etoh_298k.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Sample_C.json
--rw-r--r--   0 runner    (1001) docker     (123)    37376 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Sample_C.xls
--rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Sample_D.json
--rw-r--r--   0 runner    (1001) docker     (123)    63488 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Sample_D.xls
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Sample_E.DAT
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/bel/Sample_E.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.109256 adsorption_file_parser-0.2.5/tests/data/mic/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_A.json
--rw-r--r--   0 runner    (1001) docker     (123)   224768 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_A.xls
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_B.json
--rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_B.xls
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_C.json
--rw-r--r--   0 runner    (1001) docker     (123)    59904 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_C.xls
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_D.json
--rw-r--r--   0 runner    (1001) docker     (123)    57856 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_D.xls
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_E.json
--rw-r--r--   0 runner    (1001) docker     (123)    54784 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_E.xls
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_F.json
--rw-r--r--   0 runner    (1001) docker     (123)    57856 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_F.xls
--rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_G.json
--rw-r--r--   0 runner    (1001) docker     (123)   275456 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_G.xls
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_H.json
--rw-r--r--   0 runner    (1001) docker     (123)   153600 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_H.xls
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_I.json
--rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_I.xls
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_J.json
--rw-r--r--   0 runner    (1001) docker     (123)    61952 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_J.xls
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_K.json
--rw-r--r--   0 runner    (1001) docker     (123)    58880 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_K.xls
--rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_L.json
--rw-r--r--   0 runner    (1001) docker     (123)   270848 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_L.xls
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_M.json
--rw-r--r--   0 runner    (1001) docker     (123)    62464 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_M.xls
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_N.json
--rw-r--r--   0 runner    (1001) docker     (123)   241152 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/mic/Sample_N.xls
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.113256 adsorption_file_parser-0.2.5/tests/data/qnt/
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/RE-22 (Raw Analysis Data).json
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/RE-22 (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/qnt/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:08:28.113256 adsorption_file_parser-0.2.5/tests/data/smsdvs/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/smsdvs/13X water 30c.json
--rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/smsdvs/13X water 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json
--rw-r--r--   0 runner    (1001) docker     (123)    26328 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/smsdvs/Takeda 5A water 30c.json
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/data/smsdvs/Takeda 5A water 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/test_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/test_bel.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/test_mic.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/test_qnt.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/test_smsdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-24 23:08:09.000000 adsorption_file_parser-0.2.5/tests/test_unit_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.290859 adsorption_file_parser-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.234859 adsorption_file_parser-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.234859 adsorption_file_parser-0.2.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.234859 adsorption_file_parser-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.github/workflows/CI-CD.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-06 00:09:00.290859 adsorption_file_parser-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-06 00:09:00.290859 adsorption_file_parser-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.226859 adsorption_file_parser-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.242859 adsorption_file_parser-0.2.6/src/adsorption_file_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 00:09:00.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/mic_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/qnt_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/smsdvs_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/trp_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.246859 adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/unit_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.242859 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-06 00:09:00.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-06 00:09:00.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:09:00.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 00:09:00.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 00:09:00.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:08:43.000000 adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.250859 adsorption_file_parser-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.230859 adsorption_file_parser-0.2.6/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.262859 adsorption_file_parser-0.2.6/tests/data/3p/
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1637702 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/3p/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.274859 adsorption_file_parser-0.2.6/tests/data/bel/
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/1.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/200819-2_jis.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/200819-2_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/CEP 3xx-2-B 120529.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/CEP 3xx-2-B 120529.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-13-CH4-190K.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-13-CH4-190K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K_run2.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K_run2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-32-N2_77K(BelMax).csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-32-N2_77K(BelMax).json
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_Ar_87K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_Ar_87K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_N2_77K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_N2_77K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_273K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_273K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67-N2_77K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67-N2_77K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_DCM_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_DCM_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_EtOH_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_EtOH_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_H2O_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_H2O_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_MeOH_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_MeOH_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_acetone_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_acetone_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_hexane_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_hexane_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_isopropanol_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_isopropanol_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_toluol_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_toluol_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_wasser_298K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_wasser_298K.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-8_zn_etoh_298k.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/DUT-8_zn_etoh_298k.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Sample_C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37376 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Sample_C.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Sample_D.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63488 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Sample_D.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Sample_E.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/bel/Sample_E.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.282859 adsorption_file_parser-0.2.6/tests/data/mic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_A.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224768 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_A.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_B.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_B.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59904 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_C.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_D.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57856 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_D.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_E.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54784 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_E.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57856 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_F.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_G.json
+-rw-r--r--   0 runner    (1001) docker     (123)   275456 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_G.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_H.json
+-rw-r--r--   0 runner    (1001) docker     (123)   153600 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_H.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_I.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_I.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61952 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_J.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_K.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58880 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_K.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_L.json
+-rw-r--r--   0 runner    (1001) docker     (123)   270848 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_L.xls
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_M.json
+-rw-r--r--   0 runner    (1001) docker     (123)    62464 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_M.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_N.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241152 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/mic/Sample_N.xls
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.286859 adsorption_file_parser-0.2.6/tests/data/qnt/
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19890 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16305 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/RE-22 (Raw Analysis Data).json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/RE-22 (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/qnt/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:09:00.290859 adsorption_file_parser-0.2.6/tests/data/smsdvs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/smsdvs/13X water 30c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/smsdvs/13X water 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26328 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/smsdvs/Takeda 5A water 30c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/data/smsdvs/Takeda 5A water 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/test_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/test_bel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/test_mic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/test_qnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/test_smsdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-06 00:08:24.000000 adsorption_file_parser-0.2.6/tests/test_unit_parser.py
```

### Comparing `adsorption_file_parser-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md` & `adsorption_file_parser-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/.github/workflows/CI-CD.yaml` & `adsorption_file_parser-0.2.6/.github/workflows/CI-CD.yaml`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/.gitignore` & `adsorption_file_parser-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/LICENSE` & `adsorption_file_parser-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/PKG-INFO` & `adsorption_file_parser-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsorption_file_parser
-Version: 0.2.5
+Version: 0.2.6
 Summary: Collection of parsers for (nearly) all commercial adsorption instrumentation.
 Home-page: https://github.com/AIF-development-team/adsorption-file-parser
 Author: AIF Dev Team
 Author-email: mail@pauliacomi.com
 License: MIT license
 Project-URL: Source Code, https://github.com/AIF-development-team/adsorption-file-parser
 Keywords: adsorption,characterization,porous materials,isotherms,sorption
```

### Comparing `adsorption_file_parser-0.2.5/README.rst` & `adsorption_file_parser-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/pyproject.toml` & `adsorption_file_parser-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/setup.cfg` & `adsorption_file_parser-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/__init__.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_common.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_common.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_csv.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_csv.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_dat.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_dat.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/bel_excel.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/bel_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/mic_excel.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/mic_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/qnt_txt.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/qnt_txt.py`

 * *Files 5% similar despite different names*

```diff
@@ -250,17 +250,16 @@
     if meta['loading_unit'] in ['cc']:
         meta['loading_unit'] += '(STP)'
     meta['loading_basis'] = unit_parsing.find_loading_basis(meta['loading_unit'])
 
     if meta.get('date'):
         meta['date'] = util.handle_string_date(meta['date'])
 
-    # amount adsorbed from cc to cc/material_unit
+    # pack data
     data = dict(zip(head, map(lambda *x: list(x), *data)))
-    data['loading'] = [ld / mass for ld in data['loading']]
 
     return meta, data
 
 
 def find_key_vals_from_position(line, keys, poss):
     """Find keys of successive key-val pairs, knowing the key position"""
     vals = []
```

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/smsdvs_excel.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/smsdvs_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/trp_excel.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/trp_excel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/common_utils.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/unit_parsing.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/unit_parsing.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser/utils/units.py` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser/utils/units.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/PKG-INFO` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsorption-file-parser
-Version: 0.2.5
+Version: 0.2.6
 Summary: Collection of parsers for (nearly) all commercial adsorption instrumentation.
 Home-page: https://github.com/AIF-development-team/adsorption-file-parser
 Author: AIF Dev Team
 Author-email: mail@pauliacomi.com
 License: MIT license
 Project-URL: Source Code, https://github.com/AIF-development-team/adsorption-file-parser
 Keywords: adsorption,characterization,porous materials,isotherms,sorption
```

### Comparing `adsorption_file_parser-0.2.5/src/adsorption_file_parser.egg-info/SOURCES.txt` & `adsorption_file_parser-0.2.6/src/adsorption_file_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/conftest.py` & `adsorption_file_parser-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json` & `adsorption_file_parser-0.2.6/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx` & `adsorption_file_parser-0.2.6/tests/data/3p/AC_ref_filter_Ar_87K_run 3_rep.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/1.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/1.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/1.json` & `adsorption_file_parser-0.2.6/tests/data/bel/1.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/200819-2_jis.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/200819-2_jis.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/200819-2_jis.json` & `adsorption_file_parser-0.2.6/tests/data/bel/200819-2_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv` & `adsorption_file_parser-0.2.6/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json` & `adsorption_file_parser-0.2.6/tests/data/bel/ASch082B_Zndmbdcdabco_C2H4_Exp191004a_weight correction_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv` & `adsorption_file_parser-0.2.6/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json` & `adsorption_file_parser-0.2.6/tests/data/bel/ASch082C_Zntmbdcdabco_C2H6_Exp190819a_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv` & `adsorption_file_parser-0.2.6/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json` & `adsorption_file_parser-0.2.6/tests/data/bel/Asch065B_C2H6_298K_Exp190327a_jis.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/CEP 3xx-2-B 120529.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/CEP 3xx-2-B 120529.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/CEP 3xx-2-B 120529.json` & `adsorption_file_parser-0.2.6/tests/data/bel/CEP 3xx-2-B 120529.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-13-CH4-190K.csv` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-13-CH4-190K.csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-13-CH4-190K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-13-CH4-190K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K_run2.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K_run2.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-13_CH4_111K_run2.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-13_CH4_111K_run2.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-32-N2_77K(BelMax).csv` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-32-N2_77K(BelMax).csv`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-32-N2_77K(BelMax).json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-32-N2_77K(BelMax).json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_Ar_87K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_Ar_87K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_Ar_87K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_Ar_87K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_N2_77K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_N2_77K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_N2_77K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_N2_77K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_273K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_273K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_273K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_273K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-49_nbutane_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-49_nbutane_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67-N2_77K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67-N2_77K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67-N2_77K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67-N2_77K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_DCM_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_DCM_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_DCM_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_DCM_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_EtOH_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_EtOH_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_EtOH_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_EtOH_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_H2O_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_H2O_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_H2O_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_H2O_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_MeOH_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_MeOH_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_MeOH_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_MeOH_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_acetone_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_acetone_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_acetone_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_acetone_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_hexane_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_hexane_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_hexane_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_hexane_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_isopropanol_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_isopropanol_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_isopropanol_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_isopropanol_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_toluol_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_toluol_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_toluol_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_toluol_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_wasser_298K.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_wasser_298K.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-67_wasser_298K.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-67_wasser_298K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-8_zn_etoh_298k.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-8_zn_etoh_298k.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/DUT-8_zn_etoh_298k.json` & `adsorption_file_parser-0.2.6/tests/data/bel/DUT-8_zn_etoh_298k.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Sample_C.json` & `adsorption_file_parser-0.2.6/tests/data/bel/Sample_C.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Sample_C.xls` & `adsorption_file_parser-0.2.6/tests/data/bel/Sample_C.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Sample_D.json` & `adsorption_file_parser-0.2.6/tests/data/bel/Sample_D.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Sample_D.xls` & `adsorption_file_parser-0.2.6/tests/data/bel/Sample_D.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Sample_E.DAT` & `adsorption_file_parser-0.2.6/tests/data/bel/Sample_E.DAT`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/bel/Sample_E.json` & `adsorption_file_parser-0.2.6/tests/data/bel/Sample_E.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_A.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_A.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_A.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_A.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_B.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_B.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_B.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_B.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_C.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_C.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_C.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_C.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_D.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_D.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_D.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_D.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_E.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_E.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_E.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_E.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_F.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_F.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_F.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_F.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_G.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_G.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_G.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_G.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_H.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_H.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_H.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_H.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_I.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_I.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_I.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_I.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_J.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_J.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_J.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_J.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_K.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_K.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_K.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_K.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_L.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_L.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_L.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_L.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_M.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_M.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_M.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_M.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_N.json` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_N.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/mic/Sample_N.xls` & `adsorption_file_parser-0.2.6/tests/data/mic/Sample_N.xls`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.6/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'data'": "{'loading': [1.1352, 1.3858, 1.7488, 1.9675, 2.4531, 3.2815, 4.0705, 4.2265, 4.445, "*

 * *           '4.866, 4.962, 5.0752, 5.2688, 5.429, 5.5055, 5.5785, 5.6367, 5.6979, 5.7349, 5.82, '*

 * *           '5.9014, 5.9391, 5.9924, 6.0964, 6.194, 6.3352, 6.4539, 8.2482, 10.1578, 11.1754, '*

 * *           '11.6738, 11.9883, 12.2301, 12.4159, 12.6085, 12.73, 12.8517, 12.95, 13.0532, 13.2332, '*

 * *           '13.2471, 13.3198, 13.3526, 13.3286, 13.2816, 13.2243, 13.176, 13.1279, 13.0668, '*

 * *           '13.0103, 12.9483 […]*

```diff
@@ -165,96 +165,96 @@
             600.0,
             600.0,
             600.0,
             600.0,
             600.0
         ],
         "loading": [
-            112.3960396039604,
-            137.2079207920792,
-            173.14851485148515,
-            194.8019801980198,
-            242.8811881188119,
-            324.9009900990099,
-            403.01980198019805,
-            418.46534653465346,
-            440.09900990099015,
-            481.78217821782175,
-            491.28712871287127,
-            502.4950495049505,
-            521.6633663366337,
-            537.5247524752476,
-            545.09900990099,
-            552.3267326732673,
-            558.0891089108911,
-            564.1485148514852,
-            567.8118811881188,
-            576.2376237623763,
-            584.2970297029703,
-            588.0297029702971,
-            593.3069306930694,
-            603.6039603960396,
-            613.2673267326733,
-            627.2475247524753,
-            639.0,
-            816.6534653465347,
-            1005.7227722772277,
-            1106.4752475247526,
-            1155.821782178218,
-            1186.9603960396041,
-            1210.90099009901,
-            1229.2970297029703,
-            1248.3663366336634,
-            1260.3960396039604,
-            1272.4455445544554,
-            1282.1782178217823,
-            1292.3960396039604,
-            1310.2178217821784,
-            1311.5940594059407,
-            1318.792079207921,
-            1322.039603960396,
-            1319.6633663366338,
-            1315.009900990099,
-            1309.3366336633662,
-            1304.5544554455446,
-            1299.7920792079208,
-            1293.7425742574258,
-            1288.1485148514853,
-            1282.0099009900991,
-            1277.851485148515,
-            1273.5445544554457,
-            1269.990099009901,
-            1265.6039603960396,
-            1261.5742574257426,
-            1258.1386138613861,
-            1253.4653465346535,
-            1248.90099009901,
-            1242.4851485148515,
-            1237.6237623762377,
-            1230.5742574257426,
-            1225.069306930693,
-            1218.0594059405942,
-            1209.4752475247526,
-            1197.6138613861388,
-            1194.09900990099,
-            1177.2277227722773,
-            1157.128712871287,
-            1136.3267326732673,
-            1106.1287128712872,
-            1049.0297029702972,
-            528.950495049505,
-            468.3267326732674,
-            402.58415841584156,
-            387.7722772277228,
-            369.26732673267327,
-            340.009900990099,
-            328.970297029703,
-            328.4257425742574,
-            327.73267326732673,
-            327.21782178217825
+            1.1352,
+            1.3858,
+            1.7488,
+            1.9675,
+            2.4531,
+            3.2815,
+            4.0705,
+            4.2265,
+            4.445,
+            4.866,
+            4.962,
+            5.0752,
+            5.2688,
+            5.429,
+            5.5055,
+            5.5785,
+            5.6367,
+            5.6979,
+            5.7349,
+            5.82,
+            5.9014,
+            5.9391,
+            5.9924,
+            6.0964,
+            6.194,
+            6.3352,
+            6.4539,
+            8.2482,
+            10.1578,
+            11.1754,
+            11.6738,
+            11.9883,
+            12.2301,
+            12.4159,
+            12.6085,
+            12.73,
+            12.8517,
+            12.95,
+            13.0532,
+            13.2332,
+            13.2471,
+            13.3198,
+            13.3526,
+            13.3286,
+            13.2816,
+            13.2243,
+            13.176,
+            13.1279,
+            13.0668,
+            13.0103,
+            12.9483,
+            12.9063,
+            12.8628,
+            12.8269,
+            12.7826,
+            12.7419,
+            12.7072,
+            12.66,
+            12.6139,
+            12.5491,
+            12.5,
+            12.4288,
+            12.3732,
+            12.3024,
+            12.2157,
+            12.0959,
+            12.0604,
+            11.89,
+            11.687,
+            11.4769,
+            11.1719,
+            10.5952,
+            5.3424,
+            4.7301,
+            4.0661,
+            3.9165,
+            3.7296,
+            3.4341,
+            3.3226,
+            3.3171,
+            3.3101,
+            3.3049
         ],
         "pressure": [
             1.06,
             1.62,
             2.49,
             2.98,
             4.06,
```

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.6/tests/data/qnt/BF001 DUT-13 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.6/tests/data/qnt/CU(BIPY)(BTB)_N2_77 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.6/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.6/tests/data/qnt/DUT-6_LP_N2 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).json` & `adsorption_file_parser-0.2.6/tests/data/qnt/DUT-60_N2 (Raw Analysis Data).json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8049037629757786%*

 * *Differences: {"'data'": "{'pressure': [0.00909472, 0.00966483, 0.0102547, 0.0158041, 0.0165347, 0.0230801, "*

 * *           '0.0303859, 0.0381392, 0.0469679, 0.0562782, 0.0601997, 0.0706719, 0.0816124, '*

 * *           '0.0941736, 0.119137, 0.158206, 0.178274, 0.233424, 0.308864, 0.392869, 0.487226, '*

 * *           '0.552043, 0.628187, 0.711888, 0.788351, 0.923254, 1.15396, 1.5697, 1.76316, 2.31193, '*

 * *           '3.12107, 3.84232, 4.58744, 5.36564, 6.12081, 6.89475, 11.4328, 14.4302, 19.1699, '*

 * *           '29.3839, 35.3095, 38.084 […]*

```diff
@@ -1,680 +1,38 @@
 {
     "data": {
         "equilibration_time": [
             3.0,
             3.0,
             3.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            5.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0,
-            2.0
-        ],
-        "loading": [
-            247.3525046382189,
-            277.4211502782931,
-            309.97588126159553,
-            397.64007421150274,
-            443.4619666048237,
-            476.03525046382185,
-            501.76623376623377,
-            519.7328385899814,
-            543.9684601113172,
-            558.9944341372913,
-            581.2949907235621,
-            595.1614100185528,
-            598.3729128014842,
-            642.560296846011,
-            671.886827458256,
-            711.9480519480519,
-            734.8014842300556,
-            759.4749536178107,
-            772.4508348794063,
-            785.8144712430427,
-            799.3339517625232,
-            812.8701298701297,
-            826.200371057514,
-            839.1948051948051,
-            851.7328385899814,
-            863.7402597402596,
-            875.2801484230055,
-            887.4192949907234,
-            899.4508348794063,
-            911.2319109461966,
-            923.0612244897959,
-            935.2875695732838,
-            948.2745825602968,
-            972.1576994434135,
-            995.8552875695732,
-            1019.2708719851576,
-            1043.8200371057512,
-            1055.599257884972,
-            1066.964749536178,
-            1074.964749536178,
-            1080.294990723562,
-            1083.8163265306123,
-            1086.2875695732837,
-            1088.2430426716141,
-            1089.8719851576993,
-            1091.385899814471,
-            1092.7884972170687,
-            1094.1224489795918,
-            1095.3803339517624,
-            1096.5769944341373,
-            1097.725417439703,
-            1098.803339517625,
-            1099.8534322820037,
-            1100.8571428571427,
-            1101.860853432282,
-            1102.803339517625,
-            1103.708719851577,
-            1106.2597402597403,
-            1107.82560296846,
-            1108.9332096474955,
-            1109.857142857143,
-            1110.7105751391466,
-            1111.3191094619665,
-            1112.0519480519479,
-            1112.808905380334,
-            1113.5565862708718,
-            1114.2708719851576,
-            1114.9758812615955,
-            1116.007421150278,
-            1119.6363636363635,
-            1123.4397031539888,
-            1126.964749536178,
-            1130.1855287569572,
-            1133.1001855287568,
-            1135.8293135435993,
-            1138.3153988868276,
-            1140.6771799628941,
-            1142.8293135435993,
-            1144.8923933209646,
-            1146.857142857143,
-            1148.708719851577,
-            1150.4415584415583,
-            1152.1243042671613,
-            1153.7532467532467,
-            1155.278293135436,
-            1156.7458256029684,
-            1158.1595547309832,
-            1159.5602968460112,
-            1160.8775510204082,
-            1162.1447124304266,
-            1163.3970315398885,
-            1164.6141001855287,
-            1165.7959183673468,
-            1166.9350649350647,
-            1168.0946196660482,
-            1169.1892393320963,
-            1170.1076066790351,
-            1171.1465677179963,
-            1172.4267161410019,
-            1179.0,
-            1171.9814471243042,
-            1170.5936920222634,
-            1168.3803339517626,
-            1166.0667903525045,
-            1163.6716141001855,
-            1161.1743970315397,
-            1158.495361781076,
-            1155.5361781076067,
-            1152.8645640074212,
-            1149.3858998144713,
-            1145.5064935064934,
-            1141.3358070500926,
-            1136.6549165120593,
-            1131.269016697588,
-            1124.942486085343,
-            1117.378478664193,
-            1107.6437847866418,
-            1104.3617810760668,
-            1102.6716141001855,
-            1100.6641929499071,
-            1098.499072356215,
-            1096.103896103896,
-            1093.5102040816325,
-            1090.6808905380333,
-            1087.5602968460112,
-            1084.025974025974,
-            1079.8719851576993,
-            1074.8627087198515,
-            1068.161410018553,
-            1059.4304267161408,
-            1047.821892393321,
-            1010.0296846011132
-        ],
-        "measurement_time": [
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0
-        ],
-        "pressure": [
-            0.375289,
-            0.56417,
-            0.753489,
-            1.50871,
-            2.28019,
-            3.02256,
-            3.77764,
-            4.53021,
-            5.31581,
-            6.08451,
-            6.81558,
-            7.58728,
-            7.74643,
-            10.3938,
-            12.3077,
-            16.2692,
-            19.176,
-            22.8474,
-            25.0102,
-            27.4237,
-            30.0496,
-            32.8293,
-            35.7925,
-            38.874,
-            42.0615,
-            45.3251,
-            48.5875,
-            50.5774,
-            53.7093,
-            56.7908,
-            59.5938,
-            62.0818,
-            64.2668,
-            67.4915,
-            70.1362,
-            72.7492,
-            76.3336,
-            78.9321,
-            83.0338,
-            88.1319,
-            93.4789,
-            98.0762,
-            101.866,
-            105.206,
-            108.311,
-            111.274,
-            114.224,
-            117.099,
-            119.998,
-            122.939,
-            125.775,
-            128.648,
-            131.505,
-            134.369,
-            137.249,
-            140.106,
-            142.969,
-            143.922,
-            148.001,
-            151.255,
-            154.26,
-            157.187,
-            159.297,
-            161.973,
-            164.814,
-            167.644,
-            170.473,
-            173.327,
-            177.702,
-            194.013,
-            212.559,
-            231.683,
-            250.82,
-            269.956,
-            288.965,
-            307.998,
-            327.01,
-            345.965,
-            364.936,
-            383.85,
-            402.822,
-            421.643,
-            440.623,
-            459.482,
-            478.41,
-            497.218,
-            516.06,
-            535.051,
-            553.922,
-            572.74,
-            591.677,
-            610.534,
-            629.382,
-            648.113,
-            667.087,
-            685.899,
-            704.922,
-            723.763,
-            742.346,
-            753.108,
-            735.781,
-            713.836,
-            672.125,
-            633.947,
-            596.12,
-            558.431,
-            520.823,
-            481.743,
-            444.966,
-            407.777,
-            370.291,
-            332.852,
-            295.396,
-            258.004,
-            220.821,
-            183.943,
-            147.638,
-            140.314,
-            135.815,
-            130.419,
-            124.932,
-            119.475,
-            113.995,
-            108.55,
-            103.198,
-            97.9125,
-            92.8891,
-            88.1651,
-            83.8635,
-            80.1714,
-            77.1746,
-            71.5845
-        ],
-        "pressure_saturation": [
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27,
-            754.27
-        ],
-        "pressure_tolerance": [
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
+            3.0,
             3.0,
             3.0,
             3.0,
             3.0,
             3.0,
             3.0,
             3.0,
@@ -799,42 +157,853 @@
             3.0,
             3.0,
             3.0,
             3.0,
             3.0,
             3.0,
             3.0
+        ],
+        "loading": [
+            0.0521998,
+            0.0558248,
+            0.0594411,
+            0.085551,
+            0.0889997,
+            0.115298,
+            0.140978,
+            0.165119,
+            0.189483,
+            0.212035,
+            0.221,
+            0.242142,
+            0.261749,
+            0.28248,
+            0.315602,
+            0.356349,
+            0.373864,
+            0.411773,
+            0.452678,
+            0.488126,
+            0.52105,
+            0.540424,
+            0.561237,
+            0.582142,
+            0.600179,
+            0.629072,
+            0.673934,
+            0.746692,
+            0.778842,
+            0.865935,
+            0.987663,
+            1.0938,
+            1.20272,
+            1.31504,
+            1.42292,
+            1.53356,
+            2.1287,
+            2.49365,
+            2.99681,
+            3.83306,
+            4.22624,
+            4.40182,
+            5.08751,
+            5.36651,
+            6.05092,
+            6.32276,
+            7.01008,
+            7.3024,
+            8.08212,
+            8.6274,
+            9.62839,
+            10.2497,
+            11.8254,
+            12.9635,
+            13.7238,
+            13.9996,
+            15.0711,
+            15.5678,
+            16.5165,
+            17.1084,
+            18.6518,
+            19.9189,
+            20.9297,
+            21.5714,
+            21.7112,
+            22.3397,
+            22.4098,
+            22.633,
+            22.8717,
+            23.056,
+            23.2268,
+            23.3815,
+            23.5285,
+            23.6658,
+            23.7968,
+            23.9259,
+            24.046,
+            24.1636,
+            24.2804,
+            24.3898,
+            24.575,
+            24.6879,
+            24.7943,
+            24.8971,
+            24.9982,
+            25.0994,
+            25.2002,
+            25.2941,
+            25.3914,
+            25.4898,
+            25.59,
+            25.6923,
+            25.8125,
+            26.0794,
+            26.6435,
+            26.5956,
+            26.1597,
+            25.9568,
+            25.8153,
+            25.6985,
+            25.5875,
+            25.4806,
+            25.3757,
+            25.2728,
+            25.2028,
+            25.1571,
+            25.0528,
+            24.9449,
+            24.8343,
+            24.72,
+            24.601,
+            24.4823,
+            24.3627,
+            24.236,
+            24.1058,
+            23.974,
+            23.8257,
+            23.6797,
+            23.5282,
+            23.4145,
+            23.247,
+            23.0647,
+            22.8615,
+            22.6328,
+            22.284,
+            22.2059,
+            21.4396,
+            20.5201,
+            19.7619,
+            19.117,
+            18.8586,
+            17.5488,
+            16.689,
+            16.2637,
+            16.0533,
+            15.2807,
+            14.9062,
+            14.7156,
+            13.7917,
+            13.1377,
+            12.6414,
+            11.973,
+            11.7105,
+            10.4457,
+            9.65217,
+            9.22572,
+            9.01896,
+            8.19719,
+            7.79292,
+            7.62839,
+            6.96066,
+            6.68217,
+            6.56574,
+            5.92909,
+            5.66604,
+            4.91694,
+            4.6271,
+            4.49829,
+            3.704,
+            3.18704
+        ],
+        "measurement_time": [
+            24.4,
+            29.7,
+            34.8,
+            46.6,
+            51.9,
+            62.6,
+            73.6,
+            84.4,
+            95.6,
+            106.5,
+            115.0,
+            125.2,
+            136.9,
+            148.1,
+            160.0,
+            175.3,
+            186.8,
+            200.2,
+            212.9,
+            225.8,
+            237.4,
+            248.2,
+            258.4,
+            269.4,
+            282.2,
+            291.4,
+            300.8,
+            311.1,
+            319.9,
+            329.8,
+            340.4,
+            350.4,
+            360.4,
+            371.1,
+            381.8,
+            393.1,
+            397.9,
+            402.7,
+            411.3,
+            417.1,
+            422.1,
+            426.4,
+            432.4,
+            437.6,
+            443.9,
+            448.8,
+            455.5,
+            461.1,
+            468.6,
+            477.8,
+            486.8,
+            496.2,
+            508.2,
+            521.2,
+            533.4,
+            540.2,
+            551.7,
+            562.9,
+            573.2,
+            584.2,
+            596.9,
+            611.5,
+            628.2,
+            645.1,
+            649.9,
+            661.0,
+            664.6,
+            669.2,
+            674.0,
+            678.2,
+            682.3,
+            686.2,
+            690.1,
+            693.8,
+            697.7,
+            701.4,
+            705.1,
+            708.8,
+            712.5,
+            716.2,
+            722.2,
+            725.9,
+            729.6,
+            733.3,
+            737.0,
+            740.7,
+            744.5,
+            748.2,
+            752.0,
+            755.8,
+            759.5,
+            763.2,
+            767.1,
+            774.3,
+            782.6,
+            786.4,
+            793.6,
+            797.9,
+            801.8,
+            805.6,
+            809.4,
+            813.2,
+            816.9,
+            820.7,
+            824.4,
+            828.4,
+            832.2,
+            835.9,
+            839.7,
+            843.5,
+            847.2,
+            851.0,
+            854.8,
+            858.6,
+            862.4,
+            866.2,
+            870.2,
+            874.1,
+            878.2,
+            882.0,
+            886.1,
+            890.3,
+            894.7,
+            899.4,
+            905.2,
+            908.8,
+            919.3,
+            931.4,
+            943.5,
+            957.7,
+            964.3,
+            978.7,
+            991.0,
+            998.0,
+            1003.9,
+            1013.1,
+            1020.2,
+            1025.5,
+            1035.8,
+            1045.1,
+            1053.4,
+            1065.0,
+            1071.2,
+            1083.1,
+            1092.7,
+            1099.6,
+            1104.6,
+            1113.4,
+            1119.8,
+            1124.1,
+            1131.0,
+            1136.0,
+            1140.0,
+            1146.1,
+            1151.0,
+            1157.3,
+            1162.5,
+            1166.7,
+            1173.5,
+            1181.8
+        ],
+        "pressure": [
+            0.00909472,
+            0.00966483,
+            0.0102547,
+            0.0158041,
+            0.0165347,
+            0.0230801,
+            0.0303859,
+            0.0381392,
+            0.0469679,
+            0.0562782,
+            0.0601997,
+            0.0706719,
+            0.0816124,
+            0.0941736,
+            0.119137,
+            0.158206,
+            0.178274,
+            0.233424,
+            0.308864,
+            0.392869,
+            0.487226,
+            0.552043,
+            0.628187,
+            0.711888,
+            0.788351,
+            0.923254,
+            1.15396,
+            1.5697,
+            1.76316,
+            2.31193,
+            3.12107,
+            3.84232,
+            4.58744,
+            5.36564,
+            6.12081,
+            6.89475,
+            11.4328,
+            14.4302,
+            19.1699,
+            29.3839,
+            35.3095,
+            38.084,
+            50.4908,
+            55.9348,
+            69.4616,
+            74.8371,
+            88.5471,
+            93.7645,
+            106.466,
+            113.878,
+            127.143,
+            131.987,
+            139.687,
+            144.621,
+            149.233,
+            151.002,
+            164.339,
+            171.438,
+            184.965,
+            189.363,
+            196.53,
+            200.026,
+            203.116,
+            207.636,
+            209.634,
+            226.815,
+            229.527,
+            246.349,
+            265.098,
+            284.803,
+            303.966,
+            323.193,
+            342.318,
+            361.415,
+            380.507,
+            399.545,
+            418.601,
+            437.701,
+            456.544,
+            475.644,
+            493.947,
+            513.612,
+            532.772,
+            551.779,
+            570.678,
+            589.762,
+            608.742,
+            627.533,
+            646.812,
+            665.684,
+            684.474,
+            703.693,
+            722.446,
+            739.38,
+            755.237,
+            754.155,
+            740.59,
+            723.367,
+            703.67,
+            684.342,
+            665.265,
+            645.903,
+            626.983,
+            607.904,
+            588.472,
+            569.404,
+            550.908,
+            532.038,
+            513.013,
+            493.791,
+            475.029,
+            456.058,
+            437.001,
+            417.985,
+            398.989,
+            380.057,
+            361.196,
+            342.306,
+            323.197,
+            303.611,
+            285.498,
+            266.665,
+            247.836,
+            229.109,
+            211.665,
+            207.936,
+            197.799,
+            194.996,
+            193.045,
+            191.556,
+            191.144,
+            185.66,
+            179.931,
+            174.265,
+            171.477,
+            159.683,
+            154.557,
+            152.19,
+            142.761,
+            139.257,
+            137.208,
+            134.731,
+            134.01,
+            128.046,
+            121.967,
+            117.157,
+            114.395,
+            103.443,
+            98.0489,
+            94.9621,
+            82.5676,
+            77.4564,
+            75.3681,
+            63.1908,
+            58.2926,
+            44.5776,
+            39.6371,
+            37.5644,
+            26.0152,
+            20.1277
+        ],
+        "pressure_saturation": [
+            767.12,
+            767.14,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.24,
+            767.03,
+            767.24,
+            767.01,
+            766.88,
+            765.46,
+            765.0,
+            764.81,
+            764.5,
+            764.32,
+            764.35,
+            764.34,
+            764.36,
+            764.12,
+            763.9,
+            763.91,
+            763.85,
+            763.79,
+            763.8,
+            763.67,
+            763.71,
+            763.61,
+            763.53,
+            763.49,
+            763.52,
+            763.37,
+            763.59,
+            763.35,
+            763.21,
+            763.31,
+            763.23,
+            763.2,
+            763.19,
+            763.07,
+            762.93,
+            762.74,
+            762.76,
+            762.95,
+            762.43,
+            762.41,
+            762.34,
+            762.24,
+            762.15,
+            761.87,
+            761.78,
+            761.74,
+            761.53,
+            761.46,
+            761.31,
+            761.35,
+            761.2,
+            761.26,
+            761.22,
+            761.14,
+            761.2,
+            761.06,
+            761.1,
+            761.22,
+            761.07,
+            761.09,
+            761.03,
+            760.88,
+            761.06,
+            760.82,
+            760.69,
+            760.98,
+            760.73,
+            760.72,
+            760.8,
+            760.57,
+            760.63,
+            760.66,
+            760.24,
+            760.68,
+            760.57,
+            760.3,
+            760.57,
+            760.6,
+            760.19,
+            760.47,
+            760.51,
+            760.4,
+            760.48,
+            760.43,
+            760.35,
+            760.47,
+            760.16,
+            760.2,
+            760.27,
+            760.09,
+            760.64,
+            760.22,
+            760.37,
+            760.34,
+            760.04,
+            760.36,
+            760.35,
+            760.25,
+            760.06,
+            759.97,
+            760.07,
+            760.15,
+            760.32,
+            760.0,
+            759.67,
+            760.36,
+            760.46,
+            760.22,
+            760.07,
+            760.19,
+            760.08,
+            760.16,
+            759.81,
+            760.05,
+            759.92,
+            760.05,
+            759.85,
+            760.13,
+            759.44,
+            759.71,
+            759.71,
+            759.54,
+            759.63,
+            759.44,
+            759.72,
+            759.66,
+            759.53,
+            759.13,
+            759.24,
+            759.29,
+            758.98,
+            759.36,
+            759.39,
+            759.2,
+            759.41,
+            759.62,
+            759.37,
+            759.42,
+            759.29,
+            759.32,
+            759.23,
+            759.0,
+            759.24,
+            759.25,
+            759.1,
+            759.47
+        ],
+        "pressure_tolerance": [
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0,
+            2.0
         ]
     },
     "meta": {
         "adsorbate": "Nitrogen",
-        "adsorbate_molecular_weight": "28.0134 g",
         "adsorbate_non_ideality": "6.58e-05 1/Torr",
-        "apparatus": "Autosorb Station 1",
-        "comment": "",
-        "date": "2012-11-30T18:59:00",
+        "apparatus": "Autosorb iQ Station 1",
+        "cell": "9mm w/o rod",
+        "comment": "ih_DUT-60_183b",
+        "date": "2016-10-07T00:00:00",
         "equilibration_time_unit": null,
-        "filename": "US_540_DUT75_N2.raw",
+        "extended_info": "Available",
+        "filename": "ih_DUT-60_183b.qps",
         "loading_basis": "molar",
         "loading_unit": "cc(STP)",
-        "material": "US_540_DUT75_N2",
+        "material": "ih_DUT-60_183b",
         "material_basis": "mass",
-        "material_description": "US_540_DUT75_N2",
-        "material_mass": 0.0539,
+        "material_description": "",
+        "material_mass": 0.0081,
         "material_unit": "g",
-        "measurement_duration": "n/a",
+        "measurement_duration": "19:41 hr:min",
         "measurement_time_unit": "min",
-        "operator": "Uli",
+        "operator": "QC",
         "original_loading_string": "cc",
         "original_pressure_string": "Torr",
-        "outgas_temperature": "150.0 \u00b0C",
-        "outgas_time": "17.5 hrs",
+        "outgas_temperature": "30 \u00b0C",
+        "outgas_time": "12.0 hrs       Final",
         "pressure_mode": "absolute",
         "pressure_saturation_unit": "Torr",
         "pressure_tolerance_unit": null,
         "pressure_unit": "Torr",
         "report_date": "2020/05/06",
         "report_operator": "ir",
-        "temperature": 77.3,
+        "temperature": 77.35,
         "temperature_unit": "K"
     }
 }
```

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.6/tests/data/qnt/DUT-75_N2 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/qnt/RE-22 (Raw Analysis Data).txt` & `adsorption_file_parser-0.2.6/tests/data/qnt/RE-22 (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/smsdvs/13X water 30c.json` & `adsorption_file_parser-0.2.6/tests/data/smsdvs/13X water 30c.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/smsdvs/13X water 30c.xlsx` & `adsorption_file_parser-0.2.6/tests/data/smsdvs/13X water 30c.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json` & `adsorption_file_parser-0.2.6/tests/data/smsdvs/MIL-101Cr H2O@air 30c.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx` & `adsorption_file_parser-0.2.6/tests/data/smsdvs/MIL-101Cr H2O@air 30c.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/smsdvs/Takeda 5A water 30c.json` & `adsorption_file_parser-0.2.6/tests/data/smsdvs/Takeda 5A water 30c.json`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/data/smsdvs/Takeda 5A water 30c.xlsx` & `adsorption_file_parser-0.2.6/tests/data/smsdvs/Takeda 5A water 30c.xlsx`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/test_3p.py` & `adsorption_file_parser-0.2.6/tests/test_3p.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/test_bel.py` & `adsorption_file_parser-0.2.6/tests/test_bel.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/test_mic.py` & `adsorption_file_parser-0.2.6/tests/test_mic.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/test_qnt.py` & `adsorption_file_parser-0.2.6/tests/test_qnt.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/test_smsdvs.py` & `adsorption_file_parser-0.2.6/tests/test_smsdvs.py`

 * *Files identical despite different names*

### Comparing `adsorption_file_parser-0.2.5/tests/test_unit_parser.py` & `adsorption_file_parser-0.2.6/tests/test_unit_parser.py`

 * *Files identical despite different names*

