# Comparing `tmp/emmet-api-0.55.3.tar.gz` & `tmp/emmet-api-0.55.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.55.3.tar", last modified: Thu Jun  1 18:07:11 2023, max compression
+gzip compressed data, was "emmet-api-0.55.4.tar", last modified: Tue Jun  6 21:34:25 2023, max compression
```

## Comparing `emmet-api-0.55.3.tar` & `emmet-api-0.55.4.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-01 18:07:05.000000 emmet-api-0.55.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-01 18:07:11.300487 emmet-api-0.55.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-01 18:07:05.000000 emmet-api-0.55.3/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.272487 emmet-api-0.55.3/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.276487 emmet-api-0.55.3/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-01 18:07:11.000000 emmet-api-0.55.3/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-01 18:07:05.000000 emmet-api-0.55.3/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-06-01 18:07:05.000000 emmet-api-0.55.3/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-01 18:07:05.000000 emmet-api-0.55.3/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:07:11.300487 emmet-api-0.55.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 18:07:05.000000 emmet-api-0.55.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 18:07:05.000000 emmet-api-0.55.3/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.276487 emmet-api-0.55.3/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.276487 emmet-api-0.55.3/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 21:34:20.000000 emmet-api-0.55.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-06 21:34:25.492897 emmet-api-0.55.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-06 21:34:20.000000 emmet-api-0.55.4/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.464896 emmet-api-0.55.4/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.468896 emmet-api-0.55.4/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.468896 emmet-api-0.55.4/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.472896 emmet-api-0.55.4/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.476896 emmet-api-0.55.4/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.480897 emmet-api-0.55.4/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-06 21:34:20.000000 emmet-api-0.55.4/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-06 21:34:25.000000 emmet-api-0.55.4/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-06 21:34:25.000000 emmet-api-0.55.4/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:34:25.000000 emmet-api-0.55.4/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:34:25.000000 emmet-api-0.55.4/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 21:34:25.000000 emmet-api-0.55.4/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 21:34:25.000000 emmet-api-0.55.4/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-06 21:34:20.000000 emmet-api-0.55.4/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-06-06 21:34:20.000000 emmet-api-0.55.4/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-06 21:34:20.000000 emmet-api-0.55.4/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-06-06 21:34:20.000000 emmet-api-0.55.4/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:34:25.492897 emmet-api-0.55.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-06 21:34:20.000000 emmet-api-0.55.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-06 21:34:20.000000 emmet-api-0.55.4/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.468896 emmet-api-0.55.4/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.468896 emmet-api-0.55.4/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.484897 emmet-api-0.55.4/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.488896 emmet-api-0.55.4/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:25.492897 emmet-api-0.55.4/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-06 21:34:20.000000 emmet-api-0.55.4/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.55.3/Dockerfile` & `emmet-api-0.55.4/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM materialsproject/devops:python-3.1010.2 as base
+FROM materialsproject/devops:python-3.1010.4 as base
 RUN apt-get update && apt-get install -y --no-install-recommends libopenblas-dev libjpeg62 && apt-get clean
 
 FROM base as builder
 RUN apt-get update && apt-get install -y --no-install-recommends gcc git g++ cmake make libsnappy-dev wget && apt-get clean
 ENV PATH /root/.local/bin:$PATH
 WORKDIR /emmet-api
 ENV PIP_FLAGS "--user --no-cache-dir --compile"
@@ -27,16 +27,16 @@
 ENV PATH=/root/.local/bin:$PATH \
     PYTHONUNBUFFERED=1 \
     FLASK_APP=emmet-api \
     FLASK_ENV=production \
     PORT=10001 \
     NUM_WORKERS=4 \
     RELOAD="" \
-    MAX_REQUESTS=100000 \
-    MAX_REQUESTS_JITTER=10000 \
+    MAX_REQUESTS=200000 \
+    MAX_REQUESTS_JITTER=20000 \
     DD_TRACE_HOST=localhost:8126 \
     DD_SERVICE=next-gen-api \
     DD_ENV=prod \
     DD_VERSION=$VERSION
 
 COPY app.py .
 COPY material_resources.py .
```

### Comparing `emmet-api-0.55.3/app.py` & `emmet-api-0.55.4/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/core/api.py` & `emmet-api-0.55.4/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.55.4/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.55.4/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/core/documentation.py` & `emmet-api-0.55.4/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/core/global_header.py` & `emmet-api-0.55.4/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/core/settings.py` & `emmet-api-0.55.4/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.55.4/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.55.4/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.55.4/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.55.4/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/dois/resources.py` & `emmet-api-0.55.4/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.55.4/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.55.4/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.55.4/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.55.4/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.55.4/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.55.4/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.55.4/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.55.4/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.55.4/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.55.4/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.55.4/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/utils.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.55.4/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.55.4/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/legacy_resources.py` & `emmet-api-0.55.4/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/material_resources.py` & `emmet-api-0.55.4/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/molecule_resources.py` & `emmet-api-0.55.4/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/requirements/deployment.txt` & `emmet-api-0.55.4/requirements/deployment.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -108,17 +108,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.3
+maggma==0.51.4
     # via emmet-api (emmet/emmet-api/setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via
@@ -161,19 +161,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -201,17 +200,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -244,17 +243,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -308,16 +307,17 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.10.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -85,15 +85,21 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -108,17 +114,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -158,32 +164,33 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.14.1
     # via pymatgen
 protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -197,17 +204,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -240,17 +247,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -303,21 +310,25 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   aioitertools
+    #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
@@ -327,11 +338,13 @@
 werkzeug==2.3.4
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.10_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,46 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -145,24 +145,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -194,15 +194,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -246,19 +246,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -297,23 +296,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -365,17 +364,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -444,16 +443,17 @@
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
 tzdata==2023.3
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.11.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,35 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.2
+exceptiongroup==1.1.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -104,17 +108,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -154,19 +158,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -193,17 +196,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -236,17 +239,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -299,16 +302,17 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,41 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.2
+exceptiongroup==1.1.1
+    # via
+    #   anyio
+    #   cattrs
+    #   pytest
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -140,24 +145,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -189,15 +194,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -241,19 +246,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -292,23 +296,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -360,17 +364,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -421,29 +425,35 @@
     # via pymatgen
 tenacity==8.2.2
     # via
     #   ddtrace
     #   plotly
 threadpoolctl==3.1.0
     # via scikit-learn
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
 tzdata==2023.3
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.8.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -89,17 +89,15 @@
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   opentelemetry-api
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via matplotlib
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -114,17 +112,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -164,34 +162,31 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.14.1
     # via pymatgen
 protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
@@ -205,17 +200,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -248,17 +243,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -311,18 +306,19 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aioitertools
     #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,46 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -154,24 +154,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -203,15 +203,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -255,19 +255,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -308,23 +307,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -376,17 +375,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -455,18 +454,19 @@
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aioitertools
     #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.9.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -112,17 +112,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -162,19 +162,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -201,17 +200,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -244,17 +243,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -307,18 +306,19 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aioitertools
     #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
```

### Comparing `emmet-api-0.55.3/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,46 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -152,24 +152,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -201,15 +201,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -253,19 +253,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -304,23 +303,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -372,17 +371,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -451,18 +450,19 @@
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aioitertools
     #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -108,17 +108,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -158,19 +158,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -197,17 +196,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -240,17 +239,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -303,16 +302,17 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,46 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -111,15 +111,24 @@
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -145,24 +154,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -194,15 +203,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -246,19 +255,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -266,14 +274,16 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.3.2
@@ -297,23 +307,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -365,17 +375,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -444,22 +454,27 @@
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
+    #   aioitertools
+    #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
@@ -477,11 +492,13 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.11.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,35 +40,35 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -104,17 +104,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -154,19 +154,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -193,17 +192,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -236,17 +235,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -299,15 +298,15 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,41 +47,41 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -140,24 +140,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -189,15 +189,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -241,19 +241,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -292,23 +291,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -360,17 +359,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -434,15 +433,15 @@
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.8.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,39 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -114,17 +114,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -164,19 +164,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -205,17 +204,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -248,17 +247,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -311,18 +310,19 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aioitertools
     #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.55.4/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,46 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -118,17 +118,15 @@
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via matplotlib
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -154,24 +152,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -203,15 +201,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -255,19 +253,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -275,16 +272,14 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
 pre-commit==3.3.2
@@ -308,23 +303,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -376,17 +371,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -455,18 +450,19 @@
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   aioitertools
     #   bytecode
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.11.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -40,39 +40,35 @@
 click==8.1.3
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.0.7
     # via matplotlib
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via
-    #   anyio
-    #   cattrs
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -85,19 +81,15 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -112,17 +104,17 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
     # via pymatgen
@@ -162,19 +154,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.2
     # via
@@ -201,17 +192,17 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -244,17 +235,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -307,24 +298,21 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
@@ -334,13 +322,11 @@
 werkzeug==2.3.4
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.3/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.55.4/requirements/macos-latest_py3.11_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.142
+boto3==1.26.147
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.142
+botocore==1.29.147
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
-cattrs==22.2.0
+cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
@@ -47,46 +47,41 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==40.0.2
+cryptography==41.0.1
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.4
+ddtrace==1.14.0
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.2
+emmet-core[all]==0.55.3
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via
-    #   anyio
-    #   cattrs
-    #   pytest
-fastapi==0.95.2
+fastapi==0.96.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -111,22 +106,15 @@
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   mkdocstrings
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -152,24 +140,24 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.1
+maggma==0.51.4
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
     #   werkzeug
 matminer==0.8.0
     # via robocrys
 matplotlib==3.7.1
@@ -201,15 +189,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.1.0
+mkdocstrings-python==1.1.2
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
@@ -253,19 +241,18 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.14
+orjson==3.9.0
     # via maggma
 packaging==23.1
     # via
-    #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
@@ -304,23 +291,23 @@
     # via cffi
 pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.3
+pydash==7.0.4
     # via maggma
 pydocstyle==6.3.0
     # via emmet-api (setup.py)
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via mkdocs-material
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
@@ -372,17 +359,17 @@
     # via maggma
 requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
-robocrys==0.2.7
+robocrys==0.2.8
     # via emmet-core
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -433,44 +420,35 @@
     # via pymatgen
 tenacity==8.2.2
     # via
     #   ddtrace
     #   plotly
 threadpoolctl==3.1.0
     # via scikit-learn
-tomli==2.0.1
-    # via
-    #   coverage
-    #   mypy
-    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 types-requests==2.31.0.1
     # via emmet-api (setup.py)
 types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
-    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
@@ -488,13 +466,11 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.3/setup.py` & `emmet-api-0.55.4/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/_consumer/test_query_operators.py` & `emmet-api-0.55.4/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/_general_store/test_query_operators.py` & `emmet-api-0.55.4/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/core/test_mapi.py` & `emmet-api-0.55.4/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.55.4/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/electrodes/test_utils.py` & `emmet-api-0.55.4/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/materials/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/materials/test_utils.py` & `emmet-api-0.55.4/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/summary/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.55.4/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.55.4/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/synthesis/test_utils.py` & `emmet-api-0.55.4/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/tasks/test_utils.py` & `emmet-api-0.55.4/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/materials/xas/test_query_operators.py` & `emmet-api-0.55.4/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.3/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.55.4/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

