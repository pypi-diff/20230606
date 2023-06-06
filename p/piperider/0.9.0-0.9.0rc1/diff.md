# Comparing `tmp/piperider-0.9.0.tar.gz` & `tmp/piperider-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piperider-0.9.0.tar", last modified: Thu Sep 22 01:39:09 2022, max compression
+gzip compressed data, was "piperider-0.9.0rc1.tar", last modified: Tue Sep 20 06:48:15 2022, max compression
```

## Comparing `piperider-0.9.0.tar` & `piperider-0.9.0rc1.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.692425 piperider-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-22 01:38:25.000000 piperider-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9040 2022-09-22 01:39:09.692425 piperider-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8210 2022-09-22 01:38:25.000000 piperider-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.656425 piperider-0.9.0/piperider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9040 2022-09-22 01:39:09.000000 piperider-0.9.0/piperider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16550 2022-09-22 01:39:09.000000 piperider-0.9.0/piperider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 01:39:09.000000 piperider-0.9.0/piperider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-22 01:39:09.000000 piperider-0.9.0/piperider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-22 01:39:09.000000 piperider-0.9.0/piperider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-22 01:39:09.000000 piperider-0.9.0/piperider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/SENTRY_DNS
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-22 01:38:56.000000 piperider-0.9.0/piperider_cli/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/adapter/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11325 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/adapter/dbt_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/assertion_engine/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24636 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/assertion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/assertion_engine/recommended_rules/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/recommended_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/recommended_rules/recommender_assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)     4458 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/recommended_rules/table_assertions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4531 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/recommender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/assertion_engine/types/
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/types/assert_column_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/types/assert_column_ranges.py
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/types/assert_column_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/types/assert_rows.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_engine/types/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3315 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/assertion_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3486 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/cloud_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/compare_report.py
--rw-r--r--   0 runner    (1001) docker     (121)    12644 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-22 01:38:56.000000 piperider-0.9.0/piperider_cli/data/CONFIG
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-22 01:38:53.000000 piperider-0.9.0/piperider_cli/data/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/piperider-init-template/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/piperider-init-template/assertions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/piperider-init-template/assertions/placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/piperider-init-template/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/piperider-init-template/gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/piperider-init-template/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/piperider-init-template/plugins/customized_assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.656425 piperider-0.9.0/piperider_cli/data/report/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/report/comparison-report/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/report/comparison-report/Discord/
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/Discord/Discord-Logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.660425 piperider-0.9.0/piperider_cli/data/report/comparison-report/GitHub/
--rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/GitHub/GitHub-Logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.664425 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (121)     5783 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)    12342 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-70x70.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.656425 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.664425 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css
--rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.668425 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    20055 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/183.b8accd6c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    14053 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/276.fcb4db01.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    11803 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/357.5328e62e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/787.20f148af.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/836.945208d8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)   104944 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/903.4ec9ff75.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/903.4ec9ff75.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/906.9eefb2c7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/914.035c9fb2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    27742 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/982.4539617f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)  1199840 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.676425 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    32632 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff
--rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Black.cadfd7434852779eb395.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    25732 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    34940 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33900 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.1577ca92013647c816b5.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25152 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36168 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff
--rw-r--r--   0 runner    (1001) docker     (121)    26684 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    33960 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25220 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26736 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36220 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff
--rw-r--r--   0 runner    (1001) docker     (121)    24852 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26648 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    35756 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    34924 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff
--rw-r--r--   0 runner    (1001) docker     (121)    24764 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26696 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    35788 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33884 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25132 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26824 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36236 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff
--rw-r--r--   0 runner    (1001) docker     (121)    23980 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.222064f2a764069868f4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    32236 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.67a27362108220436ffb.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25240 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    33944 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff
--rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36280 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff
--rw-r--r--   0 runner    (1001) docker     (121)    23636 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    32084 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff
--rw-r--r--   0 runner    (1001) docker     (121)    34704 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25664 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    58892 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    53832 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    78400 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.676425 piperider-0.9.0/piperider_cli/data/report/single-report/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.676425 piperider-0.9.0/piperider_cli/data/report/single-report/Discord/
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/Discord/Discord-Logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.676425 piperider-0.9.0/piperider_cli/data/report/single-report/GitHub/
--rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/GitHub/GitHub-Logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.680425 piperider-0.9.0/piperider_cli/data/report/single-report/logo/
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (121)     5783 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)    12342 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-70x70.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.656425 piperider-0.9.0/piperider_cli/data/report/single-report/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.680425 piperider-0.9.0/piperider_cli/data/report/single-report/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css
--rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.680425 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    20055 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/183.b8accd6c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    14053 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/276.fcb4db01.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    11803 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/357.5328e62e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/787.20f148af.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/836.945208d8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)   104944 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/903.4ec9ff75.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/903.4ec9ff75.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/906.9eefb2c7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/914.035c9fb2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    27742 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/982.4539617f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)  1191712 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/main.a918e51a.js
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/js/main.a918e51a.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.688425 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    32632 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff
--rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Black.cadfd7434852779eb395.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    25732 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    34940 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33900 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Bold.1577ca92013647c816b5.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25152 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36168 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff
--rw-r--r--   0 runner    (1001) docker     (121)    26684 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    33960 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25220 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26736 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36220 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff
--rw-r--r--   0 runner    (1001) docker     (121)    24852 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26648 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    35756 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    34924 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff
--rw-r--r--   0 runner    (1001) docker     (121)    24764 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26696 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    35788 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33884 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25132 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26824 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36236 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff
--rw-r--r--   0 runner    (1001) docker     (121)    23980 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Regular.222064f2a764069868f4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    32236 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Regular.67a27362108220436ffb.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25240 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    33944 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff
--rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    36280 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff
--rw-r--r--   0 runner    (1001) docker     (121)    23636 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    32084 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff
--rw-r--r--   0 runner    (1001) docker     (121)    34704 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25664 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    58892 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    53832 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    78400 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.688425 piperider-0.9.0/piperider_cli/datasource/
--rw-r--r--   0 runner    (1001) docker     (121)     7654 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9549 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (121)     7658 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     6898 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     6824 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/datasource/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.688425 piperider-0.9.0/piperider_cli/docgen/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/docgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/docgen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6966 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.692425 piperider-0.9.0/piperider_cli/event/
--rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4762 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/event/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/event/track.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/feedback.py
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     4735 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/generate_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/guide.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.692425 piperider-0.9.0/piperider_cli/hack/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/hack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/hack/datasource_inquirer_prompt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/hack/inquirer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 01:39:09.692425 piperider-0.9.0/piperider_cli/profiler/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/profiler/event.py
--rw-r--r--   0 runner    (1001) docker     (121)    46473 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)    14500 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/profiler/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/profiler/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    25292 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     7341 2022-09-22 01:38:25.000000 piperider-0.9.0/piperider_cli/validator.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 01:39:09.692425 piperider-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-09-22 01:38:25.000000 piperider-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7579 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6746 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.110840 piperider-0.9.0rc1/piperider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7579 2022-09-20 06:48:15.000000 piperider-0.9.0rc1/piperider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16550 2022-09-20 06:48:15.000000 piperider-0.9.0rc1/piperider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 06:48:15.000000 piperider-0.9.0rc1/piperider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-20 06:48:15.000000 piperider-0.9.0rc1/piperider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-20 06:48:15.000000 piperider-0.9.0rc1/piperider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-20 06:48:15.000000 piperider-0.9.0rc1/piperider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/SENTRY_DNS
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-20 06:48:02.000000 piperider-0.9.0rc1/piperider_cli/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/adapter/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11325 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/adapter/dbt_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/assertion_engine/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24636 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/assertion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/assertion_engine/recommended_rules/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/recommended_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/recommended_rules/recommender_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4458 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/recommended_rules/table_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4531 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/recommender.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_column_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_column_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_engine/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3315 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/assertion_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3486 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/cloud_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/compare_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12644 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-20 06:48:02.000000 piperider-0.9.0rc1/piperider_cli/data/CONFIG
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-20 06:47:59.000000 piperider-0.9.0rc1/piperider_cli/data/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/assertions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/assertions/placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/plugins/customized_assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.110840 piperider-0.9.0rc1/piperider_cli/data/report/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/Discord/
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/Discord/Discord-Logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.114840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/GitHub/
+-rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/GitHub/GitHub-Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.118840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5783 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12342 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-70x70.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.110840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.118840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css
+-rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css.map
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.122840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)    20055 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/183.b8accd6c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)    14053 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/276.fcb4db01.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)    11803 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/357.5328e62e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/787.20f148af.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/836.945208d8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)   104944 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/903.4ec9ff75.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/903.4ec9ff75.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/906.9eefb2c7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/914.035c9fb2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)    27742 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/982.4539617f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)  1199840 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.126840 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/
+-rw-r--r--   0 runner    (1001) docker     (121)    32632 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Black.cadfd7434852779eb395.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    25732 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    34940 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33900 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.1577ca92013647c816b5.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25152 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36168 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    26684 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    33960 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25220 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26736 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36220 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    24852 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26648 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    35756 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    34924 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    24764 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26696 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    35788 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33884 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25132 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26824 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36236 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    23980 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.222064f2a764069868f4.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    32236 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.67a27362108220436ffb.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25240 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    33944 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36280 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    23636 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    32084 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    34704 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25664 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    58892 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    53832 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    78400 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.126840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.126840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/Discord/
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/Discord/Discord-Logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.126840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/GitHub/
+-rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/GitHub/GitHub-Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.130840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5783 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12342 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-70x70.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.110840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.130840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css
+-rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css.map
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.134840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)    20055 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/183.b8accd6c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)    14053 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/276.fcb4db01.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)    11803 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/357.5328e62e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/787.20f148af.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/836.945208d8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)   104944 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/903.4ec9ff75.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/903.4ec9ff75.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/906.9eefb2c7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/914.035c9fb2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)    27742 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/982.4539617f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (121)  1191712 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/main.a918e51a.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/main.a918e51a.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.138840 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/
+-rw-r--r--   0 runner    (1001) docker     (121)    32632 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Black.cadfd7434852779eb395.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    25732 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    34940 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33900 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Bold.1577ca92013647c816b5.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25152 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36168 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    26684 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    33960 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25220 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26736 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36220 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    24852 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26648 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    35756 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    34924 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33248 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    24764 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26696 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    35788 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    33884 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25132 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    26824 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36236 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    23980 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Regular.222064f2a764069868f4.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    32236 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Regular.67a27362108220436ffb.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25240 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    33944 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    36280 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    23636 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    32084 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    34704 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    25664 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    58892 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    53832 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    78400 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/piperider_cli/datasource/
+-rw-r--r--   0 runner    (1001) docker     (121)     7654 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9549 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7658 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6898 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6824 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/datasource/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/piperider_cli/docgen/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/docgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/docgen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6966 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/piperider_cli/event/
+-rw-r--r--   0 runner    (1001) docker     (121)     3578 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4762 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/event/collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/event/track.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4735 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/generate_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/guide.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/piperider_cli/hack/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/hack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/hack/datasource_inquirer_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/hack/inquirer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/piperider_cli/profiler/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/profiler/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46473 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14500 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/profiler/schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/profiler/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25292 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7341 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/piperider_cli/validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 06:48:15.142840 piperider-0.9.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-09-20 06:47:25.000000 piperider-0.9.0rc1/setup.py
```

### Comparing `piperider-0.9.0/LICENSE` & `piperider-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/PKG-INFO` & `piperider-0.9.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piperider
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: PiperRider CLI
 Home-page: https://github.com/InfuseAI/piperider
 Author: InfuseAI Dev Team
 Author-email: dev@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/piperider/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,15 @@
 Provides-Extra: redshift
 Provides-Extra: duckdb
 Provides-Extra: csv
 Provides-Extra: parquet
 Provides-Extra: dev
 License-File: LICENSE
 
-# PipeRider: Data Reliability Toolkit
+# PipeRider: Data Reliability Automated
 
 [![ci-tests](https://github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)
 [![release](https://img.shields.io/github/release/infuseAI/piperider-cli/all.svg?style=flat-square)](https://github.com/infuseAI/piperider-cli/releases)
 [![pipy](https://img.shields.io/pypi/v/piperider?style=flat-square)](https://pypi.org/project/piperider/)
 [![python](https://img.shields.io/pypi/pyversions/piperider?style=flat-square)](https://pypi.org/project/piperider/)
 [![downloads](https://img.shields.io/pypi/dw/piperider?style=flat-square)](https://pypi.org/project/piperider/#files)
 [![license](https://img.shields.io/github/license/infuseai/piperider?style=flat-square)](https://github.com/InfuseAI/piperider/blob/main/LICENSE)
@@ -38,85 +38,50 @@
   <a href="https://piperider.io">
     <img  src=".github/images/logo.svg" border="0" alt="PipeRider">
   </a>
 </p>
 
 
 # What's PipeRider?
-**[PipeRider](https://www.piperider.io/)** is a light-weight data reliability toolkit using warehouse-native profiling so you can have a full understanding of your data 
+[PipeRider](https://www.piperider.io/) is a light-weight data quality tool so you can be confident of your data without writing tests for every single pipeline. 
 
 **We're in an early stage, so [let us know](mailto:product@infuseai.io) if you have any questions, feedback, or need help installing PipeRider! :heart:**
 
 
-
-## Profiling as a data reliability strategy
-PipeRider will make your life easier by:
-1. Building a data profile so you can easily understand your data
-2. Creating test suggestions based on the profiling
-3. Comparing data profile reports, so you track changes over time
-
-[Read how to implement a data quality strategy using profiling + testing](https://blog.infuseai.io/add-data-profiling-and-assertions-to-dbt-with-piperider-732ca0821e3a)
-
-
-
-## Made for the modern data team
-**For data engineers**
-* :zap: 2 min install & set-up
-* :relieved: Non-intrusive & open-source: install and use locally
-* :money_with_wings: Fast & cheap: 100M rows & 8 columns (or 50M & 16 columns) takes only 18s to profile
-* :ledger: Cloud DataWarehouse native & auto-config for dbt
-
-
-
-**For data analysts**
-* :bowtie: Never waste time on analyzing wrong data: collects various metadata metrics such as freshness, uniqueness, distribution... [check all metrics](https://docs.piperider.io/data-profile-and-metrics/metrics)
-* :speech_balloon: Communicate easily your data expectations by showing the report
-* Zero-config dbt integration
-
-
-## Live Demo
-[![](https://i.imgur.com/WuFC4H6.png)](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-
-[Click here or on image to interact](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-
-<!-- # Table of contents
-* [What's PipeRider?](#what's-piperider?)
-    * [Made for...](#made-for...)
-    * [Live demo](#live-demo)
-* [Table of contents](#table-of-contents)
-* [Getting started](#getting-started)
-    * [Install piperider](#install-piperider)
-    * [Attach PipeRider to a dbt project](#attach-piperider-to-a-dbt-project)
-    * [Scan data quality from models](#scan-data-quality-from-models)
-    * [Generate reports](#generate-reports)
-    * [Generate comparison view](#generate-comparison-view)
-* [Learn more](#learn-more)
-* [Get involved](#get-involved)
-    * [Support](#support)
-    * [Contributions](#contributions)
- -->
-
-
-## Key features
+## Key Features
 * [Generate an HTML Report](https://docs.piperider.io/how-to-guides/generate-report) featuring your data profile and data assertion test results ([interactive sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
 * [Compare two reports](https://docs.piperider.io/how-to-guides/compare-reports) to understand how your data has changed over time ([interactive sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/comparison-0.8.0/index.html))
 * Test your data with data assertions:
   * Built-in [data assertions](https://docs.piperider.io/data-quality-assertions/assertion-configuration)
   * Extensible through [custom assertions](https://docs.piperider.io/data-quality-assertions/custom-assertions)
   * Auto-generated data assertions
 * Currently supports [Postgres](https://docs.piperider.io/data-sources/postgres-connector), [Snowflake](https://docs.piperider.io/data-sources/snowflake-connector), SQLite, [BigQuery](https://docs.piperider.io/data-sources/bigquery-connector), [Redshift](https://docs.piperider.io/data-sources/redshift-connector), [DuckDB](https://docs.piperider.io/data-sources/duckdb-connector/), [CSV](https://docs.piperider.io/data-sources/csv-connector/) and [Parquet](https://docs.piperider.io/data-sources/parquet-connector/).
 * Zero-config [support for dbt](https://docs.piperider.io/dbt-integration/) projects
 * Automation through [GitHub Actions](https://docs.piperider.io/how-to-guides/github-action/), [save reports in S3](https://docs.piperider.io/how-to-guides/aws-s3-+-github-ci/)
 
+## Made for...
+**For data engineers**
+* :zap: 2 min install & set-up
+* :relieved: non-intrusive & open-source: install and use locally
+* :moneybag: fast & cheap: 10M rows, 8 columns takes only 16s to profile
+
 
+**For data analysts**
+* :bowtie: never waste time on analyzing wrong data: collects various metadata metrics such as freshness, uniqueness, distribution... [check all metrics](https://docs.piperider.io/data-profile-and-metrics/metrics)
+* :speech_balloon: communicate easily your data expectations by showing the report
+
+
+## Live Demo
+[![](https://i.imgur.com/WuFC4H6.png)](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html)
 
+[Click here or on image to interact](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html)
 
 # Getting started
 
-Get started quickly below, go to [the docs](https://docs.piperider.io/), or check out this article on [how to add data observability using PipeRider ](https://blog.infuseai.io/adding-data-observability-and-alerts-to-your-data-pipeline-is-easier-than-you-think-4e005daca55b)
+Get started quickly below, or go to [the docs](https://docs.piperider.io/)
 
 ## Install PipeRider
 
 ```bash
 pip install piperider
 ```
 
@@ -137,37 +102,30 @@
 ```bash
 pip install 'piperider[postgres,snowflake]'
 ```
 
 You can follow the [quick start guide](https://docs.piperider.io/quick-start) to learn more about PipeRider.
 
 ## Attach PipeRider to a dbt project
-Initialize PipeRider inside a dbt project and your data source settings will be automatically configured
 
 `piperider init` creates `/.piperider` under a dbt project root and generates necessary configurations.
 
-![piperider_init](images/init_pipe.gif)
-
 ## Scan data quality from models
 
-`piperider run` scans the models from data sources and creates assessment results in `/.piperider/output`
-
-![piperider_run](images/run_pipe.gif)
-
-## Generate reports
+`piperider run` runs profiling, and tests against assertions, and will render an HTML report `/.piperider/outputs`
 
-`piperider generate-report` generate a static HTML report.
+You can do a run for a specific table using `piperider run --table $TABLENAME`
+You can specifying the output location of a report using `piperider generate-report -o $PATHNAME` or specifying it in the config file.
 
-![piperider_report](images/report_pipe.gif)
+[All details on generating reports](https://docs.piperider.io/how-to-guides/generate-report)
 
 ## Generate comparison view
 
 You can use `piperider compare-report` to compare 2 reports.
 
-![piperider_compare](images/compare_pipe.gif)
 
 # Learn More
 
 | PipeRider Resources | Description |
 | -------------------- | ----------- |
 | [Documentation] | PipeRider Main Doc Site |
 | [Sample_Project] | Sample Project with with sqlite |
@@ -184,14 +142,14 @@
 
 [Roadmap]: https://github.com/orgs/InfuseAI/projects/1/views/1
 
 [Blog]: https://blog.infuseai.io/data-reliability-automated-with-piperider-7a823521ef11
 
 # Get involved
 
-## Support 
+## Support :heart:
 If you like what we are building, support us! Give us a :star: or get in touch. We'd love your feedback! Send us a message on [piperider.io](https://piperider.io), join our [Discord](https://discord.com/invite/CrAxQznedH), or report an issue on [GitHub](https://github.com/InfuseAI/piperider/issues)
 
 
 ## Contributions
 
 We welcome contributions. See the [Set up dev environment](DEVELOP.md) and the [Contributing guildline](CONTRIBUTING.md) to get started.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: piperider Version: 0.9.0 Summary: PiperRider CLI
+Metadata-Version: 2.1 Name: piperider Version: 0.9.0rc1 Summary: PiperRider CLI
 Home-page: https://github.com/InfuseAI/piperider Author: InfuseAI Dev Team
 Author-email: dev@infuseai.io Project-URL: Bug Tracker, https://github.com/
 InfuseAI/piperider/issues Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Development Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type:
 text/markdown Provides-Extra: snowflake Provides-Extra: postgres Provides-
 Extra: bigquery Provides-Extra: redshift Provides-Extra: duckdb Provides-Extra:
 csv Provides-Extra: parquet Provides-Extra: dev License-File: LICENSE #
-PipeRider: Data Reliability Toolkit [![ci-tests](https://github.com/infuseai/
+PipeRider: Data Reliability Automated [![ci-tests](https://github.com/infuseai/
 piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://github.com/
 infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg) [![release]
 (https://img.shields.io/github/release/infuseAI/piperider-cli/
 all.svg?style=flat-square)](https://github.com/infuseAI/piperider-cli/releases)
 [![pipy](https://img.shields.io/pypi/v/piperider?style=flat-square)](https://
 pypi.org/project/piperider/) [![python](https://img.shields.io/pypi/pyversions/
 piperider?style=flat-square)](https://pypi.org/project/piperider/) [!
@@ -21,40 +21,22 @@
 //pypi.org/project/piperider/#files) [![license](https://img.shields.io/github/
 license/infuseai/piperider?style=flat-square)](https://github.com/InfuseAI/
 piperider/blob/main/LICENSE) [![InfuseAI Discord Invite](https://
 img.shields.io/discord/
 664381609771925514?color=%237289DA&label=chat&logo=discord&logoColor=white&style=flat-
 square)](https://discord.com/invite/5zb2aK9KBV)
                                   [PipeRider]
-# What's PipeRider? **[PipeRider](https://www.piperider.io/)** is a light-
-weight data reliability toolkit using warehouse-native profiling so you can
-have a full understanding of your data **We're in an early stage, so [let us
-know](mailto:product@infuseai.io) if you have any questions, feedback, or need
-help installing PipeRider! :heart:** ## Profiling as a data reliability
-strategy PipeRider will make your life easier by: 1. Building a data profile so
-you can easily understand your data 2. Creating test suggestions based on the
-profiling 3. Comparing data profile reports, so you track changes over time
-[Read how to implement a data quality strategy using profiling + testing]
-(https://blog.infuseai.io/add-data-profiling-and-assertions-to-dbt-with-
-piperider-732ca0821e3a) ## Made for the modern data team **For data engineers**
-* :zap: 2 min install & set-up * :relieved: Non-intrusive & open-source:
-install and use locally * :money_with_wings: Fast & cheap: 100M rows & 8
-columns (or 50M & 16 columns) takes only 18s to profile * :ledger: Cloud
-DataWarehouse native & auto-config for dbt **For data analysts** * :bowtie:
-Never waste time on analyzing wrong data: collects various metadata metrics
-such as freshness, uniqueness, distribution... [check all metrics](https://
-docs.piperider.io/data-profile-and-metrics/metrics) * :speech_balloon:
-Communicate easily your data expectations by showing the report * Zero-config
-dbt integration ## Live Demo [![](https://i.imgur.com/WuFC4H6.png)](https://
-piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-[Click here or on image to interact](https://piperider-github-readme.s3.ap-
-northeast-1.amazonaws.com/run-0.7.0/index.html)  ## Key features * [Generate an
-HTML Report](https://docs.piperider.io/how-to-guides/generate-report) featuring
-your data profile and data assertion test results ([interactive sample](https:/
-/piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
+# What's PipeRider? [PipeRider](https://www.piperider.io/) is a light-weight
+data quality tool so you can be confident of your data without writing tests
+for every single pipeline. **We're in an early stage, so [let us know](mailto:
+product@infuseai.io) if you have any questions, feedback, or need help
+installing PipeRider! :heart:** ## Key Features * [Generate an HTML Report]
+(https://docs.piperider.io/how-to-guides/generate-report) featuring your data
+profile and data assertion test results ([interactive sample](https://
+piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
 * [Compare two reports](https://docs.piperider.io/how-to-guides/compare-
 reports) to understand how your data has changed over time ([interactive
 sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/
 comparison-0.8.0/index.html)) * Test your data with data assertions: * Built-in
 [data assertions](https://docs.piperider.io/data-quality-assertions/assertion-
 configuration) * Extensible through [custom assertions](https://
 docs.piperider.io/data-quality-assertions/custom-assertions) * Auto-generated
@@ -64,48 +46,55 @@
 data-sources/bigquery-connector), [Redshift](https://docs.piperider.io/data-
 sources/redshift-connector), [DuckDB](https://docs.piperider.io/data-sources/
 duckdb-connector/), [CSV](https://docs.piperider.io/data-sources/csv-connector/
 ) and [Parquet](https://docs.piperider.io/data-sources/parquet-connector/). *
 Zero-config [support for dbt](https://docs.piperider.io/dbt-integration/
 ) projects * Automation through [GitHub Actions](https://docs.piperider.io/how-
 to-guides/github-action/), [save reports in S3](https://docs.piperider.io/how-
-to-guides/aws-s3-+-github-ci/) # Getting started Get started quickly below, go
-to [the docs](https://docs.piperider.io/), or check out this article on [how to
-add data observability using PipeRider ](https://blog.infuseai.io/adding-data-
-observability-and-alerts-to-your-data-pipeline-is-easier-than-you-think-
-4e005daca55b) ## Install PipeRider ```bash pip install piperider ``` By
-default, PipeRider supports built-in SQLite connector, extra connectors are
-available: | connectors | install | supported since | |---|---|----------------
---| | snowflake | pip install 'piperider[snowflake]' | | | postgres | pip
-install 'piperider[postgres]' | | | bigquery | pip install 'piperider
-[bigquery]' | PipeRider v0.7.0 | | redshift | pip install 'piperider[redshift]'
-| PipeRider v0.7.0 | | parquet | pip install 'piperider[parquet]' | PipeRider
-v0.8.0 | | csv | pip install 'piperider[csv]' | PipeRider v0.8.0 | | duckdb |
-pip install 'piperider[duckdb]' | PipeRider v0.8.0 | Use comma to install
-multiple connectors in one line: ```bash pip install 'piperider
-[postgres,snowflake]' ``` You can follow the [quick start guide](https://
-docs.piperider.io/quick-start) to learn more about PipeRider. ## Attach
-PipeRider to a dbt project Initialize PipeRider inside a dbt project and your
-data source settings will be automatically configured `piperider init` creates
-`/.piperider` under a dbt project root and generates necessary configurations.
-![piperider_init](images/init_pipe.gif) ## Scan data quality from models
-`piperider run` scans the models from data sources and creates assessment
-results in `/.piperider/output` ![piperider_run](images/run_pipe.gif) ##
-Generate reports `piperider generate-report` generate a static HTML report. !
-[piperider_report](images/report_pipe.gif) ## Generate comparison view You can
-use `piperider compare-report` to compare 2 reports. ![piperider_compare]
-(images/compare_pipe.gif) # Learn More | PipeRider Resources | Description | |
--------------------- | ----------- | | [Documentation] | PipeRider Main Doc
-Site | | [Sample_Project] | Sample Project with with sqlite | |
-[dbt_Sample_Project] | Sample Project with dbt | | [Roadmap] | PipeRider
+to-guides/aws-s3-+-github-ci/) ## Made for... **For data engineers** * :zap: 2
+min install & set-up * :relieved: non-intrusive & open-source: install and use
+locally * :moneybag: fast & cheap: 10M rows, 8 columns takes only 16s to
+profile **For data analysts** * :bowtie: never waste time on analyzing wrong
+data: collects various metadata metrics such as freshness, uniqueness,
+distribution... [check all metrics](https://docs.piperider.io/data-profile-and-
+metrics/metrics) * :speech_balloon: communicate easily your data expectations
+by showing the report ## Live Demo [![](https://i.imgur.com/WuFC4H6.png)]
+(https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/
+index.html) [Click here or on image to interact](https://piperider-github-
+readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html) # Getting started
+Get started quickly below, or go to [the docs](https://docs.piperider.io/) ##
+Install PipeRider ```bash pip install piperider ``` By default, PipeRider
+supports built-in SQLite connector, extra connectors are available: |
+connectors | install | supported since | |---|---|------------------| |
+snowflake | pip install 'piperider[snowflake]' | | | postgres | pip install
+'piperider[postgres]' | | | bigquery | pip install 'piperider[bigquery]' |
+PipeRider v0.7.0 | | redshift | pip install 'piperider[redshift]' | PipeRider
+v0.7.0 | | parquet | pip install 'piperider[parquet]' | PipeRider v0.8.0 | |
+csv | pip install 'piperider[csv]' | PipeRider v0.8.0 | | duckdb | pip install
+'piperider[duckdb]' | PipeRider v0.8.0 | Use comma to install multiple
+connectors in one line: ```bash pip install 'piperider[postgres,snowflake]' ```
+You can follow the [quick start guide](https://docs.piperider.io/quick-start)
+to learn more about PipeRider. ## Attach PipeRider to a dbt project `piperider
+init` creates `/.piperider` under a dbt project root and generates necessary
+configurations. ## Scan data quality from models `piperider run` runs
+profiling, and tests against assertions, and will render an HTML report
+`/.piperider/outputs` You can do a run for a specific table using `piperider
+run --table $TABLENAME` You can specifying the output location of a report
+using `piperider generate-report -o $PATHNAME` or specifying it in the config
+file. [All details on generating reports](https://docs.piperider.io/how-to-
+guides/generate-report) ## Generate comparison view You can use `piperider
+compare-report` to compare 2 reports. # Learn More | PipeRider Resources |
+Description | | -------------------- | ----------- | | [Documentation] |
+PipeRider Main Doc Site | | [Sample_Project] | Sample Project with with sqlite
+| | [dbt_Sample_Project] | Sample Project with dbt | | [Roadmap] | PipeRider
 Roadmap | | [Blog] | How we got started | [Documentation]: https://
 docs.piperider.io/ [Sample_Project]: https://github.com/InfuseAI/infuse-finance
 [dbt_Sample_Project]: https://github.com/InfuseAI/dbt-infuse-finance [Roadmap]:
 https://github.com/orgs/InfuseAI/projects/1/views/1 [Blog]: https://
 blog.infuseai.io/data-reliability-automated-with-piperider-7a823521ef11 # Get
-involved ## Support If you like what we are building, support us! Give us a :
-star: or get in touch. We'd love your feedback! Send us a message on
+involved ## Support :heart: If you like what we are building, support us! Give
+us a :star: or get in touch. We'd love your feedback! Send us a message on
 [piperider.io](https://piperider.io), join our [Discord](https://discord.com/
 invite/CrAxQznedH), or report an issue on [GitHub](https://github.com/InfuseAI/
 piperider/issues) ## Contributions We welcome contributions. See the [Set up
 dev environment](DEVELOP.md) and the [Contributing guildline](CONTRIBUTING.md)
 to get started.
```

### Comparing `piperider-0.9.0/README.md` & `piperider-0.9.0rc1/piperider.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,34 @@
-# PipeRider: Data Reliability Toolkit
+Metadata-Version: 2.1
+Name: piperider
+Version: 0.9.0rc1
+Summary: PiperRider CLI
+Home-page: https://github.com/InfuseAI/piperider
+Author: InfuseAI Dev Team
+Author-email: dev@infuseai.io
+Project-URL: Bug Tracker, https://github.com/InfuseAI/piperider/issues
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: snowflake
+Provides-Extra: postgres
+Provides-Extra: bigquery
+Provides-Extra: redshift
+Provides-Extra: duckdb
+Provides-Extra: csv
+Provides-Extra: parquet
+Provides-Extra: dev
+License-File: LICENSE
+
+# PipeRider: Data Reliability Automated
 
 [![ci-tests](https://github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)
 [![release](https://img.shields.io/github/release/infuseAI/piperider-cli/all.svg?style=flat-square)](https://github.com/infuseAI/piperider-cli/releases)
 [![pipy](https://img.shields.io/pypi/v/piperider?style=flat-square)](https://pypi.org/project/piperider/)
 [![python](https://img.shields.io/pypi/pyversions/piperider?style=flat-square)](https://pypi.org/project/piperider/)
 [![downloads](https://img.shields.io/pypi/dw/piperider?style=flat-square)](https://pypi.org/project/piperider/#files)
 [![license](https://img.shields.io/github/license/infuseai/piperider?style=flat-square)](https://github.com/InfuseAI/piperider/blob/main/LICENSE)
@@ -12,85 +38,50 @@
   <a href="https://piperider.io">
     <img  src=".github/images/logo.svg" border="0" alt="PipeRider">
   </a>
 </p>
 
 
 # What's PipeRider?
-**[PipeRider](https://www.piperider.io/)** is a light-weight data reliability toolkit using warehouse-native profiling so you can have a full understanding of your data 
+[PipeRider](https://www.piperider.io/) is a light-weight data quality tool so you can be confident of your data without writing tests for every single pipeline. 
 
 **We're in an early stage, so [let us know](mailto:product@infuseai.io) if you have any questions, feedback, or need help installing PipeRider! :heart:**
 
 
-
-## Profiling as a data reliability strategy
-PipeRider will make your life easier by:
-1. Building a data profile so you can easily understand your data
-2. Creating test suggestions based on the profiling
-3. Comparing data profile reports, so you track changes over time
-
-[Read how to implement a data quality strategy using profiling + testing](https://blog.infuseai.io/add-data-profiling-and-assertions-to-dbt-with-piperider-732ca0821e3a)
-
-
-
-## Made for the modern data team
-**For data engineers**
-* :zap: 2 min install & set-up
-* :relieved: Non-intrusive & open-source: install and use locally
-* :money_with_wings: Fast & cheap: 100M rows & 8 columns (or 50M & 16 columns) takes only 18s to profile
-* :ledger: Cloud DataWarehouse native & auto-config for dbt
-
-
-
-**For data analysts**
-* :bowtie: Never waste time on analyzing wrong data: collects various metadata metrics such as freshness, uniqueness, distribution... [check all metrics](https://docs.piperider.io/data-profile-and-metrics/metrics)
-* :speech_balloon: Communicate easily your data expectations by showing the report
-* Zero-config dbt integration
-
-
-## Live Demo
-[![](https://i.imgur.com/WuFC4H6.png)](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-
-[Click here or on image to interact](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-
-<!-- # Table of contents
-* [What's PipeRider?](#what's-piperider?)
-    * [Made for...](#made-for...)
-    * [Live demo](#live-demo)
-* [Table of contents](#table-of-contents)
-* [Getting started](#getting-started)
-    * [Install piperider](#install-piperider)
-    * [Attach PipeRider to a dbt project](#attach-piperider-to-a-dbt-project)
-    * [Scan data quality from models](#scan-data-quality-from-models)
-    * [Generate reports](#generate-reports)
-    * [Generate comparison view](#generate-comparison-view)
-* [Learn more](#learn-more)
-* [Get involved](#get-involved)
-    * [Support](#support)
-    * [Contributions](#contributions)
- -->
-
-
-## Key features
+## Key Features
 * [Generate an HTML Report](https://docs.piperider.io/how-to-guides/generate-report) featuring your data profile and data assertion test results ([interactive sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
 * [Compare two reports](https://docs.piperider.io/how-to-guides/compare-reports) to understand how your data has changed over time ([interactive sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/comparison-0.8.0/index.html))
 * Test your data with data assertions:
   * Built-in [data assertions](https://docs.piperider.io/data-quality-assertions/assertion-configuration)
   * Extensible through [custom assertions](https://docs.piperider.io/data-quality-assertions/custom-assertions)
   * Auto-generated data assertions
 * Currently supports [Postgres](https://docs.piperider.io/data-sources/postgres-connector), [Snowflake](https://docs.piperider.io/data-sources/snowflake-connector), SQLite, [BigQuery](https://docs.piperider.io/data-sources/bigquery-connector), [Redshift](https://docs.piperider.io/data-sources/redshift-connector), [DuckDB](https://docs.piperider.io/data-sources/duckdb-connector/), [CSV](https://docs.piperider.io/data-sources/csv-connector/) and [Parquet](https://docs.piperider.io/data-sources/parquet-connector/).
 * Zero-config [support for dbt](https://docs.piperider.io/dbt-integration/) projects
 * Automation through [GitHub Actions](https://docs.piperider.io/how-to-guides/github-action/), [save reports in S3](https://docs.piperider.io/how-to-guides/aws-s3-+-github-ci/)
 
+## Made for...
+**For data engineers**
+* :zap: 2 min install & set-up
+* :relieved: non-intrusive & open-source: install and use locally
+* :moneybag: fast & cheap: 10M rows, 8 columns takes only 16s to profile
+
 
+**For data analysts**
+* :bowtie: never waste time on analyzing wrong data: collects various metadata metrics such as freshness, uniqueness, distribution... [check all metrics](https://docs.piperider.io/data-profile-and-metrics/metrics)
+* :speech_balloon: communicate easily your data expectations by showing the report
+
+
+## Live Demo
+[![](https://i.imgur.com/WuFC4H6.png)](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html)
 
+[Click here or on image to interact](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html)
 
 # Getting started
 
-Get started quickly below, go to [the docs](https://docs.piperider.io/), or check out this article on [how to add data observability using PipeRider ](https://blog.infuseai.io/adding-data-observability-and-alerts-to-your-data-pipeline-is-easier-than-you-think-4e005daca55b)
+Get started quickly below, or go to [the docs](https://docs.piperider.io/)
 
 ## Install PipeRider
 
 ```bash
 pip install piperider
 ```
 
@@ -111,37 +102,30 @@
 ```bash
 pip install 'piperider[postgres,snowflake]'
 ```
 
 You can follow the [quick start guide](https://docs.piperider.io/quick-start) to learn more about PipeRider.
 
 ## Attach PipeRider to a dbt project
-Initialize PipeRider inside a dbt project and your data source settings will be automatically configured
 
 `piperider init` creates `/.piperider` under a dbt project root and generates necessary configurations.
 
-![piperider_init](images/init_pipe.gif)
-
 ## Scan data quality from models
 
-`piperider run` scans the models from data sources and creates assessment results in `/.piperider/output`
-
-![piperider_run](images/run_pipe.gif)
-
-## Generate reports
+`piperider run` runs profiling, and tests against assertions, and will render an HTML report `/.piperider/outputs`
 
-`piperider generate-report` generate a static HTML report.
+You can do a run for a specific table using `piperider run --table $TABLENAME`
+You can specifying the output location of a report using `piperider generate-report -o $PATHNAME` or specifying it in the config file.
 
-![piperider_report](images/report_pipe.gif)
+[All details on generating reports](https://docs.piperider.io/how-to-guides/generate-report)
 
 ## Generate comparison view
 
 You can use `piperider compare-report` to compare 2 reports.
 
-![piperider_compare](images/compare_pipe.gif)
 
 # Learn More
 
 | PipeRider Resources | Description |
 | -------------------- | ----------- |
 | [Documentation] | PipeRider Main Doc Site |
 | [Sample_Project] | Sample Project with with sqlite |
@@ -158,14 +142,14 @@
 
 [Roadmap]: https://github.com/orgs/InfuseAI/projects/1/views/1
 
 [Blog]: https://blog.infuseai.io/data-reliability-automated-with-piperider-7a823521ef11
 
 # Get involved
 
-## Support 
+## Support :heart:
 If you like what we are building, support us! Give us a :star: or get in touch. We'd love your feedback! Send us a message on [piperider.io](https://piperider.io), join our [Discord](https://discord.com/invite/CrAxQznedH), or report an issue on [GitHub](https://github.com/InfuseAI/piperider/issues)
 
 
 ## Contributions
 
 We welcome contributions. See the [Set up dev environment](DEVELOP.md) and the [Contributing guildline](CONTRIBUTING.md) to get started.
```

#### html2text {}

```diff
@@ -1,8 +1,19 @@
-# PipeRider: Data Reliability Toolkit [![ci-tests](https://github.com/infuseai/
+Metadata-Version: 2.1 Name: piperider Version: 0.9.0rc1 Summary: PiperRider CLI
+Home-page: https://github.com/InfuseAI/piperider Author: InfuseAI Dev Team
+Author-email: dev@infuseai.io Project-URL: Bug Tracker, https://github.com/
+InfuseAI/piperider/issues Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Classifier:
+Development Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type:
+text/markdown Provides-Extra: snowflake Provides-Extra: postgres Provides-
+Extra: bigquery Provides-Extra: redshift Provides-Extra: duckdb Provides-Extra:
+csv Provides-Extra: parquet Provides-Extra: dev License-File: LICENSE #
+PipeRider: Data Reliability Automated [![ci-tests](https://github.com/infuseai/
 piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://github.com/
 infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg) [![release]
 (https://img.shields.io/github/release/infuseAI/piperider-cli/
 all.svg?style=flat-square)](https://github.com/infuseAI/piperider-cli/releases)
 [![pipy](https://img.shields.io/pypi/v/piperider?style=flat-square)](https://
 pypi.org/project/piperider/) [![python](https://img.shields.io/pypi/pyversions/
 piperider?style=flat-square)](https://pypi.org/project/piperider/) [!
@@ -10,40 +21,22 @@
 //pypi.org/project/piperider/#files) [![license](https://img.shields.io/github/
 license/infuseai/piperider?style=flat-square)](https://github.com/InfuseAI/
 piperider/blob/main/LICENSE) [![InfuseAI Discord Invite](https://
 img.shields.io/discord/
 664381609771925514?color=%237289DA&label=chat&logo=discord&logoColor=white&style=flat-
 square)](https://discord.com/invite/5zb2aK9KBV)
                                   [PipeRider]
-# What's PipeRider? **[PipeRider](https://www.piperider.io/)** is a light-
-weight data reliability toolkit using warehouse-native profiling so you can
-have a full understanding of your data **We're in an early stage, so [let us
-know](mailto:product@infuseai.io) if you have any questions, feedback, or need
-help installing PipeRider! :heart:** ## Profiling as a data reliability
-strategy PipeRider will make your life easier by: 1. Building a data profile so
-you can easily understand your data 2. Creating test suggestions based on the
-profiling 3. Comparing data profile reports, so you track changes over time
-[Read how to implement a data quality strategy using profiling + testing]
-(https://blog.infuseai.io/add-data-profiling-and-assertions-to-dbt-with-
-piperider-732ca0821e3a) ## Made for the modern data team **For data engineers**
-* :zap: 2 min install & set-up * :relieved: Non-intrusive & open-source:
-install and use locally * :money_with_wings: Fast & cheap: 100M rows & 8
-columns (or 50M & 16 columns) takes only 18s to profile * :ledger: Cloud
-DataWarehouse native & auto-config for dbt **For data analysts** * :bowtie:
-Never waste time on analyzing wrong data: collects various metadata metrics
-such as freshness, uniqueness, distribution... [check all metrics](https://
-docs.piperider.io/data-profile-and-metrics/metrics) * :speech_balloon:
-Communicate easily your data expectations by showing the report * Zero-config
-dbt integration ## Live Demo [![](https://i.imgur.com/WuFC4H6.png)](https://
-piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-[Click here or on image to interact](https://piperider-github-readme.s3.ap-
-northeast-1.amazonaws.com/run-0.7.0/index.html)  ## Key features * [Generate an
-HTML Report](https://docs.piperider.io/how-to-guides/generate-report) featuring
-your data profile and data assertion test results ([interactive sample](https:/
-/piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
+# What's PipeRider? [PipeRider](https://www.piperider.io/) is a light-weight
+data quality tool so you can be confident of your data without writing tests
+for every single pipeline. **We're in an early stage, so [let us know](mailto:
+product@infuseai.io) if you have any questions, feedback, or need help
+installing PipeRider! :heart:** ## Key Features * [Generate an HTML Report]
+(https://docs.piperider.io/how-to-guides/generate-report) featuring your data
+profile and data assertion test results ([interactive sample](https://
+piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
 * [Compare two reports](https://docs.piperider.io/how-to-guides/compare-
 reports) to understand how your data has changed over time ([interactive
 sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/
 comparison-0.8.0/index.html)) * Test your data with data assertions: * Built-in
 [data assertions](https://docs.piperider.io/data-quality-assertions/assertion-
 configuration) * Extensible through [custom assertions](https://
 docs.piperider.io/data-quality-assertions/custom-assertions) * Auto-generated
@@ -53,48 +46,55 @@
 data-sources/bigquery-connector), [Redshift](https://docs.piperider.io/data-
 sources/redshift-connector), [DuckDB](https://docs.piperider.io/data-sources/
 duckdb-connector/), [CSV](https://docs.piperider.io/data-sources/csv-connector/
 ) and [Parquet](https://docs.piperider.io/data-sources/parquet-connector/). *
 Zero-config [support for dbt](https://docs.piperider.io/dbt-integration/
 ) projects * Automation through [GitHub Actions](https://docs.piperider.io/how-
 to-guides/github-action/), [save reports in S3](https://docs.piperider.io/how-
-to-guides/aws-s3-+-github-ci/) # Getting started Get started quickly below, go
-to [the docs](https://docs.piperider.io/), or check out this article on [how to
-add data observability using PipeRider ](https://blog.infuseai.io/adding-data-
-observability-and-alerts-to-your-data-pipeline-is-easier-than-you-think-
-4e005daca55b) ## Install PipeRider ```bash pip install piperider ``` By
-default, PipeRider supports built-in SQLite connector, extra connectors are
-available: | connectors | install | supported since | |---|---|----------------
---| | snowflake | pip install 'piperider[snowflake]' | | | postgres | pip
-install 'piperider[postgres]' | | | bigquery | pip install 'piperider
-[bigquery]' | PipeRider v0.7.0 | | redshift | pip install 'piperider[redshift]'
-| PipeRider v0.7.0 | | parquet | pip install 'piperider[parquet]' | PipeRider
-v0.8.0 | | csv | pip install 'piperider[csv]' | PipeRider v0.8.0 | | duckdb |
-pip install 'piperider[duckdb]' | PipeRider v0.8.0 | Use comma to install
-multiple connectors in one line: ```bash pip install 'piperider
-[postgres,snowflake]' ``` You can follow the [quick start guide](https://
-docs.piperider.io/quick-start) to learn more about PipeRider. ## Attach
-PipeRider to a dbt project Initialize PipeRider inside a dbt project and your
-data source settings will be automatically configured `piperider init` creates
-`/.piperider` under a dbt project root and generates necessary configurations.
-![piperider_init](images/init_pipe.gif) ## Scan data quality from models
-`piperider run` scans the models from data sources and creates assessment
-results in `/.piperider/output` ![piperider_run](images/run_pipe.gif) ##
-Generate reports `piperider generate-report` generate a static HTML report. !
-[piperider_report](images/report_pipe.gif) ## Generate comparison view You can
-use `piperider compare-report` to compare 2 reports. ![piperider_compare]
-(images/compare_pipe.gif) # Learn More | PipeRider Resources | Description | |
--------------------- | ----------- | | [Documentation] | PipeRider Main Doc
-Site | | [Sample_Project] | Sample Project with with sqlite | |
-[dbt_Sample_Project] | Sample Project with dbt | | [Roadmap] | PipeRider
+to-guides/aws-s3-+-github-ci/) ## Made for... **For data engineers** * :zap: 2
+min install & set-up * :relieved: non-intrusive & open-source: install and use
+locally * :moneybag: fast & cheap: 10M rows, 8 columns takes only 16s to
+profile **For data analysts** * :bowtie: never waste time on analyzing wrong
+data: collects various metadata metrics such as freshness, uniqueness,
+distribution... [check all metrics](https://docs.piperider.io/data-profile-and-
+metrics/metrics) * :speech_balloon: communicate easily your data expectations
+by showing the report ## Live Demo [![](https://i.imgur.com/WuFC4H6.png)]
+(https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/
+index.html) [Click here or on image to interact](https://piperider-github-
+readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html) # Getting started
+Get started quickly below, or go to [the docs](https://docs.piperider.io/) ##
+Install PipeRider ```bash pip install piperider ``` By default, PipeRider
+supports built-in SQLite connector, extra connectors are available: |
+connectors | install | supported since | |---|---|------------------| |
+snowflake | pip install 'piperider[snowflake]' | | | postgres | pip install
+'piperider[postgres]' | | | bigquery | pip install 'piperider[bigquery]' |
+PipeRider v0.7.0 | | redshift | pip install 'piperider[redshift]' | PipeRider
+v0.7.0 | | parquet | pip install 'piperider[parquet]' | PipeRider v0.8.0 | |
+csv | pip install 'piperider[csv]' | PipeRider v0.8.0 | | duckdb | pip install
+'piperider[duckdb]' | PipeRider v0.8.0 | Use comma to install multiple
+connectors in one line: ```bash pip install 'piperider[postgres,snowflake]' ```
+You can follow the [quick start guide](https://docs.piperider.io/quick-start)
+to learn more about PipeRider. ## Attach PipeRider to a dbt project `piperider
+init` creates `/.piperider` under a dbt project root and generates necessary
+configurations. ## Scan data quality from models `piperider run` runs
+profiling, and tests against assertions, and will render an HTML report
+`/.piperider/outputs` You can do a run for a specific table using `piperider
+run --table $TABLENAME` You can specifying the output location of a report
+using `piperider generate-report -o $PATHNAME` or specifying it in the config
+file. [All details on generating reports](https://docs.piperider.io/how-to-
+guides/generate-report) ## Generate comparison view You can use `piperider
+compare-report` to compare 2 reports. # Learn More | PipeRider Resources |
+Description | | -------------------- | ----------- | | [Documentation] |
+PipeRider Main Doc Site | | [Sample_Project] | Sample Project with with sqlite
+| | [dbt_Sample_Project] | Sample Project with dbt | | [Roadmap] | PipeRider
 Roadmap | | [Blog] | How we got started | [Documentation]: https://
 docs.piperider.io/ [Sample_Project]: https://github.com/InfuseAI/infuse-finance
 [dbt_Sample_Project]: https://github.com/InfuseAI/dbt-infuse-finance [Roadmap]:
 https://github.com/orgs/InfuseAI/projects/1/views/1 [Blog]: https://
 blog.infuseai.io/data-reliability-automated-with-piperider-7a823521ef11 # Get
-involved ## Support If you like what we are building, support us! Give us a :
-star: or get in touch. We'd love your feedback! Send us a message on
+involved ## Support :heart: If you like what we are building, support us! Give
+us a :star: or get in touch. We'd love your feedback! Send us a message on
 [piperider.io](https://piperider.io), join our [Discord](https://discord.com/
 invite/CrAxQznedH), or report an issue on [GitHub](https://github.com/InfuseAI/
 piperider/issues) ## Contributions We welcome contributions. See the [Set up
 dev environment](DEVELOP.md) and the [Contributing guildline](CONTRIBUTING.md)
 to get started.
```

### Comparing `piperider-0.9.0/piperider.egg-info/PKG-INFO` & `piperider-0.9.0rc1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,8 @@
-Metadata-Version: 2.1
-Name: piperider
-Version: 0.9.0
-Summary: PiperRider CLI
-Home-page: https://github.com/InfuseAI/piperider
-Author: InfuseAI Dev Team
-Author-email: dev@infuseai.io
-Project-URL: Bug Tracker, https://github.com/InfuseAI/piperider/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: snowflake
-Provides-Extra: postgres
-Provides-Extra: bigquery
-Provides-Extra: redshift
-Provides-Extra: duckdb
-Provides-Extra: csv
-Provides-Extra: parquet
-Provides-Extra: dev
-License-File: LICENSE
-
-# PipeRider: Data Reliability Toolkit
+# PipeRider: Data Reliability Automated
 
 [![ci-tests](https://github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)
 [![release](https://img.shields.io/github/release/infuseAI/piperider-cli/all.svg?style=flat-square)](https://github.com/infuseAI/piperider-cli/releases)
 [![pipy](https://img.shields.io/pypi/v/piperider?style=flat-square)](https://pypi.org/project/piperider/)
 [![python](https://img.shields.io/pypi/pyversions/piperider?style=flat-square)](https://pypi.org/project/piperider/)
 [![downloads](https://img.shields.io/pypi/dw/piperider?style=flat-square)](https://pypi.org/project/piperider/#files)
 [![license](https://img.shields.io/github/license/infuseai/piperider?style=flat-square)](https://github.com/InfuseAI/piperider/blob/main/LICENSE)
@@ -38,85 +12,50 @@
   <a href="https://piperider.io">
     <img  src=".github/images/logo.svg" border="0" alt="PipeRider">
   </a>
 </p>
 
 
 # What's PipeRider?
-**[PipeRider](https://www.piperider.io/)** is a light-weight data reliability toolkit using warehouse-native profiling so you can have a full understanding of your data 
+[PipeRider](https://www.piperider.io/) is a light-weight data quality tool so you can be confident of your data without writing tests for every single pipeline. 
 
 **We're in an early stage, so [let us know](mailto:product@infuseai.io) if you have any questions, feedback, or need help installing PipeRider! :heart:**
 
 
-
-## Profiling as a data reliability strategy
-PipeRider will make your life easier by:
-1. Building a data profile so you can easily understand your data
-2. Creating test suggestions based on the profiling
-3. Comparing data profile reports, so you track changes over time
-
-[Read how to implement a data quality strategy using profiling + testing](https://blog.infuseai.io/add-data-profiling-and-assertions-to-dbt-with-piperider-732ca0821e3a)
-
-
-
-## Made for the modern data team
-**For data engineers**
-* :zap: 2 min install & set-up
-* :relieved: Non-intrusive & open-source: install and use locally
-* :money_with_wings: Fast & cheap: 100M rows & 8 columns (or 50M & 16 columns) takes only 18s to profile
-* :ledger: Cloud DataWarehouse native & auto-config for dbt
-
-
-
-**For data analysts**
-* :bowtie: Never waste time on analyzing wrong data: collects various metadata metrics such as freshness, uniqueness, distribution... [check all metrics](https://docs.piperider.io/data-profile-and-metrics/metrics)
-* :speech_balloon: Communicate easily your data expectations by showing the report
-* Zero-config dbt integration
-
-
-## Live Demo
-[![](https://i.imgur.com/WuFC4H6.png)](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-
-[Click here or on image to interact](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-
-<!-- # Table of contents
-* [What's PipeRider?](#what's-piperider?)
-    * [Made for...](#made-for...)
-    * [Live demo](#live-demo)
-* [Table of contents](#table-of-contents)
-* [Getting started](#getting-started)
-    * [Install piperider](#install-piperider)
-    * [Attach PipeRider to a dbt project](#attach-piperider-to-a-dbt-project)
-    * [Scan data quality from models](#scan-data-quality-from-models)
-    * [Generate reports](#generate-reports)
-    * [Generate comparison view](#generate-comparison-view)
-* [Learn more](#learn-more)
-* [Get involved](#get-involved)
-    * [Support](#support)
-    * [Contributions](#contributions)
- -->
-
-
-## Key features
+## Key Features
 * [Generate an HTML Report](https://docs.piperider.io/how-to-guides/generate-report) featuring your data profile and data assertion test results ([interactive sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
 * [Compare two reports](https://docs.piperider.io/how-to-guides/compare-reports) to understand how your data has changed over time ([interactive sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/comparison-0.8.0/index.html))
 * Test your data with data assertions:
   * Built-in [data assertions](https://docs.piperider.io/data-quality-assertions/assertion-configuration)
   * Extensible through [custom assertions](https://docs.piperider.io/data-quality-assertions/custom-assertions)
   * Auto-generated data assertions
 * Currently supports [Postgres](https://docs.piperider.io/data-sources/postgres-connector), [Snowflake](https://docs.piperider.io/data-sources/snowflake-connector), SQLite, [BigQuery](https://docs.piperider.io/data-sources/bigquery-connector), [Redshift](https://docs.piperider.io/data-sources/redshift-connector), [DuckDB](https://docs.piperider.io/data-sources/duckdb-connector/), [CSV](https://docs.piperider.io/data-sources/csv-connector/) and [Parquet](https://docs.piperider.io/data-sources/parquet-connector/).
 * Zero-config [support for dbt](https://docs.piperider.io/dbt-integration/) projects
 * Automation through [GitHub Actions](https://docs.piperider.io/how-to-guides/github-action/), [save reports in S3](https://docs.piperider.io/how-to-guides/aws-s3-+-github-ci/)
 
+## Made for...
+**For data engineers**
+* :zap: 2 min install & set-up
+* :relieved: non-intrusive & open-source: install and use locally
+* :moneybag: fast & cheap: 10M rows, 8 columns takes only 16s to profile
+
 
+**For data analysts**
+* :bowtie: never waste time on analyzing wrong data: collects various metadata metrics such as freshness, uniqueness, distribution... [check all metrics](https://docs.piperider.io/data-profile-and-metrics/metrics)
+* :speech_balloon: communicate easily your data expectations by showing the report
+
+
+## Live Demo
+[![](https://i.imgur.com/WuFC4H6.png)](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html)
 
+[Click here or on image to interact](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html)
 
 # Getting started
 
-Get started quickly below, go to [the docs](https://docs.piperider.io/), or check out this article on [how to add data observability using PipeRider ](https://blog.infuseai.io/adding-data-observability-and-alerts-to-your-data-pipeline-is-easier-than-you-think-4e005daca55b)
+Get started quickly below, or go to [the docs](https://docs.piperider.io/)
 
 ## Install PipeRider
 
 ```bash
 pip install piperider
 ```
 
@@ -137,37 +76,30 @@
 ```bash
 pip install 'piperider[postgres,snowflake]'
 ```
 
 You can follow the [quick start guide](https://docs.piperider.io/quick-start) to learn more about PipeRider.
 
 ## Attach PipeRider to a dbt project
-Initialize PipeRider inside a dbt project and your data source settings will be automatically configured
 
 `piperider init` creates `/.piperider` under a dbt project root and generates necessary configurations.
 
-![piperider_init](images/init_pipe.gif)
-
 ## Scan data quality from models
 
-`piperider run` scans the models from data sources and creates assessment results in `/.piperider/output`
-
-![piperider_run](images/run_pipe.gif)
-
-## Generate reports
+`piperider run` runs profiling, and tests against assertions, and will render an HTML report `/.piperider/outputs`
 
-`piperider generate-report` generate a static HTML report.
+You can do a run for a specific table using `piperider run --table $TABLENAME`
+You can specifying the output location of a report using `piperider generate-report -o $PATHNAME` or specifying it in the config file.
 
-![piperider_report](images/report_pipe.gif)
+[All details on generating reports](https://docs.piperider.io/how-to-guides/generate-report)
 
 ## Generate comparison view
 
 You can use `piperider compare-report` to compare 2 reports.
 
-![piperider_compare](images/compare_pipe.gif)
 
 # Learn More
 
 | PipeRider Resources | Description |
 | -------------------- | ----------- |
 | [Documentation] | PipeRider Main Doc Site |
 | [Sample_Project] | Sample Project with with sqlite |
@@ -184,14 +116,14 @@
 
 [Roadmap]: https://github.com/orgs/InfuseAI/projects/1/views/1
 
 [Blog]: https://blog.infuseai.io/data-reliability-automated-with-piperider-7a823521ef11
 
 # Get involved
 
-## Support 
+## Support :heart:
 If you like what we are building, support us! Give us a :star: or get in touch. We'd love your feedback! Send us a message on [piperider.io](https://piperider.io), join our [Discord](https://discord.com/invite/CrAxQznedH), or report an issue on [GitHub](https://github.com/InfuseAI/piperider/issues)
 
 
 ## Contributions
 
 We welcome contributions. See the [Set up dev environment](DEVELOP.md) and the [Contributing guildline](CONTRIBUTING.md) to get started.
```

#### html2text {}

```diff
@@ -1,60 +1,31 @@
-Metadata-Version: 2.1 Name: piperider Version: 0.9.0 Summary: PiperRider CLI
-Home-page: https://github.com/InfuseAI/piperider Author: InfuseAI Dev Team
-Author-email: dev@infuseai.io Project-URL: Bug Tracker, https://github.com/
-InfuseAI/piperider/issues Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Development Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: snowflake Provides-Extra: postgres Provides-
-Extra: bigquery Provides-Extra: redshift Provides-Extra: duckdb Provides-Extra:
-csv Provides-Extra: parquet Provides-Extra: dev License-File: LICENSE #
-PipeRider: Data Reliability Toolkit [![ci-tests](https://github.com/infuseai/
-piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://github.com/
-infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg) [![release]
-(https://img.shields.io/github/release/infuseAI/piperider-cli/
+# PipeRider: Data Reliability Automated [![ci-tests](https://github.com/
+infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg)](https://
+github.com/infuseai/piperider-cli/actions/workflows/tests.yaml/badge.svg) [!
+[release](https://img.shields.io/github/release/infuseAI/piperider-cli/
 all.svg?style=flat-square)](https://github.com/infuseAI/piperider-cli/releases)
 [![pipy](https://img.shields.io/pypi/v/piperider?style=flat-square)](https://
 pypi.org/project/piperider/) [![python](https://img.shields.io/pypi/pyversions/
 piperider?style=flat-square)](https://pypi.org/project/piperider/) [!
 [downloads](https://img.shields.io/pypi/dw/piperider?style=flat-square)](https:
 //pypi.org/project/piperider/#files) [![license](https://img.shields.io/github/
 license/infuseai/piperider?style=flat-square)](https://github.com/InfuseAI/
 piperider/blob/main/LICENSE) [![InfuseAI Discord Invite](https://
 img.shields.io/discord/
 664381609771925514?color=%237289DA&label=chat&logo=discord&logoColor=white&style=flat-
 square)](https://discord.com/invite/5zb2aK9KBV)
                                   [PipeRider]
-# What's PipeRider? **[PipeRider](https://www.piperider.io/)** is a light-
-weight data reliability toolkit using warehouse-native profiling so you can
-have a full understanding of your data **We're in an early stage, so [let us
-know](mailto:product@infuseai.io) if you have any questions, feedback, or need
-help installing PipeRider! :heart:** ## Profiling as a data reliability
-strategy PipeRider will make your life easier by: 1. Building a data profile so
-you can easily understand your data 2. Creating test suggestions based on the
-profiling 3. Comparing data profile reports, so you track changes over time
-[Read how to implement a data quality strategy using profiling + testing]
-(https://blog.infuseai.io/add-data-profiling-and-assertions-to-dbt-with-
-piperider-732ca0821e3a) ## Made for the modern data team **For data engineers**
-* :zap: 2 min install & set-up * :relieved: Non-intrusive & open-source:
-install and use locally * :money_with_wings: Fast & cheap: 100M rows & 8
-columns (or 50M & 16 columns) takes only 18s to profile * :ledger: Cloud
-DataWarehouse native & auto-config for dbt **For data analysts** * :bowtie:
-Never waste time on analyzing wrong data: collects various metadata metrics
-such as freshness, uniqueness, distribution... [check all metrics](https://
-docs.piperider.io/data-profile-and-metrics/metrics) * :speech_balloon:
-Communicate easily your data expectations by showing the report * Zero-config
-dbt integration ## Live Demo [![](https://i.imgur.com/WuFC4H6.png)](https://
-piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.7.0/index.html)
-[Click here or on image to interact](https://piperider-github-readme.s3.ap-
-northeast-1.amazonaws.com/run-0.7.0/index.html)  ## Key features * [Generate an
-HTML Report](https://docs.piperider.io/how-to-guides/generate-report) featuring
-your data profile and data assertion test results ([interactive sample](https:/
-/piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
+# What's PipeRider? [PipeRider](https://www.piperider.io/) is a light-weight
+data quality tool so you can be confident of your data without writing tests
+for every single pipeline. **We're in an early stage, so [let us know](mailto:
+product@infuseai.io) if you have any questions, feedback, or need help
+installing PipeRider! :heart:** ## Key Features * [Generate an HTML Report]
+(https://docs.piperider.io/how-to-guides/generate-report) featuring your data
+profile and data assertion test results ([interactive sample](https://
+piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html))
 * [Compare two reports](https://docs.piperider.io/how-to-guides/compare-
 reports) to understand how your data has changed over time ([interactive
 sample](https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/
 comparison-0.8.0/index.html)) * Test your data with data assertions: * Built-in
 [data assertions](https://docs.piperider.io/data-quality-assertions/assertion-
 configuration) * Extensible through [custom assertions](https://
 docs.piperider.io/data-quality-assertions/custom-assertions) * Auto-generated
@@ -64,48 +35,55 @@
 data-sources/bigquery-connector), [Redshift](https://docs.piperider.io/data-
 sources/redshift-connector), [DuckDB](https://docs.piperider.io/data-sources/
 duckdb-connector/), [CSV](https://docs.piperider.io/data-sources/csv-connector/
 ) and [Parquet](https://docs.piperider.io/data-sources/parquet-connector/). *
 Zero-config [support for dbt](https://docs.piperider.io/dbt-integration/
 ) projects * Automation through [GitHub Actions](https://docs.piperider.io/how-
 to-guides/github-action/), [save reports in S3](https://docs.piperider.io/how-
-to-guides/aws-s3-+-github-ci/) # Getting started Get started quickly below, go
-to [the docs](https://docs.piperider.io/), or check out this article on [how to
-add data observability using PipeRider ](https://blog.infuseai.io/adding-data-
-observability-and-alerts-to-your-data-pipeline-is-easier-than-you-think-
-4e005daca55b) ## Install PipeRider ```bash pip install piperider ``` By
-default, PipeRider supports built-in SQLite connector, extra connectors are
-available: | connectors | install | supported since | |---|---|----------------
---| | snowflake | pip install 'piperider[snowflake]' | | | postgres | pip
-install 'piperider[postgres]' | | | bigquery | pip install 'piperider
-[bigquery]' | PipeRider v0.7.0 | | redshift | pip install 'piperider[redshift]'
-| PipeRider v0.7.0 | | parquet | pip install 'piperider[parquet]' | PipeRider
-v0.8.0 | | csv | pip install 'piperider[csv]' | PipeRider v0.8.0 | | duckdb |
-pip install 'piperider[duckdb]' | PipeRider v0.8.0 | Use comma to install
-multiple connectors in one line: ```bash pip install 'piperider
-[postgres,snowflake]' ``` You can follow the [quick start guide](https://
-docs.piperider.io/quick-start) to learn more about PipeRider. ## Attach
-PipeRider to a dbt project Initialize PipeRider inside a dbt project and your
-data source settings will be automatically configured `piperider init` creates
-`/.piperider` under a dbt project root and generates necessary configurations.
-![piperider_init](images/init_pipe.gif) ## Scan data quality from models
-`piperider run` scans the models from data sources and creates assessment
-results in `/.piperider/output` ![piperider_run](images/run_pipe.gif) ##
-Generate reports `piperider generate-report` generate a static HTML report. !
-[piperider_report](images/report_pipe.gif) ## Generate comparison view You can
-use `piperider compare-report` to compare 2 reports. ![piperider_compare]
-(images/compare_pipe.gif) # Learn More | PipeRider Resources | Description | |
--------------------- | ----------- | | [Documentation] | PipeRider Main Doc
-Site | | [Sample_Project] | Sample Project with with sqlite | |
-[dbt_Sample_Project] | Sample Project with dbt | | [Roadmap] | PipeRider
+to-guides/aws-s3-+-github-ci/) ## Made for... **For data engineers** * :zap: 2
+min install & set-up * :relieved: non-intrusive & open-source: install and use
+locally * :moneybag: fast & cheap: 10M rows, 8 columns takes only 16s to
+profile **For data analysts** * :bowtie: never waste time on analyzing wrong
+data: collects various metadata metrics such as freshness, uniqueness,
+distribution... [check all metrics](https://docs.piperider.io/data-profile-and-
+metrics/metrics) * :speech_balloon: communicate easily your data expectations
+by showing the report ## Live Demo [![](https://i.imgur.com/WuFC4H6.png)]
+(https://piperider-github-readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/
+index.html) [Click here or on image to interact](https://piperider-github-
+readme.s3.ap-northeast-1.amazonaws.com/run-0.8.0/index.html) # Getting started
+Get started quickly below, or go to [the docs](https://docs.piperider.io/) ##
+Install PipeRider ```bash pip install piperider ``` By default, PipeRider
+supports built-in SQLite connector, extra connectors are available: |
+connectors | install | supported since | |---|---|------------------| |
+snowflake | pip install 'piperider[snowflake]' | | | postgres | pip install
+'piperider[postgres]' | | | bigquery | pip install 'piperider[bigquery]' |
+PipeRider v0.7.0 | | redshift | pip install 'piperider[redshift]' | PipeRider
+v0.7.0 | | parquet | pip install 'piperider[parquet]' | PipeRider v0.8.0 | |
+csv | pip install 'piperider[csv]' | PipeRider v0.8.0 | | duckdb | pip install
+'piperider[duckdb]' | PipeRider v0.8.0 | Use comma to install multiple
+connectors in one line: ```bash pip install 'piperider[postgres,snowflake]' ```
+You can follow the [quick start guide](https://docs.piperider.io/quick-start)
+to learn more about PipeRider. ## Attach PipeRider to a dbt project `piperider
+init` creates `/.piperider` under a dbt project root and generates necessary
+configurations. ## Scan data quality from models `piperider run` runs
+profiling, and tests against assertions, and will render an HTML report
+`/.piperider/outputs` You can do a run for a specific table using `piperider
+run --table $TABLENAME` You can specifying the output location of a report
+using `piperider generate-report -o $PATHNAME` or specifying it in the config
+file. [All details on generating reports](https://docs.piperider.io/how-to-
+guides/generate-report) ## Generate comparison view You can use `piperider
+compare-report` to compare 2 reports. # Learn More | PipeRider Resources |
+Description | | -------------------- | ----------- | | [Documentation] |
+PipeRider Main Doc Site | | [Sample_Project] | Sample Project with with sqlite
+| | [dbt_Sample_Project] | Sample Project with dbt | | [Roadmap] | PipeRider
 Roadmap | | [Blog] | How we got started | [Documentation]: https://
 docs.piperider.io/ [Sample_Project]: https://github.com/InfuseAI/infuse-finance
 [dbt_Sample_Project]: https://github.com/InfuseAI/dbt-infuse-finance [Roadmap]:
 https://github.com/orgs/InfuseAI/projects/1/views/1 [Blog]: https://
 blog.infuseai.io/data-reliability-automated-with-piperider-7a823521ef11 # Get
-involved ## Support If you like what we are building, support us! Give us a :
-star: or get in touch. We'd love your feedback! Send us a message on
+involved ## Support :heart: If you like what we are building, support us! Give
+us a :star: or get in touch. We'd love your feedback! Send us a message on
 [piperider.io](https://piperider.io), join our [Discord](https://discord.com/
 invite/CrAxQznedH), or report an issue on [GitHub](https://github.com/InfuseAI/
 piperider/issues) ## Contributions We welcome contributions. See the [Set up
 dev environment](DEVELOP.md) and the [Contributing guildline](CONTRIBUTING.md)
 to get started.
```

### Comparing `piperider-0.9.0/piperider.egg-info/SOURCES.txt` & `piperider-0.9.0rc1/piperider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider.egg-info/requires.txt` & `piperider-0.9.0rc1/piperider.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/__init__.py` & `piperider-0.9.0rc1/piperider_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/adapter/dbt_adapter.py` & `piperider-0.9.0rc1/piperider_cli/adapter/dbt_adapter.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/assertion.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/assertion.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/recommended_rules/table_assertions.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/recommended_rules/table_assertions.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/recommender.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/recommender.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/types/__init__.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/types/__init__.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/types/assert_column_misc.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_column_misc.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/types/assert_column_ranges.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_column_ranges.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/types/assert_column_types.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_column_types.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/types/assert_rows.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/types/assert_rows.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_engine/types/base.py` & `piperider-0.9.0rc1/piperider_cli/assertion_engine/types/base.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/assertion_generator.py` & `piperider-0.9.0rc1/piperider_cli/assertion_generator.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/cli.py` & `piperider-0.9.0rc1/piperider_cli/cli.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/cloud/__init__.py` & `piperider-0.9.0rc1/piperider_cli/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/cloud_connector.py` & `piperider-0.9.0rc1/piperider_cli/cloud_connector.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/compare_report.py` & `piperider-0.9.0rc1/piperider_cli/compare_report.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/configuration.py` & `piperider-0.9.0rc1/piperider_cli/configuration.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/piperider-init-template/plugins/customized_assertions.py` & `piperider-0.9.0rc1/piperider_cli/data/piperider-init-template/plugins/customized_assertions.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/Discord/Discord-Logo.svg` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/Discord/Discord-Logo.svg`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/GitHub/GitHub-Logo.svg` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/GitHub/GitHub-Logo.svg`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/asset-manifest.json` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/index.html` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/index.html`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-144x144.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-192x192.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-36x36.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-48x48.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-72x72.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/android-icon-96x96.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-114x114.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-120x120.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-144x144.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-152x152.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-180x180.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-57x57.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-60x60.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-72x72.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-76x76.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon-precomposed.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/apple-icon.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/apple-icon.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon-16x16.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon-32x32.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon-96x96.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/favicon.ico` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/logo.svg` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/manifest.json` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/manifest.json`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-144x144.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-150x150.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-310x310.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/logo/ms-icon-70x70.png` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/logo/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css.map` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/css/main.fcbcb80f.css.map`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/183.b8accd6c.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/183.b8accd6c.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/276.fcb4db01.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/276.fcb4db01.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/357.5328e62e.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/357.5328e62e.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/787.20f148af.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/787.20f148af.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/836.945208d8.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/836.945208d8.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/903.4ec9ff75.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/903.4ec9ff75.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/906.9eefb2c7.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/906.9eefb2c7.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/914.035c9fb2.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/914.035c9fb2.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/982.4539617f.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/982.4539617f.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js.LICENSE.txt` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/js/main.3dd694e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Black.cadfd7434852779eb395.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Black.cadfd7434852779eb395.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.1577ca92013647c816b5.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.1577ca92013647c816b5.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.222064f2a764069868f4.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.222064f2a764069868f4.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.67a27362108220436ffb.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Regular.67a27362108220436ffb.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/comparison-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/comparison-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/Discord/Discord-Logo.svg` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/Discord/Discord-Logo.svg`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/GitHub/GitHub-Logo.svg` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/GitHub/GitHub-Logo.svg`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/asset-manifest.json` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/index.html` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/index.html`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-144x144.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-192x192.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-36x36.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-48x48.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-72x72.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/android-icon-96x96.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-114x114.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-120x120.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-144x144.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-152x152.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-180x180.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-57x57.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-60x60.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-72x72.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-76x76.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon-precomposed.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/apple-icon.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/apple-icon.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon-16x16.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon-32x32.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon-96x96.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/favicon.ico` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/logo.svg` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/manifest.json` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/manifest.json`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-144x144.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-150x150.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-310x310.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/logo/ms-icon-70x70.png` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/logo/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css.map` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/css/main.fcbcb80f.css.map`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/183.b8accd6c.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/183.b8accd6c.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/276.fcb4db01.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/276.fcb4db01.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/357.5328e62e.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/357.5328e62e.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/787.20f148af.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/787.20f148af.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/836.945208d8.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/836.945208d8.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/903.4ec9ff75.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/903.4ec9ff75.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/906.9eefb2c7.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/906.9eefb2c7.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/914.035c9fb2.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/914.035c9fb2.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/982.4539617f.chunk.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/982.4539617f.chunk.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/main.a918e51a.js` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/main.a918e51a.js`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/js/main.a918e51a.js.LICENSE.txt` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/js/main.a918e51a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Black.ab57b908749eb205e3ad.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Black.cadfd7434852779eb395.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Black.cadfd7434852779eb395.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.9bb4dd54e5afbea2e0ac.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BlackItalic.f0098e273d2a3758b89c.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Bold.1577ca92013647c816b5.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Bold.1577ca92013647c816b5.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Bold.f57c31edca48068386d7.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.52e97aac5945285c9933.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-BoldItalic.5b7f79817b551400186a.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.0321ea88d696270daf4b.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBold.a611efd96602ca47acd9.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.43f46f665391ff324c72.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraBoldItalic.dc0b36ae1c1bdac232e7.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.4e029f034c7e7263df9a.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLight.bafff4ae7f2a3395aa13.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.124644177779db0a8867.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ExtraLightItalic.ff3def84a34422de5487.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Italic.9736c3faff86c01270b2.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Italic.ce6bab8bc932d6080ec1.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Light.919d6ffdd987dc2e4717.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Light.aafd1643606ee83ad4cb.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.7f7cde8e1548e11231fb.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-LightItalic.e66e7a760a286c694d2b.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Medium.5a92f7b05463ecd61f45.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Medium.a6ca36dde32b3a1d0fd4.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.dbc1ed152c7b11f501a3.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-MediumItalic.e3618413f59e00041fb3.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Regular.222064f2a764069868f4.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Regular.222064f2a764069868f4.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Regular.67a27362108220436ffb.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Regular.67a27362108220436ffb.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.599ce7634f46c5024ad0.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBold.c2e7341dd6ac6502be69.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.09bc481607bd529abda7.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-SemiBoldItalic.43f7c276720845c6bb59.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Thin.92cada3d91581eb5112d.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-Thin.df0b1bcf558ccd5b48a2.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.78bf87d2ea41ac4365c1.woff`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-ThinItalic.82dd2dc2fb674d8273e4.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-italic.var.28904cc0eac675e1d19e.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter-roman.var.f05060926bf5023f9930.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/data/report/single-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2` & `piperider-0.9.0rc1/piperider_cli/data/report/single-report/static/media/Inter.var.c3f97a25f56b5b416e49.woff2`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/__init__.py` & `piperider-0.9.0rc1/piperider_cli/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/bigquery.py` & `piperider-0.9.0rc1/piperider_cli/datasource/bigquery.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/duckdb.py` & `piperider-0.9.0rc1/piperider_cli/datasource/duckdb.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/field.py` & `piperider-0.9.0rc1/piperider_cli/datasource/field.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/postgres.py` & `piperider-0.9.0rc1/piperider_cli/datasource/postgres.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/redshift.py` & `piperider-0.9.0rc1/piperider_cli/datasource/redshift.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/snowflake.py` & `piperider-0.9.0rc1/piperider_cli/datasource/snowflake.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/sqlite.py` & `piperider-0.9.0rc1/piperider_cli/datasource/sqlite.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/datasource/survey.py` & `piperider-0.9.0rc1/piperider_cli/datasource/survey.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/docgen/__main__.py` & `piperider-0.9.0rc1/piperider_cli/docgen/__main__.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/error.py` & `piperider-0.9.0rc1/piperider_cli/error.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/event/__init__.py` & `piperider-0.9.0rc1/piperider_cli/event/__init__.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/event/collector.py` & `piperider-0.9.0rc1/piperider_cli/event/collector.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/event/track.py` & `piperider-0.9.0rc1/piperider_cli/event/track.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/feedback.py` & `piperider-0.9.0rc1/piperider_cli/feedback.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/filesystem.py` & `piperider-0.9.0rc1/piperider_cli/filesystem.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/generate_report.py` & `piperider-0.9.0rc1/piperider_cli/generate_report.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/guide.py` & `piperider-0.9.0rc1/piperider_cli/guide.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/hack/datasource_inquirer_prompt.py` & `piperider-0.9.0rc1/piperider_cli/hack/datasource_inquirer_prompt.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/hack/inquirer.py` & `piperider-0.9.0rc1/piperider_cli/hack/inquirer.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/initializer.py` & `piperider-0.9.0rc1/piperider_cli/initializer.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/profiler/event.py` & `piperider-0.9.0rc1/piperider_cli/profiler/event.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/profiler/profiler.py` & `piperider-0.9.0rc1/piperider_cli/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/profiler/schema.json` & `piperider-0.9.0rc1/piperider_cli/profiler/schema.json`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/runner.py` & `piperider-0.9.0rc1/piperider_cli/runner.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/piperider_cli/validator.py` & `piperider-0.9.0rc1/piperider_cli/validator.py`

 * *Files identical despite different names*

### Comparing `piperider-0.9.0/setup.py` & `piperider-0.9.0rc1/setup.py`

 * *Files identical despite different names*

