# Comparing `tmp/clinica-0.7.4.tar.gz` & `tmp/clinica-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinica-0.7.4.tar", max compression
+gzip compressed data, was "clinica-0.7.5.tar", max compression
```

## Comparing `clinica-0.7.4.tar` & `clinica-0.7.5.tar`

### file list

```diff
@@ -1,383 +1,396 @@
--rw-r--r--   0        0        0    11842 2023-03-27 15:10:53.478462 clinica-0.7.4/LICENSE.txt
--rw-r--r--   0        0        0     8791 2023-03-27 15:10:53.478462 clinica-0.7.4/README.md
--rw-r--r--   0        0        0      175 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/__init__.py
--rw-r--r--   0        0        0     3020 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/cmdline.py
--rw-r--r--   0        0        0       67 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/compat.py
--rw-r--r--   0        0        0       33 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/engine/__init__.py
--rw-r--r--   0        0        0     5730 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/engine/cmdparser.py
--rw-r--r--   0        0        0     1908 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/engine/template.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/__init__.py
--rw-r--r--   0        0        0      225 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/abstract_converter.py
--rw-r--r--   0        0        0     1405 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/bids_dataset_description.py
--rw-r--r--   0        0        0      636 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/bids_readme.py
--rw-r--r--   0        0        0    33136 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/bids_utils.py
--rw-r--r--   0        0        0    10361 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converter_utils.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/__init__.py
--rw-r--r--   0        0        0    20026 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_json.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/__init__.py
--rw-r--r--   0        0        0     4873 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py
--rw-r--r--   0        0        0     8842 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py
--rw-r--r--   0        0        0     4761 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py
--rw-r--r--   0        0        0     7121 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py
--rw-r--r--   0        0        0     7214 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py
--rw-r--r--   0        0        0     4067 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py
--rw-r--r--   0        0        0    20724 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py
--rw-r--r--   0        0        0     4555 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py
--rw-r--r--   0        0        0    10270 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_to_bids.py
--rw-r--r--   0        0        0     2407 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py
--rw-r--r--   0        0        0    44462 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_utils.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/__init__.py
--rw-r--r--   0        0        0     2703 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py
--rw-r--r--   0        0        0     1310 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py
--rw-r--r--   0        0        0    36162 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/aibl_utils.py
--rw-r--r--   0        0        0      833 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/cli.py
--rw-r--r--   0        0        0      875 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/cli_param.py
--rw-r--r--   0        0        0     2740 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py
--rw-r--r--   0        0        0     1421 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py
--rw-r--r--   0        0        0    19517 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/habs_to_bids/__init__.py
--rw-r--r--   0        0        0     9025 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/habs_to_bids/habs_to_bids.py
--rw-r--r--   0        0        0     1040 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/__init__.py
--rw-r--r--   0        0        0     1840 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py
--rw-r--r--   0        0        0      969 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py
--rw-r--r--   0        0        0    11913 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/nifd_utils.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/__init__.py
--rw-r--r--   0        0        0     2509 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py
--rw-r--r--   0        0        0      969 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py
--rw-r--r--   0        0        0    10566 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis_to_bids/__init__.py
--rw-r--r--   0        0        0     7287 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py
--rw-r--r--   0        0        0      848 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/__init__.py
--rw-r--r--   0        0        0     2094 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py
--rw-r--r--   0        0        0     1041 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py
--rw-r--r--   0        0        0    16773 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/ukb_utils.py
--rw-r--r--   0        0        0     2383 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/data/clinical_specifications_adni_participant.tsv
--rw-r--r--   0        0        0      244 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/data/clinical_specifications_adni_scans.tsv
--rw-r--r--   0        0        0    89321 2023-03-27 15:10:53.478462 clinica-0.7.4/clinica/iotools/data/clinical_specifications_adni_sessions.tsv
--rw-r--r--   0        0        0     2708 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/data/clinical_specifications_participant.tsv
--rw-r--r--   0        0        0     1136 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/data/clinical_specifications_scans.tsv
--rw-r--r--   0        0        0    32532 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/data/clinical_specifications_sessions.tsv
--rw-r--r--   0        0        0     7743 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/data/genfi_ref.csv
--rw-r--r--   0        0        0      271 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/data/modality_equiv.tsv
--rw-r--r--   0        0        0      243 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/data/ukb_ref.csv
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/utils/__init__.py
--rw-r--r--   0        0        0     8532 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/utils/cli.py
--rw-r--r--   0        0        0    54461 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/utils/data_handling.py
--rw-r--r--   0        0        0    14060 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/iotools/utils/pipeline_handling.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/__init__.py
--rw-r--r--   0        0        0       65 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/char.m
--rw-r--r--   0        0        0      465 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/display.m
--rw-r--r--   0        0        0       67 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/double.m
--rw-r--r--   0        0        0     1135 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/image.m
--rw-r--r--   0        0        0       76 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/isempty.m
--rw-r--r--   0        0        0      671 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m
--rw-r--r--   0        0        0       85 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/mpower.m
--rw-r--r--   0        0        0     1873 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m
--rw-r--r--   0        0        0      732 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m
--rw-r--r--   0        0        0     5850 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/random.m
--rw-r--r--   0        0        0       92 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/size.m
--rw-r--r--   0        0        0       46 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/subsref.m
--rw-r--r--   0        0        0       30 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/char.m
--rw-r--r--   0        0        0      315 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/display.m
--rw-r--r--   0        0        0       33 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/double.m
--rw-r--r--   0        0        0      574 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/image.m
--rw-r--r--   0        0        0       43 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/isempty.m
--rw-r--r--   0        0        0      694 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m
--rw-r--r--   0        0        0      116 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/mpower.m
--rw-r--r--   0        0        0     1166 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m
--rw-r--r--   0        0        0      828 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m
--rw-r--r--   0        0        0       97 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/size.m
--rw-r--r--   0        0        0      178 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/subsref.m
--rw-r--r--   0        0        0     3878 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/term.m
--rw-r--r--   0        0        0      102 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/I.m
--rw-r--r--   0        0        0     1340 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m
--rw-r--r--   0        0        0     1662 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m
--rw-r--r--   0        0        0      750 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m
--rw-r--r--   0        0        0      567 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m
--rw-r--r--   0        0        0     1491 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m
--rw-r--r--   0        0        0      497 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursor.m
--rw-r--r--   0        0        0      692 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m
--rw-r--r--   0        0        0      636 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m
--rw-r--r--   0        0        0     2172 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m
--rw-r--r--   0        0        0     2384 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m
--rw-r--r--   0        0        0     3989 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m
--rw-r--r--   0        0        0     1099 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m
--rw-r--r--   0        0        0     2615 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m
--rw-r--r--   0        0        0    10279 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m
--rw-r--r--   0        0        0      946 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m
--rw-r--r--   0        0        0      995 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m
--rw-r--r--   0        0        0     1925 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m
--rw-r--r--   0        0        0     3891 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m
--rw-r--r--   0        0        0     4053 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m
--rw-r--r--   0        0        0     4282 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m
--rw-r--r--   0        0        0     4388 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m
--rw-r--r--   0        0        0     1687 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m
--rw-r--r--   0        0        0     1448 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m
--rw-r--r--   0        0        0     3855 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m
--rw-r--r--   0        0        0     1599 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m
--rw-r--r--   0        0        0     4371 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m
--rw-r--r--   0        0        0     6091 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m
--rw-r--r--   0        0        0     5816 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m
--rw-r--r--   0        0        0    17058 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m
--rw-r--r--   0        0        0    17594 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m
--rw-r--r--   0        0        0     2202 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m
--rw-r--r--   0        0        0      860 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m
--rw-r--r--   0        0        0     3190 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m
--rw-r--r--   0        0        0     5852 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m
--rw-r--r--   0        0        0     5335 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m
--rw-r--r--   0        0        0    11047 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m
--rw-r--r--   0        0        0     7015 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m
--rw-r--r--   0        0        0     7036 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m
--rw-r--r--   0        0        0     6798 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m
--rw-r--r--   0        0        0     2751 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m
--rw-r--r--   0        0        0     1976 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m
--rw-r--r--   0        0        0     1196 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m
--rw-r--r--   0        0        0     2395 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m
--rw-r--r--   0        0        0     3385 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m
--rw-r--r--   0        0        0     1231 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m
--rw-r--r--   0        0        0    19785 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m
--rw-r--r--   0        0        0      470 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/fac2var.m
--rw-r--r--   0        0        0     1588 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/gl.m
--rw-r--r--   0        0        0     1404 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD
--rw-r--r--   0        0        0      348 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.hdr
--rw-r--r--   0        0        0     4096 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc
--rw-r--r--   0        0        0     2021 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/redmod.m
--rw-r--r--   0        0        0      996 2023-03-27 15:10:53.482462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/spectral.m
--rw-r--r--   0        0        0    27286 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m
--rw-r--r--   0        0        0      836 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/var2fac.m
--rwxr-xr-x   0        0        0    25158 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/lib/clinicasurfstat/clinicasurfstat.m
--rw-r--r--   0        0        0      626 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/__init__.py
--rw-r--r--   0        0        0      369 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/cli.py
--rw-r--r--   0        0        0       45 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/cli_param/__init__.py
--rw-r--r--   0        0        0     1316 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/cli_param/argument.py
--rw-r--r--   0        0        0     5063 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/cli_param/option.py
--rw-r--r--   0        0        0      538 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/cli_param/option_group.py
--rw-r--r--   0        0        0       44 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/deeplearning_prepare_data/__init__.py
--rw-r--r--   0        0        0      584 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py
--rw-r--r--   0        0        0       33 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_connectome/__init__.py
--rw-r--r--   0        0        0     1768 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_connectome/dwi_connectome_cli.py
--rw-r--r--   0        0        0    21183 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_connectome/dwi_connectome_pipeline.py
--rw-r--r--   0        0        0     4272 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_connectome/dwi_connectome_utils.py
--rw-r--r--   0        0        0      549 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_connectome/info.json
--rw-r--r--   0        0        0       26 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_dti/__init__.py
--rw-r--r--   0        0        0     1363 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_dti/dwi_dti_cli.py
--rw-r--r--   0        0        0    19803 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_dti/dwi_dti_pipeline.py
--rw-r--r--   0        0        0     4297 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_dti/dwi_dti_utils.py
--rw-r--r--   0        0        0      523 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_dti/info.json
--rw-r--r--   0        0        0       57 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/__init__.py
--rw-r--r--   0        0        0     2042 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_cli.py
--rw-r--r--   0        0        0    21195 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_pipeline.py
--rw-r--r--   0        0        0     6071 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_utils.py
--rw-r--r--   0        0        0     9598 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_workflows.py
--rw-r--r--   0        0        0      558 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/info.json
--rw-r--r--   0        0        0       45 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/__init__.py
--rw-r--r--   0        0        0     2067 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_cli.py
--rw-r--r--   0        0        0    16188 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_pipeline.py
--rw-r--r--   0        0        0    10951 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_utils.py
--rw-r--r--   0        0        0    17286 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_workflows.py
--rw-r--r--   0        0        0      693 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/info.json
--rw-r--r--   0        0        0    34637 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/engine.py
--rw-r--r--   0        0        0       33 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/__init__.py
--rw-r--r--   0        0        0    48753 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/algorithm.py
--rw-r--r--   0        0        0     4225 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/base.py
--rw-r--r--   0        0        0     8026 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/classification_cli.py
--rw-r--r--   0        0        0    21823 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/input.py
--rw-r--r--   0        0        0     4105 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/ml_utils.py
--rw-r--r--   0        0        0    11517 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/ml_workflows.py
--rw-r--r--   0        0        0     2900 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/region_based_io.py
--rw-r--r--   0        0        0      934 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/tsv_based_io.py
--rw-r--r--   0        0        0    34670 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/validation.py
--rw-r--r--   0        0        0     1120 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/vertex_based_io.py
--rw-r--r--   0        0        0     2931 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning/voxel_based_io.py
--rw-r--r--   0        0        0       30 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/__init__.py
--rw-r--r--   0        0        0      190 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/info.json
--rw-r--r--   0        0        0     3745 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py
--rw-r--r--   0        0        0    11190 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py
--rw-r--r--   0        0        0    27936 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py
--rw-r--r--   0        0        0       29 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_linear/__init__.py
--rw-r--r--   0        0        0      283 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_linear/info.json
--rw-r--r--   0        0        0     2782 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_linear/pet_linear_cli.py
--rw-r--r--   0        0        0    17396 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_linear/pet_linear_pipeline.py
--rw-r--r--   0        0        0     6000 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_linear/pet_linear_utils.py
--rw-r--r--   0        0        0       60 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_surface/__init__.py
--rw-r--r--   0        0        0     1050 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_surface/applyInverseDeformationField.m
--rw-r--r--   0        0        0      549 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_surface/info.json
--rw-r--r--   0        0        0     2483 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_cli.py
--rw-r--r--   0        0        0     2533 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py
--rw-r--r--   0        0        0    16761 2023-03-27 15:10:53.486462 clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_pipeline.py
--rw-r--r--   0        0        0    53035 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_utils.py
--rw-r--r--   0        0        0       29 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/pet_volume/__init__.py
--rw-r--r--   0        0        0      286 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/pet_volume/info.json
--rw-r--r--   0        0        0     4136 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/pet_volume/pet_volume_cli.py
--rw-r--r--   0        0        0    31383 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/pet_volume/pet_volume_pipeline.py
--rw-r--r--   0        0        0     7995 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/pet_volume/pet_volume_utils.py
--rw-r--r--   0        0        0       37 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/__init__.py
--rw-r--r--   0        0        0     4956 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/_inputs.py
--rw-r--r--   0        0        0    32950 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/_model.py
--rw-r--r--   0        0        0     5484 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/clinica_surfstat.py
--rw-r--r--   0        0        0      346 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/info.json
--rw-r--r--   0        0        0     6600 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/statistics_surface_cli.py
--rw-r--r--   0        0        0     8864 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/statistics_surface_pipeline.py
--rw-r--r--   0        0        0     9556 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_surface/statistics_surface_utils.py
--rw-r--r--   0        0        0       36 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/__init__.py
--rw-r--r--   0        0        0      287 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/info.json
--rw-r--r--   0        0        0     5826 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/statistics_volume_cli.py
--rw-r--r--   0        0        0    19112 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py
--rw-r--r--   0        0        0    20425 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/statistics_volume_utils.py
--rw-r--r--   0        0        0      811 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_contrast.m
--rw-r--r--   0        0        0     1106 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_creation.m
--rw-r--r--   0        0        0      336 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_estimation.m
--rw-r--r--   0        0        0      781 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_results.m
--rw-r--r--   0        0        0       47 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume_correction/__init__.py
--rw-r--r--   0        0        0      180 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume_correction/info.json
--rw-r--r--   0        0        0     2588 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py
--rw-r--r--   0        0        0     9080 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py
--rw-r--r--   0        0        0     6259 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py
--rw-r--r--   0        0        0       32 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer/__init__.py
--rw-r--r--   0        0        0      306 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer/info.json
--rw-r--r--   0        0        0     2556 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py
--rw-r--r--   0        0        0     9840 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py
--rw-r--r--   0        0        0     4845 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py
--rw-r--r--   0        0        0     5011 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/__init__.py
--rw-r--r--   0        0        0      290 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/info.json
--rw-r--r--   0        0        0     7315 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py
--rw-r--r--   0        0        0     1136 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py
--rw-r--r--   0        0        0     5242 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py
--rw-r--r--   0        0        0      133 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/__init__.py
--rw-r--r--   0        0        0      324 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/info.json
--rw-r--r--   0        0        0     5953 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py
--rw-r--r--   0        0        0     2789 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py
--rw-r--r--   0        0        0     2046 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py
--rw-r--r--   0        0        0    11880 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py
--rw-r--r--   0        0        0    11872 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py
--rw-r--r--   0        0        0     1564 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py
--rw-r--r--   0        0        0    12481 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py
--rw-r--r--   0        0        0     8646 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py
--rw-r--r--   0        0        0       46 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_linear/__init__.py
--rw-r--r--   0        0        0    12481 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_linear/anat_linear_pipeline.py
--rw-r--r--   0        0        0     2233 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_linear/anat_linear_utils.py
--rw-r--r--   0        0        0     1983 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_linear/flair_linear_cli.py
--rw-r--r--   0        0        0      281 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_linear/info.json
--rw-r--r--   0        0        0     1978 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_linear/t1_linear_cli.py
--rw-r--r--   0        0        0       28 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume/__init__.py
--rw-r--r--   0        0        0      305 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume/info.json
--rw-r--r--   0        0        0     5051 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume/t1_volume_cli.py
--rw-r--r--   0        0        0       42 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_create_dartel/__init__.py
--rw-r--r--   0        0        0      300 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_create_dartel/info.json
--rw-r--r--   0        0        0     2065 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py
--rw-r--r--   0        0        0     9448 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py
--rw-r--r--   0        0        0       39 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/__init__.py
--rw-r--r--   0        0        0      312 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/info.json
--rw-r--r--   0        0        0     2362 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py
--rw-r--r--   0        0        0    12539 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py
--rw-r--r--   0        0        0      301 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_utils.py
--rw-r--r--   0        0        0       46 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_existing_template/__init__.py
--rw-r--r--   0        0        0      303 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_existing_template/info.json
--rw-r--r--   0        0        0     4479 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py
--rw-r--r--   0        0        0       41 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/__init__.py
--rw-r--r--   0        0        0      178 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/info.json
--rw-r--r--   0        0        0     1932 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py
--rw-r--r--   0        0        0     5635 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py
--rw-r--r--   0        0        0     1376 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py
--rw-r--r--   0        0        0       44 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/__init__.py
--rw-r--r--   0        0        0      301 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/info.json
--rw-r--r--   0        0        0     2048 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py
--rw-r--r--   0        0        0     7991 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py
--rw-r--r--   0        0        0     5645 2023-03-27 15:10:53.490462 clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py
--rw-r--r--   0        0        0       48 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/__init__.py
--rw-r--r--   0        0        0      343 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/info.json
--rw-r--r--   0        0        0     2488 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py
--rw-r--r--   0        0        0    11729 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py
--rw-r--r--   0        0        0     5162 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py
--rw-r--r--   0        0        0       74 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/__init__.py
--rw-r--r--   0        0        0     5861 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/engine.py
--rw-r--r--   0        0        0     2583 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/engine_utils.py
--rw-r--r--   0        0        0     4943 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/interfaces.py
--rw-r--r--   0        0        0       29 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_linear/__init__.py
--rw-r--r--   0        0        0     2975 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_linear/pet_linear_cli.py
--rw-r--r--   0        0        0     6798 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_linear/pipeline.py
--rw-r--r--   0        0        0     1718 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_linear/tasks.py
--rw-r--r--   0        0        0       29 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_volume/__init__.py
--rw-r--r--   0        0        0     3534 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_volume/pet_volume_cli.py
--rw-r--r--   0        0        0    12249 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_volume/pipeline.py
--rw-r--r--   0        0        0     4532 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/pet_volume/tasks.py
--rw-r--r--   0        0        0    10890 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/query.py
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/shared_workflows/__init__.py
--rw-r--r--   0        0        0     1408 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/shared_workflows/smoothing.py
--rw-r--r--   0        0        0       21 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_freesurfer/__init__.py
--rw-r--r--   0        0        0      817 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_freesurfer/cli.py
--rw-r--r--   0        0        0     2836 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_freesurfer/pipeline.py
--rw-r--r--   0        0        0      886 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_freesurfer/tasks.py
--rw-r--r--   0        0        0       28 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_linear/__init__.py
--rw-r--r--   0        0        0     2757 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_linear/t1_linear.py
--rw-r--r--   0        0        0     1343 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_linear/t1_linear_cli.py
--rw-r--r--   0        0        0       78 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/__init__.py
--rw-r--r--   0        0        0       18 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/create_dartel/__init__.py
--rw-r--r--   0        0        0     1834 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/create_dartel/cli.py
--rw-r--r--   0        0        0     2301 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/create_dartel/pipeline.py
--rw-r--r--   0        0        0       18 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/__init__.py
--rw-r--r--   0        0        0     1928 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/cli.py
--rw-r--r--   0        0        0     3858 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/pipeline.py
--rw-r--r--   0        0        0     2311 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/tasks.py
--rw-r--r--   0        0        0       18 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/register_dartel/__init__.py
--rw-r--r--   0        0        0     2251 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/register_dartel/cli.py
--rw-r--r--   0        0        0     3964 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/register_dartel/pipeline.py
--rw-r--r--   0        0        0     2728 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/tasks.py
--rw-r--r--   0        0        0       18 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/tissue_segmentation/__init__.py
--rw-r--r--   0        0        0     2101 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/tissue_segmentation/cli.py
--rw-r--r--   0        0        0     2452 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py
--rw-r--r--   0        0        0     1008 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/t1_volume/utils.py
--rw-r--r--   0        0        0     1093 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/tasks.py
--rw-r--r--   0        0        0     2628 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/pydra/utils.py
--rwxr-xr-x   0        0        0      966 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-AAL2.txt
--rw-r--r--   0        0        0    76312 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz
--rw-r--r--   0        0        0     2311 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-AAL2_dseg.tsv
--rwxr-xr-x   0        0        0     1779 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-AICHA.txt
--rw-r--r--   0        0        0    94631 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz
--rw-r--r--   0        0        0     8548 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-AICHA_dseg.tsv
--rw-r--r--   0        0        0     1873 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-Hammers_dseg.tsv
--rw-r--r--   0        0        0     1916 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv
--rw-r--r--   0        0        0      684 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-JHUTract_dseg.tsv
--rw-r--r--   0        0        0     1535 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-LPBA40_dseg.tsv
--rw-r--r--   0        0        0     4151 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv
--rw-r--r--   0        0        0      146 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/fmri/task-facesshapesemotion_events.tsv
--rw-r--r--   0        0        0     3872 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/label_conversion_gtmsegmentation.csv
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/mappings/.emptyfile
--rw-r--r--   0        0        0     2661 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz
--rw-r--r--   0        0        0     7028 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz
--rw-r--r--   0        0        0     1194 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz
--rw-r--r--   0        0        0     4418 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz
--rw-r--r--   0        0        0     2774 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/templates/pipeline_template/README.md.j2
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/templates/pipeline_template/__init__.py.j2
--rw-r--r--   0        0        0     2622 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/templates/pipeline_template/cli.py.j2
--rw-r--r--   0        0        0      295 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/templates/pipeline_template/info.json.j2
--rw-r--r--   0        0        0     5460 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/templates/pipeline_template/pipeline.py.j2
--rw-r--r--   0        0        0      713 2023-03-27 15:10:53.494462 clinica-0.7.4/clinica/resources/templates/pipeline_template/utils.py.j2
--rw-r--r--   0        0        0      258 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/resources/templates/pipeline_template/visualizer.py.j2
--rw-r--r--   0        0        0        0 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/__init__.py
--rw-r--r--   0        0        0    12628 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/atlas.py
--rw-r--r--   0        0        0     6513 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/check_dependency.py
--rw-r--r--   0        0        0    13165 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/dwi.py
--rw-r--r--   0        0        0     1301 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/exceptions.py
--rw-r--r--   0        0        0    17193 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/filemanip.py
--rw-r--r--   0        0        0     1670 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/fmap.py
--rw-r--r--   0        0        0    14439 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/freesurfer.py
--rw-r--r--   0        0        0      758 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/group.py
--rw-r--r--   0        0        0    22787 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/input_files.py
--rw-r--r--   0        0        0    26990 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/inputs.py
--rw-r--r--   0        0        0     3473 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/longitudinal.py
--rw-r--r--   0        0        0     1536 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/mri_registration.py
--rw-r--r--   0        0        0     1615 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/nipype.py
--rw-r--r--   0        0        0     5124 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/participant.py
--rw-r--r--   0        0        0     4967 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/pet.py
--rw-r--r--   0        0        0     4302 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/spm.py
--rw-r--r--   0        0        0     2586 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/statistics.py
--rw-r--r--   0        0        0     1035 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/stream.py
--rw-r--r--   0        0        0     6687 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/testing_utils.py
--rw-r--r--   0        0        0     5459 2023-03-27 15:10:53.498462 clinica-0.7.4/clinica/utils/ux.py
--rw-r--r--   0        0        0     2541 2023-03-27 15:10:53.522462 clinica-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    11103 1970-01-01 00:00:00.000000 clinica-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    11842 2023-06-06 07:13:19.949931 clinica-0.7.5/LICENSE.txt
+-rw-r--r--   0        0        0     8791 2023-06-06 07:13:19.949931 clinica-0.7.5/README.md
+-rw-r--r--   0        0        0      175 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/__init__.py
+-rw-r--r--   0        0        0     3020 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/cmdline.py
+-rw-r--r--   0        0        0       67 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/compat.py
+-rw-r--r--   0        0        0       33 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/engine/__init__.py
+-rw-r--r--   0        0        0     5730 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/engine/cmdparser.py
+-rw-r--r--   0        0        0     1908 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/engine/template.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/iotools/__init__.py
+-rw-r--r--   0        0        0      225 2023-06-06 07:13:19.949931 clinica-0.7.5/clinica/iotools/abstract_converter.py
+-rw-r--r--   0        0        0     1405 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/bids_dataset_description.py
+-rw-r--r--   0        0        0      636 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/bids_readme.py
+-rw-r--r--   0        0        0    33362 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/bids_utils.py
+-rw-r--r--   0        0        0    11818 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converter_utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/__init__.py
+-rw-r--r--   0        0        0    20026 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_json.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/__init__.py
+-rw-r--r--   0        0        0     4873 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py
+-rw-r--r--   0        0        0     8842 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py
+-rw-r--r--   0        0        0     4761 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py
+-rw-r--r--   0        0        0     7121 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py
+-rw-r--r--   0        0        0     7214 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py
+-rw-r--r--   0        0        0     4067 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py
+-rw-r--r--   0        0        0    20724 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py
+-rw-r--r--   0        0        0     4555 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py
+-rw-r--r--   0        0        0    10270 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_to_bids.py
+-rw-r--r--   0        0        0     2407 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py
+-rw-r--r--   0        0        0    47710 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/__init__.py
+-rw-r--r--   0        0        0     2703 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py
+-rw-r--r--   0        0        0     1310 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py
+-rw-r--r--   0        0        0    36162 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/aibl_utils.py
+-rw-r--r--   0        0        0      833 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/cli.py
+-rw-r--r--   0        0        0      875 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/cli_param.py
+-rw-r--r--   0        0        0     2738 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py
+-rw-r--r--   0        0        0     1421 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py
+-rw-r--r--   0        0        0    31992 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/habs_to_bids/__init__.py
+-rw-r--r--   0        0        0     9025 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/habs_to_bids/habs_to_bids.py
+-rw-r--r--   0        0        0     1040 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/__init__.py
+-rw-r--r--   0        0        0     1840 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py
+-rw-r--r--   0        0        0      969 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py
+-rw-r--r--   0        0        0    12134 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/nifd_utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/__init__.py
+-rw-r--r--   0        0        0     2509 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py
+-rw-r--r--   0        0        0      947 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py
+-rw-r--r--   0        0        0    11878 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis_to_bids/__init__.py
+-rw-r--r--   0        0        0     7287 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py
+-rw-r--r--   0        0        0      848 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/__init__.py
+-rw-r--r--   0        0        0     2094 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py
+-rw-r--r--   0        0        0     1041 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py
+-rw-r--r--   0        0        0    16773 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/ukb_utils.py
+-rw-r--r--   0        0        0     2383 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/clinical_specifications_adni_participant.tsv
+-rw-r--r--   0        0        0      244 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/clinical_specifications_adni_scans.tsv
+-rw-r--r--   0        0        0    89321 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/clinical_specifications_adni_sessions.tsv
+-rw-r--r--   0        0        0     2708 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/clinical_specifications_participant.tsv
+-rw-r--r--   0        0        0     1136 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/clinical_specifications_scans.tsv
+-rw-r--r--   0        0        0    32532 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/clinical_specifications_sessions.tsv
+-rw-r--r--   0        0        0     7777 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/genfi_ref.csv
+-rw-r--r--   0        0        0      271 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/modality_equiv.tsv
+-rw-r--r--   0        0        0      243 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/data/ukb_ref.csv
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/utils/__init__.py
+-rw-r--r--   0        0        0     8532 2023-06-06 07:13:19.953932 clinica-0.7.5/clinica/iotools/utils/cli.py
+-rw-r--r--   0        0        0    54461 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/iotools/utils/data_handling.py
+-rw-r--r--   0        0        0    14060 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/iotools/utils/pipeline_handling.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/char.m
+-rw-r--r--   0        0        0      465 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/display.m
+-rw-r--r--   0        0        0       67 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/double.m
+-rw-r--r--   0        0        0     1135 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/image.m
+-rw-r--r--   0        0        0       76 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/isempty.m
+-rw-r--r--   0        0        0      671 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m
+-rw-r--r--   0        0        0       85 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/mpower.m
+-rw-r--r--   0        0        0     1873 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m
+-rw-r--r--   0        0        0      732 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m
+-rw-r--r--   0        0        0     5850 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/random.m
+-rw-r--r--   0        0        0       92 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/size.m
+-rw-r--r--   0        0        0       46 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/subsref.m
+-rw-r--r--   0        0        0       30 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/char.m
+-rw-r--r--   0        0        0      315 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/display.m
+-rw-r--r--   0        0        0       33 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/double.m
+-rw-r--r--   0        0        0      574 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/image.m
+-rw-r--r--   0        0        0       43 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/isempty.m
+-rw-r--r--   0        0        0      694 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m
+-rw-r--r--   0        0        0      116 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/mpower.m
+-rw-r--r--   0        0        0     1166 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m
+-rw-r--r--   0        0        0      828 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m
+-rw-r--r--   0        0        0       97 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/size.m
+-rw-r--r--   0        0        0      178 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/subsref.m
+-rw-r--r--   0        0        0     3878 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/term.m
+-rw-r--r--   0        0        0      102 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/I.m
+-rw-r--r--   0        0        0     1340 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m
+-rw-r--r--   0        0        0     1662 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m
+-rw-r--r--   0        0        0      750 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m
+-rw-r--r--   0        0        0      567 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m
+-rw-r--r--   0        0        0     1491 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m
+-rw-r--r--   0        0        0      497 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursor.m
+-rw-r--r--   0        0        0      692 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m
+-rw-r--r--   0        0        0      636 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m
+-rw-r--r--   0        0        0     2172 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m
+-rw-r--r--   0        0        0     2384 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m
+-rw-r--r--   0        0        0     3989 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m
+-rw-r--r--   0        0        0     1099 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m
+-rw-r--r--   0        0        0     2615 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m
+-rw-r--r--   0        0        0    10279 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m
+-rw-r--r--   0        0        0      946 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m
+-rw-r--r--   0        0        0      995 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m
+-rw-r--r--   0        0        0     1925 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m
+-rw-r--r--   0        0        0     3891 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m
+-rw-r--r--   0        0        0     4053 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m
+-rw-r--r--   0        0        0     4282 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m
+-rw-r--r--   0        0        0     4388 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m
+-rw-r--r--   0        0        0     1687 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m
+-rw-r--r--   0        0        0     1448 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m
+-rw-r--r--   0        0        0     3855 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m
+-rw-r--r--   0        0        0     1599 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m
+-rw-r--r--   0        0        0     4371 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m
+-rw-r--r--   0        0        0     6091 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m
+-rw-r--r--   0        0        0     5816 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m
+-rw-r--r--   0        0        0    17058 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m
+-rw-r--r--   0        0        0    17594 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m
+-rw-r--r--   0        0        0     2202 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m
+-rw-r--r--   0        0        0      860 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m
+-rw-r--r--   0        0        0     3190 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m
+-rw-r--r--   0        0        0     5852 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m
+-rw-r--r--   0        0        0     5335 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m
+-rw-r--r--   0        0        0    11047 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m
+-rw-r--r--   0        0        0     7015 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m
+-rw-r--r--   0        0        0     7036 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m
+-rw-r--r--   0        0        0     6798 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m
+-rw-r--r--   0        0        0     2751 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m
+-rw-r--r--   0        0        0     1976 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m
+-rw-r--r--   0        0        0     1196 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m
+-rw-r--r--   0        0        0     2395 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m
+-rw-r--r--   0        0        0     3385 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m
+-rw-r--r--   0        0        0     1231 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m
+-rw-r--r--   0        0        0    19785 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m
+-rw-r--r--   0        0        0      470 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/fac2var.m
+-rw-r--r--   0        0        0     1588 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/gl.m
+-rw-r--r--   0        0        0     1404 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD
+-rw-r--r--   0        0        0      348 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.hdr
+-rw-r--r--   0        0        0     4096 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc
+-rw-r--r--   0        0        0     2021 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/redmod.m
+-rw-r--r--   0        0        0      996 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/spectral.m
+-rw-r--r--   0        0        0    27286 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m
+-rw-r--r--   0        0        0      836 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/var2fac.m
+-rwxr-xr-x   0        0        0    25158 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/lib/clinicasurfstat/clinicasurfstat.m
+-rw-r--r--   0        0        0      626 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/__init__.py
+-rw-r--r--   0        0        0      369 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/cli.py
+-rw-r--r--   0        0        0       45 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/cli_param/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/cli_param/argument.py
+-rw-r--r--   0        0        0     5190 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/cli_param/option.py
+-rw-r--r--   0        0        0      538 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/cli_param/option_group.py
+-rw-r--r--   0        0        0       44 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/deeplearning_prepare_data/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py
+-rw-r--r--   0        0        0       33 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/dwi_connectome/__init__.py
+-rw-r--r--   0        0        0     1768 2023-06-06 07:13:19.957932 clinica-0.7.5/clinica/pipelines/dwi_connectome/dwi_connectome_cli.py
+-rw-r--r--   0        0        0    21183 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_connectome/dwi_connectome_pipeline.py
+-rw-r--r--   0        0        0     4272 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_connectome/dwi_connectome_utils.py
+-rw-r--r--   0        0        0      549 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_connectome/info.json
+-rw-r--r--   0        0        0       26 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_dti/__init__.py
+-rw-r--r--   0        0        0     1363 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_dti/dwi_dti_cli.py
+-rw-r--r--   0        0        0    19803 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_dti/dwi_dti_pipeline.py
+-rw-r--r--   0        0        0     4297 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_dti/dwi_dti_utils.py
+-rw-r--r--   0        0        0      523 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_dti/info.json
+-rw-r--r--   0        0        0       57 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/__init__.py
+-rw-r--r--   0        0        0     2042 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_cli.py
+-rw-r--r--   0        0        0    18732 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_pipeline.py
+-rw-r--r--   0        0        0     6591 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_utils.py
+-rw-r--r--   0        0        0    17955 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_workflows.py
+-rw-r--r--   0        0        0      558 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/info.json
+-rw-r--r--   0        0        0       45 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_cli.py
+-rw-r--r--   0        0        0    15962 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_pipeline.py
+-rw-r--r--   0        0        0    15906 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_utils.py
+-rw-r--r--   0        0        0    19190 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_workflows.py
+-rw-r--r--   0        0        0      693 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/info.json
+-rw-r--r--   0        0        0    34637 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/engine.py
+-rw-r--r--   0        0        0       33 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/__init__.py
+-rw-r--r--   0        0        0    48753 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/algorithm.py
+-rw-r--r--   0        0        0     4225 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/base.py
+-rw-r--r--   0        0        0     8026 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/classification_cli.py
+-rw-r--r--   0        0        0    21823 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/input.py
+-rw-r--r--   0        0        0     4105 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/ml_utils.py
+-rw-r--r--   0        0        0    11517 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/ml_workflows.py
+-rw-r--r--   0        0        0     2900 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/region_based_io.py
+-rw-r--r--   0        0        0      934 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/tsv_based_io.py
+-rw-r--r--   0        0        0    34670 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/validation.py
+-rw-r--r--   0        0        0     1120 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/vertex_based_io.py
+-rw-r--r--   0        0        0     2931 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning/voxel_based_io.py
+-rw-r--r--   0        0        0       30 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/__init__.py
+-rw-r--r--   0        0        0      190 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/info.json
+-rw-r--r--   0        0        0     3745 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py
+-rw-r--r--   0        0        0    11208 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py
+-rw-r--r--   0        0        0    27936 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py
+-rw-r--r--   0        0        0       29 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_linear/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_linear/info.json
+-rw-r--r--   0        0        0     2875 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_linear/pet_linear_cli.py
+-rw-r--r--   0        0        0    17560 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_linear/pet_linear_pipeline.py
+-rw-r--r--   0        0        0     6000 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_linear/pet_linear_utils.py
+-rw-r--r--   0        0        0       60 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/__init__.py
+-rw-r--r--   0        0        0     1050 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/applyInverseDeformationField.m
+-rw-r--r--   0        0        0      549 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/info.json
+-rw-r--r--   0        0        0     2483 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_cli.py
+-rw-r--r--   0        0        0     2533 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py
+-rw-r--r--   0        0        0    16761 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_pipeline.py
+-rw-r--r--   0        0        0    53035 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_utils.py
+-rw-r--r--   0        0        0       29 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_volume/__init__.py
+-rw-r--r--   0        0        0      286 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_volume/info.json
+-rw-r--r--   0        0        0     4136 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_volume/pet_volume_cli.py
+-rw-r--r--   0        0        0    31383 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_volume/pet_volume_pipeline.py
+-rw-r--r--   0        0        0     7995 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/pet_volume/pet_volume_utils.py
+-rw-r--r--   0        0        0       37 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/statistics_surface/__init__.py
+-rw-r--r--   0        0        0     4956 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/statistics_surface/_inputs.py
+-rw-r--r--   0        0        0    32950 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/statistics_surface/_model.py
+-rw-r--r--   0        0        0     5484 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/statistics_surface/clinica_surfstat.py
+-rw-r--r--   0        0        0      346 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/statistics_surface/info.json
+-rw-r--r--   0        0        0     6600 2023-06-06 07:13:19.961932 clinica-0.7.5/clinica/pipelines/statistics_surface/statistics_surface_cli.py
+-rw-r--r--   0        0        0     8864 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_surface/statistics_surface_pipeline.py
+-rw-r--r--   0        0        0     9556 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_surface/statistics_surface_utils.py
+-rw-r--r--   0        0        0       36 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/info.json
+-rw-r--r--   0        0        0     5826 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/statistics_volume_cli.py
+-rw-r--r--   0        0        0    19177 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py
+-rw-r--r--   0        0        0    27415 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/statistics_volume_utils.py
+-rw-r--r--   0        0        0      811 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_contrast.m
+-rw-r--r--   0        0        0     1106 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_creation.m
+-rw-r--r--   0        0        0      336 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_estimation.m
+-rw-r--r--   0        0        0      781 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_results.m
+-rw-r--r--   0        0        0       47 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume_correction/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume_correction/info.json
+-rw-r--r--   0        0        0     2588 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py
+-rw-r--r--   0        0        0     9135 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py
+-rw-r--r--   0        0        0     6317 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py
+-rw-r--r--   0        0        0       32 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer/info.json
+-rw-r--r--   0        0        0     2556 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py
+-rw-r--r--   0        0        0     9840 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py
+-rw-r--r--   0        0        0     4845 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py
+-rw-r--r--   0        0        0     5011 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/__init__.py
+-rw-r--r--   0        0        0      290 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/info.json
+-rw-r--r--   0        0        0     7315 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py
+-rw-r--r--   0        0        0     1136 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py
+-rw-r--r--   0        0        0     5242 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py
+-rw-r--r--   0        0        0      133 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/__init__.py
+-rw-r--r--   0        0        0      324 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/info.json
+-rw-r--r--   0        0        0     5953 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py
+-rw-r--r--   0        0        0     2789 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py
+-rw-r--r--   0        0        0     2046 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py
+-rw-r--r--   0        0        0    11880 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py
+-rw-r--r--   0        0        0    11872 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py
+-rw-r--r--   0        0        0     1564 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py
+-rw-r--r--   0        0        0    12481 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py
+-rw-r--r--   0        0        0     8646 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py
+-rw-r--r--   0        0        0       46 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_linear/__init__.py
+-rw-r--r--   0        0        0    12571 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_linear/anat_linear_pipeline.py
+-rw-r--r--   0        0        0     2233 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_linear/anat_linear_utils.py
+-rw-r--r--   0        0        0     2103 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_linear/flair_linear_cli.py
+-rw-r--r--   0        0        0      281 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_linear/info.json
+-rw-r--r--   0        0        0     2092 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_linear/t1_linear_cli.py
+-rw-r--r--   0        0        0       28 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume/info.json
+-rw-r--r--   0        0        0     5051 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume/t1_volume_cli.py
+-rw-r--r--   0        0        0       42 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_create_dartel/__init__.py
+-rw-r--r--   0        0        0      300 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_create_dartel/info.json
+-rw-r--r--   0        0        0     2065 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py
+-rw-r--r--   0        0        0     9448 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py
+-rw-r--r--   0        0        0       39 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/__init__.py
+-rw-r--r--   0        0        0      312 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/info.json
+-rw-r--r--   0        0        0     2362 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py
+-rw-r--r--   0        0        0    12539 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py
+-rw-r--r--   0        0        0      301 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_utils.py
+-rw-r--r--   0        0        0       46 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_existing_template/__init__.py
+-rw-r--r--   0        0        0      303 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_existing_template/info.json
+-rw-r--r--   0        0        0     4479 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py
+-rw-r--r--   0        0        0       41 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/info.json
+-rw-r--r--   0        0        0     1932 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py
+-rw-r--r--   0        0        0     5635 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py
+-rw-r--r--   0        0        0     1376 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py
+-rw-r--r--   0        0        0       44 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/info.json
+-rw-r--r--   0        0        0     2048 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py
+-rw-r--r--   0        0        0     7991 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py
+-rw-r--r--   0        0        0     5645 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py
+-rw-r--r--   0        0        0       48 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/info.json
+-rw-r--r--   0        0        0     2488 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py
+-rw-r--r--   0        0        0    11729 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py
+-rw-r--r--   0        0        0     5162 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py
+-rw-r--r--   0        0        0      190 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/__init__.py
+-rw-r--r--   0        0        0     5861 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/engine.py
+-rw-r--r--   0        0        0     2583 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/engine_utils.py
+-rw-r--r--   0        0        0     4943 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/interfaces.py
+-rw-r--r--   0        0        0       30 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/machine_learning_spatial_svm/__init__.py
+-rw-r--r--   0        0        0     4011 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/machine_learning_spatial_svm/pipeline.py
+-rw-r--r--   0        0        0     3032 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/machine_learning_spatial_svm/spatial_svm_cli.py
+-rw-r--r--   0        0        0     1731 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/machine_learning_spatial_svm/tasks.py
+-rw-r--r--   0        0        0       29 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/pet_linear/__init__.py
+-rw-r--r--   0        0        0     2975 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/pet_linear/pet_linear_cli.py
+-rw-r--r--   0        0        0     6810 2023-06-06 07:13:19.965932 clinica-0.7.5/clinica/pydra/pet_linear/pipeline.py
+-rw-r--r--   0        0        0     1718 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/pet_linear/tasks.py
+-rw-r--r--   0        0        0       29 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/pet_volume/__init__.py
+-rw-r--r--   0        0        0     3534 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/pet_volume/pet_volume_cli.py
+-rw-r--r--   0        0        0    12236 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/pet_volume/pipeline.py
+-rw-r--r--   0        0        0     4532 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/pet_volume/tasks.py
+-rw-r--r--   0        0        0    11197 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/query.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/shared_workflows/__init__.py
+-rw-r--r--   0        0        0     1408 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/shared_workflows/smoothing.py
+-rw-r--r--   0        0        0       36 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume/__init__.py
+-rw-r--r--   0        0        0     7915 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume/pipeline.py
+-rw-r--r--   0        0        0     4926 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume/statistics_volume_cli.py
+-rw-r--r--   0        0        0     4336 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume/task.py
+-rw-r--r--   0        0        0       47 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume_correction/__init__.py
+-rw-r--r--   0        0        0     3319 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume_correction/pipeline.py
+-rw-r--r--   0        0        0     2340 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume_correction/statistics_volume_correction_cli.py
+-rw-r--r--   0        0        0     2441 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/statistics_volume_correction/task.py
+-rw-r--r--   0        0        0       21 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_freesurfer/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_freesurfer/cli.py
+-rw-r--r--   0        0        0     2836 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_freesurfer/pipeline.py
+-rw-r--r--   0        0        0      886 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_freesurfer/tasks.py
+-rw-r--r--   0        0        0       28 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_linear/__init__.py
+-rw-r--r--   0        0        0     2769 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_linear/t1_linear.py
+-rw-r--r--   0        0        0     1343 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_linear/t1_linear_cli.py
+-rw-r--r--   0        0        0       78 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/__init__.py
+-rw-r--r--   0        0        0       18 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/create_dartel/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/create_dartel/cli.py
+-rw-r--r--   0        0        0     2301 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/create_dartel/pipeline.py
+-rw-r--r--   0        0        0       18 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/__init__.py
+-rw-r--r--   0        0        0     1928 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/cli.py
+-rw-r--r--   0        0        0     3858 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/pipeline.py
+-rw-r--r--   0        0        0     2311 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/tasks.py
+-rw-r--r--   0        0        0       18 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/register_dartel/__init__.py
+-rw-r--r--   0        0        0     2251 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/register_dartel/cli.py
+-rw-r--r--   0        0        0     3964 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/register_dartel/pipeline.py
+-rw-r--r--   0        0        0     2728 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/tasks.py
+-rw-r--r--   0        0        0       18 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/tissue_segmentation/__init__.py
+-rw-r--r--   0        0        0     2101 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/tissue_segmentation/cli.py
+-rw-r--r--   0        0        0     2452 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py
+-rw-r--r--   0        0        0     1008 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/t1_volume/utils.py
+-rw-r--r--   0        0        0     1377 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/tasks.py
+-rw-r--r--   0        0        0     2628 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/pydra/utils.py
+-rwxr-xr-x   0        0        0      966 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-AAL2.txt
+-rw-r--r--   0        0        0    76312 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz
+-rw-r--r--   0        0        0     2311 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-AAL2_dseg.tsv
+-rwxr-xr-x   0        0        0     1779 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-AICHA.txt
+-rw-r--r--   0        0        0    94631 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz
+-rw-r--r--   0        0        0     8548 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-AICHA_dseg.tsv
+-rw-r--r--   0        0        0     1873 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-Hammers_dseg.tsv
+-rw-r--r--   0        0        0     1916 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv
+-rw-r--r--   0        0        0      684 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-JHUTract_dseg.tsv
+-rw-r--r--   0        0        0     1535 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-LPBA40_dseg.tsv
+-rw-r--r--   0        0        0     4151 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv
+-rw-r--r--   0        0        0      146 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/fmri/task-facesshapesemotion_events.tsv
+-rw-r--r--   0        0        0     3872 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/label_conversion_gtmsegmentation.csv
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/mappings/.emptyfile
+-rw-r--r--   0        0        0     2661 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz
+-rw-r--r--   0        0        0     7028 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz
+-rw-r--r--   0        0        0     1194 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz
+-rw-r--r--   0        0        0     4418 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz
+-rw-r--r--   0        0        0     2774 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/README.md.j2
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/__init__.py.j2
+-rw-r--r--   0        0        0     2622 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/cli.py.j2
+-rw-r--r--   0        0        0      295 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/info.json.j2
+-rw-r--r--   0        0        0     5460 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/pipeline.py.j2
+-rw-r--r--   0        0        0      713 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/utils.py.j2
+-rw-r--r--   0        0        0      258 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/resources/templates/pipeline_template/visualizer.py.j2
+-rw-r--r--   0        0        0        0 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/utils/__init__.py
+-rw-r--r--   0        0        0    12628 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/utils/atlas.py
+-rw-r--r--   0        0        0     6513 2023-06-06 07:13:19.969932 clinica-0.7.5/clinica/utils/check_dependency.py
+-rw-r--r--   0        0        0    20108 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/dwi.py
+-rw-r--r--   0        0        0     1301 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/exceptions.py
+-rw-r--r--   0        0        0    17681 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/filemanip.py
+-rw-r--r--   0        0        0     1670 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/fmap.py
+-rw-r--r--   0        0        0    14439 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/freesurfer.py
+-rw-r--r--   0        0        0      758 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/group.py
+-rw-r--r--   0        0        0     5006 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/image.py
+-rw-r--r--   0        0        0    23063 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/input_files.py
+-rw-r--r--   0        0        0    26990 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/inputs.py
+-rw-r--r--   0        0        0     3473 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/longitudinal.py
+-rw-r--r--   0        0        0     1536 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/mri_registration.py
+-rw-r--r--   0        0        0     1643 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/nipype.py
+-rw-r--r--   0        0        0     5124 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/participant.py
+-rw-r--r--   0        0        0     4967 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/pet.py
+-rw-r--r--   0        0        0     4302 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/spm.py
+-rw-r--r--   0        0        0     2586 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/statistics.py
+-rw-r--r--   0        0        0     1035 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/stream.py
+-rw-r--r--   0        0        0     6687 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/testing_utils.py
+-rw-r--r--   0        0        0     5459 2023-06-06 07:13:19.973932 clinica-0.7.5/clinica/utils/ux.py
+-rw-r--r--   0        0        0     2607 2023-06-06 07:13:19.997932 clinica-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    11148 1970-01-01 00:00:00.000000 clinica-0.7.5/PKG-INFO
```

### Comparing `clinica-0.7.4/LICENSE.txt` & `clinica-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/README.md` & `clinica-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/cmdline.py` & `clinica-0.7.5/clinica/cmdline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/engine/cmdparser.py` & `clinica-0.7.5/clinica/engine/cmdparser.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/engine/template.py` & `clinica-0.7.5/clinica/engine/template.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/bids_dataset_description.py` & `clinica-0.7.5/clinica/iotools/bids_dataset_description.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/bids_readme.py` & `clinica-0.7.5/clinica/iotools/bids_readme.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/bids_utils.py` & `clinica-0.7.5/clinica/iotools/bids_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -859,15 +859,15 @@
 
 def run_dcm2niix(
     input_dir: str,
     output_dir: str,
     output_fmt: str,
     compress: bool = False,
     bids_sidecar: bool = True,
-) -> None:
+) -> bool:
     """Runs the `dcm2niix` command using a subprocess.
 
     Parameters
     ----------
     input_dir : str
         Input folder.
 
@@ -881,33 +881,41 @@
 
     compress : bool, optional
         Whether to compress or not.
         Default=False.
 
     bids_sidecar : bool, optional
         Whether to generate a BIDS sidecar or not. Default=True.
+
+    Returns
+    -------
+    bool :
+        True if the conversion was successful, False otherwise.
     """
     import subprocess
 
     from clinica.utils.stream import cprint
 
+    cprint(f"Attempting to convert {output_fmt}.", lvl="info")
     command = _build_dcm2niix_command(
         input_dir, output_dir, output_fmt, compress, bids_sidecar
     )
     completed_process = subprocess.run(command, capture_output=True)
 
     if completed_process.returncode != 0:
         cprint(
             msg=(
                 "DICOM to BIDS conversion with dcm2niix failed:\n"
                 f"command: {command}\n"
                 f"{completed_process.stdout.decode('utf-8')}"
             ),
             lvl="warning",
         )
+        return False
+    return True
 
 
 def identify_modality(filename: str) -> Optional[str]:
     """Identifies the modality of a file given its name.
 
     Parameters
     ----------
@@ -915,27 +923,29 @@
         Input filename
 
     Returns
     -------
     Optional[str]:
         Modality or None if parsing uns
     """
+    import numpy as np
+
     filename = filename.lower()
     if "dwi" in filename:
         return "dwi"
     if "t1" in filename:
         return "T1"
     if "t2" in filename:
         return "T2w"
     if "fieldmap" in filename:
         return "fieldmap"
     if "fmri" in filename:
         return "rsfmri"
     else:
-        return None
+        return np.nan
 
 
 def parse_description(filepath: PathLike, start_line: int, end_line: int) -> str:
     """Parse the description of the dataset from the readme in the documentation.
 
     Parameters
     ----------
```

### Comparing `clinica-0.7.4/clinica/iotools/converter_utils.py` & `clinica-0.7.5/clinica/iotools/converter_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -311,24 +311,65 @@
         table += f"{mod_key}"
         if len(mod_key) < 8:
             table += "\t"
         table += "\t| ".join([str(mod_value.get(d, "0")) for d in diagnoses]) + "\n"
     return table
 
 
-def viscode_to_session(viscode: str) -> str:
-    """Replace the session label 'bl' with 'M000' or capitalize the session name passed as input.
+def viscode_to_session(viscode: str, baseline_identifiers: Optional[set] = None) -> str:
+    """Replace the session label from 'baseline_identifiers' with 'ses-M000'.
+
+    If `viscode` is not a baseline identifier, parse the `viscode` and return
+    a session identifier of the form `ses-MXXX`.
+
+    The `viscode` is expected to be formatted in the following way:
+    "m/M{session_number}", where session_number can be casted to an integer.
+    Otherwise, a `ValueError` will be raised.
+
+    Note: This function doesn't perform any check on the number of digits
+    of the session identifier. It will return at least three digits encoded
+    session numbers, but doesn't raise if more digits are needed (see
+    examples section below).
 
     Parameters
     ----------
     viscode: str
         The name of the session.
 
+    baseline_identifiers : set of str, optional
+        Possible identifiers for baseline session.
+        If the `viscode` is among these identifiers, `ses-M000` is returned.
+        Default={"bl", "m0"}.
+
     Returns
     -------
     str:
-        "M000" if the session is the baseline session. Otherwise returns the original session name capitalized.
+        "ses-M000" if the session is the baseline session.
+        Otherwise returns the original session name capitalized.
+
+    Raises
+    ------
+    ValueError :
+        If the `viscode` isn't formatted as expected.
+
+    Examples
+    --------
+    >>> viscode_to_session("m1")
+    'ses-M001'
+    >>> viscode_to_session("M123")
+    'ses-M123'
+    >>> viscode_to_session("m1234")
+    'ses-M1234'
     """
-    if viscode in {"bl", "m0"}:
+    import re
+
+    baseline_identifiers = baseline_identifiers or {"bl", "m0"}
+    if viscode in baseline_identifiers:
         return "ses-M000"
-    else:
+    session_pattern = "^[m,M][0-9]*"
+    if re.match(session_pattern, viscode):
         return "ses-" + f"M{(int(viscode[1:])):03d}"
+    raise ValueError(
+        f"The viscode {viscode} is not correctly formatted."
+        "Expected a session identifier of the form 'MXXX', "
+        f"or a baseline identifier among {baseline_identifiers}."
+    )
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_json.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_json.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/adni_to_bids/adni_utils.py` & `clinica-0.7.5/clinica/iotools/converters/adni_to_bids/adni_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,35 @@
-from typing import Union
+from enum import Enum, auto
+from typing import Optional, Union
+
+import pandas as pd
+
+
+class ADNIStudy(Enum):
+    """Possible versions of ADNI studies."""
+
+    ADNI1 = auto()
+    ADNI2 = auto()
+    ADNI3 = auto()
+    ADNIGO = auto()
+
+    @classmethod
+    def from_string(cls, study_name: str):
+        if study_name == "ADNI1":
+            return cls.ADNI1
+        if study_name == "ADNI2":
+            return cls.ADNI2
+        if study_name == "ADNI3":
+            return cls.ADNI3
+        if study_name == "ADNIGO":
+            return cls.ADNIGO
+        raise ValueError(
+            f"Invalid study name for ADNI: {study_name}. "
+            f"Possible values are {list(ADNIStudy)}"
+        )
 
 
 def visits_to_timepoints(
     subject,
     mri_list_subj,
     adnimerge_subj,
     modality,
@@ -31,16 +58,16 @@
     visits = dict()
     unique_visits = list(mri_list_subj[visit_field].unique())
     pending_timepoints = []
 
     # We try to obtain the corresponding image Visit for a given VISCODE
     for adni_row in adnimerge_subj.iterrows():
         visit = adni_row[1]
-
-        preferred_visit_name = get_preferred_visit_name(visit)
+        study = ADNIStudy.from_string(visit.ORIGPROT)
+        preferred_visit_name = _get_preferred_visit_name(study, visit.VISCODE)
 
         if preferred_visit_name in unique_visits:
             key_preferred_visit = (visit.VISCODE, visit.COLPROT, visit.ORIGPROT)
             if key_preferred_visit not in visits.keys():
                 visits[key_preferred_visit] = preferred_visit_name
             elif visits[key_preferred_visit] != preferred_visit_name:
                 cprint(
@@ -70,54 +97,89 @@
             cprint(
                 f"[{modality}] Subject {subject} has multiple visits for one timepoint."
             )
 
     return visits
 
 
-def get_preferred_visit_name(visit):
-    """Provide the expected visit name for a given visit.
+def _get_preferred_visit_name(study: ADNIStudy, visit_code: str) -> str:
+    """Return the expected visit name for a given visit depending
+    on the study (ADNI1, ADNI2, ADNI3, ADNIGO).
+
+    Parameters
+    ----------
+    study : ADNIStudy
+        The study for this visit.
+    visit_code : str
+        The visit code to convert to a new form.
+
+    Returns
+    -------
+    str :
+        The expected visit name.
+    """
+    if study == ADNIStudy.ADNI3:
+        return _get_preferred_visit_name_adni3(visit_code)
+    if study == ADNIStudy.ADNI2:
+        return _get_preferred_visit_name_adni2(visit_code)
+    if study == ADNIStudy.ADNI1:
+        return _get_preferred_visit_name_adni1(visit_code)
+    if study == ADNIStudy.ADNIGO:
+        return _get_preferred_visit_name_adnigo(visit_code)
+
+
+def _get_preferred_visit_name_adni3(visit_code: str) -> str:
+    if visit_code == "bl":
+        return "ADNI Screening"
+    return f"ADNI3 Year {_parse_year_from_visit_code(visit_code)} Visit"
+
+
+def _parse_year_from_visit_code(visit_code: str) -> float:
+    """Return the year corresponding to the visit code.
+    Assumes a visit code of the form 'mXXX'.
+    """
+    return _parse_month_from_visit_code(visit_code) / 12
+
+
+def _parse_month_from_visit_code(visit_code: str) -> int:
+    """Return the month corresponding to the visit code.
+    Assumes a visit code of the form 'mXXX'.
+    """
+    try:
+        return int(visit_code[1:])
+    except Exception:
+        raise ValueError(
+            f"Cannot extract month from visit code {visit_code}."
+            "Expected a code of the form 'mXXX' where XXX can be casted to an integer."
+        )
 
-    Args:
-        visit: A visit entry from ADNIMERGE
 
-    Returns:
-        string: expected visit name
-    """
-    if visit.ORIGPROT == "ADNI3":
-        if visit.VISCODE == "bl":
-            preferred_visit_name = "ADNI Screening"
-        else:
-            year = str(int(visit.VISCODE[1:]) / 12)
-            preferred_visit_name = f"ADNI3 Year {year} Visit"
-    elif visit.ORIGPROT == "ADNI2":
-        if visit.VISCODE == "bl":
-            preferred_visit_name = "ADNI2 Screening MRI-New Pt"
-        elif visit.VISCODE == "m03":
-            preferred_visit_name = "ADNI2 Month 3 MRI-New Pt"
-        elif visit.VISCODE == "m06":
-            preferred_visit_name = "ADNI2 Month 6-New Pt"
-        else:
-            year = str(int(visit.VISCODE[1:]) / 12)
-            preferred_visit_name = f"ADNI2 Year {year} Visit"
-    else:
-        if visit.VISCODE == "bl":
-            if visit.ORIGPROT == "ADNI1":
-                preferred_visit_name = "ADNI Screening"
-            else:  # ADNIGO
-                preferred_visit_name = "ADNIGO Screening MRI"
-        elif visit.VISCODE == "m03":  # Only for ADNIGO Month 3
-            preferred_visit_name = "ADNIGO Month 3 MRI"
-        else:
-            month = int(visit.VISCODE[1:])
-            if month < 54:
-                preferred_visit_name = f"ADNI1/GO Month {str(month)}"
-            else:
-                preferred_visit_name = f"ADNIGO Month {str(month)}"
-    return preferred_visit_name
+def _get_preferred_visit_name_adni2(visit_code: str) -> str:
+    if visit_code == "bl":
+        return "ADNI2 Screening MRI-New Pt"
+    if visit_code == "m03":
+        return "ADNI2 Month 3 MRI-New Pt"
+    if visit_code == "m06":
+        return "ADNI2 Month 6-New Pt"
+    return f"ADNI2 Year {_parse_year_from_visit_code(visit_code)} Visit"
+
+
+def _get_preferred_visit_name_adni1(visit_code: str) -> str:
+    if visit_code == "bl":
+        return "ADNI Screening"
+    if visit_code == "m03":
+        return "ADNIGO Month 3 MRI"  # does not make any sense...
+    month = _parse_month_from_visit_code(visit_code)
+    return f"ADNI{'1/' if month < 54 else ''}GO Month {month}"
+
+
+def _get_preferred_visit_name_adnigo(visit_code: str) -> str:
+    if visit_code == "bl":
+        return "ADNIGO Screening MRI"
+    return _get_preferred_visit_name_adni1(visit_code)
 
 
 def get_closest_visit(image, pending_timepoints, subject, visit_field, scandate_field):
     """Choose the visit with the closest date to a given image acquisition date.
 
     Args:
         image: An image entry from MPRAGEMETA
@@ -627,21 +689,46 @@
     # Fill the rid with the needed number of zero
     if 4 - len(rid) > 0:
         zeros_to_add = 4 - len(rid)
         rid = "0" * zeros_to_add + rid
     return rid
 
 
-def get_visit_id(row, location):
-    """Return a common visit ID across different files"""
-    import pandas as pd
+def _compute_session_id(df: pd.DataFrame, csv_filename: str) -> pd.DataFrame:
+    """Compute session ID from visit code.
+
+    The CSV file name is used to determine in which column of
+    the dataframe the visit code should be found.
+    """
+    visit_code_column = _get_visit_code_column_name(csv_filename)
+    if visit_code_column not in df:
+        raise ValueError(
+            f"DataFrame does not contain a column named '{visit_code_column}', "
+            "which is supposed to encode the visit code. The columns present in "
+            f"the DataFrame are: {df.columns}."
+        )
+    return df.assign(
+        session_id=lambda _df: _df[visit_code_column].apply(
+            lambda x: _get_session_id_from_visit_code(x)
+        )
+    )
+
+
+def _get_visit_code_column_name(csv_filename: str) -> str:
+    """Return the name of the column containing the visit code."""
+    if _is_a_visit_code_2_type(csv_filename):
+        return "VISCODE2"
+    if _is_a_time_point_type(csv_filename):
+        return "Timepoint"
+    return "VISCODE"
 
-    from clinica.iotools.converter_utils import viscode_to_session
 
-    locations_visicode2 = [
+def _is_a_visit_code_2_type(csv_filename: str) -> bool:
+    """If the csv file is among these files, then the visit code column is 'VISCODE2'."""
+    return csv_filename in {
         "ADAS_ADNIGO2.csv",
         "DXSUM_PDXCONV_ADNIALL.csv",
         "CDR.csv",
         "NEUROBAT.csv",
         "GDSCALE.csv",
         "MODHACH.csv",
         "MOCA.csv",
@@ -652,32 +739,48 @@
         "UWNPSYCHSUM_03_26_20.csv",
         "ECOGPT.csv",
         "ECOGSP.csv",
         "FCI.csv",
         "CCI.csv",
         "NPIQ.csv",
         "NPI.csv",
-    ]
+    }
 
-    if location in locations_visicode2:
-        if pd.isnull(row["VISCODE2"]) or row["VISCODE2"] == "f":
-            return None
-        if row["VISCODE2"] == "sc":
-            return "sc"  # visit_id = "bl"
-        else:
-            visit_id = row["VISCODE2"]
-    elif location in [
+
+def _is_a_time_point_type(csv_filename: str) -> bool:
+    """If the csv file is among these files, then the visit code column is 'Timepoint'."""
+    return csv_filename in {
         "BHR_EVERYDAY_COGNITION.csv",
         "BHR_BASELINE_QUESTIONNAIRE.csv",
         "BHR_LONGITUDINAL_QUESTIONNAIRE.csv",
-    ]:
-        visit_id = row["Timepoint"]
-    else:
-        visit_id = row["VISCODE"]
-    return viscode_to_session(visit_id)
+    }
+
+
+def _get_session_id_from_visit_code(visit_code: str) -> Optional[str]:
+    """Checks that the visit code found in the data is supported by
+    the converter utility function `viscode_to_session` before using it.
+    There are a few special cases that are handled here.
+    """
+    from clinica.iotools.converter_utils import viscode_to_session
+
+    if _is_visit_code_not_supported(visit_code):
+        return None
+    if visit_code == "sc":
+        return "sc"
+    return viscode_to_session(visit_code)
+
+
+def _is_visit_code_not_supported(visit_code: str) -> bool:
+    """Return True is the visit code is not supported by the converter.
+
+    There are a few known values like "f" or "uns1" which are present in
+    ADNI data that are not supported for a mapping to a session ID.
+    """
+    unsupported_values = {"f", "uns1"}
+    return pd.isnull(visit_code) or visit_code in unsupported_values
 
 
 def create_adni_sessions_dict(
     bids_ids, clinic_specs_path, clinical_data_dir, bids_subjs_paths
 ):
     """Extract all the data required for the sessions files and organize them in a dictionary.
 
@@ -712,18 +815,15 @@
             file_to_read_path = path.join(clinical_data_dir, location)
             cprint(f"\tReading clinical data file: {location}")
 
             df_file = pd.read_csv(file_to_read_path, dtype=str)
             df_filtered = filter_subj_bids(df_file, location, bids_ids).copy()
 
             if not df_filtered.empty:
-                # Get session ID from visit code.
-                df_filtered["session_id"] = df_filtered.apply(
-                    lambda x: get_visit_id(x, location), axis=1
-                )
+                df_filtered = _compute_session_id(df_filtered, location)
 
                 # Filter rows with invalid session IDs.
                 df_filtered.dropna(subset="session_id", inplace=True)
 
                 if location == "ADNIMERGE.csv":
                     df_filtered["AGE"] = df_filtered.apply(
                         lambda x: update_age(x), axis=1
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/aibl_to_bids/aibl_utils.py` & `clinica-0.7.5/clinica/iotools/converters/aibl_to_bids/aibl_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/cli.py` & `clinica-0.7.5/clinica/iotools/converters/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/cli_param.py` & `clinica-0.7.5/clinica/iotools/converters/cli_param.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,29 +49,27 @@
     if path_to_clinical:
         df_demographics, df_imaging, df_clinical = find_clinical_data(path_to_clinical)
     # makes a df of the imaging data
     imaging_data = read_imaging_data(path_to_dataset)
 
     # complete the data extracted
     imaging_data = merge_imaging_data(imaging_data)
-
     # complete clinical data
     if path_to_clinical:
         df_clinical_complete = complete_clinical_data(
             df_demographics, df_imaging, df_clinical
         )
 
     # intersect the data
     if path_to_clinical:
         df_complete = intersect_data(imaging_data, df_clinical_complete)
     else:
         df_complete = imaging_data
     # build the tsv
     results = dataset_to_bids(df_complete, gif)
-
     write_bids(
         to=bids_dir,
         participants=results["participants"],
         sessions=results["sessions"],
         scans=results["scans"],
     )
     # fetch data for readme from markdown
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py` & `clinica-0.7.5/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from enum import Enum
 from os import PathLike
 from pathlib import Path
-from typing import Dict, Iterable, List, Tuple
+from typing import Dict, Iterable, List, Optional, Tuple
 
 import pandas as pd
 import pydicom as pdcm
 from pandas import DataFrame
 
 
 def find_dicoms(path_to_source_data: PathLike) -> Iterable[Tuple[PathLike, PathLike]]:
@@ -16,14 +17,17 @@
         Path to the source data
 
     Returns
     -------
     Iterable[Tuple[PathLike, PathLike]]
         Path to found files and parent directory
     """
+    from clinica.utils.stream import cprint
+
+    cprint("Looking for imaging data.", lvl="info")
     for z in Path(path_to_source_data).rglob("*.dcm"):
         yield str(z), str(Path(z).parent)
 
 
 def filter_dicoms(df: DataFrame) -> DataFrame:
     """Filters modalities handled by the converter.
 
@@ -54,57 +58,77 @@
         "motioncorrected",
         "localiser",
         "localizer",
     ]
 
     df = df.drop_duplicates(subset=["source"])
     df = df.assign(
-        series_desc=lambda df: df.source_path.apply(
-            lambda x: pdcm.dcmread(x).SeriesDescription
-        )
-    )
-    df = df.assign(
-        acq_date=lambda df: df.source_path.apply(lambda x: pdcm.dcmread(x).StudyDate)
+        series_desc=lambda x: x.source_path.apply(
+            lambda y: _handle_series_description(y)
+        ),
+        acq_date=lambda x: x.source_path.apply(lambda y: pdcm.dcmread(y).StudyDate),
+        manufacturer=lambda x: x.source_path.apply(lambda y: _handle_manufacturer(y)),
     )
     df = df.set_index(["source_path"], verify_integrity=True)
-
     df = df[~df["source"].str.contains("secondary", case=False)]
     for file_mod in to_filter:
         df = df[~df["series_desc"].str.contains(file_mod, case=False)]
     return df
 
 
+def _handle_series_description(x: str) -> str:
+    """This function handles the series description used to identify the modality later on.
+
+    In the case of T1 and T2, some dicoms are misnamed. The echo time and repetition time
+    are supposed to be very different between a T1 and T2. Therefore, we use this proxy to check that the series description is coherent.
+    The values used are in milliseconds, and have been chosen arbitrarily.
+    """
+    import warnings
+
+    MAX_ECHO_TIME_FOR_A_T1 = 60
+    MAX_REPETITION_TIME_FOR_A_T1 = 2100
+    series_description = pdcm.dcmread(x).SeriesDescription
+    if any([modality in series_description.lower() for modality in ["t1", "t2"]]):
+        try:
+            echo_time = pdcm.dcmread(x).EchoTime
+            repetition_time = pdcm.dcmread(x).RepetitionTime
+            if (
+                "t2" in series_description.lower()
+                and echo_time < MAX_ECHO_TIME_FOR_A_T1
+                and repetition_time < MAX_REPETITION_TIME_FOR_A_T1
+            ):
+                return "t1"
+        except AttributeError:
+            warnings.warn(
+                message=f"The subject from DICOM {Path(x).parent} has no Echo Time or Repetition Time, it might be wrongly converted."
+            )
+    return series_description
+
+
+def _handle_manufacturer(x: str) -> str:
+    try:
+        return pdcm.dcmread(x).Manufacturer
+    except:
+        return "Unknown"
+
+
 def _check_file(directory: PathLike, pattern: str) -> PathLike:
     from pathlib import Path
 
     try:
         data_file = list(Path(directory).glob(pattern))
     except StopIteration:
         raise FileNotFoundError("Clinical data file not found.")
     if len(data_file) == 0:
         raise FileNotFoundError("Clinical data not found or incomplete. Aborting")
     if len(data_file) > 1:
         raise ValueError("Too many data files found, expected one. Aborting.")
     return data_file[0]
 
 
-def _read_file(data_file: PathLike) -> pd.DataFrame:
-
-    return (
-        pd.concat(
-            [
-                pd.read_excel(str(data_file)),
-                pd.read_excel(str(data_file), sheet_name=1),
-            ]
-        )
-        .convert_dtypes()
-        .rename(columns=lambda x: x.lower().replace(" ", "_"))
-    )
-
-
 def find_clinical_data(
     clinical_data_directory: PathLike,
 ) -> List[DataFrame]:
     """Finds the clinical data associated with the dataset.
 
     Parameters
     ----------
@@ -112,24 +136,41 @@
         Path to the clinical data.
 
     Returns
     -------
     List[DataFrame]
         Dataframes containing the clinical data
     """
+    from clinica.utils.stream import cprint
+
+    cprint("Looking for clinical data.", lvl="info")
+
     return (
         _read_file(_check_file(clinical_data_directory, pattern))
         for pattern in (
             "FINAL*DEMOGRAPHICS*.xlsx",
             "FINAL*IMAGING*.xlsx",
             "FINAL*CLINICAL*.xlsx",
         )
     )
 
 
+def _read_file(data_file: PathLike) -> pd.DataFrame:
+    return (
+        pd.concat(
+            [
+                pd.read_excel(str(data_file)),
+                pd.read_excel(str(data_file), sheet_name=1),
+            ]
+        )
+        .convert_dtypes()
+        .rename(columns=lambda x: x.lower().replace(" ", "_"))
+    )
+
+
 def complete_clinical_data(
     df_demographics: DataFrame, df_imaging: DataFrame, df_clinical: DataFrame
 ) -> DataFrame:
     """Merges the different clincal dataframes into one.
 
     Parameters
     ----------
@@ -183,16 +224,18 @@
     -------
     Dict[str, DataFrame]
         Dictionary containing as key participants, sessions and scans, and the values wanted for each tsv
     """
     import os
 
     # generates participants, sessions and scans tsv
-    complete_data_df = complete_data_df.set_index(
-        ["participant_id", "session_id", "modality", "bids_filename"],
+    complete_data_df = complete_data_df.drop_duplicates(
+        subset=["participant_id", "session_id", "modality", "run_num", "bids_filename"]
+    ).set_index(
+        ["participant_id", "session_id", "modality", "run_num", "bids_filename"],
         verify_integrity=True,
     )
     # open the reference for building the tsvs:
     path_to_ref_csv = os.path.join(
         os.path.dirname(os.path.dirname(os.path.dirname(__file__))),
         "data",
         "genfi_ref.csv",
@@ -249,15 +292,90 @@
         Dataframe containing the data extracted.
     """
     return filter_dicoms(
         pd.DataFrame(find_dicoms(source_path), columns=["source_path", "source"])
     )
 
 
-def compute_baseline_date(df: DataFrame) -> DataFrame:
+def merge_imaging_data(df: DataFrame) -> DataFrame:
+    """This function uses the raw information extracted from the images,
+    to obtain all the information necessary for the BIDS conversion.
+
+    Parameters
+    ----------
+    df: DataFrame
+        Dataframe containing the data extracted from the images
+
+    Returns
+    -------
+    DataFrame :
+        Dataframe with the data necessary for the BIDS
+    """
+    df = _compute_source_id_and_source_ses_id(df).reset_index()
+    df = _compute_genfi_version(df)
+    df = _compute_baseline_and_session_numbers(df)
+    df = _compute_participant_id(df)
+    df = _compute_modality(df)
+    df = _compute_fieldmaps(df)
+    df = _compute_runs(df)
+    df = _compute_bids_full_path(df)
+
+    return df
+
+
+def _compute_source_id_and_source_ses_id(df: DataFrame) -> DataFrame:
+    """Adds two columns built from the column 'source'.
+
+    - 'source': subject ID and session ID joined by a dash
+    - 'source_id': subject ID in the raw dataset
+    - 'source_ses_id': Session ID in the raw dataset
+
+    Example
+    -------
+    source = "'C9ORF001-11'
+    source_id = 'C9ORF001'
+    source_ses_id = '11
+    """
+    from clinica.utils.filemanip import get_parent
+
+    return df.assign(
+        source_id=lambda x: x.source.apply(
+            lambda y: get_parent(y, 2).name.split("-")[0]
+        ),
+        source_ses_id=lambda x: x.source.apply(
+            lambda y: get_parent(y, 2).name.split("-")[1]
+        ),
+    )
+
+
+def _compute_genfi_version(df: DataFrame) -> DataFrame:
+    """Compute the genfi_version from the souce_ses_id column.
+
+    The column `source_ses_id` is casted to integer values.
+    """
+    return df.assign(
+        source_ses_id=lambda x: x.source_ses_id.astype("int"),
+        genfi_version=lambda x: x.source_ses_id.apply(lambda y: f"GENFI{len(str(y))}"),
+    )
+
+
+def _compute_baseline_and_session_numbers(df: DataFrame) -> DataFrame:
+    """Compute the baseline date and session numbers
+    and merge on 'source_id` and `source_ses_id`.
+    """
+    df_with_acq_date = _compute_baseline_date(df)
+    df_with_acq_date_and_session_numbers = _compute_session_numbers(df_with_acq_date)
+    return df.merge(
+        df_with_acq_date_and_session_numbers[["baseline", "session_id"]],
+        how="inner",
+        on=["source_id", "source_ses_id"],
+    )
+
+
+def _compute_baseline_date(df: DataFrame) -> DataFrame:
     """Computes the baseline date by taking the minimum
     acq_date for each subject.
 
     Parameters
     ----------
     df: Dataframe
 
@@ -271,16 +389,17 @@
         .groupby(["source_id", "source_ses_id"])
         .min()
     )
     df_2 = df[["source_id", "acq_date"]].groupby(["source_id"]).min()
     return df_1.join(df_2.rename(columns={"acq_date": "baseline"}))
 
 
-def compute_session_numbers(df: DataFrame) -> DataFrame:
-    """Computes the session IDs obtained from the number of months between an acquisition and the baseline acquisition.
+def _compute_session_numbers(df: DataFrame) -> DataFrame:
+    """Computes the session IDs obtained from the number of months between
+    an acquisition and the baseline acquisition.
 
     Parameters
     ----------
     df: DataFrame
         Dataframe containing the timestamp of the acquisition.
 
     Returns
@@ -296,27 +415,33 @@
         ses_month=lambda x: 12
         * (x.acq_date.apply(lambda y: y.year) - x.baseline.apply(lambda y: y.year))
         + (x.acq_date.apply(lambda y: y.month) - x.baseline.apply(lambda y: y.month)),
         session_id=lambda x: x.ses_month.map(lambda y: f"ses-M{y:03d}"),
     )
 
 
-def compute_modality(df: DataFrame) -> DataFrame:
+def _compute_participant_id(df: DataFrame) -> DataFrame:
+    """Compute the 'participant_id' column from the 'source_id' column."""
+    return df.assign(participant_id=lambda x: x.source_id.apply(lambda y: f"sub-{y}"))
+
+
+def _compute_modality(df: DataFrame) -> DataFrame:
     """Parses the series_desc column to identify the modality, and map
     this modality to a metadata dictionary.
 
     Parameters
     ----------
     df: Dataframe
         DataFrame on which to compute the modality.
 
     Returns
     -------
     Dataframe
-        Contains the datatype, suffix, sidecars and task that may be needed to form the complete file name.
+        Contains the datatype, suffix, sidecars and task that may be
+        needed to form the complete file name.
     """
     from clinica.iotools.bids_utils import identify_modality
 
     modality_mapping = {
         "T2w": {
             "datatype": "anat",
             "suffix": "T2w",
@@ -339,59 +464,82 @@
             ],
             "task": "",
         },
         "rsfmri": {
             "datatype": "func",
             "suffix": "bold",
             "sidecars": ["rsfmri.json"],
-            "task": "_task-rest",
+            "task": "task-rest",
         },
         "fieldmap": {
             "datatype": "fmap",
             "suffix": "fmap",
             "sidecars": ["fmap.json"],
             "task": "",
         },
     }
-    df = df.assign(
-        modality=lambda x: x.series_desc.apply(lambda y: identify_modality(y))
+    df = (
+        df.assign(
+            modality=lambda x: x.series_desc.apply(lambda y: identify_modality(y))
+        )
+        .dropna(subset=["modality"])
+        .drop_duplicates()
     )
     return df.join(df.modality.map(modality_mapping).apply(pd.Series))
 
 
-def identify_fieldmaps(df: DataFrame) -> DataFrame:
+def _compute_fieldmaps(df: DataFrame) -> DataFrame:
+    """Compute the fieldmaps. Please add details...
+    For example, why do we need to compute the dir_num before and after ?
+    """
+    from clinica.utils.filemanip import get_parent
+
+    df_with_dir_num = df.assign(
+        dir_num=lambda x: x.source.apply(
+            lambda y: int(get_parent(y).name.split("-")[0])
+        )
+    )
+    df_suf = _merge_fieldmaps(df_with_dir_num, _identify_fieldmaps(df_with_dir_num))
+    return df_suf
+
+
+def _identify_fieldmaps(df: DataFrame) -> DataFrame:
     """Identifies the fieldmaps imaging type: magnitude or phase difference.
 
     Parameters
     ----------
     df:Dataframe
         Dataframe without the fieldmaps identified.
 
     Returns
     -------
     Dataframe
         Dataframe with the fieldmaps identified
     """
-    filter = ["source_id", "source_ses_id", "modality", "dir_num", "suffix"]
-    df1 = df[filter][df["modality"].str.contains("fieldmap")].groupby(filter[:-1]).min()
+    column_filter = ["source_id", "source_ses_id", "modality", "dir_num", "suffix"]
+    df1 = (
+        df[column_filter][df["modality"].str.contains("fieldmap")]
+        .groupby(column_filter[:-1])
+        .min()
+    )
     df2 = (
-        df[filter[:-1]][df["modality"].str.contains("fieldmap")]
-        .groupby(filter[:-2])
+        df[column_filter[:-1]][df["modality"].str.contains("fieldmap")]
+        .groupby(column_filter[:-2])
         .min()
     )
     df1 = df1.join(df2.rename(columns={"dir_num": "run_01_dir_num"}))
     df_alt = df1.reset_index().assign(
         fmap_type_p=lambda x: (x.run_01_dir_num != x.dir_num)
     )
     return df_alt.assign(
         fmap=lambda x: x.fmap_type_p.apply(lambda y: "phasediff" if y else "magnitude")
     )
 
 
-def merge_fieldmaps(df: DataFrame, df_fmap: DataFrame) -> DataFrame:
+def _merge_fieldmaps(df: DataFrame, df_fmap: DataFrame) -> DataFrame:
     """Merges the dataframe containing the fieldmaps names
 
     Parameters
     ----------
     df: Dataframe
         Initial dataframe. Fieldmaps are identified on information extracted here.
 
@@ -399,136 +547,200 @@
         Dataframe in which fieldmaps are identified.
 
     Returns
     -------
     Dataframe
         Dataframe containing the correct fieldmap for each fieldmap acquisition.
     """
-    filter = ["source_id", "source_ses_id", "modality", "dir_num", "fmap"]
-    df1 = df.merge(df_fmap[filter], how="inner", on=filter[:-1])
-    df2 = df.merge(df_fmap[filter], how="left", on=filter[:-1])
+    column_filter = ["source_id", "source_ses_id", "modality", "dir_num", "fmap"]
+    df1 = df.merge(df_fmap[column_filter], how="inner", on=column_filter[:-1])
+    df2 = df.merge(df_fmap[column_filter], how="left", on=column_filter[:-1])
     df2 = df2[~df2["modality"].str.contains("fieldmap")]
     df1 = df1.assign(suffix=lambda x: x.fmap)
     return pd.concat([df2, df1], ignore_index=True)
 
 
-def compute_runs(df: DataFrame) -> DataFrame:
-    """This functions computes the run numbers.
+def _compute_runs(df: DataFrame) -> DataFrame:
+    """Compute the run numbers."""
+    df_with_number_of_parts = _compute_number_of_scan_parts(df)
+    df_with_run_numbers = _compute_run_numbers_from_parts(df_with_number_of_parts)
+    return df.merge(
+        df_with_run_numbers[
+            [
+                "source_id",
+                "source_ses_id",
+                "suffix",
+                "dir_num",
+                "run_num",
+                "number_of_parts",
+            ]
+        ],
+        how="left",
+        on=["source_id", "source_ses_id", "suffix", "dir_num"],
+    )
+
+
+def _compute_number_of_scan_parts(df: DataFrame) -> DataFrame:
+    """Compute the number of parts. Explain me please..."""
+    df_alt = _compute_philips_parts(df)
+    df_parts = df.merge(
+        df_alt[["source_id", "source_ses_id", "suffix", "dir_num", "number_of_parts"]],
+        how="left",
+        on=["source_id", "source_ses_id", "suffix", "dir_num"],
+    )
+    df_parts[["number_of_parts"]] = df_parts[["number_of_parts"]].fillna(value="1")
+    return df_parts
+
+
+def _compute_philips_parts(df: DataFrame) -> DataFrame:
+    """Compute the parts numbers for philips dwi acquisitions.
+
+    The amount of dwi acquisitions linked together is indicated.
+    For example, if a dwi acquisition is split in 9,
+    the `number_of_parts` column will have a value of 9 for all of these acquisitions.
+    Two columns are added:
+        - part_number, which contains the number for each part of a DTI acquisition.
+        - number_of_parts, which contains the amount of parts for each DTI acquisition.
 
     Parameters
     ----------
     df: DataFrame
         Dataframe without runs.
 
     Returns
     -------
     DataFrame
-        Dataframe containing the correct run for each acquisition.
+        Dataframe containing the correct dwi part number for each acquisition. It also contains
+        the total amount of dwi parts for each subjects-session.
     """
-    filter = ["source_id", "source_ses_id", "suffix", "dir_num"]
-    df1 = df[filter].groupby(filter).min()
-    df2 = df[filter].groupby(filter[:-1]).min()
-    df1 = df1.join(df2.rename(columns={"dir_num": "run_01_dir_num"}))
-    df_alt = df1.reset_index().assign(run=lambda x: (x.run_01_dir_num != x.dir_num))
-    return df_alt.assign(run_num=lambda df: df.run.apply(lambda x: f"run-0{int(x)+1}"))
-
+    df_with_duplicate_flags = _find_duplicate_run(df)
+    df_with_part_numbers = _compute_part_numbers(df_with_duplicate_flags)
+    df_with_number_of_parts = _compute_number_of_parts(df_with_part_numbers)
+    return pd.concat(
+        [df_with_part_numbers, df_with_number_of_parts["number_of_parts"]], axis=1
+    )
 
-def get_parent(path: str, n: int = 1) -> Path:
-    """Get the path to the nth parent.
 
-    Parameters
-    ----------
-    path: str
-        path to a file.
-    n: int
-        depth we want to go up in the parents.
+def _find_duplicate_run(df: DataFrame) -> DataFrame:
+    """Create a column that contains the information of whether a run is a duplicate or not."""
+    column_filter = ["source_id", "source_ses_id", "suffix", "dir_num"]
+    df = df[df["suffix"].str.contains("dwi", case=False)]
+    df1 = df[column_filter].groupby(column_filter).min()
+    df2 = df[column_filter].groupby(column_filter[:-1]).min()
+    df1 = df1.join(df2.rename(columns={"dir_num": "part_01_dir_num"}))
+    return df1.reset_index().assign(run=lambda x: (x.part_01_dir_num != x.dir_num))
+
+
+def _compute_part_numbers(df: DataFrame) -> DataFrame:
+    """Compute the sequence number of each part."""
+    return pd.concat(
+        [
+            df,
+            pd.DataFrame(
+                _compute_scan_sequence_numbers(df.run.tolist()), columns=["part_number"]
+            ),
+        ],
+        axis=1,
+    )
 
-    Returns
-    -------
-    Path
-        Path to a parent directory.
 
-    Examples
-    --------
-    >>> get_parent('/path/to/a/file', 2)
-    /path/to
-    """
-    if n <= 0:
-        return Path(path)
-    return get_parent(Path(path).parent, n - 1)
+def _compute_number_of_parts(df: pd.DataFrame) -> DataFrame:
+    """Add the number of parts (the max value of the part_number column) to each part."""
+    column_filter = ["source_id", "source_ses_id", "suffix", "part_number"]
+    df_parts_1 = df[column_filter].groupby(column_filter).max()
+    df_parts_2 = df[column_filter].groupby(column_filter[:-1]).max()
+    return df_parts_1.join(
+        df_parts_2.rename(columns={"part_number": "number_of_parts"})
+    ).reset_index()
 
 
-def merge_imaging_data(df_dicom: DataFrame) -> DataFrame:
-    """This function uses the raw information extracted from the images,
-    to obtain all the information necessary for the BIDS conversion.
+def _compute_run_numbers_from_parts(df: DataFrame) -> DataFrame:
+    """This functions computes the run numbers.
 
     Parameters
     ----------
-    df_dicom: DataFrame
-        Dataframe containing the data extracted from the images
+    df: DataFrame
+        Dataframe without runs.
 
     Returns
     -------
-    df_sub_ses_run: DataFrame
-        Dataframe with the data necessary for the BIDS
+    DataFrame
+        Dataframe containing the correct run for each acquisition.
     """
-
-    df_dicom = df_dicom.assign(
-        source_id=lambda df: df.source.apply(
-            lambda x: get_parent(x, 2).name.split("-")[0]
-        ),
-        source_ses_id=lambda df: df.source.apply(
-            lambda x: get_parent(x, 2).name.split("-")[1]
-        ),
-        origin=lambda df: df.source.apply(lambda x: get_parent(x, 4)),
-    )
-
-    df_dicom = df_dicom.reset_index()
-
-    df_dicom = df_dicom.assign(
-        source_ses_id=lambda df: df.source_ses_id.astype("int"),
-        genfi_version=lambda df: df.source_ses_id.apply(
-            lambda x: f"GENFI{len(str(x))}"
-        ),
+    column_filter = [
+        "source_id",
+        "source_ses_id",
+        "suffix",
+        "number_of_parts",
+        "dir_num",
+    ]
+    df1 = df[column_filter].groupby(column_filter).min()
+    df2 = df[column_filter].groupby(column_filter[:-1]).min()
+    df1 = df1.join(df2.rename(columns={"dir_num": "run_01_dir_num"}))
+    df_alt = df1.reset_index().assign(run=lambda x: (x.run_01_dir_num != x.dir_num))
+    df_run = pd.concat(
+        [
+            df_alt,
+            pd.DataFrame(
+                _compute_scan_sequence_numbers(df_alt.run.tolist()),
+                columns=["run_number"],
+            ),
+        ],
+        axis=1,
     )
-    df_1 = compute_baseline_date(df_dicom)
+    return df_run.assign(run_num=lambda x: x.run_number.apply(lambda y: f"run-{y:02d}"))
 
-    df_1 = compute_session_numbers(df_1)
 
-    df_sub_ses = df_dicom.merge(
-        df_1[["baseline", "session_id"]], how="inner", on=["source_id", "source_ses_id"]
-    )
-    df_sub_ses = df_sub_ses.assign(
-        participant_id=lambda df: df.source_id.apply(lambda x: f"sub-{x}")
-    )
-    df_sub_ses = compute_modality(df_sub_ses)
+def _compute_scan_sequence_numbers(duplicate_flags: Iterable[bool]) -> List[int]:
+    """Return the run number from an iterable of booleans indicating
+    whether each scan is a duplicate or not.
 
-    df_fmap = df_sub_ses.assign(
-        dir_num=lambda x: x.source.apply(lambda y: int(get_parent(y).name))
-    )
+    Parameters
+    ---------
+    duplicate_flags : Iterable[bool]
+        If the element at index k is True, then the scan k is a duplicate.
+        Otherwise, it is the first scan of the sequence.
 
-    df_suf = merge_fieldmaps(df_fmap, identify_fieldmaps(df_fmap))
+    Returns
+    ------
+    ses_numbers : List[int]
+        The list of scan sequence numbers.
 
-    df_suf_dir = df_suf.assign(
-        dir_num=lambda x: x.source.apply(lambda y: int(get_parent(y).name))
+    Examples
+    ---------
+    >>> _compute_scan_sequence_numbers([False, True, False, True, False, False, False, True, False, True, True])
+    [1, 2, 1, 2, 1, 1, 1, 2, 1, 2, 3]
+
+    Raises
+    -----
+    ValueError :
+        If the input list is empty.
+    """
+    if len(duplicate_flags) == 0:
+        raise ValueError("Provided list is empty.")
+    ses_numbers = [1]
+    for k in range(1, len(duplicate_flags)):
+        ses_numbers.append(1 if not duplicate_flags[k] else ses_numbers[k - 1] + 1)
+    return ses_numbers
+
+
+def _compute_bids_full_path(df: DataFrame) -> DataFrame:
+    """Compute the BIDS full path."""
+    df_with_bids_filename = df.assign(
+        bids_filename=lambda x: x[
+            ["participant_id", "session_id", "task", "run_num", "suffix"]
+        ].agg("_".join, axis=1),
     )
-    df_alt = compute_runs(df_suf_dir)
-    df_sub_ses_run = df_suf_dir.merge(
-        df_alt[["source_id", "source_ses_id", "suffix", "dir_num", "run_num"]],
-        how="left",
-        on=["source_id", "source_ses_id", "suffix", "dir_num"],
+    df_with_bids_filename = df_with_bids_filename.assign(
+        bids_filename=lambda x: x.bids_filename.apply(lambda y: y.replace("__", "_"))
     )
-
-    return df_sub_ses_run.assign(
-        bids_filename=lambda df: df[
-            ["participant_id", "session_id", "run_num", "suffix"]
-        ].agg("_".join, axis=1),
-        bids_full_path=lambda df: df[
+    return df_with_bids_filename.assign(
+        bids_full_path=lambda x: x[
             ["participant_id", "session_id", "datatype", "bids_filename"]
-        ].agg("/".join, axis=1),
+        ].agg("/".join, axis=1)
     )
 
 
 def write_bids(
     to: PathLike,
     participants: DataFrame,
     sessions: DataFrame,
@@ -553,52 +765,96 @@
     import os
     from pathlib import Path
 
     from fsspec.implementations.local import LocalFileSystem
 
     from clinica.iotools.bids_dataset_description import BIDSDatasetDescription
     from clinica.iotools.bids_utils import run_dcm2niix, write_to_tsv
+    from clinica.utils.stream import cprint
 
+    cprint("Starting to write the BIDS.", lvl="info")
     to = Path(to)
     fs = LocalFileSystem(auto_mkdir=True)
-
     # Ensure BIDS hierarchy is written first.
+
+    participants = (
+        participants.reset_index()
+        .drop(["session_id", "modality", "run_num", "bids_filename", "source"], axis=1)
+        .drop_duplicates()
+        .set_index("participant_id")
+    )
     with fs.transaction:
         with fs.open(
             str(to / "dataset_description.json"), "w"
         ) as dataset_description_file:
             BIDSDatasetDescription(name="GENFI").write(to=dataset_description_file)
         with fs.open(str(to / "participants.tsv"), "w") as participant_file:
             write_to_tsv(participants, participant_file)
 
     for participant_id, data_frame in sessions.groupby(["participant_id"]):
         sessions = data_frame.droplevel(
-            ["participant_id", "modality", "bids_filename"]
+            ["participant_id", "modality", "bids_filename", "run_num"]
         ).drop_duplicates()
 
         sessions_filepath = to / str(participant_id) / f"{participant_id}_sessions.tsv"
         with fs.open(str(sessions_filepath), "w") as sessions_file:
             write_to_tsv(sessions, sessions_file)
     scans = scans.reset_index().set_index(["bids_full_path"], verify_integrity=True)
-
     for bids_full_path, metadata in scans.iterrows():
         try:
             os.makedirs(to / (Path(bids_full_path).parent))
         except OSError:
             pass
-        run_dcm2niix(
+        dcm2niix_success = run_dcm2niix(
             Path(metadata["source_path"]).parent,
             to / str(Path(bids_full_path).parent),
             metadata["bids_filename"],
             True,
         )
+        if dcm2niix_success:
+            scans_filepath = (
+                to
+                / str(metadata.participant_id)
+                / str(metadata.session_id)
+                / f"{metadata.participant_id}_{metadata.session_id}_scan.tsv"
+            )
+            row_to_write = _serialize_row(
+                metadata.drop(["participant_id", "session_id"]),
+                write_column_names=not scans_filepath.exists(),
+            )
+            with open(scans_filepath, "a") as scans_file:
+                scans_file.write(f"{row_to_write}\n")
+            if (
+                "dwi" in metadata["bids_filename"]
+                and "Philips" in metadata.manufacturer
+            ):
+                merge_philips_diffusion(
+                    to / Path(bids_full_path).with_suffix(".json"),
+                    metadata.number_of_parts,
+                    metadata.run_num,
+                )
     correct_fieldmaps_name(to)
+    delete_real_and_imaginary_files(to)
     return
 
 
+def _serialize_row(row: pd.Series, write_column_names: bool) -> str:
+    row_dict = row.to_dict()
+    to_write = (
+        [row_dict.keys(), row_dict.values()]
+        if write_column_names
+        else [row_dict.values()]
+    )
+    return "\n".join([_serialize_list(list(_)) for _ in to_write])
+
+
+def _serialize_list(data: list, sep="\t") -> str:
+    return sep.join([str(value) for value in data])
+
+
 def correct_fieldmaps_name(to: PathLike) -> None:
     """This function scans the BIDS after it has been written to correct the nameds of the fieldmap files.
 
     Parameters
     ----------
     to: PathLike
         Path to the BIDS
@@ -645,7 +901,93 @@
     import re
 
     for z in Path(to).rglob("*magnitude_e*"):
         os.rename(z, z.parent / re.sub(r"magnitude_e", "magnitude", z.name))
 
     for z in Path(to).rglob("*phasediff_e*_ph*"):
         os.rename(z, z.parent / re.sub(r"phasediff_e[1-9]_ph", "phasediff", z.name))
+
+
+def merge_philips_diffusion(
+    json_file: PathLike,
+    number_of_parts: float,
+    run_num: str,
+) -> None:
+    """Add the dwi number in the provided JSON file for each run of Philips images.
+    The 'MultipartID' field of the input JSON file is set to 'dwi_1' or 'dwi_2' depending
+    on the run number.
+    """
+    import json
+
+    from clinica.utils.stream import cprint
+
+    multipart_id = _get_multipart_id(
+        PhilipsNumberOfParts.from_int(int(number_of_parts)), run_num
+    )
+    try:
+        with open(json_file, "r+") as f:
+            if multipart_id is not None:
+                data = json.load(f)
+                data["MultipartID"] = multipart_id
+                json.dump(data, f, indent=4)
+    except FileNotFoundError:
+        cprint(msg=f"the file {json_file} does not exist.", lvl="warning")
+
+
+class PhilipsNumberOfParts(Enum):
+    """DWI scans obtained with a Philips scanner might have
+    been divided in either 5 or 9 parts. This distinction is important
+    because we will link these different parts together.
+    If the number of parts is not 5 or 9, nothing will be done.
+    """
+
+    FIVE = 5
+    NINE = 9
+    OTHER = None
+
+    @classmethod
+    def from_int(cls, nb_parts: int):
+        import warnings
+
+        for member in cls:
+            if member.value == nb_parts:
+                return member
+        warnings.warn(
+            f"Unexpected number of splits {nb_parts}. "
+            f"Should be one of {[c.value for c in cls]}."
+        )
+        return cls.OTHER
+
+
+def _get_multipart_id(nb_parts: PhilipsNumberOfParts, run_num: str) -> Optional[str]:
+    """Return the MultiPartID for the provided run number depending on the number of parts."""
+    if nb_parts == PhilipsNumberOfParts.NINE:
+        if run_num in (f"run-0{k}" for k in range(1, 5)):
+            return "dwi_2"
+        if run_num in (f"run-0{k}" for k in range(5, 10)):
+            return "dwi_1"
+        raise ValueError(f"{run_num} is outside of the scope.")
+    if nb_parts == PhilipsNumberOfParts.FIVE:
+        if run_num in (f"run-0{k}" for k in range(1, 6)):
+            return "dwi_1"
+        raise ValueError(f"{run_num} is outside of the scope.")
+    if nb_parts == PhilipsNumberOfParts.OTHER:
+        return None
+
+
+def delete_real_and_imaginary_files(bids_folder: PathLike) -> None:
+    """Delete all files with a `_real` or `_imaginary` suffix from the BIDS folder.
+    These files are generated by dcm2niix when it is not able to correctly convert the full image.
+    These files break the BIDS specification, and are therefore removed.
+
+    Parameters
+    ----------
+    bids_folder : PathLike
+        Path to the BIDS folder.
+    """
+    from clinica.utils.stream import cprint
+
+    bids_folder = Path(bids_folder)
+    for file_type in ("real", "imaginary"):
+        for f in bids_folder.rglob(f"*_{file_type}.*"):
+            f.unlink()
+            cprint(f"file {f} was deleted as it is not BIDS compliant.")
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/habs_to_bids/habs_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/habs_to_bids/habs_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/nifd_to_bids/nifd_utils.py` & `clinica-0.7.5/clinica/iotools/converters/nifd_to_bids/nifd_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from os import PathLike
-from typing import BinaryIO, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Dict, Iterable, List, Optional, Tuple
 
 from pandas import DataFrame
+from pandas.api.types import is_string_dtype
 
 
 def find_clinical_data(clinical_data_directory: PathLike) -> Optional[DataFrame]:
     from pathlib import Path
 
     from pandas import read_excel
 
@@ -240,21 +241,29 @@
     )
 
     # Compute the BIDS-compliant participant, session and scan IDs.
     scans = scans.assign(
         participant_id=lambda df: df.subject.apply(
             lambda x: f"sub-NIFD{x.replace('_', '')}"
         ),
-        session_id=lambda df: df.visit.apply(lambda x: f"ses-M{(6 * (x - 1)):03d}"),
+        session_id=lambda df: df.visit.apply(
+            lambda x: (
+                "ses-M" + x.strip("M").zfill(3)
+                if is_string_dtype(x)
+                else f"ses-M{(6 * (x - 1)):03d}"
+            )
+        ),
         filename=lambda df: df.apply(
-            lambda x: f"{x.participant_id}/{x.session_id}/{x.datatype}/"
-            f"{x.participant_id}_{x.session_id}"
-            f"{'_trc-' + x.trc_label if x.trc_label else ''}"
-            f"{'_rec-' + x.rec_label if x.rec_label else ''}"
-            f"_{x.suffix}.nii.gz",
+            lambda x: (
+                f"{x.participant_id}/{x.session_id}/{x.datatype}/"
+                f"{x.participant_id}_{x.session_id}"
+                f"{'_trc-' + x.trc_label if x.trc_label else ''}"
+                f"{'_rec-' + x.rec_label if x.rec_label else ''}"
+                f"_{x.suffix}.nii.gz"
+            ),
             axis=1,
         ),
     )
 
     # Prepare subjects manifest.
     subjects = (
         scans[["participant_id", "session_id", "group", "sex", "age"]]
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,14 @@
     Convert the imaging and clinical data of OASIS3 (https://www.oasis-brains.org), located in DATASET_DIRECTORY and
     CLINICAL_DATA_DIRECTORY respectively, to a BIDS dataset in the target BIDS_DIRECTORY.
     """
     from clinica.iotools.converters.oasis3_to_bids.oasis3_to_bids import convert_images
     from clinica.utils.check_dependency import check_dcm2niix
     from clinica.utils.stream import cprint
 
-    check_dcm2niix()
-
     convert_images(dataset_directory, bids_directory, clinical_data_directory)
 
     cprint("Conversion to BIDS succeeded.")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py` & `clinica-0.7.5/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,36 +73,64 @@
     source_path_series = pd.Series(
         find_imaging_data(imaging_data_directory), name="source_path"
     )
 
     source_dir_series = source_path_series.apply(lambda x: Path(str(x)).parent).rename(
         "source_dir"
     )
-
     file_spec_series = source_path_series.apply(lambda x: Path(str(x)).parts[0]).rename(
         "path"
     )
-
+    source_file_series = source_path_series.apply(
+        lambda x: identify_modality(str(x))
+    ).rename("modality")
+    source_run_series = source_path_series.apply(
+        lambda x: identify_runs(str(x))
+    ).rename("run_number")
     df_source = pd.concat(
         [
             source_path_series,
             file_spec_series,
             source_dir_series,
             file_spec_series.str.split("_", expand=True),
+            source_file_series,
+            source_run_series,
         ],
         axis=1,
     )
-    df_source = df_source.rename(
-        {0: "Subject", 1: "modality", 2: "Date"}, axis="columns"
-    ).drop_duplicates()
-
+    df_source = (
+        df_source.rename({0: "Subject", 1: "modality_2", 2: "Date"}, axis="columns")
+        .drop_duplicates()
+        .sort_values(by=["source_path"])
+    )
     df_source = df_source.assign(participant_id=lambda df: "sub-" + df.Subject)
+    df_source["modality"] = df_source[["modality", "modality_2"]].apply(
+        "_".join, axis=1
+    )
     return df_source
 
 
+def identify_modality(source_path: str) -> str:
+    from pathlib import Path
+
+    try:
+        return (Path(source_path).name).split(".")[0].split("_")[-1]
+    except:
+        return "nan"
+
+
+def identify_runs(source_path: str) -> str:
+    import re
+
+    try:
+        return re.search(r"run-\d+", source_path)[0]
+    except:
+        return "run-01"
+
+
 def find_imaging_data(path_to_source_data: PathLike) -> Iterable[PathLike]:
     from pathlib import Path
 
     for path in Path(path_to_source_data).rglob("*.nii.gz"):
         yield str(path.relative_to(path_to_source_data))
 
 
@@ -143,37 +171,44 @@
             lambda x: f"ses-M{ (5-(len(str(x)))) * '0' + str(int(x))}"
         )
     )
 
     df_source = df_source.join(
         df_source.modality.map(
             {
-                "MR": {"datatype": "anat", "suffix": "T1w"},
-                "FDG": {"datatype": "pet", "suffix": "pet", "trc_label": "18FFDG"},
-                "PIB": {"datatype": "pet", "suffix": "pet", "trc_label": "11CPIB"},
-                "AV45": {"datatype": "pet", "suffix": "pet", "trc_label": "18FAV45"},
+                "dwi_MR": {"datatype": "dwi", "suffix": "dwi"},
+                "T1w_MR": {"datatype": "anat", "suffix": "T1w"},
+                "T2star_MR": {"datatype": "anat", "suffix": "T2starw"},
+                "FLAIR_MR": {"datatype": "anat", "suffix": "FLAIR"},
+                "pet_FDG": {"datatype": "pet", "suffix": "pet", "trc_label": "18FFDG"},
+                "pet_PIB": {"datatype": "pet", "suffix": "pet", "trc_label": "11CPIB"},
+                "pet_AV45": {
+                    "datatype": "pet",
+                    "suffix": "pet",
+                    "trc_label": "18FAV45",
+                },
             }
         ).apply(pd.Series)
     )
     if "trc_label" in df_source.columns:
         df_source = df_source.assign(
             filename=lambda df: df.apply(
                 lambda x: f"{x.participant_id}/{x.ses}/{x.datatype}/"
                 f"{x.participant_id}_{x.ses}"
                 f"{'_trc-'+x.trc_label if pd.notna(x.trc_label) else ''}"
-                f"_{x.suffix}.nii.gz",
+                f"_{x.run_number}_{x.suffix}.nii.gz",
                 axis=1,
             )
         )
     else:
         df_source = df_source.assign(
             filename=lambda df: df.apply(
                 lambda x: f"{x.participant_id}/{x.ses}/{x.datatype}/"
                 f"{x.participant_id}_{x.ses}"
-                f"_{x.suffix}.nii.gz",
+                f"_{x.run_number}_{x.suffix}.nii.gz",
                 axis=1,
             )
         )
     df_adrc = df_adrc.merge(df_source["Subject"], how="inner", on="Subject")
     df_adrc = df_adrc.assign(
         session=lambda df: round(df["session_id"].str[1:].astype("int") / (364.25 / 2))
         * 6
@@ -317,9 +352,15 @@
             sessions_filepath = to / participant_id / f"{participant_id}_sessions.tsv"
             with fs.open(sessions_filepath, "w") as sessions_file:
                 write_to_tsv(sessions_group, sessions_file)
 
     # Perform import of imaging data next.
     for filename, metadata in scans.iterrows():
         path = Path(dataset_directory) / metadata.source_dir
-        install_bids(sourcedata_dir=path, bids_filename=to / filename)
+        if extract_suffix_from_filename(str(filename)) != "nan":
+            install_bids(sourcedata_dir=path, bids_filename=to / filename)
     return scans.index.to_list()
+
+
+def extract_suffix_from_filename(filename: str) -> str:
+
+    return filename.split("_")[-1].split(".")[0]
```

### Comparing `clinica-0.7.4/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py` & `clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py` & `clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/converters/ukb_to_bids/ukb_utils.py` & `clinica-0.7.5/clinica/iotools/converters/ukb_to_bids/ukb_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/data/clinical_specifications_adni_participant.tsv` & `clinica-0.7.5/clinica/iotools/data/clinical_specifications_adni_participant.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/data/clinical_specifications_adni_sessions.tsv` & `clinica-0.7.5/clinica/iotools/data/clinical_specifications_adni_sessions.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/data/clinical_specifications_participant.tsv` & `clinica-0.7.5/clinica/iotools/data/clinical_specifications_participant.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/data/clinical_specifications_scans.tsv` & `clinica-0.7.5/clinica/iotools/data/clinical_specifications_scans.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/data/clinical_specifications_sessions.tsv` & `clinica-0.7.5/clinica/iotools/data/clinical_specifications_sessions.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/data/genfi_ref.csv` & `clinica-0.7.5/clinica/iotools/data/genfi_ref.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 participants;sessions;scans
 participant_id;participant_id;participant_id
 source;session_id;session_id
 gender;genfi_version;bids_filename
 handedness;age_at_visit;bids_full_path
 education;date_of_scan;source_path
-genetic_group;diagnosis;
-genetic_status_1;ftld-cdr-global;
-genetic_status_2;cdr-sob;
+genetic_group;diagnosis;manufacturer
+genetic_status_1;ftld-cdr-global;run_num
+genetic_status_2;cdr-sob;number_of_parts
 ;non-brain_outer_tissue_-_background;
 ;non-brain_low;
 ;non-brain_mid;
 ;non-brain_high;
 ;non-ventricular_csf;
 ;3rd_ventricle;
 ;4th_ventricle_;
```

### Comparing `clinica-0.7.4/clinica/iotools/utils/cli.py` & `clinica-0.7.5/clinica/iotools/utils/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/utils/data_handling.py` & `clinica-0.7.5/clinica/iotools/utils/data_handling.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/iotools/utils/pipeline_handling.py` & `clinica-0.7.5/clinica/iotools/utils/pipeline_handling.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/image.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/image.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@random/random.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@random/random.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/image.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/image.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/@term/term.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/@term/term.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/gl.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/gl.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/redmod.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/redmod.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/spectral.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/spectral.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/SurfStat/var2fac.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/SurfStat/var2fac.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/lib/clinicasurfstat/clinicasurfstat.m` & `clinica-0.7.5/clinica/lib/clinicasurfstat/clinicasurfstat.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/__init__.py` & `clinica-0.7.5/clinica/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/cli_param/argument.py` & `clinica-0.7.5/clinica/pipelines/cli_param/argument.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/cli_param/option.py` & `clinica-0.7.5/clinica/pipelines/cli_param/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,20 @@
     help=(
         "TSV file containing for each PET image its point spread function (PSF) measured "
         "in mm at x, y & z coordinates. Columns must contain: "
         "participant_id, session_id, acq_label, psf_x, psf_y and psf_z."
     ),
 )
 
+random_seed = option(
+    "--random_seed",
+    type=int,
+    help="Specify the random seed for algorithms that support it.",
+)
+
 save_warped_modulated = option(
     "-swm",
     "--save_warped_modulated",
     is_flag=True,
     help="Save warped modulated images for tissues specified in --tissue_classes flag.",
 )
 
@@ -182,13 +188,14 @@
 atlas_path = option(
     "-ap",
     "--atlas_path",
     type=click.Path(exists=True, dir_okay=True, resolve_path=True),
     help="Compute atlases at the end of the path",
 )
 
+# This option is only implemented in dwi_preprocessing_using_t1 for now.
 delete_cache = option(
     "-dc",
     "--delete_cache",
     is_flag=True,
-    help="If True, large intermediary files will be deleted before the end of the pipeline.",  # This option is only implemented in dwi_preprocessing_using_t1 for now.
+    help="If True, large intermediary files will be deleted before the end of the pipeline.",
 )
```

### Comparing `clinica-0.7.4/clinica/pipelines/cli_param/option_group.py` & `clinica-0.7.5/clinica/pipelines/cli_param/option_group.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py` & `clinica-0.7.5/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_connectome/dwi_connectome_cli.py` & `clinica-0.7.5/clinica/pipelines/dwi_connectome/dwi_connectome_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_connectome/dwi_connectome_pipeline.py` & `clinica-0.7.5/clinica/pipelines/dwi_connectome/dwi_connectome_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_connectome/dwi_connectome_utils.py` & `clinica-0.7.5/clinica/pipelines/dwi_connectome/dwi_connectome_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_connectome/info.json` & `clinica-0.7.5/clinica/pipelines/dwi_connectome/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_dti/dwi_dti_cli.py` & `clinica-0.7.5/clinica/pipelines/dwi_dti/dwi_dti_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_dti/dwi_dti_pipeline.py` & `clinica-0.7.5/clinica/pipelines/dwi_dti/dwi_dti_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_dti/dwi_dti_utils.py` & `clinica-0.7.5/clinica/pipelines/dwi_dti/dwi_dti_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_dti/info.json` & `clinica-0.7.5/clinica/pipelines/dwi_dti/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_cli.py` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_pipeline.py` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -272,15 +272,14 @@
                                                    ("out_caps_smoothed_fmap", "preprocessing.@smoothed_fmap")]),
             ]
         )
         # fmt: on
 
     def build_core_nodes(self):
         """Build and connect the core nodes of the pipeline."""
-        import nipype.interfaces.ants as ants
         import nipype.interfaces.fsl as fsl
         import nipype.interfaces.mrtrix3 as mrtrix3
         import nipype.interfaces.utility as nutil
         import nipype.interfaces.utility as niu
         import nipype.pipeline.engine as npe
 
         from clinica.pipelines.dwi_preprocessing_using_t1.dwi_preprocessing_using_t1_workflows import (
@@ -289,21 +288,18 @@
         from clinica.utils.dwi import compute_average_b0
 
         from .dwi_preprocessing_using_phasediff_fmap_utils import (
             init_input_node,
             print_end_pipeline,
         )
         from .dwi_preprocessing_using_phasediff_fmap_workflows import (
+            calibrate_and_register_fmap,
             compute_reference_b0,
-            prepare_phasediff_fmap,
         )
 
-        # Step 0: Initialization
-        # ======================
-        # Initialize input parameters and print begin message
         init_node = npe.Node(
             interface=nutil.Function(
                 input_names=self.get_input_fields(),
                 output_names=[
                     "image_id",
                     "dwi",
                     "bvec",
@@ -320,54 +316,24 @@
         )
 
         reference_b0 = compute_reference_b0(
             b_value_threshold=self.parameters["low_bval"],
             use_cuda=self.parameters["use_cuda"],
             initrand=self.parameters["initrand"],
         )
-
-        # Step 2: Calibrate and register FMap
-        # ===================================
-        # Bias field correction of the magnitude image
-        bias_mag_fmap = npe.Node(
-            ants.N4BiasFieldCorrection(dimension=3), name="2a-N4MagnitudeFmap"
-        )
-        # Brain extraction of the magnitude image
-        bet_mag_fmap = npe.Node(
-            fsl.BET(frac=0.4, mask=True), name="2b-BetN4MagnitudeFmap"
-        )
-
-        # Calibrate FMap
-        calibrate_fmap = prepare_phasediff_fmap(name="2c-CalibrateFMap")
-
-        # Register the BET magnitude fmap onto the BET b0
-        bet_mag_fmap2b0 = npe.Node(
-            interface=fsl.FLIRT(), name="2d-RegistrationBetMagToB0"
-        )
-        bet_mag_fmap2b0.inputs.dof = 6
-        bet_mag_fmap2b0.inputs.output_type = "NIFTI_GZ"
-
-        # Apply the transformation on the calibrated fmap
-        fmap2b0 = npe.Node(interface=fsl.ApplyXFM(), name="2e-1-FMapToB0")
-        fmap2b0.inputs.output_type = "NIFTI_GZ"
-
-        # Apply the transformation on the magnitude image
-        mag_fmap2b0 = fmap2b0.clone("2e-2-MagFMapToB0")
-
-        # Smooth the registered (calibrated) fmap
-        smoothing = npe.Node(interface=fsl.maths.IsotropicSmooth(), name="2f-Smoothing")
-        smoothing.inputs.sigma = 4.0
+        fmap_calibration_and_registration = calibrate_and_register_fmap()
 
         # Step 3: Run FSL eddy
         # ====================
         eddy = eddy_fsl_pipeline(
             use_cuda=self.parameters["use_cuda"],
             initrand=self.parameters["initrand"],
             image_id=True,
             field=True,
+            compute_mask=False,
         )
 
         # Step 4: Bias correction
         # =======================
         # Use implementation detailed in (Jeurissen et al., 2014)
         bias = npe.Node(mrtrix3.DWIBiasCorrect(use_ants=True), name="4-RemoveBias")
 
@@ -391,92 +357,116 @@
         print_end_message = npe.Node(
             interface=nutil.Function(
                 input_names=["image_id", "final_file"], function=print_end_pipeline
             ),
             name="99-WriteEndMessage",
         )
 
-        # Connection
-        # ==========
-        # fmt: off
-        self.connect(
-            [
-                # Step 0: Initialization
-                # ======================
-                # Initialize input parameters and print begin message
-                (self.input_node, init_node, [("dwi", "dwi"),
-                                              ("bvec", "bvec"),
-                                              ("bval", "bval"),
-                                              ("dwi_json", "dwi_json"),
-                                              ("fmap_magnitude", "fmap_magnitude"),
-                                              ("fmap_phasediff", "fmap_phasediff"),
-                                              ("fmap_phasediff_json", "fmap_phasediff_json")]),
-                # Step 1: Computation of the reference b0 (i.e. average b0 but with EPI distortions)
-                # =======================================
-                (init_node, reference_b0, [("bval", "inputnode.b_values_filename"),
-                                           ("bvec", "inputnode.b_vectors_filename"),
-                                           ("dwi", "inputnode.dwi_filename"),
-                                           ("total_readout_time", "inputnode.total_readout_time"),
-                                           ("phase_encoding_direction", "inputnode.phase_encoding_direction"),
-                                           ("image_id", "inputnode.image_id")]),
-                # Step 2: Calibrate and register FMap
-                # ===================================
-                # Bias field correction of the magnitude image
-                (init_node, bias_mag_fmap, [("fmap_magnitude", "input_image")]),
-                # Brain extraction of the magnitude image
-                (bias_mag_fmap, bet_mag_fmap, [("output_image", "in_file")]),
-                # Calibration of the FMap
-                (bet_mag_fmap, calibrate_fmap, [("mask_file", "input_node.fmap_mask"),
-                                                ("out_file", "input_node.fmap_magnitude")]),
-                (init_node, calibrate_fmap, [("fmap_phasediff", "input_node.fmap_phasediff"),
-                                             ("delta_echo_time", "input_node.delta_echo_time")]),
-                # Register the BET magnitude fmap onto the BET b0
-                (bet_mag_fmap, bet_mag_fmap2b0, [("out_file", "in_file")]),
-                (reference_b0, bet_mag_fmap2b0, [("outputnode.reference_b0", "reference")]),
-                # Apply the transformation on the magnitude image
-                (bet_mag_fmap2b0, mag_fmap2b0, [("out_matrix_file", "in_matrix_file")]),
-                (bias_mag_fmap, mag_fmap2b0, [("output_image", "in_file")]),
-                (reference_b0, mag_fmap2b0, [("outputnode.reference_b0", "reference")]),
-                # Apply the transformation on the calibrated fmap
-                (bet_mag_fmap2b0, fmap2b0, [("out_matrix_file", "in_matrix_file")]),
-                (calibrate_fmap, fmap2b0, [("output_node.calibrated_fmap", "in_file")]),
-                (reference_b0, fmap2b0, [("outputnode.reference_b0", "reference")]),
-                # # Smooth the registered (calibrated) fmap
-                (fmap2b0, smoothing, [("out_file", "in_file")]),
-
-                # Step 3: Run FSL eddy
-                # ====================
-                (init_node, eddy, [("dwi", "inputnode.dwi_filename"),
-                                   ("bval", "inputnode.b_values_filename"),
-                                   ("bvec", "inputnode.b_vectors_filename"),
-                                   ("image_id", "inputnode.image_id")]),
-                (smoothing, eddy, [("out_file", "inputnode.field")]),
-                (reference_b0, eddy, [("outputnode.brainmask", "inputnode.in_mask")]),
-
-                # Step 4: Bias correction
-                # =======================
-                (init_node, bias, [("bval", "in_bval")]),
-                (eddy, bias, [("outputnode.out_rotated_bvecs", "in_bvec"),
-                              ("outputnode.out_corrected", "in_file")]),
-                # Step 5: Final brainmask
-                # =======================
-                # Compute average b0 on corrected dataset (for brain mask extraction)
-                (init_node, compute_avg_b0, [("bval", "in_bval")]),
-                (bias, compute_avg_b0, [("out_file", "in_dwi")]),
-                # Compute b0 mask on corrected avg b0
-                (compute_avg_b0, mask_avg_b0, [("reference_b0", "in_file")]),
-
-                # Print end message
-                (init_node, print_end_message, [("image_id", "image_id")]),
-                (mask_avg_b0, print_end_message, [("mask_file", "final_file")]),
-
-                # Output node
-                (init_node, self.output_node, [("bval", "preproc_bval")]),
-                (eddy, self.output_node, [("outputnode.out_rotated_bvecs", "preproc_bvec")]),
-                (bias, self.output_node, [("out_file", "preproc_dwi")]),
-                (mask_avg_b0, self.output_node, [("mask_file", "b0_mask")]),
-                (bet_mag_fmap2b0, self.output_node, [("out_file", "magnitude_on_b0")]),
-                (fmap2b0, self.output_node, [("out_file", "calibrated_fmap_on_b0")]),
-                (smoothing, self.output_node, [("out_file", "smoothed_fmap_on_b0")]),
-            ]
-        )
-        # fmt: on
+        connections = [
+            (
+                self.input_node,
+                init_node,
+                [
+                    ("dwi", "dwi"),
+                    ("bvec", "bvec"),
+                    ("bval", "bval"),
+                    ("dwi_json", "dwi_json"),
+                    ("fmap_magnitude", "fmap_magnitude"),
+                    ("fmap_phasediff", "fmap_phasediff"),
+                    ("fmap_phasediff_json", "fmap_phasediff_json"),
+                ],
+            ),
+            (
+                init_node,
+                reference_b0,
+                [
+                    ("bval", "inputnode.b_values_filename"),
+                    ("bvec", "inputnode.b_vectors_filename"),
+                    ("dwi", "inputnode.dwi_filename"),
+                    ("total_readout_time", "inputnode.total_readout_time"),
+                    ("phase_encoding_direction", "inputnode.phase_encoding_direction"),
+                    ("image_id", "inputnode.image_id"),
+                ],
+            ),
+            (
+                init_node,
+                fmap_calibration_and_registration,
+                [
+                    ("fmap_magnitude", "inputnode.bias_magnitude_fmap"),
+                    ("fmap_phasediff", "inputnode.fmap_phasediff"),
+                    ("delta_echo_time", "inputnode.delta_echo_time"),
+                ],
+            ),
+            (
+                reference_b0,
+                fmap_calibration_and_registration,
+                [("outputnode.reference_b0", "inputnode.reference_b0")],
+            ),
+            (
+                init_node,
+                eddy,
+                [
+                    ("dwi", "inputnode.dwi_filename"),
+                    ("bval", "inputnode.b_values_filename"),
+                    ("bvec", "inputnode.b_vectors_filename"),
+                    ("image_id", "inputnode.image_id"),
+                ],
+            ),
+            (
+                fmap_calibration_and_registration,
+                eddy,
+                [("outputnode.smooth_calibrated_fmap", "inputnode.field")],
+            ),
+            (reference_b0, eddy, [("outputnode.brainmask", "inputnode.in_mask")]),
+            # Step 4: Bias correction
+            # =======================
+            (init_node, bias, [("bval", "in_bval")]),
+            (
+                eddy,
+                bias,
+                [
+                    ("outputnode.out_rotated_bvecs", "in_bvec"),
+                    ("outputnode.out_corrected", "in_file"),
+                ],
+            ),
+            # Step 5: Final brainmask
+            # =======================
+            # Compute average b0 on corrected dataset (for brain mask extraction)
+            (init_node, compute_avg_b0, [("bval", "in_bval")]),
+            (bias, compute_avg_b0, [("out_file", "in_dwi")]),
+            # Compute b0 mask on corrected avg b0
+            (compute_avg_b0, mask_avg_b0, [("reference_b0", "in_file")]),
+            # Print end message
+            (init_node, print_end_message, [("image_id", "image_id")]),
+            (mask_avg_b0, print_end_message, [("mask_file", "final_file")]),
+            # Output node
+            (init_node, self.output_node, [("bval", "preproc_bval")]),
+            (
+                eddy,
+                self.output_node,
+                [("outputnode.out_rotated_bvecs", "preproc_bvec")],
+            ),
+            (bias, self.output_node, [("out_file", "preproc_dwi")]),
+            (mask_avg_b0, self.output_node, [("mask_file", "b0_mask")]),
+            (
+                fmap_calibration_and_registration,
+                self.output_node,
+                [
+                    (
+                        "outputnode.bet_magnitude_fmap_registered_onto_b0",
+                        "magnitude_on_b0",
+                    )
+                ],
+            ),
+            (
+                fmap_calibration_and_registration,
+                self.output_node,
+                [("outputnode.registered_calibrated_fmap", "calibrated_fmap_on_b0")],
+            ),
+            (
+                fmap_calibration_and_registration,
+                self.output_node,
+                [("outputnode.smooth_calibrated_fmap", "smoothed_fmap_on_b0")],
+            ),
+        ]
+
+        self.connect(connections)
```

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_utils.py` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/dwi_preprocessing_using_phasediff_fmap_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,31 +143,52 @@
 def print_end_pipeline(image_id, final_file):
     """Display end message for `image_id` when `final_file` is connected."""
     from clinica.utils.ux import print_end_image
 
     print_end_image(image_id)
 
 
-def rads2hz(in_file, delta_te, out_file=None):
-    """Convert input phase difference map to Hz."""
+def rads2hz(in_file: str, delta_te: float, out_file: str = None) -> str:
+    """Convert input phase difference map to Hz.
+
+    Parameters
+    ----------
+    in_file : str
+        Path to the phase difference map image.
+
+    delta_te : float
+        The DeltaEchoTime from BIDS specifications.
+
+    out_file : str, optional
+        Path to output file. If None, the output image
+        will be written in current folder. The file name
+        will have the same base name as in_file, but with
+        the "_radsec.nii.gz" suffix.
+
+    Returns
+    -------
+    out_file : str
+        Path to output file.
+    """
     import math
     import os
 
     import nibabel as nb
     import numpy as np
 
     if out_file is None:
         fname, fext = os.path.splitext(os.path.basename(in_file))
         if fext == ".gz":
             fname, _ = os.path.splitext(fname)
         out_file = os.path.abspath(f"./{fname}_radsec.nii.gz")
 
     im = nb.load(in_file)
-    data = im.get_data().astype(np.float32) * (1.0 / (delta_te * 2 * math.pi))
+    data = im.get_data().astype(np.float32) * (1.0 / (float(delta_te) * 2 * math.pi))
     nb.Nifti1Image(data, im.affine, im.header).to_filename(out_file)
+
     return out_file
 
 
 def resample_fmap_to_b0(in_fmap, in_b0, out_file=None):
     """Resample fieldmap onto the b0 image.
 
     Warnings:
```

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_fmap/info.json` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_fmap/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_cli.py` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_pipeline.py` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -236,19 +236,19 @@
     def build_core_nodes(self):
         """Build and connect the core nodes of the pipeline."""
         import nipype.interfaces.fsl as fsl
         import nipype.interfaces.mrtrix3 as mrtrix3
         import nipype.interfaces.utility as nutil
         import nipype.pipeline.engine as npe
 
-        from clinica.utils.dwi import compute_average_b0
+        from clinica.utils.dwi import compute_average_b0_task
 
         from .dwi_preprocessing_using_t1_utils import (
             init_input_node,
-            prepare_reference_b0,
+            prepare_reference_b0_task,
             print_end_pipeline,
         )
         from .dwi_preprocessing_using_t1_workflows import (
             eddy_fsl_pipeline,
             epi_pipeline,
         )
 
@@ -273,39 +273,37 @@
         )
 
         # Prepare b0 image for further corrections
         prepare_b0 = npe.Node(
             name="PrepareB0",
             interface=nutil.Function(
                 input_names=[
-                    "in_dwi",
-                    "in_bval",
-                    "in_bvec",
-                    "low_bval",
+                    "dwi_filename",
+                    "b_values_filename",
+                    "b_vectors_filename",
+                    "b_value_threshold",
                     "working_directory",
                 ],
                 output_names=[
                     "out_reference_b0",
                     "out_b0_dwi_merge",
                     "out_updated_bval",
                     "out_updated_bvec",
                 ],
-                function=prepare_reference_b0,
+                function=prepare_reference_b0_task,
             ),
         )
-        prepare_b0.inputs.low_bval = self.parameters["low_bval"]
+        prepare_b0.inputs.b_value_threshold = self.parameters["low_bval"]
         prepare_b0.inputs.working_directory = self.base_dir
-        # Mask b0 for computations purposes
-        mask_b0_pre = npe.Node(
-            fsl.BET(frac=0.3, mask=True, robust=True), name="PreMaskB0"
-        )
+
         # Head-motion correction + Eddy-currents correction
         eddy_fsl = eddy_fsl_pipeline(
             use_cuda=self.parameters["use_cuda"],
             initrand=self.parameters["initrand"],
+            compute_mask=True,
         )
         # Susceptibility distortion correction using T1w image
         sdc = epi_pipeline(
             self.base_dir,
             self.parameters["delete_cache"],
             name="SusceptibilityDistortionCorrection",
         )
@@ -317,21 +315,21 @@
                 out_file="Jacobian_image_maths_thresh_merged_biascorr.nii.gz",
             ),
             name="RemoveBias",
         )
         # Compute b0 mask on corrected avg b0
         compute_avg_b0 = npe.Node(
             nutil.Function(
-                input_names=["in_dwi", "in_bval"],
+                input_names=["dwi_filename", "b_value_filename"],
                 output_names=["out_b0_average"],
-                function=compute_average_b0,
+                function=compute_average_b0_task,
             ),
             name="ComputeB0Average",
         )
-        compute_avg_b0.inputs.low_bval = self.parameters["low_bval"]
+        compute_avg_b0.inputs.b_value_threshold = self.parameters["low_bval"]
 
         # Compute brain mask from reference b0
         mask_avg_b0 = npe.Node(fsl.BET(mask=True, robust=True), name="MaskB0")
 
         # Print end message
         print_end_message = npe.Node(
             interface=nutil.Function(
@@ -348,38 +346,35 @@
                 # Initialize input parameters and print begin message
                 (self.input_node, init_node, [("t1w", "t1w"),
                                               ("dwi", "dwi"),
                                               ("bvec", "bvec"),
                                               ("bval", "bval"),
                                               ("dwi_json", "dwi_json")]),
                 # Preliminary step (possible computation of a mean b0):
-                (init_node, prepare_b0, [("dwi", "in_dwi"),
-                                         ("bval", "in_bval"),
-                                         ("bvec", "in_bvec")]),
-                # Mask b0 before corrections
-                (prepare_b0, mask_b0_pre, [("out_reference_b0", "in_file")]),
+                (init_node, prepare_b0, [("dwi", "dwi_filename"),
+                                         ("bval", "b_values_filename"),
+                                         ("bvec", "b_vectors_filename")]),
                 # Head-motion correction + eddy current correction
                 (init_node, eddy_fsl, [("total_readout_time", "inputnode.total_readout_time"),
                                        ("phase_encoding_direction", "inputnode.phase_encoding_direction")]),
                 (prepare_b0, eddy_fsl, [("out_b0_dwi_merge", "inputnode.dwi_filename"),
                                         ("out_updated_bval", "inputnode.b_values_filename"),
                                         ("out_updated_bvec", "inputnode.b_vectors_filename"),
-                                        ("out_reference_b0", "inputnode.ref_b0")]),  # TODO: check if really needed...
-                (mask_b0_pre, eddy_fsl, [("mask_file", "inputnode.in_mask")]),
+                                        ("out_reference_b0", "inputnode.reference_b0")]),
                 # Magnetic susceptibility correction
                 (init_node, sdc, [("t1w", "inputnode.T1")]),
                 (eddy_fsl, sdc, [("outputnode.out_corrected", "inputnode.DWI")]),
                 (eddy_fsl, sdc, [("outputnode.out_rotated_bvecs", "inputnode.bvec")]),
                 # Bias correction
                 (prepare_b0, bias, [("out_updated_bval", "in_bval")]),
                 (sdc, bias, [("outputnode.DWIs_epicorrected", "in_file"),
                              ("outputnode.out_bvec", "in_bvec")]),
                 # Compute average b0 on corrected dataset (for brain mask extraction)
-                (prepare_b0, compute_avg_b0, [("out_updated_bval", "in_bval")]),
-                (bias, compute_avg_b0, [("out_file", "in_dwi")]),
+                (prepare_b0, compute_avg_b0, [("out_updated_bval", "b_value_filename")]),
+                (bias, compute_avg_b0, [("out_file", "dwi_filename")]),
                 # Compute b0 mask on corrected avg b0
                 (compute_avg_b0, mask_avg_b0, [("out_b0_average", "in_file")]),
                 # Print end message
                 (init_node, print_end_message, [("image_id", "image_id")]),
                 (mask_avg_b0, print_end_message, [("mask_file", "final_file")]),
                 # Output node
                 (bias, self.output_node, [("out_file", "preproc_dwi")]),
```

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,345 +1,304 @@
-def rename_into_caps(
-    in_bids_dwi: str,
-    fname_dwi: str,
-    fname_bval: str,
-    fname_bvec: str,
-    fname_brainmask: str,
-):
-    """Rename the outputs of the pipelines into CAPS.
-
-    Parameters
-    ----------
-    in_bids_dwi : str
-        Path to input BIDS DWI to extract the <source_file>
-
-    fname_dwi : str
-        Name of preprocessed DWI file.
-
-    fname_bval : str
-        Name of preprocessed bval file.
-
-    fname_bvec : str
-        Name of preprocessed bvec file.
-
-    fname_brainmask : str
-        Name of B0 mask file.
-
-    Returns
-    -------
-    Tuple[str, str, str, str]
-        The different outputs in CAPS format.
-    """
-    from clinica.utils.dwi import rename_files
-
-    return rename_files(
-        in_bids_dwi,
-        {
-            fname_dwi: "_space-T1w_preproc.nii.gz",
-            fname_bval: "_space-T1w_preproc.bval",
-            fname_bvec: "_space-T1w_preproc.bval",
-            fname_brainmask: "_space-T1w_brainmask.nii.gz",
-        },
-    )
-
-
-def change_itk_transform_type(input_affine_file):
-    """Change ITK transform type.
-
-    This function takes in the affine.txt produced by the c3d_affine_tool (which converted
-    an FSL FLIRT affine.mat into the affine.txt) it then modifies the 'Transform Type' of
-    this affine.txt so that it is compatible with the antsApplyTransforms tool and
-    produces a new affine file titled 'updated_affine.txt'.
-
-    """
+def init_input_node(caps_dir, participant_id, session_id, long_id, output_dir):
+    """Initialize the pipeline."""
     import os
+    import platform
+    from tempfile import mkdtemp
 
-    new_file_lines = []
-
-    with open(input_affine_file) as f:
-        for line in f:
-            if "Transform:" in line:
-                if "MatrixOffsetTransformBase_double_3_3" in line:
-                    transform_line = "Transform: AffineTransform_double_3_3\n"
-                    new_file_lines.append(transform_line)
-            else:
-                new_file_lines.append(line)
-
-    updated_affine_file = os.path.join(os.getcwd(), "updated_affine.txt")
-
-    with open(updated_affine_file, "wt") as f:
-        for line in new_file_lines:
-            f.write(line)
-
-    return updated_affine_file
-
-
-def expend_matrix_list(in_matrix, in_bvec):
-    import numpy as np
-
-    bvecs = np.loadtxt(in_bvec).T
-    out_matrix_list = [in_matrix]
-
-    out_matrix_list = out_matrix_list * len(bvecs)
+    from clinica.utils.longitudinal import read_sessions
+    from clinica.utils.stream import cprint
+    from clinica.utils.ux import print_begin_image
 
-    return out_matrix_list
+    # Extract <image_id>
+    image_id = "{0}_{1}_{2}".format(participant_id, session_id, long_id)
 
+    # Create SUBJECTS_DIR for recon-all (otherwise, the command won't run)
+    if platform.system().lower().startswith("darwin"):
+        # Special case: On macOS, 'recon-all -long' can failed if the $SUBJECTS_DIR is too long
+        # To circumvent this issue, we create a sym link in $(TMP) so that $SUBJECTS_DIR is a short path
+        subjects_dir = mkdtemp()
+        cprint(
+            msg=(
+                f"Needs to create a $SUBJECTS_DIR folder "
+                f"in {subjects_dir} for {image_id.replace('_', ' | ')} (macOS case)."
+            ),
+            lvl="warning",
+        )
+    else:
+        subjects_dir = os.path.join(output_dir, image_id)
 
-def ants_warp_image_multi_transform(fix_image, moving_image, ants_warp_affine):
-    import os
+    os.makedirs(subjects_dir, exist_ok=True)
 
-    out_warp = os.path.abspath("warped_epi.nii.gz")
+    # Create symbolic link containing cross-sectional segmentation(s) in SUBJECTS_DIR so that recon-all can run
+    for s_id in read_sessions(caps_dir, participant_id, long_id):
+        cross_sectional_path = os.path.join(
+            caps_dir,
+            "subjects",
+            participant_id,
+            s_id,
+            "t1",
+            "freesurfer_cross_sectional",
+            f"{participant_id}_{s_id}",
+        )
+        os.symlink(
+            cross_sectional_path,
+            os.path.join(subjects_dir, f"{participant_id}_{s_id}"),
+        )
 
-    cmd = (
-        f"WarpImageMultiTransform 3 {moving_image} {out_warp} -R {fix_image} "
-        f"{ants_warp_affine[0]} {ants_warp_affine[1]} {ants_warp_affine[2]}"
+    # Create symbolic links containing unbiased template in SUBJECTS_DIR so that recon-all can run
+    template_path = os.path.join(
+        caps_dir,
+        "subjects",
+        participant_id,
+        long_id,
+        "freesurfer_unbiased_template",
+        f"{participant_id}_{long_id}",
     )
-    os.system(cmd)
+    os.symlink(template_path, os.path.join(subjects_dir, f"{participant_id}_{long_id}"))
 
-    return out_warp
+    print_begin_image(image_id)
 
+    return subjects_dir
 
-def rotate_bvecs(in_bvec, in_matrix):
-    """Rotate the input bvec file accordingly with a list of matrices.
-
-    Notes:
-        The input affine matrix transforms points in the destination image to their corresponding
-        coordinates in the original image. Therefore, this matrix should be inverted first, as
-        we want to know the target position of :math:`\\vec{r}`.
-
-    """
-    import os
 
-    import numpy as np
+def run_recon_all_long(subjects_dir, participant_id, session_id, long_id, directive):
+    """Run recon-all to create a longitudinal correction of a time point.
 
-    name, fext = os.path.splitext(os.path.basename(in_bvec))
-    if fext == ".gz":
-        name, _ = os.path.splitext(name)
-    out_file = os.path.abspath(f"{name}_rotated.bvec")
-    # Warning, bvecs.txt are not in the good configuration, need to put '.T'
-    bvecs = np.loadtxt(in_bvec).T
-    new_bvecs = []
-
-    if len(bvecs) != len(in_matrix):
-        raise RuntimeError(
-            f"Number of b-vectors ({len(bvecs)}) and rotation matrices ({len(in_matrix)}) should match."
-        )
+    Note:
+    Longitudinal correction with FreeSurfer expects arguments to follow this syntax:
+    recon-all -long <tpN_id> <template_id> -all; e.g.: recon-all -long sub-CLNC01_ses-M000 sub-CLNC01_long-M000M018 -all
 
-    for bvec, mat in zip(bvecs, in_matrix):
-        if np.all(bvec == 0.0):
-            new_bvecs.append(bvec)
-        else:
-            invrot = np.linalg.inv(np.loadtxt(mat))[:3, :3]
-            newbvec = invrot.dot(bvec)
-            new_bvecs.append((newbvec / np.linalg.norm(newbvec)))
+    Currently, Nipype does not provide interface for "recon-all -long" case. As a result, ReconAll interface should be
+    modified to handle this situation. In the meantime, the arguments of this function follows ReconAll.inputs names
+    namely:
+        - "-long <tpN_id> <template_id>" is likely to be fed to ReconAll.inputs.args
+        - "-all" will be fed to ReconAll.inputs.directive
 
-    np.savetxt(out_file, np.array(new_bvecs).T, fmt="%0.15f")
-    return out_file
+    Folder containing the longitudinal correction has the following convention:
+    <tpN_id>.long.<template_id>; e.g.: sub-CLNC01_ses-M000.long.sub-CLNC01_long-M000M018
+    which is automatically generated by FreeSurfer.
 
+    This folder name is likely to be retrieved in ReconAll.outputs.subject_id.
 
-def ants_apply_transforms(
-    fixed_image, moving_image, transforms, warped_image, output_warped_image=True
-) -> None:
-    import os
+    See official documentation (https://surfer.nmr.mgh.harvard.edu/fswiki/LongitudinalProcessing) for details.
+    """
     import subprocess
 
-    # Convert to absolute path.
-    warped_image = os.path.abspath(warped_image)
-
-    # Whether we want the warped image or transformation field as output.
-    output = f"{warped_image}" if output_warped_image else f"[{warped_image}, 1]"
+    # Prepare arguments for recon-all.
+    flags = " -long {0}_{1} {0}_{2} ".format(participant_id, session_id, long_id)
 
-    # Common template for the command.
-    cmd = (
-        f"antsApplyTransforms -o {output} -i {moving_image} -r {fixed_image} "
-        f"-t {transforms[0]} -t {transforms[1]} -t {transforms[2]}"
+    recon_all_long_command = "recon-all {0} -sd {1} {2}".format(
+        flags, subjects_dir, directive
     )
+    subprocess_run_recon_all_long = subprocess.run(
+        recon_all_long_command,
+        shell=True,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+    )
+    if subprocess_run_recon_all_long.returncode != 0:
+        raise ValueError("recon-all -long failed, returned non-zero code")
 
-    # Perform the actual call.
-    subprocess.run(cmd, shell=True)
-
-    return warped_image
+    subject_id = "{0}_{1}.long.{0}_{2}".format(participant_id, session_id, long_id)
 
+    return subject_id
 
-def init_input_node(t1w, dwi, bvec, bval, dwi_json):
-    """Initialize the pipeline."""
-    from clinica.utils.dwi import bids_dir_to_fsl_dir, check_dwi_volume
-    from clinica.utils.filemanip import (
-        extract_metadata_from_json,
-        get_subject_id,
-        handle_missing_keys_dwi,
-    )
-    from clinica.utils.ux import print_begin_image
 
-    # Extract image ID
-    image_id = get_subject_id(t1w)
+def write_tsv_files(subjects_dir, subject_id):
+    """Generate statistics TSV files in `subjects_dir`/regional_measures folder for `subject_id`.
 
-    # Check that the number of DWI, bvec & bval are the same
-    check_dwi_volume(dwi, bvec, bval)
-
-    # Read metadata from DWI JSON file:
-    [total_readout_time, phase_encoding_direction] = extract_metadata_from_json(
-        dwi_json,
-        [
-            "TotalReadoutTime",
-            "PhaseEncodingDirection",
-        ],
-        handle_missing_keys=handle_missing_keys_dwi,
-    )
-    phase_encoding_direction = bids_dir_to_fsl_dir(phase_encoding_direction)
+    Notes:
+        We do not need to check the line "finished without error" in scripts/recon-all.log.
+        If an error occurs, it will be detected by Nipype and the next nodes (i.e.
+        write_tsv_files will not be called).
+    """
+    import os
 
-    # Print begin message
-    print_begin_image(
-        image_id,
-        ["TotalReadoutTime", "PhaseEncodingDirection"],
-        [str(total_readout_time), phase_encoding_direction],
+    from clinica.utils.freesurfer import (
+        extract_image_id_from_longitudinal_segmentation,
+        generate_regional_measures,
     )
+    from clinica.utils.stream import cprint
 
-    return (
-        image_id,
-        t1w,
-        dwi,
-        bvec,
-        bval,
-        total_readout_time,
-        phase_encoding_direction,
+    image_id = extract_image_id_from_longitudinal_segmentation(subject_id)
+    str_image_id = (
+        image_id.participant_id + "_" + image_id.session_id + "_" + image_id.long_id
     )
+    if os.path.isfile(os.path.join(subjects_dir, subject_id, "mri", "aparc+aseg.mgz")):
+        generate_regional_measures(subjects_dir, subject_id)
+    else:
+        cprint(
+            msg=(
+                f"{str_image_id.replace('_', ' | ')} does not contain mri/aseg+aparc.mgz file. "
+                "Creation of regional_measures/ folder will be skipped."
+            ),
+            lvl="warning",
+        )
+    return subject_id
 
 
-def print_end_pipeline(image_id, final_file):
-    """Display end message for `image_id` when `final_file` is connected."""
-    from clinica.utils.ux import print_end_image
-
-    print_end_image(image_id)
-
-
-def prepare_reference_b0(in_dwi, in_bval, in_bvec, low_bval=5, working_directory=None):
-    """Prepare reference b=0 image.
+def move_subjects_dir_to_source_dir(subjects_dir, source_dir, subject_id):
+    """Move content of `subjects_dir`/`subject_id` to `source_dir`.
 
-    This function prepare the data for further corrections. It co-registers the B0 images
-    and then average it in order to obtain only one average B0 images.
+    This function will move content of `subject_id` if recon-all has run
+    in $(TMP). This happens when FreeSurfer is run on macOS. Content of
+    $(TMP)/`subject_id` is copied to `source_dir` before the deletion of $(TMP).
 
     Args:
-        in_dwi (str): Input DWI file.
-        in_bvec (str): Vector file of the diffusion directions of the DWI dataset.
-        in_bval (str): B-values file.
-        low_bval (optional, int): Set b<=low_bval such that images are considered b0. Defaults to 5.
-        working_directory (str): Temporary folder results where the results are stored. Defaults to None.
+        subjects_dir: $(TMP), if segmentation was performed on macOS,
+            <base_dir>/<Pipeline.Name>/ReconAll/`subject_id` otherwise
+        source_dir: <base_dir>/<Pipeline.Name>/ReconAll folder
+        subject_id: Subject ID (e.g. "sub-CLNC01_ses-M000.long.sub-CLNC01_long-M000M018")
 
     Returns:
-        out_reference_b0 (str): Average of the B0 images or the only B0 image.
-        out_b0_dwi_merge (str): Average of B0 images merged to the DWIs.
-        out_updated_bval (str): Updated gradient values table.
-        out_updated_bvec (str): Updated gradient vectors table.
+        subject_id for node connection with Nipype
     """
-    import hashlib
     import os
-    import tempfile
-
-    from clinica.pipelines.dwi_preprocessing_using_t1.dwi_preprocessing_using_t1_workflows import (
-        b0_flirt_pipeline,
-    )
-    from clinica.utils.dwi import (
-        b0_average,
-        b0_dwi_split,
-        count_b0s,
-        insert_b0_into_dwi,
-    )
+    import shutil
 
-    # Count the number of b0s
-    nb_b0s = count_b0s(in_bval=in_bval, low_bval=low_bval)
+    from clinica.utils.freesurfer import extract_image_id_from_longitudinal_segmentation
+    from clinica.utils.stream import cprint
 
-    # Split dataset into two datasets: the b0 and the b>low_bval datasets
-    [extracted_b0, out_split_dwi, out_split_bval, out_split_bvec] = b0_dwi_split(
-        in_dwi=in_dwi, in_bval=in_bval, in_bvec=in_bvec, low_bval=low_bval
+    image_id = extract_image_id_from_longitudinal_segmentation(subject_id)
+    str_image_id = (
+        image_id.participant_id + "_" + image_id.session_id + "_" + image_id.long_id
     )
 
-    if nb_b0s == 1:
-        # The reference b0 is the extracted b0
-        # cprint('Only one b0 for %s' % in_dwi)
-        out_reference_b0 = extracted_b0
-    elif nb_b0s > 1:
-        # Register the b0 onto the first b0
-        b0_flirt = b0_flirt_pipeline(num_b0s=nb_b0s)
-        b0_flirt.inputs.inputnode.in_file = extracted_b0
-        if working_directory is None:
-            working_directory = tempfile.mkdtemp()
-        tmp_dir = os.path.join(
-            working_directory, hashlib.md5(in_dwi.encode()).hexdigest()
+    if source_dir not in subjects_dir:
+        shutil.copytree(
+            src=os.path.join(subjects_dir, subject_id),
+            dst=os.path.join(source_dir, str_image_id, subject_id),
+            symlinks=True,
         )
-        b0_flirt.base_dir = tmp_dir
-        b0_flirt.run()
-        # BUG: Nipype does allow to extract the output after running the
-        # workflow: we need to 'guess' where the output will be generated
-        # out_node = b0_flirt.get_node('outputnode')
-        registered_b0s = os.path.abspath(
-            os.path.join(
-                tmp_dir, "b0_coregistration", "concat_ref_moving", "merged_files.nii.gz"
-            )
+        shutil.copytree(
+            src=os.path.join(subjects_dir, "regional_measures"),
+            dst=os.path.join(source_dir, str_image_id, "regional_measures"),
+            symlinks=True,
         )
-        # cprint('B0 s will be averaged (file = ' + registered_b0s + ')')
-        # Average the b0s to obtain the reference b0
-        out_reference_b0 = b0_average(in_file=registered_b0s)
-    else:
-        raise ValueError(
-            f"The number of b0s should be strictly positive (b-val file: {in_bval})."
+        shutil.rmtree(subjects_dir)
+        cprint(
+            msg=(
+                f"Segmentation of {subject_id.replace('_', ' | ')} "
+                f"has moved to working directory and $SUBJECTS_DIR folder ({subjects_dir}) was deleted."
+            ),
+            lvl="warning",
         )
 
-    # Merge datasets such that bval(DWI) = (0 b1 ... bn)
-    [out_b0_dwi_merge, out_updated_bval, out_updated_bvec] = insert_b0_into_dwi(
-        in_b0=out_reference_b0,
-        in_dwi=out_split_dwi,
-        in_bval=out_split_bval,
-        in_bvec=out_split_bvec,
-    )
+    return subject_id
 
-    return out_reference_b0, out_b0_dwi_merge, out_updated_bval, out_updated_bvec
 
+def save_to_caps(source_dir, subject_id, caps_dir, overwrite_caps=False):
+    """Save `source_dir`/`subject_id`/ to CAPS folder.
 
-def extract_sub_ses_folder_name(file_path: str) -> str:
-    """This function extracts the name of the folder corresponding to a subject and a session.
+    This function copies FreeSurfer segmentation and regional_measures folder of `source_dir`/`image_id`/ to
+    `caps_dir`/subjects/<participant_id>/<session_id>/<long_id>/t1_freesurfer_longitudinal/
+    where `image_id` = <participant_id>_<session_id>_<long_id>.
 
-    Parameters
-    ----------
-    file_path: str
-        Path to a temporary file for the subject and session of interest.
-
-    Returns
-    -------
-    str:
-    Name of the folder corresponding to a subject and a session.
-
-    Examples
-    --------
-    >>> extract_sub_ses_folder_name("/localdrive10TB/users/matthieu.joulot/wd/dwi-preprocessing-using-t1/epi_pipeline/4336d63c8556bb56d4e9d1abc617fb3eaa3c38ea/MergeDWIs/Jacobian_image_maths_thresh_merged.nii.gz")
-    4336d63c8556bb56d4e9d1abc617fb3eaa3c38ea
-    """
-    from pathlib import Path
+    The `source_dir`/`image_id`/ folder should contain the following elements:
+        - fsaverage, lh.EC_average and rh.EC_average symbolic links automatically generated by recon-all
+        - symbolic links to cross-sectional segmentation(s) and unbiased template needed for recon-all
+        - <participant_id>_<session_id>.long.<participant_id>_<long_id>/ folder containing the FreeSurfer segmentation
+        - regional_measures/ folder containing TSV files
 
-    return (Path(Path(file_path).parent).parent).name
+    Notes:
+        We do not need to check the line "finished without error" in scripts/recon-all.log.
+        If an error occurs, it will be detected by Nipype and the next nodes (i.e. save_to_caps will not be called).
+    """
+    import os
+    import shutil
 
+    from clinica.utils.freesurfer import extract_image_id_from_longitudinal_segmentation
+    from clinica.utils.stream import cprint
+    from clinica.utils.ux import print_end_image
 
-def delete_temp_dirs(checkpoint: str, dir_to_del: list, base_dir: str) -> None:
-    """This function deletes the directories of the given list".
+    image_id = extract_image_id_from_longitudinal_segmentation(subject_id)
+    participant_id = image_id.participant_id
+    session_id = image_id.session_id
+    long_id = image_id.long_id
+    str_image_id = (
+        image_id.participant_id + "_" + image_id.session_id + "_" + image_id.long_id
+    )
+
+    destination_dir = os.path.join(
+        os.path.expanduser(caps_dir),
+        "subjects",
+        participant_id,
+        session_id,
+        "t1",
+        long_id,
+        "freesurfer_longitudinal",
+    )
+
+    # Save FreeSurfer segmentation
+    representative_file = os.path.join(subject_id, "mri", "aparc+aseg.mgz")
+    representative_source_file = os.path.join(
+        os.path.expanduser(source_dir), str_image_id, representative_file
+    )
+    representative_destination_file = os.path.join(destination_dir, representative_file)
+    if os.path.isfile(representative_source_file):
+        if os.path.isfile(representative_destination_file):
+            if overwrite_caps:
+                shutil.rmtree(destination_dir)
+                shutil.copytree(
+                    src=os.path.join(source_dir, subject_id, subject_id),
+                    dst=os.path.join(destination_dir, subject_id),
+                    symlinks=True,
+                )
+                shutil.copytree(
+                    src=os.path.join(source_dir, subject_id, "regional_measures"),
+                    dst=os.path.join(destination_dir, "regional_measures"),
+                    symlinks=True,
+                )
+        else:
+            shutil.copytree(
+                src=os.path.join(source_dir, str_image_id, subject_id),
+                dst=os.path.join(destination_dir, subject_id),
+                symlinks=True,
+            )
+            shutil.copytree(
+                src=os.path.join(source_dir, str_image_id, "regional_measures"),
+                dst=os.path.join(destination_dir, "regional_measures"),
+                symlinks=True,
+            )
+        print_end_image(str_image_id)
+    else:
+        cprint(
+            msg=f"{subject_id.replace('_', ' | ')}  does not contain mri/aseg+aparc.mgz file. Copy will be skipped.",
+            lvl="warning",
+        )
 
-    Parameters
-    ----------
-    checkpoint: str
-    Path to a file. Used to ensure, that the temporary directories we want to delete are not useful anymore, and to verify that the subject and session are right.
+    return str_image_id
 
-    dir_to_del: list
-    Names of the directories we want to delete.
 
-    base_dir: str
-    Path to the working directory.
+def get_processed_images(caps_directory, part_ids, sess_ids, long_ids, atlas=False):
     """
-    import shutil
-    from pathlib import Path
-
-    from clinica.utils.stream import cprint
+    Extract image IDs (e.g. ["sub-CLNC01_ses-M000_long-M000M018", "sub-CLNC01_ses-M018_long-M000M018"]) of outputs
+    already processed by T1FreeSurferLongitudinalCorrection pipeline.
+    """
+    import os
 
-    subject_session_folder_name = extract_sub_ses_folder_name(checkpoint)
-    for a in dir_to_del:
-        for z in Path(base_dir).rglob(f"*{a}*"):
-            if (Path(z).parent).name == subject_session_folder_name:
-                shutil.rmtree(z)
-                cprint(msg=f"Temporary folder {z} deleted", lvl="info")
+    image_ids = []
+    if os.path.isdir(caps_directory):
+        for (participant_id, session_id, long_id) in zip(part_ids, sess_ids, long_ids):
+            output_file_pre = os.path.join(
+                os.path.expanduser(caps_directory),
+                "subjects",
+                participant_id,
+                session_id,
+                "t1",
+                long_id,
+                "freesurfer_longitudinal",
+                f"{participant_id}_{session_id}.long.{participant_id}_{long_id}",
+            )
+            if atlas:
+                output_file = os.path.join(
+                    output_file_pre, "stat", "rh.", atlas, ".stats"
+                )
+            else:
+                output_file = os.path.join(
+                    output_file_pre,
+                    "mri",
+                    "aparc+aseg.mgz",
+                )
+            if os.path.isfile(output_file):
+                image_ids.append(f"{participant_id}_{session_id}_{long_id}")
+    return image_ids
```

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_workflows.py` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/dwi_preprocessing_using_t1_workflows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,109 @@
 from nipype.pipeline.engine import Workflow
 
 
 def eddy_fsl_pipeline(
     use_cuda: bool,
     initrand: bool,
+    compute_mask: bool = True,
     image_id: bool = False,
     field: bool = False,
+    output_dir=None,
     name: str = "eddy_fsl",
 ) -> Workflow:
     """Build a FSL-based pipeline for head motion correction and eddy current distortion correction.
 
     This pipeline needs FSL as it relies on the Eddy executable.
 
     Parameters
     ----------
     use_cuda : bool
         Boolean to indicate whether cuda should be used or not.
 
     initrand : bool
         ????
 
+    compute_mask : bool, optional
+        If True, the eddy_fsl pipeline computes the brain mask
+        of the reference B0 volume using FSL BET. And provide the
+        result to Eddy.
+        If False, a mask should be provided to the eddy_fsl
+        pipeline through the "in_mask" connection.
+        Default=True.
+
     image_id : bool, optional
         Boolean to indicate whether the Eddy node should expect
         a value for its 'out_base' parameter. This is used for
         building the names of the output files.
         Default=False.
 
     field : bool, optional
         Boolean to indicate whether the Eddy node should expect
         a value for its 'field' input.
         Default=False.
 
+    output_dir: str, optional
+        Path to output directory.
+        If provided, the pipeline will write its output in this folder.
+        Default to None.
+
     name : str, optional
         Name of the pipeline. Default='eddy_fsl'.
 
     Returns
     -------
     Workflow :
         The Nipype workflow.
         This workflow has the following inputs:
             - "dwi_filename": The path to the DWI image
             - "b_vectors_filename": The path to the associated B-vectors file
             - "b_values_filename": The path to the associated B-values file
             - "in_mask": The path to the mask image to be provided to Eddy
+              This will be used only if compute_mask is False.
             - "image_id": Prefix to be used for output files
             - "field": The path to the field image to be used by Eddy
-            - "ref_b0": ???
+            - "reference_b0": The path to the reference B0 image
+              This will be used to compute the mask only if compute_mask is True.
             - "total_readout_time": The total readout time extracted from JSON metadata
             - "phase_encoding_direction": The phase encoding direction extracted from JSON metadata
 
         And the following outputs:
             - "out_parameter": Path to the file storing the output parameters
             - "out_corrected": Path to the corrected image
             - "out_rotated_bvecs": Path to the file holding the rotated B-vectors
     """
+    import nipype.interfaces.io as nio
     import nipype.interfaces.utility as niu
     import nipype.pipeline.engine as pe
+    from nipype.interfaces.fsl import BET
     from nipype.interfaces.fsl.epi import Eddy
 
     from clinica.utils.dwi import generate_acq_file, generate_index_file
 
     inputnode = pe.Node(
         niu.IdentityInterface(
             fields=[
                 "dwi_filename",
                 "b_vectors_filename",
                 "b_values_filename",
                 "in_mask",
                 "image_id",
                 "field",
-                "ref_b0",
+                "reference_b0",
                 "total_readout_time",
                 "phase_encoding_direction",
             ]
         ),
         name="inputnode",
     )
 
+    mask_reference_b0 = pe.Node(
+        BET(frac=0.3, mask=True, robust=True), name="mask_reference_b0"
+    )
+
     generate_acq = pe.Node(
         niu.Function(
             input_names=[
                 "dwi_filename",
                 "fsl_phase_encoding_direction",
                 "total_readout_time",
                 "image_id",
@@ -108,14 +131,19 @@
     outputnode = pe.Node(
         niu.IdentityInterface(
             fields=["out_parameter", "out_corrected", "out_rotated_bvecs"]
         ),
         name="outputnode",
     )
 
+    if output_dir:
+        write_results = pe.Node(name="write_results", interface=nio.DataSink())
+        write_results.inputs.base_directory = output_dir
+        write_results.inputs.parameterization = False
+
     wf = pe.Workflow(name=name)
 
     connections = [
         (inputnode, generate_acq, [("dwi_filename", "dwi_filename")]),
         (inputnode, generate_acq, [("total_readout_time", "total_readout_time")]),
         (
             inputnode,
@@ -123,15 +151,14 @@
             [("phase_encoding_direction", "fsl_phase_encoding_direction")],
         ),
         (inputnode, generate_index, [("b_values_filename", "b_values_filename")]),
         (inputnode, generate_index, [("image_id", "image_id")]),
         (inputnode, eddy, [("b_vectors_filename", "in_bvec")]),
         (inputnode, eddy, [("b_values_filename", "in_bval")]),
         (inputnode, eddy, [("dwi_filename", "in_file")]),
-        (inputnode, eddy, [("in_mask", "in_mask")]),
         (generate_acq, eddy, [("out_file", "in_acqp")]),
         (generate_index, eddy, [("out_file", "in_index")]),
         (eddy, outputnode, [("out_parameter", "out_parameter")]),
         (eddy, outputnode, [("out_corrected", "out_corrected")]),
         (eddy, outputnode, [("out_rotated_bvecs", "out_rotated_bvecs")]),
     ]
 
@@ -140,14 +167,29 @@
             (inputnode, generate_acq, [("image_id", "image_id")]),
             (inputnode, eddy, [("image_id", "out_base")]),
         ]
 
     if field:
         connections += [(inputnode, eddy, [("field", "field")])]
 
+    if compute_mask:
+        connections += [
+            (inputnode, mask_reference_b0, [("reference_b0", "in_file")]),
+            (mask_reference_b0, eddy, [("mask_file", "in_mask")]),
+        ]
+    else:
+        connections += [(inputnode, eddy, [("in_mask", "in_mask")])]
+
+    if output_dir:
+        connections += [
+            (outputnode, write_results, [("out_parameter", "out_parameter")]),
+            (outputnode, write_results, [("out_corrected", "out_corrected")]),
+            (outputnode, write_results, [("out_rotated_bvecs", "out_rotated_bvecs")]),
+        ]
+
     wf.connect(connections)
 
     return wf
 
 
 def epi_pipeline(
     base_dir: str,
@@ -187,18 +229,18 @@
     import nipype.interfaces.c3 as c3
     import nipype.interfaces.fsl as fsl
     import nipype.interfaces.utility as niu
     import nipype.pipeline.engine as pe
 
     from .dwi_preprocessing_using_t1_utils import (
         ants_apply_transforms,
+        broadcast_matrix_filename_to_match_b_vector_length,
         change_itk_transform_type,
         delete_temp_dirs,
-        expend_matrix_list,
-        rotate_bvecs,
+        rotate_b_vectors,
     )
 
     inputnode = pe.Node(
         niu.IdentityInterface(fields=["T1", "DWI", "bvec"]), name="inputnode"
     )
 
     split = pe.Node(fsl.Split(dimension="t"), name="SplitDWIs")
@@ -208,26 +250,26 @@
     flirt_b0_2_t1 = pe.Node(interface=fsl.FLIRT(dof=6), name="flirt_B0_2_T1")
     flirt_b0_2_t1.inputs.interp = "spline"
     flirt_b0_2_t1.inputs.cost = "normmi"
     flirt_b0_2_t1.inputs.cost_func = "normmi"
 
     expend_matrix = pe.Node(
         interface=niu.Function(
-            input_names=["in_matrix", "in_bvec"],
+            input_names=["matrix_filename", "b_vectors_filename"],
             output_names=["out_matrix_list"],
-            function=expend_matrix_list,
+            function=broadcast_matrix_filename_to_match_b_vector_length,
         ),
         name="expend_matrix",
     )
 
     rot_bvec = pe.Node(
         niu.Function(
-            input_names=["in_matrix", "in_bvec"],
+            input_names=["matrix_filenames", "b_vectors_filename"],
             output_names=["out_file"],
-            function=rotate_bvecs,
+            function=rotate_b_vectors,
         ),
         name="Rotate_Bvec",
     )
 
     ants_registration = pe.Node(
         interface=ants.registration.RegistrationSynQuick(
             transform_type="br", dimension=3
@@ -345,18 +387,18 @@
     # fmt: off
     wf.connect(
         [
             (inputnode, split, [("DWI", "in_file")]),
             (split, pick_ref, [("out_files", "inlist")]),
             (pick_ref, flirt_b0_2_t1, [("out", "in_file")]),
             (inputnode, flirt_b0_2_t1, [("T1", "reference")]),
-            (inputnode, rot_bvec, [("bvec", "in_bvec")]),
-            (flirt_b0_2_t1, expend_matrix, [("out_matrix_file", "in_matrix")]),
-            (inputnode, expend_matrix, [("bvec", "in_bvec")]),
-            (expend_matrix, rot_bvec, [("out_matrix_list", "in_matrix")]),
+            (inputnode, rot_bvec, [("bvec", "b_vectors_filename")]),
+            (flirt_b0_2_t1, expend_matrix, [("out_matrix_file", "matrix_filename")]),
+            (inputnode, expend_matrix, [("bvec", "b_vectors_filename")]),
+            (expend_matrix, rot_bvec, [("out_matrix_list", "matrix_filenames")]),
             (inputnode, ants_registration, [("T1", "fixed_image")]),
             (flirt_b0_2_t1, ants_registration, [("out_file", "moving_image")]),
             (inputnode, c3d_flirt2ants, [("T1", "reference_file")]),
             (pick_ref, c3d_flirt2ants, [("out", "source_file")]),
             (flirt_b0_2_t1, c3d_flirt2ants, [("out_matrix_file", "transform_file")]),
             (c3d_flirt2ants, change_transform, [("itk_transform", "input_affine_file")]),
             (change_transform, merge_transform, [("updated_affine_file", "in1")]),
@@ -399,29 +441,34 @@
 
 
 def b0_flirt_pipeline(num_b0s, name="b0_coregistration"):
     """Rigid registration of the B0 dataset onto the first volume.
 
     Rigid registration is achieved using FLIRT and the normalized correlation.
 
-    Args:
-        num_b0s (int): Number of the B0 volumes in the dataset.
-        name (str): Name of the workflow.
+    Parameters
+    ----------
+    num_b0s : int
+        Number of B0 volumes in the dataset.
+
+    name : str, optional
+        Name of the workflow.
+        Default="b0_coregistration".
 
     Inputnode:
         in_file(str): B0 dataset.
 
     Outputnode
         out_b0_reg(str): The set of B0 volumes registered to the first volume.
     """
     import nipype.interfaces.utility as niu
     import nipype.pipeline.engine as pe
     from nipype.interfaces import fsl
 
-    from clinica.utils.dwi import merge_volumes_tdim
+    from clinica.utils.image import merge_nifti_images_in_time_dimension_task
 
     inputnode = pe.Node(niu.IdentityInterface(fields=["in_file"]), name="inputnode")
     fslroi_ref = pe.Node(fsl.ExtractROI(args="0 1"), name="b0_reference")
     tsize = num_b0s - 1
     fslroi_moving = pe.Node(fsl.ExtractROI(args="1 " + str(tsize)), name="b0_moving")
     split_moving = pe.Node(fsl.Split(dimension="t"), name="split_b0_moving")
 
@@ -453,17 +500,17 @@
 
     merge = pe.Node(fsl.Merge(dimension="t"), name="merge_registered_b0s")
     thres = pe.MapNode(
         fsl.Threshold(thresh=0.0), iterfield=["in_file"], name="remove_negative"
     )
     insert_ref = pe.Node(
         niu.Function(
-            input_names=["in_file1", "in_file2"],
+            input_names=["image1", "image2"],
             output_names=["out_file"],
-            function=merge_volumes_tdim,
+            function=merge_nifti_images_in_time_dimension_task,
         ),
         name="concat_ref_moving",
     )
 
     outputnode = pe.Node(
         niu.IdentityInterface(fields=["out_file", "out_xfms"]), name="outputnode"
     )
@@ -479,16 +526,16 @@
             (bet_ref, dilate, [("mask_file", "in_file")]),
             (dilate, flirt, [("out_file", "ref_weight"),
                              ("out_file", "in_weight")]),
             (fslroi_ref, flirt, [("roi_file", "reference")]),
             (split_moving, flirt, [("out_files", "in_file")]),
             (flirt, thres, [("out_file", "in_file")]),
             (thres, merge, [("out_file", "in_files")]),
-            (merge, insert_ref, [("merged_file", "in_file2")]),
-            (fslroi_ref, insert_ref, [("roi_file", "in_file1")]),
+            (merge, insert_ref, [("merged_file", "image2")]),
+            (fslroi_ref, insert_ref, [("roi_file", "image1")]),
             (insert_ref, outputnode, [("out_file", "out_file")]),
             (flirt, outputnode, [("out_matrix_file", "out_xfms")])
         ]
     )
     # fmt: off
 
     return wf
```

### Comparing `clinica-0.7.4/clinica/pipelines/dwi_preprocessing_using_t1/info.json` & `clinica-0.7.5/clinica/pipelines/dwi_preprocessing_using_t1/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/engine.py` & `clinica-0.7.5/clinica/pipelines/engine.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/algorithm.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/algorithm.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/base.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/base.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/classification_cli.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/classification_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/input.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/input.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/ml_utils.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/ml_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/ml_workflows.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/ml_workflows.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/region_based_io.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/region_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/tsv_based_io.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/tsv_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/validation.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/validation.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/vertex_based_io.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/vertex_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning/voxel_based_io.py` & `clinica-0.7.5/clinica/pipelines/machine_learning/voxel_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py` & `clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py` & `clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         """Check pipeline parameters."""
         from clinica.utils.group import check_group_label
 
         # Clinica compulsory parameters
         self.parameters.setdefault("group_label", None)
         check_group_label(self.parameters["group_label"])
 
-        if "orig_input_data" not in self.parameters.keys():
+        if "orig_input_data_ml" not in self.parameters.keys():
             raise KeyError(
                 "Missing compulsory orig_input_data key in pipeline parameter."
             )
 
         # Optional parameters for inputs from pet-volume pipeline
         self.parameters.setdefault("acq_label", None)
         self.parameters.setdefault("suvr_reference_region", None)
@@ -79,27 +79,27 @@
             name="LoadingCLIArguments",
             interface=nutil.IdentityInterface(
                 fields=self.get_input_fields(), mandatory_inputs=True
             ),
         )
         all_errors = []
 
-        if self.parameters["orig_input_data"] == "t1-volume":
+        if self.parameters["orig_input_data_ml"] == "t1-volume":
             caps_files_information = {
                 "pattern": os.path.join(
                     "t1",
                     "spm",
                     "dartel",
                     "group-" + self.parameters["group_label"],
                     "*_T1w_segm-graymatter_space-Ixi549Space_modulated-on_probability.nii.gz",
                 ),
                 "description": "graymatter tissue segmented in T1w MRI in Ixi549 space",
                 "needed_pipeline": "t1-volume-tissue-segmentation",
             }
-        elif self.parameters["orig_input_data"] == "pet-volume":
+        elif self.parameters["orig_input_data_ml"] == "pet-volume":
             if not (
                 self.parameters["acq_label"]
                 and self.parameters["suvr_reference_region"]
             ):
                 raise ValueError(
                     f"Missing value(s) in parameters from pet-volume pipeline. Given values:\n"
                     f"- acq_label: {self.parameters['acq_label']}\n"
@@ -111,15 +111,15 @@
                 suvr_reference_region=self.parameters["suvr_reference_region"],
                 use_brainmasked_image=False,
                 use_pvc_data=self.parameters["use_pvc_data"],
                 fwhm=0,
             )
         else:
             raise ValueError(
-                f"Image type {self.parameters['orig_input_data']} unknown."
+                f"Image type {self.parameters['orig_input_data_ml']} unknown."
             )
 
         try:
             input_image, _ = clinica_file_reader(
                 self.subjects,
                 self.sessions,
                 self.caps_directory,
@@ -196,15 +196,15 @@
             iterfield=["input_image"],
         )
         heat_solver_equation.inputs.FWHM = self.parameters["fwhm"]
 
         datasink = npe.Node(nio.DataSink(), name="sinker")
         datasink.inputs.base_directory = self.caps_directory
         datasink.inputs.parameterization = True
-        if self.parameters["orig_input_data"] == "t1-volume":
+        if self.parameters["orig_input_data_ml"] == "t1-volume":
             datasink.inputs.regexp_substitutions = [
                 (
                     r"(.*)/regularized_image/.*/(.*(sub-(.*)_ses-(.*))_T1w(.*)_probability(.*))$",
                     r"\1/subjects/sub-\4/ses-\5/machine_learning/input_spatial_svm/group-"
                     + self.parameters["group_label"]
                     + r"/\3_T1w\6_spatialregularization\7",
                 ),
@@ -222,15 +222,15 @@
                     + self.parameters["group_label"]
                     + r"/machine_learning/input_spatial_svm/group-"
                     + self.parameters["group_label"]
                     + r"_space-Ixi549Space_gram.npy",
                 ),
             ]
 
-        elif self.parameters["orig_input_data"] == "pet-volume":
+        elif self.parameters["orig_input_data_ml"] == "pet-volume":
             datasink.inputs.regexp_substitutions = [
                 (
                     r"(.*)/regularized_image/.*/(.*(sub-(.*)_ses-(.*))_(task.*)_pet(.*))$",
                     r"\1/subjects/sub-\4/ses-\5/machine_learning/input_spatial_svm/group-"
                     + self.parameters["group_label"]
                     + r"/\3_\6_spatialregularization\7",
                 ),
```

### Comparing `clinica-0.7.4/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py` & `clinica-0.7.5/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_linear/pet_linear_cli.py` & `clinica-0.7.5/clinica/pipelines/pet_linear/pet_linear_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,36 +11,38 @@
 @clinica_pipeline
 @click.command(name=pipeline_name)
 @cli_param.argument.bids_directory
 @cli_param.argument.caps_directory
 @cli_param.argument.acq_label
 @cli_param.argument.suvr_reference_region
 @cli_param.option_group.pipeline_specific_options
-@cli_param.option_group.option(
+@cli_param.option.option(
     "-ui",
     "--uncropped_image",
     is_flag=True,
     help="Do not crop the image with template (cropped image are suggested for using with DL models)",
 )
-@cli_param.option_group.option(
+@cli_param.option.option(
     "--save_pet_in_t1w_space",
     is_flag=True,
     help="Save the PET image in the T1w space computed in the intermediate step of the pipeline",
 )
+@cli_param.option.random_seed
 @cli_param.option_group.common_pipelines_options
 @cli_param.option.subjects_sessions_tsv
 @cli_param.option.working_directory
 @cli_param.option.n_procs
 def cli(
     bids_directory: str,
     caps_directory: str,
     acq_label: str,
     suvr_reference_region: str,
     uncropped_image: bool = False,
     save_pet_in_t1w_space: bool = False,
+    random_seed: Optional[int] = None,
     subjects_sessions_tsv: Optional[str] = None,
     working_directory: Optional[str] = None,
     n_procs: Optional[int] = None,
 ) -> None:
     """Affine registration of PET images to the MNI standard space.
 
        ACQ_LABEL corresponds the label given to the PET acquisition, specifying the tracer used.
@@ -60,14 +62,15 @@
     from .pet_linear_pipeline import PETLinear
 
     parameters = {
         "acq_label": acq_label,
         "suvr_reference_region": suvr_reference_region,
         "uncropped_image": uncropped_image,
         "save_PETinT1w": save_pet_in_t1w_space,
+        "random_seed": random_seed,
     }
 
     pipeline = PETLinear(
         bids_directory=bids_directory,
         caps_directory=caps_directory,
         tsv_file=subjects_sessions_tsv,
         base_dir=working_directory,
```

### Comparing `clinica-0.7.4/clinica/pipelines/pet_linear/pet_linear_pipeline.py` & `clinica-0.7.5/clinica/pipelines/pet_linear/pet_linear_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,17 @@
 
         ants_applytransform_nonlinear_node = npe.Node(
             name="antsApplyTransformNonLinear", interface=ants.ApplyTransforms()
         )
         ants_applytransform_nonlinear_node.inputs.dimension = 3
         ants_applytransform_nonlinear_node.inputs.reference_image = self.ref_template
 
+        if random_seed := self.parameters.get("random_seed", None):
+            ants_registration_nonlinear_node.inputs.random_seed = random_seed
+
         normalize_intensity_node = npe.Node(
             name="intensityNormalization",
             interface=nutil.Function(
                 function=utils.suvr_normalization,
                 input_names=["input_img", "norm_img", "ref_mask"],
                 output_names=["output_img"],
             ),
@@ -376,15 +379,16 @@
                 # STEP 2
                 (ants_registration_node, concatenate_node, [("out_matrix", "pet_to_t1w_transform")]),
                 (self.input_node, concatenate_node, [("t1w_to_mni", "t1w_to_mni_transform")]),
                 (self.input_node, ants_applytransform_node, [("pet", "input_image")]),
                 (concatenate_node, ants_applytransform_node, [("transforms_list", "transforms")]),
                 # STEP 3
                 (self.input_node, ants_registration_nonlinear_node, [("t1w", "moving_image")]),
-                (ants_registration_nonlinear_node, ants_applytransform_nonlinear_node, [("reverse_forward_transforms", "transforms")]),
+                (ants_registration_nonlinear_node, ants_applytransform_nonlinear_node,
+                 [("reverse_forward_transforms", "transforms")]),
                 (ants_applytransform_node, ants_applytransform_nonlinear_node, [("output_image", "input_image")]),
                 (ants_applytransform_node, normalize_intensity_node, [("output_image", "input_img")]),
                 (ants_applytransform_nonlinear_node, normalize_intensity_node, [("output_image", "norm_img")]),
                 # Connect to DataSink
                 (ants_registration_node, self.output_node, [("out_matrix", "affine_mat")]),
                 (normalize_intensity_node, self.output_node, [("output_img", "suvr_pet")]),
                 (self.input_node, print_end_message, [("pet", "pet")]),
```

### Comparing `clinica-0.7.4/clinica/pipelines/pet_linear/pet_linear_utils.py` & `clinica-0.7.5/clinica/pipelines/pet_linear/pet_linear_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_surface/applyInverseDeformationField.m` & `clinica-0.7.5/clinica/pipelines/pet_surface/applyInverseDeformationField.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_surface/info.json` & `clinica-0.7.5/clinica/pipelines/pet_surface/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_cli.py` & `clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py` & `clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_pipeline.py` & `clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_surface/pet_surface_utils.py` & `clinica-0.7.5/clinica/pipelines/pet_surface/pet_surface_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_volume/pet_volume_cli.py` & `clinica-0.7.5/clinica/pipelines/pet_volume/pet_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_volume/pet_volume_pipeline.py` & `clinica-0.7.5/clinica/pipelines/pet_volume/pet_volume_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/pet_volume/pet_volume_utils.py` & `clinica-0.7.5/clinica/pipelines/pet_volume/pet_volume_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_surface/_inputs.py` & `clinica-0.7.5/clinica/pipelines/statistics_surface/_inputs.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_surface/_model.py` & `clinica-0.7.5/clinica/pipelines/statistics_surface/_model.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_surface/clinica_surfstat.py` & `clinica-0.7.5/clinica/pipelines/statistics_surface/clinica_surfstat.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_surface/statistics_surface_cli.py` & `clinica-0.7.5/clinica/pipelines/statistics_surface/statistics_surface_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_surface/statistics_surface_pipeline.py` & `clinica-0.7.5/clinica/pipelines/statistics_surface/statistics_surface_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_surface/statistics_surface_utils.py` & `clinica-0.7.5/clinica/pipelines/statistics_surface/statistics_surface_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume/statistics_volume_cli.py` & `clinica-0.7.5/clinica/pipelines/statistics_volume/statistics_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py` & `clinica-0.7.5/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                     "contrast",
                     "idx_group1",
                     "idx_group2",
                     "file_list",
                     "template_file",
                 ],
                 output_names=["script_file", "covariates"],
-                function=utils.model_creation,
+                function=utils.write_matlab_model,
             ),
             name="model_creation",
             overwrite=True,
         )
         model_creation.inputs.tsv = self.tsv_file
         model_creation.inputs.contrast = self.parameters["contrast"]
         model_creation.inputs.template_file = join(
@@ -363,41 +363,41 @@
         )
 
         # 2. Model estimation
         model_estimation = npe.Node(
             nutil.Function(
                 input_names=["mat_file", "template_file"],
                 output_names=["script_file"],
-                function=utils.estimate,
+                function=utils.clean_template_file,
             ),
             name="model_estimation",
         )
         model_estimation.inputs.template_file = join(
             dirname(__file__), "template_model_estimation.m"
         )
 
         # 3. Contrast
         model_contrast = npe.Node(
             nutil.Function(
                 input_names=["mat_file", "template_file", "covariates", "class_names"],
                 output_names=["script_file"],
-                function=utils.contrast,
+                function=utils.clean_spm_contrast_file,
             ),
             name="model_contrast",
         )
         model_contrast.inputs.template_file = join(
             dirname(__file__), "template_model_contrast.m"
         )
 
         # 4. Results
         model_result_no_correction = npe.Node(
             nutil.Function(
                 input_names=["mat_file", "template_file", "method", "threshold"],
                 output_names=["script_file"],
-                function=utils.results,
+                function=utils.clean_spm_result_file,
             ),
             name="model_result_no_correction",
         )
         model_result_no_correction.inputs.template_file = join(
             dirname(__file__), "template_model_results.m"
         )
 
@@ -425,15 +425,15 @@
                     "spm_figures",
                     "variance_of_error",
                     "resels_per_voxels",
                     "mask",
                     "regression_coeff",
                     "contrasts",
                 ],
-                function=utils.read_output,
+                function=utils.copy_and_rename_spm_output_files,
             ),
             name="read_output_node",
         )
         read_output_node.inputs.group_label = self.parameters["group_label"]
         read_output_node.inputs.fwhm = self.parameters["full_width_at_half_maximum"]
         read_output_node.inputs.measure = self.parameters["measure_label"]
```

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_contrast.m` & `clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_contrast.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_creation.m` & `clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_creation.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume/template_model_results.m` & `clinica-0.7.5/clinica/pipelines/statistics_volume/template_model_results.m`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py` & `clinica-0.7.5/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py` & `clinica-0.7.5/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,35 +162,35 @@
         produce_fig_FWE_cluster_correction.inputs.c_thresh = self.parameters["FWEc"]
         produce_fig_FDR_cluster_correction.inputs.c_thresh = self.parameters["FDRc"]
         # fmt: on
 
         save_fig_peak_correction_FWE = npe.Node(
             name="save_figure_peak_correction_FWE",
             interface=nutil.Function(
-                input_names=["t_map", "figs", "name"],
+                input_names=["t_map", "figs", "correction_name"],
                 output_names=[],
                 function=utils.generate_output,
             ),
         )
-        save_fig_peak_correction_FWE.inputs.name = "FWEp"
+        save_fig_peak_correction_FWE.inputs.correction_name = "FWEp"
 
         save_fig_peak_correction_FDR = save_fig_peak_correction_FWE.clone(
             name="save_fig_peak_correction_FDR"
         )
-        save_fig_peak_correction_FDR.inputs.name = "FDRp"
+        save_fig_peak_correction_FDR.inputs.correction_name = "FDRp"
 
         save_fig_cluster_correction_FWE = save_fig_peak_correction_FWE.clone(
             name="save_fig_cluster_correction_FWE"
         )
-        save_fig_cluster_correction_FWE.inputs.name = "FWEc"
+        save_fig_cluster_correction_FWE.inputs.correction_name = "FWEc"
 
         save_fig_cluster_correction_FDR = save_fig_peak_correction_FWE.clone(
             name="save_fig_cluster_correction_FDR"
         )
-        save_fig_cluster_correction_FDR.inputs.name = "FDRc"
+        save_fig_cluster_correction_FDR.inputs.correction_name = "FDRc"
 
         # Connection
         # ==========
         # fmt: off
         self.connect(
             [
                 (self.input_node, peak_correction_FWE, [("t_map", "t_map")]),
```

### Comparing `clinica-0.7.4/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py` & `clinica-0.7.5/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,29 @@
-def peak_correction(t_map, t_threshold, output_name=None):
-    """
-    Threshold the t_map with t_threshold. Pixel intensities that are less than t_threshold are set to 0, other values
-    are left unchanged.
+from typing import List
+
 
-    Args:
-        t_map: (str) path to t-statistics nifti map
-        t_threshold: (float) threshold on t value
-        output_name: (str) optional output name
+def peak_correction(t_map: str, t_threshold: float, output_name: str = None) -> str:
+    """Threshold the t_map with t_threshold.
+
+    Pixel intensities that are less than t_threshold are set to 0, other values
+    are left unchanged.
 
-    Returns:
-        path to the generated file.
+    Parameters
+    ----------
+    t_map: str
+        Path to t-statistics nifti map
+    t_threshold: float
+        Threshold on t value
+    output_name: str, optional
+        Optional output name
+
+    Returns
+    -------
+    str:
+        Path to the generated file.
     """
     from os.path import abspath, basename, join
 
     import nibabel as nib
 
     original_nifti = nib.load(t_map)
     data = original_nifti.get_fdata(dtype="float32")
@@ -25,26 +35,37 @@
         filename = output_name
     else:
         filename = join("./peak_corrected_" + str(t_threshold) + basename(t_map))
     nib.save(new_data, filename)
     return abspath(filename)
 
 
-def cluster_correction(t_map, t_thresh, c_thresh, output_name=None):
-    """
-    Performs cluster correction. First t_map is thresholded with t_thresh (like in peak_correction()). Then, clusters
+def cluster_correction(
+    t_map: str, t_thresh: float, c_thresh: int, output_name: str = None
+) -> str:
+    """Performs cluster correction.
+
+    First t_map is thresholded with t_thresh (like in peak_correction()). Then, clusters
     that have a size less than c_thresh are removed
-    Args:
-        t_map: (str) path to t-statistics nifti map
-        t_thresh: (float) threshold on t value
-        c_thresh: (int) minimal size of clusters after thresholding
-        output_name: (str) optional output name
 
-    Returns:
-        path to the generated file.
+    Parameters
+    ----------
+    t_map: str
+        Path to t-statistics nifti map
+    t_thresh: float
+        Threshold on t value
+    c_thresh: int
+        Minimal size of clusters after thresholding
+    output_name: str, optional
+        Optional output name
+
+    Returns
+    -------
+    str:
+        Path to the generated file.
     """
     from os.path import abspath, basename, join
 
     import nibabel as nib
     import numpy as np
     from scipy.ndimage.measurements import label
 
@@ -75,27 +96,42 @@
             + str(c_thresh)
             + basename(t_map)
         )
     nib.save(new_data, filename)
     return abspath(filename)
 
 
-def produce_figures(nii_file, template, type_of_correction, t_thresh, c_thresh, n_cuts):
-    """
-    Produce the output figures
-
-    Args:
-        nii_file: (str) path to the nifti file (generated at previous steps)
-        template: (str) path to template used for the stat map plot
-        type_of_correction: (str) Can be either FWE or FDR (used only in potential figure titles)
-        t_thresh: (str) t value threshold used (used only in potential figure titles)
-        c_thresh: (int) cluster minimal size used (used only in potential figure titles)
-        n_cuts: (int) number of cuts in fig
-
-    Returns:
+def produce_figures(
+    nii_file: str,
+    template: str,
+    type_of_correction: str,
+    t_thresh: str,
+    c_thresh: int,
+    n_cuts: int,
+) -> list:
+    """Produce the output figures.
+
+    Parameters
+    ----------
+    nii_file: str
+        Path to the nifti file (generated at previous steps)
+    template: str
+        Path to template used for the stat map plot
+    type_of_correction: str
+        Can be either FWE or FDR (used only in potential figure titles)
+    t_thresh: str
+        T value threshold used (used only in potential figure titles)
+    c_thresh: int
+        Cluster minimal size used (used only in potential figure titles)
+    n_cuts: int
+        Number of cuts in fig
+
+    Returns
+    -------
+    list of string:
         List of path to image files: glass brain, statmap along x, statmap along y, statmap along z
     """
     from os.path import abspath
 
     import numpy as np
     from nilearn import plotting
 
@@ -151,61 +187,46 @@
         abspath("./glass_brain.png"),
         abspath("./statmap_x.png"),
         abspath("./statmap_y.png"),
         abspath("./statmap_z.png"),
     ]
 
 
-def generate_output(t_map, figs, name):
-    """
-        Produce output
-    Args:
-        t_map: (str) path to t-map on which whole pipeline was based
-        figs: (list of str) paths to figs to save
-        name: (str) name of the correction (ex: cluster_correction_FWE)
+def generate_output(t_map: str, figs: list, correction_name: str) -> None:
+    """Extract the output generated and copy it to the output folder
 
-    Returns:
-        Nothing
+    Parameters
+    ----------
+    t_map: str
+        Path to t-map on which whole pipeline was based
+    figs: list of str
+        Paths to figs to save
+    correction_name: str
+        Name of the correction (ex: cluster_correction_FWE)
     """
     from os import makedirs
     from os.path import basename, dirname, join, splitext
     from shutil import copyfile
 
     # Will extract group-GroupTest_AD-lt-CN_measure-fdg_fwhm-8_TStatistics from TStatistics file
     t_map_basename = splitext(basename(t_map))[0]
 
-    out_folder = join(dirname(t_map), t_map_basename.replace("TStatistics", name))
-    makedirs(out_folder)
-    copyfile(
-        figs[0],
-        join(
-            out_folder,
-            t_map_basename.replace("TStatistics", "desc-" + name + "_GlassBrain.png"),
-        ),
-    )
-    copyfile(
-        figs[1],
-        join(
-            out_folder,
-            t_map_basename.replace(
-                "TStatistics", "desc-" + name + "_axis-x_TStatistics.png"
-            ),
-        ),
+    out_folder = join(
+        dirname(t_map), t_map_basename.replace("TStatistics", correction_name)
     )
-    copyfile(
-        figs[2],
-        join(
-            out_folder,
-            t_map_basename.replace(
-                "TStatistics", "desc-" + name + "_axis-y_TStatistics.png"
-            ),
-        ),
-    )
-    copyfile(
-        figs[3],
-        join(
-            out_folder,
-            t_map_basename.replace(
-                "TStatistics", "desc-" + name + "_axis-z_TStatistics.png"
+    makedirs(out_folder)
+    suffixes = (
+        "GlassBrain.png",
+        "axis-x_TStatistics.png",
+        "axis-y_TStatistics.png",
+        "axis-z_TStatistics.png",
+    )
+    for fig, suffix in zip(figs, suffixes):
+        copyfile(
+            fig,
+            join(
+                out_folder,
+                t_map_basename.replace(
+                    "TStatistics", f"desc-{correction_name}_{suffix}"
+                ),
             ),
-        ),
-    )
+        )
```

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,304 +1,216 @@
-def init_input_node(caps_dir, participant_id, session_id, long_id, output_dir):
-    """Initialize the pipeline."""
+def init_input_node(caps_dir, participant_id, list_session_ids, output_dir):
+    """Initialize the pipeline.
+
+    This function will create folders and symbolic links in SUBJECTS_DIR env variable for upcoming run of recon-all.
+
+    Note (@alexis-g-icm):
+        There currently (as of 22 Feb 2019) is a bug in FreeSurfer recon-all -base, which in some cases (e.g., only one
+        time point), will crash as it's trying to write lines too long for the shell to handle. This is caused by
+        the path to FreeSurfer SUBJECT_DIR being too long itself.
+
+    The current function works around this issue by checking if there only is one session associated to a subject, and
+    in that case, putting the SUBJECT_DIR inside the system temporary folder so that its path is as short as possible.
+    """
     import os
-    import platform
     from tempfile import mkdtemp
 
-    from clinica.utils.longitudinal import read_sessions
+    from clinica.compat import errno
+    from clinica.utils.longitudinal import get_long_id
     from clinica.utils.stream import cprint
     from clinica.utils.ux import print_begin_image
 
     # Extract <image_id>
-    image_id = "{0}_{1}_{2}".format(participant_id, session_id, long_id)
+    long_id = get_long_id(list_session_ids)
+    image_id = f"{participant_id}_{long_id}"
 
     # Create SUBJECTS_DIR for recon-all (otherwise, the command won't run)
-    if platform.system().lower().startswith("darwin"):
-        # Special case: On macOS, 'recon-all -long' can failed if the $SUBJECTS_DIR is too long
+    if len(list_session_ids) == 1:
+        # Special case: When only one time point is used, 'recon-all -base' can failed
+        # if the $SUBJECTS_DIR is too long ('Word too long.' error).
         # To circumvent this issue, we create a sym link in $(TMP) so that $SUBJECTS_DIR is a short path
         subjects_dir = mkdtemp()
         cprint(
             msg=(
-                f"Needs to create a $SUBJECTS_DIR folder "
-                f"in {subjects_dir} for {image_id.replace('_', ' | ')} (macOS case)."
+                f"{image_id.replace('_', ' | ')} has only one time point. "
+                f"Needs to create a $SUBJECTS_DIR folder in {subjects_dir}"
             ),
             lvl="warning",
         )
     else:
         subjects_dir = os.path.join(output_dir, image_id)
 
     os.makedirs(subjects_dir, exist_ok=True)
 
-    # Create symbolic link containing cross-sectional segmentation(s) in SUBJECTS_DIR so that recon-all can run
-    for s_id in read_sessions(caps_dir, participant_id, long_id):
+    # Create symbolic links containing cross-sectional segmentation(s) in SUBJECTS_DIR so that recon-all can run
+    for session_id in list_session_ids:
         cross_sectional_path = os.path.join(
             caps_dir,
             "subjects",
             participant_id,
-            s_id,
+            session_id,
             "t1",
             "freesurfer_cross_sectional",
-            f"{participant_id}_{s_id}",
-        )
-        os.symlink(
-            cross_sectional_path,
-            os.path.join(subjects_dir, f"{participant_id}_{s_id}"),
+            f"{participant_id}_{session_id}",
         )
+        try:
+            os.symlink(
+                cross_sectional_path,
+                os.path.join(subjects_dir, f"{participant_id}_{session_id}"),
+            )
+        except FileExistsError as e:
+            if e.errno != errno.EEXIST:  # EEXIST: folder already exists
+                raise e
 
-    # Create symbolic links containing unbiased template in SUBJECTS_DIR so that recon-all can run
-    template_path = os.path.join(
-        caps_dir,
-        "subjects",
-        participant_id,
-        long_id,
-        "freesurfer_unbiased_template",
-        f"{participant_id}_{long_id}",
-    )
-    os.symlink(template_path, os.path.join(subjects_dir, f"{participant_id}_{long_id}"))
+    # Prepare arguments for recon-all.
+    flags = ""
+    for session_id in list_session_ids:
+        flags += f" -tp {participant_id}_{session_id}"
 
     print_begin_image(image_id)
 
-    return subjects_dir
+    return image_id, subjects_dir, flags
 
 
-def run_recon_all_long(subjects_dir, participant_id, session_id, long_id, directive):
-    """Run recon-all to create a longitudinal correction of a time point.
+def run_recon_all_base(subjects_dir, subject_id, flags, directive):
+    """Run recon-all to create an unbiased template from all time points.
 
     Note:
-    Longitudinal correction with FreeSurfer expects arguments to follow this syntax:
-    recon-all -long <tpN_id> <template_id> -all; e.g.: recon-all -long sub-CLNC01_ses-M000 sub-CLNC01_long-M000M018 -all
+    Unbiased template creation with FreeSurfer expects arguments to follow this syntax:
+    recon-all -base <template_id> -tp <tp1_id> -tp <tp2_id> ... -all
 
-    Currently, Nipype does not provide interface for "recon-all -long" case. As a result, ReconAll interface should be
+    Currently, Nipype does not provide interface for "recon-all -base" case. As a result, ReconAll interface should be
     modified to handle this situation. In the meantime, the arguments of this function follows ReconAll.inputs names
     namely:
-        - "-long <tpN_id> <template_id>" is likely to be fed to ReconAll.inputs.args
+        - "-base <template_id>" is likely to be fed to ReconAll.inputs.subject_id or new input (e.g. template_id?)
+        - "-tp <tp1_id> -tp <tp2_id> ..." is likely to  be fed to ReconAll.inputs.args
         - "-all" will be fed to ReconAll.inputs.directive
 
-    Folder containing the longitudinal correction has the following convention:
-    <tpN_id>.long.<template_id>; e.g.: sub-CLNC01_ses-M000.long.sub-CLNC01_long-M000M018
-    which is automatically generated by FreeSurfer.
-
-    This folder name is likely to be retrieved in ReconAll.outputs.subject_id.
-
     See official documentation (https://surfer.nmr.mgh.harvard.edu/fswiki/LongitudinalProcessing) for details.
     """
     import subprocess
 
-    # Prepare arguments for recon-all.
-    flags = " -long {0}_{1} {0}_{2} ".format(participant_id, session_id, long_id)
-
-    recon_all_long_command = "recon-all {0} -sd {1} {2}".format(
-        flags, subjects_dir, directive
+    recon_all_base_command = "recon-all -base {0} {1} -sd {2} {3}".format(
+        subject_id, flags, subjects_dir, directive
     )
-    subprocess_run_recon_all_long = subprocess.run(
-        recon_all_long_command,
+    subprocess_run_recon_all_base = subprocess.run(
+        recon_all_base_command,
         shell=True,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
-    if subprocess_run_recon_all_long.returncode != 0:
-        raise ValueError("recon-all -long failed, returned non-zero code")
+    if subprocess_run_recon_all_base.returncode != 0:
+        raise ValueError("recon-all -base failed, returned non-zero code")
 
-    subject_id = "{0}_{1}.long.{0}_{2}".format(participant_id, session_id, long_id)
-
-    return subject_id
-
-
-def write_tsv_files(subjects_dir, subject_id):
-    """Generate statistics TSV files in `subjects_dir`/regional_measures folder for `subject_id`.
-
-    Notes:
-        We do not need to check the line "finished without error" in scripts/recon-all.log.
-        If an error occurs, it will be detected by Nipype and the next nodes (i.e.
-        write_tsv_files will not be called).
-    """
-    import os
-
-    from clinica.utils.freesurfer import (
-        extract_image_id_from_longitudinal_segmentation,
-        generate_regional_measures,
-    )
-    from clinica.utils.stream import cprint
-
-    image_id = extract_image_id_from_longitudinal_segmentation(subject_id)
-    str_image_id = (
-        image_id.participant_id + "_" + image_id.session_id + "_" + image_id.long_id
-    )
-    if os.path.isfile(os.path.join(subjects_dir, subject_id, "mri", "aparc+aseg.mgz")):
-        generate_regional_measures(subjects_dir, subject_id)
-    else:
-        cprint(
-            msg=(
-                f"{str_image_id.replace('_', ' | ')} does not contain mri/aseg+aparc.mgz file. "
-                "Creation of regional_measures/ folder will be skipped."
-            ),
-            lvl="warning",
-        )
     return subject_id
 
 
 def move_subjects_dir_to_source_dir(subjects_dir, source_dir, subject_id):
-    """Move content of `subjects_dir`/`subject_id` to `source_dir`.
+    """
+    Move content of `subjects_dir`/`subject_id` to `source_dir`.
 
-    This function will move content of `subject_id` if recon-all has run
-    in $(TMP). This happens when FreeSurfer is run on macOS. Content of
-    $(TMP)/`subject_id` is copied to `source_dir` before the deletion of $(TMP).
+    This function will move content of `subject_id` if recon-all has run in $(TMP). This happens when only
+    one time point is used. Content of $(TMP)/`subject_id` is copied to `source_dir` before the deletion of $(TMP).
 
     Args:
-        subjects_dir: $(TMP), if segmentation was performed on macOS,
+        subjects_dir: $(TMP), if segmentation was performed on 1 time point,
             <base_dir>/<Pipeline.Name>/ReconAll/`subject_id` otherwise
         source_dir: <base_dir>/<Pipeline.Name>/ReconAll folder
-        subject_id: Subject ID (e.g. "sub-CLNC01_ses-M000.long.sub-CLNC01_long-M000M018")
+        subject_id: Subject ID (e.g. "sub-CLNC01_ses-M000" or "sub-CLNC01_ses-M000M018")
 
     Returns:
         subject_id for node connection with Nipype
     """
     import os
     import shutil
 
-    from clinica.utils.freesurfer import extract_image_id_from_longitudinal_segmentation
     from clinica.utils.stream import cprint
 
-    image_id = extract_image_id_from_longitudinal_segmentation(subject_id)
-    str_image_id = (
-        image_id.participant_id + "_" + image_id.session_id + "_" + image_id.long_id
-    )
-
     if source_dir not in subjects_dir:
         shutil.copytree(
             src=os.path.join(subjects_dir, subject_id),
-            dst=os.path.join(source_dir, str_image_id, subject_id),
-            symlinks=True,
-        )
-        shutil.copytree(
-            src=os.path.join(subjects_dir, "regional_measures"),
-            dst=os.path.join(source_dir, str_image_id, "regional_measures"),
+            dst=os.path.join(source_dir, subject_id, subject_id),
             symlinks=True,
         )
         shutil.rmtree(subjects_dir)
         cprint(
             msg=(
                 f"Segmentation of {subject_id.replace('_', ' | ')} "
                 f"has moved to working directory and $SUBJECTS_DIR folder ({subjects_dir}) was deleted."
             ),
             lvl="warning",
         )
 
     return subject_id
 
 
-def save_to_caps(source_dir, subject_id, caps_dir, overwrite_caps=False):
-    """Save `source_dir`/`subject_id`/ to CAPS folder.
+def save_to_caps(
+    source_dir, image_id, list_session_ids, caps_dir, overwrite_caps=False
+):
+    """Save `source_dir`/`image_id`/ to CAPS folder.
 
     This function copies FreeSurfer segmentation and regional_measures folder of `source_dir`/`image_id`/ to
-    `caps_dir`/subjects/<participant_id>/<session_id>/<long_id>/t1_freesurfer_longitudinal/
-    where `image_id` = <participant_id>_<session_id>_<long_id>.
+    `caps_dir`/subjects/<participant_id>/<long_id>/freesurfer_unbiased_template/
+    where `image_id` = <participant_id>_<long_id>.
 
     The `source_dir`/`image_id`/ folder should contain the following elements:
         - fsaverage, lh.EC_average and rh.EC_average symbolic links automatically generated by recon-all
         - symbolic links to cross-sectional segmentation(s) and unbiased template needed for recon-all
-        - <participant_id>_<session_id>.long.<participant_id>_<long_id>/ folder containing the FreeSurfer segmentation
-        - regional_measures/ folder containing TSV files
+        - <participant_id>_<long_id>/ folder containing the FreeSurfer segmentation
 
     Notes:
         We do not need to check the line "finished without error" in scripts/recon-all.log.
         If an error occurs, it will be detected by Nipype and the next nodes (i.e. save_to_caps will not be called).
     """
     import os
     import shutil
 
-    from clinica.utils.freesurfer import extract_image_id_from_longitudinal_segmentation
+    from clinica.utils.longitudinal import save_long_id
     from clinica.utils.stream import cprint
     from clinica.utils.ux import print_end_image
 
-    image_id = extract_image_id_from_longitudinal_segmentation(subject_id)
-    participant_id = image_id.participant_id
-    session_id = image_id.session_id
-    long_id = image_id.long_id
-    str_image_id = (
-        image_id.participant_id + "_" + image_id.session_id + "_" + image_id.long_id
-    )
+    participant_id = image_id.split("_")[0]
+    long_id = image_id.split("_")[1]
 
     destination_dir = os.path.join(
         os.path.expanduser(caps_dir),
         "subjects",
         participant_id,
-        session_id,
-        "t1",
         long_id,
-        "freesurfer_longitudinal",
+        "freesurfer_unbiased_template",
+    )
+
+    # Save <long_id>_sessions.tsv to retrieve sessions used to generate <long_id>
+    sessions_tsv_path = os.path.join(
+        os.path.expanduser(caps_dir), "subjects", participant_id, long_id
     )
+    if not os.path.isfile(os.path.join(sessions_tsv_path, f"{long_id}_sessions.tsv")):
+        save_long_id(list_session_ids, sessions_tsv_path, f"{long_id}_sessions.tsv")
 
     # Save FreeSurfer segmentation
-    representative_file = os.path.join(subject_id, "mri", "aparc+aseg.mgz")
+    representative_file = os.path.join(image_id, "mri", "aparc+aseg.mgz")
     representative_source_file = os.path.join(
-        os.path.expanduser(source_dir), str_image_id, representative_file
+        os.path.expanduser(source_dir), image_id, representative_file
     )
     representative_destination_file = os.path.join(destination_dir, representative_file)
     if os.path.isfile(representative_source_file):
         if os.path.isfile(representative_destination_file):
             if overwrite_caps:
                 shutil.rmtree(destination_dir)
                 shutil.copytree(
-                    src=os.path.join(source_dir, subject_id, subject_id),
-                    dst=os.path.join(destination_dir, subject_id),
-                    symlinks=True,
-                )
-                shutil.copytree(
-                    src=os.path.join(source_dir, subject_id, "regional_measures"),
-                    dst=os.path.join(destination_dir, "regional_measures"),
+                    src=os.path.join(source_dir, image_id, image_id),
+                    dst=os.path.join(destination_dir, image_id),
                     symlinks=True,
                 )
         else:
             shutil.copytree(
-                src=os.path.join(source_dir, str_image_id, subject_id),
-                dst=os.path.join(destination_dir, subject_id),
-                symlinks=True,
-            )
-            shutil.copytree(
-                src=os.path.join(source_dir, str_image_id, "regional_measures"),
-                dst=os.path.join(destination_dir, "regional_measures"),
+                src=os.path.join(source_dir, image_id, image_id),
+                dst=os.path.join(destination_dir, image_id),
                 symlinks=True,
             )
-        print_end_image(str_image_id)
+        print_end_image(image_id)
     else:
         cprint(
-            msg=f"{subject_id.replace('_', ' | ')}  does not contain mri/aseg+aparc.mgz file. Copy will be skipped.",
+            msg=f"{image_id.replace('_', ' | ')}  does not contain mri/aseg+aparc.mgz file. Copy will be skipped.",
             lvl="warning",
         )
-
-    return str_image_id
-
-
-def get_processed_images(caps_directory, part_ids, sess_ids, long_ids, atlas=False):
-    """
-    Extract image IDs (e.g. ["sub-CLNC01_ses-M000_long-M000M018", "sub-CLNC01_ses-M018_long-M000M018"]) of outputs
-    already processed by T1FreeSurferLongitudinalCorrection pipeline.
-    """
-    import os
-
-    image_ids = []
-    if os.path.isdir(caps_directory):
-        for (participant_id, session_id, long_id) in zip(part_ids, sess_ids, long_ids):
-            output_file_pre = os.path.join(
-                os.path.expanduser(caps_directory),
-                "subjects",
-                participant_id,
-                session_id,
-                "t1",
-                long_id,
-                "freesurfer_longitudinal",
-                f"{participant_id}_{session_id}.long.{participant_id}_{long_id}",
-            )
-            if atlas:
-                output_file = os.path.join(
-                    output_file_pre, "stat", "rh.", atlas, ".stats"
-                )
-            else:
-                output_file = os.path.join(
-                    output_file_pre,
-                    "mri",
-                    "aparc+aseg.mgz",
-                )
-            if os.path.isfile(output_file):
-                image_ids.append(f"{participant_id}_{session_id}_{long_id}")
-    return image_ids
+    return image_id
```

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_linear/anat_linear_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_linear/anat_linear_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,18 +217,15 @@
                 (container_path, write_node, [(("container", fix_join, self.name.replace("-", "_")), "container")]),
                 (get_ids, write_node, [("subst_ls", "substitutions")]),
                 (get_ids, write_node, [("image_id_out", "@image_id")]),
                 (self.output_node, write_node, [("outfile_reg", "@outfile_reg")]),
                 (self.output_node, write_node, [("affine_mat", "@affine_mat")]),
             ]
         )
-    
-                    
-            
-        
+
         if not (self.parameters.get("uncropped_image")):
             self.connect(
                 [
                     (self.output_node, write_node, [("outfile_crop", "@outfile_crop")]),
                 ]
             )
         # fmt: on
@@ -270,14 +267,17 @@
         ants_registration_node = npe.Node(
             name="antsRegistrationSynQuick", interface=ants.RegistrationSynQuick()
         )
         ants_registration_node.inputs.fixed_image = self.ref_template
         ants_registration_node.inputs.transform_type = "a"
         ants_registration_node.inputs.dimension = 3
 
+        if random_seed := self.parameters.get("random_seed", None):
+            ants_registration_node.inputs.random_seed = random_seed
+
         # 3. Crop image (using nifti). It uses custom interface, from utils file
 
         cropnifti = npe.Node(
             name="cropnifti",
             interface=nutil.Function(
                 function=crop_nifti,
                 input_names=["input_img", "ref_crop"],
```

### Comparing `clinica-0.7.4/clinica/pipelines/t1_linear/anat_linear_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_linear/anat_linear_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_linear/flair_linear_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_linear/flair_linear_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,37 +15,42 @@
 @cli_param.option_group.pipeline_specific_options
 @cli_param.option_group.option(
     "-ui",
     "--uncropped_image",
     is_flag=True,
     help="Do not crop the image with template (cropped image are suggested for using with DL models)",
 )
+@cli_param.option.random_seed
 @cli_param.option_group.common_pipelines_options
 @cli_param.option.subjects_sessions_tsv
 @cli_param.option.working_directory
 @cli_param.option.n_procs
 def cli(
     bids_directory: str,
     caps_directory: str,
     uncropped_image: bool = False,
+    random_seed: Optional[int] = None,
     subjects_sessions_tsv: Optional[str] = None,
     working_directory: Optional[str] = None,
     n_procs: Optional[int] = None,
 ) -> None:
     """Affine registration of Flair images to the MNI standard space.
 
     https://aramislab.paris.inria.fr/clinica/docs/public/latest/Pipelines/T1_Linear/
     """
     from networkx import Graph
 
     from clinica.utils.ux import print_end_pipeline
 
     from .anat_linear_pipeline import AnatLinear
 
-    parameters = {"uncropped_image": uncropped_image}
+    parameters = {
+        "uncropped_image": uncropped_image,
+        "random_seed": random_seed,
+    }
 
     # Most of the time, you will want to instantiate your pipeline with a
     # BIDS and CAPS directory as inputs:
     pipeline = AnatLinear(
         bids_directory=bids_directory,
         caps_directory=caps_directory,
         tsv_file=subjects_sessions_tsv,
```

### Comparing `clinica-0.7.4/clinica/pipelines/t1_linear/t1_linear_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_linear/t1_linear_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,43 +9,48 @@
 
 
 @clinica_pipeline
 @click.command(name=pipeline_name)
 @cli_param.argument.bids_directory
 @cli_param.argument.caps_directory
 @cli_param.option_group.pipeline_specific_options
-@cli_param.option_group.option(
+@cli_param.option.option(
     "-ui",
     "--uncropped_image",
     is_flag=True,
     help="Do not crop the image with template (cropped image are suggested for using with DL models)",
 )
+@cli_param.option.random_seed
 @cli_param.option_group.common_pipelines_options
 @cli_param.option.subjects_sessions_tsv
 @cli_param.option.working_directory
 @cli_param.option.n_procs
 def cli(
     bids_directory: str,
     caps_directory: str,
     uncropped_image: bool = False,
+    random_seed: Optional[int] = None,
     subjects_sessions_tsv: Optional[str] = None,
     working_directory: Optional[str] = None,
     n_procs: Optional[int] = None,
 ) -> None:
     """Affine registration of T1w images to the MNI standard space.
 
     https://aramislab.paris.inria.fr/clinica/docs/public/latest/Pipelines/T1_Linear/
     """
     from networkx import Graph
 
     from clinica.utils.ux import print_end_pipeline
 
     from .anat_linear_pipeline import AnatLinear
 
-    parameters = {"uncropped_image": uncropped_image}
+    parameters = {
+        "uncropped_image": uncropped_image,
+        "random_seed": random_seed,
+    }
 
     # Most of the time, you will want to instantiate your pipeline with a
     # BIDS and CAPS directory as inputs:
     pipeline = AnatLinear(
         bids_directory=bids_directory,
         caps_directory=caps_directory,
         tsv_file=subjects_sessions_tsv,
```

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume/t1_volume_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume/t1_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py` & `clinica-0.7.5/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/engine.py` & `clinica-0.7.5/clinica/pydra/engine.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/engine_utils.py` & `clinica-0.7.5/clinica/pydra/engine_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/interfaces.py` & `clinica-0.7.5/clinica/pydra/interfaces.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/pet_linear/pet_linear_cli.py` & `clinica-0.7.5/clinica/pydra/pet_linear/pet_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/pet_linear/pipeline.py` & `clinica-0.7.5/clinica/pydra/pet_linear/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from clinica.pydra.engine import clinica_io
 from clinica.pydra.pet_linear.tasks import (
     concatenate_transforms_task,
     crop_nifti_task,
     suvr_normalization_task,
 )
-from clinica.pydra.tasks import download_mni_template, download_ref_template
+from clinica.pydra.tasks import download_mni_template_2009c, download_ref_template
 from clinica.utils.pet import get_suvr_mask
 
 IMAGE_DIMENSION = 3
 
 
 @clinica_io
 def build_core_workflow(name: str = "core", parameters: dict = {}) -> Workflow:
@@ -51,15 +51,15 @@
     wf = Workflow(
         name,
         input_spec=input_spec,
     )
 
     wf.split(("pet", "T1w", "t1w_to_mni"))
 
-    wf.add(download_mni_template(name="download_mni_template"))
+    wf.add(download_mni_template_2009c(name="download_mni_template"))
 
     wf.add(download_ref_template(name="download_ref_template"))
 
     # RegistrationSynQuick by ANTS.
     ants_registration = Nipype1Task(
         name="ants_registration",
         interface=RegistrationSynQuick(),
```

### Comparing `clinica-0.7.4/clinica/pydra/pet_linear/tasks.py` & `clinica-0.7.5/clinica/pydra/pet_linear/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/pet_volume/pet_volume_cli.py` & `clinica-0.7.5/clinica/pydra/pet_volume/pet_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/pet_volume/pipeline.py` & `clinica-0.7.5/clinica/pydra/pet_volume/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,16 @@
         Default={}.
 
     Returns
     -------
     wf : Workflow
         The core workflow.
     """
+    from pydra.tasks import petpvc
+
     from clinica.pydra.shared_workflows.smoothing import build_smoothing_workflow
     from clinica.pydra.utils import sanitize_fwhm
     from clinica.utils.pet import get_suvr_mask
     from clinica.utils.spm import spm_standalone_is_available, use_spm_standalone
 
     if spm_standalone_is_available():
         use_spm_standalone()
@@ -270,39 +272,39 @@
                 pvc_psf_tsv=parameters["pvc_psf_tsv"],
                 pet_filename=wf.lzin.pet,
                 pet_tracer=parameters["acq_label"],
             )
         )
 
         # PET PVC
-        petpvc = Nipype1Task(
-            name="pvc",
-            interface=PETPVC(),
-        )
-        petpvc.inputs.pvc = "RBV"
-        petpvc.inputs.out_file = wf.pet_pvc_name.lzout.pet_pvc_path
-        petpvc.inputs.in_file = wf.coreg_pet_t1.lzout.coregistered_source
-        petpvc.inputs.mask_file = wf.pvc_mask.lzout.out_mask
-        petpvc.inputs.fwhm_x = wf.get_psf_task.lzout.psf_x
-        petpvc.inputs.fwhm_y = wf.get_psf_task.lzout.psf_y
-        petpvc.inputs.fwhm_z = wf.get_psf_task.lzout.psf_z
-        wf.add(petpvc)
+        wf.add(
+            petpvc.PETPVC(
+                name="pvc",
+                pvc_method="RBV",
+                output_image=wf.pet_pvc_name.lzout.pet_pvc_path,
+                input_image=wf.coreg_pet_t1.lzout.coregistered_source,
+                mask_image=wf.pvc_mask.lzout.out_mask,
+                fwhm_x=wf.get_psf_task.lzout.psf_x,
+                fwhm_y=wf.get_psf_task.lzout.psf_y,
+                fwhm_z=wf.get_psf_task.lzout.psf_z,
+            )
+        )
 
         # Spatially normalize PET into MNI
         dartel_mni_reg_pvc = Nipype1Task(
             name="dartel_mni_reg_pvc",
             interface=DARTELNorm2MNI(),
         )
         dartel_mni_reg_pvc.inputs.modulate = False
         dartel_mni_reg_pvc.inputs.fwhm = 0
         dartel_mni_reg_pvc.inputs.flowfield_files = wf.unzip_flow_fields.lzout.out_file
         dartel_mni_reg_pvc.inputs.template_file = (
             wf.unzip_dartel_template.lzout.out_file
         )
-        dartel_mni_reg_pvc.inputs.apply_to_files = wf.pvc.lzout.out_file
+        dartel_mni_reg_pvc.inputs.apply_to_files = wf.pvc.lzout.output_image
         wf.add(dartel_mni_reg_pvc)
 
         # Reslice reference region mask into PET
         reslice_pvc = Nipype1Task(
             name="reslice_pvc",
             interface=Reslice(),
         )
@@ -363,15 +365,15 @@
 
     if parameters["apply_pvc"]:
         output_connections += [
             (
                 "pet_pvc_suvr_masked_smoothed",
                 wf.pvc_smoothing_workflow.lzout.smoothed_files,
             ),
-            ("pet_pvc", wf.pvc.lzout.out_file),
+            ("pet_pvc", wf.pvc.lzout.output_image),
             ("pet_pvc_mni", wf.dartel_mni_reg_pvc.lzout.normalized_files),
             ("pet_pvc_suvr", wf.norm_to_ref_pvc.lzout.suvr_pet_path),
             ("pet_pvc_suvr_masked", wf.apply_mask_pvc.lzout.masked_image_path),
             ("pvc_atlas_statistics", wf.atlas_stats_pvc.lzout.atlas_statistics),
         ]
 
     wf.set_output(output_connections)
```

### Comparing `clinica-0.7.4/clinica/pydra/pet_volume/tasks.py` & `clinica-0.7.5/clinica/pydra/pet_volume/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/query.py` & `clinica-0.7.5/clinica/pydra/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,32 +249,38 @@
                 "needed_pipeline": "t1-volume-tissue-segmentation"
             }
         ]
     }
     """
 
     from clinica.utils.input_files import (
+        custom_pipeline,
+        pet_volume_normalized_suvr_pet,
         t1_volume_dartel_input_tissue,
         t1_volume_deformation_to_template,
         t1_volume_native_tpm,
         t1_volume_native_tpm_in_mni,
+        t1_volume_template_tpm_in_mni,
     )
 
     def t1w_to_mni_transform():
         from clinica.utils.input_files import T1W_TO_MNI_TRANSFORM
 
         return T1W_TO_MNI_TRANSFORM
 
     _query_makers = {
         "tissues": t1_volume_native_tpm,
         "mask_tissues": t1_volume_native_tpm_in_mni,
         "flow_fields": t1_volume_deformation_to_template,
         "pvc_mask_tissues": t1_volume_native_tpm,
         "dartel_input_tissue": t1_volume_dartel_input_tissue,
         "t1w_to_mni": t1w_to_mni_transform,
+        "pet_volume": pet_volume_normalized_suvr_pet,
+        "t1_volume": t1_volume_template_tpm_in_mni,
+        "custom_pipeline": custom_pipeline,
     }
 
 
 class CAPSGroupQuery(CAPSQuery):
     """CAPSGroupQuery class.
 
     This class only holds the mapping between the labels and query makers
@@ -294,21 +300,23 @@
         "description": "T1w template file of group UnitTest",
         "needed_pipeline": "t1-volume or t1-volume-create-dartel"
         }
     }
     """
 
     from clinica.utils.input_files import (
+        custom_group,
         t1_volume_final_group_template,
         t1_volume_i_th_iteration_group_template,
     )
 
     _query_makers = {
         "dartel_template": t1_volume_final_group_template,
         "dartel_iteration_templates": t1_volume_i_th_iteration_group_template,
+        "t_map": custom_group,
     }
 
 
 def query_factory(query: Dict, query_type: str) -> Query:
     """Return the Query instance initialized from passed `query`,
     based on provided `query_type`.
```

### Comparing `clinica-0.7.4/clinica/pydra/shared_workflows/smoothing.py` & `clinica-0.7.5/clinica/pydra/shared_workflows/smoothing.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_freesurfer/cli.py` & `clinica-0.7.5/clinica/pydra/t1_freesurfer/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_freesurfer/pipeline.py` & `clinica-0.7.5/clinica/pydra/t1_freesurfer/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_freesurfer/tasks.py` & `clinica-0.7.5/clinica/pydra/t1_freesurfer/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_linear/t1_linear.py` & `clinica-0.7.5/clinica/pydra/t1_linear/t1_linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pydra
 from nipype.interfaces.ants import N4BiasFieldCorrection, RegistrationSynQuick
 from pydra import Workflow
 from pydra.mark import annotate, task
 
 from clinica.pydra.engine import clinica_io
-from clinica.pydra.tasks import download_mni_template, download_ref_template
+from clinica.pydra.tasks import download_mni_template_2009c, download_ref_template
 
 n4_bias_field_correction = N4BiasFieldCorrection(bspline_fitting_distance=300)
 registration_syn_quick = RegistrationSynQuick(transform_type="a")
 
 
 @task
 @annotate({"return": {"cropped_image": PurePath}})
@@ -50,15 +50,15 @@
         name="Input",
         fields=[("T1w", str, {"mandatory": True})],
         bases=(pydra.specs.BaseSpec,),
     )
 
     wf = Workflow(name, input_spec=input_spec)
 
-    wf.add(download_mni_template(name="download_mni_template"))
+    wf.add(download_mni_template_2009c(name="download_mni_template"))
 
     wf.add(download_ref_template(name="download_ref_template"))
 
     wf.add(
         Nipype1Task(
             name="n4_bias_field_correction",
             interface=n4_bias_field_correction,
```

### Comparing `clinica-0.7.4/clinica/pydra/t1_linear/t1_linear_cli.py` & `clinica-0.7.5/clinica/pydra/t1_linear/t1_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/create_dartel/cli.py` & `clinica-0.7.5/clinica/pydra/t1_volume/create_dartel/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/create_dartel/pipeline.py` & `clinica-0.7.5/clinica/pydra/t1_volume/create_dartel/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/cli.py` & `clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/pipeline.py` & `clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/dartel2mni/tasks.py` & `clinica-0.7.5/clinica/pydra/t1_volume/dartel2mni/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/register_dartel/cli.py` & `clinica-0.7.5/clinica/pydra/t1_volume/register_dartel/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/register_dartel/pipeline.py` & `clinica-0.7.5/clinica/pydra/t1_volume/register_dartel/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/tasks.py` & `clinica-0.7.5/clinica/pydra/t1_volume/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/tissue_segmentation/cli.py` & `clinica-0.7.5/clinica/pydra/t1_volume/tissue_segmentation/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py` & `clinica-0.7.5/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/t1_volume/utils.py` & `clinica-0.7.5/clinica/pydra/t1_volume/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/pydra/tasks.py` & `clinica-0.7.5/clinica/pydra/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,30 @@
         copyfileobj(response, f)
 
     return PurePath(to)
 
 
 @task
 @annotate({"return": {"mni_template_file": PurePath}})
-def download_mni_template() -> PurePath:
+def download_mni_template_2009a() -> PurePath:
+    return _download_mni_template(version="09a")
+
+
+@task
+@annotate({"return": {"mni_template_file": PurePath}})
+def download_mni_template_2009c() -> PurePath:
+    return _download_mni_template(version="09c")
+
+
+def _download_mni_template(version: str) -> PurePath:
     from pathlib import Path
 
     return download_file(
-        url="https://aramislab.paris.inria.fr/files/data/img_t1_linear/mni_icbm152_t1_tal_nlin_sym_09c.nii.gz",
-        to=str(Path.cwd() / "mni_icbm152_t1_tal_nlin_sym_09c.nii.gz"),
+        url=f"https://aramislab.paris.inria.fr/files/data/img_t1_linear/mni_icbm152_t1_tal_nlin_sym_{version}.nii.gz",
+        to=str(Path.cwd() / f"mni_icbm152_t1_tal_nlin_sym_{version}.nii.gz"),
     )
 
 
 @task
 @annotate({"return": {"ref_template_file": PurePath}})
 def download_ref_template() -> PurePath:
     from pathlib import Path
```

### Comparing `clinica-0.7.4/clinica/pydra/utils.py` & `clinica-0.7.5/clinica/pydra/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-AAL2.txt` & `clinica-0.7.5/clinica/resources/atlases/atlas-AAL2.txt`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz` & `clinica-0.7.5/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-AAL2_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-AAL2_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-AICHA.txt` & `clinica-0.7.5/clinica/resources/atlases/atlas-AICHA.txt`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz` & `clinica-0.7.5/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-AICHA_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-AICHA_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-Hammers_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-Hammers_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-JHUTract_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-JHUTract_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-LPBA40_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-LPBA40_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv` & `clinica-0.7.5/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/label_conversion_gtmsegmentation.csv` & `clinica-0.7.5/clinica/resources/label_conversion_gtmsegmentation.csv`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz` & `clinica-0.7.5/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz` & `clinica-0.7.5/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz` & `clinica-0.7.5/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz` & `clinica-0.7.5/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/templates/pipeline_template/README.md.j2` & `clinica-0.7.5/clinica/resources/templates/pipeline_template/README.md.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/templates/pipeline_template/cli.py.j2` & `clinica-0.7.5/clinica/resources/templates/pipeline_template/cli.py.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/templates/pipeline_template/pipeline.py.j2` & `clinica-0.7.5/clinica/resources/templates/pipeline_template/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/resources/templates/pipeline_template/utils.py.j2` & `clinica-0.7.5/clinica/resources/templates/pipeline_template/utils.py.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/atlas.py` & `clinica-0.7.5/clinica/utils/atlas.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/check_dependency.py` & `clinica-0.7.5/clinica/utils/check_dependency.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/exceptions.py` & `clinica-0.7.5/clinica/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/filemanip.py` & `clinica-0.7.5/clinica/utils/filemanip.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Callable, List, Optional, Tuple
 
 
 def _zip_unzip_nii(in_file: str, same_dir: bool, compress: bool):
     import gzip
     import operator
     import shutil
@@ -593,7 +594,32 @@
     from clinica.utils.exceptions import ClinicaException
 
     if "PhaseEncodingAxis" in data:
         return data["PhaseEncodingAxis"] + "+"
     raise ClinicaException(
         "Could not recover the PhaseEncodingDirection from JSON file."
     )
+
+
+def get_parent(path: str, n: int = 1) -> Path:
+    """Get the path to the nth parent.
+
+    Parameters
+    ----------
+    path: str
+        path to a file.
+    n: int
+        depth we want to go up in the parents.
+
+    Returns
+    -------
+    Path
+        Path to a parent directory.
+
+    Examples
+    --------
+    >>> get_parent('/path/to/a/file', 2)
+    /path/to
+    """
+    if n <= 0:
+        return Path(path)
+    return get_parent(Path(path).parent, n - 1)
```

### Comparing `clinica-0.7.4/clinica/utils/fmap.py` & `clinica-0.7.5/clinica/utils/fmap.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/freesurfer.py` & `clinica-0.7.5/clinica/utils/freesurfer.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/group.py` & `clinica-0.7.5/clinica/utils/group.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/input_files.py` & `clinica-0.7.5/clinica/utils/input_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,14 +491,19 @@
         ),
         "description": f"T1w template file of group {group_label}",
         "needed_pipeline": "t1-volume or t1-volume-create-dartel",
     }
     return information
 
 
+def custom_group(pattern, description):
+    information = {"pattern": pattern, "description": description}
+    return information
+
+
 """ DWI """
 
 # BIDS
 
 DWI_NII = {"pattern": "dwi/sub-*_ses-*_dwi.nii*", "description": "DWI NIfTI"}
 
 DWI_JSON = {"pattern": "dwi/sub-*_ses-*_dwi.json", "description": "DWI JSON file"}
@@ -632,7 +637,13 @@
             "pet_linear",
             f"*_trc-{acq_label}_pet_space-MNI152NLin2009cSym{description}_res-1x1x1_suvr-{suvr_reference_region}_pet.nii.gz",
         ),
         "description": "",
         "needed_pipeline": "pet-linear",
     }
     return information
+
+
+# CUSTOM
+def custom_pipeline(pattern, description):
+    information = {"pattern": pattern, "description": description}
+    return information
```

### Comparing `clinica-0.7.4/clinica/utils/inputs.py` & `clinica-0.7.5/clinica/utils/inputs.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/longitudinal.py` & `clinica-0.7.5/clinica/utils/longitudinal.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/mri_registration.py` & `clinica-0.7.5/clinica/utils/mri_registration.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/nipype.py` & `clinica-0.7.5/clinica/utils/nipype.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 In particular, this module currently contains functions used for Nipype DataSink.
 """
 
 
 def container_from_filename(bids_or_caps_filename: str) -> str:
     """Extract container from BIDS or CAPS file.
 
-    Args:
-       bids_or_caps_filename (str): full path to BIDS or CAPS filename.
-
-    Returns:
-       Container path of the form "subjects/<participant_id>/<session_id>"
-
-    Examples:
-       >>> from clinica.utils.nipype import container_from_filename
-       >>> container_from_filename('/path/to/bids/sub-CLNC01/ses-M000/anat/sub-CLNC01_ses-M000_T1w.nii.gz')
-               'subjects/sub-CLNC01/ses-M000'
-       >>> container_from_filename('caps/subjects/sub-CLNC01/ses-M000/dwi/preprocessing/sub-CLNC01_ses-M000_preproc.nii')
-               'subjects/sub-CLNC01/ses-M000'
+    Parameters
+    ----------
+    bids_or_caps_filename : str
+        Full path to BIDS or CAPS filename.
+
+    Returns
+    -------
+    str :
+        Container path of the form "subjects/<participant_id>/<session_id>".
+
+    Examples
+    --------
+    >>> from clinica.utils.nipype import container_from_filename
+    >>> container_from_filename('/path/to/bids/sub-CLNC01/ses-M000/anat/sub-CLNC01_ses-M000_T1w.nii.gz')
+    'subjects/sub-CLNC01/ses-M000'
+    >>> container_from_filename('caps/subjects/sub-CLNC01/ses-M000/dwi/preprocessing/sub-CLNC01_ses-M000_preproc.nii')
+    'subjects/sub-CLNC01/ses-M000'
     """
     import os
     import re
 
     m = re.search(r"(sub-[a-zA-Z0-9]+)/(ses-[a-zA-Z0-9]+)", bids_or_caps_filename)
     if not m:
         raise ValueError(
```

### Comparing `clinica-0.7.4/clinica/utils/participant.py` & `clinica-0.7.5/clinica/utils/participant.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/pet.py` & `clinica-0.7.5/clinica/utils/pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/spm.py` & `clinica-0.7.5/clinica/utils/spm.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/statistics.py` & `clinica-0.7.5/clinica/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/stream.py` & `clinica-0.7.5/clinica/utils/stream.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/testing_utils.py` & `clinica-0.7.5/clinica/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/clinica/utils/ux.py` & `clinica-0.7.5/clinica/utils/ux.py`

 * *Files identical despite different names*

### Comparing `clinica-0.7.4/pyproject.toml` & `clinica-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinica"
-version = "0.7.4"
+version = "0.7.5"
 description = "Software platform for clinical neuroimaging studies"
 license = "MIT"
 authors = ["ARAMIS Lab"]
 maintainers = ["Clinica developers <clinica-user@inria.fr>"]
 readme = "README.md"
 homepage = "https://www.clinica.run"
 repository = "https://github.com/aramis-lab/clinica.git"
@@ -47,22 +47,23 @@
 networkx = "^2"
 click = "^8"
 click-option-group = "^0.5"
 xlrd = "*"
 openpyxl = "*"
 fsspec = "*"
 pydra-nipype1 = "^0.2"
-pydra = "^0.21"
+pydra = "^0.22"
 pybids = "^0.15.1"
 joblib = "^1.2.0"
 attrs = ">=20.1.0"
 cattrs = "^1.9.0"
 brainstat = "^0.3.6"
 pydra-bids = "^0.0.10"
 pydra-freesurfer = "^0.0.9"
+pydra-petpvc="^0.0.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 pre-commit = "*"
 codespell = {extras = ["toml"], version = "^2.2.2"}
 
@@ -75,14 +76,16 @@
 pymdown-extensions = "*"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-timeout = "*"
 pytest-xdist = "*"
 pytest-cov = "^3.0.0"
+pytest-mock = "*"
+pytest-random-order = "*"
 scikit-image = "^0.19"
 nibabel = "*"
 
 [tool.poetry.scripts]
 clinica = "clinica.cmdline:main"
 
 [build-system]
```

### Comparing `clinica-0.7.4/PKG-INFO` & `clinica-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinica
-Version: 0.7.4
+Version: 0.7.5
 Summary: Software platform for clinical neuroimaging studies
 Home-page: https://www.clinica.run
 License: MIT
 Keywords: bids,image processing,machine learning,neuroimaging,neuroscience
 Author: ARAMIS Lab
 Maintainer: Clinica developers
 Maintainer-email: clinica-user@inria.fr
@@ -39,18 +39,19 @@
 Requires-Dist: nilearn[plotting] (>=0.9.2,<0.10.0)
 Requires-Dist: nipype (>=1.7.1,<1.8.3)
 Requires-Dist: numpy (>=1.17,<2.0)
 Requires-Dist: openpyxl
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: pybids (>=0.15.1,<0.16.0)
 Requires-Dist: pydicom
-Requires-Dist: pydra (>=0.21,<0.22)
+Requires-Dist: pydra (>=0.22,<0.23)
 Requires-Dist: pydra-bids (>=0.0.10,<0.0.11)
 Requires-Dist: pydra-freesurfer (>=0.0.9,<0.0.10)
 Requires-Dist: pydra-nipype1 (>=0.2,<0.3)
+Requires-Dist: pydra-petpvc (>=0.0.4,<0.0.5)
 Requires-Dist: scikit-image (>=0.19,<0.20)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: xgboost
 Requires-Dist: xlrd
 Requires-Dist: xvfbwrapper
 Project-URL: Documentation, https://aramislab.paris.inria.fr/clinica/docs/public/latest
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clinica Version: 0.7.4 Summary: Software platform
+Metadata-Version: 2.1 Name: clinica Version: 0.7.5 Summary: Software platform
 for clinical neuroimaging studies Home-page: https://www.clinica.run License:
 MIT Keywords: bids,image processing,machine learning,neuroimaging,neuroscience
 Author: ARAMIS Lab Maintainer: Clinica developers Maintainer-email: clinica-
 user@inria.fr Requires-Python: >=3.8,<3.12 Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -17,22 +17,23 @@
 option-group (>=0.5,<0.6) Requires-Dist: colorlog (>=5,<6) Requires-Dist:
 fsspec Requires-Dist: jinja2 (>=3,<4) Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: matplotlib Requires-Dist: networkx (>=2,<3) Requires-Dist:
 nibabel (>=3.2.2,<4.0.0) Requires-Dist: niflow-nipype1-workflows Requires-Dist:
 nilearn[plotting] (>=0.9.2,<0.10.0) Requires-Dist: nipype (>=1.7.1,<1.8.3)
 Requires-Dist: numpy (>=1.17,<2.0) Requires-Dist: openpyxl Requires-Dist:
 pandas (>=1.4,<2.0) Requires-Dist: pybids (>=0.15.1,<0.16.0) Requires-Dist:
-pydicom Requires-Dist: pydra (>=0.21,<0.22) Requires-Dist: pydra-bids
+pydicom Requires-Dist: pydra (>=0.22,<0.23) Requires-Dist: pydra-bids
 (>=0.0.10,<0.0.11) Requires-Dist: pydra-freesurfer (>=0.0.9,<0.0.10) Requires-
-Dist: pydra-nipype1 (>=0.2,<0.3) Requires-Dist: scikit-image (>=0.19,<0.20)
-Requires-Dist: scikit-learn (>=1.0,<2.0) Requires-Dist: scipy (>=1.7,<2.0)
-Requires-Dist: xgboost Requires-Dist: xlrd Requires-Dist: xvfbwrapper Project-
-URL: Documentation, https://aramislab.paris.inria.fr/clinica/docs/public/latest
-Project-URL: Repository, https://github.com/aramis-lab/clinica.git Description-
-Content-Type: text/markdown
+Dist: pydra-nipype1 (>=0.2,<0.3) Requires-Dist: pydra-petpvc (>=0.0.4,<0.0.5)
+Requires-Dist: scikit-image (>=0.19,<0.20) Requires-Dist: scikit-learn
+(>=1.0,<2.0) Requires-Dist: scipy (>=1.7,<2.0) Requires-Dist: xgboost Requires-
+Dist: xlrd Requires-Dist: xvfbwrapper Project-URL: Documentation, https://
+aramislab.paris.inria.fr/clinica/docs/public/latest Project-URL: Repository,
+https://github.com/aramis-lab/clinica.git Description-Content-Type: text/
+markdown
                                 ****** [Logo]
                                 Clinica ******
               Software platform for clinical neuroimaging studies
   [Build_Status] [PyPI_version] [Supported_Python_versions]  [platform] [Code
                            style:_black] [Downloads]
  Homepage | Documentation | Paper | Forum | See also: AD-ML, AD-DL, ClinicaDL
 ## About The Project Clinica is a software platform for clinical research
```

