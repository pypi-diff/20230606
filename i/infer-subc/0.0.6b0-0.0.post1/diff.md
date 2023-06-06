# Comparing `tmp/infer-subc-0.0.6b0.tar.gz` & `tmp/infer-subc-0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infer-subc-0.0.6b0.tar", last modified: Tue Jun  6 19:39:56 2023, max compression
+gzip compressed data, was "infer-subc-0.0.post1.tar", last modified: Sat May 13 00:28:51 2023, max compression
```

## Comparing `infer-subc-0.0.6b0.tar` & `infer-subc-0.0.post1.tar`

### file list

```diff
@@ -1,186 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.188782 infer-subc-0.0.6b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.164782 infer-subc-0.0.6b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/.github/workflows/ci.yml.disable
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/20230221_MSI_3Dmeasurements.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/ABOUT_THIS_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-06 19:39:56.188782 infer-subc-0.0.6b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/framework.md
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/infer_subc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/infer_subc/core/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/core/file_io.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/core/img.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/infer_subc/napari/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/napari/organelle_config.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/napari/plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/infer_subc/organelles/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/cellmask.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/cytoplasm.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/er.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/golgi.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/lipid.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/lysosome.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/mitochondria.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/nuclei.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles/peroxisome.md
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/organelles.md
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/infer_subc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/utils/batch.md
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/utils/etc.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/utils/stats.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/utils/utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/infer_subc/workflow.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/docs/nbs/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/nbs/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/docs/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/env_create.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.168782 infer-subc-0.0.6b0/infer_subc/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.168782 infer-subc-0.0.6b0/infer_subc/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/core/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    44069 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/core/img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/core/zslice.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.168782 infer-subc-0.0.6b0/infer_subc/organelles/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/cellmask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/cytoplasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/er.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/golgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/lipid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/lysosome.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/mitochondria.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/nuclei.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/peroxisome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles/qc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.168782 infer-subc-0.0.6b0/infer_subc/organelles_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56566 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/all_functions.json
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.1.masks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.2.lyso.json
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.3.mito.json
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.4.golgi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.5.perox.json
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.6.ER.json
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.7.LD.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.176782 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/infer_nuclei.json
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/infer_soma.json
--rw-r--r--   0 runner    (1001) docker     (123)    18306 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/og_all_functions.json
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/test_functions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/function_guide.md
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/function_params.md
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/organelles_config/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.168782 infer-subc-0.0.6b0/infer_subc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/_aicsimage_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32061 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    24516 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/utils/stats_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.168782 infer-subc-0.0.6b0/infer_subc/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/batch_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/segmenter_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/workflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/workflow_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/workflow_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/infer_subc/workflow/workflow_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/infer_subc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 19:39:56.000000 infer-subc-0.0.6b0/infer_subc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.184782 infer-subc-0.0.6b0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/00.0_framework_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/00.1_pipeline_setup.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1580645 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/01_infer_nuclei_from-label.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50739 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/01a_infer_cytoplasm_from-composite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    72544 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/02_infer_cellmask_from-composite_with-nuclei.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50739 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/02a_infer_nuclei_from-composite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/02b_infer_cellmask_from-membrane.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    52882 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/03_infer_cytoplasm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50739 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/03a_infer_cellmask_from-composite_no-nuclei.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    67155 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/04_infer_neurites_soma_from-cellmask.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   685988 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/05_infer_lysosome.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   715292 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/06_infer_mitochondria.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   159659 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/07_infer_golgi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   412905 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/08_infer_peroxisome.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   314565 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/09_infer_ER.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   266369 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/10_infer_lipid_droplet.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/11_regionprops.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/12_batch_process.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    85559 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/13_fn_prototypes_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    89112 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/14_workflow_defs_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   213649 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/15_final_workflow.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.188782 infer-subc-0.0.6b0/notebooks/todelete/
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/00.1_pipeline_setup_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/00.2_extract_optimal_Z.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    53320 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/01_infer_nuclei_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    67064 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/02_infer_soma_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    66972 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/02a_infer_soma_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    67033 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/02b_infer_neurites_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    67027 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/02c_infer_wholecell_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    86025 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/03_infer_cytosol_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   121185 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/04_infer_lysosome_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   154818 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/05_infer_mitochondria_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    96854 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/06_infer_golgi_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    92224 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/07_infer_peroxisome_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   126036 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   127295 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/09_infer_lipid_body_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   415241 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/10_batch_process_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   345416 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/10_batch_process_3Dv2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    70614 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/999_fn_prototypes_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/A_spectral_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/_centrosome_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/_graveyard.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    73532 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/new02a_infer_soma_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   478607 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/notebooks/todelete/test_soma_seg.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-06 19:39:56.188782 infer-subc-0.0.6b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:56.172782 infer-subc-0.0.6b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 19:39:50.000000 infer-subc-0.0.6b0/windows_notes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.063383 infer-subc-0.0.post1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.027383 infer-subc-0.0.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.035383 infer-subc-0.0.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/.github/workflows/ci.yml.disable
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/20230221_MSI_3Dmeasurements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/ABOUT_THIS_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-13 00:28:51.063383 infer-subc-0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/framework.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/infer_subc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/infer_subc/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/core/file_io.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/core/img.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/infer_subc/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/napari/organelle_config.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/napari/plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/infer_subc/organelles/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/cellmask.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/cytoplasm.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/er.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/golgi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/lipid.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/lysosome.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/mitochondria.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/nuclei.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles/peroxisome.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/organelles.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/infer_subc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/utils/batch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/utils/etc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/utils/stats.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/utils/utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/infer_subc/workflow.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.039383 infer-subc-0.0.post1/docs/nbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/nbs/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/docs/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/env_create.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.031383 infer-subc-0.0.post1/infer_subc/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-13 00:28:50.000000 infer-subc-0.0.post1/infer_subc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.031383 infer-subc-0.0.post1/infer_subc/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/core/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/core/img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/core/zslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.031383 infer-subc-0.0.post1/infer_subc/organelles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/cellmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/cytoplasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/golgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/lipid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/lysosome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/mitochondria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/nuclei.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/peroxisome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles/qc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.043383 infer-subc-0.0.post1/infer_subc/organelles_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54029 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/all_functions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.1.masks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.1.masks_MCZ.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.2.lyso.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.3.mito.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.4.golgi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.5.perox.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.6.ER.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.7.LD.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.047383 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/infer_nuclei.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/infer_soma.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/og_all_functions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/depricate/test_functions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/function_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/function_params.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/organelles_config/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.035383 infer-subc-0.0.post1/infer_subc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/_aicsimage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32061 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24516 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/utils/stats_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.035383 infer-subc-0.0.post1/infer_subc/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/batch_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/segmenter_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/workflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/workflow_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/workflow_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/infer_subc/workflow/workflow_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.043383 infer-subc-0.0.post1/infer_subc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-13 00:28:50.000000 infer-subc-0.0.post1/infer_subc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-13 00:28:51.000000 infer-subc-0.0.post1/infer_subc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:28:50.000000 infer-subc-0.0.post1/infer_subc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-13 00:28:50.000000 infer-subc-0.0.post1/infer_subc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-13 00:28:50.000000 infer-subc-0.0.post1/infer_subc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 00:28:50.000000 infer-subc-0.0.post1/infer_subc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.055383 infer-subc-0.0.post1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/00.0_framework_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/00.1_pipeline_setup.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    52896 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/01_infer_nuclei-from-ERsignal_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25936 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/01_infer_nuclei.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   113828 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/02_infer_cellmask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/02a_cell_membrane.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    67191 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/02b_infer_neurites_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    47751 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/03_infer_cytoplasm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21870 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/04_infer_lysosome.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    56551 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/05_infer_mitochondria.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42408 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/06_infer_golgi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    40788 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/07_infer_peroxisome.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    51759 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/08_infer_ER.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    39618 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/09_infer_lipid_droplet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/10_regionprops.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/11_batch_process.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    81922 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/12_fn_prototypes_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    89132 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/13_workflow_defs_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   213649 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/14_final_workflow.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.059383 infer-subc-0.0.post1/notebooks/todelete/
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/00.1_pipeline_setup_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/00.2_extract_optimal_Z.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    53320 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/01_infer_nuclei_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    67064 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/02_infer_soma_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    66972 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/02a_infer_soma_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    67033 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/02b_infer_neurites_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    67027 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/02c_infer_wholecell_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    86025 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/03_infer_cytosol_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   121185 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/04_infer_lysosome_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   154818 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/05_infer_mitochondria_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    96854 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/06_infer_golgi_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    92224 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/07_infer_peroxisome_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   126036 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   127295 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/09_infer_lipid_body_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   415241 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/10_batch_process_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   345416 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/10_batch_process_3Dv2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    70614 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/999_fn_prototypes_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/A_spectral_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/_centrosome_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/_graveyard.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    73532 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/new02a_infer_soma_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   478607 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/notebooks/todelete/test_soma_seg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-13 00:28:51.063383 infer-subc-0.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:51.035383 infer-subc-0.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-13 00:28:32.000000 infer-subc-0.0.post1/windows_notes.md
```

### Comparing `infer-subc-0.0.6b0/.github/workflows/ci.yml.disable` & `infer-subc-0.0.post1/.github/workflows/ci.yml.disable`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/.github/workflows/publish.yml` & `infer-subc-0.0.post1/.github/workflows/publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 name: Publish
 on:
   push:
-    tags:
-      - "v*"
-    # branches:
-    #   - main
+    branches:
+      - main
 jobs:
   pypi:
     name: Upload release to PyPI
     runs-on: ubuntu-latest
     # environment:
     #   name: pypi
     #   url: https://pypi.org/p/<your-pypi-project-name>
```

### Comparing `infer-subc-0.0.6b0/.gitignore` & `infer-subc-0.0.post1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -134,10 +134,7 @@
 .github/templates/*
 
 #osx crud
 .DS_Store
 
 # mkdocs
 site
-
-# written by setuptools_scm
-*/_version.py
```

### Comparing `infer-subc-0.0.6b0/20230221_MSI_3Dmeasurements.csv` & `infer-subc-0.0.post1/20230221_MSI_3Dmeasurements.csv`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx` & `infer-subc-0.0.post1/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/ABOUT_THIS_TEMPLATE.md` & `infer-subc-0.0.post1/ABOUT_THIS_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/CONTRIBUTING.md` & `infer-subc-0.0.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/Makefile` & `infer-subc-0.0.post1/Makefile`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/PKG-INFO` & `infer-subc-0.0.post1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infer-subc
-Version: 0.0.6b0
+Version: 0.0.post1
 Summary: A plugin that enables organelle segmentation
 Home-page: https://github.com/ndcn/infer-subc
 Author: Andy Henrie
 Author-email: ergonyc@gmail.com
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/ndcn/infer-subc/issues
 Project-URL: Documentation, https://github.com/ndcn/infer-subc#README.md
@@ -69,68 +69,87 @@
 - [`napari`](https://napari.org/stable/) -- Used as the visualization framework, a fast, interactive, multi-domensional image viewer for Python.
 - [`scipy`](https://scipy.org/install/) -- Image analysis
 - [`scikit-image`](https://scikit-image.org/) -- Image analysis
 - [`itk`](https://itkpythonpackage.readthedocs.io/en/master/Quick_start_guide.html) -- Image analysis
 - [`numpy`](https://numpy.org/) -- Under the hood computation
 - [`Alzheimer's Disease AD Workbench`](https://www.alzheimersdata.org/ad-workbench) -- We initially wanted to use the ADDI's ADWB as a method of data sharing and to serve as a computational resource.
 
+## ADWB hints
+
+Given that the github repos are not yet whitelisted, the source directory needs to be zipped and uploaded in order to make an "editable" pip install.
+
+[uploading guide ](https://knowledgebase.aridhia.io/article/guidance-for-uploading-files/)
+[uploading files via the workspace article](https://knowledgebase.aridhia.io/article/uploading-files-via-the-workspace/).
+[Using BLOB storage](https://knowledgebase.aridhia.io/article/using-blob-storage/)
 
 ## Getting Started
 
 ### Prerequisites
 
+The following are prerequisites and should be installed prior to using the workflow.
 
+- `napari` 
+  ```
+  pip install "napari[all]"
+  ```
+
+- `scipy`
+  ```
+  python -m pip install scipy
+  ```
+
+- `scikit-image`
+  ```
+  pip install scikit-image
+  ```
+
+- `itk`
+  ```
+  pip install itk
+  ```
+- `numpy`
+  ```
+  pip install numpy
+  ```
 
 ### Installation
-`infer_subc` is  available on `PyPI` via: 
 
+`infer_subc` is not yet available on `PyPI` so must be  be `pip` ionstalled from source
 ```
-pip install infer_subc
+pip install git+https://github.com/ndcn/infer-subc.git
 ```
 
-If there are issues more details can be fouund in the [documentation](https://ndcn.github.io/infer-subc/config/)
-
+## Usage
 
-## Usage - quick start
-Its recommended that you use this repo along with the [`organelle-segmenter-plugin`](https://github.com/ndcn/organelle-segmenter-plugin) as in [Option A](#option-a-napari-organelle-segmenter-plugin) below.  Alternatively using the module functions directly as in [Option B](#option-b-python-script-or-notebook) would work just fine.
+```py
+from infer_subc.organelles import infer_lyso
+from infer_subc.core.file_io import read_czi_image
 
+img_data,meta_dict = read_czi_image("path/to/image.czi")
+lyso_obj =  infer_lyso(img_data) 
 
-### Option A: Napari `organelle-segmenter-plugin`
-
-1. Open a file in napari by dragging multi-channel .czi file onto napari which will import a multi-channel, multi-Z 'layer'. (Using the menu's defaults to `aicsIMAGEIO` reader which automatically splits mutliple channels into individual layers.  The plugin is able to support multi-dimensional data in .tiff, .tif. ome.tif, .ome.tiff, .czi)
-2. Start the plugin (open napari, go to "Plugins" --> "organelle-segmenter-plugin" --> "workflow editor")
-3. Select the image and channel to work on
-4. Select a workflow based on the example image and target segmentation based on user's data. Ideally, it is recommend to start with the example with very similar morphology as user's data.
-5. Click "Run All" to execute the whole workflow on the sample data.
-6. Adjust the parameters of steps, based on the intermediate results.  A complete list of all functions can be found [here](https://github.com/ndcn/infer-subc/blob/main/infer_subc/organelles_config/function_params.md)🚧 WIP 🚧
-7. Click "Run All" again after adjusting the parameters and repeat step 6 and 7 until the result is satisfactory.
-8. Save the workflow
-9. Close the plugin and open the **batch processing** part by (go to "Plugins" --> "organelle-segmenter-plugin" --> "batch processing")
-10. Load the customized workflow saved above 
-11. Load the folder with all the images to process
-12. Click "Run"
-13. Follow the [examples](https://github.com/ndcn/infer-subc/blob/main/notebooks/14_final_workflow.ipynb) in the `infer_subc` [repo](https://github.com/ndcn/infer-subc/) for postprocessing of the saved segmentations and generating the statistics.  
+```
 
-### Option B: python script or notebook 
+ 🚧 WIP 🚧 (🚨🚨🚨🚨 )
+> NOTE: command line capabilities not implimented
+```bash
+$ python -m infer_subc
+#or
+$ infer_subc
+```
 
-A variety of example [notebooks](https://github.com/ndcn/infer-subc/blob/main/notebooks/) demonstrating how to use the are available in the repo.  Additional information can be found at https://ndcn.github.io/infer-subc/nbs/overview/.  
+## Roadmap
 
+ - [ ] Create `PyPI` package
+ - [ ] Update installation instructions to reflect optimal use of `conda` environments
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## License
-Distributed under the terms of the [BSD-3] license,
-"organelle-segmenter-plugin" is free and open source software
+
+Distributed under the Unlicense license. See `LICENSE` for more information.  
 
 ## Issues
 
 If you encounter any problems, please file an issue with a detailed description.
-
-## ADWB hints
-
-Given that the github repos are not yet whitelisted, the source directory needs to be zipped and uploaded in order to make an "editable" pip install.
-
-[uploading guide ](https://knowledgebase.aridhia.io/article/guidance-for-uploading-files/)
-[uploading files via the workspace article](https://knowledgebase.aridhia.io/article/uploading-files-via-the-workspace/).
-[Using BLOB storage](https://knowledgebase.aridhia.io/article/using-blob-storage/)
```

### Comparing `infer-subc-0.0.6b0/docs/framework.md` & `infer-subc-0.0.post1/docs/framework.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/docs/index.md` & `infer-subc-0.0.post1/docs/index.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/docs/infer_subc/organelles.md` & `infer-subc-0.0.post1/docs/infer_subc/organelles.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/docs/infer_subc/overview.md` & `infer-subc-0.0.post1/docs/infer_subc/overview.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/docs/infer_subc/workflow.md` & `infer-subc-0.0.post1/docs/infer_subc/workflow.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/docs/nbs/overview.md` & `infer-subc-0.0.post1/docs/nbs/overview.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/docs/pipeline.md` & `infer-subc-0.0.post1/docs/pipeline.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/__init__.py` & `infer-subc-0.0.post1/infer_subc/__init__.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/cli.py` & `infer-subc-0.0.post1/infer_subc/cli.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/core/file_io.py` & `infer-subc-0.0.post1/infer_subc/core/file_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         Path.mkdir(out_data_path)
         print(f"making {out_data_path}")
 
     img_name_out = f"{img_name.stem}-{name}"
     # HACK: skip the ome
     # out_file_n = export_ome_tiff(img_out, meta_dict, img_name_out, str(out_data_path) + "/", name)
     out_file_n = export_tiff(img_out, img_name_out, out_data_path, name, meta_dict)
-    print(f"saved file: {img_name_out}")
+    print(f"saved file: {out_file_n}")
     return out_file_n
 
 
 def export_inferred_organelle_stack(img_out, layer_names, meta_dict, data_root_path):
     """
     stack all the inferred objects and stack along 0 dimension
     """
```

### Comparing `infer-subc-0.0.6b0/infer_subc/core/img.py` & `infer-subc-0.0.post1/infer_subc/core/img.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 # from skimage.filters import threshold_triangle, threshold_otsu, threshold_li, threshold_multiotsu, threshold_sauvola
 from scipy.ndimage import median_filter, extrema, distance_transform_edt, sum, minimum_filter, maximum_filter
 
 from aicssegmentation.core.utils import size_filter, hole_filling
 from aicssegmentation.core.vessel import vesselness2D
 from aicssegmentation.core.MO_threshold import MO
 
-from aicssegmentation.core.vessel import filament_2d_wrapper, filament_3d_wrapper
+from aicssegmentation.core.vessel import filament_2d_wrapper
 from aicssegmentation.core.pre_processing_utils import (
     image_smoothing_gaussian_slice_by_slice,
     # edge_preserving_smoothing_3d,
 )
-from aicssegmentation.core.seg_dot import dot_2d_slice_by_slice_wrapper, dot_3d_wrapper
+from aicssegmentation.core.seg_dot import dot_2d_slice_by_slice_wrapper
 
 from typing import Tuple, List, Union, Any
 
 from skimage.morphology import remove_small_objects, white_tophat, ball, disk, black_tophat, label
 from skimage.segmentation import clear_border, watershed
 
 from infer_subc.constants import (
@@ -211,43 +211,43 @@
     image, d = log_transform(image_in.copy())
     thresholds = threshold_multiotsu(image)
     thresholds = inverse_log_transform(thresholds, d)
     return thresholds
 
 
 def masked_object_thresh(
-    structure_img_smooth: np.ndarray, global_method: str, cutoff_size: int, local_adjust: float
+    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float
 ) -> np.ndarray:
     """
     wrapper for applying Masked Object Thresholding with just two parameters via `MO` from `aicssegmentation`
 
     Parameters
     ------------
     structure_img_smooth:
         a 3d image
-    global_method:
+    th_method:
          which method to use for calculating global threshold. Options include:
          "triangle", "median", and "ave_tri_med".
          "ave_tri_med" refers the average of "triangle" threshold and "mean" threshold.
     cutoff_size:
         Masked Object threshold `size_min`
-    local_adjust:
+    th_adjust:
         Masked Object threshold `local_adjust`
 
     Returns
     -------------
         np.ndimage
 
     """
     struct_obj = MO(
         structure_img_smooth,
         object_minArea=cutoff_size,
-        global_thresh_method=global_method,
+        global_thresh_method=th_method,
         extra_criteria=True,
-        local_adjust=local_adjust,
+        local_adjust=th_adjust,
         return_object=False,
         dilate=False,  # WARNING: dilate=True causes a bug if there is only one Z
     )
     return struct_obj
 
 
 def get_interior_labels(img_in: np.ndarray) -> np.ndarray:
@@ -402,43 +402,42 @@
             img_out += (w * 1.0) * img_in[ch]
 
     return img_out
 
 
 def make_aggregate(
     img_in: np.ndarray,
-    weight_ch0: int = 0,
-    weight_ch1: int = 0,
-    weight_ch2: int = 0,
-    weight_ch3: int = 0,
-    weight_ch4: int = 0,
-    weight_ch5: int = 0,
-    weight_ch6: int = 0,
-    weight_ch7: int = 0,
-    weight_ch8: int = 0,
-    weight_ch9: int = 0,
-    rescale: bool = True,
+    w0: int = 0,
+    w1: int = 0,
+    w2: int = 0,
+    w3: int = 0,
+    w4: int = 0,
+    w5: int = 0,
+    w6: int = 0,
+    w7: int = 0,
+    w8: int = 0,
+    w9: int = 0,
+    scale_min_max: bool = True,
 ) -> np.ndarray:
     """define multi_channel aggregate.  weighted sum wrapper (plugin)
 
     Parameters
     ------------
     w0,w1,w2,w3,w4,w5,w6,w7,w8,w9
         channel weights
-    rescale:
+    scale_min_max:
         scale to [0,1] if True. default True
 
     Returns
     -------------
         np.ndarray scaled aggregate
 
     """
-    weights = (weight_ch0, weight_ch1, weight_ch2, weight_ch3, weight_ch4,
-               weight_ch5, weight_ch6, weight_ch7, weight_ch8, weight_ch9)
-    if rescale:
+    weights = (w0, w1, w2, w3, w4, w5, w6, w7, w8, w9)
+    if scale_min_max:
         # TODO: might NOT overflow here... maybe NOT do the normaization first?
         return min_max_intensity_normalization(weighted_aggregate(min_max_intensity_normalization(img_in), *weights))
     else:
         return weighted_aggregate(img_in, *weights)
 
 
 def apply_threshold(
@@ -604,42 +603,42 @@
     else:
         z_slice = list(z_slice)
 
     return img_in[:, z_slice, :, :]
 
 
 def scale_and_smooth(
-    img_in: np.ndarray, median_size: int = 1, gauss_sigma: float = 1.34, slice_by_slice: bool = True
+    img_in: np.ndarray, median_sz: int = 1, gauss_sig: float = 1.34, slice_by_slice: bool = True
 ) -> np.ndarray:
     """
     helper to perform min-max scaling, and median+gaussian smoothign all at once
     Parameters
     ------------
     img_in: np.ndarray
         a 3d image
-    median_size: int
+    median_sz: int
         width of median filter for signal
-    gauss_sigma: float
+    gauss_sig: float
         sigma for gaussian smoothing of  signal
     slice_by_slice:
         NOT IMPLIMENTED.  toggles whether to do 3D operations or slice by slice in Z
 
     Returns
     -------------
         np.ndimage
 
     """
     img = min_max_intensity_normalization(img_in.copy())  # is this copy nescesa
 
     # TODO:  make non-slice-by-slice work
     slice_by_slice = True
     if slice_by_slice:
-        if median_size > 1:
-            img = median_filter_slice_by_slice(img, size=median_size)
-        img = image_smoothing_gaussian_slice_by_slice(img, sigma=gauss_sigma)
+        if median_sz > 1:
+            img = median_filter_slice_by_slice(img, size=median_sz)
+        img = image_smoothing_gaussian_slice_by_slice(img, sigma=gauss_sig)
     else:
         print(" PLEASE CHOOOSE 'slice-by-slice', 3D is not yet implimented")
 
     return img
 
 
 # DEPRICATED
@@ -696,51 +695,32 @@
     """
     total_florescence_ = aggregate_signal_channels(img_in, chs)
     if mask is not None:
         total_florescence_[mask] = 0.0
     return int(total_florescence_.sum(axis=(1, 2)).argmax())
 
 
-def masked_inverted_watershed(img_in: np.ndarray, 
-                                     markers: np.ndarray, 
-                                     mask: np.ndarray, 
-                                     method: str='slice-by-slice'):
+def masked_inverted_watershed(img_in, markers, mask):
     """wrapper for watershed on inverted image and masked
 
     Parameters
     ------------
     in_img:
-        a 3d image
-    markers: 
-        objects used to seed the watershed
-    mask:
-        instance segmentation of the in_img
-    method:
-        'slice-by-slice' results in a connectivity of np.ones((1,3,3), bool); '3D' results in a connectivity of np.ones((3,3,3), bool)
+        a 3d image containing all the channels
 
     """
-    if method == 'slice-by-slice':    
-        labels_out = watershed(
-            1.0 - img_in,
-            markers=markers,
-            connectivity=np.ones((1, 3, 3), bool),
-            mask=mask)
-    elif method == '3D':
-        labels_out = watershed(
+    labels_out = watershed(
         1.0 - img_in,
         markers=markers,
-        connectivity=np.ones((3, 3, 3), bool),
-        mask=mask)
-    else:
-        print(f"incompatable method: {method}")
-
+        connectivity=np.ones((1, 3, 3), bool),
+        mask=mask,
+    )
     return labels_out
 
 
-
 def choose_max_label(
     raw_signal: np.ndarray, labels_in: np.ndarray, target_labels: Union[np.ndarray, None] = None
 ) -> np.ndarray:
     """
     keep only the segmentation corresponding to the maximum raw signal.  candidate  label is taken from target_labels if not None
 
     Parameters
@@ -971,64 +951,14 @@
     result = image + white - black
     result[result > 1] = 1
     result[result < 0] = 0
 
     return result
 
 
-def filament_filter_3(in_img: np.ndarray, 
-                       filament_scale_1: float, 
-                       filament_cutoff_1: float,
-                       filament_scale_2: float, 
-                       filament_cutoff_2: float,
-                       filament_scale_3: float, 
-                       filament_cutoff_3: float,
-                       method: str
-                       ) -> np.ndarray:
-    """filament filter helper function for 3 levels (scale+cut). filter pairs are run if scale is > 0.
-
-    Parameters
-    ------------
-    in_img:
-        the image to filter on np.ndarray
-    filament_scale_1:
-        scale or size of the "filter" float
-    filament_cutoff_1:
-        cutoff for thresholding float
-    filament_scale_2:
-        scale or size of the "filter" float
-    filament_cutoff_2:
-        cutoff for thresholding float
-    filament_scale_3:
-        scale or size of the "filter" float
-    filament_cutoff_3:
-        cutoff for thresholding float
-    method:
-        either "3D" or "slice_by_slice", default is "slice_by_slice"
-
-    Returns
-    -----------
-    result:
-        filtered boolean np.ndarray
-
-    """
-    scales = [filament_scale_1, filament_scale_2, filament_scale_3]
-    cuts = [filament_cutoff_1, filament_cutoff_2, filament_cutoff_3]
-    f_param = [[sc, ct] for sc, ct in zip(scales, cuts) if sc > 0]
-
-    if method == "3D":
-        seg = filament_3d_wrapper(in_img, f_param)
-    elif method == "slice_by_slice":
-        seg = filament_2d_wrapper(in_img, f_param)
-    else:
-        print(f"undefined method: {method}")
-
-    return seg
-
-
 def filament_filter(in_img: np.ndarray, filament_scale: float, filament_cut: float) -> np.ndarray:
     """filament wrapper to properly pack parameters into filament_2d_wrapper
 
     Parameters
     ------------
     in_img:
         the image to filter on np.ndarray
@@ -1044,103 +974,54 @@
 
     """
     f2_param = [[filament_scale, filament_cut]]
     # f2_param = [[1, 0.15]]  # [scale_1, cutoff_1]
     return filament_2d_wrapper(in_img, f2_param)
 
 
-# def dot_filter_3(
-#     in_img: np.ndarray,
-#     dot_scale_1: float,
-#     dot_cut_1: float,
-#     dot_scale_2: float,
-#     dot_cut_2: float,
-#     dot_scale_3: float,
-#     dot_cut_3: float,
-# ) -> np.ndarray:
-#     """spot filter helper function for 3 levels (scale+cut).  if scale_i is > 0.0001 its skipped
-
-#     Parameters
-#     ------------
-#     in_img:
-#         a 3d  np.ndarray image of the inferred organelle (labels or boolean)
-#     dot_scale_1:
-#         scale or size of the "filter" float
-#     dot_cut_1:
-#         cutoff for thresholding float
-#     dot_scale_2:
-#         scale or size of the "filter" float
-#     dot_cut_2:
-#         cutoff for thresholding float
-#     dot_scale_3:
-#         scale or size of the "filter" float
-#     dot_cut_3:
-#         cutoff for thresholding float
-
-#     Returns
-#     -------------
-#     segmented dots over 3 scales
-
-#     """
-#     scales = [dot_scale_1, dot_scale_2, dot_scale_3]
-#     cuts = [dot_cut_1, dot_cut_2, dot_cut_3]
-
-#     s2_param = [[sc, ct] for sc, ct in zip(scales, cuts) if sc > 0.0001]
-#     # s2_param = [[dot_scale1, dot_cut1], [dot_scale2, dot_cut2], [dot_scale3, dot_cut3]]
-#     return dot_2d_slice_by_slice_wrapper(in_img, s2_param)
-
-
-def dot_filter_3(
+def spot_filter_3(
     in_img: np.ndarray,
     dot_scale_1: float,
-    dot_cutoff_1: float,
+    dot_cut_1: float,
     dot_scale_2: float,
-    dot_cutoff_2: float,
+    dot_cut_2: float,
     dot_scale_3: float,
-    dot_cutoff_3: float,
-    method: str = "slice_by_slice"
+    dot_cut_3: float,
 ) -> np.ndarray:
-    """spot filter helper function for 3 levels (scale+cut). filter pairs are run if scale is > 0.
+    """spot filter helper function for 3 levels (scale+cut).  if scale_i is > 0.0001 its skipped
 
     Parameters
     ------------
     in_img:
         a 3d  np.ndarray image of the inferred organelle (labels or boolean)
     dot_scale_1:
         scale or size of the "filter" float
-    dot_cutoff_1:
+    dot_cut_1:
         cutoff for thresholding float
     dot_scale_2:
         scale or size of the "filter" float
-    dot_cutoff_2:
+    dot_cut_2:
         cutoff for thresholding float
     dot_scale_3:
         scale or size of the "filter" float
     dot_cut_3:
         cutoff for thresholding float
-    method:
-        either "3D" or "slice_by_slice", default is "slice_by_slice"
 
     Returns
     -------------
     segmented dots over 3 scales
 
     """
     scales = [dot_scale_1, dot_scale_2, dot_scale_3]
-    cuts = [dot_cutoff_1, dot_cutoff_2, dot_cutoff_3]
-    s_param = [[sc, ct] for sc, ct in zip(scales, cuts) if sc > 0]
+    cuts = [dot_cut_1, dot_cut_2, dot_cut_3]
 
-    if method == "3D":
-        seg = dot_3d_wrapper(in_img, s_param)
-    elif method == "slice_by_slice":
-        seg = dot_2d_slice_by_slice_wrapper(in_img, s_param)
-    else:
-        print(f"undefined method: {method}")
+    s2_param = [[sc, ct] for sc, ct in zip(scales, cuts) if sc > 0.0001]
+    # s2_param = [[dot_scale1, dot_cut1], [dot_scale2, dot_cut2], [dot_scale3, dot_cut3]]
+    return dot_2d_slice_by_slice_wrapper(in_img, s2_param)
 
-    return seg
 
 # centrosome routines
 
 
 def size_similarly(labels, secondary):
     """Size the secondary matrix similarly to the labels matrix
```

### Comparing `infer-subc-0.0.6b0/infer_subc/core/zslice.py` & `infer-subc-0.0.post1/infer_subc/core/zslice.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles/__init__.py` & `infer-subc-0.0.post1/infer_subc/organelles/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # infer_subc/organelles
 
 from .nuclei import (
     infer_nuclei_fromlabel,
-    fixed_infer_nuclei_fromlabel,
+    fixed_infer_nuclei,
     infer_and_export_nuclei,
     infer_nuclei_fromlabel,
     get_nuclei,
 )
 from .cellmask import (
-    infer_cellmask_fromcomposite,
-    fixed_infer_cellmask_fromcomposite,
-    non_linear_cellmask_transform,
+    infer_cellmask_fromaggr,
+    fixed_infer_cellmask_fromaggr,
+    non_linear_cellmask_transform_MCZ,
     raw_cellmask_fromaggr,
     choose_max_label_cellmask_union_nucleus,
     infer_and_export_cellmask,
     get_cellmask,
 )
 
 # from .cellmask import infer_cellmask, fixed_infer_cellmask
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles/cytoplasm.py` & `infer-subc-0.0.post1/infer_subc/organelles/cytoplasm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from typing import Dict
 from pathlib import Path
 import time
 
 from skimage.morphology import binary_erosion
 from infer_subc.core.file_io import export_inferred_organelle, import_inferred_organelle
-from infer_subc.core.img import apply_mask, label_bool_as_uint16
+from infer_subc.core.img import apply_mask
 
 
 ##########################
 #  infer_cytoplasm
 ##########################
 def infer_cytoplasm(nuclei_object: np.ndarray, cellmask: np.ndarray, erode_nuclei: bool = True) -> np.ndarray:
     """
@@ -33,15 +33,15 @@
     nucleus_obj = apply_mask(nuclei_object, cellmask)
 
     if erode_nuclei:
         cytoplasm_mask = np.logical_xor(cellmask, binary_erosion(nucleus_obj))
     else:
         cytoplasm_mask = np.logical_xor(cellmask, nucleus_obj)
 
-    return label_bool_as_uint16(cytoplasm_mask)
+    return cytoplasm_mask
 
 
 def infer_and_export_cytoplasm(
     nuclei_object: np.ndarray, cellmask: np.ndarray, meta_dict: Dict, out_data_path: Path
 ) -> np.ndarray:
     """
     infer nucleus and write inferred nuclei to ome.tif file
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles/er.py` & `infer-subc-0.0.post1/infer_subc/organelles/lysosome.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,199 +1,153 @@
 import numpy as np
 from typing import Dict
 from pathlib import Path
 import time
 
-from infer_subc.constants import ER_CH
-from infer_subc.core.file_io import export_inferred_organelle, import_inferred_organelle
+from aicssegmentation.core.seg_dot import dot_2d_slice_by_slice_wrapper
+from aicssegmentation.core.vessel import filament_2d_wrapper
 
-from infer_subc.core.img import (
-    select_channel_from_raw,
-    scale_and_smooth,
-    label_bool_as_uint16,
-    fill_and_filter_linear_size,
-    masked_object_thresh,
-    filament_filter_3
-)
+from infer_subc.constants import LYSO_CH
+from infer_subc.core.file_io import export_inferred_organelle, import_inferred_organelle
+from infer_subc.core.img import scale_and_smooth, fill_and_filter_linear_size, select_channel_from_raw, label_uint16
 
 
 ##########################
-#  infer_ER
+#  infer_LYSOSOMES
 ##########################
-def infer_ER(in_img: np.ndarray,
-             ER_ch: int,
-             median_sz: int,
-             gauss_sig: float,
-             MO_thresh_method: str,
-             MO_cutoff_size: float,
-             MO_thresh_adj: float,
-             fil_scale_1: float,
-             fil_cut_1: float,
-             fil_scale_2: float, 
-             fil_cut_2: float, 
-             fil_scale_3: float, 
-             fil_cut_3: float,
-             fil_method: str,
-             min_hole_w: int,
-             max_hole_w: int,
-             small_obj_w: int,
-             fill_filter_method: str
-             ) -> np.ndarray:
+def infer_lyso(
+    in_img: np.ndarray,
+    median_sz: int,
+    gauss_sig: float,
+    dot_scale_1: float,
+    dot_cut_1: float,
+    dot_scale_2: float,
+    dot_cut_2: float,
+    dot_scale_3: float,
+    dot_cut_3: float,
+    filament_scale: float,
+    filament_cut: float,
+    min_hole_w: int,
+    max_hole_w: int,
+    small_obj_w: int,
+) -> np.ndarray:
     """
-    Procedure to infer ER from linearly unmixed input.
+    Procedure to infer lyso from linearly unmixed input
 
     Parameters
     ------------
-    in_img: 
-        a 3d image containing all the channels (CZYX)
-    ER_ch:
-        index of the ER channel in the input image
-    median_sz: 
+    in_img:
+        a 3d image containing all the channels
+    median_sz:
         width of median filter for signal
-    gauss_sig: 
+    gauss_sig:
         sigma for gaussian smoothing of  signal
-    mo_thresh_method: 
-         which method to use for calculating global threshold. Options include:
-         "triangle" (or "tri"), "median" (or "med"), and "ave_tri_med" (or "ave").
-         "ave" refers the average of "triangle" threshold and "mean" threshold.
-    mo_cutoff_size: 
-        Masked Object threshold `size_min`
-    mo_thresh_adjust: 
-        Masked Object threshold `local_adjust`
-    fil_scale_1: 
-        scale (log_sigma) for filament filter
-    fil_cutoff_1: 
-        threshold for filament fitered threshold, associated to fil_scale_1
-    fil_scale_2: 
+    dot_scale:
+        scales (log_sigma) for dot filter (1,2, and 3)
+    dot_cut:
+        threshold for dot filter thresholds (1,2,and 3)
+    filament_scale:
         scale (log_sigma) for filament filter
-    fil_cutoff_2: 
-        threshold for filament fitered threshold, associated to fil_scale_2
-    fil_scale_3: 
-        scale (log_sigma) for filament filter
-    fil_cutoff_3: 
-        threshold for filament fitered threshold, associated to fil_scale_3
-    fil_method:
-        decision to process the filaments "slice-by-slice" or in "3D"
-    min_hole_w: 
-        minimum size for hole filling for cellmask signal post-processing
-    max_hole_w: 
-        hole filling cutoff for ER signal post-processing
-    small_obj_w: 
-        minimum object size cutoff for ER signal post-processing
-    fill_filter_method:
-        determines if small hole filling and small object removal should be run 'sice-by-slice' or in '3D'
+    filament_cut:
+        threshold for filament fitered threshold
+    min_hole_w:
+        hole filling min for nuclei post-processing
+    max_hole_w:
+        hole filling cutoff for nuclei post-processing
+    small_obj_w:
+        minimu object size cutoff for nuclei post-processing
+
     Returns
     -------------
-    ER_object
-        mask defined extent of ER object
-    """
+    lyso_object:
+        mask defined extent of lyso object
 
+    """
+    lyso_ch = LYSO_CH
     ###################
     # EXTRACT
-    ###################    
-    ER = select_channel_from_raw(in_img, ER_ch)
+    ###################
+    lyso = select_channel_from_raw(in_img, lyso_ch)
 
     ###################
     # PRE_PROCESSING
-    ###################    
-    # er = normalized_edge_preserving_smoothing(er)
-    struct_img =  scale_and_smooth(ER,
-                                   median_size = median_sz, 
-                                   gauss_sigma = gauss_sig)
+    ###################
+    lyso = scale_and_smooth(lyso, median_sz=median_sz, gauss_sig=gauss_sig)
 
     ###################
     # CORE_PROCESSING
     ###################
-    bw1 = masked_object_thresh(struct_img, 
-                                    global_method=MO_thresh_method, 
-                                    cutoff_size=MO_cutoff_size, 
-                                    local_adjust=MO_thresh_adj)
+    s2_param = [[dot_scale_1, dot_cut_1], [dot_scale_2, dot_cut_2], [dot_scale_3, dot_cut_3]]
+    bw_spot = dot_2d_slice_by_slice_wrapper(lyso, s2_param)
 
-    bw2 = filament_filter_3(struct_img, fil_scale_1, fil_cut_1, fil_scale_2, fil_cut_2, fil_scale_3, fil_cut_3, fil_method)
+    f2_param = [[filament_scale, filament_cut]]
+    bw_filament = filament_2d_wrapper(lyso, f2_param)
+    # TODO: consider 3D version to call: aicssegmentation::vesselness3D
 
-    struct_obj = np.logical_or(bw1, bw2)
-    
-    ###################
-    # POST_PROCESSING
-    ################### 
-    struct_obj = fill_and_filter_linear_size(struct_obj, 
-                                             hole_min=min_hole_w, 
-                                             hole_max=max_hole_w, 
-                                             min_size=small_obj_w,
-                                             method=fill_filter_method)
+    bw = np.logical_or(bw_spot, bw_filament)
 
     ###################
-    # LABELING
+    # POST_PROCESSING
     ###################
-    
-    # ENSURE THAT there is ONLY ONE ER
-    struct_obj = label_bool_as_uint16(struct_obj)
-
-    return struct_obj 
+    struct_obj = fill_and_filter_linear_size(bw, hole_min=min_hole_w, hole_max=max_hole_w, min_size=small_obj_w)
+    return label_uint16(struct_obj)
 
 
 ##########################
-#  fixed_infer_ER
+#  fixed_infer_nuclei
 ##########################
-def fixed_infer_ER(in_img: np.ndarray ) -> np.ndarray:
+def fixed_infer_lyso(in_img: np.ndarray) -> np.ndarray:
     """
-    Procedure to infer endoplasmic rediculum from linearly unmixed input with *fixed parameters*
+    Procedure to infer lyso from linearly unmixed input
 
     Parameters
     ------------
-    in_img: 
+    in_img:
         a 3d image containing all the channels
 
     Returns
     -------------
-    ER_object
-        mask defined extent of ER object
+    nuclei_object:
+        mask defined extent of NU
     """
-    ER_ch = 5
-    median_sz = 3
-    gauss_sig = 2.0
-    MO_thresh_method = 'tri'
-    MO_cutoff_size = 1200
-    MO_thresh_adj = 0.7
-    fil_scale_1 = 1
-    fil_cut_1 = 0.005
-    fil_scale_2 = 2
-    fil_cut_2 = 0.005
-    fil_scale_3 = 0
-    fil_cut_3 = 0
-    fil_method = "3D"
+    median_sz = 4
+    gauss_sig = 1.34
+    dot_scale_1 = 5
+    dot_cut_1 = 0.09
+    dot_scale_2 = 2.5
+    dot_cut_2 = 0.07
+    dot_scale_3 = 1
+    dot_cut_3 = 0.01
+    filament_scale = 1
+    filament_cut = 0.15
     min_hole_w = 0
-    max_hole_w = 0
-    small_obj_w = 4
-    method = "3D"
+    max_hole_w = 25
+    small_obj_w = 3
 
-    return infer_ER(
+    return infer_lyso(
         in_img,
-        ER_ch,
         median_sz,
         gauss_sig,
-        MO_thresh_method,
-        MO_cutoff_size,
-        MO_thresh_adj,
-        fil_scale_1,
-        fil_cut_1,
-        fil_scale_2,
-        fil_cut_2,
-        fil_scale_3,
-        fil_cut_3,
-        fil_method,
+        dot_cut_1,
+        dot_scale_1,
+        dot_cut_2,
+        dot_scale_2,
+        dot_cut_3,
+        dot_scale_3,
+        filament_scale,
+        filament_cut,
         min_hole_w,
         max_hole_w,
         small_obj_w,
-        method)
+    )
 
 
-def infer_and_export_ER(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
+def infer_and_export_lyso(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
     """
-    infer ER and write inferred ER to ome.tif file
+    infer lyso and write inferred lyso to ome.tif file
 
     Parameters
     ------------
     in_img:
         a 3d  np.ndarray image of the inferred organelle (labels or boolean)
     meta_dict:
         dictionary of meta-data (ome)
@@ -201,23 +155,44 @@
         Path object where tiffs are written to
 
     Returns
     -------------
     exported file name
 
     """
-    er = fixed_infer_ER(in_img)
-    out_file_n = export_inferred_organelle(er, "ER", meta_dict, out_data_path)
-    print(f"inferred ER. wrote {out_file_n}")
-    return er
+    lyso = fixed_infer_lyso(in_img)
+    out_file_n = export_inferred_organelle(lyso, "lyso", meta_dict, out_data_path)
+    print(f"inferred lyso. wrote {out_file_n}")
+    return lyso
+
+
+def lyso_spot_filter(in_img: np.ndarray) -> np.ndarray:
+    """spot filter helper function for lyso"""
+    dot_scale_1 = 5
+    dot_cut_1 = 0.09
+    dot_scale_2 = 2.5
+    dot_cut_2 = 0.07
+    dot_scale_3 = 1
+    dot_cut_3 = 0.01
+    s2_param = [[dot_scale_1, dot_cut_1], [dot_scale_2, dot_cut_2], [dot_scale_3, dot_cut_3]]
+    return dot_2d_slice_by_slice_wrapper(in_img, s2_param)
+
+
+def lyso_filiment_filter(in_img: np.ndarray) -> np.ndarray:
+    """spot filter helper function for lyso (DEPRICATED)"""
+    filament_scale = 1
+    filament_cut = 0.15
+    f2_param = [[filament_scale, filament_cut]]
+    # f2_param = [[1, 0.15]]  # [scale_1, cutoff_1]
+    return filament_2d_wrapper(in_img, f2_param)
 
 
-def get_ER(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
+def get_lyso(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
     """
-    load endoplasmic_reticulum if it exists, otherwise calculate and write to ome.tif file
+    load lyso if it exists, otherwise calculate and write to ome.tif file
 
     Parameters
     ------------
     in_img:
         a 3d  np.ndarray image of the inferred organelle (labels or boolean)
     meta_dict:
         dictionary of meta-data (ome)
@@ -225,18 +200,20 @@
         Path object where tiffs are written to
 
     Returns
     -------------
     exported file name
 
     """
-
     try:
-        er = import_inferred_organelle("ER", meta_dict, out_data_path)
+        start = time.time()
+        lyso = import_inferred_organelle("lyso", meta_dict, out_data_path)
+        end = time.time()
+        print(f"loaded lyso in ({(end - start):0.2f}) sec")
     except:
         start = time.time()
         print("starting segmentation...")
-        er = infer_and_export_ER(in_img, meta_dict, out_data_path)
+        lyso = infer_and_export_lyso(in_img, meta_dict, out_data_path)
         end = time.time()
-        print(f"inferred (and exported) ER in ({(end - start):0.2f}) sec")
+        print(f"inferred (and exported) lyso in ({(end - start):0.2f}) sec")
 
-    return er
+    return lyso
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles/lipid.py` & `infer-subc-0.0.post1/infer_subc/organelles/lipid.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,145 +14,108 @@
 from infer_subc.constants import LD_CH
 
 
 ##########################
 #  infer_LD
 ##########################
 def infer_LD(
-            in_img: np.ndarray,
-            LD_ch: str,
-            median_sz: int,
-            gauss_sig: float,
-            method: str,
-            thresh_factor: float,
-            thresh_min: float,
-            thresh_max: float,
-            min_hole_w: int,
-            max_hole_w: int,
-            small_obj_w: int,
-            fill_filter_method: str
-            ) -> np.ndarray:
+    in_img: np.ndarray,
+    median_sz: int,
+    gauss_sig: float,
+    method: str,
+    thresh_factor: float,
+    thresh_min: float,
+    thresh_max: float,
+    max_hole_w: int,
+    small_obj_w: int,
+) -> np.ndarray:
     """
-    Procedure to infer LD from linearly unmixed input.
+    Procedure to infer peroxisome from linearly unmixed input.
 
     Parameters
     ------------
-    in_img: 
-        a 3D image containing all the channels (CZYX)
-    LD_ch:
-        index of the LD channel in the input image
-    median_sz: 
+    in_img:
+        a 3d image containing all the channels
+    median_sz:
         width of median filter for signal
-    gauss_sig: 
+    gauss_sig:
         sigma for gaussian smoothing of  signal
-    method: 
+    method:
         method for applying threshold.  "otsu"  or "li", "triangle", "median", "ave", "sauvola","multi_otsu","muiltiotsu"
     thresh_factor:
         scaling value for threshold
     thresh_min:
         absolute minumum for threshold
     thresh_max:
         absolute maximum for threshold
-    max_hole_w: 
-        hole filling cutoff for LD post-processing
-    small_obj_w: 
-        minimu object size cutoff for LD post-processing
-    fill_filter_method:
-        determines if small hole filling and small object removal should be run 'sice-by-slice' or in '3D'
+    max_hole_w:
+        hole filling cutoff for lipid post-processing
+    small_obj_w:
+        minimu object size cutoff for lipid post-processing
     Returns
     -------------
-    LD_object
-        mask defined extent of LD object
+    peroxi_object
+        mask defined extent of peroxisome object
     """
-
+    LD_ch = LD_CH
     ###################
     # EXTRACT
-    ###################    
+    ###################
     lipid = select_channel_from_raw(in_img, LD_ch)
-    
     ###################
     # PRE_PROCESSING
-    ###################                         
-    lipid =  scale_and_smooth(lipid,
-                              median_size = median_sz, 
-                              gauss_sigma = gauss_sig)
-
+    ###################
+    lipid = scale_and_smooth(lipid, median_sz=median_sz, gauss_sig=gauss_sig)
 
     ###################
     # CORE_PROCESSING
     ###################
-    bw = apply_threshold(lipid, 
-                        method= method, 
-                        thresh_factor=thresh_factor, 
-                        thresh_min=thresh_min, 
-                        thresh_max=thresh_max)
-
+    bw = apply_threshold(
+        lipid, method=method, thresh_factor=thresh_factor, thresh_min=thresh_min, thresh_max=thresh_max
+    )
 
     ###################
     # POST_PROCESSING
     ###################
     # min_hole_w = 0
-    struct_obj = fill_and_filter_linear_size(bw, 
-                                             hole_min=min_hole_w, 
-                                             hole_max=max_hole_w, 
-                                             min_size=small_obj_w,
-                                             method=fill_filter_method)
+    struct_obj = fill_and_filter_linear_size(bw, hole_min=0, hole_max=max_hole_w, min_size=small_obj_w)
 
-    ###################
-    # LABELING
-    ###################
-    struct_obj1 = label_uint16(struct_obj)
-
-    return struct_obj1
+    return label_uint16(struct_obj)
 
 
 ##########################
 #  fixed_infer_LD
 ##########################
 def fixed_infer_LD(in_img: np.ndarray) -> np.ndarray:
     """
-    Procedure to infer LD from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. "hard coded"
+    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. "hard coded"
 
     Parameters
     ------------
-    in_img: 
+    in_img:
         a 3d image containing all the channels
 
     Returns
     -------------
-    LD_object
-        mask defined extent of lipid droplets
+    LD_body_object
+        mask defined extent of liipid body
 
     """
-    LD_ch = 6
-    median_sz = 2   
-    gauss_sig = 1.34
+    median_sz = 0
+    gauss_sig = 2.34
     method = "otsu"
-    threshold_factor = 0.8
-    thresh_min = 0.05
+    threshold_factor = 0.99  # from cellProfiler
+    thresh_min = 0.5
     thresh_max = 1.0
-    min_hole_w = 0
     max_hole_w = 2.5
-    small_obj_w = 1
-    fill_filter_method = "3D"
+    small_obj_w = 4
 
     return infer_LD(
-        in_img,
-        LD_ch,  
-        median_sz, 
-        gauss_sig, 
-        method, 
-        threshold_factor, 
-        thresh_min, 
-        thresh_max, 
-        min_hole_w,
-        max_hole_w, 
-        small_obj_w,
-        fill_filter_method)
-
+        in_img, median_sz, gauss_sig, method, threshold_factor, thresh_min, thresh_max, max_hole_w, small_obj_w
+    )
 
 
 def infer_and_export_LD(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
     """
     infer lipid bodies and write inferred lipid to ome.tif file
 
     Parameters
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles/nuclei.py` & `infer-subc-0.0.post1/infer_subc/organelles/nuclei.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,135 +19,110 @@
 )
 from infer_subc.constants import NUC_CH
 
 
 ##########################
 #  infer_nuclei_fromlabel
 ##########################
-def infer_nuclei_fromlabel(in_img: np.ndarray, 
-                           nuc_ch: Union[int,None],
-                           median_size: int, 
-                           gauss_sigma: float,
-                           thresh_factor: float,
-                           thresh_min: float,
-                           thresh_max: float,
-                           min_hole_width: int,
-                           max_hole_width: int,
-                           small_obj_width: int,
-                           fill_filter_method: str
-                           ) -> np.ndarray:
+def infer_nuclei_fromlabel(
+    in_img: np.ndarray,
+    nuc_ch: Union[int, None],
+    median_sz: int,
+    gauss_sig: float,
+    thresh_factor: float,
+    thresh_min: float,
+    thresh_max: float,
+    max_hole_w: int,
+    small_obj_w: int,
+) -> np.ndarray:
     """
     Procedure to infer nuclei from linearly unmixed input.
 
     Parameters
     ------------
-    in_img: np.ndarray
-        a 3d image containing all the channels (CZYX)
-    nuc_ch:
-        index of the nuc channel in the input image
-    median_size: int
+    in_img:
+        a 3d image containing all the channels; np.ndarray
+    median_sz:
         width of median filter for signal
-    gauss_sigma: float
+    gauss_sig:
         sigma for gaussian smoothing of  signal
-    thresh_factor: float
+    thresh_factor:
         adjustment factor for log Li threholding
-    thresh_min: float
+    thresh_min:
         abs min threhold for log Li threholding
-    thresh_max: float
+    thresh_max:
         abs max threhold for log Li threholding
-    min_hole_w: 
-        minimum size for hole filling for cellmask signal post-processing
-    max_hole_w: 
-        hole filling cutoff for nuclei signal post-processing
-    small_obj_w: 
-        minimum object size cutoff for nuclei signal post-processing
-    fill_filter_method:
-        determines if small hole filling and small object removal should be run 'sice-by-slice' or in '3D'
+    max_hole_w:
+        hole filling cutoff for nuclei post-processing0
+    small_obj_w:
+        minimu object size cutoff for nuclei post-processing
 
     Returns
     -------------
     nuclei_object
         mask defined extent of NU
-    
+
     """
-    ###################
-    # EXTRACT
-    ###################                
-    nuclei = select_channel_from_raw(in_img, nuc_ch)
 
     ###################
     # PRE_PROCESSING
-    ###################                
-    nuclei =  scale_and_smooth(nuclei,
-                        median_size = median_size, 
-                        gauss_sigma = gauss_sigma)
+    ###################
+    if nuc_ch is None:
+        nuc_ch = NUC_CH
+
+    nuclei = select_channel_from_raw(in_img, nuc_ch)
+
+    nuclei = scale_and_smooth(nuclei, median_sz=median_sz, gauss_sig=gauss_sig)
 
     ###################
     # CORE_PROCESSING
     ###################
-    nuclei_object = apply_log_li_threshold(nuclei, 
-                                           thresh_factor=thresh_factor, 
-                                           thresh_min=thresh_min, 
-                                           thresh_max=thresh_max)
+    nuclei_object = apply_log_li_threshold(
+        nuclei, thresh_factor=thresh_factor, thresh_min=thresh_min, thresh_max=thresh_max
+    )
 
     ###################
     # POST_PROCESSING
     ###################
-    nuclei_object = fill_and_filter_linear_size(nuclei_object, 
-                                                hole_min=min_hole_width, 
-                                                hole_max=max_hole_width, 
-                                                min_size=small_obj_width,
-                                                method=fill_filter_method)
-
-    nuclei_labels = label_uint16(nuclei_object)
- 
-    return nuclei_labels
+    nuclei_object = fill_and_filter_linear_size(nuclei_object, hole_min=0, hole_max=max_hole_w, min_size=small_obj_w)
+
+    return label_uint16(nuclei_object)
+    # return get_interior_labels(nuclei_object)
 
 
 ##########################
 #  fixed_infer_nuclei
 ##########################
-def fixed_infer_nuclei_fromlabel(in_img: np.ndarray) -> np.ndarray:
+def fixed_infer_nuclei(in_img: np.ndarray) -> np.ndarray:
     """
     Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. "hard coded"
 
     Parameters
     ------------
-    in_img: np.ndarray
+    in_img:
         a 3d image containing all the channels
- 
+
     Returns
     -------------
     nuclei_object
         inferred nuclei
-    nap
+
     """
     nuc_ch = NUC_CH
-    median_size = 4   
-    gauss_sigma = 1.34
+    median_sz = 4
+    gauss_sig = 1.34
     thresh_factor = 0.9
     thresh_min = 0.1
     thresh_max = 1.0
-    min_hole_width = 0
-    max_hole_width = 25
-    small_obj_width = 15
-    fill_filter_method = '3D'
-
-    return infer_nuclei_fromlabel( in_img,
-                                    nuc_ch,
-                                    median_size,
-                                    gauss_sigma,
-                                    thresh_factor,
-                                    thresh_min,
-                                    thresh_max,
-                                    min_hole_width,
-                                    max_hole_width,
-                                    small_obj_width,
-                                    fill_filter_method)
+    max_hole_w = 25
+    small_obj_w = 15
 
+    return infer_nuclei_fromlabel(
+        in_img, nuc_ch, median_sz, gauss_sig, thresh_factor, thresh_min, thresh_max, max_hole_w, small_obj_w
+    )
 
 
 def infer_and_export_nuclei(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
     """
     infer nuclei and write inferred nuclei to ome.tif file
 
     Parameters
@@ -160,17 +135,17 @@
         Path object where tiffs are written to
 
     Returns
     -------------
     exported file name
 
     """
-    nuclei = fixed_infer_nuclei_fromlabel(in_img)
+    nuclei = fixed_infer_nuclei(in_img)
 
-    out_file_n = export_inferred_organelle(nuclei, "nuclei", meta_dict, out_data_path)
+    out_file_n = export_inferred_organelle(nuclei, "nuc", meta_dict, out_data_path)
     print(f"inferred nuclei. wrote {out_file_n}")
     return nuclei
 
 
 def get_nuclei(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
     """
     load nucleus if it exists, otherwise calculate and write to ome.tif file
@@ -188,56 +163,25 @@
     Returns
     -------------
     exported file name
 
     """
 
     try:
-        nuclei = import_inferred_organelle("nuclei", meta_dict, out_data_path)
+        nuclei = import_inferred_organelle("nuc", meta_dict, out_data_path)
     except:
         start = time.time()
         print("starting segmentation...")
         nuclei = infer_and_export_nuclei(in_img, meta_dict, out_data_path)
         end = time.time()
         print(f"inferred nuclei in ({(end - start):0.2f}) sec")
 
     return nuclei
 
 
-def get_nucleus(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
-    """
-    load nucleus if it exists, otherwise calculate and write to ome.tif file
-
-    Parameters
-    ------------
-    in_img:
-        a 3d  np.ndarray image of the inferred organelle (labels or boolean)
-
-    meta_dict:
-        dictionary of meta-data (ome)
-    out_data_path:
-        Path object where tiffs are written to
-
-    Returns
-    -------------
-    exported file name
-
-    """
-
-    try:
-        nucleus = import_inferred_organelle("nuc", meta_dict, out_data_path)
-    except:
-        start = time.time()
-        print("starting segmentation...")
-        nucleus = infer_and_export_nuclei(in_img, meta_dict, out_data_path)
-        end = time.time()
-        print(f"inferred nucleus in ({(end - start):0.2f}) sec")
-
-    return nucleus
-
 # def infer_nuclei_fromlabel_AICS(in_img: np.ndarray, meta_dict: Dict, out_data_path: Path) -> np.ndarray:
 #     """
 #     load nucleus if it exists, otherwise calculate and write to ome.tif file
 
 #     Parameters
 #     ------------
 #     in_img:
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles/qc.py` & `infer-subc-0.0.post1/infer_subc/organelles/qc.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/all_functions.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/all_functions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9058922182468693%*

 * *Differences: {"'apply_threshold'": "{'name': 'Apply Threshold'}",*

 * * "'choose_max_label_cellmask_union_nucleus'": "{'name': 'get cellmask + nuclei for largest signal "*

 * *                                              "label', 'parameters': {replace: "*

 * *                                              "OrderedDict([('interior_labels', "*

 * *                                              "OrderedDict([('widget_type', 'drop-down'), "*

 * *                                              "('data_type', 'bool'), ('options', [True, "*

 * *              […]*

```diff
@@ -60,15 +60,15 @@
     "apply_mask": {
         "name": "apply mask",
         "parameters": null,
         "python::function": "apply_mask",
         "python::module": "infer_subc.core.img"
     },
     "apply_threshold": {
-        "name": "Apply basic threshold",
+        "name": "Apply Threshold",
         "parameters": {
             "method": {
                 "data_type": "str",
                 "options": [
                     "otsu",
                     "li",
                     "triangle",
@@ -99,31 +99,23 @@
                 "widget_type": "slider"
             }
         },
         "python::function": "apply_threshold",
         "python::module": "infer_subc.core.img"
     },
     "choose_max_label_cellmask_union_nucleus": {
-        "name": "Select one cellmask/nuclei based on signal",
+        "name": "get cellmask + nuclei for largest signal label",
         "parameters": {
-            "interior_labels_only": {
+            "interior_labels": {
                 "data_type": "bool",
                 "options": [
                     true,
                     false
                 ],
                 "widget_type": "drop-down"
-            },
-            "watershed_method": {
-                "data_type": "str",
-                "options": [
-                    "3D",
-                    "slice-by-slice"
-                ],
-                "widget_type": "drop-down"
             }
         },
         "python::function": "choose_max_label_cellmask_union_nucleus",
         "python::module": "infer_subc.organelles.cellmask"
     },
     "choose_max_label_soma_union_nucleus": {
         "name": "get cellmask UNION nuclei for largest signal label",
@@ -157,92 +149,14 @@
                 ],
                 "widget_type": "drop-down"
             }
         },
         "python::function": "compute_3d_hessian_matrix",
         "python::module": "aicssegmentation.core.hessian"
     },
-    "dot_filter_3": {
-        "name": "'Dot' thresholding method (AICSSeg)",
-        "parameters": {
-            "dot_cutoff_1": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "dot_cutoff_2": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "dot_cutoff_3": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "dot_scale_1": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "dot_scale_2": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "dot_scale_3": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "method": {
-                "data_type": "str",
-                "options": [
-                    "3D",
-                    "slice_by_slice"
-                ],
-                "widget_type": "drop-down"
-            }
-        },
-        "python::function": "dot_filter_3",
-        "python::module": "infer_subc.core.img"
-    },
-    "dot_filter_3D": {
-        "name": "Spot Filter 3D",
-        "parameters": {
-            "cutoff": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "log_sigma": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            }
-        },
-        "python::function": "dot_3d",
-        "python::module": "aicssegmentation.core.seg_dot"
-    },
     "edge_preserving_smoothing": {
         "name": "Edge Preserving Smoothing",
         "parameters": null,
         "python::function": "edge_preserving_smoothing_3d",
         "python::module": "aicssegmentation.core.pre_processing_utils"
     },
     "erosion": {
@@ -293,71 +207,14 @@
                 "min": 0,
                 "widget_type": "slider"
             }
         },
         "python::function": "filament_filter",
         "python::module": "infer_subc.core.img"
     },
-    "filament_filter_3": {
-        "name": "'Filament' thresholding method (AICSSeg)",
-        "parameters": {
-            "filament_cutoff_1": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 2,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "filament_cutoff_2": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "filament_cutoff_3": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "filament_scale_1": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "filament_scale_2": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "filament_scale_3": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "method": {
-                "data_type": "str",
-                "options": [
-                    "3D",
-                    "slice_by_slice"
-                ],
-                "widget_type": "drop-down"
-            }
-        },
-        "python::function": "filament_filter_3",
-        "python::module": "infer_subc.core.img"
-    },
     "filament_filter_3D": {
         "name": "Filament Filter 3D",
         "parameters": {
             "cutoff": {
                 "data_type": "float",
                 "increment": 0.005,
                 "max": 0.5,
@@ -395,15 +252,15 @@
                 }
             ]
         },
         "python::function": "vesselnessSliceBySlice",
         "python::module": "aicssegmentation.core.vessel"
     },
     "fill_and_filter_linear_size": {
-        "name": "Remove small holes and objects",
+        "name": "fill holes and filter small objects - linear space constant",
         "parameters": {
             "hole_max": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 80,
                 "min": 0,
                 "widget_type": "slider"
@@ -745,15 +602,15 @@
                 "widget_type": "slider"
             }
         },
         "python::function": "infer_cellmask_fromaggr_MCZ",
         "python::module": "infer_subc.organelles.cellmask"
     },
     "infer_cytoplasm": {
-        "name": "Segment cytoplasm",
+        "name": "infer infer_cytoplasm",
         "parameters": {
             "erode_nuclei": {
                 "data_type": "bool",
                 "options": [
                     true,
                     false
                 ],
@@ -1007,52 +864,45 @@
                 "widget_type": "slider"
             }
         },
         "python::function": "infer_mito",
         "python::module": "infer_subc.organelles.mitochondria"
     },
     "infer_nuclei_fromlabel": {
-        "name": "Segment nuclei (from label)",
+        "name": "infer nuclei",
         "parameters": {
-            "gauss_sigma": {
+            "gauss_sig": {
                 "data_type": "float",
                 "increment": 0.25,
                 "max": 15.0,
                 "min": 1.25,
                 "widget_type": "slider"
             },
-            "max_hole_width": {
+            "max_hole_w": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 40,
                 "min": 4,
                 "widget_type": "slider"
             },
-            "median_size": {
+            "median_sz": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 15,
                 "min": 1,
                 "widget_type": "slider"
             },
-            "min_hole_width": {
-                "data_type": "int",
-                "increment": 1,
-                "max": 40,
-                "min": 0,
-                "widget_type": "slider"
-            },
             "nuc_ch": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "small_obj_width": {
+            "small_obj_w": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 50,
                 "min": 1,
                 "widget_type": "slider"
             },
             "thresh_factor": {
@@ -1200,27 +1050,27 @@
     "label": {
         "name": "label objects",
         "parameters": null,
         "python::function": "label",
         "python::module": "skimage.measure"
     },
     "label_bool_as_uint16": {
-        "name": "Create one object (as uint16)",
+        "name": "label single bool object as uint16",
         "parameters": null,
         "python::function": "label_bool_as_uint16",
         "python::module": "infer_subc.core.img"
     },
     "label_uint16": {
-        "name": "Label objects",
+        "name": "label objects to uint16",
         "parameters": null,
         "python::function": "label_uint16",
         "python::module": "infer_subc.core.img"
     },
     "logical_or": {
-        "name": "Combine segmentations (logical or)",
+        "name": "logical or",
         "parameters": null,
         "python::function": "logical_or",
         "python::module": "numpy"
     },
     "lyso_filiment_filter": {
         "name": "lysosome filiment filter",
         "parameters": null,
@@ -1230,88 +1080,88 @@
     "lyso_spot_filter": {
         "name": "lyso spot filter (fixed)",
         "parameters": null,
         "python::function": "lyso_spot_filter",
         "python::module": "infer_subc.organelles.lysosome"
     },
     "make_aggregate": {
-        "name": "Create composite image",
+        "name": "weighted sum wrapper (plugin)",
         "parameters": {
-            "rescale": {
+            "scale_min_max": {
                 "data_type": "bool",
                 "options": [
                     true,
                     false
                 ],
                 "widget_type": "drop-down"
             },
-            "weight_ch0": {
+            "w0": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch1": {
+            "w1": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch2": {
+            "w2": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch3": {
+            "w3": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch4": {
+            "w4": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch5": {
+            "w5": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch6": {
+            "w6": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch7": {
+            "w7": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch8": {
+            "w8": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "weight_ch9": {
+            "w9": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             }
         },
@@ -1335,38 +1185,38 @@
     "masked_inverted_watershed": {
         "name": "watershed on inverted image and masked",
         "parameters": null,
         "python::function": "masked_inverted_watershed",
         "python::module": "infer_subc.core.img"
     },
     "masked_object_thresh": {
-        "name": "Global + local threshold (AICSSeg - MO)",
+        "name": "Masked Object Threshold wrapper for widgets",
         "parameters": {
             "cutoff_size": {
                 "data_type": "int",
                 "increment": 50,
                 "max": 2000,
                 "min": 0,
                 "widget_type": "slider"
             },
-            "global_method": {
+            "th_adjust": {
+                "data_type": "float",
+                "increment": 0.02,
+                "max": 2,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "th_method": {
                 "data_type": "str",
                 "options": [
                     "triangle",
                     "median",
                     "ave_tri_med"
                 ],
                 "widget_type": "drop-down"
-            },
-            "local_adjust": {
-                "data_type": "float",
-                "increment": 0.02,
-                "max": 2,
-                "min": 0,
-                "widget_type": "slider"
             }
         },
         "python::function": "masked_object_thresh",
         "python::module": "infer_subc.core.img"
     },
     "masked_object_treshold_combined": {
         "name": "Masked Object Threshold - Combined",
@@ -1497,18 +1347,18 @@
     },
     "min_max_intensity_normalization": {
         "name": "Min Max Intesity Normalization",
         "parameters": null,
         "python::function": "min_max_intensity_normalization",
         "python::module": "infer_subc.core.img"
     },
-    "non_linear_cellmask_transform": {
-        "name": "Log transform + Scharr edge detection",
+    "non_linear_cellmask_transform_MCZ": {
+        "name": "non-linear distortion to fill out cellmask",
         "parameters": null,
-        "python::function": "non_linear_cellmask_transform",
+        "python::function": "non_linear_cellmask_transform_MCZ",
         "python::module": "infer_subc.organelles.cellmask"
     },
     "non_linear_soma_transform_MCZ": {
         "name": "non-linear filter of cellmask signal (MCZ-cellprofiler)",
         "parameters": null,
         "python::function": "non_linear_soma_transform_MCZ",
         "python::module": "infer_subc.organelles"
@@ -1549,42 +1399,42 @@
     "remove_index_object": {
         "name": "Remove Index Object",
         "parameters": null,
         "python::function": "remove_index_object",
         "python::module": "aicssegmentation.core.utils"
     },
     "scale_and_smooth": {
-        "name": "Rescale and smooth image",
+        "name": "scale and smooth",
         "parameters": {
-            "gauss_sigma": {
+            "gauss_sig": {
                 "data_type": "float",
                 "increment": 0.25,
                 "max": 15.0,
-                "min": 0,
+                "min": 1.25,
                 "widget_type": "slider"
             },
-            "median_size": {
+            "median_sz": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 15,
-                "min": 0,
+                "min": 1,
                 "widget_type": "slider"
             }
         },
         "python::function": "scale_and_smooth",
         "python::module": "infer_subc.core.img"
     },
     "segmentation_xor": {
         "name": "Segmentation XOR",
         "parameters": null,
         "python::function": "segmentation_xor",
         "python::module": "aicssegmentation.core.utils"
     },
     "select_channel_from_raw": {
-        "name": "Select a channel for segmentation",
+        "name": "select a channel ",
         "parameters": {
             "chan": {
                 "data_type": "int",
                 "options": [
                     0,
                     1,
                     2,
@@ -1748,14 +1598,84 @@
                 "min": 0,
                 "widget_type": "slider"
             }
         },
         "python::function": "soma_aggregate",
         "python::module": "infer_subc.organelles.cellmask"
     },
+    "spot_filter_3": {
+        "name": "spot filter thresholding (3 scales)",
+        "parameters": {
+            "dot_cut_1": {
+                "data_type": "float",
+                "increment": 0.001,
+                "max": 0.5,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "dot_cut_2": {
+                "data_type": "float",
+                "increment": 0.001,
+                "max": 0.5,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "dot_cut_3": {
+                "data_type": "float",
+                "increment": 0.001,
+                "max": 0.5,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "dot_scale_1": {
+                "data_type": "float",
+                "increment": 0.05,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "dot_scale_2": {
+                "data_type": "float",
+                "increment": 0.05,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "dot_scale_3": {
+                "data_type": "float",
+                "increment": 0.05,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            }
+        },
+        "python::function": "spot_filter_3",
+        "python::module": "infer_subc.core.img"
+    },
+    "spot_filter_3D": {
+        "name": "Spot Filter 3D",
+        "parameters": {
+            "cutoff": {
+                "data_type": "float",
+                "increment": 0.001,
+                "max": 0.5,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "log_sigma": {
+                "data_type": "float",
+                "increment": 0.05,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            }
+        },
+        "python::function": "dot_3d",
+        "python::module": "aicssegmentation.core.seg_dot"
+    },
     "spot_filter_slice_by_slice": {
         "name": "Spot Filter Slice by Slice",
         "parameters": {
             "cutoff": {
                 "data_type": "float",
                 "increment": 0.001,
                 "max": 1,
@@ -1782,15 +1702,15 @@
     "stack_masks": {
         "name": "stack masks",
         "parameters": null,
         "python::function": "stack_masks",
         "python::module": "infer_subc.core.img"
     },
     "topology_preserving_thinning": {
-        "name": "Thin segmentation (Topology preserving)",
+        "name": "Topology Preserving Thinning",
         "parameters": {
             "min_thickness": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 10,
                 "min": 1,
                 "widget_type": "slider"
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.2.lyso.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.1.masks.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6152777777777778%*

 * *Differences: {"'1'": "{'function': 'infer_nuclei_fromlabel', 'parameter_values': {replace: "*

 * *        "OrderedDict([('nuc_ch', 0), ('median_sz', 3), ('gauss_sig', 4.5), ('thresh_factor', "*

 * *        "0.85), ('thresh_min', 0.1), ('thresh_max', 1.0), ('max_hole_w', 25), ('small_obj_w', "*

 * *        "15)])}, 'annotation': 'get  nuclei segmentation: 1'}",*

 * * "'2'": "{'category': 'extraction', 'function': 'make_aggregate', 'parameter_values': {replace: "*

 * *        "OrderedDict([('w0', 0), ('w1', 6), ('w2', 0), ('w3', 2), ('w4', 0), (' […]*

```diff
@@ -1,78 +1,111 @@
 {
     "1": {
-        "annotation": "basic lyso segmentation: 1",
+        "annotation": "get  nuclei segmentation: 1",
         "category": "extraction",
-        "function": "select_channel_from_raw",
+        "function": "infer_nuclei_fromlabel",
         "parameter_values": {
-            "chan": 1
+            "gauss_sig": 4.5,
+            "max_hole_w": 25,
+            "median_sz": 3,
+            "nuc_ch": 0,
+            "small_obj_w": 15,
+            "thresh_factor": 0.85,
+            "thresh_max": 1.0,
+            "thresh_min": 0.1
         },
         "parent": 0
     },
     "2": {
-        "annotation": "basic lyso segmentation: 2",
-        "category": "preprocessing",
-        "function": "scale_and_smooth",
+        "annotation": " this creates an aggregate signal for the cellmask",
+        "category": "extraction",
+        "function": "make_aggregate",
         "parameter_values": {
-            "gauss_sigma": 1.34,
-            "median_size": 3
+            "scale_min_max": true,
+            "w0": 0,
+            "w1": 6,
+            "w2": 0,
+            "w3": 2,
+            "w4": 0,
+            "w5": 1,
+            "w6": 0,
+            "w7": 0,
+            "w8": 0,
+            "w9": 0
         },
-        "parent": 1
+        "parent": 0
     },
     "3": {
-        "annotation": "basic lyso - spot filter: 3",
-        "category": "core",
-        "function": "dot_filter_3",
+        "annotation": "basic nuclei segmentation: 3",
+        "category": "preprocessing",
+        "function": "scale_and_smooth",
         "parameter_values": {
-            "dot_cutoff_1": 0.09,
-            "dot_cutoff_2": 0.07,
-            "dot_cutoff_3": 0.01,
-            "dot_scale_1": 5,
-            "dot_scale_2": 2.5,
-            "dot_scale_3": 1,
-            "method": "3D"
+            "gauss_sig": 4.5,
+            "median_sz": 9
         },
         "parent": 2
     },
     "4": {
-        "annotation": "basic lyso - filament filter: 4",
-        "category": "core",
-        "function": "filament_filter_3",
-        "parameter_values": {
-            "filament_cutoff_1": 0.15,
-            "filament_cutoff_2": 0,
-            "filament_cutoff_3": 0,
-            "filament_scale_1": 1.0,
-            "filament_scale_2": 0,
-            "filament_scale_3": 0,
-            "method": "3D"
-        },
-        "parent": 2
+        "annotation": "basic nuclei segmentation: 4",
+        "category": "preprocessing",
+        "function": "non_linear_cellmask_transform_MCZ",
+        "parent": 3
     },
     "5": {
-        "annotation": "basic lyso - combine spot+filament: 5",
+        "annotation": "basic nuclei segmentation: 5",
         "category": "core",
-        "function": "logical_or",
-        "parent": [
-            3,
-            4
-        ]
+        "function": "masked_object_thresh",
+        "parameter_values": {
+            "cutoff_size": 200,
+            "th_adjust": 0.75,
+            "th_method": "ave_tri_med"
+        },
+        "parent": 4
     },
     "6": {
-        "annotation": "basic lyso - fill/filter: 6",
+        "annotation": "basic nuclei segmentation: 6",
         "category": "postprocessing",
         "function": "fill_and_filter_linear_size",
         "parameter_values": {
-            "hole_max": 25,
+            "hole_max": 45,
             "hole_min": 0,
             "method": "slice_by_slice",
-            "min_size": 0
+            "min_size": 30
         },
         "parent": 5
     },
     "7": {
-        "annotation": "label to uint16 for export 7",
+        "annotation": "basic cellmask segmentation: 7",
+        "category": "postpostprocessing",
+        "function": "choose_max_label_cellmask_union_nucleus",
+        "parameter_values": {
+            "interior_labels": true
+        },
+        "parent": [
+            3,
+            6,
+            1
+        ]
+    },
+    "8": {
+        "annotation": "infer cytoplasm: 8",
         "category": "postpostprocessing",
-        "function": "label_uint16",
-        "parent": 6
+        "function": "infer_cytoplasm",
+        "parameter_values": {
+            "erode_nuclei": true
+        },
+        "parent": [
+            1,
+            7
+        ]
+    },
+    "9": {
+        "annotation": "export  canonical masks (nuc,cellmask, cyto) 9",
+        "category": "export",
+        "function": "stack_masks",
+        "parent": [
+            1,
+            7,
+            8
+        ]
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.3.mito.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48999999999999994%*

 * *Differences: {"'1'": "{'function': 'fixed_get_optimal_Z_img', delete: ['parameter_values', 'annotation']}",*

 * * "'10'": "OrderedDict([('category', 'postprocessing'), ('function', 'size_filter_2D'), "*

 * *         "('parameter_values', OrderedDict([('min_size', 4)])), ('parent', 9)])",*

 * * "'2'": "{'category': 'extraction', 'function': 'fixed_infer_cellmask_fromaggr', delete: "*

 * *        "['parameter_values', 'annotation']}",*

 * * "'3'": "{'category': 'extraction', 'function': 'fixed_infer_nuclei', 'parent': [1, 2], delete: "*

 * *        "[ […]*

```diff
@@ -1,78 +1,74 @@
 {
     "1": {
-        "annotation": "basic mito segmentation: 1",
         "category": "extraction",
-        "function": "select_channel_from_raw",
-        "parameter_values": {
-            "chan": 2
-        },
+        "function": "fixed_get_optimal_Z_img",
         "parent": 0
     },
-    "2": {
-        "annotation": "basic mito segmentation: 2",
-        "category": "preprocessing",
-        "function": "scale_and_smooth",
+    "10": {
+        "category": "postprocessing",
+        "function": "size_filter_2D",
         "parameter_values": {
-            "gauss_sigma": 1.34,
-            "median_size": 3
+            "min_size": 4
         },
+        "parent": 9
+    },
+    "2": {
+        "category": "extraction",
+        "function": "fixed_infer_cellmask_fromaggr",
         "parent": 1
     },
     "3": {
-        "annotation": "basic mito - spot filter: 3",
-        "category": "core",
-        "function": "dot_filter_3",
-        "parameter_values": {
-            "dot_cutoff_1": 0.05,
-            "dot_cutoff_2": 0,
-            "dot_cutoff_3": 0,
-            "dot_scale_1": 1.5,
-            "dot_scale_2": 0,
-            "dot_scale_3": 0,
-            "method": "3D"
-        },
-        "parent": 2
+        "category": "extraction",
+        "function": "fixed_infer_nuclei",
+        "parent": [
+            1,
+            2
+        ]
     },
     "4": {
-        "annotation": "basic mito - filament filter: 4",
-        "category": "core",
-        "function": "filament_filter_3",
+        "category": "extraction",
+        "function": "infer_cytoplasm",
         "parameter_values": {
-            "filament_cutoff_1": 0.15,
-            "filament_cutoff_2": 0,
-            "filament_cutoff_3": 0,
-            "filament_scale_1": 1.0,
-            "filament_scale_2": 0,
-            "filament_scale_3": 0,
-            "method": "3D"
+            "erode_nuclei": true
         },
-        "parent": 2
-    },
-    "5": {
-        "annotation": "basic mito - combine spot+filament: 5",
-        "category": "core",
-        "function": "logical_or",
         "parent": [
-            3,
-            4
+            2,
+            3
         ]
     },
-    "6": {
-        "annotation": "basic mito - fill/filter: 6",
-        "category": "postprocessing",
-        "function": "fill_and_filter_linear_size",
+    "5": {
+        "category": "extraction",
+        "function": "select_channel_from_raw",
         "parameter_values": {
-            "hole_max": 0,
-            "hole_min": 0,
-            "method": "3D",
-            "min_size": 3
+            "chan": 5
         },
+        "parent": 1
+    },
+    "6": {
+        "category": "preprocessing",
+        "function": "min_max_intensity_normalization",
         "parent": 5
     },
     "7": {
-        "annotation": "label to uint16 for export 5",
-        "category": "postpostprocessing",
-        "function": "label_uint16",
+        "category": "preprocessing",
+        "function": "edge_preserving_smoothing",
         "parent": 6
+    },
+    "8": {
+        "category": "core",
+        "function": "filament_filter",
+        "parameter_values": {
+            "filament_cut": 0.15,
+            "filament_scale": 1.0
+        },
+        "parent": 7
+    },
+    "9": {
+        "category": "postprocessing",
+        "function": "apply_mask",
+        "parent": [
+            8,
+            4
+        ]
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.4.golgi.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.2.lyso.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7156250000000001%*

 * *Differences: {"'1'": "{'parameter_values': {'chan': 1}, 'annotation': 'basic lyso segmentation: 1'}",*

 * * "'2'": "{'parameter_values': {replace: OrderedDict([('median_sz', 4), ('gauss_sig', 1.4)])}, "*

 * *        "'annotation': 'basic lyso segmentation: 2'}",*

 * * "'3'": "{'function': 'spot_filter_3', 'parameter_values': {replace: OrderedDict([('dot_scale_1', "*

 * *        "5), ('dot_cut_1', 0.09), ('dot_scale_2', 2.5), ('dot_cut_2', 0.07), ('dot_scale_3', 1), "*

 * *        "('dot_cut_3', 0.01)])}, 'annotation': 'basic lyso - spot filter: […]*

```diff
@@ -1,84 +1,72 @@
 {
     "1": {
-        "annotation": "basic golgi segmentation: 1",
+        "annotation": "basic lyso segmentation: 1",
         "category": "extraction",
         "function": "select_channel_from_raw",
         "parameter_values": {
-            "chan": 3
+            "chan": 1
         },
         "parent": 0
     },
     "2": {
-        "annotation": "basic golgi segmentation: 2",
+        "annotation": "basic lyso segmentation: 2",
         "category": "preprocessing",
         "function": "scale_and_smooth",
         "parameter_values": {
-            "gauss_sigma": 1.4,
-            "median_size": 4
+            "gauss_sig": 1.4,
+            "median_sz": 4
         },
         "parent": 1
     },
     "3": {
-        "annotation": "basic golgi - mo: 3",
+        "annotation": "basic lyso - spot filter: 3",
         "category": "core",
-        "function": "masked_object_thresh",
+        "function": "spot_filter_3",
         "parameter_values": {
-            "cutoff_size": 1200,
-            "global_method": "triangle",
-            "local_adjust": 1
+            "dot_cut_1": 0.09,
+            "dot_cut_2": 0.07,
+            "dot_cut_3": 0.01,
+            "dot_scale_1": 5,
+            "dot_scale_2": 2.5,
+            "dot_scale_3": 1
         },
         "parent": 2
     },
     "4": {
-        "annotation": "basic golgi - thinning filter: 4",
+        "annotation": "basic lyso - filament filter: 4",
         "category": "core",
-        "function": "topology_preserving_thinning",
+        "function": "filament_filter",
         "parameter_values": {
-            "min_thickness": 1.6,
-            "thin": 1
-        },
-        "parent": 3
-    },
-    "5": {
-        "annotation": "basic golgi - spot filter: 5",
-        "category": "core",
-        "function": "dot_filter_3",
-        "parameter_values": {
-            "dot_cutoff_1": 0.02,
-            "dot_cutoff_2": 0,
-            "dot_cutoff_3": 0,
-            "dot_scale_1": 1.6,
-            "dot_scale_2": 0,
-            "dot_scale_3": 0,
-            "method": "3D"
+            "filament_cut": 0.15,
+            "filament_scale": 1.0
         },
         "parent": 2
     },
-    "6": {
-        "annotation": "basic golgi - combine spot+thinned: 6",
+    "5": {
+        "annotation": "basic lyso - combine spot+filament: 5",
         "category": "core",
         "function": "logical_or",
         "parent": [
-            5,
+            3,
             4
         ]
     },
-    "7": {
-        "annotation": "basic mito - fill/filter: 7",
+    "6": {
+        "annotation": "basic lyso - fill/filter: 6",
         "category": "postprocessing",
         "function": "fill_and_filter_linear_size",
         "parameter_values": {
-            "hole_max": 0,
+            "hole_max": 40,
             "hole_min": 0,
-            "method": "3D",
-            "min_size": 3
+            "method": "slice_by_slice",
+            "min_size": 4
         },
-        "parent": 6
+        "parent": 5
     },
-    "8": {
-        "annotation": "label to uint16 for export 8",
-        "category": "postpostprocessing",
+    "7": {
+        "annotation": "label to uint16 for export 7",
+        "category": "postprocessing",
         "function": "label_uint16",
-        "parent": 7
+        "parent": 6
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.5.perox.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.5.perox.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9592500000000002%*

 * *Differences: {"'2'": "{'parameter_values': {replace: OrderedDict([('median_sz', 1), ('gauss_sig', 3.0)])}}",*

 * * "'3'": "{'function': 'spot_filter_3', 'parameter_values': {'dot_cut_1': 0.01, 'dot_cut_2': 0.1, "*

 * *        "'dot_cut_3': 0.1, delete: ['dot_cutoff_1', 'dot_cutoff_2', 'dot_cutoff_3', 'method']}}",*

 * * "'4'": "{'parameter_values': {'method': 'slice_by_slice'}}",*

 * * "'5'": "{'category': 'postprocessing'}"}*

```diff
@@ -9,46 +9,45 @@
         "parent": 0
     },
     "2": {
         "annotation": "basic perox segmentation: 2",
         "category": "preprocessing",
         "function": "scale_and_smooth",
         "parameter_values": {
-            "gauss_sigma": 1.34,
-            "median_size": 0
+            "gauss_sig": 3.0,
+            "median_sz": 1
         },
         "parent": 1
     },
     "3": {
         "annotation": "basic perox - spot filter (1 scale): 3",
         "category": "core",
-        "function": "dot_filter_3",
+        "function": "spot_filter_3",
         "parameter_values": {
-            "dot_cutoff_1": 0.06,
-            "dot_cutoff_2": 0,
-            "dot_cutoff_3": 0,
+            "dot_cut_1": 0.01,
+            "dot_cut_2": 0.1,
+            "dot_cut_3": 0.1,
             "dot_scale_1": 1.0,
             "dot_scale_2": 0,
-            "dot_scale_3": 0,
-            "method": "3D"
+            "dot_scale_3": 0
         },
         "parent": 2
     },
     "4": {
         "annotation": "basic perox - fill/filter: 4",
         "category": "postprocessing",
         "function": "fill_and_filter_linear_size",
         "parameter_values": {
             "hole_max": 0,
             "hole_min": 0,
-            "method": "3D",
+            "method": "slice_by_slice",
             "min_size": 2
         },
         "parent": 3
     },
     "5": {
         "annotation": "label to uint16 for export 5",
-        "category": "postpostprocessing",
+        "category": "postprocessing",
         "function": "label_uint16",
         "parent": 4
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.6.ER.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.4.golgi.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.716875%*

 * *Differences: {"'1'": "{'parameter_values': {'chan': 3}, 'annotation': 'basic golgi segmentation: 1'}",*

 * * "'2'": "{'parameter_values': {replace: OrderedDict([('median_sz', 4), ('gauss_sig', 1.4)])}, "*

 * *        "'annotation': 'basic golgi segmentation: 2'}",*

 * * "'3'": "{'parameter_values': {'th_method': 'triangle', 'th_adjust': 0.5, delete: "*

 * *        "['global_method', 'local_adjust']}, 'annotation': 'basic golgi - mo: 3'}",*

 * * "'4'": "{'function': 'topology_preserving_thinning', 'parameter_values': {replace: "*

 * *        "Ordered […]*

```diff
@@ -1,74 +1,83 @@
 {
     "1": {
-        "annotation": "basic ER segmentation: 1",
+        "annotation": "basic golgi segmentation: 1",
         "category": "extraction",
         "function": "select_channel_from_raw",
         "parameter_values": {
-            "chan": 5
+            "chan": 3
         },
         "parent": 0
     },
     "2": {
-        "annotation": "basic ER segmentation: 2",
+        "annotation": "basic golgi segmentation: 2",
         "category": "preprocessing",
         "function": "scale_and_smooth",
         "parameter_values": {
-            "gauss_sigma": 2.0,
-            "median_size": 3
+            "gauss_sig": 1.4,
+            "median_sz": 4
         },
         "parent": 1
     },
     "3": {
-        "annotation": "basic nuclei segmentation: 3",
+        "annotation": "basic golgi - mo: 3",
         "category": "core",
         "function": "masked_object_thresh",
         "parameter_values": {
             "cutoff_size": 1200,
-            "global_method": "triangle",
-            "local_adjust": 0.7
+            "th_adjust": 0.5,
+            "th_method": "triangle"
         },
         "parent": 2
     },
     "4": {
-        "annotation": "basic mito - filament filter: 4",
+        "annotation": "basic golgi - thinning filter: 4",
         "category": "core",
-        "function": "filament_filter_3",
+        "function": "topology_preserving_thinning",
         "parameter_values": {
-            "filament_cutoff_1": 0.005,
-            "filament_cutoff_2": 0.005,
-            "filament_cutoff_3": 0,
-            "filament_scale_1": 1.0,
-            "filament_scale_2": 2,
-            "filament_scale_3": 0,
-            "method": "3D"
+            "min_thickness": 1.6,
+            "thin": 1
         },
-        "parent": 2
+        "parent": 3
     },
     "5": {
-        "annotation": "basic mito - combine spot+filament: 5",
+        "annotation": "basic golgi - spot filter: 5",
+        "category": "core",
+        "function": "spot_filter_3",
+        "parameter_values": {
+            "dot_cut_1": 0.02,
+            "dot_cut_2": 0.1,
+            "dot_cut_3": 0.1,
+            "dot_scale_1": 1.6,
+            "dot_scale_2": 0,
+            "dot_scale_3": 0
+        },
+        "parent": 2
+    },
+    "6": {
+        "annotation": "basic golgi - combine spot+thinned: 6",
         "category": "core",
         "function": "logical_or",
         "parent": [
-            3,
+            5,
             4
         ]
     },
-    "6": {
-        "annotation": "basic ER - fill/filter: 6",
+    "7": {
+        "annotation": "basic mito - fill/filter: 7",
         "category": "postprocessing",
         "function": "fill_and_filter_linear_size",
         "parameter_values": {
-            "hole_max": 0,
+            "hole_max": 25,
             "hole_min": 0,
-            "method": "3D",
-            "min_size": 4
+            "method": "slice_by_slice",
+            "min_size": 11
         },
-        "parent": 5
-    },
-    "7": {
-        "annotation": "label to uint16 for export 7",
-        "category": "postpostprocessing",
-        "function": "label_bool_as_uint16",
         "parent": 6
+    },
+    "8": {
+        "annotation": "label to uint16 for export 8",
+        "category": "postprocessing",
+        "function": "label_uint16",
+        "parent": 7
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/conf_0.7.LD.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/conf_0.3.mito.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9100000000000001%*

 * *Differences: {"'1'": "{'parameter_values': {'chan': 2}, 'annotation': 'basic mito segmentation: 1'}",*

 * * "'2'": "{'parameter_values': {replace: OrderedDict([('median_sz', 3), ('gauss_sig', 2.6)])}, "*

 * *        "'annotation': 'basic mito segmentation: 2'}",*

 * * "'3'": "{'function': 'vesselness_slice_by_slice', 'parameter_values': {replace: "*

 * *        "OrderedDict([('sigma', 1.5), ('cutoff', 0.05)])}, 'annotation': 'basic mito - vesselness "*

 * *        "filter: 3'}",*

 * * "'4'": "{'parameter_values': {'hole_max': 25, 'min_size': 11}, 'a […]*

```diff
@@ -1,51 +1,49 @@
 {
     "1": {
-        "annotation": "basic LD segmentation: 1",
+        "annotation": "basic mito segmentation: 1",
         "category": "extraction",
         "function": "select_channel_from_raw",
         "parameter_values": {
-            "chan": 6
+            "chan": 2
         },
         "parent": 0
     },
     "2": {
-        "annotation": "basic LD segmentation: 2",
+        "annotation": "basic mito segmentation: 2",
         "category": "preprocessing",
         "function": "scale_and_smooth",
         "parameter_values": {
-            "gauss_sigma": 1.34,
-            "median_size": 2
+            "gauss_sig": 2.6,
+            "median_sz": 3
         },
         "parent": 1
     },
     "3": {
-        "annotation": "basic LD segmentation: 3",
+        "annotation": "basic mito - vesselness filter: 3",
         "category": "core",
-        "function": "apply_threshold",
+        "function": "vesselness_slice_by_slice",
         "parameter_values": {
-            "method": "otsu",
-            "thresh_factor": 0.8,
-            "thresh_max": 1.0,
-            "thresh_min": 0.05
+            "cutoff": 0.05,
+            "sigma": 1.5
         },
         "parent": 2
     },
     "4": {
-        "annotation": "basic LD segmentation: 4",
+        "annotation": "basic mito - fill/filter: 4",
         "category": "postprocessing",
         "function": "fill_and_filter_linear_size",
         "parameter_values": {
-            "hole_max": 2,
+            "hole_max": 25,
             "hole_min": 0,
             "method": "3D",
-            "min_size": 1
+            "min_size": 11
         },
         "parent": 3
     },
     "5": {
         "annotation": "label to uint16 for export 5",
-        "category": "postpostprocessing",
+        "category": "postprocessing",
         "function": "label_uint16",
         "parent": 4
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7630208333333334%*

 * *Differences: {"'10'": "{'function': 'hole_filling', 'parameter_values': {replace: OrderedDict([('hole_min', 0), "*

 * *         "('hole_max', 6.25), ('fill_2d', True)])}}",*

 * * "'11'": "OrderedDict([('category', 'postprocessing'), ('function', 'apply_mask'), ('parent', [10, "*

 * *         '4])])',*

 * * "'12'": "OrderedDict([('category', 'postprocessing'), ('function', 'size_filter_2D'), "*

 * *         "('parameter_values', OrderedDict([('min_size', 16)])), ('parent', 6)])",*

 * * "'5'": "{'parameter_values': {'chan': 6}}",*

 * * "'7'": "{'function': […]*

```diff
@@ -2,20 +2,38 @@
     "1": {
         "category": "extraction",
         "function": "fixed_get_optimal_Z_img",
         "parent": 0
     },
     "10": {
         "category": "postprocessing",
-        "function": "size_filter_2D",
+        "function": "hole_filling",
         "parameter_values": {
-            "min_size": 4
+            "fill_2d": true,
+            "hole_max": 6.25,
+            "hole_min": 0
         },
         "parent": 9
     },
+    "11": {
+        "category": "postprocessing",
+        "function": "apply_mask",
+        "parent": [
+            10,
+            4
+        ]
+    },
+    "12": {
+        "category": "postprocessing",
+        "function": "size_filter_2D",
+        "parameter_values": {
+            "min_size": 16
+        },
+        "parent": 6
+    },
     "2": {
         "category": "extraction",
         "function": "fixed_infer_cellmask_fromaggr",
         "parent": 1
     },
     "3": {
         "category": "extraction",
@@ -36,39 +54,44 @@
             3
         ]
     },
     "5": {
         "category": "extraction",
         "function": "select_channel_from_raw",
         "parameter_values": {
-            "chan": 5
+            "chan": 6
         },
         "parent": 1
     },
     "6": {
         "category": "preprocessing",
         "function": "min_max_intensity_normalization",
         "parent": 5
     },
     "7": {
         "category": "preprocessing",
-        "function": "edge_preserving_smoothing",
+        "function": "median_filter_slice_by_slice",
+        "parameter_values": {
+            "size": 4
+        },
         "parent": 6
     },
     "8": {
-        "category": "core",
-        "function": "filament_filter",
+        "category": "preprocessing",
+        "function": "image_smoothing_gaussian_slice_by_slice",
         "parameter_values": {
-            "filament_cut": 0.15,
-            "filament_scale": 1.0
+            "sigma": 1.34
         },
         "parent": 7
     },
     "9": {
-        "category": "postprocessing",
-        "function": "apply_mask",
-        "parent": [
-            8,
-            4
-        ]
+        "category": "core",
+        "function": "apply_threshold",
+        "parameter_values": {
+            "method": "otsu",
+            "thresh_factor": 0.99,
+            "thresh_max": 1.0,
+            "thresh_min": 0.5
+        },
+        "parent": 8
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7385416666666668%*

 * *Differences: {"'10'": "{'category': 'core', 'function': 'fixed_infer_LD', 'parent': [1, 4], delete: "*

 * *         "['parameter_values']}",*

 * * "'11'": "{'function': 'stack_organelle_objects', 'parent': {insert: [(0, 2), (1, 3), (3, 5), (4, "*

 * *         '6), (5, 7), (6, 8), (7, 9), (8, 10)], delete: [0]}}',*

 * * "'2'": "{'category': 'core'}",*

 * * "'3'": "{'category': 'core'}",*

 * * "'4'": "{'category': 'core'}",*

 * * "'5'": "{'category': 'core', 'function': 'fixed_infer_lyso', 'parent': [1, 4], delete: "*

 * *        "['parameter_values']}",*

 * * "'6'" […]*

```diff
@@ -1,97 +1,94 @@
 {
     "1": {
         "category": "extraction",
         "function": "fixed_get_optimal_Z_img",
         "parent": 0
     },
     "10": {
-        "category": "postprocessing",
-        "function": "hole_filling",
-        "parameter_values": {
-            "fill_2d": true,
-            "hole_max": 6.25,
-            "hole_min": 0
-        },
-        "parent": 9
-    },
-    "11": {
-        "category": "postprocessing",
-        "function": "apply_mask",
+        "category": "core",
+        "function": "fixed_infer_LD",
         "parent": [
-            10,
+            1,
             4
         ]
     },
-    "12": {
+    "11": {
         "category": "postprocessing",
-        "function": "size_filter_2D",
-        "parameter_values": {
-            "min_size": 16
-        },
-        "parent": 6
+        "function": "stack_organelle_objects",
+        "parent": [
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10
+        ]
     },
     "2": {
-        "category": "extraction",
+        "category": "core",
         "function": "fixed_infer_cellmask_fromaggr",
         "parent": 1
     },
     "3": {
-        "category": "extraction",
+        "category": "core",
         "function": "fixed_infer_nuclei",
         "parent": [
             1,
             2
         ]
     },
     "4": {
-        "category": "extraction",
+        "category": "core",
         "function": "infer_cytoplasm",
         "parameter_values": {
             "erode_nuclei": true
         },
         "parent": [
             2,
             3
         ]
     },
     "5": {
-        "category": "extraction",
-        "function": "select_channel_from_raw",
-        "parameter_values": {
-            "chan": 6
-        },
-        "parent": 1
+        "category": "core",
+        "function": "fixed_infer_lyso",
+        "parent": [
+            1,
+            4
+        ]
     },
     "6": {
-        "category": "preprocessing",
-        "function": "min_max_intensity_normalization",
-        "parent": 5
+        "category": "core",
+        "function": "fixed_infer_mito",
+        "parent": [
+            1,
+            4
+        ]
     },
     "7": {
-        "category": "preprocessing",
-        "function": "median_filter_slice_by_slice",
-        "parameter_values": {
-            "size": 4
-        },
-        "parent": 6
+        "category": "core",
+        "function": "fixed_infer_golgi",
+        "parent": [
+            1,
+            4
+        ]
     },
     "8": {
-        "category": "preprocessing",
-        "function": "image_smoothing_gaussian_slice_by_slice",
-        "parameter_values": {
-            "sigma": 1.34
-        },
-        "parent": 7
+        "category": "core",
+        "function": "fixed_infer_perox",
+        "parent": [
+            1,
+            4
+        ]
     },
     "9": {
         "category": "core",
-        "function": "apply_threshold",
-        "parameter_values": {
-            "method": "otsu",
-            "thresh_factor": 0.99,
-            "thresh_max": 1.0,
-            "thresh_min": 0.5
-        },
-        "parent": 8
+        "function": "fixed_infer_ER",
+        "parent": [
+            1,
+            4
+        ]
     }
 }
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/infer_nuclei.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/infer_nuclei.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/infer_soma.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/infer_soma.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/og_all_functions.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/og_all_functions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'spot_filter_3D'": "OrderedDict([('name', 'Spot Filter 3D'), ('python::module', "*

 * *                     "'aicssegmentation.core.seg_dot'), ('python::function', 'dot_3d'), "*

 * *                     "('parameters', OrderedDict([('log_sigma', OrderedDict([('widget_type', "*

 * *                     "'slider'), ('data_type', 'float'), ('min', 0), ('max', 10), ('increment', "*

 * *                     "0.05)])), ('cutoff', OrderedDict([('widget_type', 'slider'), ('data_type', "*

 * *                     "'float'), ('min', 0), (' […]*

```diff
@@ -55,35 +55,14 @@
                 ],
                 "widget_type": "drop-down"
             }
         },
         "python::function": "compute_3d_hessian_matrix",
         "python::module": "aicssegmentation.core.hessian"
     },
-    "dot_filter_3D": {
-        "name": "Spot Filter 3D",
-        "parameters": {
-            "cutoff": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "log_sigma": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            }
-        },
-        "python::function": "dot_3d",
-        "python::module": "aicssegmentation.core.seg_dot"
-    },
     "edge_preserving_smoothing": {
         "name": "Edge Preserving Smoothing",
         "parameters": null,
         "python::function": "edge_preserving_smoothing_3d",
         "python::module": "aicssegmentation.core.pre_processing_utils"
     },
     "erosion": {
@@ -504,14 +483,35 @@
                 "min": 0,
                 "widget_type": "slider"
             }
         },
         "python::function": "size_filter",
         "python::module": "aicssegmentation.core.utils"
     },
+    "spot_filter_3D": {
+        "name": "Spot Filter 3D",
+        "parameters": {
+            "cutoff": {
+                "data_type": "float",
+                "increment": 0.001,
+                "max": 0.5,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "log_sigma": {
+                "data_type": "float",
+                "increment": 0.05,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            }
+        },
+        "python::function": "dot_3d",
+        "python::module": "aicssegmentation.core.seg_dot"
+    },
     "spot_filter_slice_by_slice": {
         "name": "Spot Filter Slice by Slice",
         "parameters": {
             "cutoff": {
                 "data_type": "float",
                 "increment": 0.001,
                 "max": 1,
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/depricate/test_functions.json` & `infer-subc-0.0.post1/infer_subc/organelles_config/depricate/test_functions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'spot_filter_3D'": "OrderedDict([('name', 'Spot Filter 3D'), ('parameters', "*

 * *                     "OrderedDict([('cutoff', OrderedDict([('data_type', 'float'), ('increment', "*

 * *                     "0.001), ('max', 0.5), ('min', 0), ('widget_type', 'slider')])), "*

 * *                     "('log_sigma', OrderedDict([('data_type', 'float'), ('increment', 0.05), "*

 * *                     "('max', 10), ('min', 0), ('widget_type', 'slider')]))])), "*

 * *                     "('python::function', 'dot_3d'), ('python::mod […]*

```diff
@@ -61,35 +61,14 @@
                 ],
                 "widget_type": "drop-down"
             }
         },
         "python::function": "compute_3d_hessian_matrix",
         "python::module": "aicssegmentation.core.hessian"
     },
-    "dot_filter_3D": {
-        "name": "Spot Filter 3D",
-        "parameters": {
-            "cutoff": {
-                "data_type": "float",
-                "increment": 0.001,
-                "max": 0.5,
-                "min": 0,
-                "widget_type": "slider"
-            },
-            "log_sigma": {
-                "data_type": "float",
-                "increment": 0.05,
-                "max": 10,
-                "min": 0,
-                "widget_type": "slider"
-            }
-        },
-        "python::function": "dot_3d",
-        "python::module": "aicssegmentation.core.seg_dot"
-    },
     "edge_preserving_smoothing": {
         "name": "Edge Preserving Smoothing",
         "parameters": null,
         "python::function": "edge_preserving_smoothing_3d",
         "python::module": "aicssegmentation.core.pre_processing_utils"
     },
     "extract_boundary_of_objects": {
@@ -524,14 +503,35 @@
                 "min": 0,
                 "widget_type": "slider"
             }
         },
         "python::function": "size_filter_2D",
         "python::module": "infer_subc.core.img"
     },
+    "spot_filter_3D": {
+        "name": "Spot Filter 3D",
+        "parameters": {
+            "cutoff": {
+                "data_type": "float",
+                "increment": 0.001,
+                "max": 0.5,
+                "min": 0,
+                "widget_type": "slider"
+            },
+            "log_sigma": {
+                "data_type": "float",
+                "increment": 0.05,
+                "max": 10,
+                "min": 0,
+                "widget_type": "slider"
+            }
+        },
+        "python::function": "dot_3d",
+        "python::module": "aicssegmentation.core.seg_dot"
+    },
     "spot_filter_slice_by_slice": {
         "name": "Spot Filter Slice by Slice",
         "parameters": {
             "cutoff": {
                 "data_type": "float",
                 "increment": 0.001,
                 "max": 1,
```

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/function_guide.md` & `infer-subc-0.0.post1/infer_subc/organelles_config/function_guide.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/function_params.md` & `infer-subc-0.0.post1/infer_subc/organelles_config/function_params.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/organelles_config/helper.py` & `infer-subc-0.0.post1/infer_subc/organelles_config/helper.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/utils/_aicsimage_reader.py` & `infer-subc-0.0.post1/infer_subc/utils/_aicsimage_reader.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/utils/batch.py` & `infer-subc-0.0.post1/infer_subc/utils/batch.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/utils/directories.py` & `infer-subc-0.0.post1/infer_subc/utils/directories.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/utils/stats.py` & `infer-subc-0.0.post1/infer_subc/utils/stats.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/utils/stats_helpers.py` & `infer-subc-0.0.post1/infer_subc/utils/stats_helpers.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/batch_workflow.py` & `infer-subc-0.0.post1/infer_subc/workflow/batch_workflow.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/segmenter_function.py` & `infer-subc-0.0.post1/infer_subc/workflow/segmenter_function.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/workflow.py` & `infer-subc-0.0.post1/infer_subc/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/workflow_config.py` & `infer-subc-0.0.post1/infer_subc/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/workflow_definition.py` & `infer-subc-0.0.post1/infer_subc/workflow/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/workflow_engine.py` & `infer-subc-0.0.post1/infer_subc/workflow/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc/workflow/workflow_step.py` & `infer-subc-0.0.post1/infer_subc/workflow/workflow_step.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/infer_subc.egg-info/PKG-INFO` & `infer-subc-0.0.post1/infer_subc.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infer-subc
-Version: 0.0.6b0
+Version: 0.0.post1
 Summary: A plugin that enables organelle segmentation
 Home-page: https://github.com/ndcn/infer-subc
 Author: Andy Henrie
 Author-email: ergonyc@gmail.com
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/ndcn/infer-subc/issues
 Project-URL: Documentation, https://github.com/ndcn/infer-subc#README.md
@@ -69,68 +69,87 @@
 - [`napari`](https://napari.org/stable/) -- Used as the visualization framework, a fast, interactive, multi-domensional image viewer for Python.
 - [`scipy`](https://scipy.org/install/) -- Image analysis
 - [`scikit-image`](https://scikit-image.org/) -- Image analysis
 - [`itk`](https://itkpythonpackage.readthedocs.io/en/master/Quick_start_guide.html) -- Image analysis
 - [`numpy`](https://numpy.org/) -- Under the hood computation
 - [`Alzheimer's Disease AD Workbench`](https://www.alzheimersdata.org/ad-workbench) -- We initially wanted to use the ADDI's ADWB as a method of data sharing and to serve as a computational resource.
 
+## ADWB hints
+
+Given that the github repos are not yet whitelisted, the source directory needs to be zipped and uploaded in order to make an "editable" pip install.
+
+[uploading guide ](https://knowledgebase.aridhia.io/article/guidance-for-uploading-files/)
+[uploading files via the workspace article](https://knowledgebase.aridhia.io/article/uploading-files-via-the-workspace/).
+[Using BLOB storage](https://knowledgebase.aridhia.io/article/using-blob-storage/)
 
 ## Getting Started
 
 ### Prerequisites
 
+The following are prerequisites and should be installed prior to using the workflow.
 
+- `napari` 
+  ```
+  pip install "napari[all]"
+  ```
+
+- `scipy`
+  ```
+  python -m pip install scipy
+  ```
+
+- `scikit-image`
+  ```
+  pip install scikit-image
+  ```
+
+- `itk`
+  ```
+  pip install itk
+  ```
+- `numpy`
+  ```
+  pip install numpy
+  ```
 
 ### Installation
-`infer_subc` is  available on `PyPI` via: 
 
+`infer_subc` is not yet available on `PyPI` so must be  be `pip` ionstalled from source
 ```
-pip install infer_subc
+pip install git+https://github.com/ndcn/infer-subc.git
 ```
 
-If there are issues more details can be fouund in the [documentation](https://ndcn.github.io/infer-subc/config/)
-
+## Usage
 
-## Usage - quick start
-Its recommended that you use this repo along with the [`organelle-segmenter-plugin`](https://github.com/ndcn/organelle-segmenter-plugin) as in [Option A](#option-a-napari-organelle-segmenter-plugin) below.  Alternatively using the module functions directly as in [Option B](#option-b-python-script-or-notebook) would work just fine.
+```py
+from infer_subc.organelles import infer_lyso
+from infer_subc.core.file_io import read_czi_image
 
+img_data,meta_dict = read_czi_image("path/to/image.czi")
+lyso_obj =  infer_lyso(img_data) 
 
-### Option A: Napari `organelle-segmenter-plugin`
-
-1. Open a file in napari by dragging multi-channel .czi file onto napari which will import a multi-channel, multi-Z 'layer'. (Using the menu's defaults to `aicsIMAGEIO` reader which automatically splits mutliple channels into individual layers.  The plugin is able to support multi-dimensional data in .tiff, .tif. ome.tif, .ome.tiff, .czi)
-2. Start the plugin (open napari, go to "Plugins" --> "organelle-segmenter-plugin" --> "workflow editor")
-3. Select the image and channel to work on
-4. Select a workflow based on the example image and target segmentation based on user's data. Ideally, it is recommend to start with the example with very similar morphology as user's data.
-5. Click "Run All" to execute the whole workflow on the sample data.
-6. Adjust the parameters of steps, based on the intermediate results.  A complete list of all functions can be found [here](https://github.com/ndcn/infer-subc/blob/main/infer_subc/organelles_config/function_params.md)🚧 WIP 🚧
-7. Click "Run All" again after adjusting the parameters and repeat step 6 and 7 until the result is satisfactory.
-8. Save the workflow
-9. Close the plugin and open the **batch processing** part by (go to "Plugins" --> "organelle-segmenter-plugin" --> "batch processing")
-10. Load the customized workflow saved above 
-11. Load the folder with all the images to process
-12. Click "Run"
-13. Follow the [examples](https://github.com/ndcn/infer-subc/blob/main/notebooks/14_final_workflow.ipynb) in the `infer_subc` [repo](https://github.com/ndcn/infer-subc/) for postprocessing of the saved segmentations and generating the statistics.  
+```
 
-### Option B: python script or notebook 
+ 🚧 WIP 🚧 (🚨🚨🚨🚨 )
+> NOTE: command line capabilities not implimented
+```bash
+$ python -m infer_subc
+#or
+$ infer_subc
+```
 
-A variety of example [notebooks](https://github.com/ndcn/infer-subc/blob/main/notebooks/) demonstrating how to use the are available in the repo.  Additional information can be found at https://ndcn.github.io/infer-subc/nbs/overview/.  
+## Roadmap
 
+ - [ ] Create `PyPI` package
+ - [ ] Update installation instructions to reflect optimal use of `conda` environments
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## License
-Distributed under the terms of the [BSD-3] license,
-"organelle-segmenter-plugin" is free and open source software
+
+Distributed under the Unlicense license. See `LICENSE` for more information.  
 
 ## Issues
 
 If you encounter any problems, please file an issue with a detailed description.
-
-## ADWB hints
-
-Given that the github repos are not yet whitelisted, the source directory needs to be zipped and uploaded in order to make an "editable" pip install.
-
-[uploading guide ](https://knowledgebase.aridhia.io/article/guidance-for-uploading-files/)
-[uploading files via the workspace article](https://knowledgebase.aridhia.io/article/uploading-files-via-the-workspace/).
-[Using BLOB storage](https://knowledgebase.aridhia.io/article/using-blob-storage/)
```

### Comparing `infer-subc-0.0.6b0/infer_subc.egg-info/SOURCES.txt` & `infer-subc-0.0.post1/infer_subc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,24 +35,14 @@
 ./infer_subc/organelles/lipid.py
 ./infer_subc/organelles/lysosome.py
 ./infer_subc/organelles/mitochondria.py
 ./infer_subc/organelles/nuclei.py
 ./infer_subc/organelles/peroxisome.py
 ./infer_subc/organelles/qc.py
 ./infer_subc/organelles_config/__init__.py
-./infer_subc/organelles_config/all_functions.json
-./infer_subc/organelles_config/conf_0.1.masks.json
-./infer_subc/organelles_config/conf_0.2.lyso.json
-./infer_subc/organelles_config/conf_0.3.mito.json
-./infer_subc/organelles_config/conf_0.4.golgi.json
-./infer_subc/organelles_config/conf_0.5.perox.json
-./infer_subc/organelles_config/conf_0.6.ER.json
-./infer_subc/organelles_config/conf_0.7.LD.json
-./infer_subc/organelles_config/function_guide.md
-./infer_subc/organelles_config/function_params.md
 ./infer_subc/organelles_config/helper.py
 ./infer_subc/utils/__init__.py
 ./infer_subc/utils/_aicsimage_reader.py
 ./infer_subc/utils/batch.py
 ./infer_subc/utils/directories.py
 ./infer_subc/utils/filesystem.py
 ./infer_subc/utils/lazy.py
@@ -122,14 +112,15 @@
 infer_subc/organelles/mitochondria.py
 infer_subc/organelles/nuclei.py
 infer_subc/organelles/peroxisome.py
 infer_subc/organelles/qc.py
 infer_subc/organelles_config/__init__.py
 infer_subc/organelles_config/all_functions.json
 infer_subc/organelles_config/conf_0.1.masks.json
+infer_subc/organelles_config/conf_0.1.masks_MCZ.json
 infer_subc/organelles_config/conf_0.2.lyso.json
 infer_subc/organelles_config/conf_0.3.mito.json
 infer_subc/organelles_config/conf_0.4.golgi.json
 infer_subc/organelles_config/conf_0.5.perox.json
 infer_subc/organelles_config/conf_0.6.ER.json
 infer_subc/organelles_config/conf_0.7.LD.json
 infer_subc/organelles_config/function_guide.md
@@ -166,33 +157,31 @@
 infer_subc/workflow/workflow.py
 infer_subc/workflow/workflow_config.py
 infer_subc/workflow/workflow_definition.py
 infer_subc/workflow/workflow_engine.py
 infer_subc/workflow/workflow_step.py
 notebooks/00.0_framework_overview.ipynb
 notebooks/00.1_pipeline_setup.ipynb
-notebooks/01_infer_nuclei_from-label.ipynb
-notebooks/01a_infer_cytoplasm_from-composite.ipynb
-notebooks/02_infer_cellmask_from-composite_with-nuclei.ipynb
-notebooks/02a_infer_nuclei_from-composite.ipynb
-notebooks/02b_infer_cellmask_from-membrane.ipynb
+notebooks/01_infer_nuclei-from-ERsignal_3D.ipynb
+notebooks/01_infer_nuclei.ipynb
+notebooks/02_infer_cellmask.ipynb
+notebooks/02a_cell_membrane.ipynb
+notebooks/02b_infer_neurites_3D.ipynb
 notebooks/03_infer_cytoplasm.ipynb
-notebooks/03a_infer_cellmask_from-composite_no-nuclei.ipynb
-notebooks/04_infer_neurites_soma_from-cellmask.ipynb
-notebooks/05_infer_lysosome.ipynb
-notebooks/06_infer_mitochondria.ipynb
-notebooks/07_infer_golgi.ipynb
-notebooks/08_infer_peroxisome.ipynb
-notebooks/09_infer_ER.ipynb
-notebooks/10_infer_lipid_droplet.ipynb
-notebooks/11_regionprops.ipynb
-notebooks/12_batch_process.ipynb
-notebooks/13_fn_prototypes_json.ipynb
-notebooks/14_workflow_defs_json.ipynb
-notebooks/15_final_workflow.ipynb
+notebooks/04_infer_lysosome.ipynb
+notebooks/05_infer_mitochondria.ipynb
+notebooks/06_infer_golgi.ipynb
+notebooks/07_infer_peroxisome.ipynb
+notebooks/08_infer_ER.ipynb
+notebooks/09_infer_lipid_droplet.ipynb
+notebooks/10_regionprops.ipynb
+notebooks/11_batch_process.ipynb
+notebooks/12_fn_prototypes_json.ipynb
+notebooks/13_workflow_defs_json.ipynb
+notebooks/14_final_workflow.ipynb
 notebooks/todelete/00.1_pipeline_setup_3D.ipynb
 notebooks/todelete/00.2_extract_optimal_Z.ipynb
 notebooks/todelete/01_infer_nuclei_3D.ipynb
 notebooks/todelete/02_infer_soma_3D.ipynb
 notebooks/todelete/02a_infer_soma_3D.ipynb
 notebooks/todelete/02b_infer_neurites_3D.ipynb
 notebooks/todelete/02c_infer_wholecell_3D.ipynb
```

### Comparing `infer-subc-0.0.6b0/mkdocs.yml` & `infer-subc-0.0.post1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/00.1_pipeline_setup.ipynb` & `infer-subc-0.0.post1/notebooks/00.1_pipeline_setup.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9670025027056277%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, '\\n'), (2, 'SCohenLab 2D Image Processing notebook "*

 * *            "00\\n')], delete: [1]}}, 1: {'source': {insert: [(2, 'The first thing we need to be "*

 * *            "able to do is access the data files and interact wiht them.\\n'), (3, '\\n'), (4, "*

 * *            "'\\n')], delete: [2]}}, 2: {'source': {insert: [(0, '\\n'), (7, '### NOTES:\\n'), (8, "*

 * *            "'There are a few convences used here worth explanation.  Note the `imports.py` and "*

 * *            '`constan […]*

```diff
@@ -2,41 +2,44 @@
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Image Processing Pipeline Setup\n",
-                "--------------"
+                "\n",
+                "SCohenLab 2D Image Processing notebook 00\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## OVERVIEW\n",
                 "\n",
-                "The first thing we need to be able to do is access the data files and interact with them (e.g., read the metadata)."
+                "The first thing we need to be able to do is access the data files and interact wiht them.\n",
+                "\n",
+                "\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "\n",
                 "## IMPORTS\n",
                 "\n",
                 "The convention with notebooks (and python in general) is to import the nescessary packages as the first thing.\n",
                 "\n",
-                "\n",
                 "We are using `napari` for visualization, and `scipy` `ndimage` and `skimage` for analyzing the image files.  The underlying data format are `numpy` `ndarrays` and tools from  Allen Institute for Cell Science.\n",
                 "\n",
-                "> #### NOTES:\n",
-                "> There are a few convences used here worth explanation.  Note the `imports.py` and `constants.py` files in the base level of the `infer_subc` module.  These provide sortcuts for keeping track of imports and constants.   cf. the bottom of the imports below.  A second thing to note is the use of the \"magics\" ([[ link to magics info %%]]) `%load_ext autoreload` `%autoreload 2`, which tells the notebook to reload any changes made in the source code of the module on change; hence, avoid re-executing the imports.\n"
+                "### NOTES:\n",
+                "There are a few convences used here worth explanation.  Note the `imports.py` and `constants.py` files in the base level of the `infer_subc` module.  These provide sortcuts for keeping track of imports and constants.   cf. the bottom of the imports below.  A second thing to note is the use of the \"magics\" ([[ link to magics info %%]]) `%load_ext autoreload` `%autoreload 2`, which tells the notebook to reload any changes made in the source code of the module on change; hence, avoid re-executing the imports.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
@@ -84,44 +87,58 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Get and load Image for processing\n",
-                "Read the image and metadata into memory as an ndarray and dictionary from the `.czi` or '.tiff' files."
+                "\n",
+                "### Get and load Image for processing\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "\n",
+                "Read the data into memeory from the `.czi` files.  (Note: there is also the 2D slice .tif file read for later comparision).  WE will also collect metatdata.\n",
+                "\n",
+                "> the `data_path` variable should have the full path to the set of images wrapped in a `Path()`.   Below the path is built in 3 stages\n",
+                "> 1. my user directory \"~\" plus\n",
+                "> 2. general imaging data directory \"Projects/Imaging/data\" plus\n",
+                "> 3. \"raw\" where the linearly unmixed zstacks are\n",
+                "\n",
+                "The image \"type\" is also set by `im_type = \".czi\"`\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# We will use one file as a test file. Here we are using the TEST_IMG_N constant to determine which image in the list we will use. \n",
+                "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
-                "# Define the path to the directory that contains the input image folder.\n",
+                "# build the datapath\n",
+                "# all the imaging data goes here.\n",
                 "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
                 "\n",
-                "# Specify which subfolder that contains the input data and the input data file extension\n",
+                "# linearly unmixed \".czi\" files are here\n",
                 "in_data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
-                "# Create a list of the file paths for each image in the input folder. Select test image path.\n",
+                "# get the list of all files\n",
                 "img_file_list = list_image_files(in_data_path,im_type)\n",
-                "test_img_name = img_file_list[test_img_n]\n",
+                "# img_file_list2 = sorted(in_data_path.glob(f'*{im_type}'))\n",
                 "\n",
-                "# Create the output directory to save the segmentation outputs in.\n",
-                "out_data_path = data_root_path / \"out\"\n",
+                "test_img_name = img_file_list[test_img_n]\n",
                 "\n",
-                "if not Path.exists(out_data_path):\n",
-                "    Path.mkdir(out_data_path)\n",
-                "    print(f\"making {out_data_path}\")"
+                "# save output \".tiff\" files here\n",
+                "out_data_path = data_root_path / \"out\"\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
@@ -131,39 +148,43 @@
                     "text": [
                         "/opt/anaconda3/envs/napariNEW/lib/python3.9/site-packages/ome_types/_convenience.py:106: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
-                "# Read in the image and metadata as an ndarray and dictionary from the test image selected above. \n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
                 "\n",
-                "# Define some of the metadata features.\n",
+                "# get some top-level info about the RAW data\n",
                 "channel_names = meta_dict['name']\n",
                 "img = meta_dict['metadata']['aicsimage']\n",
                 "scale = meta_dict['scale']\n",
-                "channel_axis = meta_dict['channel_axis']"
+                "channel_axis = meta_dict['channel_axis']\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "--------------\n",
                 "\n",
                 "## SUMMARY\n",
                 "\n",
-                "The above shows the general procedure for importing the relavent modules, setting up the file I/O, and reading in the multi channel 3D flourescence image.\n",
+                "The above shows the general procedure importing the relavent modules, setting up the file I/O and finally reading in the `img_data` multi channel 3D flourescence image.\n",
                 "\n",
-                "### NEXT:  SEGMENT NUCLEI\n",
+                "### NEXT:  CHOOZE Z-SLICE\n",
                 "\n",
                 "proceed to [01_infer_nuclei.ipynb](./01_infer_nuclei.ipynb)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -174,15 +195,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "d6148ef1fb015fb20f0b6da2ea61c87c6b848bdf3dabb03087e5d5cd0c4607e9"
             }
         }
     },
```

### Comparing `infer-subc-0.0.6b0/notebooks/01a_infer_cytoplasm_from-composite.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/01_infer_nuclei_3D.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768889118240341%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Infer ***nuclei*** - 2️⃣ \\n'), (2, '> WARNING: (🚨🚨🚨🚨 "*

 * *            "Steps 2-9 depend on establishing a good solution here.)\\n'), (4, "*

 * *            "'--------------\\n'), (6, '## OBJECTIVE: \\n'), (7, '### ✅ Infer sub-cellular "*

 * *            "component #2: ***nuclei***  in order to understand interactome \\n'), (9, 'Infer a "*

 * *            'segmentation of the ***nuclei*** in order to measure its shape, position, size, and '*

 * *            "interaction with other orga […]*

```diff
@@ -1,307 +1,341 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Infer ***nuclei*** from a composite image - 2\ufe0f\u20e3 \n",
+                "# Infer ***nuclei*** - 2\ufe0f\u20e3 \n",
+                "\n",
+                "> WARNING: (\ud83d\udea8\ud83d\udea8\ud83d\udea8\ud83d\udea8 Steps 2-9 depend on establishing a good solution here.)\n",
                 "\n",
                 "--------------\n",
                 "\n",
-                "## OVERVIEW\n",
-                "We will start by segmenting the different cell regions - the nucleus, cell, and cytoplasm - since they will be necessary for determining which organelle are in which cell. This is integral to our single cell analysis approach.\n",
+                "## OBJECTIVE: \n",
+                "### \u2705 Infer sub-cellular component #2: ***nuclei***  in order to understand interactome \n",
                 "\n",
-                "This notebook goes through the workflow steps to segment the ***nucleus*** from a fluorescent nuclei marker.\n",
+                "Infer a segmentation of the ***nuclei*** in order to measure its shape, position, size, and interaction with other organelles/cellular components.  \n",
                 "\n",
+                "## OVERVIEW:\n",
                 "\n",
-                "## OBJECTIVE: \n",
-                "### \u2705 Infer sub-cellular component #1: ***nuclei***\n",
-                "Segment the ***nuclei*** from a composite image of multiple organelle markers combined. The ***cell*** and ***cytoplasm*** masks will also be derived from the same composite image. \n",
+                "We will infer the nuclei using the nuclei channel (e.g. 'ch = 0).\n",
                 "\n",
-                "> ***Biological relevance:***\n",
-                "> The combination of organelle markers used to create the composite image for the nucleus (and cell mask in [02_infer_cellmask_from-composite.ipynb](./02_infer_cellmask_from-composite.ipynb)) segmentation depends on the organelle labeles used and the cell type. In this example, the current selection includes the lysosomes, ER, and Golgi (e.g., Ch = 1, 3, 5) which have some intracellular background fluorescence - likely from off target marker localization. The lipid droplet channel (e.g., `ch = 6`) could also be included to produce a more unbiased selection of the entire cellmask as it binds to all cellular membranes to a small extent. However, the drawback of this is that it is present in every cell which makes downstream cell selection of a single cell more challenging. \n",
-                ">\n",
-                "> *It is important to consider specifics of your system as the cell type and labeling method may differ from the example above.*\n",
+                "Dependencies:\n",
+                "***Soma*** and ***cytoplasm*** inference rely on the ***nuclei*** inference.  Therefore all of the sub-cellular objects rely on the NU segmentation.\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## preamble\n",
                 "\n",
-                "> ***Convention:***  \"nuclei\" for the segmentation of ALL nuclei in the image.  \"nucleus\" for the ***single*** nucleus associated to the single cell being analyzed."
+                "1. imports\n",
+                "2. setup\n",
+                "3. infer-nuclei\n",
+                "    * input\n",
+                "    * pre-processing\n",
+                "    * core processing\n",
+                "    * post-processing\n",
+                "    * output"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "\n",
                 "### IMPORTS"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 3,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "The autoreload extension is already loaded. To reload it, use:\n",
+                        "  %reload_ext autoreload\n"
+                    ]
+                }
+            ],
             "source": [
                 "# top level imports\n",
                 "from pathlib import Path\n",
                 "import os, sys\n",
                 "from collections import defaultdict\n",
                 "from typing import Optional\n",
                 "\n",
                 "import numpy as np\n",
                 "\n",
                 "from aicssegmentation.core.pre_processing_utils import  image_smoothing_gaussian_slice_by_slice \n",
                 "from aicssegmentation.core.utils import hole_filling\n",
                 "from skimage.measure import label\n",
-                "import skimage\n",
-                "\n",
                 "\n",
                 "# # package for io \n",
                 "from aicsimageio import AICSImage\n",
                 "\n",
                 "import napari\n",
                 "\n",
                 "### import local python functions in ../infer_subc\n",
                 "sys.path.append(os.path.abspath((os.path.join(os.getcwd(), '..'))))\n",
                 "\n",
                 "\n",
-                "from infer_subc.utils.file_io import (read_czi_image,\n",
+                "from infer_subc.core.file_io import (read_czi_image,\n",
                 "                                                                    list_image_files)\n",
-                "from infer_subc.utils.img import *\n",
+                "from infer_subc.core.img import *\n",
                 "from infer_subc.organelles import fixed_get_optimal_Z_image, fixed_find_optimal_Z, find_optimal_Z\n",
                 "from infer_subc.constants import (TEST_IMG_N,\n",
                 "                                                                    NUC_CH ,\n",
                 "                                                                    LYSO_CH ,\n",
                 "                                                                    MITO_CH ,\n",
                 "                                                                    GOLGI_CH ,\n",
-                "                                                                    PEROXI_CH ,\n",
+                "                                                                    PEROX_CH ,\n",
                 "                                                                    ER_CH ,\n",
-                "                                                                    LIPID_CH ,\n",
+                "                                                                    LD_CH ,\n",
                 "                                                                    RESIDUAL_CH, \n",
                 "                                                                    ALL_CHANNELS )          \n",
                 "\n",
-                "from infer_subc.organelles import infer_soma, fixed_infer_soma\n",
+                "from infer_subc.organelles import infer_cellmask_fromaggr, fixed_infer_cellmask_fromaggr\n",
                 "\n",
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Get and load Image for processing"
+                "\n",
+                "## SETUP\n",
+                "CUSTOMIZE WITH: \n",
+                "1. updated path to data\n",
+                "2. updated folder name for \"raw\" data\n",
+                "\n",
+                "> NOTE: we are operating on a single \"test\" image in this notebook.  The batch-processing of all the images will be happen at the end of the notebook after we have developed/confirmed the setmentation procedures and parameter settings."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
-                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/Infer-subc-2D\"\n",
-                "\n",
-                "in_data_path = data_root_path / \"raw\"\n",
+                "# build the datapath\n",
+                "# all the imaging data goes here.\n",
+                "# CUSTOMIZE HERE --->\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
+                "\n",
+                "# linearly unmixed \".czi\" files are here\n",
+                "# CUSTOMIZE HERE --->\n",
+                "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
-                "img_file_list = list_image_files(in_data_path,im_type)\n",
-                "test_img_name = img_file_list[test_img_n]\n",
-                "\n",
-                "out_data_path = data_root_path / \"out\"\n",
-                "if not Path.exists(out_data_path):\n",
-                "    Path.mkdir(out_data_path)\n",
-                "    print(f\"making {out_data_path}\")"
+                "# get the list of all files in \"raw\"\n",
+                "img_file_list = list_image_files(data_path,im_type)\n",
+                "test_img_name = img_file_list[test_img_n]\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "c:\\Users\\Shannon\\anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:112: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "/opt/anaconda3/envs/napariNEW/lib/python3.9/site-packages/ome_types/_convenience.py:106: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
+                "# isolate image as an ndarray and metadata as a dictionary\n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
                 "\n",
+                "# get some top-level info about the RAW data\n",
                 "channel_names = meta_dict['name']\n",
                 "img = meta_dict['metadata']['aicsimage']\n",
                 "scale = meta_dict['scale']\n",
                 "channel_axis = meta_dict['channel_axis']"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "---------\n",
-                "## infer ***nuclei*** from composite image\n",
+                "## infer ***nuclei***\n",
                 "\n",
                 "### summary of steps\n",
                 "\n",
                 "\u27a1\ufe0f INPUT\n",
-                "- create composite image from multiple organelle channels\n",
+                "- channel 0\n",
                 "\n",
                 "PRE-PROCESSING\n",
                 "- scale to min 0, max 1.0\n",
-                "- ~~median Filter window 4~~\n",
-                "- ~~gaussian 1.34~~\n",
+                "- median Filter window 4\n",
+                "- gaussian 1.34\n",
                 "\n",
                 "CORE-PROCESSING\n",
-                "  - threshold method otsu  \n",
-                "    - threshold correction factor: 0.05\n",
-                "    - lower / upper bounds  (0, 1)\n",
-                "  - invert segmentation\n",
+                "  - threshold method minimum cross-entropy.  \n",
+                "    - objects 50-400 pixels, \n",
+                "    - threshold smoothing scale: 1.34 (later 1 pixel\n",
+                "    - threshold correction factor: 0.9 (later 1.2 )\n",
+                "    - lower / upper bounds  (.1, 1)\n",
+                "    - log transformed thresholding\n",
                 "\n",
                 "POST-PROCESSING\n",
                 "  - fill holes\n",
                 "  - remove small objects\n",
-                "  - label\n",
-                "  - remove objects touching image edges\n",
                 "\n",
                 "OUTPUT \u27a1\ufe0f \n",
-                "- mask of NUCLEI\n"
+                "- mask of NUCLEI\n",
+                "\n",
+                "\n",
+                "> #### Note:  in later steps we will isolate individual cells for analysis. Here, all nuclei are segmented and retained.\n",
+                "\n",
+                "\n",
+                "\n",
+                "#### NOTE:  using Allen Cell Segmenter  [Nucleophosmin](https://www.allencell.org/cell-observations/category/nucleophosmin) might be a good generic mechanism.  e.g.\n",
+                "-  [playground_npm1.ipynb](https://github.com/AllenInstitute/aics-segmentation/blob/master/lookup_table_demo/playground_npm1.ipynb) and [npm1.py](https://github.com/AllenInstitute/aics-segmentation/blob/master/aicssegmentation/structure_wrapper/seg_npm1.py) and [npm1_SR.py](https://github.com/AllenInstitute/aics-segmentation/blob/master/aicssegmentation/structure_wrapper/seg_npm1_SR.py)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## INPUT (prototype)\n",
                 "\n",
                 "Get the \"raw\" signals we need to analyze as well as any other dependencies in \"inferred\" objects.  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(49, 1688, 1688)\n"
+                        "(16, 768, 768)\n"
                     ]
                 }
             ],
             "source": [
-                "# ###################\n",
-                "# # INPUT\n",
-                "# ###################\n",
-                "# # raw_nuclei = img_data[NUC_CH].copy()\n",
-                "# raw_nuclei = select_channel_from_raw(img_data, NUC_CH)\n",
-                "\n",
-                "# print(raw_nuclei.shape)\n",
+                "###################\n",
+                "# INPUT\n",
+                "###################\n",
+                "# raw_nuclei = img_data[NUC_CH].copy()\n",
+                "raw_nuclei = select_channel_from_raw(img_data, NUC_CH)\n",
                 "\n",
-                "raw_nuclei = img_data[1]\n",
                 "print(raw_nuclei.shape)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## PRE-PROCESSING (prototype)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 8,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(16, 768, 768)\n",
+                        "(16, 768, 768)\n"
+                    ]
+                }
+            ],
             "source": [
                 "###################\n",
                 "# PRE_PROCESSING\n",
                 "###################           \n",
                 "nuclei_norm = min_max_intensity_normalization(raw_nuclei)\n",
                 "\n",
-                "#### smoothing is no longer necessary here - Huygens preprocessing took care of that already\n",
-                "\n",
-                "# med_filter_size = 4   \n",
-                "# nuclei_med = median_filter_slice_by_slice(nuclei_norm,\n",
-                "#                                       size=med_filter_size)\n",
-                "# print(nuclei_med.shape)\n",
-                "\n",
-                "# gaussian_smoothing_sigma = 1.34\n",
-                "# nuclei_gaus = image_smoothing_gaussian_slice_by_slice(nuclei_med,\n",
-                "#                                                       sigma=gaussian_smoothing_sigma)\n",
-                "# print(nuclei_gaus.shape)\n"
+                "med_filter_size = 4   \n",
+                "nuclei_med = median_filter_slice_by_slice(nuclei_norm,\n",
+                "                                      size=med_filter_size)\n",
+                "print(nuclei_med.shape)\n",
+                "\n",
+                "gaussian_smoothing_sigma = 1.34\n",
+                "nuclei_gaus = image_smoothing_gaussian_slice_by_slice(nuclei_med,\n",
+                "                                                      sigma=gaussian_smoothing_sigma)\n",
+                "print(nuclei_gaus.shape)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### VISUALIZE: the nuclei image after pre-processing\n",
                 "Use this to adjust median filter size and gaussian sigma above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 91,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "WARNING: QWindowsWindow::setGeometry: Unable to set geometry 1090x686+1+15 (frame: 1108x733-8-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+2+22 (frame: 1383x906-7-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n",
-                        "15-Mar-23 16:01:10 - vispy    - WARNING  - QWindowsWindow::setGeometry: Unable to set geometry 1090x686+1+15 (frame: 1108x733-8-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+2+22 (frame: 1383x906-7-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "viewer = napari.Viewer()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 92,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'nuclei_norm' at 0x22fcfeab640>"
+                            "<Image layer 'nuclei_gaus' at 0x1cf5b5642b0>"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 92,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    raw_nuclei,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    nuclei_norm,\n",
+                "    nuclei_med,\n",
                 "    scale=scale\n",
                 ")\n",
-                "# viewer.add_image(\n",
-                "#     nuclei_gaus,\n",
-                "#     scale=scale\n",
-                "# )"
+                "viewer.add_image(\n",
+                "    nuclei_gaus,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -318,68 +352,70 @@
                 "> [Thresholding](https://en.wikipedia.org/wiki/Thresholding_%28image_processing%29) is used to create binary images. A threshold value determines the intensity value separating foreground pixels from background pixels. Foregound pixels are pixels brighter than the threshold value, background pixels are darker. In many cases, images can be adequately segmented by thresholding followed by labelling of *connected components*, which is a fancy way of saying \"groups of pixels that touch each other\".\n",
                 "> \n",
                 "> Different thresholding algorithms produce different results. [Otsu's method](https://en.wikipedia.org/wiki/Otsu%27s_method) and [Li's minimum cross entropy threshold](https://scikit-image.org/docs/dev/auto_examples/developers/plot_threshold_li.html) are two common algorithms. Below, we use Li. You can use `skimage.filters.threshold_<TAB>` to find different thresholding methods.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 87,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(17, 704, 704)\n"
+                    ]
+                }
+            ],
             "source": [
                 "\n",
                 "###################\n",
                 "# CORE_PROCESSING\n",
                 "###################\n",
-                "threshold_factor = 0.05 #from cellProfiler\n",
-                "thresh_min = 0\n",
-                "thresh_max = 1\n",
-                "threshold = apply_threshold(nuclei_norm, thresh_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "bw = nuclei_norm < threshold\n",
-                "bw_invert = 1 - bw\n",
                 "\n",
-                "bw_labeled = label(bw_invert, connectivity=1)\n"
+                "threshold_factor = 0.9 #from cellProfiler\n",
+                "thresh_min = .1\n",
+                "thresh_max = 1.\n",
+                "li_thresholded = apply_log_li_threshold(nuclei_gaus, thresh_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
+                "\n",
+                "print(li_thresholded.shape)\n",
+                "\n",
+                "\n",
+                "## **************NEED TO ADJUST THESE SETTINGS TO ISOLATE MORE OF THE TOP AND BOTTOM OF THE NUCLEI***************"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### VISUALIZE: the nuclei image after core processing\n",
                 "Use this to adjust threshold parameters above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 88,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'bw_labeled' at 0x22f80708a30>"
+                            "<Image layer 'li_thresholded' at 0x1cf8f31fe80>"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 88,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    bw,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    bw_invert,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_labels(\n",
-                "    bw_labeled,\n",
+                "    li_thresholded,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -388,103 +424,108 @@
                 "## POST PROCESSING prototype\n",
                 "\n",
                 "> NOTE: the size parameters are by convention defined as one dimensional \"width\", so the inputs to the functions need to be _squared_ i.e. raised to the power of 2: `** 2`.   For volumetric (3D) analysis this would be _cubed_:`**3`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 89,
             "metadata": {},
             "outputs": [],
             "source": [
                 "###################\n",
                 "# POST_PROCESSING\n",
                 "###################\n",
                 "\n",
-                "hole_width = 30 \n",
-                "removed_holes = hole_filling(bw_invert,\n",
+                "hole_width = 5  \n",
+                "removed_holes = hole_filling(li_thresholded,\n",
                 "                             hole_min=0, \n",
-                "                             hole_max=hole_width**3, \n",
-                "                             fill_2d=False)\n",
+                "                             hole_max=hole_width**2, \n",
+                "                             fill_2d=True)\n",
+                "# there does not seem to be any observable differences between the slice-by-slice and 3D methods here for hole filling\n",
                 "\n",
-                "small_object_width = 20\n",
+                "small_object_width = 15\n",
                 "cleaned_img = size_filter(removed_holes, \n",
                 "                          min_size= small_object_width**3, #changed this to 3 to adjust for the 3D voxel, instead of a 2D pixel \n",
                 "                          method=\"3D\",\n",
                 "                          connectivity=1)\n",
                 "\n",
-                "all_labels = label(cleaned_img, connectivity=1)\n",
-                "\n",
-                "nuclei_label = skimage.segmentation.clear_border(all_labels)\n"
+                "## ************NEED TO ADJUST THESE SETTINGS TO GET RID OF SMALL BITS*****************\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### VISUALIZE: the nuclei image after post-processing\n",
                 "Use this to adjust the size parameters above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 90,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'nuclei_label' at 0x22f80a79eb0>"
+                            "<Image layer 'cleaned_img' at 0x1cf8f2081c0>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 90,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    removed_holes,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
                 "    cleaned_img,\n",
                 "    scale=scale\n",
-                ")\n",
-                "viewer.add_labels(\n",
-                "    all_labels,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_labels(\n",
-                "    nuclei_label,\n",
-                "    scale=scale\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 45,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "ename": "RuntimeError",
+                    "evalue": "wrapped C/C++ object of type QtViewer has been deleted",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[1;31mRuntimeError\u001b[0m                              Traceback (most recent call last)",
+                        "Cell \u001b[1;32mIn[45], line 1\u001b[0m\n\u001b[1;32m----> 1\u001b[0m viewer\u001b[39m.\u001b[39;49mclose()\n",
+                        "File \u001b[1;32mc:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\napari\\viewer.py:118\u001b[0m, in \u001b[0;36mViewer.close\u001b[1;34m(self)\u001b[0m\n\u001b[0;32m    116\u001b[0m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39mlayers\u001b[39m.\u001b[39mclear()\n\u001b[0;32m    117\u001b[0m \u001b[39m# Close the main window\u001b[39;00m\n\u001b[1;32m--> 118\u001b[0m \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49mwindow\u001b[39m.\u001b[39;49mclose()\n\u001b[0;32m    120\u001b[0m \u001b[39mif\u001b[39;00m config\u001b[39m.\u001b[39masync_loading:\n\u001b[0;32m    121\u001b[0m     \u001b[39mfrom\u001b[39;00m \u001b[39m.\u001b[39;00m\u001b[39mcomponents\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mexperimental\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mchunk\u001b[39;00m \u001b[39mimport\u001b[39;00m chunk_loader\n",
+                        "File \u001b[1;32mc:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\napari\\_qt\\qt_main_window.py:1222\u001b[0m, in \u001b[0;36mWindow.close\u001b[1;34m(self)\u001b[0m\n\u001b[0;32m   1220\u001b[0m \u001b[39mif\u001b[39;00m \u001b[39mhasattr\u001b[39m(\u001b[39mself\u001b[39m, \u001b[39m'\u001b[39m\u001b[39m_qt_window\u001b[39m\u001b[39m'\u001b[39m):\n\u001b[0;32m   1221\u001b[0m     \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_teardown()\n\u001b[1;32m-> 1222\u001b[0m     \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49m_qt_viewer\u001b[39m.\u001b[39;49mclose()\n\u001b[0;32m   1223\u001b[0m     \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_qt_window\u001b[39m.\u001b[39mclose()\n\u001b[0;32m   1224\u001b[0m     \u001b[39mdel\u001b[39;00m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_qt_window\n",
+                        "\u001b[1;31mRuntimeError\u001b[0m: wrapped C/C++ object of type QtViewer has been deleted"
+                    ]
+                }
+            ],
             "source": [
                 "viewer.close()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Adjust naming and type for labels"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 46,
             "metadata": {},
             "outputs": [],
             "source": [
                 "NU_signal = raw_nuclei\n",
                 "\n",
                 "# renaming semantic segmentation of nuclei\n",
                 "nuclei_object = cleaned_img\n",
@@ -499,26 +540,37 @@
             "metadata": {},
             "source": [
                 "### VISUALIZE final segmentations"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 51,
             "metadata": {},
             "outputs": [],
             "source": [
                 "viewer = napari.Viewer()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 52,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Labels layer 'NU_labels' at 0x1cf5b1d7cd0>"
+                        ]
+                    },
+                    "execution_count": 52,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "viewer.add_image(\n",
                 "    NU_signal,\n",
                 "    scale=scale,\n",
                 ")\n",
                 "viewer.add_image(\n",
                 "    nuclei_object,\n",
@@ -530,15 +582,15 @@
                 "    scale=scale,\n",
                 "    opacity=0.3,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 53,
             "metadata": {},
             "outputs": [],
             "source": [
                 "viewer.close()"
             ]
         },
         {
@@ -549,38 +601,44 @@
                 "## DEFINE `_infer_nuclei` function\n",
                 "\n",
                 "Based on the _prototyping_ above define the function to infer nuclei.  \n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 58,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
                 "#  _infer_nuclei\n",
                 "##########################\n",
-                "def _infer_nucleifromER_3D( in_img: np.ndarray,\n",
+                "def _infer_nuclei_3D( in_img: np.ndarray,\n",
+                "                       median_sz: int, \n",
+                "                       gauss_sig: float,\n",
                 "                       thresh_factor: float,\n",
                 "                       thresh_min: float,\n",
                 "                       thresh_max: float,\n",
                 "                       max_hole_w: int,\n",
                 "                       small_obj_w: int,\n",
                 "                       sz_filter_method: str\n",
                 "                     ) -> np.ndarray:\n",
                 "    \"\"\"\n",
                 "    Procedure to infer 3D nuclei segmentation from multichannel z-stack input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
-                "    cellmask: Optional[np.ndarray] = None\n",
+                "    soma_mask: Optional[np.ndarray] = None\n",
                 "        mask\n",
+                "    median_sz: int\n",
+                "        width of median filter for signal\n",
+                "    gauss_sig: float\n",
+                "        sigma for gaussian smoothing of  signal\n",
                 "    thresh_factor: float\n",
                 "        adjustment factor for log Li threholding\n",
                 "    thresh_min: float\n",
                 "        abs min threhold for log Li threholding\n",
                 "    thresh_max: float\n",
                 "        abs max threhold for log Li threholding\n",
                 "    max_hole_w: int\n",
@@ -593,100 +651,102 @@
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "    \n",
                 "    \"\"\"\n",
                 "\n",
-                "    # nuc_ch_from_ER = ER_CH\n",
-                "    # nuclei = select_channel_from_raw(in_img, nuc_ch_from_ER)\n",
-                "    nuclei = in_img[1]\n",
+                "    nuc_ch = NUC_CH\n",
+                "    nuclei = select_channel_from_raw(in_img, nuc_ch)\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
                 "    ###################                \n",
                 "    nuclei = min_max_intensity_normalization(nuclei)\n",
+                "    nuclei = median_filter_slice_by_slice(nuclei,\n",
+                "                                          size=median_sz)\n",
+                "    nuclei = image_smoothing_gaussian_slice_by_slice(nuclei,\n",
+                "                                                     sigma=gauss_sig )\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    thresh_value = apply_threshold(nuclei, \n",
-                "                                   thresh_factor=thresh_factor, \n",
-                "                                   thresh_min=thresh_min, \n",
-                "                                   thresh_max=thresh_max)\n",
-                "    nuclei_object = nuclei < thresh_value\n",
-                "    nuclei_object = 1 - nuclei_object\n",
+                "    nuclei_object = apply_log_li_threshold(nuclei, \n",
+                "                                           thresh_factor=thresh_factor, \n",
+                "                                           thresh_min=thresh_min, \n",
+                "                                           thresh_max=thresh_max)\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
                 "    nuclei_object = hole_filling(nuclei_object, \n",
                 "                                 hole_min=0, \n",
-                "                                 hole_max=max_hole_w**3, \n",
-                "                                 fill_2d=False)\n",
+                "                                 hole_max=max_hole_w**2, \n",
+                "                                 fill_2d=True)\n",
                 "\n",
                 "    nuclei_object = size_filter(nuclei_object, \n",
                 "                                min_size = small_obj_w**3, \n",
                 "                                method = sz_filter_method,\n",
                 "                                connectivity=1)\n",
-                "    \n",
-                "    nuclei_object = label(nuclei_object, connectivity=1)\n",
-                "    \n",
-                "    nuclei_object = skimage.segmentation.clear_border(nuclei_object)\n",
+                "\n",
                 "\n",
                 "    return nuclei_object\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## DEFINE `_fixed_infer_nuclei` function\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 63,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
                 "#  fixed_infer_nuclei\n",
                 "##########################\n",
                 "def _fixed_infer_nuclei_3D(in_img: np.ndarray) -> np.ndarray:\n",
                 "    \"\"\"\n",
-                "    Procedure to infer soma from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
-                "    cellmask: np.ndarray\n",
+                "    soma_mask: np.ndarray\n",
                 "        mask\n",
                 " \n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "    \n",
                 "    \"\"\"\n",
                 "\n",
                 "    nuc_ch = NUC_CH\n",
-                "    threshold_factor = 0.05\n",
-                "    thresh_min = 0\n",
+                "    median_sz = 4   \n",
+                "    gauss_sig = 1.34\n",
+                "    threshold_factor = 0.9\n",
+                "    thresh_min = 0.1\n",
                 "    thresh_max = 1.0\n",
-                "    max_hole_w = 30\n",
-                "    small_obj_w = 20\n",
+                "    max_hole_w = 5\n",
+                "    small_obj_w = 15\n",
                 "    sz_filter_method = \"3D\"\n",
                 "\n",
-                "    return _infer_nucleifromER_3D( in_img,\n",
+                "    return _infer_nuclei_3D( in_img,\n",
+                "                             median_sz,\n",
+                "                             gauss_sig,\n",
                 "                             threshold_factor,\n",
                 "                             thresh_min,\n",
                 "                             thresh_max,\n",
                 "                             max_hole_w,\n",
                 "                             small_obj_w,\n",
                 "                             sz_filter_method )\n"
             ]
@@ -698,51 +758,42 @@
             "source": [
                 "---------------------\n",
                 "## TEST `_infer_nuclei`  function defined above\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 64,
             "metadata": {},
             "outputs": [],
             "source": [
                 "_NU_object =  _fixed_infer_nuclei_3D(img_data) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 68,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "WARNING: QWindowsWindow::setGeometry: Unable to set geometry 1090x686+2+15 (frame: 1108x733-7-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+3+22 (frame: 1383x906-6-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n",
-                        "15-Mar-23 16:08:23 - vispy    - WARNING  - QWindowsWindow::setGeometry: Unable to set geometry 1090x686+2+15 (frame: 1108x733-7-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+3+22 (frame: 1383x906-6-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "viewer = napari.Viewer()"
+                "viewer = napari.Viewer()\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 69,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_NU_object' at 0x22fac2096a0>"
+                            "<Image layer '_NU_object' at 0x1cf9214fa60>"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 69,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    NU_signal,\n",
@@ -762,47 +813,47 @@
                 "    _NU_object,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 70,
             "metadata": {},
             "outputs": [],
             "source": [
                 "viewer.close()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\"> ***SR edits stops here***</code>\n",
+                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>\n",
                 "\n",
                 "---------------------\n",
-                "# TEST `infer_nuclei` exported functions\n",
+                "# TEST `infer_nuclei_fromlabel` exported functions\n",
                 "\n",
                 "> the prototype `_infer_nuclei` was copied to the [`.organelles.nuclei`](../infer_subc/organelles/nuclei.py) sub-module \n",
                 "##\n",
-                "`infer_nuclei` procedure\n",
+                "`infer_nuclei_fromlabel` procedure\n",
                 "\n",
-                "Use the `infer_nuclei` function to infer the Nucleus and export it as an _ome.tif_ for easy reference."
+                "Use the `infer_nuclei_fromlabel` function to infer the Nucleus and export it as an _ome.tif_ for easy reference."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.organelles.nuclei import infer_nuclei, fixed_infer_nuclei\n",
+                "from infer_subc.organelles.nuclei import infer_nuclei_fromlabel, fixed_infer_nuclei\n",
                 "\n",
-                "nuclei_object =  fixed_infer_nuclei(img_2D, cellmask) \n"
+                "nuclei_object =  fixed_infer_nuclei(img_2D, soma_mask) \n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -866,46 +917,70 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-----------------\n",
-                "Write the `infer_nuclei` spec to the widget json "
+                "Write the `infer_nuclei_fromlabel` spec to the widget json "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'name': 'infer nuclei  (fixed parameters)',\n",
+                            " 'python::module': 'infer_subc.organelles',\n",
+                            " 'python::function': 'fixed_infer_nuclei',\n",
+                            " 'parameters': None}"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
                 "_fixed_infer_nuclei =  {\n",
                 "        \"name\": \"infer nuclei  (fixed parameters)\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
                 "        \"python::function\": \"fixed_infer_nuclei\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
+                "_fixed_infer_nuclei"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "\n",
                 "add_function_spec_to_widget_json(\"fixed_infer_nuclei\",_fixed_infer_nuclei)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "_infer_nuclei =  {\n",
                 "        \"name\": \"infer nuclei\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_nuclei\",\n",
+                "        \"python::function\": \"infer_nuclei_fromlabel\",\n",
                 "        \"parameters\": {\n",
                 "                \"median_sz\": {\n",
                 "                        \"widget_type\": \"slider\",\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"min\": 3,\n",
                 "                        \"max\": 15,\n",
                 "                        \"increment\": 1\n",
@@ -951,27 +1026,27 @@
                 "                        \"max\": 50,\n",
                 "                        \"min\": 1,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                }\n",
                 "        }\n",
                 "}\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"infer_nuclei\", _infer_nuclei, overwrite=True )\n",
+                "add_function_spec_to_widget_json(\"infer_nuclei_fromlabel\", _infer_nuclei, overwrite=True )\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "_median_filter_slice_by_slice =  {\n",
                 "                \"name\": \"Median Smoothing Slice by Slice\",\n",
-                "                \"python::module\": \"infer_subc.utils.img\",\n",
+                "                \"python::module\": \"infer_subc.core.img\",\n",
                 "                \"python::function\": \"median_filter_slice_by_slice\",\n",
                 "                \"parameters\": {\n",
                 "                    \"size\": {\n",
                 "                        \"widget_type\": \"slider\",\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"min\": 1,\n",
                 "                        \"max\": 20,\n",
@@ -1015,15 +1090,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "# WARNING: not a good way to set to None\n",
                 "_apply_log_li_threshold = {\n",
                 "        \"name\": \"threshold log Li\",\n",
-                "        \"python::module\": \"infer_subc.utils.img\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
                 "        \"python::function\": \"apply_log_li_threshold\",\n",
                 "        \"parameters\": {\n",
                 "            \"thresh_factor\": {\n",
                 "                \"widget_type\": \"slider\",\n",
                 "                \"data_type\": \"float\",\n",
                 "                \"min\": 0.3,\n",
                 "                \"max\": 1.1,\n",
@@ -1073,19 +1148,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "#  nulei_object = apply_mask(nuclei_object, cellmask)\n",
+                "#  nulei_object = apply_mask(nuclei_object, soma_mask)\n",
                 "\n",
                 "_apply_mask=  {\n",
                 "        \"name\": \"apply mask\",\n",
-                "        \"python::module\": \"infer_subc.utils.img\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
                 "        \"python::function\": \"apply_mask\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "# json.dumps({\"apply_mask\":_apply_mask})\n",
                 "add_function_spec_to_widget_json(\"apply_mask\",_apply_mask)        \n"
             ]
         },
@@ -1093,36 +1168,36 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "    # small_object_width = 45\n",
-                "    # nuclei_object = size_filter_2D(nuclei_object, \n",
+                "    # nuclei_object = size_filter_linear_size(nuclei_object, \n",
                 "    #                                                             min_size= small_object_width**2, \n",
                 "    #                                                             connectivity=1)\n",
                 "\n",
                 "\n",
-                "_size_filter_2D = {\n",
+                "_size_filter_linear_size = {\n",
                 "        \"name\": \"Size Filter 2D\",\n",
-                "        \"python::module\": \"infer_subc.utils.img\",\n",
-                "        \"python::function\": \"size_filter_2D\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
+                "        \"python::function\": \"size_filter_linear_size\",\n",
                 "        \"parameters\": {\n",
                 "            \"min_size\": {\n",
                 "                \"widget_type\": \"slider\",\n",
                 "                \"data_type\": \"int\",\n",
                 "                \"min\": 0,\n",
                 "                \"max\": 500,\n",
                 "                \"increment\": 1\n",
                 "            }\n",
                 "        }\n",
                 "    }\n",
-                "# json.dumps({  \"size_filter_2D\":  _size_filter_2D   })\n",
+                "# json.dumps({  \"size_filter_linear_size\":  _size_filter_linear_size   })\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"size_filter_2D\",_size_filter_2D)        \n"
+                "add_function_spec_to_widget_json(\"size_filter_linear_size\",_size_filter_linear_size)        \n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1145,15 +1220,15 @@
                 "    Procedure to infer nuclei from linearly unmixed input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
                 "\n",
-                "    cellmask: np.ndarray\n",
+                "    soma_mask: np.ndarray\n",
                 "        mask\n",
                 "\n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "\n",
@@ -1237,22 +1312,22 @@
                 "    step_name.append(\"6\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
                 "    parent.append(5)\n",
                 "\n",
                 "    # # EEEEEK I don't know how to compose where the mask comes from... \n",
-                "    # nuclei_object = apply_mask(nuclei_object, cellmask)\n",
+                "    # nuclei_object = apply_mask(nuclei_object, soma_mask)\n",
                 "\n",
                 "    # small_object_width = 15\n",
-                "    # nuclei_object = size_filter_2D(nuclei_object, \n",
+                "    # nuclei_object = size_filter_linear_size(nuclei_object, \n",
                 "    #                                                             min_size= small_object_width**2, \n",
                 "    #                                                             connectivity=1)\n",
                 "    step_name.append(\"7\")\n",
-                "    function_name.append(\"size_filter_2D\")\n",
+                "    function_name.append(\"size_filter_linear_size\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(6)\n",
                 "\n",
                 "    out_dict = dict()\n",
                 "    for i,stepn in enumerate(step_name):\n",
                 "        entry = dict(category=category[i],\n",
@@ -1319,15 +1394,15 @@
                 "    Procedure to infer nuclei from linearly unmixed input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
                 "\n",
-                "    cellmask: np.ndarray\n",
+                "    soma_mask: np.ndarray\n",
                 "        mask\n",
                 "\n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "\n",
@@ -1346,15 +1421,15 @@
                 "    function_name.append(\"fixed_get_optimal_Z_img\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(0)\n",
                 "\n",
                 "\n",
                 "    step_name.append(\"2\")\n",
-                "    function_name.append(\"fixed_infer_soma\")\n",
+                "    function_name.append(\"fixed_infer_cellmask_fromaggr\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( None )\n",
                 "    parent.append(1)\n",
                 "\n",
                 "    step_name.append(\"3\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
@@ -1432,19 +1507,19 @@
                 "    function_name.append(\"apply_mask\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append([9,2])\n",
                 "\n",
                 "\n",
                 "    # small_object_width = 15\n",
-                "    # nuclei_object = size_filter_2D(nuclei_object, \n",
+                "    # nuclei_object = size_filter_linear_size(nuclei_object, \n",
                 "    #                                                             min_size= small_object_width**2, \n",
                 "    #                                                             connectivity=1)\n",
                 "    step_name.append(\"11\")\n",
-                "    function_name.append(\"size_filter_2D\")\n",
+                "    function_name.append(\"size_filter_linear_size\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(10)\n",
                 "\n",
                 "    out_dict = dict()\n",
                 "    for i,stepn in enumerate(step_name):\n",
                 "        entry = dict(category=category[i],\n",
@@ -1477,65 +1552,64 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
                 "_infer_nuclei =  {\n",
-                "        \"name\": \"infer infer_nuclei\",\n",
+                "        \"name\": \"infer infer_nuclei_fromlabel\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_nuclei\",\n",
+                "        \"python::function\": \"infer_nuclei_fromlabel\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"infer_nuclei\",_infer_nuclei)"
+                "add_function_spec_to_widget_json(\"infer_nuclei_fromlabel\",_infer_nuclei)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-------------\n",
                 "## SUMMARY\n",
                 "\n",
                 "The above details how the nuclei object is inferred.  \n",
                 "\n",
                 "### NEXT: INFER CYTOSOL\n",
                 "\n",
-                "proceed to [03_infer_cytosol.ipynb](./03_infer_cytosol.ipynb)\n"
+                "proceed to [03_infer_cytoplasm.ipynb](./03_infer_cytoplasm.ipynb)\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "infer-subc",
+            "display_name": "napariNEW",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
-                "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
+                "hash": "d6148ef1fb015fb20f0b6da2ea61c87c6b848bdf3dabb03087e5d5cd0c4607e9"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `infer-subc-0.0.6b0/notebooks/02a_infer_nuclei_from-composite.ipynb` & `infer-subc-0.0.post1/notebooks/01_infer_nuclei-from-ERsignal_3D.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896877082292187%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Infer ***nuclei*** - 2️⃣ \\n'), (2, '> WARNING: (🚨🚨🚨🚨 "*

 * *            "Steps 2-9 depend on establishing a good solution here.)\\n'), (4, "*

 * *            "'--------------\\n'), (6, '## OBJECTIVE: \\n'), (7, '### ✅ Infer sub-cellular "*

 * *            "component #2: ***nuclei***  in order to understand interactome \\n'), (9, 'Infer a "*

 * *            'segmentation of the ***nuclei*** in order to measure its shape, position, size, and '*

 * *            "interaction with other orga […]*

```diff
@@ -1,34 +1,48 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Infer ***nuclei*** from a composite image - 2\ufe0f\u20e3 \n",
+                "# Infer ***nuclei*** - 2\ufe0f\u20e3 \n",
+                "\n",
+                "> WARNING: (\ud83d\udea8\ud83d\udea8\ud83d\udea8\ud83d\udea8 Steps 2-9 depend on establishing a good solution here.)\n",
                 "\n",
                 "--------------\n",
                 "\n",
-                "## OVERVIEW\n",
-                "We will start by segmenting the different cell regions - the nucleus, cell, and cytoplasm - since they will be necessary for determining which organelle are in which cell. This is integral to our single cell analysis approach.\n",
+                "## OBJECTIVE: \n",
+                "### \u2705 Infer sub-cellular component #2: ***nuclei***  in order to understand interactome \n",
                 "\n",
-                "This notebook goes through the workflow steps to segment the ***nucleus*** from a fluorescent nuclei marker.\n",
+                "Infer a segmentation of the ***nuclei*** in order to measure its shape, position, size, and interaction with other organelles/cellular components.  \n",
                 "\n",
+                "## OVERVIEW:\n",
                 "\n",
-                "## OBJECTIVE: \n",
-                "### \u2705 Infer sub-cellular component #1: ***nuclei***\n",
-                "Segment the ***nuclei*** from a composite image of multiple organelle markers combined. The ***cell*** and ***cytoplasm*** masks will also be derived from the same composite image. \n",
+                "We will infer the nuclei using the nuclei channel (e.g. 'ch = 0).\n",
                 "\n",
-                "> ***Biological relevance:***\n",
-                "> The combination of organelle markers used to create the composite image for the nucleus (and cell mask in [02_infer_cellmask_from-composite.ipynb](./02_infer_cellmask_from-composite.ipynb)) segmentation depends on the organelle labeles used and the cell type. In this example, the current selection includes the lysosomes, ER, and Golgi (e.g., Ch = 1, 3, 5) which have some intracellular background fluorescence - likely from off target marker localization. The lipid droplet channel (e.g., `ch = 6`) could also be included to produce a more unbiased selection of the entire cellmask as it binds to all cellular membranes to a small extent. However, the drawback of this is that it is present in every cell which makes downstream cell selection of a single cell more challenging. \n",
-                ">\n",
-                "> *It is important to consider specifics of your system as the cell type and labeling method may differ from the example above.*\n",
+                "Dependencies:\n",
+                "***Soma*** and ***cytosol*** inference rely on the ***nuclei*** inference.  Therefore all of the sub-cellular objects rely on the NU segmentation.\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## preamble\n",
                 "\n",
-                "> ***Convention:***  \"nuclei\" for the segmentation of ALL nuclei in the image.  \"nucleus\" for the ***single*** nucleus associated to the single cell being analyzed."
+                "1. imports\n",
+                "2. setup\n",
+                "3. infer-nuclei\n",
+                "    * input\n",
+                "    * pre-processing\n",
+                "    * core processing\n",
+                "    * post-processing\n",
+                "    * output"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -88,74 +102,161 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Get and load Image for processing"
+                "\n",
+                "## SETUP\n",
+                "CUSTOMIZE WITH: \n",
+                "1. updated path to data\n",
+                "2. updated folder name for \"raw\" data\n",
+                "\n",
+                "> NOTE: we are operating on a single \"test\" image in this notebook.  The batch-processing of all the images will be happen at the end of the notebook after we have developed/confirmed the setmentation procedures and parameter settings."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "#### Get and load an image - specifically for __multichannel \"raw\"__ images"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
-                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/Infer-subc-2D\"\n",
-                "\n",
-                "in_data_path = data_root_path / \"raw\"\n",
+                "# build the datapath\n",
+                "# all the imaging data goes here.\n",
+                "# CUSTOMIZE HERE --->\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
+                "\n",
+                "# linearly unmixed \".czi\" files are here\n",
+                "# CUSTOMIZE HERE --->\n",
+                "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
-                "img_file_list = list_image_files(in_data_path,im_type)\n",
-                "test_img_name = img_file_list[test_img_n]\n",
-                "\n",
-                "out_data_path = data_root_path / \"out\"\n",
-                "if not Path.exists(out_data_path):\n",
-                "    Path.mkdir(out_data_path)\n",
-                "    print(f\"making {out_data_path}\")"
+                "# get the list of all files in \"raw\"\n",
+                "img_file_list = list_image_files(data_path,im_type)\n",
+                "test_img_name = img_file_list[test_img_n]\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
+            "outputs": [],
+            "source": [
+                "# isolate image as an ndarray and metadata as a dictionary\n",
+                "img_data,meta_dict = read_czi_image(test_img_name)\n",
+                "\n",
+                "# get some top-level info about the RAW data\n",
+                "channel_names = meta_dict['name']\n",
+                "img = meta_dict['metadata']['aicsimage']\n",
+                "scale = meta_dict['scale']\n",
+                "channel_axis = meta_dict['channel_axis']"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "\n",
+                "### Get and load Image for processing - specifically for __pre-processed__ images\n",
+                "\n",
+                "> #### Preprocessing:\n",
+                "> In this instance, we are using [Huygens Essential Software](https://svi.nl/Homepage) to deconvolve 3D fluorescence confocal images. The output is an OME TIFF file which contains the z-slices and channels in axis 0 (channel 0, zslice 1-40, channel 1, etc. etc.).\n",
+                "\n",
+                "An OME TIFF reads in as a dask array (similar to a numpy array, but has a slightly different format)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "['C:\\\\Users\\\\Shannon\\\\Documents\\\\Python Scripts\\\\infer-subc\\\\neuron_raw_OME\\\\20221027_C2-107_well_1_cell_1_untreated_Linear_unmixing_decon.ome.tiff']"
+                        ]
+                    },
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# this will be the example for testing the pipeline below\n",
+                "test_img_n = TEST_IMG_N\n",
+                "\n",
+                "# build the datapath\n",
+                "# all the imaging data goes here.\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents\\Python Scripts\\infer-subc\"\n",
+                "\n",
+                "# linearly unmixed \".czi\" files are here\n",
+                "data_path = data_root_path / \"neuron_raw_OME\"\n",
+                "im_type = \".tiff\"\n",
+                "\n",
+                "# get the list of all files in \"raw\"\n",
+                "img_file_list = list_image_files(data_path,im_type)\n",
+                "# test_img_name = img_file_list[test_img_n]\n",
+                "# test_img_name\n",
+                "\n",
+                "img_file_list"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "c:\\Users\\Shannon\\anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:112: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "c:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:105: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
-                "img_data,meta_dict = read_czi_image(test_img_name)\n",
+                "#select one image\n",
+                "test_img = img_file_list[0]\n",
+                "\n",
+                "# isolate image as an ndarray and metadata as a dictionary\n",
+                "img_data, meta_dict = read_czi_image(test_img)\n",
                 "\n",
+                "# # get some top-level info about the RAW data\n",
                 "channel_names = meta_dict['name']\n",
                 "img = meta_dict['metadata']['aicsimage']\n",
                 "scale = meta_dict['scale']\n",
-                "channel_axis = meta_dict['channel_axis']"
+                "channel_axis = meta_dict['channel_axis']\n",
+                "huygens_meta = meta_dict['metadata']['raw_image_metadata']"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "---------\n",
-                "## infer ***nuclei*** from composite image\n",
+                "## infer ***nuclei***\n",
                 "\n",
                 "### summary of steps\n",
                 "\n",
                 "\u27a1\ufe0f INPUT\n",
-                "- create composite image from multiple organelle channels\n",
+                "- channel 1 (ER)\n",
                 "\n",
                 "PRE-PROCESSING\n",
                 "- scale to min 0, max 1.0\n",
                 "- ~~median Filter window 4~~\n",
                 "- ~~gaussian 1.34~~\n",
                 "\n",
                 "CORE-PROCESSING\n",
@@ -1502,15 +1603,14 @@
                 "\n",
                 "### NEXT: INFER CYTOSOL\n",
                 "\n",
                 "proceed to [03_infer_cytosol.ipynb](./03_infer_cytosol.ipynb)\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `infer-subc-0.0.6b0/notebooks/02b_infer_cellmask_from-membrane.ipynb` & `infer-subc-0.0.post1/notebooks/02a_cell_membrane.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/03a_infer_cellmask_from-composite_no-nuclei.ipynb` & `infer-subc-0.0.post1/notebooks/02b_infer_neurites_3D.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9287099999341941%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Infer ***cellmask*** -  1️⃣ \\n'), (2, '> WARNING: "*

 * *            "(🚨🚨🚨🚨 Steps 3-9 depend on establishing a good solution here.)\\n'), (5, '>> WARNING:  "*

 * *            "THIS DOES NOT WORK WELL - lacking fluorescent marker\\n'), (6, '>> #### Because we do "*

 * *            'NOT have a direct cell membrane / cellmask signal, this segmentation is trickiest and '*

 * *            'potentially most problematic part of the overall sub-cellular component inference '*

 * *            'p […]*

```diff
@@ -1,586 +1,533 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Infer ***nuclei*** from a composite image - 2\ufe0f\u20e3 \n",
+                "# Infer ***cellmask*** -  1\ufe0f\u20e3 \n",
                 "\n",
-                "--------------\n",
+                "> WARNING: (\ud83d\udea8\ud83d\udea8\ud83d\udea8\ud83d\udea8 Steps 3-9 depend on establishing a good solution here.)\n",
                 "\n",
-                "## OVERVIEW\n",
-                "We will start by segmenting the different cell regions - the nucleus, cell, and cytoplasm - since they will be necessary for determining which organelle are in which cell. This is integral to our single cell analysis approach.\n",
                 "\n",
-                "This notebook goes through the workflow steps to segment the ***nucleus*** from a fluorescent nuclei marker.\n",
+                ">> WARNING:  THIS DOES NOT WORK WELL - lacking fluorescent marker\n",
+                ">> #### Because we do NOT have a direct cell membrane / cellmask signal, this segmentation is trickiest and potentially most problematic part of the overall sub-cellular component inference pipeline. We are using the nuclei of the cell with the brightest total fluorescence (all channels) to identify a single cellmask for all downstream steps. The Cellmask (via the Cytosol mask) will be used to define ALL subsequent sub-cellular Objects.\n",
                 "\n",
+                "--------------\n",
                 "\n",
                 "## OBJECTIVE: \n",
-                "### \u2705 Infer sub-cellular component #1: ***nuclei***\n",
-                "Segment the ***nuclei*** from a composite image of multiple organelle markers combined. The ***cell*** and ***cytoplasm*** masks will also be derived from the same composite image. \n",
+                "### \u2705 Infer sub-cellular component #2: ***cellmask***/cell body in order to understand interactome \n",
+                "\n",
+                "Infer a segmentation of the cell body -- the ***cellmask*** -- in order to measure its shape, position, and size.\n",
+                "\n",
+                "CONTEXT: \"Cellmask\" is used here becuase subsequent experiments will contain neurons who's cellmask has a similar shape to an iPS cell body.\n",
                 "\n",
-                "> ***Biological relevance:***\n",
-                "> The combination of organelle markers used to create the composite image for the nucleus (and cell mask in [02_infer_cellmask_from-composite.ipynb](./02_infer_cellmask_from-composite.ipynb)) segmentation depends on the organelle labeles used and the cell type. In this example, the current selection includes the lysosomes, ER, and Golgi (e.g., Ch = 1, 3, 5) which have some intracellular background fluorescence - likely from off target marker localization. The lipid droplet channel (e.g., `ch = 6`) could also be included to produce a more unbiased selection of the entire cellmask as it binds to all cellular membranes to a small extent. However, the drawback of this is that it is present in every cell which makes downstream cell selection of a single cell more challenging. \n",
-                ">\n",
-                "> *It is important to consider specifics of your system as the cell type and labeling method may differ from the example above.*\n",
+                "## OVERVIEW: \n",
+                "\n",
+                "This method is used in the case where there is no cell fill/membrane marker.\n",
+                "\n",
+                "We will infer the cellmask from a combination of fluorescent signals. The current selection includes the lysosomes, ER, and Golgi (e.g., 'Ch = 1, 3, 5) which have some intracellular fluorescence - likely from off target marker localization to the entire cellmask and/or the cell membrane. There are two other channels, the residual channel from linear unmixing (e.g. `ch = 7`) and the lipid droplet channel (e.g., `ch = 6`) that could more lead to more unbiased selection of the entire cellmask. However, the drawback of these two markers is that they are present in every cell which makes downstream cell selection more challenging. To expand on this, we will be collecting per cell measurements, so each cell area has to be segmented individually even if there are two appropriately labeled cells within one field of view. "
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## preamble\n",
                 "\n",
-                "> ***Convention:***  \"nuclei\" for the segmentation of ALL nuclei in the image.  \"nucleus\" for the ***single*** nucleus associated to the single cell being analyzed."
+                "1. imports\n",
+                "2. setup\n",
+                "4. infer-cellmask\n",
+                "    * input\n",
+                "    * pre-processing\n",
+                "    * core processing\n",
+                "    * post-processing\n",
+                "    * select individual cell\n",
+                "    * output"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "\n",
-                "### IMPORTS"
+                "## IMPORTS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# top level imports\n",
                 "from pathlib import Path\n",
                 "import os, sys\n",
                 "from collections import defaultdict\n",
-                "from typing import Optional\n",
                 "\n",
                 "import numpy as np\n",
                 "\n",
-                "from aicssegmentation.core.pre_processing_utils import  image_smoothing_gaussian_slice_by_slice \n",
+                "from scipy import ndimage as ndi\n",
+                "from aicssegmentation.core.pre_processing_utils import ( intensity_normalization, \n",
+                "                                                         image_smoothing_gaussian_slice_by_slice )\n",
+                "from aicssegmentation.core.MO_threshold import MO\n",
                 "from aicssegmentation.core.utils import hole_filling\n",
-                "from skimage.measure import label\n",
-                "import skimage\n",
                 "\n",
+                "from skimage import filters\n",
+                "from skimage.segmentation import watershed\n",
+                "from skimage.morphology import remove_small_holes   # function for post-processing (size filter)\n",
+                "from skimage.measure import label\n",
                 "\n",
                 "# # package for io \n",
                 "from aicsimageio import AICSImage\n",
                 "\n",
                 "import napari\n",
                 "\n",
                 "### import local python functions in ../infer_subc\n",
                 "sys.path.append(os.path.abspath((os.path.join(os.getcwd(), '..'))))\n",
                 "\n",
                 "\n",
-                "from infer_subc.utils.file_io import (read_czi_image,\n",
+                "from infer_subc.core.file_io import (read_czi_image,\n",
                 "                                                                    list_image_files)\n",
-                "from infer_subc.utils.img import *\n",
-                "from infer_subc.organelles import fixed_get_optimal_Z_image, fixed_find_optimal_Z, find_optimal_Z\n",
+                "\n",
                 "from infer_subc.constants import (TEST_IMG_N,\n",
                 "                                                                    NUC_CH ,\n",
                 "                                                                    LYSO_CH ,\n",
                 "                                                                    MITO_CH ,\n",
                 "                                                                    GOLGI_CH ,\n",
-                "                                                                    PEROXI_CH ,\n",
+                "                                                                    PEROX_CH ,\n",
                 "                                                                    ER_CH ,\n",
-                "                                                                    LIPID_CH ,\n",
-                "                                                                    RESIDUAL_CH, \n",
-                "                                                                    ALL_CHANNELS )          \n",
+                "                                                                    LD_CH ,\n",
+                "                                                                    RESIDUAL_CH )                                                                    \n",
+                "from infer_subc.core.img import *\n",
                 "\n",
-                "from infer_subc.organelles import infer_soma, fixed_infer_soma\n",
+                "from infer_subc.organelles import fixed_get_optimal_Z_image, fixed_find_optimal_Z, find_optimal_Z\n",
                 "\n",
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Get and load Image for processing"
+                "## SETUP\n",
+                "CUSTOMIZE WITH: \n",
+                "1. updated path to data\n",
+                "2. updated folder name for \"raw\" data\n",
+                "\n",
+                "> NOTE: we are operating on a single \"test\" image in this notebook.  The batch-processing of all the images will be happen at the end of the notebook after we have developed/confirmed the setmentation procedures and parameter settings."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
-                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/Infer-subc-2D\"\n",
-                "\n",
-                "in_data_path = data_root_path / \"raw\"\n",
+                "# build the datapath\n",
+                "# all the imaging data goes here.\n",
+                "# CUSTOMIZE HERE --->\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
+                "\n",
+                "# linearly unmixed \".czi\" files are here\n",
+                "# CUSTOMIZE HERE --->\n",
+                "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
-                "img_file_list = list_image_files(in_data_path,im_type)\n",
-                "test_img_name = img_file_list[test_img_n]\n",
-                "\n",
-                "out_data_path = data_root_path / \"out\"\n",
-                "if not Path.exists(out_data_path):\n",
-                "    Path.mkdir(out_data_path)\n",
-                "    print(f\"making {out_data_path}\")"
+                "# get the list of all files\n",
+                "img_file_list = list_image_files(data_path,im_type)\n",
+                "test_img_name = img_file_list[test_img_n]\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "c:\\Users\\Shannon\\anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:112: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "c:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:105: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
+                "# isolate image as an ndarray and metadata as a dictionary\n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
                 "\n",
+                "# get some top-level info about the RAW data\n",
                 "channel_names = meta_dict['name']\n",
                 "img = meta_dict['metadata']['aicsimage']\n",
                 "scale = meta_dict['scale']\n",
                 "channel_axis = meta_dict['channel_axis']"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "---------\n",
-                "## infer ***nuclei*** from composite image\n",
+                "##  infer ***cellmask***\n",
                 "\n",
-                "### summary of steps\n",
+                "#### summary of steps\n",
                 "\n",
                 "\u27a1\ufe0f INPUT\n",
-                "- create composite image from multiple organelle channels\n",
+                "- multi-channel sum (6.*1, 3, 2.*5)\n",
+                "- nuclei mask\n",
                 "\n",
                 "PRE-PROCESSING\n",
-                "- scale to min 0, max 1.0\n",
-                "- ~~median Filter window 4~~\n",
-                "- ~~gaussian 1.34~~\n",
-                "\n",
-                "CORE-PROCESSING\n",
-                "  - threshold method otsu  \n",
-                "    - threshold correction factor: 0.05\n",
-                "    - lower / upper bounds  (0, 1)\n",
-                "  - invert segmentation\n",
+                "- rescaling\n",
+                "- denoise/smoothing\n",
+                "- log transform inensities\n",
+                "- scale to max 1.0\n",
+                "- create non-linear aggregate of log-intensity + scharr edge filtered intensity\n",
+                "\n",
+                "CORE PROCESSING\n",
+                "- mask object segmentation at bottom\n",
                 "\n",
                 "POST-PROCESSING\n",
                 "  - fill holes\n",
                 "  - remove small objects\n",
-                "  - label\n",
-                "  - remove objects touching image edges\n",
                 "\n",
                 "OUTPUT \u27a1\ufe0f \n",
-                "- mask of NUCLEI\n"
+                "- mask of CELLMASK\n",
+                "\n",
+                "\n",
+                "> #### Note: this pipeline will eventually include a selection step to identify the cellmask that are properly labeled with all fluorescent markers. This could be one single cell per image, or more if applicable data is available."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## INPUT (prototype)\n",
                 "\n",
-                "Get the \"raw\" signals we need to analyze as well as any other dependencies in \"inferred\" objects.  "
+                "Combine multiple channels that will allow inference of the cellmask.\n",
+                "\n",
+                "Note: the selected channels were chosen based on their qualitative ability to fill the cytoplasmic area of the cell. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(49, 1688, 1688)\n"
+                        "(17, 704, 704)\n",
+                        "(17, 704, 704)\n"
                     ]
                 }
             ],
             "source": [
-                "# ###################\n",
-                "# # INPUT\n",
-                "# ###################\n",
-                "# # raw_nuclei = img_data[NUC_CH].copy()\n",
-                "# raw_nuclei = select_channel_from_raw(img_data, NUC_CH)\n",
+                "###################\n",
+                "# INPUT\n",
+                "###################\n",
+                "struct_img_raw = (6. * img_data[LYSO_CH].copy() +\n",
+                "                  1. * img_data[ER_CH].copy() + \n",
+                "                  2. * img_data[GOLGI_CH].copy())\n",
                 "\n",
-                "# print(raw_nuclei.shape)\n",
+                "raw_nuclei = img_data[NUC_CH].copy() \n",
                 "\n",
-                "raw_nuclei = img_data[1]\n",
+                "print(struct_img_raw.shape)\n",
                 "print(raw_nuclei.shape)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## PRE-PROCESSING (prototype)"
+                "### VISUALIZE: the composite image that will be used as input\n",
+                "Use this to adjust which channels and multiplication factors to use to create the composite input image above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "###################\n",
-                "# PRE_PROCESSING\n",
-                "###################           \n",
-                "nuclei_norm = min_max_intensity_normalization(raw_nuclei)\n",
-                "\n",
-                "#### smoothing is no longer necessary here - Huygens preprocessing took care of that already\n",
-                "\n",
-                "# med_filter_size = 4   \n",
-                "# nuclei_med = median_filter_slice_by_slice(nuclei_norm,\n",
-                "#                                       size=med_filter_size)\n",
-                "# print(nuclei_med.shape)\n",
-                "\n",
-                "# gaussian_smoothing_sigma = 1.34\n",
-                "# nuclei_gaus = image_smoothing_gaussian_slice_by_slice(nuclei_med,\n",
-                "#                                                       sigma=gaussian_smoothing_sigma)\n",
-                "# print(nuclei_gaus.shape)\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### VISUALIZE: the nuclei image after pre-processing\n",
-                "Use this to adjust median filter size and gaussian sigma above."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "WARNING: QWindowsWindow::setGeometry: Unable to set geometry 1090x686+1+15 (frame: 1108x733-8-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+2+22 (frame: 1383x906-7-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n",
-                        "15-Mar-23 16:01:10 - vispy    - WARNING  - QWindowsWindow::setGeometry: Unable to set geometry 1090x686+1+15 (frame: 1108x733-8-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+2+22 (frame: 1383x906-7-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'img_data' at 0x25e5031c3a0>"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "viewer = napari.Viewer()"
+                "viewer = napari.Viewer()\n",
+                "viewer.add_image(\n",
+                "    img_data,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'nuclei_norm' at 0x22fcfeab640>"
+                            "<Image layer 'struct_img_raw' at 0x25e527b0430>"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    raw_nuclei,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    nuclei_norm,\n",
+                "    struct_img_raw,\n",
                 "    scale=scale\n",
-                ")\n",
-                "# viewer.add_image(\n",
-                "#     nuclei_gaus,\n",
-                "#     scale=scale\n",
-                "# )"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## CORE PROCESSING (prototype)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "\n",
-                "> #### ASIDE: Thresholding\n",
-                "> [Thresholding](https://en.wikipedia.org/wiki/Thresholding_%28image_processing%29) is used to create binary images. A threshold value determines the intensity value separating foreground pixels from background pixels. Foregound pixels are pixels brighter than the threshold value, background pixels are darker. In many cases, images can be adequately segmented by thresholding followed by labelling of *connected components*, which is a fancy way of saying \"groups of pixels that touch each other\".\n",
-                "> \n",
-                "> Different thresholding algorithms produce different results. [Otsu's method](https://en.wikipedia.org/wiki/Otsu%27s_method) and [Li's minimum cross entropy threshold](https://scikit-image.org/docs/dev/auto_examples/developers/plot_threshold_li.html) are two common algorithms. Below, we use Li. You can use `skimage.filters.threshold_<TAB>` to find different thresholding methods.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "\n",
-                "###################\n",
-                "# CORE_PROCESSING\n",
-                "###################\n",
-                "threshold_factor = 0.05 #from cellProfiler\n",
-                "thresh_min = 0\n",
-                "thresh_max = 1\n",
-                "threshold = apply_threshold(nuclei_norm, thresh_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "bw = nuclei_norm < threshold\n",
-                "bw_invert = 1 - bw\n",
-                "\n",
-                "bw_labeled = label(bw_invert, connectivity=1)\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### VISUALIZE: the nuclei image after core processing\n",
-                "Use this to adjust threshold parameters above."
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'bw_labeled' at 0x22f80708a30>"
+                            "<Image layer '_struct_img_raw' at 0x25e50a57340>"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "def _raw_cellmask_MCZ(img_in):\n",
+                "    \"\"\" define cellmask image\n",
+                "    \"\"\"\n",
+                "    CELLMASK_W = (6.,1.,2.)\n",
+                "    CELLMASK_CH = (LYSO_CH,ER_CH,GOLGI_CH)\n",
+                "    img_out = np.zeros_like(img_in[0]).astype(np.double)\n",
+                "    for w,ch in zip(CELLMASK_W,CELLMASK_CH):\n",
+                "        img_out += w*img_in[ch]\n",
+                "    return img_out\n",
+                "\n",
+                "_struct_img_raw = _raw_cellmask_MCZ(img_data)\n",
+                "\n",
                 "viewer.add_image(\n",
-                "    bw,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    bw_invert,\n",
+                "    _struct_img_raw,\n",
                 "    scale=scale\n",
-                ")\n",
-                "viewer.add_labels(\n",
-                "    bw_labeled,\n",
-                "    scale=scale\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## POST PROCESSING prototype\n",
-                "\n",
-                "> NOTE: the size parameters are by convention defined as one dimensional \"width\", so the inputs to the functions need to be _squared_ i.e. raised to the power of 2: `** 2`.   For volumetric (3D) analysis this would be _cubed_:`**3`"
+                "## PRE-PROCESSING (prototype)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                }
+            ],
             "source": [
+                "\n",
                 "###################\n",
-                "# POST_PROCESSING\n",
+                "# PRE_PROCESSING\n",
                 "###################\n",
                 "\n",
-                "hole_width = 30 \n",
-                "removed_holes = hole_filling(bw_invert,\n",
-                "                             hole_min=0, \n",
-                "                             hole_max=hole_width**3, \n",
-                "                             fill_2d=False)\n",
+                "################# smoothing\n",
+                "cellmask_norm = min_max_intensity_normalization(struct_img_raw)\n",
                 "\n",
-                "small_object_width = 20\n",
-                "cleaned_img = size_filter(removed_holes, \n",
-                "                          min_size= small_object_width**3, #changed this to 3 to adjust for the 3D voxel, instead of a 2D pixel \n",
-                "                          method=\"3D\",\n",
-                "                          connectivity=1)\n",
+                "med_filter_size = 15\n",
+                "cellmask_med = median_filter_slice_by_slice(cellmask_norm, \n",
+                "                                        size=med_filter_size)\n",
                 "\n",
-                "all_labels = label(cleaned_img, connectivity=1)\n",
+                "## Need to adjust image_smoothing_gaussian_slice_by_slice in pre_processing_utils.py to integrate the mode\n",
                 "\n",
-                "nuclei_label = skimage.segmentation.clear_border(all_labels)\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### VISUALIZE: the nuclei image after post-processing\n",
-                "Use this to adjust the size parameters above."
+                "gaussian_smoothing_sigma = 1.34\n",
+                "gaussian_smoothing_truncate_range = 3.0\n",
+                "cellmask_guas = ndi.gaussian_filter(cellmask_med,\n",
+                "                                sigma=gaussian_smoothing_sigma,\n",
+                "                                mode=\"nearest\", \n",
+                "                                truncate=gaussian_smoothing_truncate_range)\n",
+                "\n",
+                "\n",
+                "################# NON-Linear aggregation\n",
+                "cellmask_log, d = log_transform(cellmask_guas) \n",
+                "cellmask_log_norm = intensity_normalization(cellmask_log, scaling_param=[0])\n",
+                "\n",
+                "# cellmask_edges = filters.difference_of_gaussians(cellmask_log_norm, 2)\n",
+                "\n",
+                "# composite_cellmask = intensity_normalization(cellmask_edges, scaling_param=[0]) + cellmask_log_norm "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'nuclei_label' at 0x22f80a79eb0>"
+                            "<Image layer 'composite_cellmask' at 0x25e437c8bb0>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    removed_holes,\n",
+                "    cellmask_med,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    cleaned_img,\n",
+                "    cellmask_guas,\n",
                 "    scale=scale\n",
                 ")\n",
-                "viewer.add_labels(\n",
-                "    all_labels,\n",
+                "viewer.add_image(\n",
+                "    cellmask_log_norm,\n",
                 "    scale=scale\n",
                 ")\n",
-                "viewer.add_labels(\n",
-                "    nuclei_label,\n",
-                "    scale=scale\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer.close()"
+                "# viewer.add_image(\n",
+                "#     cellmask_edges,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "# viewer.add_image(\n",
+                "#     composite_cellmask,\n",
+                "#     scale=scale\n",
+                "# )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Adjust naming and type for labels"
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 11,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer '_log_cellmask' at 0x25e437e2d90>"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "NU_signal = raw_nuclei\n",
+                "def _non_linear_cellmask_transform_MCZ(in_img):\n",
+                "    \"\"\" non-linear distortion to fill out cellmask\n",
+                "    log + edge of smoothed composite\n",
+                "    \"\"\"\n",
+                "    # non-Linear processing\n",
+                "    log_img, d = log_transform(in_img.copy()) \n",
+                "    return intensity_normalization(log_img,scaling_param=[0])\n",
+                "    # return intensity_normalization(filters.difference_of_gaussians(log_img, 2),scaling_param=[0])  + log_img\n",
                 "\n",
-                "# renaming semantic segmentation of nuclei\n",
-                "nuclei_object = cleaned_img\n",
+                "_log_cellmask = _non_linear_cellmask_transform_MCZ(cellmask_guas)\n",
                 "\n",
-                "# creating instance segmentations for all nuclei in nuclei_object\n",
-                "NU_labels = label(cleaned_img)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### VISUALIZE final segmentations"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer = napari.Viewer()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "viewer.add_image(\n",
-                "    NU_signal,\n",
-                "    scale=scale,\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    nuclei_object,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n",
-                "viewer.add_labels(\n",
-                "    NU_labels,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer.close()"
+                "    _log_cellmask,\n",
+                "    scale=scale\n",
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## DEFINE `_infer_nuclei` function\n",
-                "\n",
-                "Based on the _prototyping_ above define the function to infer nuclei.  \n"
+                "<code style=\"background:yellow;color:black\">Eventually this will be replaced by calling the un-name mangled version of the infer nuclei code that will be in infer-subc.organelles.</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
-                "##########################\n",
-                "#  _infer_nuclei\n",
-                "##########################\n",
-                "def _infer_nucleifromER_3D( in_img: np.ndarray,\n",
+                "################# part 2 Nuclei pre-process\n",
+                "def _infer_nuclei_3D( in_img: np.ndarray,\n",
+                "                       median_sz: int, \n",
+                "                       gauss_sig: float,\n",
                 "                       thresh_factor: float,\n",
                 "                       thresh_min: float,\n",
                 "                       thresh_max: float,\n",
                 "                       max_hole_w: int,\n",
                 "                       small_obj_w: int,\n",
                 "                       sz_filter_method: str\n",
                 "                     ) -> np.ndarray:\n",
                 "    \"\"\"\n",
                 "    Procedure to infer 3D nuclei segmentation from multichannel z-stack input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
-                "    cellmask: Optional[np.ndarray] = None\n",
+                "    cellmask_mask: Optional[np.ndarray] = None\n",
                 "        mask\n",
+                "    median_sz: int\n",
+                "        width of median filter for signal\n",
+                "    gauss_sig: float\n",
+                "        sigma for gaussian smoothing of  signal\n",
                 "    thresh_factor: float\n",
                 "        adjustment factor for log Li threholding\n",
                 "    thresh_min: float\n",
                 "        abs min threhold for log Li threholding\n",
                 "    thresh_max: float\n",
                 "        abs max threhold for log Li threholding\n",
                 "    max_hole_w: int\n",
@@ -593,334 +540,826 @@
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "    \n",
                 "    \"\"\"\n",
                 "\n",
-                "    # nuc_ch_from_ER = ER_CH\n",
-                "    # nuclei = select_channel_from_raw(in_img, nuc_ch_from_ER)\n",
-                "    nuclei = in_img[1]\n",
+                "    nuc_ch = NUC_CH\n",
+                "    nuclei = select_channel_from_raw(in_img, nuc_ch)\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
                 "    ###################                \n",
                 "    nuclei = min_max_intensity_normalization(nuclei)\n",
+                "    nuclei = median_filter_slice_by_slice(nuclei,\n",
+                "                                          size=median_sz)\n",
+                "    nuclei = image_smoothing_gaussian_slice_by_slice(nuclei,\n",
+                "                                                     sigma=gauss_sig )\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    thresh_value = apply_threshold(nuclei, \n",
-                "                                   thresh_factor=thresh_factor, \n",
-                "                                   thresh_min=thresh_min, \n",
-                "                                   thresh_max=thresh_max)\n",
-                "    nuclei_object = nuclei < thresh_value\n",
-                "    nuclei_object = 1 - nuclei_object\n",
+                "    nuclei_object = apply_log_li_threshold(nuclei, \n",
+                "                                           thresh_factor=thresh_factor, \n",
+                "                                           thresh_min=thresh_min, \n",
+                "                                           thresh_max=thresh_max)\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
                 "    nuclei_object = hole_filling(nuclei_object, \n",
                 "                                 hole_min=0, \n",
-                "                                 hole_max=max_hole_w**3, \n",
-                "                                 fill_2d=False)\n",
+                "                                 hole_max=max_hole_w**2, \n",
+                "                                 fill_2d=True)\n",
                 "\n",
                 "    nuclei_object = size_filter(nuclei_object, \n",
                 "                                min_size = small_obj_w**3, \n",
                 "                                method = sz_filter_method,\n",
                 "                                connectivity=1)\n",
-                "    \n",
-                "    nuclei_object = label(nuclei_object, connectivity=1)\n",
-                "    \n",
-                "    nuclei_object = skimage.segmentation.clear_border(nuclei_object)\n",
                 "\n",
-                "    return nuclei_object\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## DEFINE `_fixed_infer_nuclei` function\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 19,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "##########################\n",
-                "#  fixed_infer_nuclei\n",
-                "##########################\n",
+                "\n",
+                "    return nuclei_object\n",
+                "\n",
+                "\n",
                 "def _fixed_infer_nuclei_3D(in_img: np.ndarray) -> np.ndarray:\n",
                 "    \"\"\"\n",
-                "    Procedure to infer soma from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
-                "    cellmask: np.ndarray\n",
+                "    cellmask_mask: np.ndarray\n",
                 "        mask\n",
                 " \n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "    \n",
                 "    \"\"\"\n",
                 "\n",
                 "    nuc_ch = NUC_CH\n",
-                "    threshold_factor = 0.05\n",
-                "    thresh_min = 0\n",
+                "    median_sz = 4     \n",
+                "    gauss_sig = 1.34\n",
+                "    threshold_factor = 0.9\n",
+                "    thresh_min = 0.1\n",
                 "    thresh_max = 1.0\n",
-                "    max_hole_w = 30\n",
-                "    small_obj_w = 20\n",
+                "    max_hole_w = 5\n",
+                "    small_obj_w = 15\n",
                 "    sz_filter_method = \"3D\"\n",
                 "\n",
-                "    return _infer_nucleifromER_3D( in_img,\n",
+                "    return _infer_nuclei_3D( in_img,\n",
+                "                             median_sz,\n",
+                "                             gauss_sig,\n",
                 "                             threshold_factor,\n",
                 "                             thresh_min,\n",
                 "                             thresh_max,\n",
                 "                             max_hole_w,\n",
                 "                             small_obj_w,\n",
-                "                             sz_filter_method )\n"
+                "                             sz_filter_method )\n",
+                "\n",
+                "\n",
+                "_NU_object =  _fixed_infer_nuclei_3D(img_data) \n",
+                "NU_labels = label(_NU_object)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "---------------------\n",
-                "## TEST `_infer_nuclei`  function defined above\n"
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 13,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "\n",
+                "def _masked_object_thresh(\n",
+                "    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float\n",
+                ") -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    wrapper for applying Masked Object Thresholding with just two parameters via `MO` from `aicssegmentation`\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    structure_img_smooth: np.ndarray\n",
+                "        a 3d image\n",
+                "    th_method: \n",
+                "         which method to use for calculating global threshold. Options include:\n",
+                "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
+                "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
+                "    cutoff_size: \n",
+                "        Masked Object threshold `size_min`\n",
+                "    th_adjust: \n",
+                "        Masked Object threshold `local_adjust`\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "        np.ndimage \n",
+                "\n",
+                "    \"\"\"\n",
+                "\n",
+                "    struct_obj = MO(\n",
+                "        structure_img_smooth,\n",
+                "        global_thresh_method=th_method,\n",
+                "        object_minArea=cutoff_size,\n",
+                "        extra_criteria=True,\n",
+                "        local_adjust=th_adjust,\n",
+                "        return_object=False,\n",
+                "        dilate=True,\n",
+                "    )\n",
+                "    return struct_obj\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## CORE PROCESSING"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
-                "_NU_object =  _fixed_infer_nuclei_3D(img_data) "
+                "###################\n",
+                "# CORE_PROCESSING\n",
+                "###################\n",
+                "low_level_min_size =  50\n",
+                "\n",
+                "# ################# part 1\n",
+                "cellmask_binary = _masked_object_thresh(cellmask_log_norm, \n",
+                "                           th_method='ave', \n",
+                "                           cutoff_size=low_level_min_size, \n",
+                "                           th_adjust= 0.15)                                           "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "WARNING: QWindowsWindow::setGeometry: Unable to set geometry 1090x686+2+15 (frame: 1108x733-7-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+3+22 (frame: 1383x906-6-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n",
-                        "15-Mar-23 16:08:23 - vispy    - WARNING  - QWindowsWindow::setGeometry: Unable to set geometry 1090x686+2+15 (frame: 1108x733-7-23) on QWidgetWindow/\"_QtMainWindowClassWindow\" on \"\\\\.\\DISPLAY1\". Resulting geometry: 1365x859+3+22 (frame: 1383x906-6-16) margins: 9, 38, 9, 9 minimum size: 612x589 MINMAXINFO maxSize=0,0 maxpos=0,0 mintrack=630,636 maxtrack=0,0)\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'cellmask_binary' at 0x25e438999d0>"
+                        ]
+                    },
+                    "execution_count": 15,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "viewer = napari.Viewer()"
+                "viewer.add_image(\n",
+                "    cellmask_binary,\n",
+                "    scale=scale\n",
+                ")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## POST-PROCESSING\n",
+                "\n",
+                "<code style=\"background:yellow;color:black\">Watershed (with or without the nuclei as a marker) does not work well here to get an instance segmentation</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 16,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "###################\n",
+                "# POST_PROCESSING\n",
+                "###################\n",
+                "hole_width = 100\n",
+                "removed_holes = hole_filling(cellmask_binary, \n",
+                "                            hole_min=0, \n",
+                "                            hole_max=hole_width**2,\n",
+                "                            fill_2d = True) \n",
+                "\n",
+                "\n",
+                "small_object_width = 45\n",
+                "cleaned_img = size_filter_2D(removed_holes, \n",
+                "                             min_size= small_object_width**3, \n",
+                "                             connectivity=1)\n",
+                "\n",
+                "\n",
+                "watershed_mask = cleaned_img \n",
+                "inverted_img = 1. - cleaned_img\n",
+                "\n",
+                "labels_out = watershed(\n",
+                "            inverted_img,\n",
+                "            markers=NU_labels,\n",
+                "            connectivity= 3, # np.ones((1,3,3), bool),\n",
+                "            mask=watershed_mask,\n",
+                "            )"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_NU_object' at 0x22fac2096a0>"
+                            "<Labels layer 'labels_out' at 0x25e52d71a60>"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    NU_signal,\n",
-                "    scale=scale,\n",
+                "    removed_holes,\n",
+                "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    nuclei_object,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n",
-                "viewer.add_labels(\n",
-                "    NU_labels,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
+                "    cleaned_img,\n",
+                "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    _NU_object,\n",
+                "    inverted_img,\n",
+                "    scale=scale\n",
+                ")\n",
+                "viewer.add_labels(\n",
+                "    labels_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 19,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Labels layer '_labels_out [1]' at 0x25e43b8f550>"
+                        ]
+                    },
+                    "execution_count": 19,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "viewer.close()"
+                "def _masked_inverted_watershed(img_in, markers, mask):\n",
+                "    \"\"\"wrapper for watershed on inverted image and masked\n",
+                "\n",
+                "    \"\"\"\n",
+                "    labels_out = watershed(\n",
+                "                1. - img_in,\n",
+                "                markers=markers,\n",
+                "                connectivity=3,\n",
+                "                mask=mask,\n",
+                "                )\n",
+                "    return labels_out\n",
+                "\n",
+                "\n",
+                "_labels_out = _masked_inverted_watershed(cleaned_img, NU_labels, cleaned_img)\n",
+                "\n",
+                "viewer.add_labels(\n",
+                "    _labels_out,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\"> ***SR edits stops here***</code>\n",
+                "## POST POST-PROCESSING\n",
                 "\n",
-                "---------------------\n",
-                "# TEST `infer_nuclei` exported functions\n",
+                "<code style=\"background:yellow;color:black\">This should eventually be altered to maintain all cells that have the correct number of organelle markers</code>\n",
+                "\n",
+                "What is we used the nuclei (or an expanded nuclei) to select the cells with the most signal, then after selecting the nuclei with signal, use those as the watershed marker - I think it may resolve some conflicts, but not all"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 20,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'cellmask_out' at 0x25e52975190>"
+                        ]
+                    },
+                    "execution_count": 20,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "###################\n",
+                "# POST- POST_PROCESSING\n",
+                "###################\n",
+                "# keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "all_labels = np.unique(labels_out)[1:]\n",
+                "\n",
+                "total_signal = [cellmask_norm[labels_out == label].sum() for label in all_labels]\n",
+                "keep_label = all_labels[np.argmax(total_signal)]\n",
+                "keep_label\n",
                 "\n",
-                "> the prototype `_infer_nuclei` was copied to the [`.organelles.nuclei`](../infer_subc/organelles/nuclei.py) sub-module \n",
-                "##\n",
-                "`infer_nuclei` procedure\n",
+                "cellmask_out = np.zeros_like(labels_out)\n",
+                "cellmask_out[labels_out==keep_label] = 1\n",
                 "\n",
-                "Use the `infer_nuclei` function to infer the Nucleus and export it as an _ome.tif_ for easy reference."
+                "viewer.add_image(\n",
+                "    cellmask_out,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 21,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer '_cellmask_out' at 0x25e43926160>"
+                        ]
+                    },
+                    "execution_count": 21,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "from infer_subc.organelles.nuclei import infer_nuclei, fixed_infer_nuclei\n",
+                "def _choose_max_label(raw_signal: np.ndarray, labels_in: np.ndarray):\n",
+                "    \"\"\" keep only the label with the maximum raw signal\n",
+                "\n",
+                "    \"\"\"\n",
+                "\n",
+                "    all_labels = np.unique(labels_in)[1:]\n",
+                "\n",
+                "    total_signal = [raw_signal[labels_in == label].sum() for label in all_labels]\n",
+                "    # combine NU and \"labels\" to make a CELLMASK\n",
+                "    keep_label = all_labels[np.argmax(total_signal)]\n",
+                "\n",
+                "    labels_max = np.zeros_like(labels_in)\n",
+                "    labels_max[labels_in==keep_label] = 1\n",
+                "    return labels_max\n",
                 "\n",
-                "nuclei_object =  fixed_infer_nuclei(img_2D, cellmask) \n"
+                "_cellmask_out = _choose_max_label(cellmask_norm,labels_out)\n",
+                "\n",
+                "viewer.add_image(\n",
+                "    _cellmask_out,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Visualize  2\n"
+                "\n",
+                "\n",
+                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## DEFINE parameterized  `_infer_cellmask` function\n",
+                "\n",
+                "A function to infer_cellmask from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
+                "-  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 37,
             "metadata": {},
             "outputs": [],
             "source": [
-                "viewer.add_image(\n",
-                "    _NU_object,\n",
+                "##########################\n",
+                "# 1. infer_cellmask\n",
+                "##########################\n",
+                "\n",
+                "def _infer_cellmask_3D(in_img: np.ndarray,\n",
+                "    nuclei_labels: np.ndarray,\n",
+                "    median_sz_cellmask: int,\n",
+                "    gauss_sig_cellmask: float,\n",
+                "    gauss_truc_rang: float,\n",
+                "    mo_method: str,\n",
+                "    mo_adjust: float,\n",
+                "    mo_cutoff_size: int,\n",
+                "    max_hole_w_cellmask: int,\n",
+                "    small_obj_w_cellmask: int\n",
+                ") -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input.\n",
+                "\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    in_img: \n",
+                "        a 3d image containing all the channels\n",
+                "    nuclei_labels:\n",
+                "        a 3d mask of nuclei\n",
+                "    median_sz_cellmask: \n",
+                "        width of median filter for _cellmask_ signal\n",
+                "    gauss_sig_cellmask: \n",
+                "        sigma for gaussian smoothing of _cellmask_ signal\n",
+                "    gauss_truc_rang:\n",
+                "        cutoff value for gaussian\n",
+                "    mo_method: \n",
+                "         which method to use for calculating global threshold. Options include:\n",
+                "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
+                "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
+                "    mo_adjust: \n",
+                "        Masked Object threshold `local_adjust`\n",
+                "    mo_cutoff_size: \n",
+                "        Masked Object threshold `size_min`\n",
+                "    max_hole_w_cellmask: \n",
+                "        hole filling cutoff for cellmask signal post-processing\n",
+                "    small_obj_w_cellmask: \n",
+                "        minimu object size cutoff for cellmask signal post-processing\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "    cellmask_mask:\n",
+                "        a logical/labels object defining boundaries of cellmask\n",
+                "\n",
+                "    \"\"\"\n",
+                "\n",
+                "    ###################\n",
+                "    # EXTRACT\n",
+                "    ###################\n",
+                "    struct_img = _raw_cellmask_MCZ(in_img)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
                 "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n",
+                "    name=1\n",
+                "    )\n",
                 "\n",
                 "\n",
-                "viewer.add_labels(\n",
-                "    label(_NU_object),\n",
+                "    ###################\n",
+                "    # PRE_PROCESSING\n",
+                "    ###################                         \n",
+                "    ################# part 1- cellmask\n",
+                "    struct_img = min_max_intensity_normalization(struct_img)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
                 "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")\n"
+                "    name=2\n",
+                "    )\n",
+                "\n",
+                "    # make a copy for post-post processing\n",
+                "    scaled_signal = struct_img.copy()\n",
+                "\n",
+                "    # Linear-ish processing\n",
+                "    struct_img = median_filter_slice_by_slice(struct_img, \n",
+                "                                              size=median_sz_cellmask)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
+                "    scale=scale,\n",
+                "    name=3\n",
+                "    )\n",
+                "\n",
+                "    struct_img = ndi.gaussian_filter(struct_img,\n",
+                "                                     sigma=gauss_sig_cellmask,\n",
+                "                                     mode=\"nearest\",\n",
+                "                                     truncate=gauss_truc_rang)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
+                "    scale=scale,\n",
+                "    name=4\n",
+                "    )\n",
+                "\n",
+                "\n",
+                "    # struct_img_non_lin, d = log_transform(struct_img)\n",
+                "    # struct_img_non_lin = intensity_normalization(struct_img_non_lin, scaling_param=[0])\n",
+                "    struct_img_non_lin = _non_linear_cellmask_transform_MCZ(struct_img)\n",
+                "    viewer.add_image(\n",
+                "    struct_img_non_lin,\n",
+                "    scale=scale,\n",
+                "    name=5\n",
+                "    )\n",
+                "   \n",
+                "    ###################\n",
+                "    # CORE_PROCESSING\n",
+                "    ###################    \n",
+                "    struct_obj = _masked_object_thresh(struct_img_non_lin, \n",
+                "                                       th_method=mo_method, \n",
+                "                                       cutoff_size=mo_cutoff_size, \n",
+                "                                       th_adjust=mo_adjust)               \n",
+                "    viewer.add_image(\n",
+                "    struct_obj,\n",
+                "    scale=scale,\n",
+                "    name=6\n",
+                "    )\n",
+                "\n",
+                "    ###################\n",
+                "    # POST_PROCESSING\n",
+                "    ###################\n",
+                "    struct_obj = hole_filling(struct_obj, \n",
+                "                              hole_min =0 , \n",
+                "                              hole_max=max_hole_w_cellmask**2, \n",
+                "                              fill_2d = True) \n",
+                "    viewer.add_image(\n",
+                "    struct_obj,\n",
+                "    scale=scale,\n",
+                "    name=7\n",
+                "    )\n",
+                "\n",
+                "    struct_obj = size_filter_2D(struct_obj, \n",
+                "                                min_size= small_obj_w_cellmask**3, \n",
+                "                                connectivity=1)\n",
+                "    viewer.add_image(\n",
+                "    struct_obj,\n",
+                "    scale=scale,\n",
+                "    name=8\n",
+                "    )\n",
+                "\n",
+                "    labels_out = _masked_inverted_watershed(struct_obj, nuclei_labels, struct_obj)\n",
+                "    viewer.add_image(\n",
+                "    labels_out,\n",
+                "    scale=scale,\n",
+                "    name=9\n",
+                "    )\n",
+                "\n",
+                "    ###################\n",
+                "    # POST- POST_PROCESSING\n",
+                "    ###################\n",
+                "    # keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "    cellmask_out = _choose_max_label(struct_img, labels_out)\n",
+                "\n",
+                "    return cellmask_out\n",
+                "\n",
+                "\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## DEFINE `_fixed_infer_cellmask` function\n",
+                "\n",
+                "Based on the _prototyping_ above define the function to infer cellmask. with a *fixed* set of parameters for each step in the procedure.  That is they are all \"hard coded\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 34,
             "metadata": {},
             "outputs": [],
             "source": [
+                "##########################\n",
+                "# 1. fixed_infer_cellmask\n",
+                "##########################\n",
+                "\n",
+                "\n",
+                "def _fixed_infer_cellmask_3D(in_img: np.ndarray, nuclei_labels: np.ndarray) -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
+                "\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    in_img: \n",
+                "        a 3d image containing all the channels\n",
+                "    nuclei_object:\n",
+                "        a 3d mask of nuclei\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "    cellmask_mask:\n",
+                "        a logical/labels object defining boundaries of cellmask\n",
+                "    \"\"\"\n",
+                "    \n",
+                "\n",
+                "    ###################\n",
+                "    # PARAMETERS\n",
+                "    ###################   \n",
+                "    median_sz_cellmask = 15\n",
+                "    gauss_sig_cellmask = 1.34\n",
+                "    gauss_truc_rang = 3.0\n",
+                "    mo_method = \"ave\"\n",
+                "    mo_adjust = 0.15\n",
+                "    mo_cutoff_size = 50\n",
+                "    max_hole_w_cellmask = 100\n",
+                "    small_obj_w_cellmask = 45\n",
+                "\n",
+                "    cellmask_out = _infer_cellmask_3D(in_img,\n",
+                "                              nuclei_labels,\n",
+                "                              median_sz_cellmask,\n",
+                "                              gauss_sig_cellmask,\n",
+                "                              gauss_truc_rang,\n",
+                "                              mo_method,\n",
+                "                              mo_adjust,\n",
+                "                              mo_cutoff_size,\n",
+                "                              max_hole_w_cellmask,\n",
+                "                              small_obj_w_cellmask) \n",
+                "\n",
+                "    return cellmask_out\n",
+                "\n",
+                "\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 38,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                }
+            ],
+            "source": [
+                "\n",
+                "SO_label =  _fixed_infer_cellmask_3D(img_data, NU_labels) "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 39,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'SO_label [1]' at 0x25ea42fd970>"
+                        ]
+                    },
+                    "execution_count": 39,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
                 "viewer.add_image(\n",
-                "    nuclei_object,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n"
+                "    SO_label,\n",
+                "    scale=scale\n",
+                ")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "---------------------\n",
+                "# TEST `_infer_cellmask`  function defined above\n",
+                "\n",
+                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>\n",
+                "##\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from napari.utils.notebook_display import nbscreenshot\n",
+                "from infer_subc.organelles import fixed_infer_cellmask, infer_cellmask\n",
                 "\n",
-                "# viewer.dims.ndisplay = 3\n",
-                "# viewer.camera.angles = (-30, 25, 120)\n",
-                "nbscreenshot(viewer, canvas_only=True)\n"
+                "cellmask_ =  fixed_infer_cellmask(img_2D) "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "viewer.close()"
+                "viewer.add_image(\n",
+                "    SO_label,\n",
+                "    scale=scale\n",
+                ")\n",
+                "viewer.add_image(\n",
+                "    cellmask_,\n",
+                "    scale=scale \n",
+                ")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "-----------------\n",
-                "Write the `infer_nuclei` spec to the widget json "
+                "Write the `infer_cellmask` spec to the widget json"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
-                "_fixed_infer_nuclei =  {\n",
-                "        \"name\": \"infer nuclei  (fixed parameters)\",\n",
+                "_fixed_infer_cellmask =  {\n",
+                "        \"name\": \" infer cellmask mask (fixed parameters)\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"fixed_infer_nuclei\",\n",
+                "        \"python::function\": \"fixed_infer_cellmask\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"fixed_infer_nuclei\",_fixed_infer_nuclei)"
+                "add_function_spec_to_widget_json(\"fixed_infer_cellmask\", _fixed_infer_cellmask, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "_infer_nuclei =  {\n",
-                "        \"name\": \"infer nuclei\",\n",
+                "_infer_cellmask =  {\n",
+                "        \"name\": \" infer cellmask mask\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_nuclei\",\n",
+                "        \"python::function\": \"infer_cellmask\",\n",
                 "        \"parameters\": {\n",
-                "                \"median_sz\": {\n",
+                "                \"median_sz_cellmask\": {\n",
                 "                        \"widget_type\": \"slider\",\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"min\": 3,\n",
                 "                        \"max\": 15,\n",
                 "                        \"increment\": 1\n",
                 "                },\n",
-                "                \"gauss_sig\": {\n",
+                "                \"gauss_sig_cellmask\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.25,\n",
                 "                        \"max\": 15.0,\n",
                 "                        \"min\": 1.25,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
+                "                \"median_sz_nuc\": {\n",
+                "                        \"widget_type\": \"slider\",\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"min\": 3,\n",
+                "                        \"max\": 15,\n",
+                "                        \"increment\": 1\n",
+                "                },\n",
+                "                \"gauss_sig_nuc\": {\n",
+                "                        \"data_type\": \"float\",\n",
+                "                        \"increment\": 0.25,\n",
+                "                        \"max\": 15.0,\n",
+                "                        \"min\": 1.25,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },\n",
+                "                \"mo_method\": {\n",
+                "                        \"data_type\": \"str\",\n",
+                "                        \"widget_type\": \"drop-down\",\n",
+                "                        \"options\": [\n",
+                "                                \"triangle\",\n",
+                "                                \"median\",\n",
+                "                                \"ave_tri_med\"\n",
+                "                                ]\n",
+                "                },\n",
+                "                \"mo_adjust\": {\n",
+                "                        \"data_type\": \"float\",\n",
+                "                        \"increment\": 0.05,\n",
+                "                        \"max\": 1.0,\n",
+                "                        \"min\": 0.0,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },\n",
+                "                \"mo_cutoff_size\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"increment\": 10,\n",
+                "                        \"max\": 250,\n",
+                "                        \"min\": 10,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },\n",
                 "                \"thresh_factor\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.05,\n",
                 "                        \"max\": 1.2,\n",
                 "                        \"min\": 0.6,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
@@ -934,329 +1373,402 @@
                 "                \"thresh_max\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.05,\n",
                 "                        \"max\": 1.0,\n",
                 "                        \"min\": 0.1,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"max_hole_w\": {\n",
+                "                \"max_hole_w_nuc\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 1,\n",
                 "                        \"max\": 40,\n",
                 "                        \"min\": 4,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },           \n",
-                "                \"small_obj_w\": {\n",
+                "                \"small_obj_w_nuc\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 1,\n",
                 "                        \"max\": 50,\n",
                 "                        \"min\": 1,\n",
                 "                        \"widget_type\": \"slider\"\n",
-                "                }\n",
+                "                },                           \n",
+                "                \"max_hole_w_cellmask\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"increment\": 2,\n",
+                "                        \"max\": 100,\n",
+                "                        \"min\": 20,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },           \n",
+                "                \"small_obj_w_cellmask\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"increment\": 1,\n",
+                "                        \"max\": 50,\n",
+                "                        \"min\": 1,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },        \n",
                 "        }\n",
                 "}\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"infer_nuclei\", _infer_nuclei, overwrite=True )\n",
+                "add_function_spec_to_widget_json(\"infer_cellmask\", _infer_cellmask, overwrite=True )\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "_median_filter_slice_by_slice =  {\n",
-                "                \"name\": \"Median Smoothing Slice by Slice\",\n",
-                "                \"python::module\": \"infer_subc.utils.img\",\n",
-                "                \"python::function\": \"median_filter_slice_by_slice\",\n",
-                "                \"parameters\": {\n",
-                "                    \"size\": {\n",
-                "                        \"widget_type\": \"slider\",\n",
-                "                        \"data_type\": \"int\",\n",
-                "                        \"min\": 1,\n",
-                "                        \"max\": 20,\n",
-                "                        \"increment\": 1\n",
-                "                    }\n",
-                "                }\n",
-                "            } \n",
-                "add_function_spec_to_widget_json(\"median_filter_slice_by_slice\",_median_filter_slice_by_slice)"
+                "\n",
+                "_raw_cellmask_MCZ =  {\n",
+                "        \"name\": \"define weighted aggregate cellmask signal (MCZ-cellprofiler)\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"raw_cellmask_MCZ\",\n",
+                "        \"parameters\": None\n",
+                "        }\n",
+                "\n",
+                "add_function_spec_to_widget_json(\"raw_cellmask_MCZ\", _raw_cellmask_MCZ, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "\n",
-                "_image_smoothing_gaussian_slice_by_slice = {\n",
-                "        \"name\": \"Gaussian Smoothing Slice by Slice\",\n",
-                "        \"python::module\": \"aicssegmentation.core.pre_processing_utils\",\n",
-                "        \"python::function\": \"image_smoothing_gaussian_slice_by_slice\",\n",
-                "        \"parameters\": {\n",
-                "            \"sigma\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.8,\n",
-                "                \"max\": 20,\n",
-                "                \"increment\": 0.2\n",
-                "            }\n",
-                "        }\n",
+                "_non_linear_cellmask_transform_MCZ =  {\n",
+                "        \"name\": \"non-linear filter of cellmask signal (MCZ-cellprofiler)\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"non_linear_cellmask_transform_MCZ\",\n",
+                "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "# json.dumps({\"image_smoothing_gaussian_slice_by_slice\": _image_smoothing_gaussian_slice_by_slice} )\n",
-                "add_function_spec_to_widget_json(\"image_smoothing_gaussian_slice_by_slice\",_image_smoothing_gaussian_slice_by_slice)        \n"
+                "add_function_spec_to_widget_json(\"non_linear_cellmask_transform_MCZ\", _non_linear_cellmask_transform_MCZ)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "# WARNING: not a good way to set to None\n",
-                "_apply_log_li_threshold = {\n",
-                "        \"name\": \"threshold log Li\",\n",
-                "        \"python::module\": \"infer_subc.utils.img\",\n",
-                "        \"python::function\": \"apply_log_li_threshold\",\n",
-                "        \"parameters\": {\n",
-                "            \"thresh_factor\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.3,\n",
-                "                \"max\": 1.1,\n",
-                "                \"increment\": 0.05\n",
-                "            },\n",
-                "            \"thresh_min\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.0,\n",
-                "                \"max\": 0.8,\n",
-                "                \"increment\": 0.01\n",
-                "            },\n",
-                "            \"thresh_max\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.3,\n",
-                "                \"max\": 1.0,\n",
-                "                \"increment\": 0.05\n",
-                "            },\n",
-                "        }\n",
+                "_masked_inverted_watershed =  {\n",
+                "        \"name\": \"watershed on inverted image and masked\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"masked_inverted_watershed\",\n",
+                "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "# json.dumps({\"apply_log_li_threshold\": _apply_log_li_threshold} )\n",
-                "add_function_spec_to_widget_json(\"apply_log_li_threshold\",_apply_log_li_threshold,overwrite=True)        \n"
+                "add_function_spec_to_widget_json(\"masked_inverted_watershed\", _masked_inverted_watershed)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "\n",
-                "    # NU_labels = label(nuclei_object)\n",
-                "\n",
-                "_label =  {\n",
-                "        \"name\": \"label objects\",\n",
-                "        \"python::module\": \"skimage.measure\",\n",
-                "        \"python::function\": \"label\",\n",
+                "_choose_max_label =  {\n",
+                "        \"name\": \"keep only the label with the maximum raw signa\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
+                "        \"python::function\": \"choose_max_label\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
-                "# json.dumps({\"label\":_label})\n",
-                "add_function_spec_to_widget_json(\"label\",_label)        \n"
+                "\n",
+                "add_function_spec_to_widget_json(\"choose_max_label\", _choose_max_label)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "#  nulei_object = apply_mask(nuclei_object, cellmask)\n",
-                "\n",
-                "_apply_mask=  {\n",
-                "        \"name\": \"apply mask\",\n",
-                "        \"python::module\": \"infer_subc.utils.img\",\n",
-                "        \"python::function\": \"apply_mask\",\n",
+                "_min_max_intensity_normalization =  {\n",
+                "        \"name\": \"Min Max Intesity Normalization\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
+                "        \"python::function\": \"min_max_intensity_normalization\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
-                "# json.dumps({\"apply_mask\":_apply_mask})\n",
-                "add_function_spec_to_widget_json(\"apply_mask\",_apply_mask)        \n"
+                "\n",
+                "add_function_spec_to_widget_json(\"min_max_intensity_normalization\", _min_max_intensity_normalization)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
-                "    # small_object_width = 45\n",
-                "    # nuclei_object = size_filter_2D(nuclei_object, \n",
-                "    #                                                             min_size= small_object_width**2, \n",
-                "    #                                                             connectivity=1)\n",
-                "\n",
-                "\n",
-                "_size_filter_2D = {\n",
-                "        \"name\": \"Size Filter 2D\",\n",
-                "        \"python::module\": \"infer_subc.utils.img\",\n",
-                "        \"python::function\": \"size_filter_2D\",\n",
+                "_masked_object_thresh =  {\n",
+                "        \"name\": \"Masked Object Threshold wrapper for widgets\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
+                "        \"python::function\": \"masked_object_thresh\",\n",
                 "        \"parameters\": {\n",
-                "            \"min_size\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"int\",\n",
-                "                \"min\": 0,\n",
-                "                \"max\": 500,\n",
-                "                \"increment\": 1\n",
-                "            }\n",
+                "                \"th_method\": {\n",
+                "                        \"data_type\": \"str\",\n",
+                "                        \"widget_type\": \"drop-down\",\n",
+                "                        \"options\": [\n",
+                "                        \"triangle\",\n",
+                "                        \"median\",\n",
+                "                        \"ave_tri_med\"\n",
+                "                        ]\n",
+                "                },\n",
+                "                \"cutoff_size\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"widget_type\": \"slider\",\n",
+                "                        \"min\": 0,\n",
+                "                        \"max\": 2000,\n",
+                "                        \"increment\": 50\n",
+                "                },\n",
+                "                \"th_adjust\": {\n",
+                "                        \"data_type\": \"float\",\n",
+                "                        \"widget_type\": \"slider\",\n",
+                "                        \"min\": 0,\n",
+                "                        \"max\": 2,\n",
+                "                        \"increment\": 0.02\n",
+                "                }\n",
                 "        }\n",
-                "    }\n",
-                "# json.dumps({  \"size_filter_2D\":  _size_filter_2D   })\n",
+                "}\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"size_filter_2D\",_size_filter_2D)        \n"
+                "add_function_spec_to_widget_json(\"masked_object_thresh\", _masked_object_thresh, overwrite=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "-------------------------------\n",
-                "## Write workflow .json\n",
-                "Now that we've added our function specs we can compose workflows."
+                "--------------------------\n",
+                "\n",
+                "# TEST `infer_cellmask` exported functions\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.constants import NUC_CH\n",
-                "\n",
+                "from infer_subc.organelles import fixed_infer_cellmask\n",
                 "\n",
-                "def make_infer_nuclei_dict():\n",
-                "    \"\"\"\n",
-                "    Procedure to infer nuclei from linearly unmixed input.\n",
+                "cellmask_mask =  fixed_infer_cellmask(img_2D) "
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Visualize  2\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# viewer = napari.Viewer()\n",
                 "\n",
-                "    Parameters\n",
-                "    ------------\n",
-                "    in_img: np.ndarray\n",
-                "        a 3d image containing all the channels\n",
+                "viewer.scale_bar.visible = True\n",
                 "\n",
-                "    cellmask: np.ndarray\n",
-                "        mask\n",
+                "viewer.add_labels(\n",
+                "    cellmask_mask,\n",
+                "    scale=scale,\n",
+                "    blending='additive'\n",
+                ")\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "\n",
-                "    Returns\n",
-                "    -------------\n",
-                "    nuclei_object\n",
-                "        mask defined extent of NU\n",
+                "from napari.utils.notebook_display import nbscreenshot\n",
                 "\n",
+                "# viewer.dims.ndisplay = 3\n",
+                "# viewer.camera.angles = (-30, 25, 120)\n",
+                "nbscreenshot(viewer, canvas_only=True)\n",
+                "viewer.close()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "-------------------------------\n",
+                "## Write workflow .json\n",
+                "Now that we've added our function specs we can compose workflows."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def make_infer_cellmask_step_by_step_dict():\n",
+                "    \"\"\"\n",
+                "    crete .json version of infer_cellmask\n",
                 "    \"\"\"\n",
                 "    step_name = []\n",
                 "    function_name = []\n",
                 "    category =[]\n",
                 "    parameter_values = []\n",
                 "    parent = []\n",
-                "   \n",
+                "\n",
                 "    ###################\n",
                 "    # EXTRACT\n",
                 "    ###################   \n",
+                "    # struct_img = _raw_cellmask_MCZ(in_img)\n",
                 "    step_name.append(\"1\")\n",
+                "    function_name.append(\"raw_cellmask_MCZ\")\n",
+                "    category.append(\"extraction\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(0)\n",
+                "\n",
+                "    step_name.append(\"2\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( dict(chan = NUC_CH) )\n",
                 "    parent.append(0)\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
-                "    ###################                         \n",
-                "    # nuclei = min_max_intensity_normalization(in_img[NUC_CH].copy() )\n",
-                "    step_name.append(\"2\")\n",
+                "    ###################\n",
+                "    #CELLMASK\n",
+                "    step_name.append(\"3\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(1)\n",
                 "\n",
-                "    # size = 4   \n",
-                "    # nuclei = median_filter_slice_by_slice( \n",
-                "    #                                                                 nuclei,\n",
-                "    #                                                                 size=size  )\n",
-                "    step_name.append(\"3\")\n",
+                "\n",
+                "    step_name.append(\"4\")\n",
                 "    function_name.append(\"median_filter_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parameter_values.append(dict(size = 15 ))\n",
+                "    parent.append(3)\n",
+                "\n",
+                "\n",
+                "    step_name.append(\"5\")\n",
+                "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
+                "    parent.append(4)\n",
+                "\n",
+                "    step_name.append(\"6\")\n",
+                "    function_name.append(\"non_linear_cellmask_transform_MCZ\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(5)\n",
+                "\n",
+                "    #NUC\n",
+                "    step_name.append(\"7\")\n",
+                "    function_name.append(\"min_max_intensity_normalization\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
                 "    parent.append(2)\n",
                 "\n",
-                "    # sigma = 1.34\n",
-                "    # truncate_range = 3.0\n",
-                "    # nuclei = image_smoothing_gaussian_slice_by_slice(  nuclei,\n",
-                "    #                                                                                             sigma=sigma,\n",
-                "    #                                                                                             truncate_range = truncate_range\n",
-                "    #                                                                                             )\n",
-                "    step_name.append(\"4\")\n",
+                "    step_name.append(\"8\")\n",
+                "    function_name.append(\"median_filter_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parent.append(7)\n",
+                "\n",
+                "    step_name.append(\"9\")\n",
                 "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict( sigma = 1.34 ))\n",
-                "    parent.append(3)\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
+                "    parent.append(8)\n",
                 "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    # threshold_factor = 0.9 \n",
-                "    # thresh_min = .1\n",
-                "    # thresh_max = 1.\n",
-                "    # nuclei_object = apply_log_li_threshold(nuclei, threshold_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "    step_name.append(\"5\")\n",
+                "    # CELLMASK\n",
+                "    step_name.append(\"10\")\n",
+                "    function_name.append(\"masked_object_thresh\")\n",
+                "    category.append(\"core\")\n",
+                "    parameter_values.append(dict( th_method=\"ave_tri_med\",\n",
+                "                                                            cutoff_size = 100,\n",
+                "                                                            th_adjust = 0.5))\n",
+                "    parent.append(6)\n",
+                "\n",
+                "\n",
+                "    # NUCLEI\n",
+                "    step_name.append(\"11\")\n",
                 "    function_name.append(\"apply_log_li_threshold\")\n",
                 "    category.append(\"core\")\n",
                 "    parameter_values.append(dict(thresh_factor = 0.9, \n",
                 "                                                            thresh_min = .1,\n",
                 "                                                            thresh_max = 1.))\n",
-                "    parent.append(4)\n",
-                "\n",
-                "\n",
-                "    # NU_labels = label(nuclei_object)\n",
-                "    step_name.append(\"6\")\n",
-                "    function_name.append(\"label\")\n",
-                "    category.append(\"core\")\n",
-                "    parameter_values.append(None)\n",
-                "    parent.append(5)\n",
+                "    parent.append(9)\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
-                "    # hole_width = 5  \n",
-                "    # nuclei_object = hole_filling(nuclei_object, hole_min=0, hole_max=hole_width**2, fill_2d=True)\n",
-                "    step_name.append(\"6\")\n",
+                "    # NUCLEI\n",
+                "    step_name.append(\"12\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
-                "    parent.append(5)\n",
+                "    parent.append(11)\n",
                 "\n",
-                "    # # EEEEEK I don't know how to compose where the mask comes from... \n",
-                "    # nuclei_object = apply_mask(nuclei_object, cellmask)\n",
+                "    step_name.append(\"13\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( min_size = 15**2  ))\n",
+                "    parent.append(12)\n",
                 "\n",
-                "    # small_object_width = 15\n",
-                "    # nuclei_object = size_filter_2D(nuclei_object, \n",
-                "    #                                                             min_size= small_object_width**2, \n",
-                "    #                                                             connectivity=1)\n",
-                "    step_name.append(\"7\")\n",
+                "    step_name.append(\"14\")\n",
+                "    function_name.append(\"label\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(13)\n",
+                "\n",
+                "    # CELLMASK\n",
+                "    step_name.append(\"15\")\n",
+                "    function_name.append(\"hole_filling\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
+                "    parent.append(10)\n",
+                "\n",
+                "    step_name.append(\"16\")\n",
                 "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
-                "    parent.append(6)\n",
+                "    parent.append(15)\n",
+                "\n",
+                "    step_name.append(\"17\")\n",
+                "    function_name.append(\"masked_inverted_watershed\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([ 5 , 14, 16])\n",
                 "\n",
+                "    ###################\n",
+                "    # POST- POST_PROCESSING\n",
+                "    ###################\n",
+                "    # keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "    step_name.append(\"18\")\n",
+                "    function_name.append(\"choose_max_label\")\n",
+                "    category.append(\"postpostprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([5, 17])\n",
+                "\n",
+                "    ##########################\n",
                 "    out_dict = dict()\n",
                 "    for i,stepn in enumerate(step_name):\n",
                 "        entry = dict(category=category[i],\n",
                 "                            function=function_name[i],\n",
                 "                            parameter_values=parameter_values[i],\n",
                 "                            parent=parent[i]\n",
                 "        )\n",
@@ -1269,186 +1781,195 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.utils.directories import Directories\n",
-                "import json\n",
-                "\n",
-                "def _write_workflow_json(wf_name, wf_dict):\n",
-                "\n",
-                "    # read all_functions.json into dict\n",
-                "    # if not wf_name.startswith(\"conf\"):\n",
-                "    #     wf_name = f\"conf_{wf_name}\"\n",
-                "    path = Directories.get_structure_config_dir() / f\"{wf_name}.json\"\n",
-                "\n",
-                "    # re-write file\n",
-                "    with open(path, \"w\") as file:\n",
-                "        json.dump(wf_dict, file, indent=4, sort_keys=False)\n",
-                "\n",
-                "    return path\n",
-                "\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "from infer_subc.organelles_config.helper import write_workflow_json\n",
                 "\n",
-                "infer_nuclei_dict = make_infer_nuclei_dict()\n",
+                "infer_cellmask_stepbystep_dict = make_infer_cellmask_step_by_step_dict()\n",
                 "\n",
-                "write_workflow_json(\"conf_2.2.nuclei_stepbystep\", infer_nuclei_dict)"
+                "write_workflow_json(\"conf_2.1.cellmask_stepbystep\", infer_cellmask_stepbystep_dict )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.constants import NUC_CH\n",
-                "\n",
-                "\n",
-                "def make_infer_nuclei_from_raw_dict():\n",
+                "def make_infer_cellmask_step_by_step_from_raw_dict():\n",
                 "    \"\"\"\n",
                 "    Procedure to infer nuclei from linearly unmixed input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
                 "\n",
-                "    cellmask: np.ndarray\n",
+                "    cellmask_mask: np.ndarray\n",
                 "        mask\n",
                 "\n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "\n",
                 "    \"\"\"\n",
                 "    step_name = []\n",
                 "    function_name = []\n",
                 "    category =[]\n",
                 "    parameter_values = []\n",
                 "    parent = []\n",
-                "   \n",
+                "\n",
                 "    ###################\n",
                 "    # EXTRACT\n",
                 "    ###################   \n",
-                "\n",
                 "    step_name.append(\"1\")\n",
                 "    function_name.append(\"fixed_get_optimal_Z_img\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(0)\n",
                 "\n",
-                "\n",
+                "    # CELLMASK\n",
                 "    step_name.append(\"2\")\n",
-                "    function_name.append(\"fixed_infer_soma\")\n",
+                "    function_name.append(\"raw_cellmask_MCZ\")\n",
                 "    category.append(\"extraction\")\n",
-                "    parameter_values.append( None )\n",
+                "    parameter_values.append(None)\n",
                 "    parent.append(1)\n",
                 "\n",
+                "    # NUC\n",
                 "    step_name.append(\"3\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( dict(chan = NUC_CH) )\n",
                 "    parent.append(1)\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
-                "    ###################                         \n",
-                "    # nuclei = min_max_intensity_normalization(in_img[NUC_CH].copy() )\n",
+                "    ###################\n",
+                "    # CELLMASK\n",
                 "    step_name.append(\"4\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
-                "    parent.append(3)\n",
+                "    parent.append(2)\n",
                 "\n",
-                "    # size = 4   \n",
-                "    # nuclei = median_filter_slice_by_slice( \n",
-                "    #                                                                 nuclei,\n",
-                "    #                                                                 size=size  )\n",
                 "    step_name.append(\"5\")\n",
                 "    function_name.append(\"median_filter_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parameter_values.append(dict(size = 15 ))\n",
                 "    parent.append(4)\n",
                 "\n",
-                "    # sigma = 1.34\n",
-                "    # truncate_range = 3.0\n",
-                "    # nuclei = image_smoothing_gaussian_slice_by_slice(  nuclei,\n",
-                "    #                                                                                             sigma=sigma,\n",
-                "    #                                                                                             truncate_range = truncate_range\n",
-                "    #                                                                                             )\n",
                 "    step_name.append(\"6\")\n",
                 "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict( sigma = 1.34 ))\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
                 "    parent.append(5)\n",
                 "\n",
+                "    step_name.append(\"7\")\n",
+                "    function_name.append(\"non_linear_cellmask_transform_MCZ\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(6)\n",
+                "\n",
+                "    #NUC\n",
+                "    step_name.append(\"8\")\n",
+                "    function_name.append(\"min_max_intensity_normalization\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(3)\n",
+                "\n",
+                "    step_name.append(\"9\")\n",
+                "    function_name.append(\"median_filter_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parent.append(8)\n",
+                "\n",
+                "    step_name.append(\"10\")\n",
+                "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
+                "    parent.append(9)\n",
+                "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    # threshold_factor = 0.9 \n",
-                "    # thresh_min = .1\n",
-                "    # thresh_max = 1.\n",
-                "    # nuclei_object = apply_log_li_threshold(nuclei, threshold_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "    step_name.append(\"7\")\n",
+                "    # CELLMASK\n",
+                "    step_name.append(\"11\")\n",
+                "    function_name.append(\"masked_object_thresh\")\n",
+                "    category.append(\"core\")\n",
+                "    parameter_values.append(dict( th_method=\"ave_tri_med\",\n",
+                "                                                            cutoff_size = 100,\n",
+                "                                                            th_adjust = 0.5))\n",
+                "    parent.append(7)\n",
+                "\n",
+                "    # NUC\n",
+                "    step_name.append(\"12\")\n",
                 "    function_name.append(\"apply_log_li_threshold\")\n",
                 "    category.append(\"core\")\n",
                 "    parameter_values.append(dict(thresh_factor = 0.9, \n",
                 "                                                            thresh_min = .1,\n",
                 "                                                            thresh_max = 1.))\n",
-                "    parent.append(6)\n",
-                "\n",
-                "\n",
-                "    # NU_labels = label(nuclei_object)\n",
-                "    step_name.append(\"8\")\n",
-                "    function_name.append(\"label\")\n",
-                "    category.append(\"core\")\n",
-                "    parameter_values.append(None)\n",
-                "    parent.append(7)\n",
-                "\n",
+                "    parent.append(10)\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
-                "    # hole_width = 5  \n",
-                "    # nuclei_object = hole_filling(nuclei_object, hole_min=0, hole_max=hole_width**2, fill_2d=True)\n",
-                "    step_name.append(\"9\")\n",
+                "    # nUC\n",
+                "    step_name.append(\"13\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
-                "    parent.append(8)\n",
+                "    parent.append(12)\n",
                 "\n",
-                "    step_name.append(\"10\")\n",
-                "    function_name.append(\"apply_mask\")\n",
+                "    step_name.append(\"14\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( min_size = 15**2  ))\n",
+                "    parent.append(13)\n",
+                "\n",
+                "    step_name.append(\"15\")\n",
+                "    function_name.append(\"label\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
-                "    parent.append([9,2])\n",
+                "    parent.append(14)\n",
                 "\n",
                 "\n",
-                "    # small_object_width = 15\n",
-                "    # nuclei_object = size_filter_2D(nuclei_object, \n",
-                "    #                                                             min_size= small_object_width**2, \n",
-                "    #                                                             connectivity=1)\n",
-                "    step_name.append(\"11\")\n",
+                "    # CELLMASK\n",
+                "    step_name.append(\"16\")\n",
+                "    function_name.append(\"hole_filling\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
+                "    parent.append(11)\n",
+                "\n",
+                "    step_name.append(\"17\")\n",
                 "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
-                "    parent.append(10)\n",
+                "    parent.append(16)\n",
                 "\n",
+                "    step_name.append(\"18\")\n",
+                "    function_name.append(\"masked_inverted_watershed\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([  7 , 15,17 ])\n",
+                "\n",
+                "    ###################\n",
+                "    # POST- POST_PROCESSING\n",
+                "    ###################\n",
+                "    # keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "    step_name.append(\"19\")\n",
+                "    function_name.append(\"choose_max_label\")\n",
+                "    category.append(\"postpostprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([6,18])\n",
+                "\n",
+                "    ##########################\n",
                 "    out_dict = dict()\n",
                 "    for i,stepn in enumerate(step_name):\n",
                 "        entry = dict(category=category[i],\n",
                 "                            function=function_name[i],\n",
                 "                            parameter_values=parameter_values[i],\n",
                 "                            parent=parent[i]\n",
                 "        )\n",
@@ -1461,59 +1982,34 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.organelles_config.helper import write_workflow_json\n",
                 "\n",
-                "infer_nuclei_dict = make_infer_nuclei_from_raw_dict()\n",
+                "infer_cellmask_stepbystep_from_raw_dict = make_infer_cellmask_step_by_step_from_raw_dict()\n",
                 "\n",
-                "write_workflow_json(\"conf_1.2.nuclei_stepbystep_from_raw\", infer_nuclei_dict)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
-                "\n",
-                "_infer_nuclei =  {\n",
-                "        \"name\": \"infer infer_nuclei\",\n",
-                "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_nuclei\",\n",
-                "        \"parameters\": None\n",
-                "        }\n",
-                "\n",
-                "add_function_spec_to_widget_json(\"infer_nuclei\",_infer_nuclei)"
+                "write_workflow_json(\"conf_1.1.cellmask_stepbystep_from_raw\", infer_cellmask_stepbystep_from_raw_dict)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-------------\n",
                 "## SUMMARY\n",
                 "\n",
-                "The above details how the nuclei object is inferred.  \n",
+                "The above explains the overall framework.  \n",
                 "\n",
-                "### NEXT: INFER CYTOSOL\n",
+                "### NEXT: INFER NUCLEI\n",
                 "\n",
-                "proceed to [03_infer_cytosol.ipynb](./03_infer_cytosol.ipynb)\n"
+                "proceed to [02_infer_nuclei.ipynb](./02_infer_nuclei.ipynb)\n"
             ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "infer-subc",
             "language": "python",
             "name": "python3"
@@ -1524,16 +2020,17 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.15 (main, Nov 24 2022, 14:39:17) [MSC v.1916 64 bit (AMD64)]"
         },
+        "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
             }
         }
     },
     "nbformat": 4,
```

### Comparing `infer-subc-0.0.6b0/notebooks/04_infer_neurites_soma_from-cellmask.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/02_infer_soma_3D.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986361425952269%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(6, '>> #### Because we do NOT have a direct cell membrane / "*

 * *            'cellmask signal, this segmentation is trickiest and potentially most problematic part '*

 * *            'of the overall sub-cellular component inference pipeline. We are using the nuclei of '*

 * *            'the cell with the brightest total fluorescence (all channels) to identify a single '*

 * *            'cellmask for all downstream steps. The Soma (via the Cytosol mask) will be used to '*

 * *            'd […]*

```diff
@@ -7,24 +7,24 @@
             "source": [
                 "# Infer ***cellmask*** -  1\ufe0f\u20e3 \n",
                 "\n",
                 "> WARNING: (\ud83d\udea8\ud83d\udea8\ud83d\udea8\ud83d\udea8 Steps 3-9 depend on establishing a good solution here.)\n",
                 "\n",
                 "\n",
                 ">> WARNING:  THIS DOES NOT WORK WELL - lacking fluorescent marker\n",
-                ">> #### Because we do NOT have a direct cell membrane / cellmask signal, this segmentation is trickiest and potentially most problematic part of the overall sub-cellular component inference pipeline. We are using the nuclei of the cell with the brightest total fluorescence (all channels) to identify a single cellmask for all downstream steps. The Cellmask (via the Cytosol mask) will be used to define ALL subsequent sub-cellular Objects.\n",
+                ">> #### Because we do NOT have a direct cell membrane / cellmask signal, this segmentation is trickiest and potentially most problematic part of the overall sub-cellular component inference pipeline. We are using the nuclei of the cell with the brightest total fluorescence (all channels) to identify a single cellmask for all downstream steps. The Soma (via the Cytosol mask) will be used to define ALL subsequent sub-cellular Objects.\n",
                 "\n",
                 "--------------\n",
                 "\n",
                 "## OBJECTIVE: \n",
                 "### \u2705 Infer sub-cellular component #2: ***cellmask***/cell body in order to understand interactome \n",
                 "\n",
                 "Infer a segmentation of the cell body -- the ***cellmask*** -- in order to measure its shape, position, and size.\n",
                 "\n",
-                "CONTEXT: \"Cellmask\" is used here becuase subsequent experiments will contain neurons who's cellmask has a similar shape to an iPS cell body.\n",
+                "CONTEXT: \"Soma\" is used here becuase subsequent experiments will contain neurons who's cellmask has a similar shape to an iPS cell body.\n",
                 "\n",
                 "## OVERVIEW: \n",
                 "\n",
                 "This method is used in the case where there is no cell fill/membrane marker.\n",
                 "\n",
                 "We will infer the cellmask from a combination of fluorescent signals. The current selection includes the lysosomes, ER, and Golgi (e.g., 'Ch = 1, 3, 5) which have some intracellular fluorescence - likely from off target marker localization to the entire cellmask and/or the cell membrane. There are two other channels, the residual channel from linear unmixing (e.g. `ch = 7`) and the lipid droplet channel (e.g., `ch = 6`) that could more lead to more unbiased selection of the entire cellmask. However, the drawback of these two markers is that they are present in every cell which makes downstream cell selection more challenging. To expand on this, we will be collecting per cell measurements, so each cell area has to be segmented individually even if there are two appropriately labeled cells within one field of view. "
             ]
@@ -132,14 +132,15 @@
                 "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
                 "# build the datapath\n",
                 "# all the imaging data goes here.\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
                 "\n",
                 "# linearly unmixed \".czi\" files are here\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
                 "# get the list of all files\n",
@@ -152,15 +153,15 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "c:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:105: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "/opt/anaconda3/envs/napariNEW/lib/python3.9/site-packages/ome_types/_convenience.py:106: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
                 "# isolate image as an ndarray and metadata as a dictionary\n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
@@ -196,15 +197,15 @@
                 "- mask object segmentation at bottom\n",
                 "\n",
                 "POST-PROCESSING\n",
                 "  - fill holes\n",
                 "  - remove small objects\n",
                 "\n",
                 "OUTPUT \u27a1\ufe0f \n",
-                "- mask of CELLMASK\n",
+                "- mask of SOMA\n",
                 "\n",
                 "\n",
                 "> #### Note: this pipeline will eventually include a selection step to identify the cellmask that are properly labeled with all fluorescent markers. This could be one single cell per image, or more if applicable data is available."
             ]
         },
         {
             "attachments": {},
@@ -223,16 +224,16 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(17, 704, 704)\n",
-                        "(17, 704, 704)\n"
+                        "(16, 768, 768)\n",
+                        "(16, 768, 768)\n"
                     ]
                 }
             ],
             "source": [
                 "###################\n",
                 "# INPUT\n",
                 "###################\n",
@@ -259,15 +260,15 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'img_data' at 0x25e5031c3a0>"
+                            "<Image layer 'img_data' at 0x1081fb490>"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -283,15 +284,15 @@
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'struct_img_raw' at 0x25e527b0430>"
+                            "<Image layer 'struct_img_raw' at 0x1686a6970>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -314,34 +315,34 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_struct_img_raw' at 0x25e50a57340>"
+                            "<Image layer '_struct_img_raw' at 0x16fafd0d0>"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "def _raw_cellmask_MCZ(img_in):\n",
+                "def _raw_soma_MCZ(img_in):\n",
                 "    \"\"\" define cellmask image\n",
                 "    \"\"\"\n",
-                "    CELLMASK_W = (6.,1.,2.)\n",
-                "    CELLMASK_CH = (LYSO_CH,ER_CH,GOLGI_CH)\n",
+                "    SOMA_W = (6.,1.,2.)\n",
+                "    SOMA_CH = (LYSO_CH,ER_CH,GOLGI_CH)\n",
                 "    img_out = np.zeros_like(img_in[0]).astype(np.double)\n",
-                "    for w,ch in zip(CELLMASK_W,CELLMASK_CH):\n",
+                "    for w,ch in zip(SOMA_W,SOMA_CH):\n",
                 "        img_out += w*img_in[ch]\n",
                 "    return img_out\n",
                 "\n",
-                "_struct_img_raw = _raw_cellmask_MCZ(img_data)\n",
+                "_struct_img_raw = _raw_soma_MCZ(img_data)\n",
                 "\n",
                 "viewer.add_image(\n",
                 "    _struct_img_raw,\n",
                 "    scale=scale\n",
                 ")\n"
             ]
         },
@@ -351,15 +352,15 @@
             "metadata": {},
             "source": [
                 "## PRE-PROCESSING (prototype)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
@@ -369,138 +370,138 @@
             "source": [
                 "\n",
                 "###################\n",
                 "# PRE_PROCESSING\n",
                 "###################\n",
                 "\n",
                 "################# smoothing\n",
-                "cellmask_norm = min_max_intensity_normalization(struct_img_raw)\n",
+                "soma_norm = min_max_intensity_normalization(struct_img_raw)\n",
                 "\n",
                 "med_filter_size = 15\n",
-                "cellmask_med = median_filter_slice_by_slice(cellmask_norm, \n",
+                "soma_med = median_filter_slice_by_slice(soma_norm, \n",
                 "                                        size=med_filter_size)\n",
                 "\n",
                 "## Need to adjust image_smoothing_gaussian_slice_by_slice in pre_processing_utils.py to integrate the mode\n",
                 "\n",
                 "gaussian_smoothing_sigma = 1.34\n",
                 "gaussian_smoothing_truncate_range = 3.0\n",
-                "cellmask_guas = ndi.gaussian_filter(cellmask_med,\n",
+                "soma_guas = ndi.gaussian_filter(soma_med,\n",
                 "                                sigma=gaussian_smoothing_sigma,\n",
                 "                                mode=\"nearest\", \n",
                 "                                truncate=gaussian_smoothing_truncate_range)\n",
                 "\n",
                 "\n",
                 "################# NON-Linear aggregation\n",
-                "cellmask_log, d = log_transform(cellmask_guas) \n",
-                "cellmask_log_norm = intensity_normalization(cellmask_log, scaling_param=[0])\n",
+                "soma_log, d = log_transform(soma_guas) \n",
+                "soma_log_norm = intensity_normalization(soma_log, scaling_param=[0])\n",
                 "\n",
-                "# cellmask_edges = filters.difference_of_gaussians(cellmask_log_norm, 2)\n",
+                "# soma_edges = filters.difference_of_gaussians(soma_log_norm, 2)\n",
                 "\n",
-                "# composite_cellmask = intensity_normalization(cellmask_edges, scaling_param=[0]) + cellmask_log_norm "
+                "# composite_soma = intensity_normalization(soma_edges, scaling_param=[0]) + soma_log_norm "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'composite_cellmask' at 0x25e437c8bb0>"
+                            "<Image layer 'soma_log_norm' at 0x1701565b0>"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    cellmask_med,\n",
+                "    soma_med,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    cellmask_guas,\n",
+                "    soma_guas,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    cellmask_log_norm,\n",
+                "    soma_log_norm,\n",
                 "    scale=scale\n",
                 ")\n",
                 "# viewer.add_image(\n",
-                "#     cellmask_edges,\n",
+                "#     soma_edges,\n",
                 "#     scale=scale\n",
                 "# )\n",
                 "# viewer.add_image(\n",
-                "#     composite_cellmask,\n",
+                "#     composite_soma,\n",
                 "#     scale=scale\n",
                 "# )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_log_cellmask' at 0x25e437e2d90>"
+                            "<Image layer '_log_soma' at 0x170345e80>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "def _non_linear_cellmask_transform(in_img):\n",
+                "def _non_linear_soma_transform_MCZ(in_img):\n",
                 "    \"\"\" non-linear distortion to fill out cellmask\n",
                 "    log + edge of smoothed composite\n",
                 "    \"\"\"\n",
                 "    # non-Linear processing\n",
                 "    log_img, d = log_transform(in_img.copy()) \n",
                 "    return intensity_normalization(log_img,scaling_param=[0])\n",
                 "    # return intensity_normalization(filters.difference_of_gaussians(log_img, 2),scaling_param=[0])  + log_img\n",
                 "\n",
-                "_log_cellmask = _non_linear_cellmask_transform(cellmask_guas)\n",
+                "_log_soma = _non_linear_soma_transform_MCZ(soma_guas)\n",
                 "\n",
                 "viewer.add_image(\n",
-                "    _log_cellmask,\n",
+                "    _log_soma,\n",
                 "    scale=scale\n",
                 ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Eventually this will be replaced by calling the un-name mangled version of the infer nuclei code that will be in infer-subc.organelles.</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "################# part 2 Nuclei pre-process\n",
                 "def _infer_nuclei_3D( in_img: np.ndarray,\n",
                 "                       median_sz: int, \n",
                 "                       gauss_sig: float,\n",
@@ -514,15 +515,15 @@
                 "    \"\"\"\n",
                 "    Procedure to infer 3D nuclei segmentation from multichannel z-stack input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
-                "    cellmask_mask: Optional[np.ndarray] = None\n",
+                "    soma_mask: Optional[np.ndarray] = None\n",
                 "        mask\n",
                 "    median_sz: int\n",
                 "        width of median filter for signal\n",
                 "    gauss_sig: float\n",
                 "        sigma for gaussian smoothing of  signal\n",
                 "    thresh_factor: float\n",
                 "        adjustment factor for log Li threholding\n",
@@ -588,26 +589,26 @@
                 "    \"\"\"\n",
                 "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
-                "    cellmask_mask: np.ndarray\n",
+                "    soma_mask: np.ndarray\n",
                 "        mask\n",
                 " \n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "    \n",
                 "    \"\"\"\n",
                 "\n",
                 "    nuc_ch = NUC_CH\n",
-                "    median_sz = 4     \n",
+                "    median_sz = 4   \n",
                 "    gauss_sig = 1.34\n",
                 "    threshold_factor = 0.9\n",
                 "    thresh_min = 0.1\n",
                 "    thresh_max = 1.0\n",
                 "    max_hole_w = 5\n",
                 "    small_obj_w = 15\n",
                 "    sz_filter_method = \"3D\"\n",
@@ -633,15 +634,15 @@
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "def _masked_object_thresh(\n",
                 "    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float\n",
                 ") -> np.ndarray:\n",
@@ -684,49 +685,49 @@
             "metadata": {},
             "source": [
                 "## CORE PROCESSING"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "###################\n",
                 "# CORE_PROCESSING\n",
                 "###################\n",
                 "low_level_min_size =  50\n",
                 "\n",
                 "# ################# part 1\n",
-                "cellmask_binary = _masked_object_thresh(cellmask_log_norm, \n",
+                "soma_binary = _masked_object_thresh(soma_log_norm, \n",
                 "                           th_method='ave', \n",
                 "                           cutoff_size=low_level_min_size, \n",
                 "                           th_adjust= 0.15)                                           "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'cellmask_binary' at 0x25e438999d0>"
+                            "<Image layer 'soma_binary' at 0x170345100>"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    cellmask_binary,\n",
+                "    soma_binary,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -735,30 +736,30 @@
                 "## POST-PROCESSING\n",
                 "\n",
                 "<code style=\"background:yellow;color:black\">Watershed (with or without the nuclei as a marker) does not work well here to get an instance segmentation</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
                 "###################\n",
                 "# POST_PROCESSING\n",
                 "###################\n",
                 "hole_width = 100\n",
-                "removed_holes = hole_filling(cellmask_binary, \n",
+                "removed_holes = hole_filling(soma_binary, \n",
                 "                            hole_min=0, \n",
                 "                            hole_max=hole_width**2,\n",
                 "                            fill_2d = True) \n",
                 "\n",
                 "\n",
                 "small_object_width = 45\n",
-                "cleaned_img = size_filter_2D(removed_holes, \n",
+                "cleaned_img = size_filter_linear_size(removed_holes, \n",
                 "                             min_size= small_object_width**3, \n",
                 "                             connectivity=1)\n",
                 "\n",
                 "\n",
                 "watershed_mask = cleaned_img \n",
                 "inverted_img = 1. - cleaned_img\n",
                 "\n",
@@ -768,24 +769,24 @@
                 "            connectivity= 3, # np.ones((1,3,3), bool),\n",
                 "            mask=watershed_mask,\n",
                 "            )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'labels_out' at 0x25e52d71a60>"
+                            "<Labels layer 'labels_out' at 0x170f63460>"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    removed_holes,\n",
@@ -811,24 +812,24 @@
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer '_labels_out [1]' at 0x25e43b8f550>"
+                            "<Labels layer '_labels_out' at 0x17114a700>"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def _masked_inverted_watershed(img_in, markers, mask):\n",
                 "    \"\"\"wrapper for watershed on inverted image and masked\n",
@@ -861,84 +862,84 @@
                 "<code style=\"background:yellow;color:black\">This should eventually be altered to maintain all cells that have the correct number of organelle markers</code>\n",
                 "\n",
                 "What is we used the nuclei (or an expanded nuclei) to select the cells with the most signal, then after selecting the nuclei with signal, use those as the watershed marker - I think it may resolve some conflicts, but not all"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'cellmask_out' at 0x25e52975190>"
+                            "<Image layer 'soma_out' at 0x171659340>"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "###################\n",
                 "# POST- POST_PROCESSING\n",
                 "###################\n",
-                "# keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "# keep the \"SOMA\" label which contains the highest total signal\n",
                 "all_labels = np.unique(labels_out)[1:]\n",
                 "\n",
-                "total_signal = [cellmask_norm[labels_out == label].sum() for label in all_labels]\n",
+                "total_signal = [soma_norm[labels_out == label].sum() for label in all_labels]\n",
                 "keep_label = all_labels[np.argmax(total_signal)]\n",
                 "keep_label\n",
                 "\n",
-                "cellmask_out = np.zeros_like(labels_out)\n",
-                "cellmask_out[labels_out==keep_label] = 1\n",
+                "soma_out = np.zeros_like(labels_out)\n",
+                "soma_out[labels_out==keep_label] = 1\n",
                 "\n",
                 "viewer.add_image(\n",
-                "    cellmask_out,\n",
+                "    soma_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_cellmask_out' at 0x25e43926160>"
+                            "<Image layer '_soma_out' at 0x171659b80>"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def _choose_max_label(raw_signal: np.ndarray, labels_in: np.ndarray):\n",
                 "    \"\"\" keep only the label with the maximum raw signal\n",
                 "\n",
                 "    \"\"\"\n",
                 "\n",
                 "    all_labels = np.unique(labels_in)[1:]\n",
                 "\n",
                 "    total_signal = [raw_signal[labels_in == label].sum() for label in all_labels]\n",
-                "    # combine NU and \"labels\" to make a CELLMASK\n",
+                "    # combine NU and \"labels\" to make a SOMA\n",
                 "    keep_label = all_labels[np.argmax(total_signal)]\n",
                 "\n",
                 "    labels_max = np.zeros_like(labels_in)\n",
                 "    labels_max[labels_in==keep_label] = 1\n",
                 "    return labels_max\n",
                 "\n",
-                "_cellmask_out = _choose_max_label(cellmask_norm,labels_out)\n",
+                "_soma_out = _choose_max_label(soma_norm,labels_out)\n",
                 "\n",
                 "viewer.add_image(\n",
-                "    _cellmask_out,\n",
+                "    _soma_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -949,80 +950,80 @@
                 "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## DEFINE parameterized  `_infer_cellmask` function\n",
+                "## DEFINE parameterized  `_infer_cellmask_fromaggr` function\n",
                 "\n",
-                "A function to infer_cellmask from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
+                "A function to infer_cellmask_fromaggr from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
                 "-  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
-                "# 1. infer_cellmask\n",
+                "# 1. infer_cellmask_fromaggr\n",
                 "##########################\n",
                 "\n",
-                "def _infer_cellmask_3D(in_img: np.ndarray,\n",
+                "def _infer_cellmask_fromaggr_3D(in_img: np.ndarray,\n",
                 "    nuclei_labels: np.ndarray,\n",
-                "    median_sz_cellmask: int,\n",
-                "    gauss_sig_cellmask: float,\n",
+                "    median_sz_soma: int,\n",
+                "    gauss_sig_soma: float,\n",
                 "    gauss_truc_rang: float,\n",
                 "    mo_method: str,\n",
                 "    mo_adjust: float,\n",
                 "    mo_cutoff_size: int,\n",
-                "    max_hole_w_cellmask: int,\n",
-                "    small_obj_w_cellmask: int\n",
+                "    max_hole_w_soma: int,\n",
+                "    small_obj_w_soma: int\n",
                 ") -> np.ndarray:\n",
                 "    \"\"\"\n",
                 "    Procedure to infer cellmask from linearly unmixed input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: \n",
                 "        a 3d image containing all the channels\n",
                 "    nuclei_labels:\n",
                 "        a 3d mask of nuclei\n",
-                "    median_sz_cellmask: \n",
-                "        width of median filter for _cellmask_ signal\n",
-                "    gauss_sig_cellmask: \n",
-                "        sigma for gaussian smoothing of _cellmask_ signal\n",
+                "    median_sz_soma: \n",
+                "        width of median filter for _soma_ signal\n",
+                "    gauss_sig_soma: \n",
+                "        sigma for gaussian smoothing of _soma_ signal\n",
                 "    gauss_truc_rang:\n",
                 "        cutoff value for gaussian\n",
                 "    mo_method: \n",
                 "         which method to use for calculating global threshold. Options include:\n",
                 "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
                 "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
                 "    mo_adjust: \n",
                 "        Masked Object threshold `local_adjust`\n",
                 "    mo_cutoff_size: \n",
                 "        Masked Object threshold `size_min`\n",
-                "    max_hole_w_cellmask: \n",
+                "    max_hole_w_soma: \n",
                 "        hole filling cutoff for cellmask signal post-processing\n",
-                "    small_obj_w_cellmask: \n",
+                "    small_obj_w_soma: \n",
                 "        minimu object size cutoff for cellmask signal post-processing\n",
                 "\n",
                 "    Returns\n",
                 "    -------------\n",
-                "    cellmask_mask:\n",
+                "    soma_mask:\n",
                 "        a logical/labels object defining boundaries of cellmask\n",
                 "\n",
                 "    \"\"\"\n",
                 "\n",
                 "    ###################\n",
                 "    # EXTRACT\n",
                 "    ###################\n",
-                "    struct_img = _raw_cellmask_MCZ(in_img)\n",
+                "    struct_img = _raw_soma_MCZ(in_img)\n",
                 "    viewer.add_image(\n",
                 "    struct_img,\n",
                 "    scale=scale,\n",
                 "    name=1\n",
                 "    )\n",
                 "\n",
                 "\n",
@@ -1038,35 +1039,35 @@
                 "    )\n",
                 "\n",
                 "    # make a copy for post-post processing\n",
                 "    scaled_signal = struct_img.copy()\n",
                 "\n",
                 "    # Linear-ish processing\n",
                 "    struct_img = median_filter_slice_by_slice(struct_img, \n",
-                "                                              size=median_sz_cellmask)\n",
+                "                                              size=median_sz_soma)\n",
                 "    viewer.add_image(\n",
                 "    struct_img,\n",
                 "    scale=scale,\n",
                 "    name=3\n",
                 "    )\n",
                 "\n",
                 "    struct_img = ndi.gaussian_filter(struct_img,\n",
-                "                                     sigma=gauss_sig_cellmask,\n",
+                "                                     sigma=gauss_sig_soma,\n",
                 "                                     mode=\"nearest\",\n",
                 "                                     truncate=gauss_truc_rang)\n",
                 "    viewer.add_image(\n",
                 "    struct_img,\n",
                 "    scale=scale,\n",
                 "    name=4\n",
                 "    )\n",
                 "\n",
                 "\n",
                 "    # struct_img_non_lin, d = log_transform(struct_img)\n",
                 "    # struct_img_non_lin = intensity_normalization(struct_img_non_lin, scaling_param=[0])\n",
-                "    struct_img_non_lin = _non_linear_cellmask_transform(struct_img)\n",
+                "    struct_img_non_lin = _non_linear_soma_transform_MCZ(struct_img)\n",
                 "    viewer.add_image(\n",
                 "    struct_img_non_lin,\n",
                 "    scale=scale,\n",
                 "    name=5\n",
                 "    )\n",
                 "   \n",
                 "    ###################\n",
@@ -1083,24 +1084,24 @@
                 "    )\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
                 "    struct_obj = hole_filling(struct_obj, \n",
                 "                              hole_min =0 , \n",
-                "                              hole_max=max_hole_w_cellmask**2, \n",
+                "                              hole_max=max_hole_w_soma**2, \n",
                 "                              fill_2d = True) \n",
                 "    viewer.add_image(\n",
                 "    struct_obj,\n",
                 "    scale=scale,\n",
                 "    name=7\n",
                 "    )\n",
                 "\n",
-                "    struct_obj = size_filter_2D(struct_obj, \n",
-                "                                min_size= small_obj_w_cellmask**3, \n",
+                "    struct_obj = size_filter_linear_size(struct_obj, \n",
+                "                                min_size= small_obj_w_soma**3, \n",
                 "                                connectivity=1)\n",
                 "    viewer.add_image(\n",
                 "    struct_obj,\n",
                 "    scale=scale,\n",
                 "    name=8\n",
                 "    )\n",
                 "\n",
@@ -1110,118 +1111,118 @@
                 "    scale=scale,\n",
                 "    name=9\n",
                 "    )\n",
                 "\n",
                 "    ###################\n",
                 "    # POST- POST_PROCESSING\n",
                 "    ###################\n",
-                "    # keep the \"CELLMASK\" label which contains the highest total signal\n",
-                "    cellmask_out = _choose_max_label(struct_img, labels_out)\n",
+                "    # keep the \"SOMA\" label which contains the highest total signal\n",
+                "    soma_out = _choose_max_label(struct_img, labels_out)\n",
                 "\n",
-                "    return cellmask_out\n",
+                "    return soma_out\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## DEFINE `_fixed_infer_cellmask` function\n",
+                "## DEFINE `_fixed_infer_cellmask_fromaggr` function\n",
                 "\n",
                 "Based on the _prototyping_ above define the function to infer cellmask. with a *fixed* set of parameters for each step in the procedure.  That is they are all \"hard coded\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
-                "# 1. fixed_infer_cellmask\n",
+                "# 1. fixed_infer_cellmask_fromaggr\n",
                 "##########################\n",
                 "\n",
                 "\n",
-                "def _fixed_infer_cellmask_3D(in_img: np.ndarray, nuclei_labels: np.ndarray) -> np.ndarray:\n",
+                "def _fixed_infer_cellmask_fromaggr_3D(in_img: np.ndarray, nuclei_labels: np.ndarray) -> np.ndarray:\n",
                 "    \"\"\"\n",
                 "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: \n",
                 "        a 3d image containing all the channels\n",
                 "    nuclei_object:\n",
                 "        a 3d mask of nuclei\n",
                 "\n",
                 "    Returns\n",
                 "    -------------\n",
-                "    cellmask_mask:\n",
+                "    soma_mask:\n",
                 "        a logical/labels object defining boundaries of cellmask\n",
                 "    \"\"\"\n",
                 "    \n",
                 "\n",
                 "    ###################\n",
                 "    # PARAMETERS\n",
                 "    ###################   \n",
-                "    median_sz_cellmask = 15\n",
-                "    gauss_sig_cellmask = 1.34\n",
+                "    median_sz_soma = 15\n",
+                "    gauss_sig_soma = 1.34\n",
                 "    gauss_truc_rang = 3.0\n",
                 "    mo_method = \"ave\"\n",
                 "    mo_adjust = 0.15\n",
                 "    mo_cutoff_size = 50\n",
-                "    max_hole_w_cellmask = 100\n",
-                "    small_obj_w_cellmask = 45\n",
+                "    max_hole_w_soma = 100\n",
+                "    small_obj_w_soma = 45\n",
                 "\n",
-                "    cellmask_out = _infer_cellmask_3D(in_img,\n",
+                "    soma_out = _infer_cellmask_fromaggr_3D(in_img,\n",
                 "                              nuclei_labels,\n",
-                "                              median_sz_cellmask,\n",
-                "                              gauss_sig_cellmask,\n",
+                "                              median_sz_soma,\n",
+                "                              gauss_sig_soma,\n",
                 "                              gauss_truc_rang,\n",
                 "                              mo_method,\n",
                 "                              mo_adjust,\n",
                 "                              mo_cutoff_size,\n",
-                "                              max_hole_w_cellmask,\n",
-                "                              small_obj_w_cellmask) \n",
+                "                              max_hole_w_soma,\n",
+                "                              small_obj_w_soma) \n",
                 "\n",
-                "    return cellmask_out\n",
+                "    return soma_out\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
-                "SO_label =  _fixed_infer_cellmask_3D(img_data, NU_labels) "
+                "SO_label =  _fixed_infer_cellmask_fromaggr_3D(img_data, NU_labels) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'SO_label [1]' at 0x25ea42fd970>"
+                            "<Image layer 'SO_label' at 0x171ace910>"
                         ]
                     },
-                    "execution_count": 39,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    SO_label,\n",
@@ -1231,92 +1232,92 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "---------------------\n",
-                "# TEST `_infer_cellmask`  function defined above\n",
+                "# TEST `_infer_cellmask_fromaggr`  function defined above\n",
                 "\n",
                 "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>\n",
                 "##\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.organelles import fixed_infer_cellmask, infer_cellmask\n",
+                "from infer_subc.organelles import fixed_infer_cellmask_fromaggr, infer_cellmask_fromaggr\n",
                 "\n",
-                "cellmask_ =  fixed_infer_cellmask(img_2D) "
+                "soma_ =  fixed_infer_cellmask_fromaggr(img_2D) "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "viewer.add_image(\n",
                 "    SO_label,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    cellmask_,\n",
+                "    soma_,\n",
                 "    scale=scale \n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Write the `infer_cellmask` spec to the widget json"
+                "Write the `infer_cellmask_fromaggr` spec to the widget json"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
-                "_fixed_infer_cellmask =  {\n",
+                "_fixed_infer_cellmask_fromaggr =  {\n",
                 "        \"name\": \" infer cellmask mask (fixed parameters)\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"fixed_infer_cellmask\",\n",
+                "        \"python::function\": \"fixed_infer_cellmask_fromaggr\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"fixed_infer_cellmask\", _fixed_infer_cellmask, overwrite=True)"
+                "add_function_spec_to_widget_json(\"fixed_infer_cellmask_fromaggr\", _fixed_infer_cellmask_fromaggr, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "_infer_cellmask =  {\n",
+                "_infer_cellmask_fromaggr =  {\n",
                 "        \"name\": \" infer cellmask mask\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_cellmask\",\n",
+                "        \"python::function\": \"infer_cellmask_fromaggr\",\n",
                 "        \"parameters\": {\n",
-                "                \"median_sz_cellmask\": {\n",
+                "                \"median_sz_soma\": {\n",
                 "                        \"widget_type\": \"slider\",\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"min\": 3,\n",
                 "                        \"max\": 15,\n",
                 "                        \"increment\": 1\n",
                 "                },\n",
-                "                \"gauss_sig_cellmask\": {\n",
+                "                \"gauss_sig_soma\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.25,\n",
                 "                        \"max\": 15.0,\n",
                 "                        \"min\": 1.25,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
                 "                \"median_sz_nuc\": {\n",
@@ -1387,67 +1388,67 @@
                 "                \"small_obj_w_nuc\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 1,\n",
                 "                        \"max\": 50,\n",
                 "                        \"min\": 1,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },                           \n",
-                "                \"max_hole_w_cellmask\": {\n",
+                "                \"max_hole_w_soma\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 2,\n",
                 "                        \"max\": 100,\n",
                 "                        \"min\": 20,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },           \n",
-                "                \"small_obj_w_cellmask\": {\n",
+                "                \"small_obj_w_soma\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 1,\n",
                 "                        \"max\": 50,\n",
                 "                        \"min\": 1,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },        \n",
                 "        }\n",
                 "}\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"infer_cellmask\", _infer_cellmask, overwrite=True )\n",
+                "add_function_spec_to_widget_json(\"infer_cellmask_fromaggr\", _infer_cellmask_fromaggr, overwrite=True )\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "_raw_cellmask_MCZ =  {\n",
+                "_raw_soma_MCZ =  {\n",
                 "        \"name\": \"define weighted aggregate cellmask signal (MCZ-cellprofiler)\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"raw_cellmask_MCZ\",\n",
+                "        \"python::function\": \"raw_soma_MCZ\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"raw_cellmask_MCZ\", _raw_cellmask_MCZ, overwrite=True)"
+                "add_function_spec_to_widget_json(\"raw_soma_MCZ\", _raw_soma_MCZ, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "_non_linear_cellmask_transform =  {\n",
+                "_non_linear_soma_transform_MCZ =  {\n",
                 "        \"name\": \"non-linear filter of cellmask signal (MCZ-cellprofiler)\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"non_linear_cellmask_transform\",\n",
+                "        \"python::function\": \"non_linear_soma_transform_MCZ\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"non_linear_cellmask_transform\", _non_linear_cellmask_transform)"
+                "add_function_spec_to_widget_json(\"non_linear_soma_transform_MCZ\", _non_linear_soma_transform_MCZ)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1542,26 +1543,26 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "--------------------------\n",
                 "\n",
-                "# TEST `infer_cellmask` exported functions\n"
+                "# TEST `infer_cellmask_fromaggr` exported functions\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.organelles import fixed_infer_cellmask\n",
+                "from infer_subc.organelles import fixed_infer_cellmask_fromaggr\n",
                 "\n",
-                "cellmask_mask =  fixed_infer_cellmask(img_2D) "
+                "soma_mask =  fixed_infer_cellmask_fromaggr(img_2D) "
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1575,15 +1576,15 @@
             "outputs": [],
             "source": [
                 "# viewer = napari.Viewer()\n",
                 "\n",
                 "viewer.scale_bar.visible = True\n",
                 "\n",
                 "viewer.add_labels(\n",
-                "    cellmask_mask,\n",
+                "    soma_mask,\n",
                 "    scale=scale,\n",
                 "    blending='additive'\n",
                 ")\n"
             ]
         },
         {
             "cell_type": "code",
@@ -1611,44 +1612,44 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def make_infer_cellmask_step_by_step_dict():\n",
+                "def make_infer_cellmask_fromaggr_step_by_step_dict():\n",
                 "    \"\"\"\n",
-                "    crete .json version of infer_cellmask\n",
+                "    crete .json version of infer_cellmask_fromaggr\n",
                 "    \"\"\"\n",
                 "    step_name = []\n",
                 "    function_name = []\n",
                 "    category =[]\n",
                 "    parameter_values = []\n",
                 "    parent = []\n",
                 "\n",
                 "    ###################\n",
                 "    # EXTRACT\n",
                 "    ###################   \n",
-                "    # struct_img = _raw_cellmask_MCZ(in_img)\n",
+                "    # struct_img = _raw_soma_MCZ(in_img)\n",
                 "    step_name.append(\"1\")\n",
-                "    function_name.append(\"raw_cellmask_MCZ\")\n",
+                "    function_name.append(\"raw_soma_MCZ\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(0)\n",
                 "\n",
                 "    step_name.append(\"2\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( dict(chan = NUC_CH) )\n",
                 "    parent.append(0)\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
                 "    ###################\n",
-                "    #CELLMASK\n",
+                "    #SOMA\n",
                 "    step_name.append(\"3\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(1)\n",
                 "\n",
                 "\n",
@@ -1662,15 +1663,15 @@
                 "    step_name.append(\"5\")\n",
                 "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(dict( sigma = 1.4 ))\n",
                 "    parent.append(4)\n",
                 "\n",
                 "    step_name.append(\"6\")\n",
-                "    function_name.append(\"non_linear_cellmask_transform\")\n",
+                "    function_name.append(\"non_linear_soma_transform_MCZ\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(5)\n",
                 "\n",
                 "    #NUC\n",
                 "    step_name.append(\"7\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
@@ -1689,15 +1690,15 @@
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(dict( sigma = 1.4 ))\n",
                 "    parent.append(8)\n",
                 "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    # CELLMASK\n",
+                "    # SOMA\n",
                 "    step_name.append(\"10\")\n",
                 "    function_name.append(\"masked_object_thresh\")\n",
                 "    category.append(\"core\")\n",
                 "    parameter_values.append(dict( th_method=\"ave_tri_med\",\n",
                 "                                                            cutoff_size = 100,\n",
                 "                                                            th_adjust = 0.5))\n",
                 "    parent.append(6)\n",
@@ -1720,48 +1721,48 @@
                 "    step_name.append(\"12\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
                 "    parent.append(11)\n",
                 "\n",
                 "    step_name.append(\"13\")\n",
-                "    function_name.append(\"size_filter_2D\")\n",
+                "    function_name.append(\"size_filter_linear_size\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(12)\n",
                 "\n",
                 "    step_name.append(\"14\")\n",
                 "    function_name.append(\"label\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(13)\n",
                 "\n",
-                "    # CELLMASK\n",
+                "    # SOMA\n",
                 "    step_name.append(\"15\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
                 "    parent.append(10)\n",
                 "\n",
                 "    step_name.append(\"16\")\n",
-                "    function_name.append(\"size_filter_2D\")\n",
+                "    function_name.append(\"size_filter_linear_size\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(15)\n",
                 "\n",
                 "    step_name.append(\"17\")\n",
                 "    function_name.append(\"masked_inverted_watershed\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append([ 5 , 14, 16])\n",
                 "\n",
                 "    ###################\n",
                 "    # POST- POST_PROCESSING\n",
                 "    ###################\n",
-                "    # keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "    # keep the \"SOMA\" label which contains the highest total signal\n",
                 "    step_name.append(\"18\")\n",
                 "    function_name.append(\"choose_max_label\")\n",
                 "    category.append(\"postpostprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append([5, 17])\n",
                 "\n",
                 "    ##########################\n",
@@ -1783,35 +1784,35 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from infer_subc.organelles_config.helper import write_workflow_json\n",
                 "\n",
-                "infer_cellmask_stepbystep_dict = make_infer_cellmask_step_by_step_dict()\n",
+                "infer_cellmask_fromaggr_stepbystep_dict = make_infer_cellmask_fromaggr_step_by_step_dict()\n",
                 "\n",
-                "write_workflow_json(\"conf_2.1.cellmask_stepbystep\", infer_cellmask_stepbystep_dict )"
+                "write_workflow_json(\"conf_2.1.soma_stepbystep\", infer_cellmask_fromaggr_stepbystep_dict )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def make_infer_cellmask_step_by_step_from_raw_dict():\n",
+                "def make_infer_cellmask_fromaggr_step_by_step_from_raw_dict():\n",
                 "    \"\"\"\n",
                 "    Procedure to infer nuclei from linearly unmixed input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
                 "\n",
-                "    cellmask_mask: np.ndarray\n",
+                "    soma_mask: np.ndarray\n",
                 "        mask\n",
                 "\n",
                 "    Returns\n",
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "\n",
@@ -1827,32 +1828,32 @@
                 "    ###################   \n",
                 "    step_name.append(\"1\")\n",
                 "    function_name.append(\"fixed_get_optimal_Z_img\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(0)\n",
                 "\n",
-                "    # CELLMASK\n",
+                "    # SOMA\n",
                 "    step_name.append(\"2\")\n",
-                "    function_name.append(\"raw_cellmask_MCZ\")\n",
+                "    function_name.append(\"raw_soma_MCZ\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(1)\n",
                 "\n",
                 "    # NUC\n",
                 "    step_name.append(\"3\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( dict(chan = NUC_CH) )\n",
                 "    parent.append(1)\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
                 "    ###################\n",
-                "    # CELLMASK\n",
+                "    # SOMA\n",
                 "    step_name.append(\"4\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(2)\n",
                 "\n",
                 "    step_name.append(\"5\")\n",
@@ -1864,15 +1865,15 @@
                 "    step_name.append(\"6\")\n",
                 "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(dict( sigma = 1.4 ))\n",
                 "    parent.append(5)\n",
                 "\n",
                 "    step_name.append(\"7\")\n",
-                "    function_name.append(\"non_linear_cellmask_transform\")\n",
+                "    function_name.append(\"non_linear_soma_transform_MCZ\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(6)\n",
                 "\n",
                 "    #NUC\n",
                 "    step_name.append(\"8\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
@@ -1891,15 +1892,15 @@
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(dict( sigma = 1.4 ))\n",
                 "    parent.append(9)\n",
                 "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    # CELLMASK\n",
+                "    # SOMA\n",
                 "    step_name.append(\"11\")\n",
                 "    function_name.append(\"masked_object_thresh\")\n",
                 "    category.append(\"core\")\n",
                 "    parameter_values.append(dict( th_method=\"ave_tri_med\",\n",
                 "                                                            cutoff_size = 100,\n",
                 "                                                            th_adjust = 0.5))\n",
                 "    parent.append(7)\n",
@@ -1920,49 +1921,49 @@
                 "    step_name.append(\"13\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
                 "    parent.append(12)\n",
                 "\n",
                 "    step_name.append(\"14\")\n",
-                "    function_name.append(\"size_filter_2D\")\n",
+                "    function_name.append(\"size_filter_linear_size\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(13)\n",
                 "\n",
                 "    step_name.append(\"15\")\n",
                 "    function_name.append(\"label\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(14)\n",
                 "\n",
                 "\n",
-                "    # CELLMASK\n",
+                "    # SOMA\n",
                 "    step_name.append(\"16\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
                 "    parent.append(11)\n",
                 "\n",
                 "    step_name.append(\"17\")\n",
-                "    function_name.append(\"size_filter_2D\")\n",
+                "    function_name.append(\"size_filter_linear_size\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(16)\n",
                 "\n",
                 "    step_name.append(\"18\")\n",
                 "    function_name.append(\"masked_inverted_watershed\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append([  7 , 15,17 ])\n",
                 "\n",
                 "    ###################\n",
                 "    # POST- POST_PROCESSING\n",
                 "    ###################\n",
-                "    # keep the \"CELLMASK\" label which contains the highest total signal\n",
+                "    # keep the \"SOMA\" label which contains the highest total signal\n",
                 "    step_name.append(\"19\")\n",
                 "    function_name.append(\"choose_max_label\")\n",
                 "    category.append(\"postpostprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append([6,18])\n",
                 "\n",
                 "    ##########################\n",
@@ -1983,17 +1984,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "infer_cellmask_stepbystep_from_raw_dict = make_infer_cellmask_step_by_step_from_raw_dict()\n",
+                "infer_cellmask_fromaggr_stepbystep_from_raw_dict = make_infer_cellmask_fromaggr_step_by_step_from_raw_dict()\n",
                 "\n",
-                "write_workflow_json(\"conf_1.1.cellmask_stepbystep_from_raw\", infer_cellmask_stepbystep_from_raw_dict)"
+                "write_workflow_json(\"conf_1.1.soma_stepbystep_from_raw\", infer_cellmask_fromaggr_stepbystep_from_raw_dict)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2006,33 +2007,33 @@
                 "\n",
                 "proceed to [02_infer_nuclei.ipynb](./02_infer_nuclei.ipynb)\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "infer-subc",
+            "display_name": "napariNEW",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15 (main, Nov 24 2022, 14:39:17) [MSC v.1916 64 bit (AMD64)]"
+            "version": "3.9.16"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
-                "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
+                "hash": "d6148ef1fb015fb20f0b6da2ea61c87c6b848bdf3dabb03087e5d5cd0c4607e9"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `infer-subc-0.0.6b0/notebooks/11_regionprops.ipynb` & `infer-subc-0.0.post1/notebooks/10_regionprops.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/12_batch_process.ipynb` & `infer-subc-0.0.post1/notebooks/11_batch_process.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/13_fn_prototypes_json.ipynb` & `infer-subc-0.0.post1/notebooks/12_fn_prototypes_json.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926636579878099%*

 * *Differences: {"'cells'": "{0: {delete: ['attachments']}, 2: {'execution_count': 2}, 16: {'execution_count': 13, "*

 * *            "'outputs': {1: {'execution_count': 13}}, 'source': {insert: [(8, "*

 * *            '\'                        "min": 1,\\n\'), (16, \'                        "min": '*

 * *            "1.25,\\n')], delete: [16, 8]}}, 23: {'outputs': {0: {'text': ['function "*

 * *            "non_linear_cellmask_transform_MCZ is already in all_functions.json\\n', 'overwriting  "*

 * *            "non_linear_cellmask_transform_MCZ\ […]*

```diff
@@ -1,11 +1,10 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Export function prototypes \n",
                 "\n",
                 "We need to compose workflows and place the function prototypes into their proper place."
             ]
@@ -16,15 +15,15 @@
             "metadata": {},
             "source": [
                 "### IMports\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "from infer_subc.organelles_config.helper import write_workflow_json\n",
                 "import numpy as np"
             ]
@@ -662,15 +661,15 @@
                 "}\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"select_channel_from_raw\",_select_channel_from_raw_dict, overwrite=True )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "function scale_and_smooth is already in all_functions.json\n",
@@ -679,37 +678,37 @@
                 },
                 {
                     "data": {
                         "text/plain": [
                             "1"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "_scale_and_smooth_dict =  {\n",
                 "        \"name\": \"scale and smooth\",\n",
                 "        \"python::module\": \"infer_subc.core.img\",\n",
                 "        \"python::function\": \"scale_and_smooth\",\n",
                 "        \"parameters\": {\n",
                 "                \"median_sz\": {\n",
                 "                        \"widget_type\": \"slider\",\n",
                 "                        \"data_type\": \"int\",\n",
-                "                        \"min\": 0,\n",
+                "                        \"min\": 1,\n",
                 "                        \"max\": 15,\n",
                 "                        \"increment\": 1\n",
                 "                },\n",
                 "                \"gauss_sig\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.25,\n",
                 "                        \"max\": 15.0,\n",
-                "                        \"min\": 0,\n",
+                "                        \"min\": 1.25,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
                 "        }\n",
                 "}\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"scale_and_smooth\",_scale_and_smooth_dict, overwrite=True )"
             ]
@@ -992,16 +991,16 @@
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "function non_linear_cellmask_transform is already in all_functions.json\n",
-                        "overwriting  non_linear_cellmask_transform\n"
+                        "function non_linear_cellmask_transform_MCZ is already in all_functions.json\n",
+                        "overwriting  non_linear_cellmask_transform_MCZ\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "1"
                         ]
@@ -1009,22 +1008,22 @@
                     "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "\n",
-                "_non_linear_cellmask_transform =  {\n",
+                "_non_linear_cellmask_transform_MCZ =  {\n",
                 "        \"name\": \"non-linear distortion to fill out cellmask\",\n",
                 "        \"python::module\": \"infer_subc.organelles.cellmask\",\n",
-                "        \"python::function\": \"non_linear_cellmask_transform\",\n",
+                "        \"python::function\": \"non_linear_cellmask_transform_MCZ\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"non_linear_cellmask_transform\", _non_linear_cellmask_transform, overwrite=True)"
+                "add_function_spec_to_widget_json(\"non_linear_cellmask_transform_MCZ\", _non_linear_cellmask_transform_MCZ, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
@@ -1561,15 +1560,14 @@
                 "- `filament_filter`\n",
                 "\n",
                 "numpy\n",
                 "- 'logical_or'\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "##  helper function definitions\n",
                 "\n",
                 "Wrappers for spot and filiment filters"
             ]
@@ -1624,101 +1622,15 @@
                 "\n",
                 "add_function_spec_to_widget_json(\"filament_filter\", _filament_filter, overwrite=True )\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "function filament_filter_3 is already in all_functions.json\n",
-                        "overwriting  filament_filter_3\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "1"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "\n",
-                "_filament_filter_3 =  {\n",
-                "        \"name\": \"filament filter thresholding\",\n",
-                "        \"python::module\": \"infer_subc.core.img\",\n",
-                "        \"python::function\": \"filament_filter\",\n",
-                "        \"parameters\": {\n",
-                "                \"filament_scale_1\": {\n",
-                "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.01,\n",
-                "                        \"max\": 10,\n",
-                "                        \"min\": 0,\n",
-                "                        \"widget_type\": \"slider\"\n",
-                "                },\n",
-                "                \"filament_cutoff_1\": {\n",
-                "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.0001,\n",
-                "                        \"max\": 5,\n",
-                "                        \"min\": 0,\n",
-                "                        \"widget_type\": \"slider\"\n",
-                "                },\n",
-                "                \"filament_scale_2\": {\n",
-                "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.01,\n",
-                "                        \"max\": 10,\n",
-                "                        \"min\": 0,\n",
-                "                        \"widget_type\": \"slider\"\n",
-                "                },\n",
-                "                \"filament_cutoff_2\": {\n",
-                "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.0001,\n",
-                "                        \"max\": 5,\n",
-                "                        \"min\": 0,\n",
-                "                        \"widget_type\": \"slider\"\n",
-                "                },\n",
-                "                \"filament_scale_3\": {\n",
-                "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.01,\n",
-                "                        \"max\": 10,\n",
-                "                        \"min\": 0,\n",
-                "                        \"widget_type\": \"slider\"\n",
-                "                },\n",
-                "                \"filament_cutoff_3\": {\n",
-                "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.0001,\n",
-                "                        \"max\": 5,\n",
-                "                        \"min\": 0,\n",
-                "                        \"widget_type\": \"slider\"\n",
-                "                },\n",
-                "                \"method\": {\n",
-                "                        \"data_type\": \"str\",\n",
-                "                        \"options\": [\"3D\", \"slice_by_slice\"],\n",
-                "                        \"widget_type\": \"drop-down\"\n",
-                "                }\n",
-                "                \n",
-                "        }\n",
-                "}\n",
-                "\n",
-                "add_function_spec_to_widget_json(\"filament_filter_3\", _filament_filter_3, overwrite=True )\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "function spot_filter_3 is already in all_functions.json\n",
@@ -1727,73 +1639,68 @@
                 },
                 {
                     "data": {
                         "text/plain": [
                             "1"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "\n",
                 "_spot_filter_3 =  {\n",
                 "        \"name\": \"spot filter thresholding (3 scales)\",\n",
                 "        \"python::module\": \"infer_subc.core.img\",\n",
                 "        \"python::function\": \"spot_filter_3\",\n",
                 "        \"parameters\": {\n",
-                "                \"spot_scale_1\": {\n",
+                "                \"dot_scale_1\": {\n",
                 "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.01,\n",
+                "                        \"increment\": 0.05,\n",
                 "                        \"max\": 10,\n",
                 "                        \"min\": 0,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"spot_cutoff_1\": {\n",
+                "                \"dot_cut_1\": {\n",
                 "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.0001,\n",
-                "                        \"max\": 5,\n",
+                "                        \"increment\": 0.001,\n",
+                "                        \"max\": 0.5,\n",
                 "                        \"min\": 0,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"spot_scale_2\": {\n",
+                "                \"dot_scale_2\": {\n",
                 "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.01,\n",
+                "                        \"increment\": 0.05,\n",
                 "                        \"max\": 10,\n",
                 "                        \"min\": 0,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"spot_cutoff_2\": {\n",
+                "                \"dot_cut_2\": {\n",
                 "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.0001,\n",
-                "                        \"max\": 5,\n",
+                "                        \"increment\": 0.001,\n",
+                "                        \"max\": 0.5,\n",
                 "                        \"min\": 0,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"spot_scale_3\": {\n",
+                "                \"dot_scale_3\": {\n",
                 "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.01,\n",
+                "                        \"increment\": 0.05,\n",
                 "                        \"max\": 10,\n",
                 "                        \"min\": 0,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"spot_cutoff_3\": {\n",
+                "                \"dot_cut_3\": {\n",
                 "                        \"data_type\": \"float\",\n",
-                "                        \"increment\": 0.0001,\n",
-                "                        \"max\": 5,\n",
+                "                        \"increment\": 0.001,\n",
+                "                        \"max\": 0.5,\n",
                 "                        \"min\": 0,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"method\": {\n",
-                "                        \"data_type\": \"str\",\n",
-                "                        \"options\": [\"3D\", \"slice_by_slice\"],\n",
-                "                        \"widget_type\": \"drop-down\"\n",
-                "                }\n",
                 "        }\n",
                 "}\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"spot_filter_3\", _spot_filter_3, overwrite=True )\n",
                 "\n"
             ]
         },
@@ -1897,15 +1804,14 @@
                 "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"logical_or\",_logical_or)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-----------------\n",
                 "# MITOCHONDRIA"
             ]
         },
@@ -2235,15 +2141,14 @@
                 "}\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"infer_golgi\", _infer_golgi, overwrite=True )\n",
                 "\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-----------------\n",
                 "## PEROXISOME"
             ]
         },
@@ -2345,15 +2250,14 @@
                 "}\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"infer_perox\", _infer_perox, overwrite=True )\n",
                 "\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-----------------\n",
                 "# ER"
             ]
         },
@@ -2449,15 +2353,14 @@
                 "}\n",
                 "\n",
                 "add_function_spec_to_widget_json(\"infer_er\", _infer_er, overwrite=True )\n",
                 "\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-----------------\n",
                 "## LIPID"
             ]
         },
@@ -2602,15 +2505,14 @@
                 "\n",
                 "## HELPERS (lipid)\n",
                 "- `apply_threshold`\n",
                 "-\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "##  helper function definitions\n",
                 "\n",
                 "Wrappers for vessleness filters"
             ]
@@ -2753,15 +2655,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.10.10"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "d6148ef1fb015fb20f0b6da2ea61c87c6b848bdf3dabb03087e5d5cd0c4607e9"
             }
         }
```

### Comparing `infer-subc-0.0.6b0/notebooks/14_workflow_defs_json.ipynb` & `infer-subc-0.0.post1/notebooks/13_workflow_defs_json.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999885762123629%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(58, '    "*

 * *            'function_name.append("non_linear_cellmask_transform_MCZ")\\n\')], delete: [58]}}, 8: '*

 * *            "{'source': {insert: [(71, '    "*

 * *            'function_name.append("non_linear_cellmask_transform_MCZ")\\n\')], delete: [71]}}, 28: '*

 * *            "{'source': {insert: [(71, '    "*

 * *            'function_name.append("non_linear_cellmask_transform_MCZ")\\n\')], delete: [71]}}, 32: '*

 * *            '{\'outputs\': {0: {\'data\': {\'text/plain\': {insert:  […]*

```diff
@@ -117,15 +117,15 @@
                 "    parameter_values.append(dict(median_sz = 4, gauss_sig=4.5 ))\n",
                 "    parent.append(cellmask_input_step)\n",
                 "    annotation.append(f\"cellmask segmentation: {step_n}\")\n",
                 "    struct_img_step = step_n\n",
                 "    step_n += 1\n",
                 "\n",
                 "    step_name.append(f\"{step_n}\")\n",
-                "    function_name.append(\"non_linear_cellmask_transform\")\n",
+                "    function_name.append(\"non_linear_cellmask_transform_MCZ\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    annotation.append(f\"cellmask segmentation: {step_n}\")\n",
                 "    parent.append(step_n-1)\n",
                 "\n",
                 "    step_n += 1\n",
                 "\n",
@@ -307,15 +307,15 @@
                 "    parameter_values.append(dict(median_sz = 9, gauss_sig=4.5 ))\n",
                 "    parent.append(cellmask_input_step)\n",
                 "    annotation.append(f\"basic nuclei segmentation: {step_n}\")\n",
                 "    struct_img_step = step_n\n",
                 "    step_n += 1\n",
                 "\n",
                 "    step_name.append(f\"{step_n}\")\n",
-                "    function_name.append(\"non_linear_cellmask_transform\")\n",
+                "    function_name.append(\"non_linear_cellmask_transform_MCZ\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    annotation.append(f\"basic nuclei segmentation: {step_n}\")\n",
                 "    parent.append(step_n-1)\n",
                 "\n",
                 "    step_n += 1\n",
                 "\n",
@@ -1366,15 +1366,15 @@
                 "    parameter_values.append(dict(median_sz = 4, gauss_sig=1.4 ))\n",
                 "    parent.append(cellmask_input_step)\n",
                 "    annotation.append(f\"basic nuclei segmentation: {step_n}\")\n",
                 "    struct_img_step = step_n\n",
                 "    step_n += 1\n",
                 "\n",
                 "    step_name.append(f\"{step_n}\")\n",
-                "    function_name.append(\"non_linear_cellmask_transform\")\n",
+                "    function_name.append(\"non_linear_cellmask_transform_MCZ\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    annotation.append(f\"basic nuclei segmentation: {step_n}\")\n",
                 "    parent.append(step_n-1)\n",
                 "\n",
                 "    step_n += 1\n",
                 "\n",
@@ -1606,15 +1606,15 @@
                             "   'annotation': ' this creates an aggregate signal for the cellmask'},\n",
                             "  '3': {'category': 'preprocessing',\n",
                             "   'function': 'scale_and_smooth',\n",
                             "   'parameter_values': {'median_sz': 4, 'gauss_sig': 3.4},\n",
                             "   'parent': 2,\n",
                             "   'annotation': 'cellmask segmentation: 3'},\n",
                             "  '4': {'category': 'preprocessing',\n",
-                            "   'function': 'non_linear_cellmask_transform',\n",
+                            "   'function': 'non_linear_cellmask_transform_MCZ',\n",
                             "   'parent': 3,\n",
                             "   'annotation': 'cellmask segmentation: 4'},\n",
                             "  '5': {'category': 'core',\n",
                             "   'function': 'masked_object_thresh',\n",
                             "   'parameter_values': {'th_method': 'ave_tri_med',\n",
                             "    'cutoff_size': 100,\n",
                             "    'th_adjust': 0.8},\n",
@@ -1862,15 +1862,15 @@
                             "  'annotation': ' this creates an aggregate signal for the cellmask'},\n",
                             " '3': {'category': 'preprocessing',\n",
                             "  'function': 'scale_and_smooth',\n",
                             "  'parameter_values': {'median_sz': 4, 'gauss_sig': 3.4},\n",
                             "  'parent': 2,\n",
                             "  'annotation': 'cellmask segmentation: 3'},\n",
                             " '4': {'category': 'preprocessing',\n",
-                            "  'function': 'non_linear_cellmask_transform',\n",
+                            "  'function': 'non_linear_cellmask_transform_MCZ',\n",
                             "  'parent': 3,\n",
                             "  'annotation': 'cellmask segmentation: 4'},\n",
                             " '5': {'category': 'core',\n",
                             "  'function': 'masked_object_thresh',\n",
                             "  'parameter_values': {'th_method': 'ave_tri_med',\n",
                             "   'cutoff_size': 100,\n",
                             "   'th_adjust': 0.8},\n",
```

### Comparing `infer-subc-0.0.6b0/notebooks/15_final_workflow.ipynb` & `infer-subc-0.0.post1/notebooks/14_final_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/00.1_pipeline_setup_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/00.1_pipeline_setup_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/00.2_extract_optimal_Z.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/00.2_extract_optimal_Z.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/01_infer_nuclei_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/02a_infer_soma_3D.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9229051196506659%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Infer ***cellmask*** -  1️⃣ \\n'), (2, '> WARNING: "*

 * *            "(🚨🚨🚨🚨 Steps 3-9 depend on establishing a good solution here.)\\n'), (3, '\\n'), (4, "*

 * *            "'\\n'), (5, '>> WARNING:  THIS DOES NOT WORK WELL - lacking fluorescent marker\\n'), "*

 * *            "(6, '>> #### Because we do NOT have a direct cell membrane / cellmask signal, this "*

 * *            'segmentation is trickiest and potentially most problematic part of the overall '*

 * *            'sub-cellul […]*

```diff
@@ -1,166 +1,166 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Infer ***nuclei*** - 2\ufe0f\u20e3 \n",
+                "# Infer ***cellmask*** -  1\ufe0f\u20e3 \n",
                 "\n",
-                "> WARNING: (\ud83d\udea8\ud83d\udea8\ud83d\udea8\ud83d\udea8 Steps 2-9 depend on establishing a good solution here.)\n",
+                "> WARNING: (\ud83d\udea8\ud83d\udea8\ud83d\udea8\ud83d\udea8 Steps 3-9 depend on establishing a good solution here.)\n",
+                "\n",
+                "\n",
+                ">> WARNING:  THIS DOES NOT WORK WELL - lacking fluorescent marker\n",
+                ">> #### Because we do NOT have a direct cell membrane / cellmask signal, this segmentation is trickiest and potentially most problematic part of the overall sub-cellular component inference pipeline. We are using the nuclei of the cell with the brightest total fluorescence (all channels) to identify a single cellmask for all downstream steps. The Soma (via the Cytosol mask) will be used to define ALL subsequent sub-cellular Objects.\n",
                 "\n",
                 "--------------\n",
                 "\n",
                 "## OBJECTIVE: \n",
-                "### \u2705 Infer sub-cellular component #2: ***nuclei***  in order to understand interactome \n",
+                "### \u2705 Infer sub-cellular component #2: ***cellmask***/cell body in order to understand interactome \n",
                 "\n",
-                "Infer a segmentation of the ***nuclei*** in order to measure its shape, position, size, and interaction with other organelles/cellular components.  \n",
+                "Infer a segmentation of the cell body -- the ***cellmask*** -- in order to measure its shape, position, and size.\n",
                 "\n",
-                "## OVERVIEW:\n",
+                "CONTEXT: \"Soma\" is used here becuase subsequent experiments will contain neurons who's cellmask has a similar shape to an iPS cell body.\n",
                 "\n",
-                "We will infer the nuclei using the nuclei channel (e.g. 'ch = 0).\n",
+                "## OVERVIEW: \n",
                 "\n",
-                "Dependencies:\n",
-                "***Soma*** and ***cytoplasm*** inference rely on the ***nuclei*** inference.  Therefore all of the sub-cellular objects rely on the NU segmentation.\n"
+                "This method is used in the case where there is no cell fill/membrane marker.\n",
+                "\n",
+                "We will infer the cellmask from a combination of fluorescent signals. The current selection includes the lysosomes, ER, and Golgi (e.g., 'Ch = 1, 3, 5) which have some intracellular fluorescence - likely from off target marker localization to the entire cellmask and/or the cell membrane. There are two other channels, the residual channel from linear unmixing (e.g. `ch = 7`) and the lipid droplet channel (e.g., `ch = 6`) that could more lead to more unbiased selection of the entire cellmask. However, the drawback of these two markers is that they are present in every cell which makes downstream cell selection more challenging. To expand on this, we will be collecting per cell measurements, so each cell area has to be segmented individually even if there are two appropriately labeled cells within one field of view. "
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## preamble\n",
                 "\n",
                 "1. imports\n",
                 "2. setup\n",
-                "3. infer-nuclei\n",
+                "4. infer-cellmask\n",
                 "    * input\n",
                 "    * pre-processing\n",
                 "    * core processing\n",
                 "    * post-processing\n",
+                "    * select individual cell\n",
                 "    * output"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "\n",
-                "### IMPORTS"
+                "## IMPORTS"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "The autoreload extension is already loaded. To reload it, use:\n",
-                        "  %reload_ext autoreload\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# top level imports\n",
                 "from pathlib import Path\n",
                 "import os, sys\n",
                 "from collections import defaultdict\n",
-                "from typing import Optional\n",
                 "\n",
                 "import numpy as np\n",
                 "\n",
-                "from aicssegmentation.core.pre_processing_utils import  image_smoothing_gaussian_slice_by_slice \n",
+                "from scipy import ndimage as ndi\n",
+                "from aicssegmentation.core.pre_processing_utils import ( intensity_normalization, \n",
+                "                                                         image_smoothing_gaussian_slice_by_slice )\n",
+                "from aicssegmentation.core.MO_threshold import MO\n",
                 "from aicssegmentation.core.utils import hole_filling\n",
+                "\n",
+                "from skimage import filters\n",
+                "from skimage.segmentation import watershed\n",
+                "from skimage.morphology import remove_small_holes   # function for post-processing (size filter)\n",
                 "from skimage.measure import label\n",
                 "\n",
                 "# # package for io \n",
                 "from aicsimageio import AICSImage\n",
                 "\n",
                 "import napari\n",
                 "\n",
                 "### import local python functions in ../infer_subc\n",
                 "sys.path.append(os.path.abspath((os.path.join(os.getcwd(), '..'))))\n",
                 "\n",
                 "\n",
                 "from infer_subc.core.file_io import (read_czi_image,\n",
                 "                                                                    list_image_files)\n",
-                "from infer_subc.core.img import *\n",
-                "from infer_subc.organelles import fixed_get_optimal_Z_image, fixed_find_optimal_Z, find_optimal_Z\n",
+                "\n",
                 "from infer_subc.constants import (TEST_IMG_N,\n",
                 "                                                                    NUC_CH ,\n",
                 "                                                                    LYSO_CH ,\n",
                 "                                                                    MITO_CH ,\n",
                 "                                                                    GOLGI_CH ,\n",
                 "                                                                    PEROX_CH ,\n",
                 "                                                                    ER_CH ,\n",
                 "                                                                    LD_CH ,\n",
-                "                                                                    RESIDUAL_CH, \n",
-                "                                                                    ALL_CHANNELS )          \n",
+                "                                                                    RESIDUAL_CH )                                                                    \n",
+                "from infer_subc.core.img import *\n",
                 "\n",
-                "from infer_subc.organelles import infer_cellmask_fromaggr, fixed_infer_cellmask_fromaggr\n",
+                "from infer_subc.organelles import fixed_get_optimal_Z_image, fixed_find_optimal_Z, find_optimal_Z\n",
                 "\n",
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "\n",
                 "## SETUP\n",
                 "CUSTOMIZE WITH: \n",
                 "1. updated path to data\n",
                 "2. updated folder name for \"raw\" data\n",
                 "\n",
                 "> NOTE: we are operating on a single \"test\" image in this notebook.  The batch-processing of all the images will be happen at the end of the notebook after we have developed/confirmed the setmentation procedures and parameter settings."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
                 "# build the datapath\n",
                 "# all the imaging data goes here.\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
-                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
                 "\n",
                 "# linearly unmixed \".czi\" files are here\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
-                "# get the list of all files in \"raw\"\n",
+                "# get the list of all files\n",
                 "img_file_list = list_image_files(data_path,im_type)\n",
                 "test_img_name = img_file_list[test_img_n]\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/opt/anaconda3/envs/napariNEW/lib/python3.9/site-packages/ome_types/_convenience.py:106: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "c:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:105: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
                 "# isolate image as an ndarray and metadata as a dictionary\n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
@@ -173,449 +173,338 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## infer ***nuclei***\n",
+                "##  infer ***cellmask***\n",
                 "\n",
-                "### summary of steps\n",
+                "#### summary of steps\n",
                 "\n",
                 "\u27a1\ufe0f INPUT\n",
-                "- channel 0\n",
+                "- multi-channel sum (6.*1, 3, 2.*5)\n",
+                "- nuclei mask\n",
                 "\n",
                 "PRE-PROCESSING\n",
-                "- scale to min 0, max 1.0\n",
-                "- median Filter window 4\n",
-                "- gaussian 1.34\n",
-                "\n",
-                "CORE-PROCESSING\n",
-                "  - threshold method minimum cross-entropy.  \n",
-                "    - objects 50-400 pixels, \n",
-                "    - threshold smoothing scale: 1.34 (later 1 pixel\n",
-                "    - threshold correction factor: 0.9 (later 1.2 )\n",
-                "    - lower / upper bounds  (.1, 1)\n",
-                "    - log transformed thresholding\n",
+                "- rescaling\n",
+                "- denoise/smoothing\n",
+                "- log transform inensities\n",
+                "- scale to max 1.0\n",
+                "- create non-linear aggregate of log-intensity + scharr edge filtered intensity\n",
+                "\n",
+                "CORE PROCESSING\n",
+                "- mask object segmentation at bottom\n",
                 "\n",
                 "POST-PROCESSING\n",
                 "  - fill holes\n",
                 "  - remove small objects\n",
                 "\n",
                 "OUTPUT \u27a1\ufe0f \n",
-                "- mask of NUCLEI\n",
-                "\n",
-                "\n",
-                "> #### Note:  in later steps we will isolate individual cells for analysis. Here, all nuclei are segmented and retained.\n",
+                "- mask of SOMA\n",
                 "\n",
                 "\n",
-                "\n",
-                "#### NOTE:  using Allen Cell Segmenter  [Nucleophosmin](https://www.allencell.org/cell-observations/category/nucleophosmin) might be a good generic mechanism.  e.g.\n",
-                "-  [playground_npm1.ipynb](https://github.com/AllenInstitute/aics-segmentation/blob/master/lookup_table_demo/playground_npm1.ipynb) and [npm1.py](https://github.com/AllenInstitute/aics-segmentation/blob/master/aicssegmentation/structure_wrapper/seg_npm1.py) and [npm1_SR.py](https://github.com/AllenInstitute/aics-segmentation/blob/master/aicssegmentation/structure_wrapper/seg_npm1_SR.py)\n"
+                "> #### Note: this pipeline will eventually include a selection step to identify the cellmask that are properly labeled with all fluorescent markers. This could be one single cell per image, or more if applicable data is available."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## INPUT (prototype)\n",
                 "\n",
-                "Get the \"raw\" signals we need to analyze as well as any other dependencies in \"inferred\" objects.  "
+                "Combine multiple channels that will allow inference of the cellmask.\n",
+                "\n",
+                "Note: the selected channels were chosen based on their qualitative ability to fill the cytoplasmic area of the cell. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(16, 768, 768)\n"
+                        "(17, 704, 704)\n",
+                        "(17, 704, 704)\n"
                     ]
                 }
             ],
             "source": [
                 "###################\n",
                 "# INPUT\n",
                 "###################\n",
-                "# raw_nuclei = img_data[NUC_CH].copy()\n",
-                "raw_nuclei = select_channel_from_raw(img_data, NUC_CH)\n",
-                "\n",
-                "print(raw_nuclei.shape)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## PRE-PROCESSING (prototype)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "(16, 768, 768)\n",
-                        "(16, 768, 768)\n"
-                    ]
-                }
-            ],
-            "source": [
-                "###################\n",
-                "# PRE_PROCESSING\n",
-                "###################           \n",
-                "nuclei_norm = min_max_intensity_normalization(raw_nuclei)\n",
+                "struct_img_raw = (6. * img_data[LYSO_CH].copy() +\n",
+                "                  1. * img_data[ER_CH].copy() + \n",
+                "                  2. * img_data[GOLGI_CH].copy())\n",
                 "\n",
-                "med_filter_size = 4   \n",
-                "nuclei_med = median_filter_slice_by_slice(nuclei_norm,\n",
-                "                                      size=med_filter_size)\n",
-                "print(nuclei_med.shape)\n",
+                "raw_nuclei = img_data[NUC_CH].copy() \n",
                 "\n",
-                "gaussian_smoothing_sigma = 1.34\n",
-                "nuclei_gaus = image_smoothing_gaussian_slice_by_slice(nuclei_med,\n",
-                "                                                      sigma=gaussian_smoothing_sigma)\n",
-                "print(nuclei_gaus.shape)\n"
+                "print(struct_img_raw.shape)\n",
+                "print(raw_nuclei.shape)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### VISUALIZE: the nuclei image after pre-processing\n",
-                "Use this to adjust median filter size and gaussian sigma above."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 91,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer = napari.Viewer()"
+                "### VISUALIZE: the composite image that will be used as input\n",
+                "Use this to adjust which channels and multiplication factors to use to create the composite input image above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 92,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'nuclei_gaus' at 0x1cf5b5642b0>"
+                            "<Image layer 'img_data' at 0x25e5031c3a0>"
                         ]
                     },
-                    "execution_count": 92,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "viewer = napari.Viewer()\n",
                 "viewer.add_image(\n",
-                "    raw_nuclei,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    nuclei_med,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    nuclei_gaus,\n",
+                "    img_data,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## CORE PROCESSING (prototype)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "\n",
-                "> #### ASIDE: Thresholding\n",
-                "> [Thresholding](https://en.wikipedia.org/wiki/Thresholding_%28image_processing%29) is used to create binary images. A threshold value determines the intensity value separating foreground pixels from background pixels. Foregound pixels are pixels brighter than the threshold value, background pixels are darker. In many cases, images can be adequately segmented by thresholding followed by labelling of *connected components*, which is a fancy way of saying \"groups of pixels that touch each other\".\n",
-                "> \n",
-                "> Different thresholding algorithms produce different results. [Otsu's method](https://en.wikipedia.org/wiki/Otsu%27s_method) and [Li's minimum cross entropy threshold](https://scikit-image.org/docs/dev/auto_examples/developers/plot_threshold_li.html) are two common algorithms. Below, we use Li. You can use `skimage.filters.threshold_<TAB>` to find different thresholding methods.\n"
-            ]
-        },
-        {
             "cell_type": "code",
-            "execution_count": 87,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "(17, 704, 704)\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'struct_img_raw' at 0x25e527b0430>"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "\n",
-                "###################\n",
-                "# CORE_PROCESSING\n",
-                "###################\n",
-                "\n",
-                "threshold_factor = 0.9 #from cellProfiler\n",
-                "thresh_min = .1\n",
-                "thresh_max = 1.\n",
-                "li_thresholded = apply_log_li_threshold(nuclei_gaus, thresh_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "\n",
-                "print(li_thresholded.shape)\n",
-                "\n",
-                "\n",
-                "## **************NEED TO ADJUST THESE SETTINGS TO ISOLATE MORE OF THE TOP AND BOTTOM OF THE NUCLEI***************"
+                "viewer.add_image(\n",
+                "    struct_img_raw,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### VISUALIZE: the nuclei image after core processing\n",
-                "Use this to adjust threshold parameters above."
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 88,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'li_thresholded' at 0x1cf8f31fe80>"
+                            "<Image layer '_struct_img_raw' at 0x25e50a57340>"
                         ]
                     },
-                    "execution_count": 88,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "def _raw_soma_MCZ(img_in):\n",
+                "    \"\"\" define cellmask image\n",
+                "    \"\"\"\n",
+                "    SOMA_W = (6.,1.,2.)\n",
+                "    SOMA_CH = (LYSO_CH,ER_CH,GOLGI_CH)\n",
+                "    img_out = np.zeros_like(img_in[0]).astype(np.double)\n",
+                "    for w,ch in zip(SOMA_W,SOMA_CH):\n",
+                "        img_out += w*img_in[ch]\n",
+                "    return img_out\n",
+                "\n",
+                "_struct_img_raw = _raw_soma_MCZ(img_data)\n",
+                "\n",
                 "viewer.add_image(\n",
-                "    li_thresholded,\n",
+                "    _struct_img_raw,\n",
                 "    scale=scale\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## POST PROCESSING prototype\n",
-                "\n",
-                "> NOTE: the size parameters are by convention defined as one dimensional \"width\", so the inputs to the functions need to be _squared_ i.e. raised to the power of 2: `** 2`.   For volumetric (3D) analysis this would be _cubed_:`**3`"
+                "## PRE-PROCESSING (prototype)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 89,
+            "execution_count": 10,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                }
+            ],
             "source": [
+                "\n",
                 "###################\n",
-                "# POST_PROCESSING\n",
+                "# PRE_PROCESSING\n",
                 "###################\n",
                 "\n",
-                "hole_width = 5  \n",
-                "removed_holes = hole_filling(li_thresholded,\n",
-                "                             hole_min=0, \n",
-                "                             hole_max=hole_width**2, \n",
-                "                             fill_2d=True)\n",
-                "# there does not seem to be any observable differences between the slice-by-slice and 3D methods here for hole filling\n",
+                "################# smoothing\n",
+                "soma_norm = min_max_intensity_normalization(struct_img_raw)\n",
                 "\n",
-                "small_object_width = 15\n",
-                "cleaned_img = size_filter(removed_holes, \n",
-                "                          min_size= small_object_width**3, #changed this to 3 to adjust for the 3D voxel, instead of a 2D pixel \n",
-                "                          method=\"3D\",\n",
-                "                          connectivity=1)\n",
+                "med_filter_size = 15\n",
+                "soma_med = median_filter_slice_by_slice(soma_norm, \n",
+                "                                        size=med_filter_size)\n",
                 "\n",
-                "## ************NEED TO ADJUST THESE SETTINGS TO GET RID OF SMALL BITS*****************\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### VISUALIZE: the nuclei image after post-processing\n",
-                "Use this to adjust the size parameters above."
+                "## Need to adjust image_smoothing_gaussian_slice_by_slice in pre_processing_utils.py to integrate the mode\n",
+                "\n",
+                "gaussian_smoothing_sigma = 1.34\n",
+                "gaussian_smoothing_truncate_range = 3.0\n",
+                "soma_guas = ndi.gaussian_filter(soma_med,\n",
+                "                                sigma=gaussian_smoothing_sigma,\n",
+                "                                mode=\"nearest\", \n",
+                "                                truncate=gaussian_smoothing_truncate_range)\n",
+                "\n",
+                "\n",
+                "################# NON-Linear aggregation\n",
+                "soma_log, d = log_transform(soma_guas) \n",
+                "soma_log_norm = intensity_normalization(soma_log, scaling_param=[0])\n",
+                "\n",
+                "# soma_edges = filters.difference_of_gaussians(soma_log_norm, 2)\n",
+                "\n",
+                "# composite_soma = intensity_normalization(soma_edges, scaling_param=[0]) + soma_log_norm "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 90,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'cleaned_img' at 0x1cf8f2081c0>"
+                            "<Image layer 'composite_soma' at 0x25e437c8bb0>"
                         ]
                     },
-                    "execution_count": 90,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    removed_holes,\n",
+                "    soma_med,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    cleaned_img,\n",
+                "    soma_guas,\n",
                 "    scale=scale\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 45,
-            "metadata": {},
-            "outputs": [
-                {
-                    "ename": "RuntimeError",
-                    "evalue": "wrapped C/C++ object of type QtViewer has been deleted",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[1;31mRuntimeError\u001b[0m                              Traceback (most recent call last)",
-                        "Cell \u001b[1;32mIn[45], line 1\u001b[0m\n\u001b[1;32m----> 1\u001b[0m viewer\u001b[39m.\u001b[39;49mclose()\n",
-                        "File \u001b[1;32mc:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\napari\\viewer.py:118\u001b[0m, in \u001b[0;36mViewer.close\u001b[1;34m(self)\u001b[0m\n\u001b[0;32m    116\u001b[0m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39mlayers\u001b[39m.\u001b[39mclear()\n\u001b[0;32m    117\u001b[0m \u001b[39m# Close the main window\u001b[39;00m\n\u001b[1;32m--> 118\u001b[0m \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49mwindow\u001b[39m.\u001b[39;49mclose()\n\u001b[0;32m    120\u001b[0m \u001b[39mif\u001b[39;00m config\u001b[39m.\u001b[39masync_loading:\n\u001b[0;32m    121\u001b[0m     \u001b[39mfrom\u001b[39;00m \u001b[39m.\u001b[39;00m\u001b[39mcomponents\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mexperimental\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mchunk\u001b[39;00m \u001b[39mimport\u001b[39;00m chunk_loader\n",
-                        "File \u001b[1;32mc:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\napari\\_qt\\qt_main_window.py:1222\u001b[0m, in \u001b[0;36mWindow.close\u001b[1;34m(self)\u001b[0m\n\u001b[0;32m   1220\u001b[0m \u001b[39mif\u001b[39;00m \u001b[39mhasattr\u001b[39m(\u001b[39mself\u001b[39m, \u001b[39m'\u001b[39m\u001b[39m_qt_window\u001b[39m\u001b[39m'\u001b[39m):\n\u001b[0;32m   1221\u001b[0m     \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_teardown()\n\u001b[1;32m-> 1222\u001b[0m     \u001b[39mself\u001b[39;49m\u001b[39m.\u001b[39;49m_qt_viewer\u001b[39m.\u001b[39;49mclose()\n\u001b[0;32m   1223\u001b[0m     \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_qt_window\u001b[39m.\u001b[39mclose()\n\u001b[0;32m   1224\u001b[0m     \u001b[39mdel\u001b[39;00m \u001b[39mself\u001b[39m\u001b[39m.\u001b[39m_qt_window\n",
-                        "\u001b[1;31mRuntimeError\u001b[0m: wrapped C/C++ object of type QtViewer has been deleted"
-                    ]
-                }
-            ],
-            "source": [
-                "viewer.close()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Adjust naming and type for labels"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 46,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "NU_signal = raw_nuclei\n",
-                "\n",
-                "# renaming semantic segmentation of nuclei\n",
-                "nuclei_object = cleaned_img\n",
-                "\n",
-                "# creating instance segmentations for all nuclei in nuclei_object\n",
-                "NU_labels = label(cleaned_img)"
+                ")\n",
+                "viewer.add_image(\n",
+                "    soma_log_norm,\n",
+                "    scale=scale\n",
+                ")\n",
+                "# viewer.add_image(\n",
+                "#     soma_edges,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "# viewer.add_image(\n",
+                "#     composite_soma,\n",
+                "#     scale=scale\n",
+                "# )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### VISUALIZE final segmentations"
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 51,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer = napari.Viewer()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'NU_labels' at 0x1cf5b1d7cd0>"
+                            "<Image layer '_log_soma' at 0x25e437e2d90>"
                         ]
                     },
-                    "execution_count": 52,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "def _non_linear_soma_transform_MCZ(in_img):\n",
+                "    \"\"\" non-linear distortion to fill out cellmask\n",
+                "    log + edge of smoothed composite\n",
+                "    \"\"\"\n",
+                "    # non-Linear processing\n",
+                "    log_img, d = log_transform(in_img.copy()) \n",
+                "    return intensity_normalization(log_img,scaling_param=[0])\n",
+                "    # return intensity_normalization(filters.difference_of_gaussians(log_img, 2),scaling_param=[0])  + log_img\n",
+                "\n",
+                "_log_soma = _non_linear_soma_transform_MCZ(soma_guas)\n",
+                "\n",
                 "viewer.add_image(\n",
-                "    NU_signal,\n",
-                "    scale=scale,\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    nuclei_object,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n",
-                "viewer.add_labels(\n",
-                "    NU_labels,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 53,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "viewer.close()"
+                "    _log_soma,\n",
+                "    scale=scale\n",
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## DEFINE `_infer_nuclei` function\n",
-                "\n",
-                "Based on the _prototyping_ above define the function to infer nuclei.  \n"
+                "<code style=\"background:yellow;color:black\">Eventually this will be replaced by calling the un-name mangled version of the infer nuclei code that will be in infer-subc.organelles.</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 58,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
-                "##########################\n",
-                "#  _infer_nuclei\n",
-                "##########################\n",
+                "################# part 2 Nuclei pre-process\n",
                 "def _infer_nuclei_3D( in_img: np.ndarray,\n",
                 "                       median_sz: int, \n",
                 "                       gauss_sig: float,\n",
                 "                       thresh_factor: float,\n",
                 "                       thresh_min: float,\n",
                 "                       thresh_max: float,\n",
                 "                       max_hole_w: int,\n",
@@ -688,34 +577,17 @@
                 "\n",
                 "    nuclei_object = size_filter(nuclei_object, \n",
                 "                                min_size = small_obj_w**3, \n",
                 "                                method = sz_filter_method,\n",
                 "                                connectivity=1)\n",
                 "\n",
                 "\n",
-                "    return nuclei_object\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## DEFINE `_fixed_infer_nuclei` function\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 63,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "##########################\n",
-                "#  fixed_infer_nuclei\n",
-                "##########################\n",
+                "    return nuclei_object\n",
+                "\n",
+                "\n",
                 "def _fixed_infer_nuclei_3D(in_img: np.ndarray) -> np.ndarray:\n",
                 "    \"\"\"\n",
                 "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
@@ -744,258 +616,750 @@
                 "                             median_sz,\n",
                 "                             gauss_sig,\n",
                 "                             threshold_factor,\n",
                 "                             thresh_min,\n",
                 "                             thresh_max,\n",
                 "                             max_hole_w,\n",
                 "                             small_obj_w,\n",
-                "                             sz_filter_method )\n"
+                "                             sz_filter_method )\n",
+                "\n",
+                "\n",
+                "_NU_object =  _fixed_infer_nuclei_3D(img_data) \n",
+                "NU_labels = label(_NU_object)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "---------------------\n",
-                "## TEST `_infer_nuclei`  function defined above\n"
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 64,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
-                "_NU_object =  _fixed_infer_nuclei_3D(img_data) "
+                "\n",
+                "def _masked_object_thresh(\n",
+                "    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float\n",
+                ") -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    wrapper for applying Masked Object Thresholding with just two parameters via `MO` from `aicssegmentation`\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    structure_img_smooth: np.ndarray\n",
+                "        a 3d image\n",
+                "    th_method: \n",
+                "         which method to use for calculating global threshold. Options include:\n",
+                "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
+                "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
+                "    cutoff_size: \n",
+                "        Masked Object threshold `size_min`\n",
+                "    th_adjust: \n",
+                "        Masked Object threshold `local_adjust`\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "        np.ndimage \n",
+                "\n",
+                "    \"\"\"\n",
+                "\n",
+                "    struct_obj = MO(\n",
+                "        structure_img_smooth,\n",
+                "        global_thresh_method=th_method,\n",
+                "        object_minArea=cutoff_size,\n",
+                "        extra_criteria=True,\n",
+                "        local_adjust=th_adjust,\n",
+                "        return_object=False,\n",
+                "        dilate=True,\n",
+                "    )\n",
+                "    return struct_obj\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## CORE PROCESSING"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 68,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
-                "viewer = napari.Viewer()\n"
+                "###################\n",
+                "# CORE_PROCESSING\n",
+                "###################\n",
+                "low_level_min_size =  50\n",
+                "\n",
+                "# ################# part 1\n",
+                "soma_binary = _masked_object_thresh(soma_log_norm, \n",
+                "                           th_method='ave', \n",
+                "                           cutoff_size=low_level_min_size, \n",
+                "                           th_adjust= 0.15)                                           "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 69,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_NU_object' at 0x1cf9214fa60>"
+                            "<Image layer 'soma_binary' at 0x25e438999d0>"
                         ]
                     },
-                    "execution_count": 69,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    NU_signal,\n",
-                "    scale=scale,\n",
+                "    soma_binary,\n",
+                "    scale=scale\n",
+                ")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## POST-PROCESSING\n",
+                "\n",
+                "<code style=\"background:yellow;color:black\">Watershed (with or without the nuclei as a marker) does not work well here to get an instance segmentation</code>"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "###################\n",
+                "# POST_PROCESSING\n",
+                "###################\n",
+                "hole_width = 100\n",
+                "removed_holes = hole_filling(soma_binary, \n",
+                "                            hole_min=0, \n",
+                "                            hole_max=hole_width**2,\n",
+                "                            fill_2d = True) \n",
+                "\n",
+                "\n",
+                "small_object_width = 45\n",
+                "cleaned_img = size_filter_2D(removed_holes, \n",
+                "                             min_size= small_object_width**3, \n",
+                "                             connectivity=1)\n",
+                "\n",
+                "\n",
+                "watershed_mask = cleaned_img \n",
+                "inverted_img = 1. - cleaned_img\n",
+                "\n",
+                "labels_out = watershed(\n",
+                "            inverted_img,\n",
+                "            markers=NU_labels,\n",
+                "            connectivity= 3, # np.ones((1,3,3), bool),\n",
+                "            mask=watershed_mask,\n",
+                "            )"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Labels layer 'labels_out' at 0x25e52d71a60>"
+                        ]
+                    },
+                    "execution_count": 17,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "viewer.add_image(\n",
+                "    removed_holes,\n",
+                "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    nuclei_object,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n",
-                "viewer.add_labels(\n",
-                "    NU_labels,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
+                "    cleaned_img,\n",
+                "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    _NU_object,\n",
+                "    inverted_img,\n",
+                "    scale=scale\n",
+                ")\n",
+                "viewer.add_labels(\n",
+                "    labels_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 70,
+            "execution_count": 19,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Labels layer '_labels_out [1]' at 0x25e43b8f550>"
+                        ]
+                    },
+                    "execution_count": 19,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "viewer.close()"
+                "def _masked_inverted_watershed(img_in, markers, mask):\n",
+                "    \"\"\"wrapper for watershed on inverted image and masked\n",
+                "\n",
+                "    \"\"\"\n",
+                "    labels_out = watershed(\n",
+                "                1. - img_in,\n",
+                "                markers=markers,\n",
+                "                connectivity=3,\n",
+                "                mask=mask,\n",
+                "                )\n",
+                "    return labels_out\n",
+                "\n",
+                "\n",
+                "_labels_out = _masked_inverted_watershed(cleaned_img, NU_labels, cleaned_img)\n",
+                "\n",
+                "viewer.add_labels(\n",
+                "    _labels_out,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>\n",
+                "## POST POST-PROCESSING\n",
                 "\n",
-                "---------------------\n",
-                "# TEST `infer_nuclei_fromlabel` exported functions\n",
+                "<code style=\"background:yellow;color:black\">This should eventually be altered to maintain all cells that have the correct number of organelle markers</code>\n",
                 "\n",
-                "> the prototype `_infer_nuclei` was copied to the [`.organelles.nuclei`](../infer_subc/organelles/nuclei.py) sub-module \n",
-                "##\n",
-                "`infer_nuclei_fromlabel` procedure\n",
+                "What is we used the nuclei (or an expanded nuclei) to select the cells with the most signal, then after selecting the nuclei with signal, use those as the watershed marker - I think it may resolve some conflicts, but not all"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 20,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'soma_out' at 0x25e52975190>"
+                        ]
+                    },
+                    "execution_count": 20,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "###################\n",
+                "# POST- POST_PROCESSING\n",
+                "###################\n",
+                "# keep the \"SOMA\" label which contains the highest total signal\n",
+                "all_labels = np.unique(labels_out)[1:]\n",
+                "\n",
+                "total_signal = [soma_norm[labels_out == label].sum() for label in all_labels]\n",
+                "keep_label = all_labels[np.argmax(total_signal)]\n",
+                "keep_label\n",
                 "\n",
-                "Use the `infer_nuclei_fromlabel` function to infer the Nucleus and export it as an _ome.tif_ for easy reference."
+                "soma_out = np.zeros_like(labels_out)\n",
+                "soma_out[labels_out==keep_label] = 1\n",
+                "\n",
+                "viewer.add_image(\n",
+                "    soma_out,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 21,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer '_soma_out' at 0x25e43926160>"
+                        ]
+                    },
+                    "execution_count": 21,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "from infer_subc.organelles.nuclei import infer_nuclei_fromlabel, fixed_infer_nuclei\n",
+                "def _choose_max_label(raw_signal: np.ndarray, labels_in: np.ndarray):\n",
+                "    \"\"\" keep only the label with the maximum raw signal\n",
                 "\n",
-                "nuclei_object =  fixed_infer_nuclei(img_2D, soma_mask) \n"
+                "    \"\"\"\n",
+                "\n",
+                "    all_labels = np.unique(labels_in)[1:]\n",
+                "\n",
+                "    total_signal = [raw_signal[labels_in == label].sum() for label in all_labels]\n",
+                "    # combine NU and \"labels\" to make a SOMA\n",
+                "    keep_label = all_labels[np.argmax(total_signal)]\n",
+                "\n",
+                "    labels_max = np.zeros_like(labels_in)\n",
+                "    labels_max[labels_in==keep_label] = 1\n",
+                "    return labels_max\n",
+                "\n",
+                "_soma_out = _choose_max_label(soma_norm,labels_out)\n",
+                "\n",
+                "viewer.add_image(\n",
+                "    _soma_out,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Visualize  2\n"
+                "\n",
+                "\n",
+                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "viewer.add_image(\n",
-                "    _NU_object,\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n",
+                "## DEFINE parameterized  `_infer_cellmask_fromaggr` function\n",
                 "\n",
-                "\n",
-                "viewer.add_labels(\n",
-                "    label(_NU_object),\n",
-                "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")\n"
+                "A function to infer_cellmask_fromaggr from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
+                "-  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 37,
             "metadata": {},
             "outputs": [],
             "source": [
-                "viewer.add_image(\n",
-                "    nuclei_object,\n",
+                "##########################\n",
+                "# 1. infer_cellmask_fromaggr\n",
+                "##########################\n",
+                "\n",
+                "def _infer_cellmask_fromaggr_3D(in_img: np.ndarray,\n",
+                "    nuclei_labels: np.ndarray,\n",
+                "    median_sz_soma: int,\n",
+                "    gauss_sig_soma: float,\n",
+                "    gauss_truc_rang: float,\n",
+                "    mo_method: str,\n",
+                "    mo_adjust: float,\n",
+                "    mo_cutoff_size: int,\n",
+                "    max_hole_w_soma: int,\n",
+                "    small_obj_w_soma: int\n",
+                ") -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input.\n",
+                "\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    in_img: \n",
+                "        a 3d image containing all the channels\n",
+                "    nuclei_labels:\n",
+                "        a 3d mask of nuclei\n",
+                "    median_sz_soma: \n",
+                "        width of median filter for _soma_ signal\n",
+                "    gauss_sig_soma: \n",
+                "        sigma for gaussian smoothing of _soma_ signal\n",
+                "    gauss_truc_rang:\n",
+                "        cutoff value for gaussian\n",
+                "    mo_method: \n",
+                "         which method to use for calculating global threshold. Options include:\n",
+                "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
+                "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
+                "    mo_adjust: \n",
+                "        Masked Object threshold `local_adjust`\n",
+                "    mo_cutoff_size: \n",
+                "        Masked Object threshold `size_min`\n",
+                "    max_hole_w_soma: \n",
+                "        hole filling cutoff for cellmask signal post-processing\n",
+                "    small_obj_w_soma: \n",
+                "        minimu object size cutoff for cellmask signal post-processing\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "    soma_mask:\n",
+                "        a logical/labels object defining boundaries of cellmask\n",
+                "\n",
+                "    \"\"\"\n",
+                "\n",
+                "    ###################\n",
+                "    # EXTRACT\n",
+                "    ###################\n",
+                "    struct_img = _raw_soma_MCZ(in_img)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
+                "    scale=scale,\n",
+                "    name=1\n",
+                "    )\n",
+                "\n",
+                "\n",
+                "    ###################\n",
+                "    # PRE_PROCESSING\n",
+                "    ###################                         \n",
+                "    ################# part 1- cellmask\n",
+                "    struct_img = min_max_intensity_normalization(struct_img)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
+                "    scale=scale,\n",
+                "    name=2\n",
+                "    )\n",
+                "\n",
+                "    # make a copy for post-post processing\n",
+                "    scaled_signal = struct_img.copy()\n",
+                "\n",
+                "    # Linear-ish processing\n",
+                "    struct_img = median_filter_slice_by_slice(struct_img, \n",
+                "                                              size=median_sz_soma)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
+                "    scale=scale,\n",
+                "    name=3\n",
+                "    )\n",
+                "\n",
+                "    struct_img = ndi.gaussian_filter(struct_img,\n",
+                "                                     sigma=gauss_sig_soma,\n",
+                "                                     mode=\"nearest\",\n",
+                "                                     truncate=gauss_truc_rang)\n",
+                "    viewer.add_image(\n",
+                "    struct_img,\n",
+                "    scale=scale,\n",
+                "    name=4\n",
+                "    )\n",
+                "\n",
+                "\n",
+                "    # struct_img_non_lin, d = log_transform(struct_img)\n",
+                "    # struct_img_non_lin = intensity_normalization(struct_img_non_lin, scaling_param=[0])\n",
+                "    struct_img_non_lin = _non_linear_soma_transform_MCZ(struct_img)\n",
+                "    viewer.add_image(\n",
+                "    struct_img_non_lin,\n",
+                "    scale=scale,\n",
+                "    name=5\n",
+                "    )\n",
+                "   \n",
+                "    ###################\n",
+                "    # CORE_PROCESSING\n",
+                "    ###################    \n",
+                "    struct_obj = _masked_object_thresh(struct_img_non_lin, \n",
+                "                                       th_method=mo_method, \n",
+                "                                       cutoff_size=mo_cutoff_size, \n",
+                "                                       th_adjust=mo_adjust)               \n",
+                "    viewer.add_image(\n",
+                "    struct_obj,\n",
+                "    scale=scale,\n",
+                "    name=6\n",
+                "    )\n",
+                "\n",
+                "    ###################\n",
+                "    # POST_PROCESSING\n",
+                "    ###################\n",
+                "    struct_obj = hole_filling(struct_obj, \n",
+                "                              hole_min =0 , \n",
+                "                              hole_max=max_hole_w_soma**2, \n",
+                "                              fill_2d = True) \n",
+                "    viewer.add_image(\n",
+                "    struct_obj,\n",
+                "    scale=scale,\n",
+                "    name=7\n",
+                "    )\n",
+                "\n",
+                "    struct_obj = size_filter_2D(struct_obj, \n",
+                "                                min_size= small_obj_w_soma**3, \n",
+                "                                connectivity=1)\n",
+                "    viewer.add_image(\n",
+                "    struct_obj,\n",
                 "    scale=scale,\n",
-                "    opacity=0.3,\n",
-                ")    \n"
+                "    name=8\n",
+                "    )\n",
+                "\n",
+                "    labels_out = _masked_inverted_watershed(struct_obj, nuclei_labels, struct_obj)\n",
+                "    viewer.add_image(\n",
+                "    labels_out,\n",
+                "    scale=scale,\n",
+                "    name=9\n",
+                "    )\n",
+                "\n",
+                "    ###################\n",
+                "    # POST- POST_PROCESSING\n",
+                "    ###################\n",
+                "    # keep the \"SOMA\" label which contains the highest total signal\n",
+                "    soma_out = _choose_max_label(struct_img, labels_out)\n",
+                "\n",
+                "    return soma_out\n",
+                "\n",
+                "\n"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "from napari.utils.notebook_display import nbscreenshot\n",
+                "## DEFINE `_fixed_infer_cellmask_fromaggr` function\n",
                 "\n",
-                "# viewer.dims.ndisplay = 3\n",
-                "# viewer.camera.angles = (-30, 25, 120)\n",
-                "nbscreenshot(viewer, canvas_only=True)\n"
+                "Based on the _prototyping_ above define the function to infer cellmask. with a *fixed* set of parameters for each step in the procedure.  That is they are all \"hard coded\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 34,
             "metadata": {},
             "outputs": [],
             "source": [
-                "viewer.close()"
+                "##########################\n",
+                "# 1. fixed_infer_cellmask_fromaggr\n",
+                "##########################\n",
+                "\n",
+                "\n",
+                "def _fixed_infer_cellmask_fromaggr_3D(in_img: np.ndarray, nuclei_labels: np.ndarray) -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
+                "\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    in_img: \n",
+                "        a 3d image containing all the channels\n",
+                "    nuclei_object:\n",
+                "        a 3d mask of nuclei\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "    soma_mask:\n",
+                "        a logical/labels object defining boundaries of cellmask\n",
+                "    \"\"\"\n",
+                "    \n",
+                "\n",
+                "    ###################\n",
+                "    # PARAMETERS\n",
+                "    ###################   \n",
+                "    median_sz_soma = 15\n",
+                "    gauss_sig_soma = 1.34\n",
+                "    gauss_truc_rang = 3.0\n",
+                "    mo_method = \"ave\"\n",
+                "    mo_adjust = 0.15\n",
+                "    mo_cutoff_size = 50\n",
+                "    max_hole_w_soma = 100\n",
+                "    small_obj_w_soma = 45\n",
+                "\n",
+                "    soma_out = _infer_cellmask_fromaggr_3D(in_img,\n",
+                "                              nuclei_labels,\n",
+                "                              median_sz_soma,\n",
+                "                              gauss_sig_soma,\n",
+                "                              gauss_truc_rang,\n",
+                "                              mo_method,\n",
+                "                              mo_adjust,\n",
+                "                              mo_cutoff_size,\n",
+                "                              max_hole_w_soma,\n",
+                "                              small_obj_w_soma) \n",
+                "\n",
+                "    return soma_out\n",
+                "\n",
+                "\n"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 38,
             "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                }
+            ],
             "source": [
-                "-----------------\n",
-                "Write the `infer_nuclei_fromlabel` spec to the widget json "
+                "\n",
+                "SO_label =  _fixed_infer_cellmask_fromaggr_3D(img_data, NU_labels) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 39,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'name': 'infer nuclei  (fixed parameters)',\n",
-                            " 'python::module': 'infer_subc.organelles',\n",
-                            " 'python::function': 'fixed_infer_nuclei',\n",
-                            " 'parameters': None}"
+                            "<Image layer 'SO_label [1]' at 0x25ea42fd970>"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 39,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
+                "viewer.add_image(\n",
+                "    SO_label,\n",
+                "    scale=scale\n",
+                ")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "---------------------\n",
+                "# TEST `_infer_cellmask_fromaggr`  function defined above\n",
                 "\n",
-                "_fixed_infer_nuclei =  {\n",
-                "        \"name\": \"infer nuclei  (fixed parameters)\",\n",
-                "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"fixed_infer_nuclei\",\n",
-                "        \"parameters\": None\n",
-                "        }\n",
+                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>\n",
+                "##\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from infer_subc.organelles import fixed_infer_cellmask_fromaggr, infer_cellmask_fromaggr\n",
                 "\n",
-                "_fixed_infer_nuclei"
+                "soma_ =  fixed_infer_cellmask_fromaggr(img_2D) "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "viewer.add_image(\n",
+                "    SO_label,\n",
+                "    scale=scale\n",
+                ")\n",
+                "viewer.add_image(\n",
+                "    soma_,\n",
+                "    scale=scale \n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Write the `infer_cellmask_fromaggr` spec to the widget json"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"fixed_infer_nuclei\",_fixed_infer_nuclei)"
+                "_fixed_infer_cellmask_fromaggr =  {\n",
+                "        \"name\": \" infer cellmask mask (fixed parameters)\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"fixed_infer_cellmask_fromaggr\",\n",
+                "        \"parameters\": None\n",
+                "        }\n",
+                "\n",
+                "add_function_spec_to_widget_json(\"fixed_infer_cellmask_fromaggr\", _fixed_infer_cellmask_fromaggr, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "_infer_nuclei =  {\n",
-                "        \"name\": \"infer nuclei\",\n",
+                "_infer_cellmask_fromaggr =  {\n",
+                "        \"name\": \" infer cellmask mask\",\n",
                 "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_nuclei_fromlabel\",\n",
+                "        \"python::function\": \"infer_cellmask_fromaggr\",\n",
                 "        \"parameters\": {\n",
-                "                \"median_sz\": {\n",
+                "                \"median_sz_soma\": {\n",
                 "                        \"widget_type\": \"slider\",\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"min\": 3,\n",
                 "                        \"max\": 15,\n",
                 "                        \"increment\": 1\n",
                 "                },\n",
-                "                \"gauss_sig\": {\n",
+                "                \"gauss_sig_soma\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.25,\n",
                 "                        \"max\": 15.0,\n",
                 "                        \"min\": 1.25,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
+                "                \"median_sz_nuc\": {\n",
+                "                        \"widget_type\": \"slider\",\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"min\": 3,\n",
+                "                        \"max\": 15,\n",
+                "                        \"increment\": 1\n",
+                "                },\n",
+                "                \"gauss_sig_nuc\": {\n",
+                "                        \"data_type\": \"float\",\n",
+                "                        \"increment\": 0.25,\n",
+                "                        \"max\": 15.0,\n",
+                "                        \"min\": 1.25,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },\n",
+                "                \"mo_method\": {\n",
+                "                        \"data_type\": \"str\",\n",
+                "                        \"widget_type\": \"drop-down\",\n",
+                "                        \"options\": [\n",
+                "                                \"triangle\",\n",
+                "                                \"median\",\n",
+                "                                \"ave_tri_med\"\n",
+                "                                ]\n",
+                "                },\n",
+                "                \"mo_adjust\": {\n",
+                "                        \"data_type\": \"float\",\n",
+                "                        \"increment\": 0.05,\n",
+                "                        \"max\": 1.0,\n",
+                "                        \"min\": 0.0,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },\n",
+                "                \"mo_cutoff_size\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"increment\": 10,\n",
+                "                        \"max\": 250,\n",
+                "                        \"min\": 10,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },\n",
                 "                \"thresh_factor\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.05,\n",
                 "                        \"max\": 1.2,\n",
                 "                        \"min\": 0.6,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
@@ -1009,329 +1373,402 @@
                 "                \"thresh_max\": {\n",
                 "                        \"data_type\": \"float\",\n",
                 "                        \"increment\": 0.05,\n",
                 "                        \"max\": 1.0,\n",
                 "                        \"min\": 0.1,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },\n",
-                "                \"max_hole_w\": {\n",
+                "                \"max_hole_w_nuc\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 1,\n",
                 "                        \"max\": 40,\n",
                 "                        \"min\": 4,\n",
                 "                        \"widget_type\": \"slider\"\n",
                 "                },           \n",
-                "                \"small_obj_w\": {\n",
+                "                \"small_obj_w_nuc\": {\n",
                 "                        \"data_type\": \"int\",\n",
                 "                        \"increment\": 1,\n",
                 "                        \"max\": 50,\n",
                 "                        \"min\": 1,\n",
                 "                        \"widget_type\": \"slider\"\n",
-                "                }\n",
+                "                },                           \n",
+                "                \"max_hole_w_soma\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"increment\": 2,\n",
+                "                        \"max\": 100,\n",
+                "                        \"min\": 20,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },           \n",
+                "                \"small_obj_w_soma\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"increment\": 1,\n",
+                "                        \"max\": 50,\n",
+                "                        \"min\": 1,\n",
+                "                        \"widget_type\": \"slider\"\n",
+                "                },        \n",
                 "        }\n",
                 "}\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"infer_nuclei_fromlabel\", _infer_nuclei, overwrite=True )\n",
+                "add_function_spec_to_widget_json(\"infer_cellmask_fromaggr\", _infer_cellmask_fromaggr, overwrite=True )\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "_median_filter_slice_by_slice =  {\n",
-                "                \"name\": \"Median Smoothing Slice by Slice\",\n",
-                "                \"python::module\": \"infer_subc.core.img\",\n",
-                "                \"python::function\": \"median_filter_slice_by_slice\",\n",
-                "                \"parameters\": {\n",
-                "                    \"size\": {\n",
-                "                        \"widget_type\": \"slider\",\n",
-                "                        \"data_type\": \"int\",\n",
-                "                        \"min\": 1,\n",
-                "                        \"max\": 20,\n",
-                "                        \"increment\": 1\n",
-                "                    }\n",
-                "                }\n",
-                "            } \n",
-                "add_function_spec_to_widget_json(\"median_filter_slice_by_slice\",_median_filter_slice_by_slice)"
+                "\n",
+                "_raw_soma_MCZ =  {\n",
+                "        \"name\": \"define weighted aggregate cellmask signal (MCZ-cellprofiler)\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"raw_soma_MCZ\",\n",
+                "        \"parameters\": None\n",
+                "        }\n",
+                "\n",
+                "add_function_spec_to_widget_json(\"raw_soma_MCZ\", _raw_soma_MCZ, overwrite=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "\n",
-                "_image_smoothing_gaussian_slice_by_slice = {\n",
-                "        \"name\": \"Gaussian Smoothing Slice by Slice\",\n",
-                "        \"python::module\": \"aicssegmentation.core.pre_processing_utils\",\n",
-                "        \"python::function\": \"image_smoothing_gaussian_slice_by_slice\",\n",
-                "        \"parameters\": {\n",
-                "            \"sigma\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.8,\n",
-                "                \"max\": 20,\n",
-                "                \"increment\": 0.2\n",
-                "            }\n",
-                "        }\n",
+                "_non_linear_soma_transform_MCZ =  {\n",
+                "        \"name\": \"non-linear filter of cellmask signal (MCZ-cellprofiler)\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"non_linear_soma_transform_MCZ\",\n",
+                "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "# json.dumps({\"image_smoothing_gaussian_slice_by_slice\": _image_smoothing_gaussian_slice_by_slice} )\n",
-                "add_function_spec_to_widget_json(\"image_smoothing_gaussian_slice_by_slice\",_image_smoothing_gaussian_slice_by_slice)        \n"
+                "add_function_spec_to_widget_json(\"non_linear_soma_transform_MCZ\", _non_linear_soma_transform_MCZ)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "# WARNING: not a good way to set to None\n",
-                "_apply_log_li_threshold = {\n",
-                "        \"name\": \"threshold log Li\",\n",
-                "        \"python::module\": \"infer_subc.core.img\",\n",
-                "        \"python::function\": \"apply_log_li_threshold\",\n",
-                "        \"parameters\": {\n",
-                "            \"thresh_factor\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.3,\n",
-                "                \"max\": 1.1,\n",
-                "                \"increment\": 0.05\n",
-                "            },\n",
-                "            \"thresh_min\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.0,\n",
-                "                \"max\": 0.8,\n",
-                "                \"increment\": 0.01\n",
-                "            },\n",
-                "            \"thresh_max\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"float\",\n",
-                "                \"min\": 0.3,\n",
-                "                \"max\": 1.0,\n",
-                "                \"increment\": 0.05\n",
-                "            },\n",
-                "        }\n",
+                "_masked_inverted_watershed =  {\n",
+                "        \"name\": \"watershed on inverted image and masked\",\n",
+                "        \"python::module\": \"infer_subc.organelles\",\n",
+                "        \"python::function\": \"masked_inverted_watershed\",\n",
+                "        \"parameters\": None\n",
                 "        }\n",
                 "\n",
-                "# json.dumps({\"apply_log_li_threshold\": _apply_log_li_threshold} )\n",
-                "add_function_spec_to_widget_json(\"apply_log_li_threshold\",_apply_log_li_threshold,overwrite=True)        \n"
+                "add_function_spec_to_widget_json(\"masked_inverted_watershed\", _masked_inverted_watershed)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "\n",
-                "    # NU_labels = label(nuclei_object)\n",
-                "\n",
-                "_label =  {\n",
-                "        \"name\": \"label objects\",\n",
-                "        \"python::module\": \"skimage.measure\",\n",
-                "        \"python::function\": \"label\",\n",
+                "_choose_max_label =  {\n",
+                "        \"name\": \"keep only the label with the maximum raw signa\",\n",
+                "        \"python::module\": \"infer_subc.core.img\",\n",
+                "        \"python::function\": \"choose_max_label\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
-                "# json.dumps({\"label\":_label})\n",
-                "add_function_spec_to_widget_json(\"label\",_label)        \n"
+                "\n",
+                "add_function_spec_to_widget_json(\"choose_max_label\", _choose_max_label)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
-                "#  nulei_object = apply_mask(nuclei_object, soma_mask)\n",
-                "\n",
-                "_apply_mask=  {\n",
-                "        \"name\": \"apply mask\",\n",
+                "_min_max_intensity_normalization =  {\n",
+                "        \"name\": \"Min Max Intesity Normalization\",\n",
                 "        \"python::module\": \"infer_subc.core.img\",\n",
-                "        \"python::function\": \"apply_mask\",\n",
+                "        \"python::function\": \"min_max_intensity_normalization\",\n",
                 "        \"parameters\": None\n",
                 "        }\n",
-                "# json.dumps({\"apply_mask\":_apply_mask})\n",
-                "add_function_spec_to_widget_json(\"apply_mask\",_apply_mask)        \n"
+                "\n",
+                "add_function_spec_to_widget_json(\"min_max_intensity_normalization\", _min_max_intensity_normalization)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
-                "    # small_object_width = 45\n",
-                "    # nuclei_object = size_filter_linear_size(nuclei_object, \n",
-                "    #                                                             min_size= small_object_width**2, \n",
-                "    #                                                             connectivity=1)\n",
-                "\n",
-                "\n",
-                "_size_filter_linear_size = {\n",
-                "        \"name\": \"Size Filter 2D\",\n",
+                "_masked_object_thresh =  {\n",
+                "        \"name\": \"Masked Object Threshold wrapper for widgets\",\n",
                 "        \"python::module\": \"infer_subc.core.img\",\n",
-                "        \"python::function\": \"size_filter_linear_size\",\n",
+                "        \"python::function\": \"masked_object_thresh\",\n",
                 "        \"parameters\": {\n",
-                "            \"min_size\": {\n",
-                "                \"widget_type\": \"slider\",\n",
-                "                \"data_type\": \"int\",\n",
-                "                \"min\": 0,\n",
-                "                \"max\": 500,\n",
-                "                \"increment\": 1\n",
-                "            }\n",
+                "                \"th_method\": {\n",
+                "                        \"data_type\": \"str\",\n",
+                "                        \"widget_type\": \"drop-down\",\n",
+                "                        \"options\": [\n",
+                "                        \"triangle\",\n",
+                "                        \"median\",\n",
+                "                        \"ave_tri_med\"\n",
+                "                        ]\n",
+                "                },\n",
+                "                \"cutoff_size\": {\n",
+                "                        \"data_type\": \"int\",\n",
+                "                        \"widget_type\": \"slider\",\n",
+                "                        \"min\": 0,\n",
+                "                        \"max\": 2000,\n",
+                "                        \"increment\": 50\n",
+                "                },\n",
+                "                \"th_adjust\": {\n",
+                "                        \"data_type\": \"float\",\n",
+                "                        \"widget_type\": \"slider\",\n",
+                "                        \"min\": 0,\n",
+                "                        \"max\": 2,\n",
+                "                        \"increment\": 0.02\n",
+                "                }\n",
                 "        }\n",
-                "    }\n",
-                "# json.dumps({  \"size_filter_linear_size\":  _size_filter_linear_size   })\n",
+                "}\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"size_filter_linear_size\",_size_filter_linear_size)        \n"
+                "add_function_spec_to_widget_json(\"masked_object_thresh\", _masked_object_thresh, overwrite=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "-------------------------------\n",
-                "## Write workflow .json\n",
-                "Now that we've added our function specs we can compose workflows."
+                "--------------------------\n",
+                "\n",
+                "# TEST `infer_cellmask_fromaggr` exported functions\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.constants import NUC_CH\n",
-                "\n",
+                "from infer_subc.organelles import fixed_infer_cellmask_fromaggr\n",
                 "\n",
-                "def make_infer_nuclei_dict():\n",
-                "    \"\"\"\n",
-                "    Procedure to infer nuclei from linearly unmixed input.\n",
+                "soma_mask =  fixed_infer_cellmask_fromaggr(img_2D) "
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Visualize  2\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# viewer = napari.Viewer()\n",
                 "\n",
-                "    Parameters\n",
-                "    ------------\n",
-                "    in_img: np.ndarray\n",
-                "        a 3d image containing all the channels\n",
+                "viewer.scale_bar.visible = True\n",
                 "\n",
-                "    soma_mask: np.ndarray\n",
-                "        mask\n",
+                "viewer.add_labels(\n",
+                "    soma_mask,\n",
+                "    scale=scale,\n",
+                "    blending='additive'\n",
+                ")\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "\n",
-                "    Returns\n",
-                "    -------------\n",
-                "    nuclei_object\n",
-                "        mask defined extent of NU\n",
+                "from napari.utils.notebook_display import nbscreenshot\n",
                 "\n",
+                "# viewer.dims.ndisplay = 3\n",
+                "# viewer.camera.angles = (-30, 25, 120)\n",
+                "nbscreenshot(viewer, canvas_only=True)\n",
+                "viewer.close()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "-------------------------------\n",
+                "## Write workflow .json\n",
+                "Now that we've added our function specs we can compose workflows."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def make_infer_cellmask_fromaggr_step_by_step_dict():\n",
+                "    \"\"\"\n",
+                "    crete .json version of infer_cellmask_fromaggr\n",
                 "    \"\"\"\n",
                 "    step_name = []\n",
                 "    function_name = []\n",
                 "    category =[]\n",
                 "    parameter_values = []\n",
                 "    parent = []\n",
-                "   \n",
+                "\n",
                 "    ###################\n",
                 "    # EXTRACT\n",
                 "    ###################   \n",
+                "    # struct_img = _raw_soma_MCZ(in_img)\n",
                 "    step_name.append(\"1\")\n",
+                "    function_name.append(\"raw_soma_MCZ\")\n",
+                "    category.append(\"extraction\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(0)\n",
+                "\n",
+                "    step_name.append(\"2\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( dict(chan = NUC_CH) )\n",
                 "    parent.append(0)\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
-                "    ###################                         \n",
-                "    # nuclei = min_max_intensity_normalization(in_img[NUC_CH].copy() )\n",
-                "    step_name.append(\"2\")\n",
+                "    ###################\n",
+                "    #SOMA\n",
+                "    step_name.append(\"3\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(1)\n",
                 "\n",
-                "    # size = 4   \n",
-                "    # nuclei = median_filter_slice_by_slice( \n",
-                "    #                                                                 nuclei,\n",
-                "    #                                                                 size=size  )\n",
-                "    step_name.append(\"3\")\n",
+                "\n",
+                "    step_name.append(\"4\")\n",
                 "    function_name.append(\"median_filter_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parameter_values.append(dict(size = 15 ))\n",
+                "    parent.append(3)\n",
+                "\n",
+                "\n",
+                "    step_name.append(\"5\")\n",
+                "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
+                "    parent.append(4)\n",
+                "\n",
+                "    step_name.append(\"6\")\n",
+                "    function_name.append(\"non_linear_soma_transform_MCZ\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(5)\n",
+                "\n",
+                "    #NUC\n",
+                "    step_name.append(\"7\")\n",
+                "    function_name.append(\"min_max_intensity_normalization\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
                 "    parent.append(2)\n",
                 "\n",
-                "    # sigma = 1.34\n",
-                "    # truncate_range = 3.0\n",
-                "    # nuclei = image_smoothing_gaussian_slice_by_slice(  nuclei,\n",
-                "    #                                                                                             sigma=sigma,\n",
-                "    #                                                                                             truncate_range = truncate_range\n",
-                "    #                                                                                             )\n",
-                "    step_name.append(\"4\")\n",
+                "    step_name.append(\"8\")\n",
+                "    function_name.append(\"median_filter_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parent.append(7)\n",
+                "\n",
+                "    step_name.append(\"9\")\n",
                 "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict( sigma = 1.34 ))\n",
-                "    parent.append(3)\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
+                "    parent.append(8)\n",
                 "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    # threshold_factor = 0.9 \n",
-                "    # thresh_min = .1\n",
-                "    # thresh_max = 1.\n",
-                "    # nuclei_object = apply_log_li_threshold(nuclei, threshold_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "    step_name.append(\"5\")\n",
+                "    # SOMA\n",
+                "    step_name.append(\"10\")\n",
+                "    function_name.append(\"masked_object_thresh\")\n",
+                "    category.append(\"core\")\n",
+                "    parameter_values.append(dict( th_method=\"ave_tri_med\",\n",
+                "                                                            cutoff_size = 100,\n",
+                "                                                            th_adjust = 0.5))\n",
+                "    parent.append(6)\n",
+                "\n",
+                "\n",
+                "    # NUCLEI\n",
+                "    step_name.append(\"11\")\n",
                 "    function_name.append(\"apply_log_li_threshold\")\n",
                 "    category.append(\"core\")\n",
                 "    parameter_values.append(dict(thresh_factor = 0.9, \n",
                 "                                                            thresh_min = .1,\n",
                 "                                                            thresh_max = 1.))\n",
-                "    parent.append(4)\n",
-                "\n",
-                "\n",
-                "    # NU_labels = label(nuclei_object)\n",
-                "    step_name.append(\"6\")\n",
-                "    function_name.append(\"label\")\n",
-                "    category.append(\"core\")\n",
-                "    parameter_values.append(None)\n",
-                "    parent.append(5)\n",
+                "    parent.append(9)\n",
                 "\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
-                "    # hole_width = 5  \n",
-                "    # nuclei_object = hole_filling(nuclei_object, hole_min=0, hole_max=hole_width**2, fill_2d=True)\n",
-                "    step_name.append(\"6\")\n",
+                "    # NUCLEI\n",
+                "    step_name.append(\"12\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
-                "    parent.append(5)\n",
+                "    parent.append(11)\n",
                 "\n",
-                "    # # EEEEEK I don't know how to compose where the mask comes from... \n",
-                "    # nuclei_object = apply_mask(nuclei_object, soma_mask)\n",
+                "    step_name.append(\"13\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( min_size = 15**2  ))\n",
+                "    parent.append(12)\n",
                 "\n",
-                "    # small_object_width = 15\n",
-                "    # nuclei_object = size_filter_linear_size(nuclei_object, \n",
-                "    #                                                             min_size= small_object_width**2, \n",
-                "    #                                                             connectivity=1)\n",
-                "    step_name.append(\"7\")\n",
-                "    function_name.append(\"size_filter_linear_size\")\n",
+                "    step_name.append(\"14\")\n",
+                "    function_name.append(\"label\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(13)\n",
+                "\n",
+                "    # SOMA\n",
+                "    step_name.append(\"15\")\n",
+                "    function_name.append(\"hole_filling\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
+                "    parent.append(10)\n",
+                "\n",
+                "    step_name.append(\"16\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
-                "    parent.append(6)\n",
+                "    parent.append(15)\n",
+                "\n",
+                "    step_name.append(\"17\")\n",
+                "    function_name.append(\"masked_inverted_watershed\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([ 5 , 14, 16])\n",
                 "\n",
+                "    ###################\n",
+                "    # POST- POST_PROCESSING\n",
+                "    ###################\n",
+                "    # keep the \"SOMA\" label which contains the highest total signal\n",
+                "    step_name.append(\"18\")\n",
+                "    function_name.append(\"choose_max_label\")\n",
+                "    category.append(\"postpostprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([5, 17])\n",
+                "\n",
+                "    ##########################\n",
                 "    out_dict = dict()\n",
                 "    for i,stepn in enumerate(step_name):\n",
                 "        entry = dict(category=category[i],\n",
                 "                            function=function_name[i],\n",
                 "                            parameter_values=parameter_values[i],\n",
                 "                            parent=parent[i]\n",
                 "        )\n",
@@ -1344,56 +1781,28 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.utils.directories import Directories\n",
-                "import json\n",
-                "\n",
-                "def _write_workflow_json(wf_name, wf_dict):\n",
-                "\n",
-                "    # read all_functions.json into dict\n",
-                "    # if not wf_name.startswith(\"conf\"):\n",
-                "    #     wf_name = f\"conf_{wf_name}\"\n",
-                "    path = Directories.get_structure_config_dir() / f\"{wf_name}.json\"\n",
-                "\n",
-                "    # re-write file\n",
-                "    with open(path, \"w\") as file:\n",
-                "        json.dump(wf_dict, file, indent=4, sort_keys=False)\n",
-                "\n",
-                "    return path\n",
-                "\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "from infer_subc.organelles_config.helper import write_workflow_json\n",
                 "\n",
-                "infer_nuclei_dict = make_infer_nuclei_dict()\n",
+                "infer_cellmask_fromaggr_stepbystep_dict = make_infer_cellmask_fromaggr_step_by_step_dict()\n",
                 "\n",
-                "write_workflow_json(\"conf_2.2.nuclei_stepbystep\", infer_nuclei_dict)"
+                "write_workflow_json(\"conf_2.1.soma_stepbystep\", infer_cellmask_fromaggr_stepbystep_dict )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.constants import NUC_CH\n",
-                "\n",
-                "\n",
-                "def make_infer_nuclei_from_raw_dict():\n",
+                "def make_infer_cellmask_fromaggr_step_by_step_from_raw_dict():\n",
                 "    \"\"\"\n",
                 "    Procedure to infer nuclei from linearly unmixed input.\n",
                 "\n",
                 "    Parameters\n",
                 "    ------------\n",
                 "    in_img: np.ndarray\n",
                 "        a 3d image containing all the channels\n",
@@ -1408,122 +1817,159 @@
                 "\n",
                 "    \"\"\"\n",
                 "    step_name = []\n",
                 "    function_name = []\n",
                 "    category =[]\n",
                 "    parameter_values = []\n",
                 "    parent = []\n",
-                "   \n",
+                "\n",
                 "    ###################\n",
                 "    # EXTRACT\n",
                 "    ###################   \n",
-                "\n",
                 "    step_name.append(\"1\")\n",
                 "    function_name.append(\"fixed_get_optimal_Z_img\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append(None)\n",
                 "    parent.append(0)\n",
                 "\n",
-                "\n",
+                "    # SOMA\n",
                 "    step_name.append(\"2\")\n",
-                "    function_name.append(\"fixed_infer_cellmask_fromaggr\")\n",
+                "    function_name.append(\"raw_soma_MCZ\")\n",
                 "    category.append(\"extraction\")\n",
-                "    parameter_values.append( None )\n",
+                "    parameter_values.append(None)\n",
                 "    parent.append(1)\n",
                 "\n",
+                "    # NUC\n",
                 "    step_name.append(\"3\")\n",
                 "    function_name.append(\"select_channel_from_raw\")\n",
                 "    category.append(\"extraction\")\n",
                 "    parameter_values.append( dict(chan = NUC_CH) )\n",
                 "    parent.append(1)\n",
                 "\n",
                 "    ###################\n",
                 "    # PRE_PROCESSING\n",
-                "    ###################                         \n",
-                "    # nuclei = min_max_intensity_normalization(in_img[NUC_CH].copy() )\n",
+                "    ###################\n",
+                "    # SOMA\n",
                 "    step_name.append(\"4\")\n",
                 "    function_name.append(\"min_max_intensity_normalization\")\n",
                 "    category.append(\"preprocessing\")\n",
                 "    parameter_values.append(None)\n",
-                "    parent.append(3)\n",
+                "    parent.append(2)\n",
                 "\n",
-                "    # size = 4   \n",
-                "    # nuclei = median_filter_slice_by_slice( \n",
-                "    #                                                                 nuclei,\n",
-                "    #                                                                 size=size  )\n",
                 "    step_name.append(\"5\")\n",
                 "    function_name.append(\"median_filter_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parameter_values.append(dict(size = 15 ))\n",
                 "    parent.append(4)\n",
                 "\n",
-                "    # sigma = 1.34\n",
-                "    # truncate_range = 3.0\n",
-                "    # nuclei = image_smoothing_gaussian_slice_by_slice(  nuclei,\n",
-                "    #                                                                                             sigma=sigma,\n",
-                "    #                                                                                             truncate_range = truncate_range\n",
-                "    #                                                                                             )\n",
                 "    step_name.append(\"6\")\n",
                 "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
                 "    category.append(\"preprocessing\")\n",
-                "    parameter_values.append(dict( sigma = 1.34 ))\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
                 "    parent.append(5)\n",
                 "\n",
+                "    step_name.append(\"7\")\n",
+                "    function_name.append(\"non_linear_soma_transform_MCZ\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(6)\n",
+                "\n",
+                "    #NUC\n",
+                "    step_name.append(\"8\")\n",
+                "    function_name.append(\"min_max_intensity_normalization\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append(3)\n",
+                "\n",
+                "    step_name.append(\"9\")\n",
+                "    function_name.append(\"median_filter_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict(size = 4 ))\n",
+                "    parent.append(8)\n",
+                "\n",
+                "    step_name.append(\"10\")\n",
+                "    function_name.append(\"image_smoothing_gaussian_slice_by_slice\")\n",
+                "    category.append(\"preprocessing\")\n",
+                "    parameter_values.append(dict( sigma = 1.4 ))\n",
+                "    parent.append(9)\n",
+                "\n",
                 "    ###################\n",
                 "    # CORE_PROCESSING\n",
                 "    ###################\n",
-                "    # threshold_factor = 0.9 \n",
-                "    # thresh_min = .1\n",
-                "    # thresh_max = 1.\n",
-                "    # nuclei_object = apply_log_li_threshold(nuclei, threshold_factor=threshold_factor, thresh_min=thresh_min, thresh_max=thresh_max)\n",
-                "    step_name.append(\"7\")\n",
+                "    # SOMA\n",
+                "    step_name.append(\"11\")\n",
+                "    function_name.append(\"masked_object_thresh\")\n",
+                "    category.append(\"core\")\n",
+                "    parameter_values.append(dict( th_method=\"ave_tri_med\",\n",
+                "                                                            cutoff_size = 100,\n",
+                "                                                            th_adjust = 0.5))\n",
+                "    parent.append(7)\n",
+                "\n",
+                "    # NUC\n",
+                "    step_name.append(\"12\")\n",
                 "    function_name.append(\"apply_log_li_threshold\")\n",
                 "    category.append(\"core\")\n",
                 "    parameter_values.append(dict(thresh_factor = 0.9, \n",
                 "                                                            thresh_min = .1,\n",
                 "                                                            thresh_max = 1.))\n",
-                "    parent.append(6)\n",
-                "\n",
-                "\n",
-                "    # NU_labels = label(nuclei_object)\n",
-                "    step_name.append(\"8\")\n",
-                "    function_name.append(\"label\")\n",
-                "    category.append(\"core\")\n",
-                "    parameter_values.append(None)\n",
-                "    parent.append(7)\n",
-                "\n",
+                "    parent.append(10)\n",
                 "\n",
                 "    ###################\n",
                 "    # POST_PROCESSING\n",
                 "    ###################\n",
-                "    # hole_width = 5  \n",
-                "    # nuclei_object = hole_filling(nuclei_object, hole_min=0, hole_max=hole_width**2, fill_2d=True)\n",
-                "    step_name.append(\"9\")\n",
+                "    # nUC\n",
+                "    step_name.append(\"13\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
-                "    parent.append(8)\n",
+                "    parent.append(12)\n",
                 "\n",
-                "    step_name.append(\"10\")\n",
-                "    function_name.append(\"apply_mask\")\n",
+                "    step_name.append(\"14\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( min_size = 15**2  ))\n",
+                "    parent.append(13)\n",
+                "\n",
+                "    step_name.append(\"15\")\n",
+                "    function_name.append(\"label\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(None)\n",
-                "    parent.append([9,2])\n",
+                "    parent.append(14)\n",
                 "\n",
                 "\n",
-                "    # small_object_width = 15\n",
-                "    # nuclei_object = size_filter_linear_size(nuclei_object, \n",
-                "    #                                                             min_size= small_object_width**2, \n",
-                "    #                                                             connectivity=1)\n",
-                "    step_name.append(\"11\")\n",
-                "    function_name.append(\"size_filter_linear_size\")\n",
+                "    # SOMA\n",
+                "    step_name.append(\"16\")\n",
+                "    function_name.append(\"hole_filling\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
+                "    parent.append(11)\n",
+                "\n",
+                "    step_name.append(\"17\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
-                "    parent.append(10)\n",
+                "    parent.append(16)\n",
                 "\n",
+                "    step_name.append(\"18\")\n",
+                "    function_name.append(\"masked_inverted_watershed\")\n",
+                "    category.append(\"postprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([  7 , 15,17 ])\n",
+                "\n",
+                "    ###################\n",
+                "    # POST- POST_PROCESSING\n",
+                "    ###################\n",
+                "    # keep the \"SOMA\" label which contains the highest total signal\n",
+                "    step_name.append(\"19\")\n",
+                "    function_name.append(\"choose_max_label\")\n",
+                "    category.append(\"postpostprocessing\")\n",
+                "    parameter_values.append(None)\n",
+                "    parent.append([6,18])\n",
+                "\n",
+                "    ##########################\n",
                 "    out_dict = dict()\n",
                 "    for i,stepn in enumerate(step_name):\n",
                 "        entry = dict(category=category[i],\n",
                 "                            function=function_name[i],\n",
                 "                            parameter_values=parameter_values[i],\n",
                 "                            parent=parent[i]\n",
                 "        )\n",
@@ -1536,63 +1982,39 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from infer_subc.organelles_config.helper import write_workflow_json\n",
-                "\n",
-                "infer_nuclei_dict = make_infer_nuclei_from_raw_dict()\n",
-                "\n",
-                "write_workflow_json(\"conf_1.2.nuclei_stepbystep_from_raw\", infer_nuclei_dict)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from infer_subc.organelles_config.helper import add_function_spec_to_widget_json\n",
                 "\n",
-                "_infer_nuclei =  {\n",
-                "        \"name\": \"infer infer_nuclei_fromlabel\",\n",
-                "        \"python::module\": \"infer_subc.organelles\",\n",
-                "        \"python::function\": \"infer_nuclei_fromlabel\",\n",
-                "        \"parameters\": None\n",
-                "        }\n",
+                "infer_cellmask_fromaggr_stepbystep_from_raw_dict = make_infer_cellmask_fromaggr_step_by_step_from_raw_dict()\n",
                 "\n",
-                "add_function_spec_to_widget_json(\"infer_nuclei_fromlabel\",_infer_nuclei)"
+                "write_workflow_json(\"conf_1.1.soma_stepbystep_from_raw\", infer_cellmask_fromaggr_stepbystep_from_raw_dict)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "-------------\n",
                 "## SUMMARY\n",
                 "\n",
-                "The above details how the nuclei object is inferred.  \n",
+                "The above explains the overall framework.  \n",
                 "\n",
-                "### NEXT: INFER CYTOSOL\n",
+                "### NEXT: INFER NUCLEI\n",
                 "\n",
-                "proceed to [03_infer_cytoplasm.ipynb](./03_infer_cytoplasm.ipynb)\n"
+                "proceed to [02_infer_nuclei.ipynb](./02_infer_nuclei.ipynb)\n"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "napariNEW",
+            "display_name": "infer-subc",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -1600,16 +2022,17 @@
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.16"
         },
+        "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
-                "hash": "d6148ef1fb015fb20f0b6da2ea61c87c6b848bdf3dabb03087e5d5cd0c4607e9"
+                "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/02_infer_soma_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/02b_infer_neurites_3D.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989112485716553%*

 * *Differences: {"'cells'": "{5: {'source': {delete: [7]}}, 6: {'outputs': {0: {'text': {insert: [(0, "*

 * *            '"c:\\\\Users\\\\Shannon\\\\Anaconda3\\\\envs\\\\infer-subc\\\\lib\\\\site-packages\\\\ome_types\\\\_convenience.py:105: '*

 * *            "FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in "*

 * *            'version 0.4.0.  To silence this warning, please provide the `parser` argument, '*

 * *            "specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain  […]*

```diff
@@ -132,15 +132,14 @@
                 "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
                 "# build the datapath\n",
                 "# all the imaging data goes here.\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
-                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
                 "\n",
                 "# linearly unmixed \".czi\" files are here\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
                 "# get the list of all files\n",
@@ -153,15 +152,15 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/opt/anaconda3/envs/napariNEW/lib/python3.9/site-packages/ome_types/_convenience.py:106: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "c:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:105: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
                 "# isolate image as an ndarray and metadata as a dictionary\n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
@@ -224,16 +223,16 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(16, 768, 768)\n",
-                        "(16, 768, 768)\n"
+                        "(17, 704, 704)\n",
+                        "(17, 704, 704)\n"
                     ]
                 }
             ],
             "source": [
                 "###################\n",
                 "# INPUT\n",
                 "###################\n",
@@ -260,15 +259,15 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'img_data' at 0x1081fb490>"
+                            "<Image layer 'img_data' at 0x25e5031c3a0>"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -284,15 +283,15 @@
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'struct_img_raw' at 0x1686a6970>"
+                            "<Image layer 'struct_img_raw' at 0x25e527b0430>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -315,15 +314,15 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_struct_img_raw' at 0x16fafd0d0>"
+                            "<Image layer '_struct_img_raw' at 0x25e50a57340>"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -352,15 +351,15 @@
             "metadata": {},
             "source": [
                 "## PRE-PROCESSING (prototype)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
@@ -403,15 +402,15 @@
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'soma_log_norm' at 0x1701565b0>"
+                            "<Image layer 'composite_soma' at 0x25e437c8bb0>"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -444,31 +443,31 @@
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_log_soma' at 0x170345e80>"
+                            "<Image layer '_log_soma' at 0x25e437e2d90>"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def _non_linear_soma_transform_MCZ(in_img):\n",
                 "    \"\"\" non-linear distortion to fill out cellmask\n",
@@ -493,15 +492,15 @@
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Eventually this will be replaced by calling the un-name mangled version of the infer nuclei code that will be in infer-subc.organelles.</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "################# part 2 Nuclei pre-process\n",
                 "def _infer_nuclei_3D( in_img: np.ndarray,\n",
                 "                       median_sz: int, \n",
                 "                       gauss_sig: float,\n",
@@ -600,15 +599,15 @@
                 "    -------------\n",
                 "    nuclei_object\n",
                 "        mask defined extent of NU\n",
                 "    \n",
                 "    \"\"\"\n",
                 "\n",
                 "    nuc_ch = NUC_CH\n",
-                "    median_sz = 4   \n",
+                "    median_sz = 4      222\n",
                 "    gauss_sig = 1.34\n",
                 "    threshold_factor = 0.9\n",
                 "    thresh_min = 0.1\n",
                 "    thresh_max = 1.0\n",
                 "    max_hole_w = 5\n",
                 "    small_obj_w = 15\n",
                 "    sz_filter_method = \"3D\"\n",
@@ -634,15 +633,15 @@
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "def _masked_object_thresh(\n",
                 "    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float\n",
                 ") -> np.ndarray:\n",
@@ -685,15 +684,15 @@
             "metadata": {},
             "source": [
                 "## CORE PROCESSING"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "###################\n",
                 "# CORE_PROCESSING\n",
                 "###################\n",
                 "low_level_min_size =  50\n",
@@ -703,24 +702,24 @@
                 "                           th_method='ave', \n",
                 "                           cutoff_size=low_level_min_size, \n",
                 "                           th_adjust= 0.15)                                           "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'soma_binary' at 0x170345100>"
+                            "<Image layer 'soma_binary' at 0x25e438999d0>"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    soma_binary,\n",
@@ -736,30 +735,30 @@
                 "## POST-PROCESSING\n",
                 "\n",
                 "<code style=\"background:yellow;color:black\">Watershed (with or without the nuclei as a marker) does not work well here to get an instance segmentation</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "###################\n",
                 "# POST_PROCESSING\n",
                 "###################\n",
                 "hole_width = 100\n",
                 "removed_holes = hole_filling(soma_binary, \n",
                 "                            hole_min=0, \n",
                 "                            hole_max=hole_width**2,\n",
                 "                            fill_2d = True) \n",
                 "\n",
                 "\n",
                 "small_object_width = 45\n",
-                "cleaned_img = size_filter_linear_size(removed_holes, \n",
+                "cleaned_img = size_filter_2D(removed_holes, \n",
                 "                             min_size= small_object_width**3, \n",
                 "                             connectivity=1)\n",
                 "\n",
                 "\n",
                 "watershed_mask = cleaned_img \n",
                 "inverted_img = 1. - cleaned_img\n",
                 "\n",
@@ -769,24 +768,24 @@
                 "            connectivity= 3, # np.ones((1,3,3), bool),\n",
                 "            mask=watershed_mask,\n",
                 "            )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'labels_out' at 0x170f63460>"
+                            "<Labels layer 'labels_out' at 0x25e52d71a60>"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    removed_holes,\n",
@@ -812,24 +811,24 @@
             "metadata": {},
             "source": [
                 "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer '_labels_out' at 0x17114a700>"
+                            "<Labels layer '_labels_out [1]' at 0x25e43b8f550>"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def _masked_inverted_watershed(img_in, markers, mask):\n",
                 "    \"\"\"wrapper for watershed on inverted image and masked\n",
@@ -862,24 +861,24 @@
                 "<code style=\"background:yellow;color:black\">This should eventually be altered to maintain all cells that have the correct number of organelle markers</code>\n",
                 "\n",
                 "What is we used the nuclei (or an expanded nuclei) to select the cells with the most signal, then after selecting the nuclei with signal, use those as the watershed marker - I think it may resolve some conflicts, but not all"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'soma_out' at 0x171659340>"
+                            "<Image layer 'soma_out' at 0x25e52975190>"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "###################\n",
                 "# POST- POST_PROCESSING\n",
@@ -898,24 +897,24 @@
                 "    soma_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_soma_out' at 0x171659b80>"
+                            "<Image layer '_soma_out' at 0x25e43926160>"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def _choose_max_label(raw_signal: np.ndarray, labels_in: np.ndarray):\n",
                 "    \"\"\" keep only the label with the maximum raw signal\n",
@@ -958,15 +957,15 @@
                 "\n",
                 "A function to infer_cellmask_fromaggr from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
                 "-  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 37,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
                 "# 1. infer_cellmask_fromaggr\n",
                 "##########################\n",
                 "\n",
@@ -1092,15 +1091,15 @@
                 "                              fill_2d = True) \n",
                 "    viewer.add_image(\n",
                 "    struct_obj,\n",
                 "    scale=scale,\n",
                 "    name=7\n",
                 "    )\n",
                 "\n",
-                "    struct_obj = size_filter_linear_size(struct_obj, \n",
+                "    struct_obj = size_filter_2D(struct_obj, \n",
                 "                                min_size= small_obj_w_soma**3, \n",
                 "                                connectivity=1)\n",
                 "    viewer.add_image(\n",
                 "    struct_obj,\n",
                 "    scale=scale,\n",
                 "    name=8\n",
                 "    )\n",
@@ -1130,15 +1129,15 @@
                 "## DEFINE `_fixed_infer_cellmask_fromaggr` function\n",
                 "\n",
                 "Based on the _prototyping_ above define the function to infer cellmask. with a *fixed* set of parameters for each step in the procedure.  That is they are all \"hard coded\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 34,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
                 "# 1. fixed_infer_cellmask_fromaggr\n",
                 "##########################\n",
                 "\n",
@@ -1187,15 +1186,15 @@
                 "    return soma_out\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 38,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
@@ -1205,24 +1204,24 @@
             "source": [
                 "\n",
                 "SO_label =  _fixed_infer_cellmask_fromaggr_3D(img_data, NU_labels) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 39,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'SO_label' at 0x171ace910>"
+                            "<Image layer 'SO_label [1]' at 0x25ea42fd970>"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 39,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
                 "    SO_label,\n",
@@ -1721,15 +1720,15 @@
                 "    step_name.append(\"12\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
                 "    parent.append(11)\n",
                 "\n",
                 "    step_name.append(\"13\")\n",
-                "    function_name.append(\"size_filter_linear_size\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(12)\n",
                 "\n",
                 "    step_name.append(\"14\")\n",
                 "    function_name.append(\"label\")\n",
                 "    category.append(\"postprocessing\")\n",
@@ -1740,15 +1739,15 @@
                 "    step_name.append(\"15\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
                 "    parent.append(10)\n",
                 "\n",
                 "    step_name.append(\"16\")\n",
-                "    function_name.append(\"size_filter_linear_size\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(15)\n",
                 "\n",
                 "    step_name.append(\"17\")\n",
                 "    function_name.append(\"masked_inverted_watershed\")\n",
                 "    category.append(\"postprocessing\")\n",
@@ -1921,15 +1920,15 @@
                 "    step_name.append(\"13\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=5**2, fill_2d=True))\n",
                 "    parent.append(12)\n",
                 "\n",
                 "    step_name.append(\"14\")\n",
-                "    function_name.append(\"size_filter_linear_size\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(13)\n",
                 "\n",
                 "    step_name.append(\"15\")\n",
                 "    function_name.append(\"label\")\n",
                 "    category.append(\"postprocessing\")\n",
@@ -1941,15 +1940,15 @@
                 "    step_name.append(\"16\")\n",
                 "    function_name.append(\"hole_filling\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( hole_min=0, hole_max=25**2, fill_2d=True))\n",
                 "    parent.append(11)\n",
                 "\n",
                 "    step_name.append(\"17\")\n",
-                "    function_name.append(\"size_filter_linear_size\")\n",
+                "    function_name.append(\"size_filter_2D\")\n",
                 "    category.append(\"postprocessing\")\n",
                 "    parameter_values.append(dict( min_size = 15**2  ))\n",
                 "    parent.append(16)\n",
                 "\n",
                 "    step_name.append(\"18\")\n",
                 "    function_name.append(\"masked_inverted_watershed\")\n",
                 "    category.append(\"postprocessing\")\n",
@@ -2007,33 +2006,33 @@
                 "\n",
                 "proceed to [02_infer_nuclei.ipynb](./02_infer_nuclei.ipynb)\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "napariNEW",
+            "display_name": "infer-subc",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.9.15 (main, Nov 24 2022, 14:39:17) [MSC v.1916 64 bit (AMD64)]"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
-                "hash": "d6148ef1fb015fb20f0b6da2ea61c87c6b848bdf3dabb03087e5d5cd0c4607e9"
+                "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/02a_infer_soma_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/02c_infer_wholecell_3D.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986916208791209%*

 * *Differences: {"'cells'": "{3: {'execution_count': 1}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15 (main, Nov 24 2022, 14:39:17) [MSC v.1916 64 "*

 * *               "bit (AMD64)]'}}"}*

```diff
@@ -55,15 +55,15 @@
                 "\n",
                 "\n",
                 "## IMPORTS"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# top level imports\n",
                 "from pathlib import Path\n",
                 "import os, sys\n",
                 "from collections import defaultdict\n",
@@ -2020,15 +2020,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.9.15 (main, Nov 24 2022, 14:39:17) [MSC v.1916 64 bit (AMD64)]"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
             }
         }
```

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/02b_infer_neurites_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/new02a_infer_soma_3D.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9607552346404633%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(13, 'from skimage import filters, morphology\\n'), (17, "*

 * *            "'import skimage\\n'), (29, '                                         "*

 * *            "list_image_files)\\n')], delete: [41, 28, 13]}}, 4: {'source': {insert: [(1, '### Get "*

 * *            'and load Image for processing - specifically for __raw multichannel__ image (.czi '*

 * *            "format)\\n')]}}, 5: {'source': {insert: [(7, 'data_root_path = "*

 * *            'Path(os.path.expanduser("~")) / "Projects/ […]*

```diff
@@ -72,54 +72,55 @@
                 "\n",
                 "from scipy import ndimage as ndi\n",
                 "from aicssegmentation.core.pre_processing_utils import ( intensity_normalization, \n",
                 "                                                         image_smoothing_gaussian_slice_by_slice )\n",
                 "from aicssegmentation.core.MO_threshold import MO\n",
                 "from aicssegmentation.core.utils import hole_filling\n",
                 "\n",
-                "from skimage import filters\n",
+                "from skimage import filters, morphology\n",
                 "from skimage.segmentation import watershed\n",
                 "from skimage.morphology import remove_small_holes   # function for post-processing (size filter)\n",
                 "from skimage.measure import label\n",
+                "import skimage\n",
                 "\n",
                 "# # package for io \n",
                 "from aicsimageio import AICSImage\n",
                 "\n",
                 "import napari\n",
                 "\n",
                 "### import local python functions in ../infer_subc\n",
                 "sys.path.append(os.path.abspath((os.path.join(os.getcwd(), '..'))))\n",
                 "\n",
                 "\n",
                 "from infer_subc.core.file_io import (read_czi_image,\n",
-                "                                                                    list_image_files)\n",
+                "                                         list_image_files)\n",
                 "\n",
                 "from infer_subc.constants import (TEST_IMG_N,\n",
                 "                                                                    NUC_CH ,\n",
                 "                                                                    LYSO_CH ,\n",
                 "                                                                    MITO_CH ,\n",
                 "                                                                    GOLGI_CH ,\n",
                 "                                                                    PEROX_CH ,\n",
                 "                                                                    ER_CH ,\n",
                 "                                                                    LD_CH ,\n",
                 "                                                                    RESIDUAL_CH )                                                                    \n",
                 "from infer_subc.core.img import *\n",
                 "\n",
-                "from infer_subc.organelles import fixed_get_optimal_Z_image, fixed_find_optimal_Z, find_optimal_Z\n",
                 "\n",
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## SETUP\n",
+                "### Get and load Image for processing - specifically for __raw multichannel__ image (.czi format)\n",
                 "CUSTOMIZE WITH: \n",
                 "1. updated path to data\n",
                 "2. updated folder name for \"raw\" data\n",
                 "\n",
                 "> NOTE: we are operating on a single \"test\" image in this notebook.  The batch-processing of all the images will be happen at the end of the notebook after we have developed/confirmed the setmentation procedures and parameter settings."
             ]
         },
@@ -132,14 +133,15 @@
                 "# this will be the example image for testing the pipeline below\n",
                 "test_img_n = TEST_IMG_N\n",
                 "\n",
                 "# build the datapath\n",
                 "# all the imaging data goes here.\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents/Python Scripts/infer-subc\"\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
                 "\n",
                 "# linearly unmixed \".czi\" files are here\n",
                 "# CUSTOMIZE HERE --->\n",
                 "data_path = data_root_path / \"raw\"\n",
                 "im_type = \".czi\"\n",
                 "\n",
                 "# get the list of all files\n",
@@ -152,15 +154,15 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "c:\\Users\\Shannon\\Anaconda3\\envs\\infer-subc\\lib\\site-packages\\ome_types\\_convenience.py:105: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
+                        "/opt/anaconda3/envs/napariNEW/lib/python3.9/site-packages/ome_types/_convenience.py:106: FutureWarning: The default XML parser will be changing from 'xmlschema' to 'lxml' in version 0.4.0.  To silence this warning, please provide the `parser` argument, specifying either 'lxml' (to opt into the new behavior), or'xmlschema' (to retain the old behavior).\n",
                         "  d = to_dict(os.fspath(xml), parser=parser, validate=validate)\n"
                     ]
                 }
             ],
             "source": [
                 "# isolate image as an ndarray and metadata as a dictionary\n",
                 "img_data,meta_dict = read_czi_image(test_img_name)\n",
@@ -169,14 +171,160 @@
                 "channel_names = meta_dict['name']\n",
                 "img = meta_dict['metadata']['aicsimage']\n",
                 "scale = meta_dict['scale']\n",
                 "channel_axis = meta_dict['channel_axis']"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(8, 16, 768, 768)"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "img_data.shape"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "\n",
+                "### Get and load Image for processing - specifically for __pre-processed__ images (.OME TIF format)\n",
+                "\n",
+                "> #### Preprocessing:\n",
+                "> \n",
+                "> In this instance, we are using [Huygens Essential Software](https://svi.nl/Homepage) to deconvolve 3D fluorescence confocal images. The output is one 3-dimensional .tif file for each channel in the original image.\n",
+                "\n",
+                "The basic steps here include:\n",
+                "1. creating a separate list of image names for each channel\n",
+                "2. use reader_function to isolate the image and associate metadata from one image (from your list of choice)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "['/Users/ahenrie/Projects/Imaging/data/inferred_objectsNU_object.ome.tiff',\n",
+                            " '/Users/ahenrie/Projects/Imaging/data/20221027_C2-107_well_1_cell_1_untreated_Linear_unmixing_decon.ome.tiff']"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# this will be the example for testing the pipeline below\n",
+                "test_img_n = TEST_IMG_N\n",
+                "\n",
+                "# build the datapath\n",
+                "# all the imaging data goes here.\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Documents\\Python Scripts\\infer-subc\"\n",
+                "data_root_path = Path(os.path.expanduser(\"~\")) / \"Projects/Imaging/data\"\n",
+                "\n",
+                "# linearly unmixed \".czi\" files are here\n",
+                "data_path = data_root_path #/ \"neuron_raw_OME\"\n",
+                "im_type = \"ome.tiff\"\n",
+                "\n",
+                "# get the list of all files in \"raw\"\n",
+                "img_file_list = list_image_files(data_path,im_type)\n",
+                "# test_img_name = img_file_list[test_img_n]\n",
+                "# test_img_name\n",
+                "\n",
+                "img_file_list"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#select one image\n",
+                "test_img = img_file_list[1]\n",
+                "\n",
+                "# isolate image as an ndarray and metadata as a dictionary\n",
+                "img_data, meta_dict = read_czi_image(test_img)\n",
+                "\n",
+                "# # get some top-level info about the RAW data\n",
+                "channel_names = meta_dict['name']\n",
+                "img = meta_dict['metadata']['aicsimage']\n",
+                "scale = meta_dict['scale']\n",
+                "channel_axis = meta_dict['channel_axis']\n",
+                "huygens_meta = meta_dict['metadata']['raw_image_metadata']"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(6, 49, 1688, 1688)"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "img_data.shape"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "viewer = napari.Viewer()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'img_data' at 0x15f500880>"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "viewer.add_image(\n",
+                "    img_data,\n",
+                "    scale=scale\n",
+                ")"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "##  infer ***cellmask***\n",
                 "\n",
                 "#### summary of steps\n",
@@ -216,709 +364,740 @@
                 "Combine multiple channels that will allow inference of the cellmask.\n",
                 "\n",
                 "Note: the selected channels were chosen based on their qualitative ability to fill the cytoplasmic area of the cell. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(17, 704, 704)\n",
-                        "(17, 704, 704)\n"
+                        "(49, 1688, 1688)\n"
                     ]
                 }
             ],
             "source": [
                 "###################\n",
                 "# INPUT\n",
                 "###################\n",
-                "struct_img_raw = (6. * img_data[LYSO_CH].copy() +\n",
-                "                  1. * img_data[ER_CH].copy() + \n",
-                "                  2. * img_data[GOLGI_CH].copy())\n",
+                "LYSO_CH = 3\n",
+                "ER_CH = 1\n",
+                "GOLGI_CH = 2\n",
+                "LD_CH = 0\n",
+                "MITO_CH = 4\n",
+                "PEROX_CH = 5\n",
+                "\n",
+                "struct_img_raw = (1. * img_data[LYSO_CH].copy() +\n",
+                "                  4. * img_data[ER_CH].copy() + \n",
+                "                  1. * img_data[GOLGI_CH].copy()+\n",
+                "                  0. * img_data[LD_CH].copy()+   #because this channel labels everything, it is causing stuff outside of the the main cell to be emphasized - not great!\n",
+                "                  2. * img_data[MITO_CH].copy()+\n",
+                "                  2. * img_data[PEROX_CH].copy())\n",
                 "\n",
-                "raw_nuclei = img_data[NUC_CH].copy() \n",
+                "# raw_nuclei = img_data[NUC_CH].copy() \n",
                 "\n",
                 "print(struct_img_raw.shape)\n",
-                "print(raw_nuclei.shape)"
+                "# print(raw_nuclei.shape)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### VISUALIZE: the composite image that will be used as input\n",
                 "Use this to adjust which channels and multiplication factors to use to create the composite input image above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'img_data' at 0x25e5031c3a0>"
+                            "<Image layer 'struct_img_raw' at 0x145509dc0>"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "viewer = napari.Viewer()\n",
                 "viewer.add_image(\n",
-                "    img_data,\n",
+                "    struct_img_raw,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## PRE-PROCESSING (prototype)\n"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 12,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
+                    ]
+                }
+            ],
+            "source": [
+                "\n",
+                "###################\n",
+                "# PRE_PROCESSING\n",
+                "###################\n",
+                "\n",
+                "################# smoothing\n",
+                "soma_norm = min_max_intensity_normalization(struct_img_raw)\n",
+                "\n",
+                "\n",
+                "### No longer need smoothing with preprocessed images ###\n",
+                "# med_filter_size = 15\n",
+                "# soma_med = median_filter_slice_by_slice(soma_norm, \n",
+                "#                                         size=med_filter_size)\n",
+                "\n",
+                "# gaussian_smoothing_sigma = 1.34\n",
+                "# gaussian_smoothing_truncate_range = 3.0\n",
+                "# soma_guas = ndi.gaussian_filter(soma_med,\n",
+                "#                                 sigma=gaussian_smoothing_sigma,\n",
+                "#                                 mode=\"nearest\", \n",
+                "#                                 truncate=gaussian_smoothing_truncate_range)\n",
+                "\n",
+                "\n",
+                "################# NON-Linear aggregation\n",
+                "soma_log, d = log_transform(soma_norm) \n",
+                "soma_log_norm = intensity_normalization(soma_log, scaling_param=[0])\n",
+                "\n",
+                "# soma_edges = filters.difference_of_gaussians(soma_log_norm, 2)\n",
+                "\n",
+                "# composite_soma = intensity_normalization(soma_edges, scaling_param=[0]) + soma_log_norm "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'struct_img_raw' at 0x25e527b0430>"
+                            "<Image layer 'soma_log_norm' at 0x145509af0>"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "# viewer.add_image(\n",
+                "#     soma_med,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "# viewer.add_image(\n",
+                "#     soma_guas,\n",
+                "#     scale=scale\n",
+                "# )\n",
                 "viewer.add_image(\n",
-                "    struct_img_raw,\n",
+                "    soma_log_norm,\n",
                 "    scale=scale\n",
-                ")"
+                ")\n",
+                "# viewer.add_image(\n",
+                "#     soma_edges,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "# viewer.add_image(\n",
+                "#     composite_soma,\n",
+                "#     scale=scale\n",
+                "# )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
+                "## CORE PROCESSING"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 14,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "###################\n",
+                "# CORE_PROCESSING\n",
+                "###################\n",
+                "low_level_min_size =  50\n",
+                "\n",
+                "# ################# part 1\n",
+                "soma_binary = MO(soma_log_norm, \n",
+                "                   global_thresh_method='ave', \n",
+                "                   object_minArea=low_level_min_size, \n",
+                "                   extra_criteria=True,\n",
+                "                   local_adjust= 0.05,\n",
+                "                   return_object=False,\n",
+                "                   dilate=False)                      "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_struct_img_raw' at 0x25e50a57340>"
+                            "<Image layer 'soma_binary' at 0x168ec8730>"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "def _raw_soma_MCZ(img_in):\n",
-                "    \"\"\" define cellmask image\n",
-                "    \"\"\"\n",
-                "    SOMA_W = (6.,1.,2.)\n",
-                "    SOMA_CH = (LYSO_CH,ER_CH,GOLGI_CH)\n",
-                "    img_out = np.zeros_like(img_in[0]).astype(np.double)\n",
-                "    for w,ch in zip(SOMA_W,SOMA_CH):\n",
-                "        img_out += w*img_in[ch]\n",
-                "    return img_out\n",
-                "\n",
-                "_struct_img_raw = _raw_soma_MCZ(img_data)\n",
-                "\n",
                 "viewer.add_image(\n",
-                "    _struct_img_raw,\n",
+                "    soma_binary,\n",
                 "    scale=scale\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## PRE-PROCESSING (prototype)\n"
+                "## POST-PROCESSING"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 16,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "\n",
                 "###################\n",
-                "# PRE_PROCESSING\n",
+                "# POST_PROCESSING\n",
                 "###################\n",
-                "\n",
-                "################# smoothing\n",
-                "soma_norm = min_max_intensity_normalization(struct_img_raw)\n",
-                "\n",
-                "med_filter_size = 15\n",
-                "soma_med = median_filter_slice_by_slice(soma_norm, \n",
-                "                                        size=med_filter_size)\n",
-                "\n",
-                "## Need to adjust image_smoothing_gaussian_slice_by_slice in pre_processing_utils.py to integrate the mode\n",
-                "\n",
-                "gaussian_smoothing_sigma = 1.34\n",
-                "gaussian_smoothing_truncate_range = 3.0\n",
-                "soma_guas = ndi.gaussian_filter(soma_med,\n",
-                "                                sigma=gaussian_smoothing_sigma,\n",
-                "                                mode=\"nearest\", \n",
-                "                                truncate=gaussian_smoothing_truncate_range)\n",
+                "hole_width = 30\n",
+                "removed_holes = hole_filling(soma_binary, \n",
+                "                            hole_min=0, \n",
+                "                            hole_max=hole_width**3,\n",
+                "                            fill_2d = False) \n",
                 "\n",
                 "\n",
-                "################# NON-Linear aggregation\n",
-                "soma_log, d = log_transform(soma_guas) \n",
-                "soma_log_norm = intensity_normalization(soma_log, scaling_param=[0])\n",
-                "\n",
-                "# soma_edges = filters.difference_of_gaussians(soma_log_norm, 2)\n",
-                "\n",
-                "# composite_soma = intensity_normalization(soma_edges, scaling_param=[0]) + soma_log_norm "
+                "small_object_width = 10\n",
+                "cleaned_img = size_filter(removed_holes, \n",
+                "                          min_size= small_object_width**3, \n",
+                "                          connectivity=1)\n",
+                "\n",
+                "### Watershed instance segmentation is not necessary here becuase we are assuming that there is ~ one cell per image and all of the objects, even if they aren't connected are from the same cell\n",
+                "### For the same reason, label() is no necessary here\n",
+                "# watershed_mask = cleaned_img \n",
+                "# inverted_img = 1. - cleaned_img\n",
+                "\n",
+                "# labels_out = watershed(\n",
+                "#             inverted_img,\n",
+                "#             # markers=NU_labels,\n",
+                "#             connectivity= 3, # np.ones((1,3,3), bool),\n",
+                "#             mask=watershed_mask,\n",
+                "#             )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'composite_soma' at 0x25e437c8bb0>"
+                            "<Image layer 'cleaned_img' at 0x145509b50>"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "viewer.add_image(\n",
-                "    soma_med,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    soma_guas,\n",
+                "    removed_holes,\n",
                 "    scale=scale\n",
                 ")\n",
                 "viewer.add_image(\n",
-                "    soma_log_norm,\n",
+                "    cleaned_img,\n",
                 "    scale=scale\n",
                 ")\n",
                 "# viewer.add_image(\n",
-                "#     soma_edges,\n",
+                "#     inverted_img,\n",
                 "#     scale=scale\n",
                 "# )\n",
-                "# viewer.add_image(\n",
-                "#     composite_soma,\n",
+                "# viewer.add_labels(\n",
+                "#     labels_out,\n",
                 "#     scale=scale\n",
                 "# )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
+                "## POST POST-PROCESSING\n",
+                "\n",
+                "This process is unnecessary for neuron images, but I think its fine to keep since it doesn't do any harm"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 18,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "###################\n",
+                "# POST- POST_PROCESSING\n",
+                "###################\n",
+                "# keep the \"SOMA\" label which contains the highest total signal\n",
+                "all_labels = np.unique(cleaned_img)[1:]\n",
+                "\n",
+                "total_signal = [soma_norm[cleaned_img == lab].sum() for lab in all_labels]\n",
+                "keep_label = all_labels[np.argmax(total_signal)]\n",
+                "keep_label\n",
+                "\n",
+                "soma_out = np.zeros_like(cleaned_img)\n",
+                "soma_out[cleaned_img==keep_label] = 1\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
-                            "<Image layer '_log_soma' at 0x25e437e2d90>"
+                            "<Image layer 'soma_out' at 0x168d29d30>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "def _non_linear_soma_transform_MCZ(in_img):\n",
-                "    \"\"\" non-linear distortion to fill out cellmask\n",
-                "    log + edge of smoothed composite\n",
-                "    \"\"\"\n",
-                "    # non-Linear processing\n",
-                "    log_img, d = log_transform(in_img.copy()) \n",
-                "    return intensity_normalization(log_img,scaling_param=[0])\n",
-                "    # return intensity_normalization(filters.difference_of_gaussians(log_img, 2),scaling_param=[0])  + log_img\n",
-                "\n",
-                "_log_soma = _non_linear_soma_transform_MCZ(soma_guas)\n",
                 "\n",
                 "viewer.add_image(\n",
-                "    _log_soma,\n",
+                "    soma_out,\n",
                 "    scale=scale\n",
-                ")\n"
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\">Eventually this will be replaced by calling the un-name mangled version of the infer nuclei code that will be in infer-subc.organelles.</code>"
+                "## Finding the nuclei using the inverse of the cell mask"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
-                "################# part 2 Nuclei pre-process\n",
-                "def _infer_nuclei_3D( in_img: np.ndarray,\n",
-                "                       median_sz: int, \n",
-                "                       gauss_sig: float,\n",
-                "                       thresh_factor: float,\n",
-                "                       thresh_min: float,\n",
-                "                       thresh_max: float,\n",
-                "                       max_hole_w: int,\n",
-                "                       small_obj_w: int,\n",
-                "                       sz_filter_method: str\n",
-                "                     ) -> np.ndarray:\n",
-                "    \"\"\"\n",
-                "    Procedure to infer 3D nuclei segmentation from multichannel z-stack input.\n",
-                "\n",
-                "    Parameters\n",
-                "    ------------\n",
-                "    in_img: np.ndarray\n",
-                "        a 3d image containing all the channels\n",
-                "    soma_mask: Optional[np.ndarray] = None\n",
-                "        mask\n",
-                "    median_sz: int\n",
-                "        width of median filter for signal\n",
-                "    gauss_sig: float\n",
-                "        sigma for gaussian smoothing of  signal\n",
-                "    thresh_factor: float\n",
-                "        adjustment factor for log Li threholding\n",
-                "    thresh_min: float\n",
-                "        abs min threhold for log Li threholding\n",
-                "    thresh_max: float\n",
-                "        abs max threhold for log Li threholding\n",
-                "    max_hole_w: int\n",
-                "        hole filling cutoff for nuclei post-processing\n",
-                "    small_obj_w: int\n",
-                "        minimum object size cutoff for nuclei post-processing\n",
-                "    sz_filter_method: str\n",
-                "        method for size filtering; either \"3D\" or \"slice_by_slice\"\n",
-                "\n",
-                "    Returns\n",
-                "    -------------\n",
-                "    nuclei_object\n",
-                "        mask defined extent of NU\n",
-                "    \n",
-                "    \"\"\"\n",
-                "\n",
-                "    nuc_ch = NUC_CH\n",
-                "    nuclei = select_channel_from_raw(in_img, nuc_ch)\n",
-                "\n",
-                "\n",
-                "    ###################\n",
-                "    # PRE_PROCESSING\n",
-                "    ###################                \n",
-                "    nuclei = min_max_intensity_normalization(nuclei)\n",
-                "    nuclei = median_filter_slice_by_slice(nuclei,\n",
-                "                                          size=median_sz)\n",
-                "    nuclei = image_smoothing_gaussian_slice_by_slice(nuclei,\n",
-                "                                                     sigma=gauss_sig )\n",
+                "#################################\n",
+                "####### label-free nuclei #######\n",
+                "#################################\n",
+                "inverted_mask = 1 - soma_out\n",
                 "\n",
+                "inverted_labels = label(inverted_mask, connectivity=1)\n",
                 "\n",
-                "    ###################\n",
-                "    # CORE_PROCESSING\n",
-                "    ###################\n",
-                "    nuclei_object = apply_log_li_threshold(nuclei, \n",
-                "                                           thresh_factor=thresh_factor, \n",
-                "                                           thresh_min=thresh_min, \n",
-                "                                           thresh_max=thresh_max)\n",
-                "\n",
-                "\n",
-                "    ###################\n",
-                "    # POST_PROCESSING\n",
-                "    ###################\n",
-                "    nuclei_object = hole_filling(nuclei_object, \n",
-                "                                 hole_min=0, \n",
-                "                                 hole_max=max_hole_w**2, \n",
-                "                                 fill_2d=True)\n",
-                "\n",
-                "    nuclei_object = size_filter(nuclei_object, \n",
-                "                                min_size = small_obj_w**3, \n",
-                "                                method = sz_filter_method,\n",
-                "                                connectivity=1)\n",
-                "\n",
-                "\n",
-                "    return nuclei_object\n",
-                "\n",
-                "\n",
-                "def _fixed_infer_nuclei_3D(in_img: np.ndarray) -> np.ndarray:\n",
-                "    \"\"\"\n",
-                "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
-                "\n",
-                "    Parameters\n",
-                "    ------------\n",
-                "    in_img: np.ndarray\n",
-                "        a 3d image containing all the channels\n",
-                "    soma_mask: np.ndarray\n",
-                "        mask\n",
-                " \n",
-                "    Returns\n",
-                "    -------------\n",
-                "    nuclei_object\n",
-                "        mask defined extent of NU\n",
-                "    \n",
-                "    \"\"\"\n",
+                "hole_width = 30 \n",
+                "removed_holes_nuc = hole_filling(inverted_mask,\n",
+                "                             hole_min=0, \n",
+                "                             hole_max=hole_width**3, \n",
+                "                             fill_2d=False)\n",
                 "\n",
-                "    nuc_ch = NUC_CH\n",
-                "    median_sz = 4      222\n",
-                "    gauss_sig = 1.34\n",
-                "    threshold_factor = 0.9\n",
-                "    thresh_min = 0.1\n",
-                "    thresh_max = 1.0\n",
-                "    max_hole_w = 5\n",
-                "    small_obj_w = 15\n",
-                "    sz_filter_method = \"3D\"\n",
+                "small_object_width = 20\n",
+                "cleaned_img_nuc = size_filter(removed_holes_nuc, \n",
+                "                          min_size= small_object_width**3,\n",
+                "                          method=\"3D\",\n",
+                "                          connectivity=3)\n",
                 "\n",
-                "    return _infer_nuclei_3D( in_img,\n",
-                "                             median_sz,\n",
-                "                             gauss_sig,\n",
-                "                             threshold_factor,\n",
-                "                             thresh_min,\n",
-                "                             thresh_max,\n",
-                "                             max_hole_w,\n",
-                "                             small_obj_w,\n",
-                "                             sz_filter_method )\n",
+                "all_labels_nuc = label(cleaned_img_nuc)\n",
                 "\n",
                 "\n",
-                "_NU_object =  _fixed_infer_nuclei_3D(img_data) \n",
-                "NU_labels = label(_NU_object)"
+                "nuc_from_neg = cleaned_img\n",
+                "nuclei_label = skimage.segmentation.clear_border(cleaned_img_nuc)"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 28,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
+                "test_lab = label(removed_holes_nuc, connectivity=1)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 33,
             "metadata": {},
             "outputs": [],
             "source": [
+                "rem_hol = np.zeros_like(removed_holes_nuc)\n",
+                "rem_hol[removed_holes_nuc>0]=255\n",
                 "\n",
-                "def _masked_object_thresh(\n",
-                "    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float\n",
-                ") -> np.ndarray:\n",
-                "    \"\"\"\n",
-                "    wrapper for applying Masked Object Thresholding with just two parameters via `MO` from `aicssegmentation`\n",
-                "    Parameters\n",
-                "    ------------\n",
-                "    structure_img_smooth: np.ndarray\n",
-                "        a 3d image\n",
-                "    th_method: \n",
-                "         which method to use for calculating global threshold. Options include:\n",
-                "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
-                "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
-                "    cutoff_size: \n",
-                "        Masked Object threshold `size_min`\n",
-                "    th_adjust: \n",
-                "        Masked Object threshold `local_adjust`\n",
-                "\n",
-                "    Returns\n",
-                "    -------------\n",
-                "        np.ndimage \n",
-                "\n",
-                "    \"\"\"\n",
-                "\n",
-                "    struct_obj = MO(\n",
-                "        structure_img_smooth,\n",
-                "        global_thresh_method=th_method,\n",
-                "        object_minArea=cutoff_size,\n",
-                "        extra_criteria=True,\n",
-                "        local_adjust=th_adjust,\n",
-                "        return_object=False,\n",
-                "        dilate=True,\n",
-                "    )\n",
-                "    return struct_obj\n"
+                "test_lab2 = label(rem_hol, connectivity=2)\n"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 34,
             "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 34,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "## CORE PROCESSING"
+                "np.all(test_lab==test_lab2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "###################\n",
-                "# CORE_PROCESSING\n",
-                "###################\n",
-                "low_level_min_size =  50\n",
-                "\n",
-                "# ################# part 1\n",
-                "soma_binary = _masked_object_thresh(soma_log_norm, \n",
-                "                           th_method='ave', \n",
-                "                           cutoff_size=low_level_min_size, \n",
-                "                           th_adjust= 0.15)                                           "
+                "test_fill = hole_filling(inverted_mask,\n",
+                "                             hole_min=0, \n",
+                "                             hole_max=hole_width**3, \n",
+                "                             fill_2d=False)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Image layer 'soma_binary' at 0x25e438999d0>"
+                            "(49, 1688, 1688)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "viewer.add_image(\n",
-                "    soma_binary,\n",
-                "    scale=scale\n",
-                ")"
+                "all_labels_nuc.shape"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 22,
             "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Image layer 'removed_holes_nuc' at 0x16a560100>"
+                        ]
+                    },
+                    "execution_count": 22,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "## POST-PROCESSING\n",
-                "\n",
-                "<code style=\"background:yellow;color:black\">Watershed (with or without the nuclei as a marker) does not work well here to get an instance segmentation</code>"
+                "viewer.add_image(\n",
+                "    removed_holes_nuc,\n",
+                "    scale=scale\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 23,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "<Labels layer 'all_labels_nuc' at 0x16d1eb400>"
+                        ]
+                    },
+                    "execution_count": 23,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "###################\n",
-                "# POST_PROCESSING\n",
-                "###################\n",
-                "hole_width = 100\n",
-                "removed_holes = hole_filling(soma_binary, \n",
-                "                            hole_min=0, \n",
-                "                            hole_max=hole_width**2,\n",
-                "                            fill_2d = True) \n",
-                "\n",
-                "\n",
-                "small_object_width = 45\n",
-                "cleaned_img = size_filter_2D(removed_holes, \n",
-                "                             min_size= small_object_width**3, \n",
-                "                             connectivity=1)\n",
-                "\n",
-                "\n",
-                "watershed_mask = cleaned_img \n",
-                "inverted_img = 1. - cleaned_img\n",
-                "\n",
-                "labels_out = watershed(\n",
-                "            inverted_img,\n",
-                "            markers=NU_labels,\n",
-                "            connectivity= 3, # np.ones((1,3,3), bool),\n",
-                "            mask=watershed_mask,\n",
-                "            )"
+                "# viewer.add_image(\n",
+                "#     inverted_mask,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "viewer.add_labels(\n",
+                "    inverted_labels,\n",
+                "    scale=scale\n",
+                ")\n",
+                "# viewer.add_image(\n",
+                "#     removed_holes_nuc,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "# viewer.add_image(\n",
+                "#     cleaned_img_nuc,\n",
+                "#     scale=scale\n",
+                "# )\n",
+                "viewer.add_labels(\n",
+                "    all_labels_nuc,\n",
+                "    scale=scale\n",
+                ")\n",
+                "# viewer.add_labels(\n",
+                "#     nuclei_label,\n",
+                "#     scale=scale\n",
+                "# )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<Labels layer 'labels_out' at 0x25e52d71a60>"
+                            "<Labels layer 'Labels' at 0x178868ee0>"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "viewer.add_labels(label(soma_out), scale=scale)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Playing around with methods to isolate cellmask and neurites independently"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "z_scale_ratio = scale[0]/scale[1]\n",
+                "spacing = (z_scale_ratio, 1, 1)\n",
+                "\n",
+                "eroded = skimage.morphology.isotropic_erosion(filled, radius=10, spacing=spacing)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "viewer.add_image(\n",
-                "    removed_holes,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_image(\n",
-                "    cleaned_img,\n",
+                "    eroded,\n",
                 "    scale=scale\n",
-                ")\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dilated = skimage.morphology.isotropic_dilation(eroded, radius=10, spacing=spacing)\n",
                 "viewer.add_image(\n",
-                "    inverted_img,\n",
-                "    scale=scale\n",
-                ")\n",
-                "viewer.add_labels(\n",
-                "    labels_out,\n",
+                "    dilated,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<code style=\"background:yellow;color:black\">Consider moving this to the definition section below</code>"
+                "\n",
+                "\n",
+                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 19,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "<Labels layer '_labels_out [1]' at 0x25e43b8f550>"
-                        ]
-                    },
-                    "execution_count": 19,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
             "source": [
-                "def _masked_inverted_watershed(img_in, markers, mask):\n",
-                "    \"\"\"wrapper for watershed on inverted image and masked\n",
+                "## DEFINE parameterized  `_infer_cellmask_fromaggr` function\n",
                 "\n",
+                "A function to infer_cellmask_fromaggr from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
+                "-  "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def _non_linear_soma_transform_MCZ(in_img):\n",
+                "    \"\"\" non-linear distortion to fill out cellmask\n",
+                "    log + edge of smoothed composite\n",
                 "    \"\"\"\n",
-                "    labels_out = watershed(\n",
-                "                1. - img_in,\n",
-                "                markers=markers,\n",
-                "                connectivity=3,\n",
-                "                mask=mask,\n",
-                "                )\n",
-                "    return labels_out\n",
+                "    # non-Linear processing\n",
+                "    log_img, d = log_transform(in_img.copy()) \n",
+                "    return intensity_normalization(log_img,scaling_param=[0])\n",
+                "    # return intensity_normalization(filters.difference_of_gaussians(log_img, 2),scaling_param=[0])  + log_img\n",
                 "\n",
+                "_log_soma = _non_linear_soma_transform_MCZ(soma_guas)\n",
                 "\n",
-                "_labels_out = _masked_inverted_watershed(cleaned_img, NU_labels, cleaned_img)\n",
+                "viewer.add_image(\n",
+                "    _log_soma,\n",
+                "    scale=scale\n",
+                ")\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def _raw_soma_MCZ(img_in):\n",
+                "    \"\"\" define cellmask image\n",
+                "    \"\"\"\n",
+                "    SOMA_W = (6.,1.,2.)\n",
+                "    SOMA_CH = (LYSO_CH,ER_CH,GOLGI_CH)\n",
+                "    img_out = np.zeros_like(img_in[0]).astype(np.double)\n",
+                "    for w,ch in zip(SOMA_W,SOMA_CH):\n",
+                "        img_out += w*img_in[ch]\n",
+                "    return img_out\n",
                 "\n",
-                "viewer.add_labels(\n",
-                "    _labels_out,\n",
+                "_struct_img_raw = _raw_soma_MCZ(img_data)\n",
+                "\n",
+                "viewer.add_image(\n",
+                "    _struct_img_raw,\n",
                 "    scale=scale\n",
-                ")"
+                ")\n"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## POST POST-PROCESSING\n",
+                "def _masked_object_thresh(\n",
+                "    structure_img_smooth: np.ndarray, th_method: str, cutoff_size: int, th_adjust: float\n",
+                ") -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    wrapper for applying Masked Object Thresholding with just two parameters via `MO` from `aicssegmentation`\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    structure_img_smooth: np.ndarray\n",
+                "        a 3d image\n",
+                "    th_method: \n",
+                "         which method to use for calculating global threshold. Options include:\n",
+                "         \"triangle\" (or \"tri\"), \"median\" (or \"med\"), and \"ave_tri_med\" (or \"ave\").\n",
+                "         \"ave\" refers the average of \"triangle\" threshold and \"mean\" threshold.\n",
+                "    cutoff_size: \n",
+                "        Masked Object threshold `size_min`\n",
+                "    th_adjust: \n",
+                "        Masked Object threshold `local_adjust`\n",
+                "\n",
+                "    Returns\n",
+                "    -------------\n",
+                "        np.ndimage \n",
                 "\n",
-                "<code style=\"background:yellow;color:black\">This should eventually be altered to maintain all cells that have the correct number of organelle markers</code>\n",
+                "    \"\"\"\n",
                 "\n",
-                "What is we used the nuclei (or an expanded nuclei) to select the cells with the most signal, then after selecting the nuclei with signal, use those as the watershed marker - I think it may resolve some conflicts, but not all"
+                "    struct_obj = MO(\n",
+                "        structure_img_smooth,\n",
+                "        global_thresh_method=th_method,\n",
+                "        object_minArea=cutoff_size,\n",
+                "        extra_criteria=True,\n",
+                "        local_adjust=th_adjust,\n",
+                "        return_object=False,\n",
+                "        dilate=True,\n",
+                "    )\n",
+                "    return struct_obj\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "<Image layer 'soma_out' at 0x25e52975190>"
-                        ]
-                    },
-                    "execution_count": 20,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "###################\n",
-                "# POST- POST_PROCESSING\n",
-                "###################\n",
-                "# keep the \"SOMA\" label which contains the highest total signal\n",
-                "all_labels = np.unique(labels_out)[1:]\n",
+                "def _masked_inverted_watershed(img_in, markers, mask):\n",
+                "    \"\"\"wrapper for watershed on inverted image and masked\n",
                 "\n",
-                "total_signal = [soma_norm[labels_out == label].sum() for label in all_labels]\n",
-                "keep_label = all_labels[np.argmax(total_signal)]\n",
-                "keep_label\n",
+                "    \"\"\"\n",
+                "    labels_out = watershed(\n",
+                "                1. - img_in,\n",
+                "                markers=markers,\n",
+                "                connectivity=3,\n",
+                "                mask=mask,\n",
+                "                )\n",
+                "    return labels_out\n",
                 "\n",
-                "soma_out = np.zeros_like(labels_out)\n",
-                "soma_out[labels_out==keep_label] = 1\n",
                 "\n",
-                "viewer.add_image(\n",
-                "    soma_out,\n",
+                "_labels_out = _masked_inverted_watershed(cleaned_img, NU_labels, cleaned_img)\n",
+                "\n",
+                "viewer.add_labels(\n",
+                "    _labels_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "<Image layer '_soma_out' at 0x25e43926160>"
-                        ]
-                    },
-                    "execution_count": 21,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "def _choose_max_label(raw_signal: np.ndarray, labels_in: np.ndarray):\n",
                 "    \"\"\" keep only the label with the maximum raw signal\n",
                 "\n",
                 "    \"\"\"\n",
                 "\n",
                 "    all_labels = np.unique(labels_in)[1:]\n",
@@ -936,36 +1115,149 @@
                 "viewer.add_image(\n",
                 "    _soma_out,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
+                "################# part 2 Nuclei pre-process\n",
+                "def _infer_nuclei_3D( in_img: np.ndarray,\n",
+                "                       median_sz: int, \n",
+                "                       gauss_sig: float,\n",
+                "                       thresh_factor: float,\n",
+                "                       thresh_min: float,\n",
+                "                       thresh_max: float,\n",
+                "                       max_hole_w: int,\n",
+                "                       small_obj_w: int,\n",
+                "                       sz_filter_method: str\n",
+                "                     ) -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    Procedure to infer 3D nuclei segmentation from multichannel z-stack input.\n",
                 "\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    in_img: np.ndarray\n",
+                "        a 3d image containing all the channels\n",
+                "    soma_mask: Optional[np.ndarray] = None\n",
+                "        mask\n",
+                "    median_sz: int\n",
+                "        width of median filter for signal\n",
+                "    gauss_sig: float\n",
+                "        sigma for gaussian smoothing of  signal\n",
+                "    thresh_factor: float\n",
+                "        adjustment factor for log Li threholding\n",
+                "    thresh_min: float\n",
+                "        abs min threhold for log Li threholding\n",
+                "    thresh_max: float\n",
+                "        abs max threhold for log Li threholding\n",
+                "    max_hole_w: int\n",
+                "        hole filling cutoff for nuclei post-processing\n",
+                "    small_obj_w: int\n",
+                "        minimum object size cutoff for nuclei post-processing\n",
+                "    sz_filter_method: str\n",
+                "        method for size filtering; either \"3D\" or \"slice_by_slice\"\n",
                 "\n",
-                "<code style=\"background:yellow;color:black\">***WIP*** 2D-->3D transition stops here</code>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## DEFINE parameterized  `_infer_cellmask_fromaggr` function\n",
+                "    Returns\n",
+                "    -------------\n",
+                "    nuclei_object\n",
+                "        mask defined extent of NU\n",
+                "    \n",
+                "    \"\"\"\n",
                 "\n",
-                "A function to infer_cellmask_fromaggr from our (Channel, 1 Z slice, X, Y) image accourding the the following parameters: \n",
-                "-  "
+                "    nuc_ch = NUC_CH\n",
+                "    nuclei = select_channel_from_raw(in_img, nuc_ch)\n",
+                "\n",
+                "\n",
+                "    ###################\n",
+                "    # PRE_PROCESSING\n",
+                "    ###################                \n",
+                "    nuclei = min_max_intensity_normalization(nuclei)\n",
+                "    nuclei = median_filter_slice_by_slice(nuclei,\n",
+                "                                          size=median_sz)\n",
+                "    nuclei = image_smoothing_gaussian_slice_by_slice(nuclei,\n",
+                "                                                     sigma=gauss_sig )\n",
+                "\n",
+                "\n",
+                "    ###################\n",
+                "    # CORE_PROCESSING\n",
+                "    ###################\n",
+                "    nuclei_object = apply_log_li_threshold(nuclei, \n",
+                "                                           thresh_factor=thresh_factor, \n",
+                "                                           thresh_min=thresh_min, \n",
+                "                                           thresh_max=thresh_max)\n",
+                "\n",
+                "\n",
+                "    ###################\n",
+                "    # POST_PROCESSING\n",
+                "    ###################\n",
+                "    nuclei_object = hole_filling(nuclei_object, \n",
+                "                                 hole_min=0, \n",
+                "                                 hole_max=max_hole_w**2, \n",
+                "                                 fill_2d=True)\n",
+                "\n",
+                "    nuclei_object = size_filter(nuclei_object, \n",
+                "                                min_size = small_obj_w**3, \n",
+                "                                method = sz_filter_method,\n",
+                "                                connectivity=1)\n",
+                "\n",
+                "\n",
+                "    return nuclei_object\n",
+                "\n",
+                "\n",
+                "def _fixed_infer_nuclei_3D(in_img: np.ndarray) -> np.ndarray:\n",
+                "    \"\"\"\n",
+                "    Procedure to infer cellmask from linearly unmixed input, with a *fixed* set of parameters for each step in the procedure.  i.e. \"hard coded\"\n",
+                "\n",
+                "    Parameters\n",
+                "    ------------\n",
+                "    in_img: np.ndarray\n",
+                "        a 3d image containing all the channels\n",
+                "    soma_mask: np.ndarray\n",
+                "        mask\n",
+                " \n",
+                "    Returns\n",
+                "    -------------\n",
+                "    nuclei_object\n",
+                "        mask defined extent of NU\n",
+                "    \n",
+                "    \"\"\"\n",
+                "\n",
+                "    nuc_ch = NUC_CH\n",
+                "    median_sz = 4   \n",
+                "    gauss_sig = 1.34\n",
+                "    threshold_factor = 0.9\n",
+                "    thresh_min = 0.1\n",
+                "    thresh_max = 1.0\n",
+                "    max_hole_w = 5\n",
+                "    small_obj_w = 15\n",
+                "    sz_filter_method = \"3D\"\n",
+                "\n",
+                "    return _infer_nuclei_3D( in_img,\n",
+                "                             median_sz,\n",
+                "                             gauss_sig,\n",
+                "                             threshold_factor,\n",
+                "                             thresh_min,\n",
+                "                             thresh_max,\n",
+                "                             max_hole_w,\n",
+                "                             small_obj_w,\n",
+                "                             sz_filter_method )\n",
+                "\n",
+                "\n",
+                "_NU_object =  _fixed_infer_nuclei_3D(img_data) \n",
+                "NU_labels = label(_NU_object)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
                 "# 1. infer_cellmask_fromaggr\n",
                 "##########################\n",
                 "\n",
@@ -1129,15 +1421,15 @@
                 "## DEFINE `_fixed_infer_cellmask_fromaggr` function\n",
                 "\n",
                 "Based on the _prototyping_ above define the function to infer cellmask. with a *fixed* set of parameters for each step in the procedure.  That is they are all \"hard coded\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "##########################\n",
                 "# 1. fixed_infer_cellmask_fromaggr\n",
                 "##########################\n",
                 "\n",
@@ -1186,46 +1478,27 @@
                 "    return soma_out\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "intensity normalization: min-max normalization with NO absoluteintensity upper bound\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "\n",
                 "SO_label =  _fixed_infer_cellmask_fromaggr_3D(img_data, NU_labels) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "<Image layer 'SO_label [1]' at 0x25ea42fd970>"
-                        ]
-                    },
-                    "execution_count": 39,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "viewer.add_image(\n",
                 "    SO_label,\n",
                 "    scale=scale\n",
                 ")"
             ]
         },
@@ -2020,15 +2293,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15 (main, Nov 24 2022, 14:39:17) [MSC v.1916 64 bit (AMD64)]"
+            "version": "3.9.16"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "182b63330db9794b59aa776c624821fb477d854325ad145fa5385f0d56c0c6f3"
             }
         }
```

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/03_infer_cytosol_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/03_infer_cytosol_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/04_infer_lysosome_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/04_infer_lysosome_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/05_infer_mitochondria_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/05_infer_mitochondria_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/06_infer_golgi_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/06_infer_golgi_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/07_infer_peroxisome_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/07_infer_peroxisome_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/09_infer_lipid_body_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/09_infer_lipid_body_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/10_batch_process_3D.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/10_batch_process_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/10_batch_process_3Dv2.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/10_batch_process_3Dv2.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/999_fn_prototypes_json.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/999_fn_prototypes_json.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/A_spectral_test.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/A_spectral_test.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/_centrosome_routines.py` & `infer-subc-0.0.post1/notebooks/todelete/_centrosome_routines.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/_graveyard.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/_graveyard.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/notebooks/todelete/test_soma_seg.ipynb` & `infer-subc-0.0.post1/notebooks/todelete/test_soma_seg.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/setup.cfg` & `infer-subc-0.0.post1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 	numpy
 	aicsimageio >= 4.7.0
 	scipy    #>=1.1.0
 	numpy    #>=1.15.1
 	scikit-image #>=0.18.0,<0.19.0
 	pandas   #>=0.23.4
 	jupyter
-	centrosome
 platforms = any
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	= .
 setup_requires = setuptools_scm
 
@@ -53,15 +52,15 @@
 where = .
 
 [options.entry_points]
 console_scripts = 
 	infer_subc = infer_subc.__main__:main
 
 [options.package_data]
-* = *.yaml, *.json, *.md
+* = *.yaml
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `infer-subc-0.0.6b0/test.yaml` & `infer-subc-0.0.post1/test.yaml`

 * *Files identical despite different names*

### Comparing `infer-subc-0.0.6b0/windows_notes.md` & `infer-subc-0.0.post1/windows_notes.md`

 * *Files identical despite different names*

