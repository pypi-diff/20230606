# Comparing `tmp/pyiron_base-0.5.8.tar.gz` & `tmp/pyiron_base-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.5.8.tar", last modified: Tue Mar 15 20:53:08 2022, max compression
+gzip compressed data, was "pyiron_base-0.5.9.tar", last modified: Tue Mar 29 12:57:45 2022, max compression
```

## Comparing `pyiron_base-0.5.8.tar` & `pyiron_base-0.5.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.723233 pyiron_base-0.5.8/pyiron_base/archiving/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/archiving/import_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.723233 pyiron_base-0.5.8/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.723233 pyiron_base-0.5.8/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12648 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (121)    43116 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8823 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (121)     8397 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7769 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.731233 pyiron_base-0.5.8/pyiron_base/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31298 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     6409 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/filedata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)    34775 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (121)    48981 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/jedi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/object.py
--rw-r--r--   0 runner    (1001) docker     (121)    32625 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    14354 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/units.py
--rw-r--r--   0 runner    (1001) docker     (121)    10729 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/generic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.731233 pyiron_base-0.5.8/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/interfaces/has_hdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.735233 pyiron_base-0.5.8/pyiron_base/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34498 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/executable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/external.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    67494 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13242 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5152 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     9527 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/jobstatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     9444 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (121)    15129 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/path.py
--rw-r--r--   0 runner    (1001) docker     (121)    16427 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/template.py
--rw-r--r--   0 runner    (1001) docker     (121)    13758 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    14502 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.739233 pyiron_base-0.5.8/pyiron_base/master/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9885 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (121)    18775 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13510 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/list.py
--rw-r--r--   0 runner    (1001) docker     (121)    36271 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    17995 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     8090 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/master/submissionstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.739233 pyiron_base-0.5.8/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    60215 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     9360 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (121)    12776 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.743233 pyiron_base-0.5.8/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.743233 pyiron_base-0.5.8/pyiron_base/pyio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/pyio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29090 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/pyio/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.743233 pyiron_base-0.5.8/pyiron_base/server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15466 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12794 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/server/runmode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.743233 pyiron_base-0.5.8/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5839 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6073 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    19378 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/pyiron_base/table/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/pyiron_base/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.723233 pyiron_base-0.5.8/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-15 20:53:08.000000 pyiron_base-0.5.8/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-03-15 20:53:08.000000 pyiron_base-0.5.8/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 20:53:08.000000 pyiron_base-0.5.8/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-15 20:53:08.000000 pyiron_base-0.5.8/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-03-15 20:53:08.000000 pyiron_base-0.5.8/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-15 20:53:08.000000 pyiron_base-0.5.8/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-03-15 20:53:07.000000 pyiron_base-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/test_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/test_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:08.747233 pyiron_base-0.5.8/test_benchmarks/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/test_benchmarks/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/test_benchmarks/generic/test_filehdfio.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-03-15 20:53:04.000000 pyiron_base-0.5.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base/archiving/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/archiving/import_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12648 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43659 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8823 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8397 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7769 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.940418 pyiron_base-0.5.9/pyiron_base/generic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31106 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6409 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34775 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48981 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/object.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32625 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14354 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/units.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10729 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.940418 pyiron_base-0.5.9/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/interfaces/has_hdf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.940418 pyiron_base-0.5.9/pyiron_base/job/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34498 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/executable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/external.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67494 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13242 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5152 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9527 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/jobstatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9444 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15129 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16427 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13758 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14502 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/master/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9885 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18775 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13510 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36271 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17995 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8090 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/submissionstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60215 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9360 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12776 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/path.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/pyio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/pyio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29090 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/pyio/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/server/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15466 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12794 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/runmode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5839 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6073 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19378 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/table/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-03-29 12:57:44.000000 pyiron_base-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/test_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/test_benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/test_benchmarks/generic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/test_benchmarks/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/test_benchmarks/generic/test_filehdfio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/versioneer.py
```

### Comparing `pyiron_base-0.5.8/LICENSE` & `pyiron_base-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/PKG-INFO` & `pyiron_base-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.5.8
+Version: 0.5.9
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Platform: UNKNOWN
```

### Comparing `pyiron_base-0.5.8/README.rst` & `pyiron_base-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/__init__.py` & `pyiron_base-0.5.9/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/_tests.py` & `pyiron_base-0.5.9/pyiron_base/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/archiving/export_archive.py` & `pyiron_base-0.5.9/pyiron_base/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/archiving/import_archive.py` & `pyiron_base-0.5.9/pyiron_base/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/cli/__init__.py` & `pyiron_base-0.5.9/pyiron_base/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/cli/install.py` & `pyiron_base-0.5.9/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/cli/ls.py` & `pyiron_base-0.5.9/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.5.9/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/cli/rm.py` & `pyiron_base-0.5.9/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/cli/wrapper.py` & `pyiron_base-0.5.9/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/database/filetable.py` & `pyiron_base-0.5.9/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/database/generic.py` & `pyiron_base-0.5.9/pyiron_base/database/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,20 @@
     @staticmethod
     def _get_filtered_job_table(
         df: pandas.DataFrame, **kwargs: dict
     ) -> pandas.DataFrame:
         """
         Get a job table in a project based on matching values from any column in the project database
 
+        The values in `kwargs` can be wildcards, with the following special charaters:
+            - !value matches in the inverse of value
+            - *value matches anything that ends in value
+            - value* matches anything that starts with value
+            - *value* matches anything that contains value
+
         Args:
             df (pandas.DataFrame): DataFrame to be filtered
             **kwargs (dict): Optional arguments for filtering with keys matching the project database column name
                             (eg. status="finished")
 
         Returns:
             list: DataFrame containing filtered jobs
@@ -102,24 +108,31 @@
         mask = np.ones_like(df.index, dtype=bool)
         for key in kwargs.keys():
             if key not in list(df.columns):
                 raise ValueError(
                     f"Column name {key} does not exist in the project database!"
                 )
         for key, val in kwargs.items():
+            invert = False
+            if val is not None and val[0] == "!":
+                invert = True
+                val = val[1:]
             if val is None:
-                mask &= df[key].isnull()
+                update = df[key].isnull()
             elif str(val).startswith("*") and str(val).endswith("*"):
-                mask &= df[key].str.contains(str(val).replace("*", ""))
+                update = df[key].str.contains(str(val).replace("*", ""))
             elif str(val).endswith("*"):
-                mask &= df[key].str.startswith(str(val).replace("*", ""))
+                update = df[key].str.startswith(str(val).replace("*", ""))
             elif str(val).startswith("*"):
-                mask &= df[key].str.endswith(str(val).replace("*", ""))
+                update = df[key].str.endswith(str(val).replace("*", ""))
             else:
-                mask &= df[key] == val
+                update = df[key] == val
+            if invert:
+                update = ~update
+            mask &= update
         return df[mask]
 
     def job_table(
         self,
         sql_query,
         user,
         project_path,
```

### Comparing `pyiron_base-0.5.8/pyiron_base/database/jobtable.py` & `pyiron_base-0.5.9/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/database/manager.py` & `pyiron_base-0.5.9/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/database/performance.py` & `pyiron_base-0.5.9/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/database/tables.py` & `pyiron_base-0.5.9/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/datacontainer.py` & `pyiron_base-0.5.9/pyiron_base/generic/datacontainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,33 +207,28 @@
     >>> e.my_fancy_field
     42
     >>> e
     ExtendedContainer({'foo': 1, 'bar': 5})
 
     Or a class that uses a DataContainer for storage, but doesn't derive from it.
 
-    >>> class FancyClass:
+    >>> from pyiron_base.generic.object import HasStorage
+    >>> class FancyClass(HasStorage):
     ...     def __init__(self, foo):
-    ...         self.storage = DataContainer()
+    ...         super().__init__()
     ...         self.storage.foo = foo
     ...
     ...     @property
     ...     def foo(self):
     ...         return self.storage.foo
     ...
     ...     @foo.setter
     ...     def foo(self, val):
     ...         self.storage.foo = val
     ...
-    ...     def from_hdf(self, hdf, group_name):
-    ...         self.storage.from_hdf(hdf=hdf, group_name=group_name)
-    ...
-    ...     def to_hdf(self, hdf, group_name):
-    ...         self.storage.to_hdf(hdf=hdf, group_name=group_name)
-    ...
     ...     def _repr_json_(self):
     ...         return self.storage._repr_json_()
 
     """
 
     __version__ = "0.1.0"
     __hdf_version__ = "0.2.0"
```

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/dynamic.py` & `pyiron_base-0.5.9/pyiron_base/generic/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/factory.py` & `pyiron_base-0.5.9/pyiron_base/generic/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/filedata.py` & `pyiron_base-0.5.9/pyiron_base/generic/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/fileio.py` & `pyiron_base-0.5.9/pyiron_base/generic/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/flattenedstorage.py` & `pyiron_base-0.5.9/pyiron_base/generic/flattenedstorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/hdfio.py` & `pyiron_base-0.5.9/pyiron_base/generic/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/hdfstub.py` & `pyiron_base-0.5.9/pyiron_base/generic/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/jedi.py` & `pyiron_base-0.5.9/pyiron_base/generic/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/object.py` & `pyiron_base-0.5.9/pyiron_base/generic/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/parameters.py` & `pyiron_base-0.5.9/pyiron_base/generic/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/units.py` & `pyiron_base-0.5.9/pyiron_base/generic/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/generic/util.py` & `pyiron_base-0.5.9/pyiron_base/generic/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.5.9/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.5.9/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/core.py` & `pyiron_base-0.5.9/pyiron_base/job/core.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/executable.py` & `pyiron_base-0.5.9/pyiron_base/job/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/external.py` & `pyiron_base-0.5.9/pyiron_base/job/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/factory.py` & `pyiron_base-0.5.9/pyiron_base/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/generic.py` & `pyiron_base-0.5.9/pyiron_base/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/interactive.py` & `pyiron_base-0.5.9/pyiron_base/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/interactivewrapper.py` & `pyiron_base-0.5.9/pyiron_base/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/jobstatus.py` & `pyiron_base-0.5.9/pyiron_base/job/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/jobtype.py` & `pyiron_base-0.5.9/pyiron_base/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/path.py` & `pyiron_base-0.5.9/pyiron_base/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/script.py` & `pyiron_base-0.5.9/pyiron_base/job/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/template.py` & `pyiron_base-0.5.9/pyiron_base/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/util.py` & `pyiron_base-0.5.9/pyiron_base/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/worker.py` & `pyiron_base-0.5.9/pyiron_base/job/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/job/wrapper.py` & `pyiron_base-0.5.9/pyiron_base/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/master/flexible.py` & `pyiron_base-0.5.9/pyiron_base/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/master/generic.py` & `pyiron_base-0.5.9/pyiron_base/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/master/list.py` & `pyiron_base-0.5.9/pyiron_base/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/master/parallel.py` & `pyiron_base-0.5.9/pyiron_base/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/master/serial.py` & `pyiron_base-0.5.9/pyiron_base/master/serial.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/master/submissionstatus.py` & `pyiron_base-0.5.9/pyiron_base/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/project/data.py` & `pyiron_base-0.5.9/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/project/generic.py` & `pyiron_base-0.5.9/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/project/gui.py` & `pyiron_base-0.5.9/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/project/maintenance.py` & `pyiron_base-0.5.9/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/project/path.py` & `pyiron_base-0.5.9/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.5.9/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/pyio/parser.py` & `pyiron_base-0.5.9/pyiron_base/pyio/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/server/generic.py` & `pyiron_base-0.5.9/pyiron_base/server/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/server/queuestatus.py` & `pyiron_base-0.5.9/pyiron_base/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/server/runmode.py` & `pyiron_base-0.5.9/pyiron_base/server/runmode.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/__init__.py` & `pyiron_base-0.5.9/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/install.py` & `pyiron_base-0.5.9/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/logger.py` & `pyiron_base-0.5.9/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/publications.py` & `pyiron_base-0.5.9/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.5.9/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/settings.py` & `pyiron_base-0.5.9/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/state/update.py` & `pyiron_base-0.5.9/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/table/datamining.py` & `pyiron_base-0.5.9/pyiron_base/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base/toolkit.py` & `pyiron_base-0.5.9/pyiron_base/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.5.9/pyiron_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-base
-Version: 0.5.8
+Version: 0.5.9
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Platform: UNKNOWN
```

### Comparing `pyiron_base-0.5.8/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.5.9/pyiron_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/setup.py` & `pyiron_base-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         'pathlib2>=2.3.7.post1',
         'pint>=0.18',
         'psutil>=5.9.0',
         'pyfileindex>=0.0.6',
         'pysqa>=0.0.16',
         'sqlalchemy>=1.4.32',
         'tables>=3.7.0',
-        'tqdm>=4.63.0'
+        'tqdm>=4.63.1'
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     entry_points = {
             "console_scripts": [
                 'pyiron=pyiron_base.cli:main'
             ]
```

### Comparing `pyiron_base-0.5.8/test_benchmarks/generic/test_filehdfio.py` & `pyiron_base-0.5.9/test_benchmarks/generic/test_filehdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.8/versioneer.py` & `pyiron_base-0.5.9/versioneer.py`

 * *Files identical despite different names*

