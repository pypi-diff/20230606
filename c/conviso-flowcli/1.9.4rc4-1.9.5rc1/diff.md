# Comparing `tmp/conviso-flowcli-1.9.4rc4.tar.gz` & `tmp/conviso-flowcli-1.9.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conviso-flowcli-1.9.4rc4.tar", last modified: Wed Feb  9 16:15:32 2022, max compression
+gzip compressed data, was "dist/conviso-flowcli-1.9.5rc1.tar", last modified: Thu Nov 11 14:39:20 2021, max compression
```

## Comparing `conviso-flowcli-1.9.4rc4.tar` & `conviso-flowcli-1.9.5rc1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:32.002373 conviso-flowcli-1.9.4rc4/
--rw-r--r--   0 root         (0) root         (0)     4746 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4483 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4746 2022-02-09 16:15:31.000000 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3377 2022-02-09 16:15:31.000000 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-09 16:15:31.000000 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2022-02-09 16:15:31.000000 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      180 2022-02-09 16:15:31.000000 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-02-09 16:15:31.000000 conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/convisoappsec/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/convisoappsec/common/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4111 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/common/box.py
--rw-r--r--   0 root         (0) root         (0)    10235 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/common/docker.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/common/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/convisoappsec/flow/
--rw-r--r--   0 root         (0) root         (0)       81 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10635 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/
--rw-r--r--   0 root         (0) root         (0)      227 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1458 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/scc.py
--rw-r--r--   0 root         (0) root         (0)     4429 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/source_code_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/convisoappsec/flow/util/
--rw-r--r--   0 root         (0) root         (0)      160 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)      321 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/util/metrics.py
--rw-r--r--   0 root         (0) root         (0)      508 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/util/source_code_compressor.py
--rw-r--r--   0 root         (0) root         (0)     9512 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_control_system_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/
--rw-r--r--   0 root         (0) root         (0)      294 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2657 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     1266 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/timebased_version_seacher.py
--rw-r--r--   0 root         (0) root         (0)      943 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/version_searcher_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flow/versioning_style/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/versioning_style/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flow/versioning_style/semantic_versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/
--rw-r--r--   0 root         (0) root         (0)       64 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3242 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/common.py
--rw-r--r--   0 root         (0) root         (0)      583 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/
--rw-r--r--   0 root         (0) root         (0)       54 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/
--rw-r--r--   0 root         (0) root         (0)       54 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/context.py
--rw-r--r--   0 root         (0) root         (0)      677 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
--rw-r--r--   0 root         (0) root         (0)       64 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
--rw-r--r--   0 root         (0) root         (0)      675 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
--rw-r--r--   0 root         (0) root         (0)       56 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2607 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
--rw-r--r--   0 root         (0) root         (0)     3292 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     3235 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/values.py
--rw-r--r--   0 root         (0) root         (0)      353 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      715 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/ls.py
--rw-r--r--   0 root         (0) root         (0)      922 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/show.py
--rw-r--r--   0 root         (0) root         (0)     1608 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/
--rw-r--r--   0 root         (0) root         (0)       56 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/
--rw-r--r--   0 root         (0) root         (0)       54 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      268 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      308 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/with_/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2761 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/with_/version_tracker.py
--rw-r--r--   0 root         (0) root         (0)      266 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      331 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/help_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sast/
--rw-r--r--   0 root         (0) root         (0)       49 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     8963 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sast/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sca/
--rw-r--r--   0 root         (0) root         (0)       47 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sca/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     5969 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sca/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/vulnerability/
--rw-r--r--   0 root         (0) root         (0)       67 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/vulnerability/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1778 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/vulnerability/assert_security_rules.py
--rw-r--r--   0 root         (0) root         (0)      335 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/vulnerability/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/convisoappsec/sast/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/sast/decision.py
--rw-r--r--   0 root         (0) root         (0)     5958 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/sast/sastbox.py
--rw-r--r--   0 root         (0) root         (0)       27 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/convisoappsec/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.994373 conviso-flowcli-1.9.4rc4/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-09 16:15:31.998373 conviso-flowcli-1.9.4rc4/scripts/shell_completer/
--rw-r--r--   0 root         (0) root         (0)      624 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/scripts/shell_completer/flow_bash_completer.sh
--rw-r--r--   0 root         (0) root         (0)      147 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/scripts/shell_completer/flow_fish_completer.fish
--rw-r--r--   0 root         (0) root         (0)      844 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/scripts/shell_completer/flow_zsh_completer.sh
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-09 16:15:32.002373 conviso-flowcli-1.9.4rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1539 2022-02-09 16:15:28.000000 conviso-flowcli-1.9.4rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/
+-rw-r--r--   0 root         (0) root         (0)     5816 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/util/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/util/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/util/source_code_compressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4429 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/source_code_scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/scc.py
+-rw-rw-rw-   0 root         (0) root         (0)     9512 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_control_system_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/versioning_style/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/versioning_style/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/versioning_style/semantic_versioning.py
+-rw-rw-rw-   0 root         (0) root         (0)    10635 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/
+-rw-rw-rw-   0 root         (0) root         (0)      294 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
+-rw-rw-rw-   0 root         (0) root         (0)      943 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/version_searcher_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/timebased_version_seacher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/sast/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/sast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5958 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/sast/sastbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/sast/decision.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/common/
+-rw-rw-rw-   0 root         (0) root         (0)      230 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/common/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/common/box.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/common/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sast/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9003 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sast/run.py
+-rw-rw-rw-   0 root         (0) root         (0)      245 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sast/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sca/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sca/run.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sca/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/help_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/with_/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/with_/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/with_/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/with_/version_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/vulnerability/
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/vulnerability/assert_security_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/vulnerability/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/vulnerability/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/show.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
+-rw-rw-rw-   0 root         (0) root         (0)     2647 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/values.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/ls.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       99 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/convisoappsec/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/scripts/shell_completer/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/scripts/shell_completer/flow_fish_completer.fish
+-rw-rw-rw-   0 root         (0) root         (0)      624 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/scripts/shell_completer/flow_bash_completer.sh
+-rw-rw-rw-   0 root         (0) root         (0)      844 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/scripts/shell_completer/flow_zsh_completer.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4483 2021-11-11 14:39:14.000000 conviso-flowcli-1.9.5rc1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-11-11 14:39:20.000000 conviso-flowcli-1.9.5rc1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5816 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3377 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2021-11-11 14:39:19.000000 conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/requires.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `conviso-flowcli-1.9.4rc4/PKG-INFO` & `conviso-flowcli-1.9.5rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: conviso-flowcli
-Version: 1.9.4rc4
-Summary: UNKNOWN
-Maintainer: Jean Carlos Sales Pantoja
-Maintainer-email: jpantoja@convisoappsec.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
 # Flowcli
 
 This is a command line tool to interact with [convisoappsec] flow api. This aims to be very useful for integrations development.
 
 # Installation
 To install flowcli some dependecies are required:
 * python3 >= 3.4. See [python3 download]
@@ -135,9 +124,8 @@
 [generating project code]: <https://appsecflow.helpy.io/>
 [appsec flow]: <https://appsecflow.helpy.io/>
 [CI/CD]: <https://en.wikipedia.org/wiki/CI/CD>
 [SAST]: <https://blog.convisoappsec.com/en/code-review-and-sast-whats-the-difference/>
 [DAST]: <https://blog.convisoappsec.com/en/code-review-and-sast-whats-the-difference/>
 [creating project]: <https://appsecflow.helpy.io/>
 [appsec flow account]: <https://appsecflow.helpy.io/>
-[Flow AppSec]: <https://app.conviso.com.br/>
-
+[Flow AppSec]: <https://app.conviso.com.br/>
```

### Comparing `conviso-flowcli-1.9.4rc4/README.md` & `conviso-flowcli-1.9.5rc1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,142 @@
-# Flowcli
-
-This is a command line tool to interact with [convisoappsec] flow api. This aims to be very useful for integrations development.
-
-# Installation
-To install flowcli some dependecies are required:
-* python3 >= 3.4. See [python3 download]
-* pip. See [pip guide]
-* git. See [git download]
-* Docker. See [docker download]
-
-If you have system admin privileges just execute one of the following commands.
-```sh
-$ pip install conviso-flowcli
-```
-or
-```sh
-$ python3 -m pip install conviso-flowcli
-```
-If you haven't system admin privileges execute one of the following commands.
-```sh
-$ pip install --user conviso-flowcli
-```
-or
-```sh
-$ python3 -m pip install --user conviso-flowcli
-```
-Check if the install command was well succeeded.
-```sh
-$ flow --version
-```
-The command will print the current version and exit with success. Now we are ready to proceed.
-
-# Getting started
-## Overview
-The primary goal of the flowcli aims to be a developer friendly tool. The tool will automate as many steps as possible to decrease spent time on an integration with [appsec flow]. Using this tool the integration with your [CI/CD] platform will be easy. At your [CI/CD] you be able to perform [SAST] and [DAST] analysis, send source code to be reviewed by our analysts and order features availables in your [appsec flow account].
-
-# Shell Completion
-This section will guide you to activate the flow shell completion. This is not required to use the tool so you can skip it if you want. 
-
-## Bash
-Open your .bashrc file at ~/.bashrc and place the following snippet in the end of file.
-```sh
-FLOW_COMPLETER="$(which flow_bash_completer.sh)"
-
-[ -f "$FLOW_COMPLETER" ] && {
-  source "$FLOW_COMPLETER"
-}
-```
-Start a new bash shell session and the shell completion will be available.
-
-## Zsh
-Open your .zshrc file at ~/.zshrc and place the following snippet in the end of file.
-```sh
-FLOW_COMPLETER="$(which flow_zsh_completer.sh)"
-
-[ -f "$FLOW_COMPLETER" ] && {
-  source "$FLOW_COMPLETER"
-}
-```
-Start a new zsh shell session and the shell completion will be available.
-
-## Fish
-Start a fish shell session and execute the following command.
-```sh
-$ mkdir -p ~/.config/fish/completions
-$ cp (which flow_fish_completer.fish) ~/.config/fish/completions/flow.fish
-```
-Start a new fish shell session and the shell completion will be available.
-
-## Main command
-The main command of flowcli is flow. To see the command help run the following command.
-```sh
-$ flow -h
-```
-or
-```sh
-$ flow --help
-```
-## Authentication
-To start with flowcli an [appsec flow] api key(See [generating api key]) will be necessary. After you got it you can export the key as system environment variable
-and use the flowcli.
-
-```sh
-$ export FLOW_API_KEY='you-api-key'
-```
-or the api key can be set as option argument
-```sh
-$ flow --api-key 'you-api-key' [SOME COMMAND]
-```
-
-## Static program analysis(SAST)
-With the flowcli is very simple to perform a SAST at your source code repository. Let's see some examples.
-
-### Reporting the SAST results to [Flow AppSec] API
-
-To report the SAST result to flow api a project code will be required. The project is created at [Flow AppSec] Web View. See [creating project].
-
-Assuming that my_source_code_repository is a git repository, so:
-
-```sh
-$ export FLOW_API_KEY='your-api-key'
-$ export FLOW_PROJECT_CODE='your-project-code'
-$ cd my_source_code_repository
-$ flow sast run
-```
-
-The following instructions has the same effect.
-
-```sh
-$ cd my_source_code_repository
-$ flow --api-key 'your-api-key' sast run --project-code 'your-project-code'
-```
-
-[python3 download]: <https://www.python.org/downloads/>
-[git download]: <https://git-scm.com/downloads>
-[pip guide]: <https://packaging.python.org/tutorials/installing-packages/#installing-from-pypi>
-[docker download]: <https://docs.docker.com/engine/install/>
-[bash]: <https://www.gnu.org/software/bash/>
-[zsh]: <https://www.zsh.org/>
-[fish]: <https://fishshell.com/>
-[convisoappsec]: <https://convisoappsec.com/>
-[generating api key]: <https://appsecflow.helpy.io/>
-[generating project code]: <https://appsecflow.helpy.io/>
-[appsec flow]: <https://appsecflow.helpy.io/>
-[CI/CD]: <https://en.wikipedia.org/wiki/CI/CD>
-[SAST]: <https://blog.convisoappsec.com/en/code-review-and-sast-whats-the-difference/>
-[DAST]: <https://blog.convisoappsec.com/en/code-review-and-sast-whats-the-difference/>
-[creating project]: <https://appsecflow.helpy.io/>
-[appsec flow account]: <https://appsecflow.helpy.io/>
-[Flow AppSec]: <https://app.conviso.com.br/>
+Metadata-Version: 2.1
+Name: conviso-flowcli
+Version: 1.9.5rc1
+Summary: UNKNOWN
+Home-page: UNKNOWN
+Maintainer: Jean Carlos Sales Pantoja
+Maintainer-email: jpantoja@convisoappsec.com
+License: UNKNOWN
+Description: # Flowcli
+        
+        This is a command line tool to interact with [convisoappsec] flow api. This aims to be very useful for integrations development.
+        
+        # Installation
+        To install flowcli some dependecies are required:
+        * python3 >= 3.4. See [python3 download]
+        * pip. See [pip guide]
+        * git. See [git download]
+        * Docker. See [docker download]
+        
+        If you have system admin privileges just execute one of the following commands.
+        ```sh
+        $ pip install conviso-flowcli
+        ```
+        or
+        ```sh
+        $ python3 -m pip install conviso-flowcli
+        ```
+        If you haven't system admin privileges execute one of the following commands.
+        ```sh
+        $ pip install --user conviso-flowcli
+        ```
+        or
+        ```sh
+        $ python3 -m pip install --user conviso-flowcli
+        ```
+        Check if the install command was well succeeded.
+        ```sh
+        $ flow --version
+        ```
+        The command will print the current version and exit with success. Now we are ready to proceed.
+        
+        # Getting started
+        ## Overview
+        The primary goal of the flowcli aims to be a developer friendly tool. The tool will automate as many steps as possible to decrease spent time on an integration with [appsec flow]. Using this tool the integration with your [CI/CD] platform will be easy. At your [CI/CD] you be able to perform [SAST] and [DAST] analysis, send source code to be reviewed by our analysts and order features availables in your [appsec flow account].
+        
+        # Shell Completion
+        This section will guide you to activate the flow shell completion. This is not required to use the tool so you can skip it if you want. 
+        
+        ## Bash
+        Open your .bashrc file at ~/.bashrc and place the following snippet in the end of file.
+        ```sh
+        FLOW_COMPLETER="$(which flow_bash_completer.sh)"
+        
+        [ -f "$FLOW_COMPLETER" ] && {
+          source "$FLOW_COMPLETER"
+        }
+        ```
+        Start a new bash shell session and the shell completion will be available.
+        
+        ## Zsh
+        Open your .zshrc file at ~/.zshrc and place the following snippet in the end of file.
+        ```sh
+        FLOW_COMPLETER="$(which flow_zsh_completer.sh)"
+        
+        [ -f "$FLOW_COMPLETER" ] && {
+          source "$FLOW_COMPLETER"
+        }
+        ```
+        Start a new zsh shell session and the shell completion will be available.
+        
+        ## Fish
+        Start a fish shell session and execute the following command.
+        ```sh
+        $ mkdir -p ~/.config/fish/completions
+        $ cp (which flow_fish_completer.fish) ~/.config/fish/completions/flow.fish
+        ```
+        Start a new fish shell session and the shell completion will be available.
+        
+        ## Main command
+        The main command of flowcli is flow. To see the command help run the following command.
+        ```sh
+        $ flow -h
+        ```
+        or
+        ```sh
+        $ flow --help
+        ```
+        ## Authentication
+        To start with flowcli an [appsec flow] api key(See [generating api key]) will be necessary. After you got it you can export the key as system environment variable
+        and use the flowcli.
+        
+        ```sh
+        $ export FLOW_API_KEY='you-api-key'
+        ```
+        or the api key can be set as option argument
+        ```sh
+        $ flow --api-key 'you-api-key' [SOME COMMAND]
+        ```
+        
+        ## Static program analysis(SAST)
+        With the flowcli is very simple to perform a SAST at your source code repository. Let's see some examples.
+        
+        ### Reporting the SAST results to [Flow AppSec] API
+        
+        To report the SAST result to flow api a project code will be required. The project is created at [Flow AppSec] Web View. See [creating project].
+        
+        Assuming that my_source_code_repository is a git repository, so:
+        
+        ```sh
+        $ export FLOW_API_KEY='your-api-key'
+        $ export FLOW_PROJECT_CODE='your-project-code'
+        $ cd my_source_code_repository
+        $ flow sast run
+        ```
+        
+        The following instructions has the same effect.
+        
+        ```sh
+        $ cd my_source_code_repository
+        $ flow --api-key 'your-api-key' sast run --project-code 'your-project-code'
+        ```
+        
+        [python3 download]: <https://www.python.org/downloads/>
+        [git download]: <https://git-scm.com/downloads>
+        [pip guide]: <https://packaging.python.org/tutorials/installing-packages/#installing-from-pypi>
+        [docker download]: <https://docs.docker.com/engine/install/>
+        [bash]: <https://www.gnu.org/software/bash/>
+        [zsh]: <https://www.zsh.org/>
+        [fish]: <https://fishshell.com/>
+        [convisoappsec]: <https://convisoappsec.com/>
+        [generating api key]: <https://appsecflow.helpy.io/>
+        [generating project code]: <https://appsecflow.helpy.io/>
+        [appsec flow]: <https://appsecflow.helpy.io/>
+        [CI/CD]: <https://en.wikipedia.org/wiki/CI/CD>
+        [SAST]: <https://blog.convisoappsec.com/en/code-review-and-sast-whats-the-difference/>
+        [DAST]: <https://blog.convisoappsec.com/en/code-review-and-sast-whats-the-difference/>
+        [creating project]: <https://appsecflow.helpy.io/>
+        [appsec flow account]: <https://appsecflow.helpy.io/>
+        [Flow AppSec]: <https://app.conviso.com.br/>
+Platform: UNKNOWN
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
```

### Comparing `conviso-flowcli-1.9.4rc4/conviso_flowcli.egg-info/SOURCES.txt` & `conviso-flowcli-1.9.5rc1/conviso_flowcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/common/box.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/common/box.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/common/docker.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/common/docker.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/api.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/api.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/scc.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/scc.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/source_code_scanner/source_code_scanner.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/source_code_scanner/source_code_scanner.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_control_system_adapter.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_control_system_adapter.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/timebased_version_seacher.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/timebased_version_seacher.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/version_searchers/version_searcher_result.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/version_searchers/version_searcher_result.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flow/versioning_style/semantic_versioning.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flow/versioning_style/semantic_versioning.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/common.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 from pipes import quote
 import io
-
+import sys
+import requests
 
 class DeployFormatter(object):
     DEFAULT = 'default'
     ENV_VARS = 'env_vars'
 
     def __init__(self, format):
         self.stategy = self._select_strategy(format)
@@ -115,7 +116,21 @@
     if project_code_param not in args:
         paramsdecl = args + (project_code_param, )
 
     return click.option(
         *paramsdecl,
         **kargs,
     )
+
+def on_http_error(error):
+    try:
+        raise error
+    except requests.exceptions.HTTPError as e:
+        message = error.response.text
+
+        if not message:
+            return
+
+        click.echo(
+            "HttpErrorResponse: {0}".format(message),
+            file=sys.stderr
+        )
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/context.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/context.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/entrypoint.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 # TODO: refactoring. all deploy create share some behavior
 from convisoappsec.flow.util import project_metrics
 from convisoappsec.flow.version_searchers import TimeBasedVersionSearcher
 from convisoappsec.flow.version_control_system_adapter import GitAdapter
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flowcli import help_option
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 from convisoappsec.flowcli.deploy.create.context import pass_create_context
 from convisoappsec.flowcli.deploy.create.with_.tag_tracker.context import (
     pass_tag_tracker_context
 )
 
 
 @click.command('time')
@@ -76,8 +76,9 @@
             project_metrics=project_metrics(repository_dir)
         )
 
         click.echo(
             create_context.output_formatter.format(deploy)
         )
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 # TODO: refactoring. all deploy create share some behavior
 from convisoappsec.flow.util import project_metrics
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flow.version_searchers import SortedByVersioningStyle
 from convisoappsec.flow.version_control_system_adapter import GitAdapter
 from convisoappsec.flowcli import help_option
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 from convisoappsec.flowcli.deploy.create.context import pass_create_context
 
 from convisoappsec.flowcli.deploy.create.with_.tag_tracker.context import (
     pass_tag_tracker_context
 )
 
 
@@ -104,8 +104,9 @@
             project_metrics=project_metrics(repository_dir)
         )
 
         click.echo(
             create_context.output_formatter.format(deploy)
         )
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/create/with_/values.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/create/with_/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # TODO: refactoring. all deploy create share some behavior
 from convisoappsec.flow.util import project_metrics
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.deploy.create.context import pass_create_context
 from convisoappsec.flow import GitAdapter
 from convisoappsec.flow import api
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 
 
 @click.command()
 @help_option
 @project_code_option()
 @click.option(
     "-c",
@@ -99,8 +99,9 @@
             project_metrics=project_metrics(repository_dir)
         )
 
         click.echo(
             create_context.output_formatter.format(deploy)
         )
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/ls.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/ls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import json
 
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flowcli import help_option
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 
 
 @click.command()
 @project_code_option()
 @click.option(
     '-c',
     '--current-tag',
@@ -19,8 +19,9 @@
 def ls(flow_context, project_code, current_tag):
     try:
         flow = flow_context.create_flow_api_client()
         deploys = flow.deploys.list(project_code, current_tag)
         deploys_json = json.dumps(deploys, indent=2)
         click.echo(deploys_json)
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/deploy/show.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/deploy/show.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.common import DeployFormatter
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 
 
 @click.command()
 @help_option
 @project_code_option()
 @click.argument('current-tag', required=True)
 @click.option(
@@ -24,8 +24,9 @@
         flow = flow_context.create_flow_api_client()
         deploy = flow.deploys.get(project_code, current_tag)
         formatter = DeployFormatter(output_format)
         click.echo(
             formatter.format(deploy)
         )
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/entrypoint.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/finding/create/with_/version_tracker.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/finding/create/with_/version_tracker.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sast/run.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sast/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import click
 import sys
 
+
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.sast.sastbox import SASTBox
 from convisoappsec.flow import GitAdapter
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 from convisoappsec.sast.decision import Decision
 from convisoappsec.sast.decision import Severity
 
 def log_func(msg, new_line=True, clear=False):
     click.echo(msg, nl=new_line, err=True)
 
 
@@ -260,16 +261,16 @@
                 for issue in issues:
                     click.echo('{issue_name}\n{filepath} at line {line_index}\n'.format(
                         issue_name=issue['title'],
                         filepath=issue['filename'],
                         line_index=issue['line']
                     ))
             sys.exit(1)
-
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
 
 
 EPILOG = '''
 Examples:
 
   \b
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/sca/run.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/sca/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 import click_log
 import logging
 
 from convisoappsec.flowcli import help_option
 from convisoappsec.flowcli.context import pass_flow_context
 from convisoappsec.flow import GitAdapter
-from convisoappsec.flowcli.common import project_code_option
+from convisoappsec.flowcli.common import project_code_option, on_http_error
 from convisoappsec.common.box import Box
 
 logger = logging.getLogger(__name__)
 click_log.basic_config(logger)
 
 @click.command()
 @click_log.simple_verbosity_option(logger)
@@ -174,14 +174,15 @@
                         unit.name
                     ))
             
         # TODO add CI Decision block code
         click.secho('\U00002705 SCA Scan Finished', bold=True)
         
     except Exception as e:
+        on_http_error(e)
         raise click.ClickException(str(e)) from e
 
 
 EPILOG = '''
 Examples:
 
   \b
```

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/flowcli/vulnerability/assert_security_rules.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/flowcli/vulnerability/assert_security_rules.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/sast/decision.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/sast/decision.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/convisoappsec/sast/sastbox.py` & `conviso-flowcli-1.9.5rc1/convisoappsec/sast/sastbox.py`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/scripts/shell_completer/flow_bash_completer.sh` & `conviso-flowcli-1.9.5rc1/scripts/shell_completer/flow_bash_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/scripts/shell_completer/flow_zsh_completer.sh` & `conviso-flowcli-1.9.5rc1/scripts/shell_completer/flow_zsh_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-flowcli-1.9.4rc4/setup.py` & `conviso-flowcli-1.9.5rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,9 +48,9 @@
         flow=convisoappsec.flowcli.entrypoint:cli
     ''',
     scripts=[
         path.join(SCRIPTS_SHELL_COMPLETER_DIR, 'flow_bash_completer.sh'),
         path.join(SCRIPTS_SHELL_COMPLETER_DIR, 'flow_zsh_completer.sh'),
         path.join(SCRIPTS_SHELL_COMPLETER_DIR, 'flow_fish_completer.fish'),
     ],
-    python_requires='>=3.5',
+    python_requires='>=3.4',
 )
```

