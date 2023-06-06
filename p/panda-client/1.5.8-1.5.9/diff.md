# Comparing `tmp/panda-client-1.5.8.tar.gz` & `tmp/panda-client-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-client-1.5.8.tar", last modified: Wed Mar 30 07:38:08 2022, max compression
+gzip compressed data, was "panda-client-1.5.9.tar", last modified: Thu Apr 28 11:35:17 2022, max compression
```

## Comparing `panda-client-1.5.8.tar` & `panda-client-1.5.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.641849 panda-client-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)    53356 2022-03-30 07:37:37.000000 panda-client-1.5.8/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-30 07:37:37.000000 panda-client-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-03-30 07:37:37.000000 panda-client-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-03-30 07:38:08.641849 panda-client-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-03-30 07:37:37.000000 panda-client-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.629849 panda-client-1.5.8/glade/
--rw-r--r--   0 runner    (1001) docker     (121)    24104 2022-03-30 07:37:37.000000 panda-client-1.5.8/glade/pbook.glade
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-03-30 07:37:37.000000 panda-client-1.5.8/glade/pbook.gladep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.633849 panda-client-1.5.8/icons/
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/back.png
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/config.png
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/forward.png
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/green.png
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/kill.png
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/orange.png
--rw-r--r--   0 runner    (1001) docker     (121)     6271 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/pandamon.png
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/red.png
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/retry.png
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/savannah.png
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/sync.png
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/update.png
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-03-30 07:37:37.000000 panda-client-1.5.8/icons/yellow.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.633849 panda-client-1.5.8/panda_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-03-30 07:38:07.000000 panda-client-1.5.8/panda_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-03-30 07:38:08.000000 panda-client-1.5.8/panda_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-30 07:38:07.000000 panda-client-1.5.8/panda_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-03-30 07:38:08.000000 panda-client-1.5.8/panda_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-30 07:38:08.000000 panda-client-1.5.8/panda_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.641849 panda-client-1.5.8/pandaclient/
--rw-r--r--   0 runner    (1001) docker     (121)    65210 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/AthenaUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/BookConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32382 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/BookGUI.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    53277 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/Client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3118 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/Group_argparse.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    25986 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)    13691 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/LocalJobSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)    11007 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/LocalJobsetSpec.py
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/MiscUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15025 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/MyproxyUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16016 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PBookCore.py
--rw-r--r--   0 runner    (1001) docker     (121)    15844 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PBookScript.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PLogger.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PandaToolsPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (121)    15441 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/ParseJobXML.py
--rw-r--r--   0 runner    (1001) docker     (121)   101218 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PathenaScript.py
--rw-r--r--   0 runner    (1001) docker     (121)    10137 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PchainScript.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      247 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PcontainerScript.py
--rw-r--r--   0 runner    (1001) docker     (121)    24834 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PdbUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    27416 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PhpoScript.py
--rw-r--r--   0 runner    (1001) docker     (121)   103032 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PrunScript.py
--rw-r--r--   0 runner    (1001) docker     (121)    32151 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/PsubUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/example_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/idds_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/localSpecs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10171 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/openidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9679 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/panda_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/panda_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/panda_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7280 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/pcontainer_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-03-30 07:37:37.000000 panda-client-1.5.8/pandaclient/queryPandaMonUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.641849 panda-client-1.5.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      118 2022-03-30 07:37:37.000000 panda-client-1.5.8/scripts/pathena
--rwxr-xr-x   0 runner    (1001) docker     (121)      139 2022-03-30 07:37:37.000000 panda-client-1.5.8/scripts/pbook
--rwxr-xr-x   0 runner    (1001) docker     (121)      135 2022-03-30 07:37:37.000000 panda-client-1.5.8/scripts/pchain
--rwxr-xr-x   0 runner    (1001) docker     (121)      121 2022-03-30 07:37:37.000000 panda-client-1.5.8/scripts/pcontainer
--rwxr-xr-x   0 runner    (1001) docker     (121)      133 2022-03-30 07:37:37.000000 panda-client-1.5.8/scripts/phpo
--rwxr-xr-x   0 runner    (1001) docker     (121)      133 2022-03-30 07:37:37.000000 panda-client-1.5.8/scripts/prun
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-03-30 07:38:08.641849 panda-client-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9112 2022-03-30 07:37:37.000000 panda-client-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.641849 panda-client-1.5.8/share/
--rwxr-xr-x   0 runner    (1001) docker     (121)    19929 2022-03-30 07:37:37.000000 panda-client-1.5.8/share/ConfigExtractor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2648 2022-03-30 07:37:37.000000 panda-client-1.5.8/share/FakeAppMgr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-03-30 07:37:37.000000 panda-client-1.5.8/share/functions.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 07:38:08.641849 panda-client-1.5.8/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-03-30 07:37:37.000000 panda-client-1.5.8/templates/conda_meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-03-30 07:37:37.000000 panda-client-1.5.8/templates/panda_setup.csh.template
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-03-30 07:37:37.000000 panda-client-1.5.8/templates/panda_setup.example.cfg.template
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-03-30 07:37:37.000000 panda-client-1.5.8/templates/panda_setup.sh.template
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-03-30 07:37:37.000000 panda-client-1.5.8/templates/site_path.sh.template
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.504989 panda-client-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    53404 2022-04-28 11:34:56.000000 panda-client-1.5.9/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-28 11:34:56.000000 panda-client-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-04-28 11:34:56.000000 panda-client-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-04-28 11:35:17.504989 panda-client-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-04-28 11:34:56.000000 panda-client-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.496988 panda-client-1.5.9/glade/
+-rw-r--r--   0 runner    (1001) docker     (121)    24104 2022-04-28 11:34:56.000000 panda-client-1.5.9/glade/pbook.glade
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-04-28 11:34:56.000000 panda-client-1.5.9/glade/pbook.gladep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.496988 panda-client-1.5.9/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/back.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/config.png
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/forward.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/green.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/kill.png
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/orange.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6271 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/pandamon.png
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/red.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/retry.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/savannah.png
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/sync.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/update.png
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2022-04-28 11:34:56.000000 panda-client-1.5.9/icons/yellow.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.496988 panda-client-1.5.9/panda_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-04-28 11:35:16.000000 panda-client-1.5.9/panda_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-04-28 11:35:17.000000 panda-client-1.5.9/panda_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 11:35:16.000000 panda-client-1.5.9/panda_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-04-28 11:35:17.000000 panda-client-1.5.9/panda_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-28 11:35:17.000000 panda-client-1.5.9/panda_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.500989 panda-client-1.5.9/pandaclient/
+-rw-r--r--   0 runner    (1001) docker     (121)    65210 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/AthenaUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/BookConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    32382 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/BookGUI.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    53277 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/Client.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3118 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/Group_argparse.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    25986 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13691 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/LocalJobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11007 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/LocalJobsetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/MiscUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15025 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/MyproxyUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16016 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PBookCore.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15844 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PBookScript.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PLogger.py
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PandaToolsPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15441 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/ParseJobXML.py
+-rw-r--r--   0 runner    (1001) docker     (121)   101487 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PathenaScript.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10137 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PchainScript.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      247 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PcontainerScript.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24834 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PdbUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27416 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PhpoScript.py
+-rw-r--r--   0 runner    (1001) docker     (121)   103317 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PrunScript.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32151 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/PsubUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/example_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/idds_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/localSpecs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10171 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/openidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9679 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/panda_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/panda_gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/panda_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7280 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/pcontainer_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-04-28 11:34:56.000000 panda-client-1.5.9/pandaclient/queryPandaMonUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.500989 panda-client-1.5.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      118 2022-04-28 11:34:56.000000 panda-client-1.5.9/scripts/pathena
+-rwxr-xr-x   0 runner    (1001) docker     (121)      139 2022-04-28 11:34:56.000000 panda-client-1.5.9/scripts/pbook
+-rwxr-xr-x   0 runner    (1001) docker     (121)      135 2022-04-28 11:34:56.000000 panda-client-1.5.9/scripts/pchain
+-rwxr-xr-x   0 runner    (1001) docker     (121)      121 2022-04-28 11:34:56.000000 panda-client-1.5.9/scripts/pcontainer
+-rwxr-xr-x   0 runner    (1001) docker     (121)      133 2022-04-28 11:34:56.000000 panda-client-1.5.9/scripts/phpo
+-rwxr-xr-x   0 runner    (1001) docker     (121)      133 2022-04-28 11:34:56.000000 panda-client-1.5.9/scripts/prun
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-04-28 11:35:17.504989 panda-client-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     9112 2022-04-28 11:34:56.000000 panda-client-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.504989 panda-client-1.5.9/share/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19929 2022-04-28 11:34:56.000000 panda-client-1.5.9/share/ConfigExtractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2648 2022-04-28 11:34:56.000000 panda-client-1.5.9/share/FakeAppMgr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-04-28 11:34:56.000000 panda-client-1.5.9/share/functions.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 11:35:17.504989 panda-client-1.5.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-04-28 11:34:56.000000 panda-client-1.5.9/templates/conda_meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-04-28 11:34:56.000000 panda-client-1.5.9/templates/panda_setup.csh.template
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-04-28 11:34:56.000000 panda-client-1.5.9/templates/panda_setup.example.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-04-28 11:34:56.000000 panda-client-1.5.9/templates/panda_setup.sh.template
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-04-28 11:34:56.000000 panda-client-1.5.9/templates/site_path.sh.template
```

### Comparing `panda-client-1.5.8/ChangeLog.txt` & `panda-client-1.5.9/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 ** Release Notes
 
+1.5.9
+  * added --fixedCpuTime to pathena/prun
+
 1.5.8
   * fixed --architecture of pathena/prun to keep cmtconfig stuff in task.architecture
 
 1.5.7
   * added --vo, --prodSourceLabel, and --workingGroup to pchain
 
 1.5.6
```

### Comparing `panda-client-1.5.8/LICENSE` & `panda-client-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/PKG-INFO` & `panda-client-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-client
-Version: 1.5.8
+Version: 1.5.9
 Summary: PanDA Client Package
 Home-page: https://panda-wms.readthedocs.io/en/latest/
 Author: PanDA Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `panda-client-1.5.8/README.md` & `panda-client-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/glade/pbook.glade` & `panda-client-1.5.9/glade/pbook.glade`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/back.png` & `panda-client-1.5.9/icons/back.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/config.png` & `panda-client-1.5.9/icons/config.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/forward.png` & `panda-client-1.5.9/icons/forward.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/green.png` & `panda-client-1.5.9/icons/green.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/kill.png` & `panda-client-1.5.9/icons/kill.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/orange.png` & `panda-client-1.5.9/icons/orange.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/pandamon.png` & `panda-client-1.5.9/icons/pandamon.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/red.png` & `panda-client-1.5.9/icons/red.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/retry.png` & `panda-client-1.5.9/icons/retry.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/savannah.png` & `panda-client-1.5.9/icons/savannah.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/update.png` & `panda-client-1.5.9/icons/update.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/icons/yellow.png` & `panda-client-1.5.9/icons/yellow.png`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/panda_client.egg-info/PKG-INFO` & `panda-client-1.5.9/panda_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-client
-Version: 1.5.8
+Version: 1.5.9
 Summary: PanDA Client Package
 Home-page: https://panda-wms.readthedocs.io/en/latest/
 Author: PanDA Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `panda-client-1.5.8/panda_client.egg-info/SOURCES.txt` & `panda-client-1.5.9/panda_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/AthenaUtils.py` & `panda-client-1.5.9/pandaclient/AthenaUtils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/BookConfig.py` & `panda-client-1.5.9/pandaclient/BookConfig.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/BookGUI.py` & `panda-client-1.5.9/pandaclient/BookGUI.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/Client.py` & `panda-client-1.5.9/pandaclient/Client.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/FileSpec.py` & `panda-client-1.5.9/pandaclient/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/Group_argparse.py` & `panda-client-1.5.9/pandaclient/Group_argparse.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/JobSpec.py` & `panda-client-1.5.9/pandaclient/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/LocalJobSpec.py` & `panda-client-1.5.9/pandaclient/LocalJobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/LocalJobsetSpec.py` & `panda-client-1.5.9/pandaclient/LocalJobsetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/MiscUtils.py` & `panda-client-1.5.9/pandaclient/MiscUtils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/MyproxyUtils.py` & `panda-client-1.5.9/pandaclient/MyproxyUtils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PBookCore.py` & `panda-client-1.5.9/pandaclient/PBookCore.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PBookScript.py` & `panda-client-1.5.9/pandaclient/PBookScript.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PLogger.py` & `panda-client-1.5.9/pandaclient/PLogger.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/ParseJobXML.py` & `panda-client-1.5.9/pandaclient/ParseJobXML.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PathenaScript.py` & `panda-client-1.5.9/pandaclient/PathenaScript.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,16 @@
                        'Note that priorities of tasks are relevant only in ' \
                        "each user's share, i.e., your tasks cannot jump over other user's tasks " \
                        'even if you give higher priorities.')
 group_submit.add_argument('--osMatching', action='store_const', const=True, dest='osMatching', default=False,
                   help='To let the brokerage choose sites which have the same OS as the local machine has.')
 group_job.add_argument('--cpuTimePerEvent', action='store', dest='cpuTimePerEvent', default=-1, type=int,
                 help='Expected HS06 seconds per event (~= 10 * the expected duration per event in seconds)')
+group_job.add_argument('--fixedCpuTime', action='store_const', const=True, dest='fixedCpuTime', default=False,
+                       help='Use fixed cpuTime instead of estimated cpuTime')
 group_job.add_argument('--maxWalltime', action='store', dest='maxWalltime', default=0, type=int,
   help='Max walltime for each job in hours. Note that this option works only ' \
                      'when the nevents metadata of input files are available in rucio')
 
 from pandaclient import MiscUtils
 from pandaclient.MiscUtils import commands_get_output, commands_get_status_output, commands_get_status_output_with_env
 
@@ -1467,14 +1469,16 @@
 if options.noLoopingCheck:
     taskParamMap['noLoopingCheck'] = True
 if options.maxWalltime > 0:
     taskParamMap['maxWalltime'] = options.maxWalltime
 if options.cpuTimePerEvent > 0:
     taskParamMap['cpuTime'] = options.cpuTimePerEvent
     taskParamMap['cpuTimeUnit'] = 'HS06sPerEvent'
+if options.fixedCpuTime:
+    taskParamMap['cpuTimeUnit'] = 'HS06sPerEventFixed'
 if options.memory > 0:
     taskParamMap['ramCount'] = options.memory
 if options.outDiskCount is not None:
     taskParamMap['outDiskCount'] = options.outDiskCount
     taskParamMap['outDiskUnit'] = 'kBFixed'
 if options.nCore > 1:
     taskParamMap['coreCount'] = options.nCore
```

### Comparing `panda-client-1.5.8/pandaclient/PchainScript.py` & `panda-client-1.5.9/pandaclient/PchainScript.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PdbUtils.py` & `panda-client-1.5.9/pandaclient/PdbUtils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PhpoScript.py` & `panda-client-1.5.9/pandaclient/PhpoScript.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/PrunScript.py` & `panda-client-1.5.9/pandaclient/PrunScript.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,16 @@
                            'Note that priorities of tasks are relevant only in ' \
                            "each user's share, i.e., your tasks cannot jump over other user's tasks " \
                            'even if you give higher priorities.')
     group_submit.add_argument('--osMatching', action='store_const', const=True, dest='osMatching', default=False,
                       help='To let the brokerage choose sites which have the same OS as the local machine has.')
     group_job.add_argument('--cpuTimePerEvent', action='store', dest='cpuTimePerEvent', default=-1, type=int,
                     help='Expected HS06 seconds per event (~= 10 * the expected duration per event in seconds)')
+    group_job.add_argument('--fixedCpuTime', action='store_const', const=True, dest='fixedCpuTime', default=False,
+                           help='Use fixed cpuTime instead of estimated cpuTime')
     group_job.add_argument('--maxWalltime', action='store', dest='maxWalltime', default=0, type=int,
                     help='Max walltime for each job in hours. Note that this option works only ' \
                          'when the nevents metadata of input files are available in rucio')
     group_build.add_argument("-3", action="store_true", dest="python3", default=False,
                       help="Use python3")
 
     from pandaclient import MiscUtils
@@ -1377,14 +1379,16 @@
     if options.noLoopingCheck:
         taskParamMap['noLoopingCheck'] = True
     if options.maxWalltime > 0:
         taskParamMap['maxWalltime'] = options.maxWalltime
     if options.cpuTimePerEvent > 0:
         taskParamMap['cpuTime'] = options.cpuTimePerEvent
         taskParamMap['cpuTimeUnit'] = 'HS06sPerEvent'
+    if options.fixedCpuTime:
+        taskParamMap['cpuTimeUnit'] = 'HS06sPerEventFixed'
     if options.memory > 0:
         taskParamMap['ramCount'] = options.memory
     if options.outDiskCount is not None:
         taskParamMap['outDiskCount'] = options.outDiskCount
         taskParamMap['outDiskUnit'] = 'kBFixed'
     if options.nCore > 1:
         taskParamMap['coreCount'] = options.nCore
```

### Comparing `panda-client-1.5.8/pandaclient/PsubUtils.py` & `panda-client-1.5.9/pandaclient/PsubUtils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/example_task.py` & `panda-client-1.5.9/pandaclient/example_task.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/idds_api.py` & `panda-client-1.5.9/pandaclient/idds_api.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/localSpecs.py` & `panda-client-1.5.9/pandaclient/localSpecs.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/openidc_utils.py` & `panda-client-1.5.9/pandaclient/openidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/panda_api.py` & `panda-client-1.5.9/pandaclient/panda_api.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/panda_gui.py` & `panda-client-1.5.9/pandaclient/panda_gui.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/panda_jupyter.py` & `panda-client-1.5.9/pandaclient/panda_jupyter.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/pcontainer_core.py` & `panda-client-1.5.9/pandaclient/pcontainer_core.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/pandaclient/queryPandaMonUtils.py` & `panda-client-1.5.9/pandaclient/queryPandaMonUtils.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/setup.py` & `panda-client-1.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/share/ConfigExtractor.py` & `panda-client-1.5.9/share/ConfigExtractor.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/share/FakeAppMgr.py` & `panda-client-1.5.9/share/FakeAppMgr.py`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/share/functions.sh` & `panda-client-1.5.9/share/functions.sh`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/templates/conda_meta.yaml.template` & `panda-client-1.5.9/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-client-1.5.8/templates/panda_setup.example.cfg.template` & `panda-client-1.5.9/templates/panda_setup.example.cfg.template`

 * *Files identical despite different names*

