# Comparing `tmp/chalkpy-2.5.9.tar.gz` & `tmp/chalkpy-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalkpy-2.5.9.tar", last modified: Sat Jun  3 02:15:53 2023, max compression
+gzip compressed data, was "chalkpy-2.6.0.tar", last modified: Mon Jun  5 21:58:44 2023, max compression
```

## Comparing `chalkpy-2.5.9.tar` & `chalkpy-2.6.0.tar`

### file list

```diff
@@ -1,940 +1,940 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.538320 chalkpy-2.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-03 02:15:32.000000 chalkpy-2.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-03 02:15:53.538320 chalkpy-2.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-06-03 02:15:32.000000 chalkpy-2.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.462320 chalkpy-2.5.9/chalk/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.462320 chalkpy-2.5.9/chalk/_autosql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_autosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_autosql/autosql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.462320 chalkpy-2.5.9/chalk/_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_monitoring/Chart.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_monitoring/charts_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_monitoring/charts_enums_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_monitoring/charts_series_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_monitoring/gql_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.462320 chalkpy-2.5.9/chalk/_reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/_reporting/rich/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/rich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/rich/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/rich/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_reporting/rich/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_validation/feature_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/client/
--rw-r--r--   0 runner    (1001) docker     (123)    46588 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61742 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27259 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/client/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/client/serialization/query_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/clogging/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/clogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/clogging/chalk_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/config/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/config/project_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/df/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/df/ChalkDataFrameImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/df/ast_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/feature_n/
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/feature_n/feature_1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_1/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/feature_n/feature_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_10/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/feature_n/feature_100/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_100/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_100/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/feature_n/feature_101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_101/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.466321 chalkpy-2.5.9/chalk/feature_n/feature_102/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_102/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_102/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_103/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_103/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_103/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_104/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_104/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_104/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_105/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_105/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_105/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_106/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_106/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_106/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_107/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_107/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_107/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_108/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_108/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_108/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_109/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_109/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_11/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_110/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_110/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_110/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_111/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_111/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_111/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_112/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_112/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_112/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_113/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_113/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_113/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_114/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_115/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_115/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_115/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_116/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_116/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_116/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_117/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_117/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_117/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_118/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_118/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_118/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.470321 chalkpy-2.5.9/chalk/feature_n/feature_119/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_119/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_119/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_12/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_120/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_120/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_120/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_121/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_121/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_121/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_122/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_123/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_123/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_124/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_124/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_124/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_125/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_125/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_126/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_126/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_126/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_127/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_127/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_127/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_128/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_128/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_128/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_129/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_129/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_129/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_13/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_130/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_130/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_131/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_131/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_132/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_132/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_133/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_133/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_133/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.474321 chalkpy-2.5.9/chalk/feature_n/feature_134/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_134/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_134/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_135/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_135/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_135/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_136/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_136/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_136/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_137/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_137/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_137/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_138/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_138/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_138/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_139/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_139/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_139/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_14/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_14/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_140/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_140/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_141/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_141/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_142/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_142/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_142/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_143/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_143/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_143/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_144/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_144/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_144/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_145/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_145/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_145/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_146/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_146/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_146/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_147/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_147/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_147/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_148/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_148/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_148/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.478320 chalkpy-2.5.9/chalk/feature_n/feature_149/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_149/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_149/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_15/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_15/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_150/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_150/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_151/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_151/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_152/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_152/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_153/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_153/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_153/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_154/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_154/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_154/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_155/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_155/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_155/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_156/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_156/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_156/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_157/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_157/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_157/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_158/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_158/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_158/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_159/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_159/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_159/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_16/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_16/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_160/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_160/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_161/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_161/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_161/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_162/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_162/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_162/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_163/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_163/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_163/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.482320 chalkpy-2.5.9/chalk/feature_n/feature_164/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_164/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_164/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_165/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_165/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_165/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_166/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_166/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_167/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_167/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_167/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_168/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_168/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_168/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_169/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_169/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_169/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_17/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_17/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_170/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_170/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_170/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_171/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_171/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_171/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_172/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_172/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_172/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_173/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_173/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_173/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_174/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_174/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_174/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_175/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_175/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_175/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_176/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_176/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_176/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_177/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_177/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_177/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_178/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_178/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_178/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_179/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_179/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_179/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_18/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_18/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_18/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.486320 chalkpy-2.5.9/chalk/feature_n/feature_180/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_180/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_180/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_181/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_181/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_182/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_182/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_182/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_183/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_183/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_183/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_184/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_184/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_184/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_185/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_185/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_185/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_186/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_186/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_186/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_187/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_187/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_187/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_188/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_188/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_188/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_189/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_189/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_189/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_19/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_19/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_19/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_190/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_190/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_190/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_191/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_191/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_191/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_192/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_192/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_192/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_193/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_193/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_193/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_194/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_194/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_194/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_195/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_195/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_195/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_196/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_196/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_196/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_197/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_197/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_197/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.490320 chalkpy-2.5.9/chalk/feature_n/feature_198/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_198/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_198/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_199/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_199/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_199/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_2/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_20/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_200/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_200/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_201/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_201/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_201/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_202/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_202/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_202/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_203/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_203/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_203/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_204/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_204/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_204/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_205/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_205/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_206/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_206/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_206/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_207/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_207/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_207/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_208/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_208/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_208/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_209/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_21/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_21/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_210/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_211/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_211/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_211/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_212/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_212/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_212/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_213/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_213/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_213/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.494320 chalkpy-2.5.9/chalk/feature_n/feature_214/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_214/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_214/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_215/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_215/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_215/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_216/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_216/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_216/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_217/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_217/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_217/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_218/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_218/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_218/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_219/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_219/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_219/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_22/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_220/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_221/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_221/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_221/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_222/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_222/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_223/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_223/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_223/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_224/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_224/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_224/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_225/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_225/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_225/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_226/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_226/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_226/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_227/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_227/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_227/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_228/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_228/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_228/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_229/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_229/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_229/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.498320 chalkpy-2.5.9/chalk/feature_n/feature_23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_23/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_230/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_230/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_230/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_231/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_231/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_232/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_232/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_232/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_233/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_233/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_233/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_234/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_234/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_234/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_235/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_235/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_235/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_236/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_236/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_236/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_237/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_237/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_237/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_238/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_238/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_238/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_239/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_239/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_239/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_24/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_24/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_240/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_240/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_241/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_241/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_241/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.502320 chalkpy-2.5.9/chalk/feature_n/feature_242/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_242/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_242/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_243/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_243/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_243/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_244/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_244/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_244/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_245/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_245/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_245/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_246/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_246/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_246/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_247/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_247/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_247/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_248/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_248/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_248/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_249/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_249/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_249/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_25/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_25/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_250/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_250/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_250/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_251/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_251/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_251/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_252/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_252/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_252/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_253/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_253/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_253/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_254/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_254/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_254/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.506320 chalkpy-2.5.9/chalk/feature_n/feature_255/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_255/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_255/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_256/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_256/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_256/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_26/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_27/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_27/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_28/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_28/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_28/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_29/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_29/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_29/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_3/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_30/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_30/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_30/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_31/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_31/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_32/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_32/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_33/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_34/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_34/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_35/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_35/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_35/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_36/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_36/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_37/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_37/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_38/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_38/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_38/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_39/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_39/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_39/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_4/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.510320 chalkpy-2.5.9/chalk/feature_n/feature_40/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_40/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_41/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_41/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_41/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_42/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_42/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_43/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_43/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_43/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_44/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_44/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_44/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_45/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_45/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_45/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_46/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_46/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_46/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_47/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_47/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_48/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_48/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_48/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_49/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_49/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_49/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_5/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_50/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_50/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_51/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_51/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_51/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_52/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_52/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_52/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_53/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_53/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_54/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_54/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_54/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_55/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_55/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_55/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.514320 chalkpy-2.5.9/chalk/feature_n/feature_56/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_56/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_57/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_57/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_57/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_58/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_58/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_58/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_59/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_59/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_59/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_6/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_60/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_60/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_60/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_61/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_61/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_62/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_62/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_62/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_63/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_63/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_63/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_64/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_64/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_65/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_65/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_65/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_66/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_66/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_66/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_67/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_67/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_67/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_68/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_68/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_68/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_69/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_69/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_69/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_7/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_70/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_70/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_70/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.518320 chalkpy-2.5.9/chalk/feature_n/feature_71/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_71/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_71/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_72/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_72/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_72/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_73/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_73/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_73/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_74/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_74/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_74/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_75/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_75/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_75/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_76/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_76/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_76/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_77/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_77/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_77/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_78/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_78/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_78/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_79/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_79/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_79/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_8/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_80/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_80/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_80/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_81/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_81/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_81/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_82/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_82/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_82/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_83/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_83/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_83/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_84/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_84/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_84/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_85/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_85/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_85/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_86/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_86/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_86/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_87/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_87/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_87/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_88/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_88/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_88/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.522320 chalkpy-2.5.9/chalk/feature_n/feature_89/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_89/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_89/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_9/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_90/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_90/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_90/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_91/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_91/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_91/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_92/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_92/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_92/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_93/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_93/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_93/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_94/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_94/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_94/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_95/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_95/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_95/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_96/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_96/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_96/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_97/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_97/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_97/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_98/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_98/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_98/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.526320 chalkpy-2.5.9/chalk/feature_n/feature_99/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_99/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/feature_n/feature_99/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_chalkop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_class_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/features/_encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/missing_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/_encoding/serialized_dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/features/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/dataframe/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    55087 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/dataframe/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/dataframe/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/feature_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/feature_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/feature_set_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/feature_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/feature_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/live_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/pseudofeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    69931 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/features/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/gitignore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/gitignore/gitignore_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/gitignore/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/integrations/named.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/mypy_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.530320 chalkpy-2.5.9/chalk/parsed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/parsed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/parsed/_graph_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/parsed/duplicate_input_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/parsed/json_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/parsed/user_types_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/serialization/parsed_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/sink/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sink/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    30340 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/sql/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/incremental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/sql/_internal/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/sql/_internal/integrations/psycopg3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/psycopg3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/integrations/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    24571 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/sql_file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/sql_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/_internal/string_chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/finalized_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/sql/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/streams/
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/_file_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/_kafka_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/_kinesis_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/streams/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.534320 chalkpy-2.5.9/chalk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.538320 chalkpy-2.5.9/chalk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/annotation_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/cached_type_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/collection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/environment_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/log_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/metaprogramming.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/missing_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-06-03 02:15:32.000000 chalkpy-2.5.9/chalk/utils/stubgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 02:15:53.538320 chalkpy-2.5.9/chalkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-03 02:15:53.000000 chalkpy-2.5.9/chalkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-06-03 02:15:32.000000 chalkpy-2.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 02:15:53.538320 chalkpy-2.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-03 02:15:32.000000 chalkpy-2.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.114300 chalkpy-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 21:58:23.000000 chalkpy-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-05 21:58:44.114300 chalkpy-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-06-05 21:58:23.000000 chalkpy-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.018299 chalkpy-2.6.0/chalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.018299 chalkpy-2.6.0/chalk/_autosql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_autosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_autosql/autosql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.018299 chalkpy-2.6.0/chalk/_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_monitoring/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_monitoring/charts_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_monitoring/charts_enums_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_monitoring/charts_series_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_monitoring/gql_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.018299 chalkpy-2.6.0/chalk/_reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.018299 chalkpy-2.6.0/chalk/_reporting/rich/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/rich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/rich/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/rich/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_reporting/rich/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.018299 chalkpy-2.6.0/chalk/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_validation/feature_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    46608 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61704 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27259 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/client/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/client/serialization/query_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/clogging/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/clogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/clogging/chalk_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/config/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/config/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/df/ChalkDataFrameImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/df/ast_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/feature_n/
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/feature_n/feature_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_1/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/feature_n/feature_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_10/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/feature_n/feature_100/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_100/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_100/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/feature_n/feature_101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_101/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.022299 chalkpy-2.6.0/chalk/feature_n/feature_102/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_102/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_102/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_103/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_103/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_103/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_104/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_104/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_104/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_105/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_105/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_105/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_106/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_106/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_106/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_107/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_107/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_107/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_108/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_108/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_108/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_109/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_109/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_11/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_110/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_110/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_110/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_111/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_111/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_111/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_112/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_112/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_112/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_113/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_113/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_113/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.026299 chalkpy-2.6.0/chalk/feature_n/feature_114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_114/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_115/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_115/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_115/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_116/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_116/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_116/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_117/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_118/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_118/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_118/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_119/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_119/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_119/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_12/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_120/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_120/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_120/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_121/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_121/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_121/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_122/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_123/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_123/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_124/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_124/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_124/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_125/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.030299 chalkpy-2.6.0/chalk/feature_n/feature_126/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_126/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_126/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_127/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_127/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_127/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_128/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_128/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_128/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_129/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_129/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_129/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_13/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_130/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_131/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_131/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_132/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_133/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_133/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_133/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_134/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_134/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_134/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_135/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_135/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_135/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_136/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_136/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_136/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_137/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_137/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_137/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.034299 chalkpy-2.6.0/chalk/feature_n/feature_138/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_138/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_138/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_139/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_139/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_139/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_14/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_14/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_140/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_141/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_142/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_142/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_142/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_143/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_143/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_143/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_144/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_144/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_144/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_145/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_145/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_145/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_146/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_146/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_146/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_147/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_147/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_147/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_148/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_148/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_148/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_149/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_149/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_149/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.038299 chalkpy-2.6.0/chalk/feature_n/feature_15/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_15/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_150/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_151/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_152/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_153/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_153/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_153/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_154/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_154/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_154/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_155/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_155/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_155/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_156/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_156/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_156/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_157/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_157/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_157/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_158/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_158/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_158/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_159/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_159/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_159/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_16/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_16/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_160/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.042299 chalkpy-2.6.0/chalk/feature_n/feature_161/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_161/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_161/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_162/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_162/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_162/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_163/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_163/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_163/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_164/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_164/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_164/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_165/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_165/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_165/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_166/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_166/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_167/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_167/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_167/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_168/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_168/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_168/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_169/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_169/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_169/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_17/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_17/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_170/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_170/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_170/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_171/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_171/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_171/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.046299 chalkpy-2.6.0/chalk/feature_n/feature_172/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_172/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_172/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_173/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_173/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_173/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_174/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_174/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_174/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_175/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_175/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_175/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_176/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_176/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_176/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_177/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_177/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_177/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_178/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_178/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_178/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_179/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_179/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_179/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_18/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_18/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_180/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_180/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_180/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_181/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_181/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_182/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_182/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_182/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.050299 chalkpy-2.6.0/chalk/feature_n/feature_183/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_183/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_183/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_184/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_184/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_184/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_185/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_185/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_185/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_186/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_186/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_186/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_187/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_187/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_187/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_188/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_188/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_188/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_189/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_189/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_189/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_19/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_19/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_19/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_190/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_190/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_190/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_191/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_191/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_191/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_192/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_192/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_192/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_193/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_193/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_193/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_194/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_194/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_194/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.054299 chalkpy-2.6.0/chalk/feature_n/feature_195/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_195/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_195/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_196/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_196/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_196/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_197/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_197/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_197/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_198/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_198/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_198/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_199/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_199/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_199/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_2/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_20/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_200/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_200/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_201/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_201/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_201/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_202/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_202/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_202/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_203/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_203/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_203/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_204/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_204/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_204/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_205/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_205/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.058299 chalkpy-2.6.0/chalk/feature_n/feature_206/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_206/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_206/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_207/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_207/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_207/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_208/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_208/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_208/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_209/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_21/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_210/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_211/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_211/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_211/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_212/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_212/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_212/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_213/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_213/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_213/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_214/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_214/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_214/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_215/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_215/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_215/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_216/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_216/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_216/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.062299 chalkpy-2.6.0/chalk/feature_n/feature_217/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_217/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_217/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_218/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_218/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_218/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_219/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_219/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_219/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_22/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_220/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_221/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_221/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_221/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_222/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_222/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_223/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_223/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_223/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_224/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_224/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_224/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_225/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_225/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_225/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_226/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_226/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_226/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_227/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_227/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_227/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_228/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_228/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_228/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_229/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_229/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_229/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_23/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_230/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_230/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_230/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.066299 chalkpy-2.6.0/chalk/feature_n/feature_231/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_231/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_232/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_232/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_232/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_233/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_233/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_233/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_234/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_234/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_234/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_235/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_235/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_235/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_236/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_236/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_236/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_237/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_237/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_237/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_238/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_238/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_238/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_239/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_239/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_239/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_24/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_24/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_240/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_241/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_241/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_241/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_242/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_242/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_242/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_243/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_243/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_243/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.070299 chalkpy-2.6.0/chalk/feature_n/feature_244/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_244/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_244/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_245/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_245/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_245/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_246/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_246/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_246/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_247/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_247/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_247/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_248/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_248/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_248/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_249/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_249/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_249/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_25/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_25/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_250/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_250/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_250/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_251/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_251/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_251/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_252/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_252/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_252/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_253/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_253/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_253/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_254/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_254/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_254/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_255/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_255/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_255/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_256/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_256/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_256/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_26/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_27/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_27/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.074299 chalkpy-2.6.0/chalk/feature_n/feature_28/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_28/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_28/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_29/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_29/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_29/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_3/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_30/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_30/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_30/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_31/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_32/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_32/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_33/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_34/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_34/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_35/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_35/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_35/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_36/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_36/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_37/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_37/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_38/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_38/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_38/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_39/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_39/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_39/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_4/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_40/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_40/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_41/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_41/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_41/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_42/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_42/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.078299 chalkpy-2.6.0/chalk/feature_n/feature_43/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_43/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_43/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_44/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_44/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_44/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_45/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_45/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_45/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_46/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_46/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_46/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_47/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_48/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_48/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_48/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_49/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_49/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_49/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_5/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_50/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_50/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_51/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_51/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_51/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_52/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_52/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_52/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_53/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_53/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_54/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_54/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_54/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.082299 chalkpy-2.6.0/chalk/feature_n/feature_55/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_55/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_55/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_56/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_56/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_57/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_57/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_57/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_58/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_58/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_58/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_59/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_59/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_59/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_6/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_60/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_60/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_60/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_61/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_61/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_62/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_62/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_62/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_63/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_63/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_63/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_64/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_64/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_65/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_65/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_65/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_66/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_66/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_66/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.086299 chalkpy-2.6.0/chalk/feature_n/feature_67/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_67/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_67/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_68/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_68/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_69/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_69/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_69/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_7/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_70/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_70/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_70/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_71/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_71/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_71/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_72/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_72/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_72/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_73/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_73/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_73/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_74/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_74/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_74/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_75/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_75/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_75/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_76/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_76/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_76/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_77/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_77/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_77/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_78/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_78/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_78/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.090299 chalkpy-2.6.0/chalk/feature_n/feature_79/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_79/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_79/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_8/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_80/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_80/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_80/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_81/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_81/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_81/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_82/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_82/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_83/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_83/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_83/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_84/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_84/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_84/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_85/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_85/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_85/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_86/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_86/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_86/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_87/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_87/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_87/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_88/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_88/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_88/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_89/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_89/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_9/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.094299 chalkpy-2.6.0/chalk/feature_n/feature_90/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_90/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_90/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_91/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_91/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_91/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_92/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_92/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_92/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_93/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_93/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_93/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_94/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_94/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_94/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_95/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_95/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_95/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_96/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_96/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_96/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_97/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_97/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_97/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_98/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_98/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_98/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.098299 chalkpy-2.6.0/chalk/feature_n/feature_99/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_99/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/feature_n/feature_99/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_chalkop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_class_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/features/_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/missing_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/_encoding/serialized_dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/features/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/dataframe/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58896 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/dataframe/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/dataframe/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/feature_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/feature_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/feature_set_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/feature_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/feature_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/live_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/pseudofeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69931 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/features/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/gitignore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/gitignore/gitignore_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/gitignore/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/integrations/named.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.102300 chalkpy-2.6.0/chalk/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/mypy_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.106299 chalkpy-2.6.0/chalk/parsed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/parsed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/parsed/_graph_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/parsed/duplicate_input_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/parsed/json_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/parsed/user_types_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.106299 chalkpy-2.6.0/chalk/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/serialization/parsed_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.106299 chalkpy-2.6.0/chalk/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sink/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.106299 chalkpy-2.6.0/chalk/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    30340 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.106299 chalkpy-2.6.0/chalk/sql/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.106299 chalkpy-2.6.0/chalk/sql/_internal/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.110299 chalkpy-2.6.0/chalk/sql/_internal/integrations/psycopg3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/psycopg3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/integrations/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24588 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/sql_file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/sql_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/_internal/string_chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/finalized_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/sql/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.110299 chalkpy-2.6.0/chalk/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/_kafka_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/_kinesis_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/streams/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.110299 chalkpy-2.6.0/chalk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.110299 chalkpy-2.6.0/chalk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/annotation_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/cached_type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/environment_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/log_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/metaprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/missing_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-06-05 21:58:23.000000 chalkpy-2.6.0/chalk/utils/stubgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:58:44.110299 chalkpy-2.6.0/chalkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-05 21:58:43.000000 chalkpy-2.6.0/chalkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-06-05 21:58:23.000000 chalkpy-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:58:44.114300 chalkpy-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-05 21:58:23.000000 chalkpy-2.6.0/setup.py
```

### Comparing `chalkpy-2.5.9/PKG-INFO` & `chalkpy-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalkpy
-Version: 2.5.9
+Version: 2.6.0
 Summary: Python SDK for Chalk
 Author: Chalk AI, Inc.
 Project-URL: homepage, https://chalk.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `chalkpy-2.5.9/README.md` & `chalkpy-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/__init__.py` & `chalkpy-2.6.0/chalk/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_autosql/autosql.py` & `chalkpy-2.6.0/chalk/_autosql/autosql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_monitoring/Chart.py` & `chalkpy-2.6.0/chalk/_monitoring/Chart.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_monitoring/charts_codegen.py` & `chalkpy-2.6.0/chalk/_monitoring/charts_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_monitoring/charts_enums_codegen.py` & `chalkpy-2.6.0/chalk/_monitoring/charts_enums_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_monitoring/charts_series_base.py` & `chalkpy-2.6.0/chalk/_monitoring/charts_series_base.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_monitoring/gql_conversion.py` & `chalkpy-2.6.0/chalk/_monitoring/gql_conversion.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_reporting/models.py` & `chalkpy-2.6.0/chalk/_reporting/models.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_reporting/progress.py` & `chalkpy-2.6.0/chalk/_reporting/progress.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_reporting/rich/live.py` & `chalkpy-2.6.0/chalk/_reporting/rich/live.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/_validation/validation.py` & `chalkpy-2.6.0/chalk/_validation/validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/cli.py` & `chalkpy-2.6.0/chalk/cli.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/client/__init__.py` & `chalkpy-2.6.0/chalk/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1246,15 +1246,15 @@
             and the branch exists, then that branch will be deployed
             to.
         source_deployment_id
             (Optional) the specific deployment ID to use for the
             branch. If not specified, the latest live deployment on
             the server will be used. You can see which deployments
             are available by clicking on the 'Deployments' tab on
-            the project page in the Chalk UI.
+            the project page in the Chalk dashboard.
         environment
             The environment under which to create the branch. API
             tokens can be scoped to an environment. If no environment
             is specified in the query, the environment will be taken
             from the client's cached token.
         """
         ...
@@ -1291,15 +1291,15 @@
             The name of the branch to use
         """
         ...
 
     def __new__(cls, *args: Any, **kwargs: Any):
         from chalk.client.client_impl import ChalkAPIClientImpl
 
-        return ChalkAPIClientImpl(*args, **kwargs)
+        return ChalkAPIClientImpl.__new__(cls, *args, **kwargs)
 
 
 ChalkAPIClientProtocol: TypeAlias = ChalkClient
 """Deprecated. Use `ChalkClient` instead."""
 
 __all__ = [
     "ChalkAPIClientProtocol",
```

### Comparing `chalkpy-2.5.9/chalk/client/client_impl.py` & `chalkpy-2.6.0/chalk/client/client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,14 @@
         branch_text = ""
         if self._config.branch is not None:
             branch_text = f", branch='{self._config.branch}'"
         return f"chalk.client.ChalkClient<{self._config.name}{branch_text}>"
 
     def __new__(cls, *args: Any, **kwargs: Any) -> ChalkClient:
         obj = object.__new__(ChalkAPIClientImpl)
-        obj.__init__(*args, **kwargs)
         return obj
 
     def __init__(
         self,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         environment: Optional[EnvironmentId] = None,
```

### Comparing `chalkpy-2.5.9/chalk/client/dataset.py` & `chalkpy-2.6.0/chalk/client/dataset.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/client/exc.py` & `chalkpy-2.6.0/chalk/client/exc.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/client/models.py` & `chalkpy-2.6.0/chalk/client/models.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/client/serialization/query_serialization.py` & `chalkpy-2.6.0/chalk/client/serialization/query_serialization.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/config/auth_config.py` & `chalkpy-2.6.0/chalk/config/auth_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/config/project_config.py` & `chalkpy-2.6.0/chalk/config/project_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/df/ast_parser.py` & `chalkpy-2.6.0/chalk/df/ast_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/__init__.py` & `chalkpy-2.6.0/chalk/feature_n/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/codegen.py` & `chalkpy-2.6.0/chalk/feature_n/codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_10/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_10/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_100/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_100/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_101/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_101/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_102/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_102/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_103/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_103/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_104/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_104/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_105/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_105/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_106/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_106/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_107/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_107/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_108/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_108/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_109/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_109/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_11/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_11/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_110/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_110/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_111/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_111/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_112/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_112/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_113/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_113/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_114/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_114/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_115/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_115/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_116/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_116/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_117/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_117/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_118/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_118/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_119/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_119/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_12/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_12/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_120/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_120/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_121/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_121/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_122/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_122/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_123/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_123/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_124/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_124/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_125/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_125/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_126/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_126/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_127/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_127/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_128/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_128/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_129/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_129/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_13/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_13/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_130/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_130/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_131/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_131/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_132/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_132/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_133/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_133/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_134/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_134/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_135/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_135/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_136/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_136/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_137/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_137/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_138/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_138/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_139/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_139/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_14/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_14/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_140/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_140/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_141/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_141/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_142/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_142/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_143/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_143/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_144/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_144/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_145/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_145/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_146/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_146/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_147/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_147/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_148/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_148/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_149/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_149/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_15/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_15/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_150/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_150/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_151/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_151/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_152/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_152/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_153/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_153/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_154/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_154/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_155/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_155/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_156/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_156/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_157/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_157/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_158/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_158/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_159/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_159/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_16/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_16/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_160/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_160/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_161/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_161/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_162/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_162/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_163/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_163/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_164/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_164/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_165/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_165/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_166/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_166/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_167/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_167/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_168/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_168/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_169/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_169/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_17/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_17/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_170/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_170/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_171/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_171/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_172/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_172/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_173/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_173/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_174/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_174/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_175/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_175/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_176/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_176/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_177/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_177/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_178/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_178/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_179/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_179/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_18/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_18/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_180/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_180/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_181/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_181/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_182/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_182/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_183/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_183/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_184/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_184/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_185/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_185/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_186/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_186/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_187/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_187/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_188/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_188/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_189/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_189/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_19/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_19/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_190/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_190/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_191/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_191/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_192/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_192/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_193/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_193/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_194/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_194/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_195/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_195/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_196/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_196/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_197/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_197/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_198/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_198/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_199/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_199/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_20/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_20/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_200/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_200/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_201/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_201/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_202/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_202/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_203/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_203/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_204/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_204/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_205/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_205/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_206/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_206/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_207/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_207/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_208/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_208/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_209/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_209/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_21/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_21/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_210/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_210/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_211/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_211/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_212/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_212/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_213/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_213/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_214/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_214/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_215/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_215/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_216/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_216/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_217/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_217/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_218/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_218/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_219/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_219/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_22/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_22/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_220/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_220/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_221/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_221/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_222/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_222/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_223/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_223/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_224/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_224/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_225/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_225/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_226/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_226/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_227/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_227/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_228/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_228/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_229/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_229/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_23/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_23/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_230/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_230/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_231/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_231/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_232/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_232/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_233/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_233/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_234/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_234/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_235/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_235/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_236/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_236/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_237/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_237/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_238/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_238/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_239/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_239/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_24/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_24/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_240/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_240/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_241/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_241/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_242/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_242/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_243/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_243/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_244/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_244/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_245/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_245/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_246/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_246/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_247/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_247/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_248/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_248/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_249/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_249/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_25/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_25/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_250/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_250/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_251/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_251/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_252/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_252/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_253/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_253/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_254/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_254/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_255/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_255/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_256/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_256/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_26/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_26/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_27/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_27/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_28/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_28/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_29/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_29/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_30/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_30/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_31/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_31/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_32/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_32/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_33/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_33/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_34/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_34/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_35/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_35/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_36/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_36/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_37/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_37/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_38/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_38/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_39/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_39/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_40/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_40/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_41/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_41/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_42/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_42/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_43/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_43/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_44/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_44/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_45/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_45/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_46/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_46/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_47/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_47/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_48/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_48/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_49/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_49/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_50/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_50/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_51/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_51/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_52/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_52/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_53/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_53/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_54/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_54/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_55/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_55/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_56/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_56/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_57/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_57/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_58/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_58/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_59/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_59/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_60/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_60/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_61/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_61/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_62/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_62/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_63/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_63/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_64/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_64/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_65/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_65/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_66/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_66/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_67/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_67/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_68/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_68/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_69/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_69/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_7/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_7/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_70/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_70/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_71/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_71/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_72/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_72/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_73/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_73/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_74/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_74/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_75/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_75/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_76/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_76/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_77/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_77/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_78/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_78/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_79/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_79/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_8/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_8/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_80/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_80/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_81/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_81/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_82/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_82/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_83/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_83/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_84/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_84/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_85/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_85/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_86/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_86/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_87/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_87/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_88/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_88/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_89/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_89/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_9/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_9/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_90/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_90/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_91/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_91/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_92/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_92/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_93/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_93/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_94/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_94/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_95/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_95/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_96/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_96/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_97/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_97/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_98/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_98/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/feature_n/feature_99/feature.py` & `chalkpy-2.6.0/chalk/feature_n/feature_99/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/__init__.py` & `chalkpy-2.6.0/chalk/features/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/_chalkop.py` & `chalkpy-2.6.0/chalk/features/_chalkop.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/_class_property.py` & `chalkpy-2.6.0/chalk/features/_class_property.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/_encoding/converter.py` & `chalkpy-2.6.0/chalk/features/_encoding/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def __init__(
         self,
         name: str,
         is_nullable: bool,
         rich_default: Union[_TRich, ellipsis] = ...,
         primitive_default: Union[_TPrim, ellipsis] = ...,
         rich_type: Union[Type[_TRich], ellipsis] = ...,
-        pyarrow_dtype: Optional[pa.DataType] = None,
+        pyarrow_dtype: Optional[pa.DataType[Any]] = None,
         encoder: Optional[TEncoder[_TPrim, _TRich]] = None,
         decoder: Optional[TDecoder[_TPrim, _TRich]] = None,
     ) -> None:
         self._name = name
         self._rich_type = unwrap_annotated_if_needed(rich_type)
         if pyarrow_dtype is None:
             if rich_type is ...:
```

### Comparing `chalkpy-2.5.9/chalk/features/_encoding/inputs.py` & `chalkpy-2.6.0/chalk/features/_encoding/inputs.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/_encoding/json.py` & `chalkpy-2.6.0/chalk/features/_encoding/json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/_encoding/pyarrow.py` & `chalkpy-2.6.0/chalk/features/_encoding/pyarrow.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/_encoding/rich.py` & `chalkpy-2.6.0/chalk/features/_encoding/rich.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from datetime import date, datetime, time, timedelta
 from typing import Any, FrozenSet, List, Set, Tuple, Type, TypeVar, Union, cast
 
 import attrs
 import cattrs
 import dateutil.parser
 import isodate
+import pydantic
 from pydantic import BaseModel
 from typing_extensions import get_args, get_origin, is_typeddict
 
 from chalk.features._encoding.primitive import TPrimitive
 from chalk.utils.cached_type_hints import cached_get_type_hints
 from chalk.utils.collections import is_namedtuple, unwrap_optional_and_annotated_if_needed
 from chalk.utils.enum import get_enum_value_type
@@ -336,14 +337,21 @@
                 return True
         if np and isinstance(obj, np.bool_):
             return bool(obj)
         raise ValueError(
             f"Cannot convert {obj} to a boolean. Allowed values are y, yes, t, true, 1, n, no, f, false, 0."
         )
 
+    if (
+        isinstance(obj, (list, set, frozenset, dict, tuple, pydantic.BaseModel))
+        or dataclasses.is_dataclass(obj)
+        or attrs.has(type(obj))
+    ):
+        raise ValueError(f"Object {obj} of type {type(obj).__name__} cannot be converted into a {typ.__name__}")
+
     return typ(obj)
 
 
 _rich_converter.register_structure_hook(int, _structure_rich)
 _rich_converter.register_structure_hook(float, _structure_rich)
 _rich_converter.register_structure_hook(bytes, _structure_rich)
 _rich_converter.register_structure_hook(str, _structure_rich)
```

### Comparing `chalkpy-2.5.9/chalk/features/_encoding/serialized_dtype.py` & `chalkpy-2.6.0/chalk/features/_encoding/serialized_dtype.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/dataframe/_filters.py` & `chalkpy-2.6.0/chalk/features/dataframe/_filters.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/dataframe/_impl.py` & `chalkpy-2.6.0/chalk/features/dataframe/_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,203 +201,22 @@
         namespaces = [x.path[0].parent.namespace if len(x.path) > 0 else x.namespace for x in cls.columns]
         # Remove the pseudo-columns
         namespaces = [x for x in namespaces if not x.startswith("__chalk__")]
         return get_unique_item(namespaces, f"dataframe {cls.__name__} column namespaces")
 
 
 class DataFrame(metaclass=DataFrameMeta):
+
     filters: ClassVar[Tuple[Filter, ...]] = ()
     columns: Tuple[Feature, ...]  # set via a @property on the metaclass
     __columns__: ClassVar[Tuple[Feature, ...]] = ()
     references_feature_set: Optional[Type[Features]]  # set via a @property on the metaclass
     __references_feature_set__: ClassVar[Optional[Type[Features]]] = None
     __pydantic_model__: ClassVar[Optional[Type[BaseModel]]] = None
 
-    def join(
-        self,
-        df: DataFrame,
-        on: Any | List[Any],
-        how: Literal["inner", "left", "outer"] = "left",
-    ) -> DataFrame:
-        on = ensure_tuple(on)
-        p = self._underlying.join(
-            df._underlying,
-            on=[str(t) for t in on],
-            how=how,
-        )
-        return DataFrame(p)
-
-    def group_by(
-        self,
-        group: Mapping[Union[Feature, Any], Union[Feature, Any]],
-        agg: Mapping[Any, Any],
-    ) -> DataFrame:
-        """
-        Parameters
-        ----------
-        group
-            A mapping from the desired column name in the resulting `DataFrame`
-            to the name of the column in the source `DataFrame`.
-        agg
-            A mapping from the desired column name in the resulting `DataFrame`
-            to the aggregation operation to perform on the source `DataFrame`.
-
-        Returns
-        -------
-        DataFrame
-            The `DataFrame` with the specified aggregations applied.
-        """
-        import polars as pl
-
-        from chalk.features.feature_set import FeatureSetBase
-
-        group = [pl.col(str(v)).alias(str(k)) for k, v in group.items()]
-        materialized = self._materialize()
-
-        namespaces = {unwrap_feature(a).namespace for a in agg.keys()}
-        namespace = namespaces.pop() if len(namespaces) == 1 else None
-        timestamp_feature = None if namespace is None else FeatureSetBase.registry[namespace].__chalk_ts__
-
-        now = datetime.now(tz=timezone.utc)
-        cols = []
-        operation: Aggregation
-        for alias, operation in agg.items():
-            # if isinstance(operation, int):
-            #     operation = op.count(FeatureWrapper.len_registry[operation])
-            # c = pl.col(str(operation.col))
-            c = operation.col
-            if len(operation.filters) > 0:
-                c = c.filter(
-                    convert_filters_to_pl_expr(
-                        operation.filters,
-                        self._underlying.schema,
-                        timestamp_feature,
-                        now,
-                    )
-                )
-
-            cols.append(operation.fn(c).alias(str(alias)))
-
-        agged = materialized.lazy().groupby(group).agg(cols).collect()
-
-        return DataFrame(
-            agged,
-            convert_dtypes=self._convert_dtypes,
-            pydantic_model=self._pydantic_model,
-        )
-
-    def vstack(self, other: DataFrame) -> DataFrame:
-        return DataFrame(
-            self._underlying.collect().vstack(other._underlying.collect()).lazy(),
-            convert_dtypes=self._convert_dtypes,
-            pydantic_model=self._pydantic_model,
-        )
-
-    def rename(self, mapping: Mapping[Any, Any]) -> DataFrame:
-        """Rename columns in the `DataFrame`.
-
-        Parameters
-        ----------
-        mapping
-            A mapping from the current feature for a column to the desired
-            feature for the column.
-
-        Returns
-        -------
-        DataFrame
-            The `DataFrame` with the specified columns renamed.
-
-        Examples
-        --------
-        >>> df = DataFrame([
-        ...     User(id=1, first="Sam", last="Wu"),
-        ...     User(id=2, first="Iris", last="Xi")
-        ... ]).rename({User.last: User.family})
-        """
-        return DataFrame(
-            self._underlying.rename({unwrap_feature(k).fqn: unwrap_feature(v).fqn for k, v in mapping.items()}),
-            convert_dtypes=self._convert_dtypes,
-            pydantic_model=self._pydantic_model,
-        )
-
-    def with_columns(self, c: Mapping[Any, Any]) -> DataFrame:
-        """Add columns to the `DataFrame`.
-
-        Parameters
-        ----------
-        c
-            A `Mapping` from the desired name of the column
-            in the `DataFrame` to the definition of the new
-            column.
-
-        Examples
-        --------
-        >>> df = DataFrame([
-        ...     User(id=1, first="Sam", last="Wu"),
-        ...     User(id=2, first="Iris", last="Xi")
-        ... ])
-        >>> # Set the fraud score to 0 for all users
-        >>> df.with_columns({User.fraud_score: 0})
-        >>> # Create a full name as the concatenation of first & last
-        >>> df.with_columns({
-        ...     User.full_name: op.concat(User.first, User.last)
-        ... })
-        >>> # Alias a column name
-        >>> df.with_columns({
-        ...     User.first_name: User.first
-        ... })
-
-
-        Returns
-        -------
-        DataFrame
-            A new `DataFrame` with all the existing columns,
-            plus those specified in this function.
-        """
-        import polars as pl
-
-        from chalk.features.feature_set import FeatureSetBase
-
-        namespaces = {unwrap_feature(a).namespace for a in c.keys()}
-        namespace = namespaces.pop() if len(namespaces) == 1 else None
-        timestamp_feature = None if namespace is None else FeatureSetBase.registry[namespace].__chalk_ts__
-
-        now = datetime.now(tz=timezone.utc)
-        cols = []
-        for alias, operation in c.items():
-            # if isinstance(operation, int):
-            #     operation = op.count(FeatureWrapper.len_registry[operation])
-            # c = pl.col(str(operation.col))
-
-            if isinstance(operation, Aggregation):
-                c = operation.col
-                if len(operation.filters) > 0:
-                    c = c.filter(
-                        convert_filters_to_pl_expr(
-                            operation.filters,
-                            self._underlying.schema,
-                            timestamp_feature,
-                            now,
-                        )
-                    )
-
-                cols.append(operation.fn(c).alias(str(alias)))
-            elif isinstance(operation, FeatureWrapper):
-                cols.append(pl.col(str(operation)).alias(str(alias)))
-            else:
-                cols.append(pl.lit(operation).alias(str(alias)))
-
-        agged = self._materialize().lazy().with_columns(cols).collect()
-
-        return DataFrame(
-            agged,
-            convert_dtypes=self._convert_dtypes,
-            pydantic_model=self._pydantic_model,
-        )
-
     def __init__(
         self,
         data: Union[
             Dict[Union[str, Feature, Any], Sequence[Any]],
             Sequence[Union[Features, Any]],
             pl.DataFrame,
             pl.LazyFrame,
@@ -409,14 +228,15 @@
         pandas_dataframe: Optional[pd.DataFrame] = None,  # For backwards compatibility
         # By default, data should match the dtype of the feature.
         # However, when doing comparisons, data will be converted to bools,
         # in which case the data types should no longer be converted.
         # This is an undocumented parameter, so it does not appear in the docstring
         convert_dtypes: bool = True,
         pydantic_model: Optional[Type[BaseModel]] = None,
+        verify_validity: bool = True,
     ):
         """Construct a Chalk `DataFrame`.
 
         Parameters
         ----------
         data
             The data. Can be an existing `pandas.DataFrame`,
@@ -426,38 +246,47 @@
         missing_value_strategy
             The strategy to use to handle missing values.
 
             A feature value is "missing" if it is an ellipsis (`...`),
             or it is `None` and the feature is not annotated as `Optional[...]`.
 
             The available strategies are:
-                `'error'`: Raise a `TypeError` if any missing values are found.
+                - `'error'`: Raise a `TypeError` if any missing values are found.
                     Do not attempt to replace missing values with the default
                     value for the feature.
-                `'default_or_error'`: If the feature has a default value, then
+                - `'default_or_error'`: If the feature has a default value, then
                     replace missing values with the default value for the feature.
                     Otherwise, raise a `TypeError`.
-                `'default_or_allow'`:  If the feature has a default value, then
+                - `'default_or_allow'`:  If the feature has a default value, then
                     replace missing values with the default value for the feature.
                     Otherwise, leave it as `None`. This is the default strategy.
-                `'allow'`: Allow missing values to be stored in the `DataFrame`.
+                - `'allow'`: Allow missing values to be stored in the `DataFrame`.
                     This option may result non-nullable features being assigned
                     `None` values.
 
         Examples
         --------
+        Row-wise construction
+
         >>> df = DataFrame([
         ...     User(id=1, first="Sam", last="Wu"),
         ...     User(id=2, first="Iris", last="Xi")
         ... ])
+
+        Column-wise construction
+
         >>> df = DataFrame({
         ...     User.id: [1, 2],
         ...     User.first: ["Sam", "Iris"],
         ...     User.last: ["Wu", "Xi"]
         ... })
+
+        Construction from `polars.DataFrame`
+
+        >>> import polars
         >>> df = DataFrame(polars.DataFrame({
         ...     "user.id": [1, 2],
         ...     "user.first": ["Sam", "Iris"],
         ...     "user.last": ["Wu", "Xi"]
         ... }))
         """
         from chalk.features.feature_set import Features, FeatureSetBase
@@ -584,15 +413,16 @@
                 )
         else:
             self.columns = ()
 
         # Convert columns to the correct dtype to match the fqn
         if self._pydantic_model is None and convert_dtypes:
             underlying = validate_df_schema(underlying)
-            underlying = validate_nulls(underlying, missing_value_strategy=missing_value_strategy)
+            if verify_validity:
+                underlying = validate_nulls(underlying, missing_value_strategy=missing_value_strategy)
 
         if isinstance(underlying, pl.DataFrame):
             underlying = underlying.lazy()
         self._underlying = underlying
 
         # Remove the pseudo-features when determining the namespace
         namespaces = (x.path[0].parent.namespace if len(x.path) > 0 else x.namespace for x in self.columns)
@@ -601,43 +431,360 @@
             self.namespace = get_unique_item(namespaces_set, f"dataframe column namespaces")
             self.references_feature_set = FeatureSetBase.registry[self.namespace]
         else:
             # Allow empty dataframes or dataframes with multiple namespaces
             self.namespace = None
             self.references_feature_set = None
 
+    #######################
+    # Filtering / Selecting
+    #######################
+    def __getitem__(self, item: Any) -> DataFrame:
+        """Filter the rows of a `DataFrame` or project out columns.
+
+        You can select columns out of a `DataFrame` from
+        the set of columns already present to produce a new
+        `DataFrame` scoped down to those columns.
+
+        Or, you can filter the rows of a `DataFrame` by using
+        Python's built-in operations on feature columns.
+
+        Parameters
+        ----------
+        item
+            The item to filter or project by.
+
+        Returns
+        -------
+        DataFrame
+            The filtered `DataFrame`.
+
+        Examples
+        --------
+        >>> df = DataFrame({
+        ...     User.age: [21, 22, 23],
+        ...     User.email: [...],
+        ... })
+
+        Filtering
+
+        >>> df = df[
+        ...     User.age > 21 and
+        ...     User.email == "joe@chalk.ai"
+        ... ]
+
+        Projecting
+
+        >>> df[User.name]
+
+        Filtering & Projecting
+
+        >>> df = df[
+        ...     User.age > 21 and
+        ...     User.email == "joe@chalk.ai",
+        ...     User.name
+        ... ]
+        """
+        if isinstance(item, int) and not isinstance(item, bool):
+            if item >= 0:
+                l = len(self)
+                if item >= l:
+                    raise IndexError(f"Index {item} out of range (length {l})")
+                underlying = self._underlying.head(item + 1).tail(1)
+            else:
+                underlying = self._underlying.tail(-item).head(1)
+
+            df = DataFrame(
+                underlying,
+                convert_dtypes=False,
+                pydantic_model=self._pydantic_model,
+            )
+            return list(df.to_features())[0]
+
+        has_bool_or_filter_value = any(isinstance(x, (bool, Filter)) for x in ensure_tuple(item))
+        if has_bool_or_filter_value:
+            # If we have a boolean or Filter value, then that means we need to ast-parse the caller since
+            # python has already evaluated AND, OR, and IN operations into literal booleans or Filters
+            # Skipping the parsing unless if we have need to for efficiency and to eliminate conflicts
+            # with pytest
+            from chalk.df.ast_parser import parse_dataframe_getitem
+
+            item = parse_dataframe_getitem()
+        if any(isinstance(x, (FeatureWrapper, Feature, Filter)) for x in ensure_tuple(item)):
+            return DataFrame(
+                filter_data_frame(item, namespace=self.namespace, underlying=self._underlying),
+                pydantic_model=self._pydantic_model,
+                verify_validity=False,
+            )
+        else:
+            # Otherwise, use the standard polars selection format
+            # Must materialize the dataframe to use __getitem__
+            materialized = self._materialize()
+            df = materialized[item]
+            return DataFrame(df, pydantic_model=self._pydantic_model, verify_validity=False)
+
+    def group_by(
+        self,
+        group: Mapping[Union[Feature, Any], Union[Feature, Any]],
+        agg: Mapping[Any, Any],
+    ) -> DataFrame:
+        """Aggregate the `DataFrame` by the specified columns.
+
+        Parameters
+        ----------
+        group
+            A mapping from the desired column name in the resulting `DataFrame`
+            to the name of the column in the source `DataFrame`.
+        agg
+            A mapping from the desired column name in the resulting `DataFrame`
+            to the aggregation operation to perform on the source `DataFrame`.
+
+        Returns
+        -------
+        DataFrame
+            The `DataFrame` with the specified aggregations applied.
+
+        Examples
+        --------
+        >>> from chalk.features import DataFrame
+        >>> df = DataFrame(
+        ...     {
+        ...         User.id: [1, 1, 3],
+        ...         User.val: [1, 5, 10],
+        ...     }
+        ... ).group_by(
+        ...      group={User.id: User.id}
+        ...      agg={User.val: op.median(User.val)}
+        ... )
+        ╭─────────┬──────────╮
+        │ User.id │ User.val │
+        ╞═════════╪══════════╡
+        │  1      │ 3        │
+        ├─────────┼──────────┤
+        │  3      │ 10       │
+        ╰─────────┴──────────╯
+        """
+        import polars as pl
+
+        from chalk.features.feature_set import FeatureSetBase
+
+        group = [pl.col(str(v)).alias(str(k)) for k, v in group.items()]
+        materialized = self._materialize()
+
+        namespaces = {unwrap_feature(a).namespace for a in agg.keys()}
+        namespace = namespaces.pop() if len(namespaces) == 1 else None
+        timestamp_feature = None if namespace is None else FeatureSetBase.registry[namespace].__chalk_ts__
+
+        now = datetime.now(tz=timezone.utc)
+        cols = []
+        operation: Aggregation
+        for alias, operation in agg.items():
+            # if isinstance(operation, int):
+            #     operation = op.count(FeatureWrapper.len_registry[operation])
+            # c = pl.col(str(operation.col))
+            c = operation.col
+            if len(operation.filters) > 0:
+                c = c.filter(
+                    convert_filters_to_pl_expr(
+                        operation.filters,
+                        self._underlying.schema,
+                        timestamp_feature,
+                        now,
+                    )
+                )
+
+            cols.append(operation.fn(c).alias(str(alias)))
+
+        agged = materialized.lazy().groupby(group).agg(cols).collect()
+
+        return DataFrame(
+            agged,
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def join(
+        self,
+        df: DataFrame,
+        on: Any | List[Any],
+        how: Literal["inner", "left", "outer"] = "left",
+    ) -> DataFrame:
+        on = ensure_tuple(on)
+        p = self._underlying.join(
+            df._underlying,
+            on=[str(t) for t in on],
+            how=how,
+        )
+        return DataFrame(p)
+
+    def vstack(self, other: DataFrame) -> DataFrame:
+        """Vertically stack the `DataFrame` with another `DataFrame`
+        containing the same columns. The `DataFrame` other will
+        be appended to the bottom of this `DataFrame`.
+
+        Parameters
+        ----------
+        other
+            The other `DataFrame` to stack with this `DataFrame`.
+
+        Returns
+        -------
+        DataFrame
+            The `DataFrame` with the other `DataFrame` stacked on the bottom.
+
+        Examples
+        --------
+        >>> from chalk.features import DataFrame
+        >>> df = DataFrame([
+        ...     User(id=1, first="Sam", last="Wu"),
+        ...     User(id=2, first="Iris", last="Xi")
+        ... ])
+        >>> df.vstack(df)
+        """
+        return DataFrame(
+            self._underlying.collect().vstack(other._underlying.collect()).lazy(),
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def rename(self, mapping: Mapping[Any, Any]) -> DataFrame:
+        """Rename columns in the `DataFrame`.
+
+        Parameters
+        ----------
+        mapping
+            A mapping from the current feature for a column to the desired
+            feature for the column.
+
+        Returns
+        -------
+        DataFrame
+            The `DataFrame` with the specified columns renamed.
+
+        Examples
+        --------
+        >>> df = DataFrame([
+        ...     User(id=1, first="Sam", last="Wu"),
+        ...     User(id=2, first="Iris", last="Xi")
+        ... ]).rename({User.last: User.family})
+        """
+        return DataFrame(
+            self._underlying.rename({unwrap_feature(k).fqn: unwrap_feature(v).fqn for k, v in mapping.items()}),
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def with_columns(self, c: Mapping[Any, Any]) -> DataFrame:
+        """Add columns to the `DataFrame`.
+
+        Parameters
+        ----------
+        c
+            A `Mapping` from the desired name of the column
+            in the `DataFrame` to the definition of the new
+            column.
+
+        Examples
+        --------
+        >>> df = DataFrame([
+        ...     User(id=1, first="Sam", last="Wu"),
+        ...     User(id=2, first="Iris", last="Xi")
+        ... ])
+        >>> # Set the fraud score to 0 for all users
+        >>> df.with_columns({User.fraud_score: 0})
+        >>> # Create a full name as the concatenation of first & last
+        >>> df.with_columns({
+        ...     User.full_name: op.concat(User.first, User.last)
+        ... })
+        >>> # Alias a column name
+        >>> df.with_columns({
+        ...     User.first_name: User.first
+        ... })
+
+
+        Returns
+        -------
+        DataFrame
+            A new `DataFrame` with all the existing columns,
+            plus those specified in this function.
+        """
+        import polars as pl
+
+        from chalk.features.feature_set import FeatureSetBase
+
+        namespaces = {unwrap_feature(a).namespace for a in c.keys()}
+        namespace = namespaces.pop() if len(namespaces) == 1 else None
+        timestamp_feature = None if namespace is None else FeatureSetBase.registry[namespace].__chalk_ts__
+
+        now = datetime.now(tz=timezone.utc)
+        cols = []
+        for alias, operation in c.items():
+            # if isinstance(operation, int):
+            #     operation = op.count(FeatureWrapper.len_registry[operation])
+            # c = pl.col(str(operation.col))
+
+            if isinstance(operation, Aggregation):
+                c = operation.col
+                if len(operation.filters) > 0:
+                    c = c.filter(
+                        convert_filters_to_pl_expr(
+                            operation.filters,
+                            self._underlying.schema,
+                            timestamp_feature,
+                            now,
+                        )
+                    )
+
+                cols.append(operation.fn(c).alias(str(alias)))
+            elif isinstance(operation, FeatureWrapper):
+                cols.append(pl.col(str(operation)).alias(str(alias)))
+            else:
+                cols.append(pl.lit(operation).alias(str(alias)))
+
+        agged = self._materialize().lazy().with_columns(cols).collect()
+
+        return DataFrame(
+            agged,
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
     ##############
     # Classmethods
     ##############
 
     @classmethod
     def from_dict(
         cls: Type[TDataFrame],
         data: Dict[Union[str, Feature, FeatureWrapper, Any], Sequence[Any]],
     ) -> TDataFrame:
+        """Deprecated. Use DataFrame(...) instead."""
         warnings.warn(DeprecationWarning("DataFrame.from_dict(...) is deprecated. Instead, use DataFrame(...)"))
         df = cls(data)
         return df
 
     @overload
     @classmethod
     def from_list(
         cls: Type[TDataFrame],
         data: Sequence[Features],
         /,
     ) -> TDataFrame:
+        """Deprecated. Use DataFrame(...) instead."""
         ...
 
     @overload
     @classmethod
     def from_list(cls: Type[TDataFrame], *data: Features) -> TDataFrame:
+        """Deprecated. Use DataFrame(...) instead."""
         ...
 
     @classmethod
     def from_list(cls: Type[TDataFrame], *data: Union[Features, Sequence[Features]]) -> TDataFrame:
+        """Deprecated. Use DataFrame(...) instead."""
         warnings.warn(DeprecationWarning("DataFrame.from_list(...) is deprecated. Instead, use DataFrame(...)"))
         if len(data) == 1 and isinstance(data[0], collections.abc.Sequence):
             # Passed a list as the first argument
             features_seq = data[0]
         else:
             data = cast("Tuple[Features]", data)
             features_seq = data
@@ -807,15 +954,15 @@
         return cls(data)
 
     @classmethod
     def read_avro(
         cls: Type[TDataFrame],
         path: Union[str, pathlib.Path],
     ) -> TDataFrame:
-        """Read a .avro file as a `DataFrame`.
+        """Read a `.avro` file as a `DataFrame`.
 
         Parameters
         ----------
         path
             The path to the `.avro` file. This may be a S3 or GCS
             storage url.
 
@@ -831,15 +978,14 @@
         ... )
         """
         try:
             import polars as pl
         except ImportError:
             raise missing_dependency_exception("chalkpy[runtime]")
 
-        data = None
         if isinstance(path, str) and path.startswith("s3://"):
             try:
                 import fsspec
             except ImportError:
                 raise missing_dependency_exception("fsspec")
             try:
                 import s3fs
@@ -911,14 +1057,38 @@
         ╞═════════╪══════════╡
         │ 2       │ 5        │
         ╰─────────┴──────────╯
         """
         return DataFrame(self._underlying.mean(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def median(self):
+        """Compute the median value of each of the columns in the `DataFrame`.
+        The resulting `DataFrame` will have a single row with the median value
+        of each column.
+
+        Returns
+        -------
+        DataFrame
+            A `DataFrame` with the median value of each column.
+
+        Examples
+        --------
+        >>> from chalk.features import DataFrame
+        >>> df = DataFrame(
+        ...     {
+        ...         User.id: [1, 2, 3],
+        ...         User.val: [1, 4, 10],
+        ...     }
+        ... ).median()
+        ╭─────────┬──────────╮
+        │ User.id │ User.val │
+        ╞═════════╪══════════╡
+        │ 2       │ 4        │
+        ╰─────────┴──────────╯
+        """
         return DataFrame(self._underlying.median(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def min(self):
         return DataFrame(self._underlying.min(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def std(self, ddof: int = 1):
         return DataFrame(self._underlying.std(ddof), convert_dtypes=False, pydantic_model=self._pydantic_model)
@@ -983,46 +1153,42 @@
             The number of rows in the `DataFrame`.
 
         Examples
         --------
         >>> from chalk.features import DataFrame
         >>> df = DataFrame(
         ...     {
-
         ...         User.id: [1, 2, 3],
         ...         User.val: [1, 4, 10],
         ...     }
         ... )
         >>> len(df)
         3
         >>> df.count()
         3
         """
         return len(self)
 
     @property
     def shape(self) -> tuple[int, int]:
-        """Get the shape of the `DataFrame`.
-
-        Returns
-        -------
-        tuple[int, int]
-            The shape of the `DataFrame` as a tuple of (num_rows, num_columns).
+        """The shape of the `DataFrame` as a `tuple` of `(num_rows, num_columns)`.
 
         Examples
         --------
-        >>> df = DataFrame({User.id: [1, 2, 3, 4, 5]})
-        >>> df.shape
+        >>> DataFrame({User.id: [1, 2, 3, 4, 5]}).shape
         (5, 1)
         """
         materialized = self._materialize()
         return materialized.shape
 
     def item(self):
-        """Get the only item from the `DataFrame`."""
+        """Get the only item from the `DataFrame`.
+        This method will raise an error if the `DataFrame` contains
+        more than one row or more than column.
+        """
         materialized = self._materialize()
         if materialized.shape == (1, 1):
             return materialized.rows()[0][0]
         raise ValueError(
             "The dataframe contains multiple items. DataFrame.item() can only be used if the dataframe has a single element."
         )
 
@@ -1122,14 +1288,15 @@
                 return self._perform_comp_df(op, other, convert_dtypes=convert_dtypes)
             else:
                 return DataFrame(
                     getattr(operator, op)(materialized, other),
                     convert_dtypes=convert_dtypes,
                     pydantic_model=self._pydantic_model,
                 )
+
         assert callable(op)
         return DataFrame(
             op(materialized, other),
             convert_dtypes=convert_dtypes,
             pydantic_model=self._pydantic_model,
         )
 
@@ -1253,15 +1420,15 @@
         -------
         polars.LazyFrame
             The underlying `polars.LazyFrame`.
         """
         return self._underlying
 
     def to_pyarrow(self) -> pa.Table:
-        """Get the underlying dataframe as a `pyarrow.Table`.
+        """Get the underlying `DataFrame` as a `pyarrow.Table`.
 
         Returns
         -------
         pyarrow.Table
             The underlying `pyarrow.Table`. This format is the canonical
             representation of the data in Chalk.
         """
@@ -1292,15 +1459,15 @@
         # For pandas, the columns should be the Features, not the root fqns
         # So, convert the columns to object types, and then set them to the features
         pd_dataframe.columns = pd_dataframe.columns.astype("object")
         pd_dataframe = pd_dataframe.rename(columns={x.root_fqn: x for x in self.columns})
         return pd_dataframe
 
     def to_features(self) -> Sequence[Features]:
-        """Get values in the dataframe as `Features` instances.
+        """Get values in the `DataFrame` as `Features` instances.
 
         Examples
         --------
         >>> df = DataFrame({
         ...     SpaceShip.id: [1, 2],
         ...     SpaceShip.volume: [4_000, 5_000]
         ... })
@@ -1346,65 +1513,14 @@
                     features_cls = Feature.from_root_fqn(rooted_prefix).joined_class
                     assert features_cls is not None
                     parent_rooted_prefix, feature_name = ".".join(rooted_prefix_split[:-1]), rooted_prefix_split[-1]
                     del feature_name  # unused
                     rooted_prefix_to_values[parent_rooted_prefix][rooted_prefix] = features_cls(**sub_kwargs)
         return ans
 
-    #######################
-    # Filtering / Selecting
-    #######################
-    def __getitem__(self, item: Any) -> DataFrame:
-        """Filter by rows or by columns.
-
-        Parameters
-        ----------
-        item
-
-        Returns
-        -------
-
-        """
-        if isinstance(item, int) and not isinstance(item, bool):
-            if item >= 0:
-                l = len(self)
-                if item >= l:
-                    raise IndexError(f"Index {item} out of range (length {l})")
-                underlying = self._underlying.head(item + 1).tail(1)
-            else:
-                underlying = self._underlying.tail(-item).head(1)
-
-            df = DataFrame(
-                underlying,
-                convert_dtypes=False,
-                pydantic_model=self._pydantic_model,
-            )
-            return list(df.to_features())[0]
-
-        has_bool_or_filter_value = any(isinstance(x, (bool, Filter)) for x in ensure_tuple(item))
-        if has_bool_or_filter_value:
-            # If we have a boolean or Filter value, then that means we need to ast-parse the caller since
-            # python has already evaluated AND, OR, and IN operations into literal booleans or Filters
-            # Skipping the parsing unless if we have need to for efficiency and to eliminate conflicts
-            # with pytest
-            from chalk.df.ast_parser import parse_dataframe_getitem
-
-            item = parse_dataframe_getitem()
-        if any(isinstance(x, (FeatureWrapper, Feature, Filter)) for x in ensure_tuple(item)):
-            return DataFrame(
-                filter_data_frame(item, namespace=self.namespace, underlying=self._underlying),
-                pydantic_model=self._pydantic_model,
-            )
-        else:
-            # Otherwise, use the standard polars selection format
-            # Must materialize the dataframe to use __getitem__
-            materialized = self._materialize()
-            df = materialized[item]
-            return DataFrame(df, pydantic_model=self._pydantic_model)
-
     def slice(self, offset: int = 0, length: Optional[int] = None) -> DataFrame:
         """Slice the `DataFrame`.
 
         Parameters
         ----------
         offset
             The offset to start at.
```

### Comparing `chalkpy-2.5.9/chalk/features/dataframe/_validation.py` & `chalkpy-2.6.0/chalk/features/dataframe/_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 from typing import TYPE_CHECKING, Union, cast
 
 import dateutil.parser
 import isodate
 
 from chalk.features._encoding.missing_value import MissingValueStrategy
-from chalk.features.feature_field import Feature
+from chalk.features.feature_field import Feature, FeatureNotFoundException
 
 if TYPE_CHECKING:
     import polars as pl
 
 try:
     import zoneinfo
 except ImportError:
@@ -152,29 +152,35 @@
 
     return underlying
 
 
 def validate_nulls(
     underlying: Union[pl.DataFrame, pl.LazyFrame],
     missing_value_strategy: MissingValueStrategy,
+    tolerate_missing_features: bool = False,
 ) -> pl.DataFrame:
     """Validate that any null values are in columns that support nullable values"""
     # This is called from within DataFrame.__init__, which validates that polars is installed
     import polars as pl
 
     if isinstance(underlying, pl.LazyFrame):
         underlying = underlying.collect()
     schema = underlying.schema
     null_count_rows = underlying.null_count().to_dicts()
     if len(null_count_rows) == 0:
         return underlying  # Empty dataframe
     assert len(null_count_rows) == 1
     null_counts = null_count_rows[0]
     for col_name, null_count in null_counts.items():
-        feature = Feature.from_root_fqn(col_name)
+        try:
+            feature = Feature.from_root_fqn(col_name)
+        except FeatureNotFoundException:
+            if tolerate_missing_features:
+                continue
+            raise
         if null_count > 0 and not feature.typ.is_nullable and not isinstance(schema[col_name], pl.Struct):
             if missing_value_strategy == "allow":
                 warnings.warn(
                     UserWarning(
                         f"Allowing missing value for feature '{col_name}' with type '{feature.typ}' strategy "
                         f"'default_or_allow'"
                     )
```

### Comparing `chalkpy-2.5.9/chalk/features/feature_field.py` & `chalkpy-2.6.0/chalk/features/feature_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,25 +32,27 @@
 from chalk.features._encoding.converter import FeatureConverter, TDecoder, TEncoder
 from chalk.features._encoding.primitive import TPrimitive
 from chalk.features.tag import Tags
 from chalk.serialization.parsed_annotation import ParsedAnnotation
 from chalk.streams import Windowed
 from chalk.utils.collections import ensure_tuple
 from chalk.utils.duration import Duration, parse_chalk_duration
+from chalk.utils.log_with_context import get_logger
 from chalk.utils.string import to_snake_case
 
 if TYPE_CHECKING:
     from chalk.features.feature_set import Features
     from chalk.features.filter import Filter
 
 _TRich = TypeVar("_TRich")
 _TPrim = TypeVar("_TPrim", bound=TPrimitive)
 
 __all__ = ["Feature", "feature", "has_one", "has_many"]
 
+_logger = get_logger(__name__)
 
 @dataclasses.dataclass
 class HasOnePathObj:
     parent: Feature
     child: Feature
     parent_to_child_attribute_name: str
 
@@ -338,17 +340,20 @@
         from chalk.features.feature_set import FeatureSetBase
         from chalk.features.pseudofeatures import PSEUDOFEATURES
 
         for x in PSEUDOFEATURES:
             if root_fqn == x.root_fqn or root_fqn == x.name:
                 return x
 
-        root_fqn = to_snake_case(root_fqn)
         split_fqn = root_fqn.split(".")
         root_ns = split_fqn[0]
+        root_ns_snake_case = to_snake_case(root_ns)
+        if root_ns_snake_case != root_ns:
+            _logger.warning(f"Namespace of {root_fqn=} is not in snake_case, which is unexpected. Converting to snake case and continuing.")
+        root_ns = root_ns_snake_case
         split_fqn = split_fqn[1:]
 
         if root_ns not in FeatureSetBase.registry:
             raise FeatureNotFoundException(root_fqn)
         features_cls = FeatureSetBase.registry[root_ns]
 
         # FQNs are by name, so must lookup the feature in features_cls.features instead of using getattr
```

### Comparing `chalkpy-2.5.9/chalk/features/feature_set.py` & `chalkpy-2.6.0/chalk/features/feature_set.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/feature_set_decorator.py` & `chalkpy-2.6.0/chalk/features/feature_set_decorator.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/feature_time.py` & `chalkpy-2.6.0/chalk/features/feature_time.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/feature_wrapper.py` & `chalkpy-2.6.0/chalk/features/feature_wrapper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/filter.py` & `chalkpy-2.6.0/chalk/features/filter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/hooks.py` & `chalkpy-2.6.0/chalk/features/hooks.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/live_updates.py` & `chalkpy-2.6.0/chalk/features/live_updates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Any, Dict, List, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import cloudpickle
 
 from chalk.utils import notebook
 from chalk.utils.log_with_context import get_logger
 
 _logger = get_logger(__name__)
@@ -52,15 +52,14 @@
             f"Failed to upload features/resolvers to branch server on branch '{client.get_branch()}'.", exc_info=True
         )
         raise
     return resp
 
 
 def _print_responses(responses: List["UpdateGraphEntityResponse"]):
-    print(f"Uploaded {len(responses)} resolvers/features to branch server.")
     from chalk.client.models import SingleEntityUpdate
 
     all_errors = [e for r in responses for e in (r.errors or [])]
     if all_errors:
         for e in all_errors:
             _logger.error(e.message)
         return
@@ -145,32 +144,51 @@
     _UPDATED_RESOLVERS_CACHE.clear()
     _UPDATED_FEATURES_CACHE.clear()
 
 
 def _deploy_objects(entities: List[Union["Features", "Resolver"]]):
     try:
         # Validation
+        from chalk.features.feature_set import FeatureSetBase, is_features_cls
+        from chalk.features.resolver import Resolver
         from chalk.parsed.duplicate_input_gql import GraphLogSeverity
 
         if len(errors := _validate_current_graph()) > 0:
             for err in errors:
                 _logger.error(f"{err.severity}: {err.header}")
                 _logger.error(f"{err.severity}: --- {err.subheader}")
             if any(err.severity == GraphLogSeverity.ERROR for err in errors):
                 raise ValueError(f"Failed to validate updated graph ({len(errors)} errors).")
         # Upload
         resps = []
+        num_resolvers = len([e for e in entities if isinstance(e, Resolver)])
+        num_feature_classes = len([e for e in entities if is_features_cls(e)])
+        log_messages = filter(
+            None,
+            [
+                _pluralize(num_feature_classes, "feature class", "feature classes"),
+                _pluralize(num_resolvers, "resolver", "resolvers"),
+            ],
+        )
+        log_message_combined = " and ".join(log_messages)
+        print(f"Uploading {log_message_combined} to branch server...")
         for e in entities:
             resps.append(_upload_object(e))
         _print_responses(resps)
     except Exception:
         for obj in entities:
             _remove_object_from_registries(obj)
 
 
+def _pluralize(count: int, singular_word: str, plural_word: str) -> Optional[str]:
+    if count == 0:
+        return None
+    return f"{count} {singular_word if count == 1 else plural_word}"
+
+
 def _deploy_objects_from_cache(result: "IPython.ExecutionResult"):
     """
     Runs after a Jupyter cell has finished execution.
     Validates and deploys any new entities defined in the cell to the branch server.
     TODO (rkargon): Currently this uploads objects one at a time.
     This works and should still avoid the forward reference/validation issues in the client.
     :param result: IPython result object.
```

### Comparing `chalkpy-2.5.9/chalk/features/primary.py` & `chalkpy-2.6.0/chalk/features/primary.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/pseudofeatures.py` & `chalkpy-2.6.0/chalk/features/pseudofeatures.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/resolver.py` & `chalkpy-2.6.0/chalk/features/resolver.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/features/tag.py` & `chalkpy-2.6.0/chalk/features/tag.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/gitignore/gitignore_parser.py` & `chalkpy-2.6.0/chalk/gitignore/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/gitignore/helper.py` & `chalkpy-2.6.0/chalk/gitignore/helper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/importer.py` & `chalkpy-2.6.0/chalk/importer.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/integrations/named.py` & `chalkpy-2.6.0/chalk/integrations/named.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/logging/__init__.py` & `chalkpy-2.6.0/chalk/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/mypy_plugin.py` & `chalkpy-2.6.0/chalk/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/parsed/_graph_validation.py` & `chalkpy-2.6.0/chalk/parsed/_graph_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/parsed/duplicate_input_gql.py` & `chalkpy-2.6.0/chalk/parsed/duplicate_input_gql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/parsed/json_conversions.py` & `chalkpy-2.6.0/chalk/parsed/json_conversions.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/parsed/user_types_to_json.py` & `chalkpy-2.6.0/chalk/parsed/user_types_to_json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/serialization/parsed_annotation.py` & `chalkpy-2.6.0/chalk/serialization/parsed_annotation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/__init__.py` & `chalkpy-2.6.0/chalk/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/chalk_query.py` & `chalkpy-2.6.0/chalk/sql/_internal/chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/incremental.py` & `chalkpy-2.6.0/chalk/sql/_internal/incremental.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/bigquery.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/bigquery.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/cloudsql.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/cloudsql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/databricks.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/databricks.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/mysql.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/mysql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/postgres.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/postgres.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/redshift.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/redshift.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/snowflake.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/snowflake.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/integrations/sqlite.py` & `chalkpy-2.6.0/chalk/sql/_internal/integrations/sqlite.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/sql_file_resolver.py` & `chalkpy-2.6.0/chalk/sql/_internal/sql_file_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 }
 
 
 class IncrementalSettings(BaseModel):
     incremental_column: Optional[str]
     lookback_period: Optional[str]
     mode: Literal["row", "group", "parameter"]
-    incremental_timestamp: Literal["feature_time", "resolver_execution_time"]
+    incremental_timestamp: Literal["feature_time", "resolver_execution_time"] = "feature_time"
 
     @validator("lookback_period")
     @classmethod
     def validate_lookback_period(cls, value: Optional[str]):
         if value is None:
             return None
         try:
```

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/sql_source.py` & `chalkpy-2.6.0/chalk/sql/_internal/sql_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/_internal/string_chalk_query.py` & `chalkpy-2.6.0/chalk/sql/_internal/string_chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/finalized_query.py` & `chalkpy-2.6.0/chalk/sql/finalized_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/sql/protocols.py` & `chalkpy-2.6.0/chalk/sql/protocols.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/state.py` & `chalkpy-2.6.0/chalk/state.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/streams/__init__.py` & `chalkpy-2.6.0/chalk/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/streams/_kafka_source.py` & `chalkpy-2.6.0/chalk/streams/_kafka_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/streams/_kinesis_source.py` & `chalkpy-2.6.0/chalk/streams/_kinesis_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/streams/_windows.py` & `chalkpy-2.6.0/chalk/streams/_windows.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/streams/types.py` & `chalkpy-2.6.0/chalk/streams/types.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/testing/__init__.py` & `chalkpy-2.6.0/chalk/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/annotation_parsing.py` & `chalkpy-2.6.0/chalk/utils/annotation_parsing.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/collections.py` & `chalkpy-2.6.0/chalk/utils/collections.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/duration.py` & `chalkpy-2.6.0/chalk/utils/duration.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/enum.py` & `chalkpy-2.6.0/chalk/utils/enum.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/environment_parsing.py` & `chalkpy-2.6.0/chalk/utils/environment_parsing.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/log_with_context.py` & `chalkpy-2.6.0/chalk/utils/log_with_context.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/metaprogramming.py` & `chalkpy-2.6.0/chalk/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/notebook.py` & `chalkpy-2.6.0/chalk/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/paths.py` & `chalkpy-2.6.0/chalk/utils/paths.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/string.py` & `chalkpy-2.6.0/chalk/utils/string.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalk/utils/stubgen.py` & `chalkpy-2.6.0/chalk/utils/stubgen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/chalkpy.egg-info/SOURCES.txt` & `chalkpy-2.6.0/chalkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chalkpy-2.5.9/pyproject.toml` & `chalkpy-2.6.0/pyproject.toml`

 * *Files identical despite different names*

