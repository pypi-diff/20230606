# Comparing `tmp/netCDF4-1.6.3.tar.gz` & `tmp/netCDF4-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netCDF4-1.6.3.tar", last modified: Fri Mar  3 03:00:41 2023, max compression
+gzip compressed data, was "dist/netCDF4-1.6.4.tar", last modified: Mon Jun  5 22:29:11 2023, max compression
```

## Comparing `netCDF4-1.6.3.tar` & `netCDF4-1.6.4.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/
--rw-r--r--   0 jsw        (501) wheel        (0)    71659 2023-03-03 03:00:07.000000 netCDF4-1.6.3/Changelog
--rw-r--r--   0 jsw        (501) wheel        (0)     1056 2023-03-03 03:00:04.000000 netCDF4-1.6.3/LICENSE
--rw-r--r--   0 jsw        (501) wheel        (0)      552 2023-03-03 03:00:04.000000 netCDF4-1.6.3/MANIFEST.in
--rw-r--r--   0 jsw        (501) wheel        (0)     1570 2023-03-03 03:00:41.000000 netCDF4-1.6.3/PKG-INFO
--rw-r--r--   0 jsw        (501) wheel        (0)      298 2023-03-03 03:00:04.000000 netCDF4-1.6.3/README.htmldocs
--rw-r--r--   0 jsw        (501) wheel        (0)    17090 2023-03-03 03:00:04.000000 netCDF4-1.6.3/README.md
--rw-r--r--   0 jsw        (501) wheel        (0)     1336 2023-03-03 03:00:04.000000 netCDF4-1.6.3/README.release
--rw-r--r--   0 jsw        (501) wheel        (0)     3796 2023-03-03 03:00:04.000000 netCDF4-1.6.3/README.wheels.md
--rw-r--r--   0 jsw        (501) wheel        (0)      263 2023-03-03 03:00:04.000000 netCDF4-1.6.3/checkversion.py
--rw-r--r--   0 jsw        (501) wheel        (0)      469 2023-03-03 03:00:04.000000 netCDF4-1.6.3/create_docs.sh
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/docs/
--rw-r--r--   0 jsw        (501) wheel        (0)   386898 2023-03-03 03:00:07.000000 netCDF4-1.6.3/docs/index.html
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/examples/
--rw-r--r--   0 jsw        (501) wheel        (0)      941 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/README.md
--rw-r--r--   0 jsw        (501) wheel        (0)     1607 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/bench.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1896 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/bench_compress.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2604 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/bench_compress2.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2788 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/bench_compress3.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1988 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/bench_compress4.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2750 2023-03-03 03:00:04.000000 netCDF4-1.6.3/examples/bench_diskless.py
--rw-r--r--   0 jsw        (501) wheel        (0)      688 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/json_att.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1471 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/mpi_example.py
--rw-r--r--   0 jsw        (501) wheel        (0)      690 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/mpi_example_compressed.py
--rw-r--r--   0 jsw        (501) wheel        (0)      647 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/subset.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1883 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/test_stringarr.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1690 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/threaded_read.py
--rw-r--r--   0 jsw        (501) wheel        (0)    13476 2023-03-03 03:00:05.000000 netCDF4-1.6.3/examples/tutorial.py
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/include/
--rw-r--r--   0 jsw        (501) wheel        (0)      952 2023-03-03 03:00:05.000000 netCDF4-1.6.3/include/membuf.pyx
--rw-r--r--   0 jsw        (501) wheel        (0)      425 2023-03-03 03:00:05.000000 netCDF4-1.6.3/include/mpi-compat.h
--rw-r--r--   0 jsw        (501) wheel        (0)    21010 2023-03-03 03:00:05.000000 netCDF4-1.6.3/include/netCDF4.pxi
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/man/
--rw-r--r--   0 jsw        (501) wheel        (0)     3188 2023-03-03 03:00:05.000000 netCDF4-1.6.3/man/nc3tonc4.1
--rw-r--r--   0 jsw        (501) wheel        (0)     1374 2023-03-03 03:00:05.000000 netCDF4-1.6.3/man/nc4tonc3.1
--rw-r--r--   0 jsw        (501) wheel        (0)     1312 2023-03-03 03:00:05.000000 netCDF4-1.6.3/man/ncinfo.1
--rw-r--r--   0 jsw        (501) wheel        (0)     2026 2023-03-03 03:00:05.000000 netCDF4-1.6.3/pyproject.toml
--rw-r--r--   0 jsw        (501) wheel        (0)      193 2023-03-03 03:00:41.000000 netCDF4-1.6.3/setup.cfg
--rw-r--r--   0 jsw        (501) wheel        (0)    28565 2023-03-03 03:00:05.000000 netCDF4-1.6.3/setup.py
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/netCDF4/
--rw-r--r--   0 jsw        (501) wheel        (0)     1420 2023-03-03 03:00:05.000000 netCDF4-1.6.3/src/netCDF4/__init__.py
--rw-r--r--   0 jsw        (501) wheel        (0)   312495 2023-03-03 03:00:05.000000 netCDF4-1.6.3/src/netCDF4/_netCDF4.pyx
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/netCDF4/plugins/
--rw-r--r--   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:05.000000 netCDF4-1.6.3/src/netCDF4/plugins/empty.txt
--rw-r--r--   0 jsw        (501) wheel        (0)    37383 2023-03-03 03:00:05.000000 netCDF4-1.6.3/src/netCDF4/utils.py
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/netCDF4.egg-info/
--rw-r--r--   0 jsw        (501) wheel        (0)     1570 2023-03-03 03:00:40.000000 netCDF4-1.6.3/src/netCDF4.egg-info/PKG-INFO
--rw-r--r--   0 jsw        (501) wheel        (0)     2200 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/netCDF4.egg-info/SOURCES.txt
--rw-r--r--   0 jsw        (501) wheel        (0)        1 2023-03-03 03:00:40.000000 netCDF4-1.6.3/src/netCDF4.egg-info/dependency_links.txt
--rw-r--r--   0 jsw        (501) wheel        (0)      116 2023-03-03 03:00:40.000000 netCDF4-1.6.3/src/netCDF4.egg-info/entry_points.txt
--rw-r--r--   0 jsw        (501) wheel        (0)       13 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/netCDF4.egg-info/requires.txt
--rw-r--r--   0 jsw        (501) wheel        (0)        8 2023-03-03 03:00:41.000000 netCDF4-1.6.3/src/netCDF4.egg-info/top_level.txt
-drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-03-03 03:00:41.000000 netCDF4-1.6.3/test/
--rw-r--r--   0 jsw        (501) wheel        (0)   266966 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/20171025_2056.Cloud_Top_Height.nc
--rw-r--r--   0 jsw        (501) wheel        (0)   174660 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/CRM032_test1.nc
--rw-r--r--   0 jsw        (501) wheel        (0)     6184 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/issue1152.nc
--rw-r--r--   0 jsw        (501) wheel        (0)   123416 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/issue671.nc
--rw-r--r--   0 jsw        (501) wheel        (0)   224227 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/issue672.nc
--rw-r--r--   0 jsw        (501) wheel        (0)    16376 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/netcdf_dummy_file.nc
--rwxr-xr-x   0 jsw        (501) wheel        (0)     3677 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/run_all.py
--rw-r--r--   0 jsw        (501) wheel        (0)   222747 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/test_gold.nc
--rw-r--r--   0 jsw        (501) wheel        (0)     1832 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_Unsigned.py
--rw-r--r--   0 jsw        (501) wheel        (0)     5676 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_alignment.py
--rw-r--r--   0 jsw        (501) wheel        (0)     9842 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_atts.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1347 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_cdf5.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1624 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_cdl.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1570 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_chunk_cache.py
--rw-r--r--   0 jsw        (501) wheel        (0)    38017 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compound_alignment.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2644 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compoundatt.py
--rw-r--r--   0 jsw        (501) wheel        (0)     6011 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compoundvar.py
--rw-r--r--   0 jsw        (501) wheel        (0)     7378 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compression.py
--rw-r--r--   0 jsw        (501) wheel        (0)     4029 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compression_blosc.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2136 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compression_bzip2.py
--rw-r--r--   0 jsw        (501) wheel        (0)     5096 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compression_quant.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1716 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compression_szip.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2133 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_compression_zstd.py
--rw-r--r--   0 jsw        (501) wheel        (0)      924 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_create_mem.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1346 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_dap.py
--rw-r--r--   0 jsw        (501) wheel        (0)     6049 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_dims.py
--rw-r--r--   0 jsw        (501) wheel        (0)     3009 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_diskless.py
--rw-r--r--   0 jsw        (501) wheel        (0)     6046 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_endian.py
--rw-r--r--   0 jsw        (501) wheel        (0)     3348 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_enum.py
--rw-r--r--   0 jsw        (501) wheel        (0)     6576 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_fancyslicing.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1067 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_filepath.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1771 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_get_variables_by_attributes.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2519 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_grps.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1334 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_grps2.py
--rw-r--r--   0 jsw        (501) wheel        (0)      378 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_issue908.py
--rw-r--r--   0 jsw        (501) wheel        (0)     6127 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_masked.py
--rwxr-xr-x   0 jsw        (501) wheel        (0)     4211 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_masked2.py
--rwxr-xr-x   0 jsw        (501) wheel        (0)     5568 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_masked3.py
--rwxr-xr-x   0 jsw        (501) wheel        (0)     4136 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_masked4.py
--rwxr-xr-x   0 jsw        (501) wheel        (0)     1787 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_masked5.py
--rw-r--r--   0 jsw        (501) wheel        (0)     3641 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_masked6.py
--rw-r--r--   0 jsw        (501) wheel        (0)     6239 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_multifile.py
--rw-r--r--   0 jsw        (501) wheel        (0)     4945 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_multifile2.py
--rw-r--r--   0 jsw        (501) wheel        (0)      986 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_open_mem.py
--rw-r--r--   0 jsw        (501) wheel        (0)      978 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_refcount.py
--rw-r--r--   0 jsw        (501) wheel        (0)     5167 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_rename.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1821 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_scalarvar.py
--rwxr-xr-x   0 jsw        (501) wheel        (0)     7326 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_scaled.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1126 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_shape.py
--rw-r--r--   0 jsw        (501) wheel        (0)    10135 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_slicing.py
--rw-r--r--   0 jsw        (501) wheel        (0)     3409 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_stringarr.py
--rw-r--r--   0 jsw        (501) wheel        (0)     3886 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_types.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1180 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_unicode.py
--rw-r--r--   0 jsw        (501) wheel        (0)     1344 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_unicodeatt.py
--rw-r--r--   0 jsw        (501) wheel        (0)     2210 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_unlimdim.py
--rw-r--r--   0 jsw        (501) wheel        (0)    13906 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_utils.py
--rw-r--r--   0 jsw        (501) wheel        (0)     3378 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_vars.py
--rw-r--r--   0 jsw        (501) wheel        (0)     7675 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/tst_vlen.py
--rw-r--r--   0 jsw        (501) wheel        (0)      224 2023-03-03 03:00:05.000000 netCDF4-1.6.3/test/ubyte.nc
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/
+-rw-r--r--   0 jsw        (501) wheel        (0)    72121 2023-06-05 22:28:27.000000 netCDF4-1.6.4/Changelog
+-rw-r--r--   0 jsw        (501) wheel        (0)     1056 2023-06-05 22:28:27.000000 netCDF4-1.6.4/LICENSE
+-rw-r--r--   0 jsw        (501) wheel        (0)      552 2023-06-05 22:28:27.000000 netCDF4-1.6.4/MANIFEST.in
+-rw-r--r--   0 jsw        (501) wheel        (0)     1570 2023-06-05 22:29:11.000000 netCDF4-1.6.4/PKG-INFO
+-rw-r--r--   0 jsw        (501) wheel        (0)      298 2023-06-05 22:28:27.000000 netCDF4-1.6.4/README.htmldocs
+-rw-r--r--   0 jsw        (501) wheel        (0)    17485 2023-06-05 22:28:27.000000 netCDF4-1.6.4/README.md
+-rw-r--r--   0 jsw        (501) wheel        (0)     1336 2023-06-05 22:28:27.000000 netCDF4-1.6.4/README.release
+-rw-r--r--   0 jsw        (501) wheel        (0)     3796 2023-06-05 22:28:27.000000 netCDF4-1.6.4/README.wheels.md
+-rw-r--r--   0 jsw        (501) wheel        (0)      263 2023-06-05 22:28:27.000000 netCDF4-1.6.4/checkversion.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      469 2023-06-05 22:28:27.000000 netCDF4-1.6.4/create_docs.sh
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/docs/
+-rw-r--r--   0 jsw        (501) wheel        (0)   386898 2023-06-05 22:28:27.000000 netCDF4-1.6.4/docs/index.html
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/examples/
+-rw-r--r--   0 jsw        (501) wheel        (0)      941 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/README.md
+-rw-r--r--   0 jsw        (501) wheel        (0)     1607 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/bench.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1896 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/bench_compress.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2604 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/bench_compress2.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2788 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/bench_compress3.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1988 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/bench_compress4.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2750 2023-06-05 22:28:27.000000 netCDF4-1.6.4/examples/bench_diskless.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      688 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/json_att.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1471 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/mpi_example.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      690 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/mpi_example_compressed.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      647 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/subset.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1883 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/test_stringarr.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1690 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/threaded_read.py
+-rw-r--r--   0 jsw        (501) wheel        (0)    13476 2023-06-05 22:28:30.000000 netCDF4-1.6.4/examples/tutorial.py
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/include/
+-rw-r--r--   0 jsw        (501) wheel        (0)      952 2023-06-05 22:28:30.000000 netCDF4-1.6.4/include/membuf.pyx
+-rw-r--r--   0 jsw        (501) wheel        (0)      425 2023-06-05 22:28:30.000000 netCDF4-1.6.4/include/mpi-compat.h
+-rw-r--r--   0 jsw        (501) wheel        (0)    21058 2023-06-05 22:28:30.000000 netCDF4-1.6.4/include/netCDF4.pxi
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/man/
+-rw-r--r--   0 jsw        (501) wheel        (0)     3188 2023-06-05 22:28:30.000000 netCDF4-1.6.4/man/nc3tonc4.1
+-rw-r--r--   0 jsw        (501) wheel        (0)     1374 2023-06-05 22:28:30.000000 netCDF4-1.6.4/man/nc4tonc3.1
+-rw-r--r--   0 jsw        (501) wheel        (0)     1312 2023-06-05 22:28:30.000000 netCDF4-1.6.4/man/ncinfo.1
+-rw-r--r--   0 jsw        (501) wheel        (0)     2041 2023-06-05 22:28:30.000000 netCDF4-1.6.4/pyproject.toml
+-rw-r--r--   0 jsw        (501) wheel        (0)      193 2023-06-05 22:29:11.000000 netCDF4-1.6.4/setup.cfg
+-rw-r--r--   0 jsw        (501) wheel        (0)    28981 2023-06-05 22:28:30.000000 netCDF4-1.6.4/setup.py
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/netCDF4/
+-rw-r--r--   0 jsw        (501) wheel        (0)     1420 2023-06-05 22:28:30.000000 netCDF4-1.6.4/src/netCDF4/__init__.py
+-rw-r--r--   0 jsw        (501) wheel        (0)   313296 2023-06-05 22:28:30.000000 netCDF4-1.6.4/src/netCDF4/_netCDF4.pyx
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/netCDF4/plugins/
+-rw-r--r--   0 jsw        (501) wheel        (0)        0 2023-06-05 22:28:30.000000 netCDF4-1.6.4/src/netCDF4/plugins/empty.txt
+-rw-r--r--   0 jsw        (501) wheel        (0)    37383 2023-06-05 22:28:30.000000 netCDF4-1.6.4/src/netCDF4/utils.py
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/netCDF4.egg-info/
+-rw-r--r--   0 jsw        (501) wheel        (0)     1570 2023-06-05 22:29:10.000000 netCDF4-1.6.4/src/netCDF4.egg-info/PKG-INFO
+-rw-r--r--   0 jsw        (501) wheel        (0)     2232 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/netCDF4.egg-info/SOURCES.txt
+-rw-r--r--   0 jsw        (501) wheel        (0)        1 2023-06-05 22:29:10.000000 netCDF4-1.6.4/src/netCDF4.egg-info/dependency_links.txt
+-rw-r--r--   0 jsw        (501) wheel        (0)      116 2023-06-05 22:29:10.000000 netCDF4-1.6.4/src/netCDF4.egg-info/entry_points.txt
+-rw-r--r--   0 jsw        (501) wheel        (0)       21 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/netCDF4.egg-info/requires.txt
+-rw-r--r--   0 jsw        (501) wheel        (0)        8 2023-06-05 22:29:11.000000 netCDF4-1.6.4/src/netCDF4.egg-info/top_level.txt
+drwxr-xr-x   0 jsw        (501) wheel        (0)        0 2023-06-05 22:29:11.000000 netCDF4-1.6.4/test/
+-rw-r--r--   0 jsw        (501) wheel        (0)   266966 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/20171025_2056.Cloud_Top_Height.nc
+-rw-r--r--   0 jsw        (501) wheel        (0)   174660 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/CRM032_test1.nc
+-rw-r--r--   0 jsw        (501) wheel        (0)     6184 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/issue1152.nc
+-rw-r--r--   0 jsw        (501) wheel        (0)   123416 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/issue671.nc
+-rw-r--r--   0 jsw        (501) wheel        (0)   224227 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/issue672.nc
+-rw-r--r--   0 jsw        (501) wheel        (0)    16376 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/netcdf_dummy_file.nc
+-rwxr-xr-x   0 jsw        (501) wheel        (0)     3881 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/run_all.py
+-rw-r--r--   0 jsw        (501) wheel        (0)   222747 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/test_gold.nc
+-rw-r--r--   0 jsw        (501) wheel        (0)     1832 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_Unsigned.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     5676 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_alignment.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     9842 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_atts.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1347 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_cdf5.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1624 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_cdl.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1570 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_chunk_cache.py
+-rw-r--r--   0 jsw        (501) wheel        (0)    38017 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compound_alignment.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2644 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compoundatt.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     6011 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compoundvar.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     7378 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compression.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     4029 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compression_blosc.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2136 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compression_bzip2.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     5096 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compression_quant.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1716 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compression_szip.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2133 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_compression_zstd.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      924 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_create_mem.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1246 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_dap.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     6049 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_dims.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     3009 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_diskless.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     6046 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_endian.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     3348 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_enum.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     6576 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_fancyslicing.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1067 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_filepath.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1771 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_get_variables_by_attributes.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2519 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_grps.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1334 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_grps2.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      378 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_issue908.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     6127 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_masked.py
+-rwxr-xr-x   0 jsw        (501) wheel        (0)     4211 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_masked2.py
+-rwxr-xr-x   0 jsw        (501) wheel        (0)     5568 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_masked3.py
+-rwxr-xr-x   0 jsw        (501) wheel        (0)     4136 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_masked4.py
+-rwxr-xr-x   0 jsw        (501) wheel        (0)     1787 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_masked5.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     3641 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_masked6.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     6295 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_multifile.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     4945 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_multifile2.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1810 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_multiple_open_close.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      986 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_open_mem.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      978 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_refcount.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     5167 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_rename.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1821 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_scalarvar.py
+-rwxr-xr-x   0 jsw        (501) wheel        (0)     7326 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_scaled.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1126 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_shape.py
+-rw-r--r--   0 jsw        (501) wheel        (0)    10135 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_slicing.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     3409 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_stringarr.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     3886 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_types.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1180 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_unicode.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     1344 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_unicodeatt.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     2210 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_unlimdim.py
+-rw-r--r--   0 jsw        (501) wheel        (0)    13906 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_utils.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     3378 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_vars.py
+-rw-r--r--   0 jsw        (501) wheel        (0)     7675 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/tst_vlen.py
+-rw-r--r--   0 jsw        (501) wheel        (0)      224 2023-06-05 22:28:30.000000 netCDF4-1.6.4/test/ubyte.nc
```

### Comparing `netCDF4-1.6.3/Changelog` & `netCDF4-1.6.4/Changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+ version 1.6.4 (tag v1.6.4rel)
+===============================
+ * set path to SSL certificates internally, so https DAP URLs work with wheels
+   (issue #1246, requires nc_rc_set function available starting with netcdf-c
+   4.9.1, plus bugfix in netcdf-c PR #2690).
+   Added certifi as a dependency.
+ * Added `isopen` method to `MFDataset` object to check if underlying files are open.
+
  version 1.6.3 (tag v1.6.3rel)
 ==============================
  * Use ``nc_put_vars`` for strided writes for netcdf-c >= 4.6.2 (issue #1222).
- * _Unsigned="false" should be same as not having _Unsigned set (issue #1232). 
+ * _Unsigned="false" should be same as not having _Unsigned set (issue #1232).
    _Unsigned now must be set to "true" or "True" for variable to be interpreted
    as unsigned, instead of just having _Unsigned be set (to anything).
+ * pypi wheels built with netcdf-c 4.9.1.
 
  version 1.6.2 (tag v1.6.2rel)
 ==============================
  * Added ``netCDF4.__has_set_alignment__`` property to help identify if the
    underlying netcdf4 supports setting the HDF5 alignment.
  * Slicing multi-dimensional variables with an all False boolean index array
    now returns an empty numpy array (instead of raising an exception - issue #1197).
    Behavior now consistent with numpy slicing.
  * fix problem with compiling using netcdf-c < 4.9.0 (issue #1209)
+ * pypi wheels build with netcdf-c 4.9.0.
 
  version 1.6.1 (tag v1.6.1rel)
 ==============================
  * add Dataset methods has_<name>_filter (where <name>=zstd,blosc,bzip2,szip)
    to check for availability of extra compression filters.
  * release GIL for all C-lib calls (issue #1180).
  * Add support for nc_set_alignment and nc_get_alignment to control alignment
@@ -45,23 +55,23 @@
    directory with the compression plugin lib__nc* files, then the compression plugins will
    be installed within the package and be automatically available (the binary
    wheels have this).  Otherwise, the environment variable HDF5_PLUGIN_PATH
    needs to be set at runtime  to point to plugins in order to use the new compression
    options.
  * MFDataset did not aggregate 'name' variable attribute (issue #1153).
  * issue warning instead of raising an exception if missing_value or
-   _FillValue can't be cast to the variable type when creating a 
-   masked array (issue #1152).  
+   _FillValue can't be cast to the variable type when creating a
+   masked array (issue #1152).
  * Define MPI_Session for compatibility with current mpi4py (PR #1156).
 
  version 1.5.8 (tag v1.5.8rel)
 ==============================
  * Fix Enum bug (issue #1128): the enum_dict member of an EnumType read from a file
    contains invalid values when the enum is large enough (more than 127 or 255
-   members). 
+   members).
  * Binary wheels for aarch64 and python 3.10.
 
  version 1.5.7 (tag v1.5.7rel)
 ==============================
  * don't try to mask vlens with default  _FillValue, since vlens don't have a default _FillValue.
    This gets rid of numpy DeprecationWarning (issue #1099).
  * update docs to reflect the fact that a variable must be in collective mode before writing
@@ -108,15 +118,15 @@
    default chunk cache sizes before opening a Dataset (issue #1018).
  * replace use of numpy's deprecated tostring() method with tobytes()
    (issue #1023).
  * bump minimal numpy version to 1.9 (first version to have tobytes()).
 
  version 1.5.3 (tag v1.5.3rel)
 ==============================
- * make sure arrays are masked that are not filled when auto_fill is off 
+ * make sure arrays are masked that are not filled when auto_fill is off
    (issue #972).
  * python 3.8 binary wheels.
 
  version 1.5.2 (tag v1.5.2rel)
 ==============================
  * fix for scaling bug when _Unsigned attribute is set and byteorder of data
    does not match native byteorder (issue #930).
@@ -150,15 +160,15 @@
  * make sure data gets converted to type of scale_factor when add_offset=0
    and scale_factor=1 (issue #913).
  * fix for reading empty (NIL) string attributes (issue #915).
 
  version 1.5.0.1 (tag v1.5.0.1rel)
 ==================================
  * binary wheels for linux and macosx rebuilt against netcdf-c 4.6.3 (instead
-   of 4.4.1.1).  
+   of 4.4.1.1).
  * add read-shared mode (mode='rs'). Significantly speeds up reads of NETCDF3
    files (pull request #902).
 
  version 1.5.0 (tag v1.5.0rel)
 ===============================
  * added support for parallel IO in the classic netcdf-3 formats through the
    pnetcdf library (pull request #897).
```

### Comparing `netCDF4-1.6.3/LICENSE` & `netCDF4-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/MANIFEST.in` & `netCDF4-1.6.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/PKG-INFO` & `netCDF4-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netCDF4
-Version: 1.6.3
+Version: 1.6.4
 Summary: Provides an object-oriented python interface to the netCDF version 4 library
 Author-email: Jeff Whitaker <jeffrey.s.whitaker@noaa.gov>
 License: MIT
 Project-URL: Documentation, https://unidata.github.io/netcdf4-python/
 Project-URL: Repository, https://github.com/Unidata/netcdf4-python
 Keywords: numpy,netcdf,data,science,network,oceanography,meteorology,climate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netCDF4-1.6.3/README.md` & `netCDF4-1.6.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # [netcdf4-python](http://unidata.github.io/netcdf4-python)
 [Python](http://python.org)/[numpy](http://numpy.org) interface to the netCDF [C library](https://github.com/Unidata/netcdf-c).
 
 [![Build status](https://github.com/Unidata/netcdf4-python/workflows/Build%20and%20Test/badge.svg)](https://github.com/Unidata/netcdf4-python/actions)
-[![PyPI package](https://badge.fury.io/py/netCDF4.svg)](http://python.org/pypi/netCDF4)
+[![PyPI package](https://img.shields.io/pypi/v/netCDF4.svg)](http://python.org/pypi/netCDF4)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/netCDF4/badges/version.svg)](https://anaconda.org/conda-forge/netCDF4)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2592291.svg)](https://doi.org/10.5281/zenodo.2592290)
 
 
 ## News
 For details on the latest updates, see the [Changelog](https://github.com/Unidata/netcdf4-python/blob/master/Changelog).
 
+6/4/2023:  Version [1.6.4](https://pypi.python.org/pypi/netCDF4/1.6.4) released.  Now requires 
+[certifi](https://github.com/certifi/python-certifi) to locate SSL certificates - this allows 
+OpenDAP https URLs to work with linux wheels (issue [#1246](https://github.com/Unidata/netcdf4-python/issues/1246).
+
+3/3/2023:  Version [1.6.3](https://pypi.python.org/pypi/netCDF4/1.6.3) released.
+
 11/15/2022:  Version [1.6.2](https://pypi.python.org/pypi/netCDF4/1.6.2) released. Fix for
 compilation with netcdf-c < 4.9.0 (issue [#1209](https://github.com/Unidata/netcdf4-python/issues/1209)).  
 Slicing multi-dimensional variables with an all False boolean index array
 now returns an empty numpy array (instead of raising an exception - issue [#1197](https://github.com/Unidata/netcdf4-python/issues/1197)).
 
 09/18/2022:  Version [1.6.1](https://pypi.python.org/pypi/netCDF4/1.6.1) released.  GIL now
 released for all C lib calls, `set_alignment` and `get_alignment` module functions
```

### Comparing `netCDF4-1.6.3/README.release` & `netCDF4-1.6.4/README.release`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/README.wheels.md` & `netCDF4-1.6.4/README.wheels.md`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/docs/index.html` & `netCDF4-1.6.4/docs/index.html`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/README.md` & `netCDF4-1.6.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/bench.py` & `netCDF4-1.6.4/examples/bench.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/bench_compress.py` & `netCDF4-1.6.4/examples/bench_compress.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/bench_compress2.py` & `netCDF4-1.6.4/examples/bench_compress2.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/bench_compress3.py` & `netCDF4-1.6.4/examples/bench_compress3.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/bench_compress4.py` & `netCDF4-1.6.4/examples/bench_compress4.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/bench_diskless.py` & `netCDF4-1.6.4/examples/bench_diskless.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/json_att.py` & `netCDF4-1.6.4/examples/json_att.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/mpi_example.py` & `netCDF4-1.6.4/examples/mpi_example.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/mpi_example_compressed.py` & `netCDF4-1.6.4/examples/mpi_example_compressed.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/subset.py` & `netCDF4-1.6.4/examples/subset.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/test_stringarr.py` & `netCDF4-1.6.4/examples/test_stringarr.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/threaded_read.py` & `netCDF4-1.6.4/examples/threaded_read.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/examples/tutorial.py` & `netCDF4-1.6.4/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/include/membuf.pyx` & `netCDF4-1.6.4/include/membuf.pyx`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/include/netCDF4.pxi` & `netCDF4-1.6.4/include/netCDF4.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,15 @@
     int nc_def_enum(int ncid, nc_type base_typeid, char *name, nc_type *typeidp) nogil
     int nc_insert_enum(int ncid, nc_type xtype, char *name, void *value) nogil
     int nc_inq_enum(int ncid, nc_type xtype, char *name, nc_type *base_nc_typep,\
 	    size_t *base_sizep, size_t *num_membersp) nogil
     int nc_inq_enum_member(int ncid, nc_type xtype, int idx, char *name, void *value) nogil
 
     int nc_inq_enum_ident(int ncid, nc_type xtype, long long value, char *identifier) nogil
+    int nc_rc_set(char* key, char* value) nogil
 
 IF HAS_QUANTIZATION_SUPPORT:
     cdef extern from "netcdf.h":
         cdef enum:
             NC_NOQUANTIZE
             NC_QUANTIZE_BITGROOM
             NC_QUANTIZE_GRANULARBR
```

### Comparing `netCDF4-1.6.3/man/nc3tonc4.1` & `netCDF4-1.6.4/man/nc3tonc4.1`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/man/nc4tonc3.1` & `netCDF4-1.6.4/man/nc4tonc3.1`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/man/ncinfo.1` & `netCDF4-1.6.4/man/ncinfo.1`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/pyproject.toml` & `netCDF4-1.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Compression",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "cftime",
+    "certifi",
     "numpy",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 nc3tonc4 = "netCDF4.utils:nc3tonc4"
 nc4tonc3 = "netCDF4.utils:nc4tonc3"
```

### Comparing `netCDF4-1.6.3/setup.py` & `netCDF4-1.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     has_szip_support = False
     has_quantize = False
     has_zstandard = False
     has_bzip2 = False
     has_blosc = False
     has_ncfilter = False
     has_set_alignment = False
+    has_nc_rc_set = False
 
     for d in inc_dirs:
         try:
             f = open(os.path.join(d, 'netcdf.h'), **open_kwargs)
         except OSError:
             continue
 
@@ -79,14 +80,16 @@
                 has_nc_inq_format_extended = True
             if line.startswith('#define NC_FORMAT_64BIT_DATA'):
                 has_cdf5_format = True
             if line.startswith('nc_def_var_quantize'):
                 has_quantize = True
             if line.startswith('nc_set_alignment'):
                 has_set_alignment = True
+            if line.startswith('EXTERNL int nc_rc_set'):
+                has_nc_rc_set = True
 
         if has_nc_open_mem:
             try:
                 f = open(os.path.join(d, 'netcdf_mem.h'), **open_kwargs)
             except OSError:
                 continue
             for line in f:
@@ -146,15 +149,16 @@
         elif netcdf_lib_version == "4.6.1" and not has_parallel4_support and has_parallel_support:
             has_parallel4_support = True
         break
 
     return has_rename_grp, has_nc_inq_path, has_nc_inq_format_extended, \
            has_cdf5_format, has_nc_open_mem, has_nc_create_mem, \
            has_parallel4_support, has_pnetcdf_support, has_szip_support, has_quantize, \
-           has_zstandard, has_bzip2, has_blosc, has_set_alignment, has_ncfilter
+           has_zstandard, has_bzip2, has_blosc, has_set_alignment, has_ncfilter, \
+           has_nc_rc_set
 
 
 def getnetcdfvers(libdirs):
     """
     Get the version string for the first netcdf lib found in libdirs.
     (major.minor.release). If nothing found, return None.
     """
@@ -560,15 +564,15 @@
     if len(sys.argv) >= 2:
         if os.path.exists(netcdf4_src_c):
             os.remove(netcdf4_src_c)
     # this determines whether renameGroup and filepath methods will work.
     has_rename_grp, has_nc_inq_path, has_nc_inq_format_extended, \
     has_cdf5_format, has_nc_open_mem, has_nc_create_mem, \
     has_parallel4_support, has_pnetcdf_support, has_szip_support, has_quantize, \
-    has_zstandard, has_bzip2, has_blosc, has_set_alignment, has_ncfilter = \
+    has_zstandard, has_bzip2, has_blosc, has_set_alignment, has_ncfilter, has_nc_rc_set = \
     check_api(inc_dirs,netcdf_lib_version)
     # for netcdf 4.4.x CDF5 format is always enabled.
     if netcdf_lib_version is not None and\
        (netcdf_lib_version > "4.4" and netcdf_lib_version < "4.5"):
         has_cdf5_format = True
 
     # disable parallel support if mpi4py not available.
@@ -682,14 +686,21 @@
     if has_ncfilter:
         sys.stdout.write('netcdf lib has nc_inq_filter_avail function\n')
         f.write('DEF HAS_NCFILTER = 1\n')
     else:
         sys.stdout.write('netcdf lib does not have nc_inq_filter_avail function\n')
         f.write('DEF HAS_NCFILTER = 0\n')
 
+    if has_nc_rc_set:
+        sys.stdout.write('netcdf lib has nc_rc_set function\n')
+        f.write('DEF HAS_NCRCSET = 1\n')
+    else:
+        sys.stdout.write('netcdf lib does not have nc_rc_set function\n')
+        f.write('DEF HAS_NCRCSET = 0\n')
+
     f.close()
 
     if has_parallel4_support or has_pnetcdf_support:
         import mpi4py
         inc_dirs.append(mpi4py.get_include())
         # mpi_incdir should not be needed if using nc-config
         # (should be included in nc-config --cflags)
```

### Comparing `netCDF4-1.6.3/src/netCDF4/__init__.py` & `netCDF4-1.6.4/src/netCDF4/__init__.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/src/netCDF4/_netCDF4.pyx` & `netCDF4-1.6.4/src/netCDF4/_netCDF4.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Version 1.6.3
+Version 1.6.4
 -------------
 
 # Introduction
 
 netcdf4-python is a Python interface to the netCDF C library.
 
 [netCDF](http://www.unidata.ucar.edu/software/netcdf/) version 4 has many features
@@ -29,15 +29,15 @@
    (or if you use the [conda](http://conda.io) package manager `conda install -c conda-forge netCDF4`).
 
 ## Developer Install
 
  - Clone the
    [github repository](http://github.com/Unidata/netcdf4-python).
  - Make sure the dependencies are satisfied (Python 3.7 or later,
-   [numpy](http://numpy.scipy.org), 
+   [numpy](http://numpy.scipy.org),
    [Cython](http://cython.org),
    [cftime](https://github.com/Unidata/cftime),
    [setuptools](https://pypi.python.org/pypi/setuptools),
    the [HDF5 C library](https://www.hdfgroup.org/solutions/hdf5/),
    and the [netCDF C library](https://www.unidata.ucar.edu/software/netcdf/)).
    For MPI parallel IO support, an MPI-enabled versions of the netcdf library
    is required, as is [mpi4py](http://mpi4py.scipy.org).
@@ -151,20 +151,20 @@
 ```python
 >>> rootgrp = Dataset("test.nc", "a")
 >>> fcstgrp = rootgrp.createGroup("forecasts")
 >>> analgrp = rootgrp.createGroup("analyses")
 >>> print(rootgrp.groups)
 {'forecasts': <class 'netCDF4._netCDF4.Group'>
 group /forecasts:
-    dimensions(sizes): 
-    variables(dimensions): 
+    dimensions(sizes):
+    variables(dimensions):
     groups: , 'analyses': <class 'netCDF4._netCDF4.Group'>
 group /analyses:
-    dimensions(sizes): 
-    variables(dimensions): 
+    dimensions(sizes):
+    variables(dimensions):
     groups: }
 >>>
 ```
 
 Groups can exist within groups in a `Dataset`, just as directories
 exist within directories in a unix filesystem. Each `Group` instance
 has a `groups` attribute dictionary containing all of the group
@@ -192,40 +192,40 @@
 >>> def walktree(top):
 ...     yield top.groups.values()
 ...     for value in top.groups.values():
 ...         yield from walktree(value)
 >>> print(rootgrp)
 <class 'netCDF4._netCDF4.Dataset'>
 root group (NETCDF4 data model, file format HDF5):
-    dimensions(sizes): 
-    variables(dimensions): 
+    dimensions(sizes):
+    variables(dimensions):
     groups: forecasts, analyses
 >>> for children in walktree(rootgrp):
 ...     for child in children:
 ...         print(child)
 <class 'netCDF4._netCDF4.Group'>
 group /forecasts:
-    dimensions(sizes): 
-    variables(dimensions): 
+    dimensions(sizes):
+    variables(dimensions):
     groups: model1, model2
 <class 'netCDF4._netCDF4.Group'>
 group /analyses:
-    dimensions(sizes): 
-    variables(dimensions): 
-    groups: 
+    dimensions(sizes):
+    variables(dimensions):
+    groups:
 <class 'netCDF4._netCDF4.Group'>
 group /forecasts/model1:
-    dimensions(sizes): 
-    variables(dimensions): 
-    groups: 
+    dimensions(sizes):
+    variables(dimensions):
+    groups:
 <class 'netCDF4._netCDF4.Group'>
 group /forecasts/model2:
-    dimensions(sizes): 
-    variables(dimensions): 
-    groups: 
+    dimensions(sizes):
+    variables(dimensions):
+    groups:
 ```
 
 ## Dimensions in a netCDF file
 
 netCDF defines the sizes of all variables in terms of dimensions, so
 before any variables can be created the dimensions they use must be
 created first. A special case, not often used in practice, is that of a
@@ -352,17 +352,17 @@
 You can also query a `Dataset` or `Group` instance directly to obtain `Group` or
 `Variable` instances using paths.
 
 ```python
 >>> print(rootgrp["/forecasts/model1"])  # a Group instance
 <class 'netCDF4._netCDF4.Group'>
 group /forecasts/model1:
-    dimensions(sizes): 
+    dimensions(sizes):
     variables(dimensions): float32 temp(time,level,lat,lon)
-    groups: 
+    groups:
 >>> print(rootgrp["/forecasts/model1/temp"])  # a Variable instance
 <class 'netCDF4._netCDF4.Variable'>
 float32 temp(time, level, lat, lon)
 path = /forecasts/model1
 unlimited dimensions: time, level
 current shape = (0, 0, 73, 144)
 filling on, default _FillValue of 9.969209968386869e+36 used
@@ -380,19 +380,19 @@
 current shape = (0,)
 filling on, default _FillValue of 9.969209968386869e+36 used, 'level': <class 'netCDF4._netCDF4.Variable'>
 int32 level(level)
 unlimited dimensions: level
 current shape = (0,)
 filling on, default _FillValue of -2147483647 used, 'lat': <class 'netCDF4._netCDF4.Variable'>
 float32 lat(lat)
-unlimited dimensions: 
+unlimited dimensions:
 current shape = (73,)
 filling on, default _FillValue of 9.969209968386869e+36 used, 'lon': <class 'netCDF4._netCDF4.Variable'>
 float32 lon(lon)
-unlimited dimensions: 
+unlimited dimensions:
 current shape = (144,)
 filling on, default _FillValue of 9.969209968386869e+36 used, 'temp': <class 'netCDF4._netCDF4.Variable'>
 float32 temp(time, level, lat, lon)
     units: K
 unlimited dimensions: time, level
 current shape = (0, 0, 73, 144)
 filling on, default _FillValue of 9.969209968386869e+36 used}
@@ -668,15 +668,15 @@
 and `endian` keyword arguments to
 `Dataset.createVariable`.  These keyword arguments only
 are relevant for `NETCDF4` and `NETCDF4_CLASSIC` files (where the
 underlying file format is HDF5) and are silently ignored if the file
 format is `NETCDF3_CLASSIC`, `NETCDF3_64BIT_OFFSET` or `NETCDF3_64BIT_DATA`.
 If the HDF5 library is built with szip support, compression=`szip` can also
 be used (in conjunction with the `szip_coding` and `szip_pixels_per_block` keyword
-arguments).  
+arguments).
 
 If your data only has a certain number of digits of precision (say for
 example, it is temperature data that was measured with a precision of
 0.1 degrees), you can dramatically improve compression by
 quantizing (or truncating) the data. There are two methods supplied for
 doing this.  You can use the `least_significant_digit`
 keyword argument to `Dataset.createVariable` to specify
@@ -778,15 +778,15 @@
 
 ```python
 >>> print(f)
 <class 'netCDF4._netCDF4.Dataset'>
 root group (NETCDF4 data model, file format HDF5):
     dimensions(sizes): x_dim(3)
     variables(dimensions): {'names':['real','imag'], 'formats':['<f8','<f8'], 'offsets':[0,8], 'itemsize':16, 'aligned':True} cmplx_var(x_dim)
-    groups: 
+    groups:
 >>> print(f.variables["cmplx_var"])
 <class 'netCDF4._netCDF4.Variable'>
 compound cmplx_var(x_dim)
 compound data type: {'names':['real','imag'], 'formats':['<f8','<f8'], 'offsets':[0,8], 'itemsize':16, 'aligned':True}
 unlimited dimensions: x_dim
 current shape = (3,)
 >>> print(f.cmptypes)
@@ -847,20 +847,20 @@
  [array([1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=int32)
   array([1, 2, 3, 4, 5], dtype=int32) array([1, 2], dtype=int32)]]
 >>> print(f)
 <class 'netCDF4._netCDF4.Dataset'>
 root group (NETCDF4 data model, file format HDF5):
     dimensions(sizes): x(3), y(4)
     variables(dimensions): int32 phony_vlen_var(y,x)
-    groups: 
+    groups:
 >>> print(f.variables["phony_vlen_var"])
 <class 'netCDF4._netCDF4.Variable'>
 vlen phony_vlen_var(y, x)
 vlen data type: int32
-unlimited dimensions: 
+unlimited dimensions:
 current shape = (4, 3)
 >>> print(f.vltypes["phony_vlen"])
 <class 'netCDF4._netCDF4.VLType'>: name = 'phony_vlen', numpy dtype = int32
 ```
 
 Numpy object arrays containing python strings can also be written as vlen
 variables,  For vlen strings, you don't need to create a vlen data type.
@@ -889,20 +889,20 @@
 ['Lh' '25F8wBbMI' '53rmM' 'vvjnb3t63ao' 'qjRBQk6w' 'aJh' 'QF'
  'jtIJbJACaQk4' '3Z5' 'bftIIq']
 >>> print(f)
 <class 'netCDF4._netCDF4.Dataset'>
 root group (NETCDF4 data model, file format HDF5):
     dimensions(sizes): x(3), y(4), z(10)
     variables(dimensions): int32 phony_vlen_var(y,x), <class 'str'> strvar(z)
-    groups: 
+    groups:
 >>> print(f.variables["strvar"])
 <class 'netCDF4._netCDF4.Variable'>
 vlen strvar(z)
 vlen data type: <class 'str'>
-unlimited dimensions: 
+unlimited dimensions:
 current shape = (10,)
 ```
 
 It is also possible to set contents of vlen string variables with numpy arrays
 of any string or unicode data type. Note, however, that accessing the contents
 of such variables will always return numpy arrays with dtype `object`.
 
@@ -963,15 +963,15 @@
 >>> nc.close()
 ```
 
 ## Parallel IO
 
 If MPI parallel enabled versions of netcdf and hdf5 or pnetcdf are detected,
 and [mpi4py](https://mpi4py.scipy.org) is installed, netcdf4-python will
-be built with parallel IO capabilities enabled. Parallel IO of NETCDF4 or 
+be built with parallel IO capabilities enabled. Parallel IO of NETCDF4 or
 NETCDF4_CLASSIC formatted files is only available if the MPI parallel HDF5
 library is available. Parallel IO of classic netcdf-3 file formats is only
 available if the [PnetCDF](https://parallel-netcdf.github.io/) library is
 available. To use parallel IO, your program must be running in an MPI
 environment using [mpi4py](https://mpi4py.scipy.org).
 
 ```python
@@ -1150,15 +1150,15 @@
 >>> v = nc.createVariable('v',np.int32,'x')
 >>> v[0:5] = np.arange(5)
 >>> print(nc)
 <class 'netCDF4._netCDF4.Dataset'>
 root group (NETCDF4 data model, file format HDF5):
     dimensions(sizes): x(5)
     variables(dimensions): int32 v(x)
-    groups: 
+    groups:
 >>> print(nc['v'][:])
 [0 1 2 3 4]
 >>> nc.close() # file saved to disk
 >>> # create an in-memory dataset from an existing python
 >>> # python memory buffer.
 >>> # read the newly created netcdf file into a python
 >>> # bytes object.
@@ -1167,15 +1167,15 @@
 >>> # create a netCDF in-memory dataset from the bytes object.
 >>> nc = Dataset('inmemory.nc', memory=nc_bytes)
 >>> print(nc)
 <class 'netCDF4._netCDF4.Dataset'>
 root group (NETCDF4 data model, file format HDF5):
     dimensions(sizes): x(5)
     variables(dimensions): int32 v(x)
-    groups: 
+    groups:
 >>> print(nc['v'][:])
 [0 1 2 3 4]
 >>> nc.close()
 >>> # create an in-memory Dataset and retrieve memory buffer
 >>> # estimated size is 1028 bytes - this is actually only
 >>> # used if format is NETCDF3
 >>> # (ignored for NETCDF4/HDF5 files).
@@ -1222,16 +1222,17 @@
 from cpython.buffer cimport PyObject_GetBuffer, PyBuffer_Release, PyBUF_SIMPLE, PyBUF_ANY_CONTIGUOUS
 from cpython.bytes cimport PyBytes_FromStringAndSize
 
 # pure python utilities
 from .utils import (_StartCountStride, _quantize, _find_dim, _walk_grps,
                     _out_array_shape, _sortbylist, _tostr, _safecast, _is_int)
 import sys
+import functools
 
-__version__ = "1.6.3"
+__version__ = "1.6.4"
 
 # Initialize numpy
 import posixpath
 from cftime import date2num, num2date, date2index
 import numpy
 cimport numpy
 import weakref
@@ -1254,22 +1255,36 @@
                                MPI_COMM_WORLD
     ctypedef MPI.Comm Comm
     ctypedef MPI.Info Info
 ELSE:
     ctypedef object Comm
     ctypedef object Info
 
+# set path to SSL certificates (issue #1246)
+IF HAS_NCRCSET: # available starting in version 4.9.1
+    import certifi
+    cdef _set_curl_certpath(certpath):
+        cdef char *cert_path
+        cdef char *key
+        cdef int ierr
+        bytestr = _strencode(certpath)
+        cert_path = bytestr
+        ierr = nc_rc_set("HTTP.SSL.CAINFO",cert_path)
+        if ierr != 0:
+            raise RuntimeError('error setting path to SSL certificates')
+    _set_curl_certpath(certifi.where())
+
 # check for required version of netcdf-4 and hdf5.
 
 def _gethdf5libversion():
     cdef unsigned int majorvers, minorvers, releasevers
     cdef herr_t ierr
     with nogil:
         ierr = H5get_libversion( &majorvers, &minorvers, &releasevers)
-    if ierr < 0:
+    if ierr != 0:
         raise RuntimeError('error getting HDF5 library version info')
     return '%d.%d.%d' % (majorvers,minorvers,releasevers)
 
 def getlibversion():
     """
 **`getlibversion()`**
 
@@ -1388,17 +1403,17 @@
                (__netcdf4libversion__.startswith("4.4.0") and \
                 "-development" in __netcdf4libversion__)
 
 # issue warning for hdf5 1.10 (issue #549)
 if __netcdf4libversion__[0:5] < "4.4.1" and\
    __hdf5libversion__.startswith("1.10"):
     msg = """
-WARNING: Backwards incompatible files will be created with HDF5 1.10.x 
-and netCDF < 4.4.1. Upgrading to netCDF4 >= 4.4.1 or downgrading to 
-to HDF5 version 1.8.x is highly recommended 
+WARNING: Backwards incompatible files will be created with HDF5 1.10.x
+and netCDF < 4.4.1. Upgrading to netCDF4 >= 4.4.1 or downgrading to
+to HDF5 version 1.8.x is highly recommended
 (see https://github.com/Unidata/netcdf-c/issues/250)."""
     warnings.warn(msg)
 
 # numpy data type <--> netCDF 4 data type mapping.
 _nptonctype  = {'S1' : NC_CHAR,
                 'i1' : NC_BYTE,
                 'u1' : NC_UBYTE,
@@ -2115,16 +2130,16 @@
         **`filename`**: Name of netCDF file to hold dataset. Can also
         be a python 3 pathlib instance or the URL of an OpenDAP dataset.  When memory is
         set this is just used to set the `filepath()`.
 
         **`mode`**: access mode. `r` means read-only; no data can be
         modified. `w` means write; a new file is created, an existing file with
         the same name is deleted. `x` means write, but fail if an existing
-        file with the same name already exists. `a` and `r+` mean append; 
-        an existing file is opened for reading and writing, if 
+        file with the same name already exists. `a` and `r+` mean append;
+        an existing file is opened for reading and writing, if
         file does not exist already, one is created.
         Appending `s` to modes `r`, `w`, `r+` or `a` will enable unbuffered shared
         access to `NETCDF3_CLASSIC`, `NETCDF3_64BIT_OFFSET` or
         `NETCDF3_64BIT_DATA` formatted files.
         Unbuffered access may be useful even if you don't need shared
         access, since it may be faster for programs that don't access data
         sequentially. This option is ignored for `NETCDF4` and `NETCDF4_CLASSIC`
@@ -2397,15 +2412,15 @@
                     ierr = nc_open(path, NC_SHARE, &grpid)
         elif mode == 'ws' or (mode in ['as','r+s'] and not os.path.exists(filename)):
             _set_default_format(format=format)
             if clobber:
                 if parallel:
                     # NC_SHARE ignored
                     IF HAS_PARALLEL4_SUPPORT or HAS_PNETCDF_SUPPORT:
-                        cmode = NC_CLOBBER | parmode 
+                        cmode = NC_CLOBBER | parmode
                         with nogil:
                             ierr = nc_create_par(path, NC_CLOBBER | cmode, \
                                    mpicomm, mpiinfo, &grpid)
                     ELSE:
                         pass
                 elif diskless:
                     if persist:
@@ -2613,15 +2628,17 @@
 **`isopen(self)`**
 
 Is the Dataset open or closed?
         """
         return bool(self._isopen)
 
     def __dealloc__(self):
-        # close file when there are no references to object left
+        # close file when there are no references to object left and clear the cache.
+        if self.get_variables_by_attributes:
+            self.get_variables_by_attributes.cache_clear()
         if self._isopen:
            self._close(False)
 
     def __reduce__(self):
         # raise error is user tries to pickle a Dataset object.
         raise NotImplementedError('Dataset is not picklable')
 
@@ -2759,15 +2776,15 @@
 
 The return value is the `EnumType` class instance describing the new
 datatype."""
         self.enumtypes[datatype_name] = EnumType(self, datatype, datatype_name,
                 enum_dict)
         return self.enumtypes[datatype_name]
 
-    def createVariable(self, varname, datatype, dimensions=(), 
+    def createVariable(self, varname, datatype, dimensions=(),
             compression=None, zlib=False,
             complevel=4, shuffle=True,
             szip_coding='nn',szip_pixels_per_block=8,
             blosc_shuffle=1,fletcher32=False, contiguous=False,
             chunksizes=None, endian='native', least_significant_digit=None,
             significant_digits=None,quantize_mode='BitGroom',fill_value=None, chunk_cache=None):
         """
@@ -2811,15 +2828,15 @@
 compressed in the netCDF file using the specified compression algorithm.
 Currently `zlib`,`szip`,`zstd`,`bzip2`,`blosc_lz`,`blosc_lz4`,`blosc_lz4hc`,
 `blosc_zlib` and `blosc_zstd` are supported.
 Default is `None` (no compression).  All of the compressors except
 `zlib` and `szip` use the HDF5 plugin architecture.
 
 If the optional keyword `zlib` is `True`, the data will be compressed in
-the netCDF file using zlib compression (default `False`).  The use of this option is 
+the netCDF file using zlib compression (default `False`).  The use of this option is
 deprecated in favor of `compression='zlib'`.
 
 The optional keyword `complevel` is an integer between 0 and 9 describing
 the level of compression desired (default 4). Ignored if `compression=None`.
 A value of zero disables compression.
 
 If the optional keyword `shuffle` is `True`, the HDF5 shuffle filter
@@ -3329,17 +3346,18 @@
         for var in _vars.values():
             var.set_ncstring_attrs(value)
 
         for groups in _walk_grps(self):
             for group in groups:
                 group.set_ncstring_attrs(value) # recurse into subgroups...
 
+    @functools.lru_cache(maxsize=128)
     def get_variables_by_attributes(self, **kwargs):
         """
-**`get_variables_by_attribute(self, **kwargs)`**
+**`get_variables_by_attributes(self, **kwargs)`**
 
 Returns a list of variables that match specific conditions.
 
 Can pass in key=value parameters and variables are returned that
 contain all of the matches. For example,
 
 ```python
@@ -3418,23 +3436,23 @@
 suffix replaced by `.nc` is used..
 
 **`mode`**:  Access mode to open Dataset (Default `'a'`).
 
 **`format`**: underlying file format to use (one of `'NETCDF4',
 'NETCDF4_CLASSIC', 'NETCDF3_CLASSIC'`, `'NETCDF3_64BIT_OFFSET'` or
 `'NETCDF3_64BIT_DATA'`. Default `'NETCDF4'`.
-       
+
 Dataset instance for `ncfilename` is returned.
- 
+
 [ncgen]: https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_utilities_guide.html#ncgen_guide
 [cdl]: https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_utilities_guide.html#cdl_guide
         """
         if ncfilename is None:
             filepath = pathlib.Path(cdlfilename)
-            ncfilename = filepath.with_suffix('.nc') 
+            ncfilename = filepath.with_suffix('.nc')
         formatcodes = {'NETCDF4': 4,
                        'NETCDF4_CLASSIC': 7,
                        'NETCDF3_CLASSIC': 3,
                        'NETCDF3_64BIT': 6, # legacy
                        'NETCDF3_64BIT_OFFSET': 6,
                        'NETCDF3_64BIT_DATA': 5}
         if format not in formatcodes:
@@ -3820,21 +3838,21 @@
 **`significant_digits`**: New in version 1.6.0. Describes the number of significant
 digits in the data the contains a reliable value.  Data is
 truncated to retain this number of significant digits when it is assigned to the
 `Variable` instance. If `None`, the data is not truncated.
 Only available with netcdf-c >= 4.9.0,
 and only works with `NETCDF4` or `NETCDF4_CLASSIC` formatted files.
 The number of significant digits used in the quantization of variable data can be
-obtained using the `Variable.significant_digits` method. Default `None` - 
+obtained using the `Variable.significant_digits` method. Default `None` -
 no quantization done.
 
 **`quantize_mode`**: New in version 1.6.0. Controls
 the quantization algorithm (default 'BitGroom', 'BitRound' and
 'GranularBitRound' also available).  The 'GranularBitRound'
-algorithm may result in better compression for typical geophysical datasets. 
+algorithm may result in better compression for typical geophysical datasets.
 Ignored if `significant_digits` not specified. If 'BitRound' is used, then
 `significant_digits` is interpreted as binary (not decimal) digits.
 
 **`__orthogonal_indexing__`**: Always `True`.  Indicates to client code
 that the object supports 'orthogonal indexing', which means that slices
 that are 1d arrays or lists slice along each dimension independently.  This
 behavior is similar to Fortran or Matlab, but different than numpy.
@@ -3850,15 +3868,15 @@
     cdef public _name, ndim, dtype, mask, scale, always_mask, chartostring,  _isprimitive, \
     _iscompound, _isvlen, _isenum, _grp, _cmptype, _vltype, _enumtype,\
     __orthogonal_indexing__, _has_lsd, _use_get_vars, _ncstring_attrs__
 
     def __init__(self, grp, name, datatype, dimensions=(),
             compression=None, zlib=False,
             complevel=4, shuffle=True, szip_coding='nn', szip_pixels_per_block=8,
-            blosc_shuffle=1, 
+            blosc_shuffle=1,
             fletcher32=False, contiguous=False,
             chunksizes=None, endian='native', least_significant_digit=None,
             significant_digits=None,quantize_mode='BitGroom',fill_value=None, chunk_cache=None, **kwargs):
         """
         **`__init__(self, group, name, datatype, dimensions=(), compression=None, zlib=False,
         complevel=4, shuffle=True, szip_coding='nn', szip_pixels_per_block=8,
         blosc_shuffle=1, fletcher32=False, contiguous=False,
@@ -3890,15 +3908,15 @@
         (for a variable-length string array). Numpy string and unicode datatypes with
         length greater than one are aliases for `str`.
 
         **`dimensions`**: a tuple containing the variable's Dimension instances
         (defined previously with `createDimension`). Default is an empty tuple
         which means the variable is a scalar (and therefore has no dimensions).
 
-        **`compression`**: compression algorithm to use. 
+        **`compression`**: compression algorithm to use.
         Currently `zlib`,`szip`,`zstd`,`bzip2`,`blosc_lz`,`blosc_lz4`,`blosc_lz4hc`,
         `blosc_zlib` and `blosc_zstd` are supported.
         Default is `None` (no compression).  All of the compressors except
         `zlib` and `szip` use the HDF5 plugin architecture.
 
         **`zlib`**: if `True`, data assigned to the `Variable`
         instance is compressed on disk. Default `False`. Deprecated - use
@@ -3916,15 +3934,15 @@
         Can be 0 (no blosc shuffle), 1 (bytewise shuffle) or 2 (bitwise
         shuffle)). Default is 1. Ignored if blosc compressor not used.
 
         **`szip_coding`**: szip coding method. Can be `ec` (entropy coding)
         or `nn` (nearest neighbor coding). Default is `nn`.
         Ignored if szip compressor not used.
 
-        **`szip_pixels_per_block`**: Can be 4,8,16 or 32 (Default 8). 
+        **`szip_pixels_per_block`**: Can be 4,8,16 or 32 (Default 8).
         Ignored if szip compressor not used.
 
         **`fletcher32`**: if `True` (default `False`), the Fletcher32 checksum
         algorithm is used for error detection.
 
         **`contiguous`**: if `True` (default `False`), the variable data is
         stored contiguously on disk.  Default `False`. Setting to `True` for
@@ -3997,15 +4015,15 @@
         cdef nc_type xtype
         cdef int *dimids
         cdef size_t sizep, nelemsp
         cdef size_t *chunksizesp
         cdef float preemptionp
         # flag to indicate that orthogonal indexing is supported
         self.__orthogonal_indexing__ = True
-        # For backwards compatibility, deprecated zlib kwarg takes 
+        # For backwards compatibility, deprecated zlib kwarg takes
         # precedence if compression kwarg not set.
         if zlib and not compression:
             compression = 'zlib'
         # if complevel is set to zero, turn off compression
         if not complevel:
             compression = None
         zlib = False
@@ -4496,15 +4514,15 @@
         def __get__(self):
             return self._getname()
         def __set__(self,value):
             raise AttributeError("name cannot be altered")
 
     property datatype:
         """numpy data type (for primitive data types) or
-        VLType/CompoundType/EnumType instance 
+        VLType/CompoundType/EnumType instance
         (for compound, vlen  or enum data types)"""
         def __get__(self):
             if self._iscompound:
                 return self._cmptype
             elif self._isvlen:
                 return self._vltype
             elif self._isenum:
@@ -4636,16 +4654,16 @@
         cdef int ierr,ideflate,ishuffle,icomplevel,ifletcher32
         cdef int izstd=0
         cdef int ibzip2=0
         cdef int iblosc=0
         cdef int iszip=0
         cdef int iszip_coding=0
         cdef int iszip_pixels_per_block=0
-        cdef int icomplevel_zstd=0 
-        cdef int icomplevel_bzip2=0 
+        cdef int icomplevel_zstd=0
+        cdef int icomplevel_bzip2=0
         cdef unsigned int iblosc_shuffle=0
         cdef unsigned int iblosc_compressor=0
         cdef unsigned int iblosc_blocksize=0
         cdef unsigned int iblosc_complevel=0
         filtdict = {'zlib':False,'szip':False,'zstd':False,'bzip2':False,'blosc':False,'shuffle':False,'complevel':0,'fletcher32':False}
         if self._grp.data_model not in ['NETCDF4_CLASSIC','NETCDF4']: return
         with nogil:
@@ -5568,15 +5586,15 @@
 for each data type). If the variable has no missing_value attribute, the
 _FillValue is used instead. If the variable has valid_min/valid_max and
 missing_value attributes, data outside the specified range will be masked.
 When data is written to a variable, the masked
 array is converted back to a regular numpy array by replacing all the
 masked values by the missing_value attribute of the variable (if it
 exists).  If the variable has no missing_value attribute, the _FillValue
-is used instead. 
+is used instead.
 
 If `maskandscale` is set to `True`, and the variable has a
 `scale_factor` or an `add_offset` attribute, then data read
 from that variable is unpacked using::
 
     data = self.scale_factor*data + self.add_offset
 
@@ -5658,15 +5676,15 @@
 for each data type). If the variable has no missing_value attribute, the
 _FillValue is used instead. If the variable has valid_min/valid_max and
 missing_value attributes, data outside the specified range will be masked.
 When data is written to a variable, the masked
 array is converted back to a regular numpy array by replacing all the
 masked values by the missing_value attribute of the variable (if it
 exists).  If the variable has no missing_value attribute, the _FillValue
-is used instead. 
+is used instead.
 
 The default value of `mask` is `True`
 (automatic conversions are performed).
         """
         self.mask = bool(mask)
 
     def set_always_mask(self,always_mask):
@@ -6926,14 +6944,22 @@
         **`close(self)`**
 
         close all the open files.
         """
         for dset in self._cdf:
             dset.close()
 
+    def isopen(self):
+        """
+        **`isopen(self)`**
+
+        True if all files are open, False otherwise.
+        """
+        return all(map(lambda dset: dset.isopen(), self._cdf))
+
     def __repr__(self):
         ncdump = [repr(type(self))]
         dimnames = tuple(str(dimname) for dimname in self.dimensions.keys())
         varnames = tuple(str(varname) for varname in self.variables.keys())
         grpnames = ()
         if self.path == '/':
             ncdump.append('root group (%s data model, file format %s):' %
```

### Comparing `netCDF4-1.6.3/src/netCDF4/utils.py` & `netCDF4-1.6.4/src/netCDF4/utils.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/src/netCDF4.egg-info/PKG-INFO` & `netCDF4-1.6.4/src/netCDF4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netCDF4
-Version: 1.6.3
+Version: 1.6.4
 Summary: Provides an object-oriented python interface to the netCDF version 4 library
 Author-email: Jeff Whitaker <jeffrey.s.whitaker@noaa.gov>
 License: MIT
 Project-URL: Documentation, https://unidata.github.io/netcdf4-python/
 Project-URL: Repository, https://github.com/Unidata/netcdf4-python
 Keywords: numpy,netcdf,data,science,network,oceanography,meteorology,climate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netCDF4-1.6.3/src/netCDF4.egg-info/SOURCES.txt` & `netCDF4-1.6.4/src/netCDF4.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 test/tst_masked2.py
 test/tst_masked3.py
 test/tst_masked4.py
 test/tst_masked5.py
 test/tst_masked6.py
 test/tst_multifile.py
 test/tst_multifile2.py
+test/tst_multiple_open_close.py
 test/tst_open_mem.py
 test/tst_refcount.py
 test/tst_rename.py
 test/tst_scalarvar.py
 test/tst_scaled.py
 test/tst_shape.py
 test/tst_slicing.py
```

### Comparing `netCDF4-1.6.3/test/20171025_2056.Cloud_Top_Height.nc` & `netCDF4-1.6.4/test/20171025_2056.Cloud_Top_Height.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/CRM032_test1.nc` & `netCDF4-1.6.4/test/CRM032_test1.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/issue1152.nc` & `netCDF4-1.6.4/test/issue1152.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/issue671.nc` & `netCDF4-1.6.4/test/issue671.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/issue672.nc` & `netCDF4-1.6.4/test/issue672.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/netcdf_dummy_file.nc` & `netCDF4-1.6.4/test/netcdf_dummy_file.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/run_all.py` & `netCDF4-1.6.4/test/run_all.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,19 @@
     test_files.insert(0,'tst_dap.py')
 
 # Don't run CDL test (that requires ncdump/ncgen)
 if os.getenv('NO_CDL'):
     test_files.remove('tst_cdl.py');
     sys.stdout.write('not running tst_cdl.py ...\n')
 
+# Don't run computationally intensive test
+if not os.getenv('MEMORY_LEAK_TEST'):
+    test_files.remove('tst_multiple_open_close.py');
+    sys.stdout.write('not running tst_multiple_open_close.py ...\n')
+
 # Build the test suite from the tests found in the test files.
 testsuite = unittest.TestSuite()
 for f in test_files:
     m = __import__(os.path.splitext(f)[0])
     testsuite.addTests(unittest.TestLoader().loadTestsFromModule(m))
 
 # Run the test suite.
```

### Comparing `netCDF4-1.6.3/test/test_gold.nc` & `netCDF4-1.6.4/test/test_gold.nc`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_Unsigned.py` & `netCDF4-1.6.4/test/tst_Unsigned.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_alignment.py` & `netCDF4-1.6.4/test/tst_alignment.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_atts.py` & `netCDF4-1.6.4/test/tst_atts.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_cdf5.py` & `netCDF4-1.6.4/test/tst_cdf5.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_cdl.py` & `netCDF4-1.6.4/test/tst_cdl.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_chunk_cache.py` & `netCDF4-1.6.4/test/tst_chunk_cache.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compound_alignment.py` & `netCDF4-1.6.4/test/tst_compound_alignment.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compoundatt.py` & `netCDF4-1.6.4/test/tst_compoundatt.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compoundvar.py` & `netCDF4-1.6.4/test/tst_compoundvar.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compression.py` & `netCDF4-1.6.4/test/tst_compression.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compression_blosc.py` & `netCDF4-1.6.4/test/tst_compression_blosc.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compression_bzip2.py` & `netCDF4-1.6.4/test/tst_compression_bzip2.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compression_quant.py` & `netCDF4-1.6.4/test/tst_compression_quant.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compression_szip.py` & `netCDF4-1.6.4/test/tst_compression_szip.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_compression_zstd.py` & `netCDF4-1.6.4/test/tst_compression_zstd.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_create_mem.py` & `netCDF4-1.6.4/test/tst_create_mem.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_dap.py` & `netCDF4-1.6.4/test/tst_dap.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 from datetime import datetime, timedelta
 from numpy.testing import assert_array_almost_equal
 
 # test accessing data over http with opendap.
 
 yesterday = datetime.utcnow() - timedelta(days=1)
-URL = "http://nomads.ncep.noaa.gov/dods/gfs_1p00/gfs%s/gfs_1p00_00z" % yesterday.strftime('%Y%m%d')
-URL_https = 'https://podaac-opendap.jpl.nasa.gov/opendap/allData/modis/L3/aqua/11um/v2019.0/4km/daily/2017/365/AQUA_MODIS.20171231.L3m.DAY.NSST.sst.4km.nc'
+URL = f'http://nomads.ncep.noaa.gov/dods/gfs_1p00/gfs{yesterday:%Y%m%d}/gfs_1p00_00z'
+URL_https = 'https://www.neracoos.org/erddap/griddap/WW3_EastCoast_latest'
 varname = 'hgtsfc'
 data_min = -40; data_max = 5900
 varshape = (181, 360)
 
 class DapTestCase(unittest.TestCase):
 
     def setUp(self):
@@ -29,12 +29,12 @@
         data = var[0,...]
         assert data.shape == varshape
         assert(np.abs(data.min()-data_min) < 10)
         assert(np.abs(data.max()-data_max) < 100)
         ncfile.close()
         # test https support (linked curl lib must built with openssl support)
         ncfile = netCDF4.Dataset(URL_https)
-        assert(ncfile['sst'].long_name=='Sea Surface Temperature')    
+        assert(ncfile['hs'].long_name=='Significant Wave Height')
         ncfile.close()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `netCDF4-1.6.3/test/tst_dims.py` & `netCDF4-1.6.4/test/tst_dims.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_diskless.py` & `netCDF4-1.6.4/test/tst_diskless.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_endian.py` & `netCDF4-1.6.4/test/tst_endian.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_enum.py` & `netCDF4-1.6.4/test/tst_enum.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_fancyslicing.py` & `netCDF4-1.6.4/test/tst_fancyslicing.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_filepath.py` & `netCDF4-1.6.4/test/tst_filepath.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_get_variables_by_attributes.py` & `netCDF4-1.6.4/test/tst_get_variables_by_attributes.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_grps.py` & `netCDF4-1.6.4/test/tst_grps.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_grps2.py` & `netCDF4-1.6.4/test/tst_grps2.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_masked.py` & `netCDF4-1.6.4/test/tst_masked.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_masked2.py` & `netCDF4-1.6.4/test/tst_masked2.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_masked3.py` & `netCDF4-1.6.4/test/tst_masked3.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_masked4.py` & `netCDF4-1.6.4/test/tst_masked4.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_masked5.py` & `netCDF4-1.6.4/test/tst_masked5.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_masked6.py` & `netCDF4-1.6.4/test/tst_masked6.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_multifile.py` & `netCDF4-1.6.4/test/tst_multifile.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,17 @@
         varin = f.variables['data']
         assert_array_equal(varin[4:-4:4,3:5,2:8],data2[4:-4:4,3:5,2:8])
         f.close()
         # testing multi-file get_variables_by_attributes
         f = MFDataset(self.files,check=True)
         assert f.get_variables_by_attributes(axis='T') == []
         f.get_variables_by_attributes(units='zlotys')[0] == f['x']
+        assert f.isopen()
         f.close()
+        assert not f.isopen()
 
 class NonuniformTimeTestCase(unittest.TestCase):
     ninc = 365
     def setUp(self):
 
         self.files = [tempfile.NamedTemporaryFile(suffix='.nc', delete=False).name for nfile in range(2)]
         for nfile,file in enumerate(self.files):
```

### Comparing `netCDF4-1.6.3/test/tst_multifile2.py` & `netCDF4-1.6.4/test/tst_multifile2.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_open_mem.py` & `netCDF4-1.6.4/test/tst_open_mem.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_refcount.py` & `netCDF4-1.6.4/test/tst_refcount.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_rename.py` & `netCDF4-1.6.4/test/tst_rename.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_scalarvar.py` & `netCDF4-1.6.4/test/tst_scalarvar.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_scaled.py` & `netCDF4-1.6.4/test/tst_scaled.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_shape.py` & `netCDF4-1.6.4/test/tst_shape.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_slicing.py` & `netCDF4-1.6.4/test/tst_slicing.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_stringarr.py` & `netCDF4-1.6.4/test/tst_stringarr.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_types.py` & `netCDF4-1.6.4/test/tst_types.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_unicode.py` & `netCDF4-1.6.4/test/tst_unicode.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_unicodeatt.py` & `netCDF4-1.6.4/test/tst_unicodeatt.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_unlimdim.py` & `netCDF4-1.6.4/test/tst_unlimdim.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_utils.py` & `netCDF4-1.6.4/test/tst_utils.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_vars.py` & `netCDF4-1.6.4/test/tst_vars.py`

 * *Files identical despite different names*

### Comparing `netCDF4-1.6.3/test/tst_vlen.py` & `netCDF4-1.6.4/test/tst_vlen.py`

 * *Files identical despite different names*

