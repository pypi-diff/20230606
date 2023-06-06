# Comparing `tmp/font-CLI-0.9.8.tar.gz` & `tmp/font-CLI-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "font-CLI-0.9.8.tar", last modified: Mon Apr 17 05:18:12 2023, max compression
+gzip compressed data, was "font-CLI-0.9.9.tar", last modified: Wed Apr 19 16:40:43 2023, max compression
```

## Comparing `font-CLI-0.9.8.tar` & `font-CLI-0.9.9.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 05:17:58.000000 font-CLI-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-17 05:18:12.533495 font-CLI-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    86796 2023-04-17 05:17:58.000000 font-CLI-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/font_CLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 05:18:12.000000 font-CLI-0.9.8/font_CLI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/
--rw-r--r--   0 runner    (1001) docker     (123)    28606 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/Font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/VFont.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/assistant/fonts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/assistant/styles_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/otf_to_ttf.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/sfnt_to_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/ttf_to_otf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/variable_to_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/converters/web_to_sfnt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.529495 font-CLI-0.9.8/ftCLI/Lib/cui/
--rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/cui/CUI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/cui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/ftCLI/Lib/tables/
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/OS_2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/head.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/tables/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/ftCLI/Lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/click_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/glyphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/Lib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:18:12.533495 font-CLI-0.9.8/ftCLI/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_cff.py
--rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_os2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_print.py
--rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/commands/ftcli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-17 05:17:58.000000 font-CLI-0.9.8/ftCLI/ftCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:18:12.533495 font-CLI-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-17 05:17:58.000000 font-CLI-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.758474 font-CLI-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 16:40:32.000000 font-CLI-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-19 16:40:43.758474 font-CLI-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    86796 2023-04-19 16:40:32.000000 font-CLI-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.746474 font-CLI-0.9.9/font_CLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 16:40:43.000000 font-CLI-0.9.9/font_CLI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.746474 font-CLI-0.9.9/ftCLI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.750474 font-CLI-0.9.9/ftCLI/Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    28606 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/Font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/VFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.750474 font-CLI-0.9.9/ftCLI/Lib/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/assistant/fonts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/assistant/styles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.750474 font-CLI-0.9.9/ftCLI/Lib/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/converters/otf_to_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/converters/sfnt_to_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/converters/ttf_to_otf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/converters/variable_to_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/converters/web_to_sfnt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.750474 font-CLI-0.9.9/ftCLI/Lib/cui/
+-rw-r--r--   0 runner    (1001) docker     (123)    30721 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/cui/CUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/cui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.754474 font-CLI-0.9.9/ftCLI/Lib/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/tables/OS_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/tables/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/tables/hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/tables/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/tables/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.754474 font-CLI-0.9.9/ftCLI/Lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/utils/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/utils/click_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/utils/glyphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/Lib/utils/subsetter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:43.758474 font-CLI-0.9.9/ftCLI/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17345 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_cff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_os2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22992 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/commands/ftcli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 16:40:32.000000 font-CLI-0.9.9/ftCLI/ftCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:40:43.758474 font-CLI-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-19 16:40:32.000000 font-CLI-0.9.9/setup.py
```

### Comparing `font-CLI-0.9.8/LICENSE` & `font-CLI-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/PKG-INFO` & `font-CLI-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-CLI
-Version: 0.9.8
+Version: 0.9.9
 Summary: A set of command line tools to edit fonts with FontTools
 Home-page: https://github.com/ftCLI/ftCLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.11
```

### Comparing `font-CLI-0.9.8/README.md` & `font-CLI-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/font_CLI.egg-info/PKG-INFO` & `font-CLI-0.9.9/font_CLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: font-CLI
-Version: 0.9.8
+Version: 0.9.9
 Summary: A set of command line tools to edit fonts with FontTools
 Home-page: https://github.com/ftCLI/ftCLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.11
```

### Comparing `font-CLI-0.9.8/font_CLI.egg-info/SOURCES.txt` & `font-CLI-0.9.9/font_CLI.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 ftCLI/Lib/tables/name.py
 ftCLI/Lib/tables/post.py
 ftCLI/Lib/utils/__init__.py
 ftCLI/Lib/utils/cli_tools.py
 ftCLI/Lib/utils/click_tools.py
 ftCLI/Lib/utils/glyphs.py
 ftCLI/Lib/utils/misc.py
+ftCLI/Lib/utils/subsetter.py
 ftCLI/commands/__init__.py
 ftCLI/commands/ftcli_assistant.py
 ftCLI/commands/ftcli_cff.py
 ftCLI/commands/ftcli_converter.py
 ftCLI/commands/ftcli_fix.py
 ftCLI/commands/ftcli_hhea.py
 ftCLI/commands/ftcli_metrics.py
```

### Comparing `font-CLI-0.9.8/ftCLI/Lib/Font.py` & `font-CLI-0.9.9/ftCLI/Lib/Font.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/VFont.py` & `font-CLI-0.9.9/ftCLI/Lib/VFont.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/assistant/fonts_data.py` & `font-CLI-0.9.9/ftCLI/Lib/assistant/fonts_data.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/assistant/styles_mapping.py` & `font-CLI-0.9.9/ftCLI/Lib/assistant/styles_mapping.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/constants.py` & `font-CLI-0.9.9/ftCLI/Lib/constants.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/converters/otf_to_ttf.py` & `font-CLI-0.9.9/ftCLI/Lib/converters/otf_to_ttf.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/converters/ttf_to_otf.py` & `font-CLI-0.9.9/ftCLI/Lib/converters/ttf_to_otf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cffsubr
 import pathops
 from fontTools.fontBuilder import FontBuilder
 from fontTools.pens.qu2cuPen import Qu2CuPen
 from fontTools.pens.t2CharStringPen import T2CharStringPen
-from fontTools.subset import Subsetter
+from ftCLI.Lib.utils.subsetter import BaseSubsetter
 
 from ftCLI.Lib.Font import Font
 from ftCLI.Lib.utils.click_tools import generic_error_message, generic_warning_message
 
 
 class Options(object):
     def __init__(self):
@@ -110,32 +110,24 @@
             minMemType1=self.font["post"].minMemType1,
             maxMemType1=self.font["post"].maxMemType1,
         )
         return post_info
 
     def purge_glyphs(self):
         glyph_ids_to_remove = []
-        for g in [".null", "NULL", "uni0000", "CR", "nonmarkingreturn", "uni000D"]:
+        for g in [".null", "NUL", "NULL", "uni0000", "CR", "nonmarkingreturn", "uni000D"]:
             try:
                 glyph_ids_to_remove.append(self.font.getGlyphID(g))
             except KeyError:
                 pass
 
         glyph_ids = [i for i in self.font.getReverseGlyphMap().values() if i not in glyph_ids_to_remove]
         if len(glyph_ids_to_remove) > 0:
-            subsetter = Subsetter()
-            subsetter.options.drop_tables = []
-            subsetter.options.passthrough_tables = True
-            subsetter.options.name_IDs = "*"
-            subsetter.options.name_legacy = True
-            subsetter.options.name_languages = "*"
-            subsetter.options.layout_features = "*"
-            subsetter.options.hinting = False
-            subsetter.glyph_ids_requested = glyph_ids
-            Subsetter.subset(subsetter, self.font)
+            subsetter = BaseSubsetter(glyph_ids=glyph_ids)
+            subsetter.subset(self.font)
 
     def get_qu2cu_charstrings(self, tolerance: float = 1, all_cubic: bool = True):
         charstrings = {}
         glyph_set = self.font.getGlyphSet()
 
         for k, v in glyph_set.items():
             # Correct contours direction and remove overlaps with pathops
```

### Comparing `font-CLI-0.9.8/ftCLI/Lib/converters/variable_to_static.py` & `font-CLI-0.9.9/ftCLI/Lib/converters/variable_to_static.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     file_saved_message,
     generic_error_message,
 )
 
 
 class Options(object):
     def __init__(self):
-        self.cleanup = (True,)
-        self.update_name_table = (True,)
+        self.cleanup = True
+        self.update_name_table = True
         self.output_dir = None
         self.overwrite = True
 
 
 class VariableToStatic(object):
     def __init__(self):
         self.options = Options()
@@ -56,14 +56,17 @@
                 axisLimits=instance.coordinates,
                 inplace=False,
                 overlap=OverlapMode.REMOVE_AND_IGNORE_ERRORS,
                 optimize=True,
                 updateFontNames=self.options.update_name_table,
             )
 
+            if "cvar" in static_instance:
+                del static_instance["cvar"]
+
             if self.options.cleanup:
                 name_ids_to_delete = variable_font.get_var_name_ids_to_delete() if self.options.cleanup else []
                 static_instance.name_table.del_names(name_ids=name_ids_to_delete)
 
                 if "STAT" in static_instance:
                     del static_instance["STAT"]
```

### Comparing `font-CLI-0.9.8/ftCLI/Lib/cui/CUI.py` & `font-CLI-0.9.9/ftCLI/Lib/cui/CUI.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/tables/OS_2.py` & `font-CLI-0.9.9/ftCLI/Lib/tables/OS_2.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/tables/head.py` & `font-CLI-0.9.9/ftCLI/Lib/tables/head.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/tables/hhea.py` & `font-CLI-0.9.9/ftCLI/Lib/tables/hhea.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/tables/name.py` & `font-CLI-0.9.9/ftCLI/Lib/tables/name.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/utils/cli_tools.py` & `font-CLI-0.9.9/ftCLI/Lib/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/utils/click_tools.py` & `font-CLI-0.9.9/ftCLI/Lib/utils/click_tools.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/Lib/utils/glyphs.py` & `font-CLI-0.9.9/ftCLI/Lib/utils/glyphs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from fontTools.misc.psCharStrings import T2CharString
 
 
 def get_glyph_bounds(glyph_set, glyph_name: str) -> dict:
     if glyph_set.get(glyph_name) is None:
         return dict(xMin=0, yMin=0, xMax=0, yMax=0)
     bounds = T2CharString.calcBounds(glyph_set[glyph_name], glyph_set)
-    if bounds is not None:
+    if bounds:
         return dict(xMin=bounds[0], yMin=bounds[1], xMax=bounds[2], yMax=bounds[3])
     else:
         return dict(xMin=0, yMin=0, xMax=0, yMax=0)
 
 
 def get_glyphs_bounds_all(glyph_set) -> dict:
     metrics = {}
     for glyph_name in glyph_set.keys():
         bounds = T2CharString.calcBounds(glyph_set[glyph_name], glyph_set)
-        if bounds is not None:
+        if bounds:
             metrics[glyph_name] = dict(xMin=bounds[0], yMin=bounds[1], xMax=bounds[2], yMax=bounds[3])
         else:
             metrics[glyph_name] = None
 
     return metrics
```

### Comparing `font-CLI-0.9.8/ftCLI/Lib/utils/misc.py` & `font-CLI-0.9.9/ftCLI/Lib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_assistant.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_assistant.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_cff.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_cff.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_converter.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,23 +67,23 @@
     is_flag=True,
     help="""
               Performs optional outline quality checks and removes overlaps with afdko.checkoutlinesufo
               """,
 )
 @add_common_options()
 def ttf2otf(
-        input_path,
-        tolerance=1,
-        safe=False,
-        purge_glyphs=False,
-        subroutinize=True,
-        check_outlines=False,
-        outputDir=None,
-        recalcTimestamp=False,
-        overWrite=True,
+    input_path,
+    tolerance=1,
+    safe=False,
+    purge_glyphs=False,
+    subroutinize=True,
+    check_outlines=False,
+    outputDir=None,
+    recalcTimestamp=False,
+    overWrite=True,
 ):
     """
     Converts TTF fonts (or TrueType flavored woff/woff2 web fonts) to OTF fonts (or CFF flavored woff/woff2 web fonts).
     """
 
     from ftCLI.Lib.converters.ttf_to_otf import TrueTypeToCFF
 
@@ -112,14 +112,15 @@
             output_file = makeOutputFileName(
                 file, suffix=suffix, extension=ext, outputDir=output_dir, overWrite=overWrite
             )
 
             if safe:
                 # Create a temporary OTF file with T2CharStringPen...
                 from ftCLI.Lib.converters.otf_to_ttf import CFFToTrueType
+
                 ttf2otf_converter_temp = TrueTypeToCFF(source_font)
                 ttf2otf_converter_temp.options.charstring_source = "t2"
                 ttf2otf_converter_temp.options.subroutinize = False
                 ttf2otf_converter_temp.options.purge_glyphs = purge_glyphs
                 temp_cff_font = ttf2otf_converter_temp.run()
 
                 # ... and convert it back to a temporary TTF file that will be used for conversion
@@ -137,14 +138,15 @@
             ttf2otf_converter.options.subroutinize = subroutinize
             ttf2otf_converter.options.purge_glyphs = purge_glyphs
             cff_font = ttf2otf_converter.run()
             cff_font.save(output_file)
 
             if check_outlines:
                 from afdko import checkoutlinesufo
+
                 generic_info_message("Checking outlines...")
                 checkoutlinesufo.run(args=[output_file, "--error-correction-mode", "--quiet-mode"])
 
             converted_files_counter += 1
             generic_info_message(f"Done in {round(time.time() - t, 3)} seconds")
             file_saved_message(output_file)
 
@@ -161,18 +163,15 @@
 def otf_2_ttf():
     pass
 
 
 @otf_2_ttf.command()
 @add_file_or_path_argument()
 @click.option(
-    "--max-err",
-    type=click.FloatRange(0.0, 3.0),
-    default=1.0,
-    help="""Approximation error, measured in UPEM"""
+    "--max-err", type=click.FloatRange(0.0, 3.0), default=1.0, help="""Approximation error, measured in UPEM"""
 )
 @add_common_options()
 def otf2ttf(input_path, max_err, outputDir=None, recalcTimestamp=False, overWrite=True):
     """
     Converts fonts from OTF to TTF format.
     """
     from ftCLI.Lib.converters.otf_to_ttf import CFFToTrueType
@@ -232,20 +231,20 @@
     is_flag=True,
     help="""
               Deletes the source files after conversion.
               """,
 )
 @add_common_options()
 def wf2ft(
-        input_path,
-        flavor=None,
-        delete_source_file=False,
-        outputDir=None,
-        recalcTimestamp=False,
-        overWrite=True,
+    input_path,
+    flavor=None,
+    delete_source_file=False,
+    outputDir=None,
+    recalcTimestamp=False,
+    overWrite=True,
 ):
     """
     Converts web fonts (WOFF and WOFF2) to SFNT fonts (TTF or OTF)
     """
     from ftCLI.Lib.converters.web_to_sfnt import WebToSFNT
 
     if not flavor:
@@ -262,19 +261,15 @@
             suffix = web_font.get_real_extension()
 
             converter = WebToSFNT(font=web_font)
             desktop_font = converter.run()
 
             new_extension = desktop_font.get_real_extension()
             output_file = makeOutputFileName(
-                file,
-                extension=new_extension,
-                suffix=suffix,
-                outputDir=output_dir,
-                overWrite=overWrite
+                file, extension=new_extension, suffix=suffix, outputDir=output_dir, overWrite=overWrite
             )
             desktop_font.save(output_file, reorderTables=False)
             if delete_source_file:
                 os.remove(file)
             file_saved_message(output_file)
         except Exception as e:
             generic_error_message(e)
@@ -309,22 +304,25 @@
     output_flavors = ["woff", "woff2"]
     if flavor is not None:
         output_flavors = [flavor]
 
     for file in files:
         try:
             font = Font(file, recalcTimestamp=recalcTimestamp)
+            suffix = font.get_real_extension()
             if font.flavor is not None:
                 continue
             for flavor in output_flavors:
                 font.flavor = flavor
                 converter = SFNTToWeb(font=font, flavor=flavor)
                 web_font = converter.run()
                 extension = web_font.get_real_extension()
-                output_file = makeOutputFileName(file, extension=extension, outputDir=output_dir, overWrite=overWrite)
+                output_file = makeOutputFileName(
+                    file, suffix=suffix, extension=extension, outputDir=output_dir, overWrite=overWrite
+                )
                 web_font.save(output_file, reorderTables=False)
                 file_saved_message(output_file)
         except Exception as e:
             generic_error_message(e)
 
 
 @click.group()
@@ -415,21 +413,21 @@
     default=False,
     help="""
               Update the instantiated font's `name` table. Input font must have a STAT table with Axis Value Tables
               """,
 )
 @add_common_options()
 def var2static(
-        input_path,
-        select_instance=False,
-        cleanup=True,
-        update_name_table=False,
-        outputDir=None,
-        recalcTimestamp=False,
-        overWrite=True,
+    input_path,
+    select_instance=False,
+    cleanup=True,
+    update_name_table=False,
+    outputDir=None,
+    recalcTimestamp=False,
+    overWrite=True,
 ):
     """
     Exports static instances from variable fonts.
     """
 
     from ftCLI.Lib.VFont import VariableFont
     from ftCLI.Lib.converters.variable_to_static import VariableToStatic
@@ -474,15 +472,15 @@
                 instances = [selected_instance]
 
             converter.run(variable_font=variable_font, instances=instances)
 
         except Exception as e:
             generic_error_message(e)
 
-        generic_info_message(f"Total files : {len(files)}")
+        generic_info_message(f"Total files     : {len(files)}")
         generic_info_message(f"Elapsed time    : {round(time.time() - start_time)} seconds")
 
 
 cli = click.CommandCollection(
     sources=[
         otf_2_ttf,
         ttf_to_otf,
```

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_fix.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_fix.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_hhea.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_hhea.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_metrics.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_metrics.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_name.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_name.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_os2.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_os2.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_post.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_post.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_print.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_print.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/ftCLI/commands/ftcli_utils.py` & `font-CLI-0.9.9/ftCLI/commands/ftcli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 import cffsubr
 import click
 from afdko import checkoutlinesufo
 from dehinter.font import dehint
 from fontTools.cffLib.specializer import specializeProgram
 from fontTools.misc.cliTools import makeOutputFileName
-from fontTools.subset import Subsetter
 from fontTools.ttLib.removeOverlaps import removeOverlaps
 from pathvalidate import sanitize_filepath, sanitize_filename
 
 from ftCLI.Lib.Font import Font
 from ftCLI.Lib.utils.cli_tools import check_output_dir, check_input_path
 from ftCLI.Lib.utils.click_tools import (
     add_file_or_path_argument,
     add_common_options,
     generic_error_message,
     file_saved_message,
     file_not_changed_message,
     generic_info_message,
 )
+from ftCLI.Lib.utils.subsetter import BaseSubsetter
 
 
 @click.group()
 def add_dummy_dsig():
     pass
 
 
@@ -588,26 +588,17 @@
     """
     files = check_input_path(input_path, allow_ttf=False, allow_variable=False)
     output_dir = check_output_dir(input_path=input_path, output_path=outputDir)
 
     for file in files:
         try:
             font = Font(file, recalcTimestamp=recalcTimestamp)
-
-            subsetter = Subsetter()
-            subsetter.options.drop_tables = []
-            subsetter.options.passthrough_tables = True
-            subsetter.options.name_IDs = "*"
-            subsetter.options.name_legacy = True
-            subsetter.options.name_languages = "*"
-            subsetter.options.layout_features = "*"
-            subsetter.options.hinting = False
-            subsetter.glyph_ids_requested = [i for i in font.getReverseGlyphMap().values()]
-            Subsetter.subset(subsetter, font)
-
+            glyph_ids = [i for i in font.getReverseGlyphMap().values()]
+            subsetter = BaseSubsetter(glyph_ids=glyph_ids)
+            subsetter.subset(font)
             output_file = makeOutputFileName(font.file, outputDir=output_dir, overWrite=overWrite)
             font.save(output_file)
             file_saved_message(output_file)
 
         except Exception as e:
             generic_error_message(e)
```

### Comparing `font-CLI-0.9.8/ftCLI/ftCLI.py` & `font-CLI-0.9.9/ftCLI/ftCLI.py`

 * *Files identical despite different names*

### Comparing `font-CLI-0.9.8/setup.py` & `font-CLI-0.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="font-CLI",
-    version="0.9.8",
+    version="0.9.9",
     description="A set of command line tools to edit fonts with FontTools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ftCLI",
     author_email="ftcli@proton.me",
     url="https://github.com/ftCLI/ftCLI",
     packages=setuptools.find_packages(),
@@ -21,15 +21,15 @@
         "fonttools>=4.39.2",
         "afdko==3.9.3",
         "beziers==0.5.0",
         "brotli==1.0.9",
         "click==8.1.3",
         "dehinter==4.0.0",
         "pathvalidate==2.5.2",
-        "rich>=13.3.2",
+        "rich>=13.3.3",
         "skia-pathops==0.7.4",
         "ttfautohint-py==0.5.1",
         "ufo2ft==2.31.0",
         "zopfli==0.2.2",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
```

