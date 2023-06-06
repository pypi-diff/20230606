# Comparing `tmp/cle-9.2.8.tar.gz` & `tmp/cle-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cle-9.2.8.tar", last modified: Tue Jun 28 17:02:30 2022, max compression
+gzip compressed data, was "cle-9.2.9.tar", last modified: Tue Jul  5 17:02:19 2022, max compression
```

## Comparing `cle-9.2.8.tar` & `cle-9.2.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.012376 cle-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-06-28 17:01:16.000000 cle-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-06-28 17:01:16.000000 cle-9.2.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     4920 2022-06-28 17:02:30.012376 cle-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     4478 2022-06-28 17:01:16.000000 cle-9.2.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.000375 cle-9.2.8/cle/
--rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-06-28 17:01:36.000000 cle-9.2.8/cle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2669 2022-06-28 17:01:16.000000 cle-9.2.8/cle/address_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.004375 cle-9.2.8/cle/backends/
--rw-r--r--   0 vsts      (1001) docker     (121)    20073 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9502 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/binja.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3691 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/blob.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.004375 cle-9.2.8/cle/backends/cgc/
--rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/cgc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3009 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/cgc/backedcgc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1352 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/cgc/cgc.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.004375 cle-9.2.8/cle/backends/elf/
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      619 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/compilation_unit.py
--rw-r--r--   0 vsts      (1001) docker     (121)    58527 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/elf.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22467 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/elfcore.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4088 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/hashtable.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6268 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/lsda.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19627 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/metaelf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2289 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/regions.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/elf/relocation/
--rw-r--r--   0 vsts      (1001) docker     (121)     1417 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/amd64.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14355 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/arm.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3003 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/arm64.py
--rw-r--r--   0 vsts      (1001) docker     (121)       97 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/arm_cortex_m.py
--rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/armel.py
--rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/armhf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      805 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/elfreloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6671 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/generic.py
--rw-r--r--   0 vsts      (1001) docker     (121)      718 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/i386.py
--rw-r--r--   0 vsts      (1001) docker     (121)      951 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/mips.py
--rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/mips64.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4448 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/pcc64.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8832 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/ppc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      475 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/relocation/s390x.py
--rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/subprogram.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2415 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/symbol.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5506 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/symbol_type.py
--rw-r--r--   0 vsts      (1001) docker     (121)      586 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/variable.py
--rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/elf/variable_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/externs/
--rw-r--r--   0 vsts      (1001) docker     (121)    10298 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/externs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/externs/simdata/
--rw-r--r--   0 vsts      (1001) docker     (121)     2500 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/externs/simdata/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3338 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/externs/simdata/common.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2362 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/externs/simdata/glibc_startup.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3425 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/externs/simdata/io_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5750 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/ihex.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/java/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/java/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4080 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/java/android_lifecycle.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10142 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/java/apk.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3125 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/java/jar.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7185 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/java/soot.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/macho/
--rw-r--r--   0 vsts      (1001) docker     (121)      211 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16618 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/binding.py
--rw-r--r--   0 vsts      (1001) docker     (121)    40533 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/macho.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1801 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/macho_load_commands.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3027 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/section.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2180 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/segment.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13910 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/structs.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12199 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/macho/symbol.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/minidump/
--rw-r--r--   0 vsts      (1001) docker     (121)     6446 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/minidump/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2401 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/named_region.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/pe/
--rw-r--r--   0 vsts      (1001) docker     (121)       19 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11526 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/pe.py
--rw-r--r--   0 vsts      (1001) docker     (121)      910 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/regions.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.008376 cle-9.2.8/cle/backends/pe/relocation/
--rw-r--r--   0 vsts      (1001) docker     (121)     1415 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      443 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/amd64.py
--rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/arm.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2968 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/generic.py
--rw-r--r--   0 vsts      (1001) docker     (121)      441 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/i386.py
--rw-r--r--   0 vsts      (1001) docker     (121)      583 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/mips.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2142 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/pereloc.py
--rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/relocation/riscv.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1239 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/pe/symbol.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5646 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/region.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5032 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/regions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5039 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/relocation.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1568 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/static_archive.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4274 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/symbol.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.012376 cle-9.2.8/cle/backends/tls/
--rw-r--r--   0 vsts      (1001) docker     (121)     2309 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/tls/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6302 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/tls/elf_tls.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1755 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/tls/elfcore_tls.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1303 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/tls/minidump_tls.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4786 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/tls/pe_tls.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3851 2022-06-28 17:01:16.000000 cle-9.2.8/cle/backends/xbe.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1075 2022-06-28 17:01:16.000000 cle-9.2.8/cle/errors.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3605 2022-06-28 17:01:16.000000 cle-9.2.8/cle/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (121)    50620 2022-06-28 17:01:16.000000 cle-9.2.8/cle/loader.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21543 2022-06-28 17:01:16.000000 cle-9.2.8/cle/memory.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-06-28 17:01:16.000000 cle-9.2.8/cle/patched_stream.py
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-06-28 17:01:16.000000 cle-9.2.8/cle/py.typed
--rw-r--r--   0 vsts      (1001) docker     (121)     3681 2022-06-28 17:01:16.000000 cle-9.2.8/cle/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:30.004375 cle-9.2.8/cle.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4920 2022-06-28 17:02:29.000000 cle-9.2.8/cle.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2798 2022-06-28 17:02:29.000000 cle-9.2.8/cle.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:02:29.000000 cle-9.2.8/cle.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      142 2022-06-28 17:02:29.000000 cle-9.2.8/cle.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        4 2022-06-28 17:02:29.000000 cle-9.2.8/cle.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       98 2022-06-28 17:01:36.000000 cle-9.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      874 2022-06-28 17:02:30.012376 cle-9.2.8/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.493122 cle-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-07-05 17:01:18.000000 cle-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-07-05 17:01:18.000000 cle-9.2.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     4920 2022-07-05 17:02:19.493122 cle-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     4478 2022-07-05 17:01:18.000000 cle-9.2.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.481122 cle-9.2.9/cle/
+-rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-07-05 17:01:36.000000 cle-9.2.9/cle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2669 2022-07-05 17:01:18.000000 cle-9.2.9/cle/address_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.481122 cle-9.2.9/cle/backends/
+-rw-r--r--   0 vsts      (1001) docker     (121)    20073 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9502 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/binja.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3691 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/blob.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.485122 cle-9.2.9/cle/backends/cgc/
+-rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/cgc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3009 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/cgc/backedcgc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1352 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/cgc/cgc.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.485122 cle-9.2.9/cle/backends/elf/
+-rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      619 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/compilation_unit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    58527 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/elf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22467 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/elfcore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4088 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/hashtable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6268 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/lsda.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19627 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/metaelf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2289 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/regions.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.485122 cle-9.2.9/cle/backends/elf/relocation/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1417 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14355 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/arm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3003 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/arm64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       97 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/arm_cortex_m.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/armel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/armhf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      805 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/elfreloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6671 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/generic.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      718 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/i386.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      951 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/mips.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/mips64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4448 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/pcc64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8832 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/ppc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      475 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/relocation/s390x.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/subprogram.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2415 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/symbol.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5506 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/symbol_type.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      586 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/variable.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/elf/variable_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.489122 cle-9.2.9/cle/backends/externs/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10298 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/externs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.489122 cle-9.2.9/cle/backends/externs/simdata/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2500 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/externs/simdata/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3338 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/externs/simdata/common.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2362 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/externs/simdata/glibc_startup.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3425 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/externs/simdata/io_file.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5750 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/ihex.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.489122 cle-9.2.9/cle/backends/java/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/java/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4080 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/java/android_lifecycle.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10142 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/java/apk.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3125 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/java/jar.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7185 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/java/soot.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.489122 cle-9.2.9/cle/backends/macho/
+-rw-r--r--   0 vsts      (1001) docker     (121)      211 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16618 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/binding.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    40533 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/macho.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1801 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/macho_load_commands.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3027 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/section.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2180 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/segment.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13910 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/structs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12199 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/macho/symbol.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.489122 cle-9.2.9/cle/backends/minidump/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6446 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/minidump/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2401 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/named_region.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.489122 cle-9.2.9/cle/backends/pe/
+-rw-r--r--   0 vsts      (1001) docker     (121)       19 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11526 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      910 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/regions.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.493122 cle-9.2.9/cle/backends/pe/relocation/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1415 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      443 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/arm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2968 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/generic.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      441 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/i386.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      583 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/mips.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2142 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/pereloc.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/relocation/riscv.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1239 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/pe/symbol.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5646 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/region.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5032 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/regions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5039 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/relocation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1568 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/static_archive.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4274 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/symbol.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.493122 cle-9.2.9/cle/backends/tls/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2309 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/tls/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6302 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/tls/elf_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1755 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/tls/elfcore_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1303 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/tls/minidump_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4786 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/tls/pe_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3851 2022-07-05 17:01:18.000000 cle-9.2.9/cle/backends/xbe.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1075 2022-07-05 17:01:18.000000 cle-9.2.9/cle/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3605 2022-07-05 17:01:18.000000 cle-9.2.9/cle/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    50620 2022-07-05 17:01:18.000000 cle-9.2.9/cle/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21543 2022-07-05 17:01:18.000000 cle-9.2.9/cle/memory.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-05 17:01:18.000000 cle-9.2.9/cle/patched_stream.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-07-05 17:01:18.000000 cle-9.2.9/cle/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (121)     3681 2022-07-05 17:01:18.000000 cle-9.2.9/cle/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:19.481122 cle-9.2.9/cle.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4920 2022-07-05 17:02:19.000000 cle-9.2.9/cle.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2798 2022-07-05 17:02:19.000000 cle-9.2.9/cle.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:02:19.000000 cle-9.2.9/cle.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      142 2022-07-05 17:02:19.000000 cle-9.2.9/cle.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        4 2022-07-05 17:02:19.000000 cle-9.2.9/cle.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       98 2022-07-05 17:01:36.000000 cle-9.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)      874 2022-07-05 17:02:19.493122 cle-9.2.9/setup.cfg
```

### Comparing `cle-9.2.8/LICENSE` & `cle-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/PKG-INFO` & `cle-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cle
-Version: 9.2.8
+Version: 9.2.9
 Summary: |
 Home-page: https://github.com/angr/cle
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `cle-9.2.8/README.md` & `cle-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/__init__.py` & `cle-9.2.9/cle/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 CLE is an extensible binary loader. Its main goal is to take an executable program and any libraries it depends on and
 produce an address space where that program is loaded and ready to run.
 
 The primary interface to CLE is the Loader class.
 """
 
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 if bytes is str:
     raise Exception("This module is designed for python 3 only. Please install an older version to use python 2.")
 
 import logging
 logging.getLogger(name=__name__).addHandler(logging.NullHandler())
```

### Comparing `cle-9.2.8/cle/address_translator.py` & `cle-9.2.9/cle/address_translator.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/__init__.py` & `cle-9.2.9/cle/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/binja.py` & `cle-9.2.9/cle/backends/binja.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/blob.py` & `cle-9.2.9/cle/backends/blob.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/cgc/backedcgc.py` & `cle-9.2.9/cle/backends/cgc/backedcgc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/cgc/cgc.py` & `cle-9.2.9/cle/backends/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/compilation_unit.py` & `cle-9.2.9/cle/backends/elf/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/elf.py` & `cle-9.2.9/cle/backends/elf/elf.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/elfcore.py` & `cle-9.2.9/cle/backends/elf/elfcore.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/hashtable.py` & `cle-9.2.9/cle/backends/elf/hashtable.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/lsda.py` & `cle-9.2.9/cle/backends/elf/lsda.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/metaelf.py` & `cle-9.2.9/cle/backends/elf/metaelf.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/regions.py` & `cle-9.2.9/cle/backends/elf/regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/__init__.py` & `cle-9.2.9/cle/backends/elf/relocation/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/amd64.py` & `cle-9.2.9/cle/backends/elf/relocation/amd64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/arm.py` & `cle-9.2.9/cle/backends/elf/relocation/arm.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/arm64.py` & `cle-9.2.9/cle/backends/elf/relocation/arm64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/elfreloc.py` & `cle-9.2.9/cle/backends/elf/relocation/elfreloc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/generic.py` & `cle-9.2.9/cle/backends/elf/relocation/generic.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/i386.py` & `cle-9.2.9/cle/backends/elf/relocation/i386.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/mips.py` & `cle-9.2.9/cle/backends/elf/relocation/mips.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/pcc64.py` & `cle-9.2.9/cle/backends/elf/relocation/pcc64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/relocation/ppc.py` & `cle-9.2.9/cle/backends/elf/relocation/ppc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/symbol.py` & `cle-9.2.9/cle/backends/elf/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/symbol_type.py` & `cle-9.2.9/cle/backends/elf/symbol_type.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/variable.py` & `cle-9.2.9/cle/backends/elf/variable.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/elf/variable_type.py` & `cle-9.2.9/cle/backends/elf/variable_type.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/externs/__init__.py` & `cle-9.2.9/cle/backends/externs/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/externs/simdata/__init__.py` & `cle-9.2.9/cle/backends/externs/simdata/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/externs/simdata/common.py` & `cle-9.2.9/cle/backends/externs/simdata/common.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/externs/simdata/glibc_startup.py` & `cle-9.2.9/cle/backends/externs/simdata/glibc_startup.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/externs/simdata/io_file.py` & `cle-9.2.9/cle/backends/externs/simdata/io_file.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/ihex.py` & `cle-9.2.9/cle/backends/ihex.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/java/android_lifecycle.py` & `cle-9.2.9/cle/backends/java/android_lifecycle.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/java/apk.py` & `cle-9.2.9/cle/backends/java/apk.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/java/jar.py` & `cle-9.2.9/cle/backends/java/jar.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/java/soot.py` & `cle-9.2.9/cle/backends/java/soot.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/binding.py` & `cle-9.2.9/cle/backends/macho/binding.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/macho.py` & `cle-9.2.9/cle/backends/macho/macho.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/macho_load_commands.py` & `cle-9.2.9/cle/backends/macho/macho_load_commands.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/section.py` & `cle-9.2.9/cle/backends/macho/section.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/segment.py` & `cle-9.2.9/cle/backends/macho/segment.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/structs.py` & `cle-9.2.9/cle/backends/macho/structs.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/macho/symbol.py` & `cle-9.2.9/cle/backends/macho/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/minidump/__init__.py` & `cle-9.2.9/cle/backends/minidump/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/named_region.py` & `cle-9.2.9/cle/backends/named_region.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/pe.py` & `cle-9.2.9/cle/backends/pe/pe.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/regions.py` & `cle-9.2.9/cle/backends/pe/regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/relocation/__init__.py` & `cle-9.2.9/cle/backends/pe/relocation/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/relocation/arm.py` & `cle-9.2.9/cle/backends/pe/relocation/arm.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/relocation/generic.py` & `cle-9.2.9/cle/backends/pe/relocation/generic.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/relocation/mips.py` & `cle-9.2.9/cle/backends/pe/relocation/mips.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/relocation/pereloc.py` & `cle-9.2.9/cle/backends/pe/relocation/pereloc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/relocation/riscv.py` & `cle-9.2.9/cle/backends/pe/relocation/riscv.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/pe/symbol.py` & `cle-9.2.9/cle/backends/pe/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/region.py` & `cle-9.2.9/cle/backends/region.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/regions.py` & `cle-9.2.9/cle/backends/regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/relocation.py` & `cle-9.2.9/cle/backends/relocation.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/static_archive.py` & `cle-9.2.9/cle/backends/static_archive.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/symbol.py` & `cle-9.2.9/cle/backends/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/tls/__init__.py` & `cle-9.2.9/cle/backends/tls/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/tls/elf_tls.py` & `cle-9.2.9/cle/backends/tls/elf_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/tls/elfcore_tls.py` & `cle-9.2.9/cle/backends/tls/elfcore_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/tls/minidump_tls.py` & `cle-9.2.9/cle/backends/tls/minidump_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/tls/pe_tls.py` & `cle-9.2.9/cle/backends/tls/pe_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/backends/xbe.py` & `cle-9.2.9/cle/backends/xbe.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/errors.py` & `cle-9.2.9/cle/errors.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/gdb.py` & `cle-9.2.9/cle/gdb.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/loader.py` & `cle-9.2.9/cle/loader.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/memory.py` & `cle-9.2.9/cle/memory.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/patched_stream.py` & `cle-9.2.9/cle/patched_stream.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle/utils.py` & `cle-9.2.9/cle/utils.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/cle.egg-info/PKG-INFO` & `cle-9.2.9/cle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cle
-Version: 9.2.8
+Version: 9.2.9
 Summary: |
 Home-page: https://github.com/angr/cle
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `cle-9.2.8/cle.egg-info/SOURCES.txt` & `cle-9.2.9/cle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cle-9.2.8/setup.cfg` & `cle-9.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	memory.
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 install_requires = 
 	pyelftools >= 0.27
-	pyvex == 9.2.8
+	pyvex == 9.2.9
 	pefile
 	sortedcontainers >= 2.0
 python_requires = >= 3.8
 packages = find:
 tests_require = cffi
 
 [options.extras_require]
```

