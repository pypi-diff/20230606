# Comparing `tmp/pyvex-9.2.8.tar.gz` & `tmp/pyvex-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvex-9.2.8.tar", last modified: Tue Jun 28 17:02:15 2022, max compression
+gzip compressed data, was "pyvex-9.2.9.tar", last modified: Tue Jul  5 17:02:09 2022, max compression
```

## Comparing `pyvex-9.2.8.tar` & `pyvex-9.2.9.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.834912 pyvex-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-06-28 17:01:14.000000 pyvex-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      149 2022-06-28 17:01:14.000000 pyvex-9.2.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     8892 2022-06-28 17:02:15.834912 pyvex-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     8473 2022-06-28 17:01:14.000000 pyvex-9.2.8/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5185 2022-06-28 17:01:14.000000 pyvex-9.2.8/make_ffi.py
--rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-06-28 17:01:36.000000 pyvex-9.2.8/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.790907 pyvex-9.2.8/pyvex/
--rw-r--r--   0 vsts      (1001) docker     (121)     3004 2022-06-28 17:01:36.000000 pyvex-9.2.8/pyvex/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24074 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/block.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9436 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/const.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1759 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/data_ref.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4434 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/enums.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1191 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/errors.py
--rw-r--r--   0 vsts      (1001) docker     (121)    26298 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/expr.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.790907 pyvex-9.2.8/pyvex/lifting/
--rw-r--r--   0 vsts      (1001) docker     (121)    12928 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.794908 pyvex-9.2.8/pyvex/lifting/gym/
--rw-r--r--   0 vsts      (1001) docker     (121)      204 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/gym/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1298 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/gym/aarch64_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14836 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/gym/arm_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3224 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/gym/x86_spotter.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3764 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/libvex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5067 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (121)      297 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/post_processor.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.794908 pyvex-9.2.8/pyvex/lifting/util/
--rw-r--r--   0 vsts      (1001) docker     (121)      178 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17795 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/util/instr_helper.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2496 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/util/irsb_postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4916 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/util/lifter_helper.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8852 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/util/syntax_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10255 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/util/vex_helper.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2572 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/lifting/zerodivision.py
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/py.typed
--rw-r--r--   0 vsts      (1001) docker     (121)    22211 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/stmt.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1358 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.790907 pyvex-9.2.8/pyvex.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     8892 2022-06-28 17:02:15.000000 pyvex-9.2.8/pyvex.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     5469 2022-06-28 17:02:15.000000 pyvex-9.2.8/pyvex.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:02:15.000000 pyvex-9.2.8/pyvex.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       75 2022-06-28 17:02:15.000000 pyvex-9.2.8/pyvex.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-06-28 17:02:15.000000 pyvex-9.2.8/pyvex.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.794908 pyvex-9.2.8/pyvex_c/
--rw-r--r--   0 vsts      (1001) docker     (121)    35147 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     1405 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/Makefile-msvc
--rw-r--r--   0 vsts      (1001) docker     (121)    20113 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/analysis.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2765 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/e4c_lite.h
--rw-r--r--   0 vsts      (1001) docker     (121)      794 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/logging.c
--rw-r--r--   0 vsts      (1001) docker     (121)      226 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/logging.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12044 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/postprocess.c
--rw-r--r--   0 vsts      (1001) docker     (121)    10821 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/pyvex.c
--rw-r--r--   0 vsts      (1001) docker     (121)      923 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/pyvex.def
--rw-r--r--   0 vsts      (1001) docker     (121)     1689 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/pyvex.h
--rw-r--r--   0 vsts      (1001) docker     (121)      543 2022-06-28 17:01:14.000000 pyvex-9.2.8/pyvex_c/pyvex_internal.h
--rw-r--r--   0 vsts      (1001) docker     (121)      699 2022-06-28 17:02:15.838912 pyvex-9.2.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     4648 2022-06-28 17:01:14.000000 pyvex-9.2.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.794908 pyvex-9.2.8/vex/
--rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/.git
--rw-r--r--   0 vsts      (1001) docker     (121)       83 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)      176 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/HACKING.README
--rw-r--r--   0 vsts      (1001) docker     (121)    18011 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/LICENSE.GPL
--rw-r--r--   0 vsts      (1001) docker     (121)      996 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/LICENSE.README
--rw-r--r--   0 vsts      (1001) docker     (121)     5157 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/Makefile-gcc
--rw-r--r--   0 vsts      (1001) docker     (121)     1211 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/Makefile-msvc
--rw-r--r--   0 vsts      (1001) docker     (121)      133 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)     1028 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/TODO.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.794908 pyvex-9.2.8/vex/auxprogs/
--rw-r--r--   0 vsts      (1001) docker     (121)    31177 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/auxprogs/genoffsets.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2795 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/common.mk
--rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/nanoarm.orig
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.798908 pyvex-9.2.8/vex/orig_amd64/
--rw-r--r--   0 vsts      (1001) docker     (121)     1612 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_amd64/Compare.hs
--rw-r--r--   0 vsts      (1001) docker     (121)      580 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_amd64/SortedToOrig.hs
--rw-r--r--   0 vsts      (1001) docker     (121)    77851 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_amd64/test1.orig
--rw-r--r--   0 vsts      (1001) docker     (121)    64255 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_amd64/test1.sorted
--rw-r--r--   0 vsts      (1001) docker     (121)   349947 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_amd64/test2.orig
--rw-r--r--   0 vsts      (1001) docker     (121)   349312 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_amd64/test2.sorted
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.798908 pyvex-9.2.8/vex/orig_arm/
--rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_arm/nanoarm
--rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_arm/nanoarm.orig
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.802909 pyvex-9.2.8/vex/orig_ppc32/
--rw-r--r--   0 vsts      (1001) docker     (121)  3443743 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_ppc32/date.orig
--rw-r--r--   0 vsts      (1001) docker     (121)  1156810 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_ppc32/loadsafp.orig
--rw-r--r--   0 vsts      (1001) docker     (121)   212994 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_ppc32/morefp.orig
--rw-r--r--   0 vsts      (1001) docker     (121)  1511720 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_ppc32/return0.orig
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.806909 pyvex-9.2.8/vex/orig_x86/
--rw-r--r--   0 vsts      (1001) docker     (121)   420476 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_x86/exit42.orig
--rw-r--r--   0 vsts      (1001) docker     (121)   869782 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_x86/fpu_mmx_sse.orig
--rw-r--r--   0 vsts      (1001) docker     (121)   426379 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/orig_x86/manyfp.orig
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.826911 pyvex-9.2.8/vex/priv/
--rw-r--r--   0 vsts      (1001) docker     (121)    23305 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_amd64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   158770 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_amd64_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)  1196572 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_amd64_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13043 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_arm64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    68566 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_arm64_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)   552369 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_arm64_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12853 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_arm_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    50250 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_arm_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)   882026 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_arm_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)    50108 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_generic_bb_to_IR.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7961 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_generic_bb_to_IR.h
--rw-r--r--   0 vsts      (1001) docker     (121)    39860 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_generic_x87.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4929 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_generic_x87.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6065 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_mips_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29340 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_mips_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)   807179 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_mips_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6731 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_ppc_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34775 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_ppc_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)  1130268 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_ppc_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17479 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_s390_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   101697 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_s390_helpers.c
--rwxr-xr-x   0 vsts      (1001) docker     (121)    10118 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_s390_insn_formats.py
--rw-r--r--   0 vsts      (1001) docker     (121)   727610 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_s390_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4954 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_tilegx_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20766 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_tilegx_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)    79947 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_tilegx_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16605 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_x86_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   100948 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_x86_helpers.c
--rw-r--r--   0 vsts      (1001) docker     (121)   552835 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/guest_x86_toIR.c
--rw-r--r--   0 vsts      (1001) docker     (121)   145172 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_amd64_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    30093 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_amd64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   191170 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_amd64_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)   218996 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_arm64_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    37441 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_arm64_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   163347 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_arm64_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)   183248 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_arm_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    35420 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_arm_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   257988 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_arm_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11045 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_maddf.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1870 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_maddf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    60281 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_reg_alloc2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    55387 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_reg_alloc3.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11727 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_regs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17459 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_regs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13196 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_simd128.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3773 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_simd128.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2155 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_simd256.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2066 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_simd256.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43649 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_simd64.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7296 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_generic_simd64.h
--rw-r--r--   0 vsts      (1001) docker     (121)   131651 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_mips_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    26553 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_mips_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   151524 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_mips_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)   231014 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_ppc_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    43619 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_ppc_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   266473 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_ppc_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)   329366 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_s390_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    34560 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_s390_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   174718 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_s390_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)    76788 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_tilegx_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20244 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_tilegx_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    56164 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_tilegx_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)   120030 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_x86_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    26278 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_x86_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)   164986 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/host_x86_isel.c
--rw-r--r--   0 vsts      (1001) docker     (121)   190764 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/ir_defs.c
--rw-r--r--   0 vsts      (1001) docker     (121)    10919 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/ir_inject.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3802 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/ir_match.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3145 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/ir_match.h
--rw-r--r--   0 vsts      (1001) docker     (121)   230984 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/ir_opt.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2820 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/ir_opt.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/main_globals.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2803 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/main_globals.h
--rw-r--r--   0 vsts      (1001) docker     (121)    82312 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/main_main.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18330 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/main_util.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5609 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/main_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3163 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/multiarch_main_main.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6083 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/s390_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14758 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/s390_disasm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3277 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/s390_disasm.h
--rw-r--r--   0 vsts      (1001) docker     (121)   180250 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/tilegx_disasm.c
--rw-r--r--   0 vsts      (1001) docker     (121)    28210 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/priv/tilegx_disasm.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.830911 pyvex-9.2.8/vex/pub/
--rw-r--r--   0 vsts      (1001) docker     (121)    41629 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6453 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_basictypes.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4889 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_emnote.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8755 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_amd64.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7926 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_arm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6526 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_arm64.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6330 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_mips32.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6397 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_mips64.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11695 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_ppc32.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13411 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_ppc64.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7258 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_s390x.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4896 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_tilegx.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12432 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_guest_x86.h
--rw-r--r--   0 vsts      (1001) docker     (121)   122233 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_ir.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5025 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_s390x_common.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4451 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/pub/libvex_trc_values.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.830911 pyvex-9.2.8/vex/switchback/
--rw-r--r--   0 vsts      (1001) docker     (121)      257 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/Makefile
--rwxr-xr-x   0 vsts      (1001) docker     (121)     9974 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/binary_switchback.pl
--rw-r--r--   0 vsts      (1001) docker     (121)    45293 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/linker.c
--rw-r--r--   0 vsts      (1001) docker     (121)      113 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/linker.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24229 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/switchback.c
--rw-r--r--   0 vsts      (1001) docker     (121)   184904 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/test_bzip2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    53078 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/test_emfloat.c
--rw-r--r--   0 vsts      (1001) docker     (121)      286 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/test_hello.c
--rw-r--r--   0 vsts      (1001) docker     (121)   115291 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/test_ppc_jm1.c
--rw-r--r--   0 vsts      (1001) docker     (121)      180 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/switchback/test_simple.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.834912 pyvex-9.2.8/vex/test/
--rw-r--r--   0 vsts      (1001) docker     (121)      542 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fldenv.c
--rw-r--r--   0 vsts      (1001) docker     (121)      224 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fp1.c
--rw-r--r--   0 vsts      (1001) docker     (121)      792 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fp1.s
--rw-r--r--   0 vsts      (1001) docker     (121)     1572 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fpconst.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1451 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fpgames.s
--rw-r--r--   0 vsts      (1001) docker     (121)      555 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fpspeed.c
--rw-r--r--   0 vsts      (1001) docker     (121)      660 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fpucw.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1906 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/frstor.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1557 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fsave.c
--rw-r--r--   0 vsts      (1001) docker     (121)      393 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fstenv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3462 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/fxsave.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20405 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/mmxtest.c
--rw-r--r--   0 vsts      (1001) docker     (121)      694 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/mxcsr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2169 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/rounderr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2157 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-amd64-muldiv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4715 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-amd64-shift.h
--rw-r--r--   0 vsts      (1001) docker     (121)    45441 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-amd64.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6381 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-amd64.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1521 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-i386-muldiv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4022 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-i386-shift.h
--rw-r--r--   0 vsts      (1001) docker     (121)    44331 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-i386.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5372 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/test-i386.h
--rw-r--r--   0 vsts      (1001) docker     (121)      926 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/x87fxam.c
--rw-r--r--   0 vsts      (1001) docker     (121)      403 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/test/x87tst.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.834912 pyvex-9.2.8/vex/unused/
--rw-r--r--   0 vsts      (1001) docker     (121)     1593 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/unused/arena.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2502 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/unused/dispatch.c
--rw-r--r--   0 vsts      (1001) docker     (121)    43051 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/unused/linker.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:15.834912 pyvex-9.2.8/vex/useful/
--rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/Makefile-vex
--rw-r--r--   0 vsts      (1001) docker     (121)     1326 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/cpuid.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19175 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/fp_80_64.c
--rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/fpround.c
--rw-r--r--   0 vsts      (1001) docker     (121)      383 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/fspill.c
--rw-r--r--   0 vsts      (1001) docker     (121)      201 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/gradual_underflow.c
--rw-r--r--   0 vsts      (1001) docker     (121)    54111 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/hd_fpu.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4886 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/show_fp_state.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7171 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/smchash.c
--rw-r--r--   0 vsts      (1001) docker     (121)    89474 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/test_main.c
--rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/test_main.h
--rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/test_main.h.base
--rw-r--r--   0 vsts      (1001) docker     (121)     8384 2022-06-28 17:01:16.000000 pyvex-9.2.8/vex/useful/x87_to_vex_and_back.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.257102 pyvex-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-07-05 17:01:14.000000 pyvex-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      149 2022-07-05 17:01:14.000000 pyvex-9.2.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     8892 2022-07-05 17:02:09.257102 pyvex-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     8473 2022-07-05 17:01:14.000000 pyvex-9.2.9/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     5185 2022-07-05 17:01:14.000000 pyvex-9.2.9/make_ffi.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-07-05 17:01:36.000000 pyvex-9.2.9/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.205102 pyvex-9.2.9/pyvex/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3004 2022-07-05 17:01:36.000000 pyvex-9.2.9/pyvex/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24074 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9436 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/const.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1759 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/data_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4434 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1191 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26298 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/expr.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.205102 pyvex-9.2.9/pyvex/lifting/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12928 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.205102 pyvex-9.2.9/pyvex/lifting/gym/
+-rw-r--r--   0 vsts      (1001) docker     (121)      204 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/gym/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1298 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/gym/aarch64_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14836 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/gym/arm_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3224 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/gym/x86_spotter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3764 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/libvex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5067 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      297 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/post_processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.205102 pyvex-9.2.9/pyvex/lifting/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)      178 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17795 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/util/instr_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2496 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/util/irsb_postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4916 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/util/lifter_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8852 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/util/syntax_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10255 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/util/vex_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2572 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/lifting/zerodivision.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (121)    22211 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/stmt.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1358 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.205102 pyvex-9.2.9/pyvex.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8892 2022-07-05 17:02:09.000000 pyvex-9.2.9/pyvex.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     5469 2022-07-05 17:02:09.000000 pyvex-9.2.9/pyvex.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:02:09.000000 pyvex-9.2.9/pyvex.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       75 2022-07-05 17:02:09.000000 pyvex-9.2.9/pyvex.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-07-05 17:02:09.000000 pyvex-9.2.9/pyvex.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.209102 pyvex-9.2.9/pyvex_c/
+-rw-r--r--   0 vsts      (1001) docker     (121)    35147 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)     1405 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/Makefile-msvc
+-rw-r--r--   0 vsts      (1001) docker     (121)    20113 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/analysis.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2765 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/e4c_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      794 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/logging.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      226 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12044 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/postprocess.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    10821 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/pyvex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      923 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/pyvex.def
+-rw-r--r--   0 vsts      (1001) docker     (121)     1689 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/pyvex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      543 2022-07-05 17:01:14.000000 pyvex-9.2.9/pyvex_c/pyvex_internal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      699 2022-07-05 17:02:09.257102 pyvex-9.2.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)     4648 2022-07-05 17:01:14.000000 pyvex-9.2.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.209102 pyvex-9.2.9/vex/
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/.git
+-rw-r--r--   0 vsts      (1001) docker     (121)       83 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (121)      176 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/HACKING.README
+-rw-r--r--   0 vsts      (1001) docker     (121)    18011 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/LICENSE.GPL
+-rw-r--r--   0 vsts      (1001) docker     (121)      996 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/LICENSE.README
+-rw-r--r--   0 vsts      (1001) docker     (121)     5157 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/Makefile-gcc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1211 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/Makefile-msvc
+-rw-r--r--   0 vsts      (1001) docker     (121)      133 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)     1028 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/TODO.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.209102 pyvex-9.2.9/vex/auxprogs/
+-rw-r--r--   0 vsts      (1001) docker     (121)    31177 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/auxprogs/genoffsets.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2795 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/common.mk
+-rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/nanoarm.orig
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.213102 pyvex-9.2.9/vex/orig_amd64/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1612 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_amd64/Compare.hs
+-rw-r--r--   0 vsts      (1001) docker     (121)      580 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_amd64/SortedToOrig.hs
+-rw-r--r--   0 vsts      (1001) docker     (121)    77851 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_amd64/test1.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)    64255 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_amd64/test1.sorted
+-rw-r--r--   0 vsts      (1001) docker     (121)   349947 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_amd64/test2.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)   349312 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_amd64/test2.sorted
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.213102 pyvex-9.2.9/vex/orig_arm/
+-rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_arm/nanoarm
+-rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_arm/nanoarm.orig
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.217102 pyvex-9.2.9/vex/orig_ppc32/
+-rw-r--r--   0 vsts      (1001) docker     (121)  3443743 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_ppc32/date.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)  1156810 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_ppc32/loadsafp.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)   212994 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_ppc32/morefp.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)  1511720 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_ppc32/return0.orig
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.221102 pyvex-9.2.9/vex/orig_x86/
+-rw-r--r--   0 vsts      (1001) docker     (121)   420476 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_x86/exit42.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)   869782 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_x86/fpu_mmx_sse.orig
+-rw-r--r--   0 vsts      (1001) docker     (121)   426379 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/orig_x86/manyfp.orig
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.245102 pyvex-9.2.9/vex/priv/
+-rw-r--r--   0 vsts      (1001) docker     (121)    23305 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_amd64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   158770 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_amd64_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)  1196572 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_amd64_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13043 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_arm64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    68566 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_arm64_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   552369 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_arm64_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12853 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_arm_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    50250 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_arm_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   882026 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_arm_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    50108 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_generic_bb_to_IR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7961 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_generic_bb_to_IR.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    39860 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_generic_x87.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4929 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_generic_x87.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6065 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_mips_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29340 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_mips_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   807179 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_mips_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6731 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_ppc_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34775 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_ppc_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)  1130268 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_ppc_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17479 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_s390_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   101697 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_s390_helpers.c
+-rwxr-xr-x   0 vsts      (1001) docker     (121)    10118 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_s390_insn_formats.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   727610 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_s390_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4954 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_tilegx_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20766 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_tilegx_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    79947 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_tilegx_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16605 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_x86_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   100948 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_x86_helpers.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   552835 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/guest_x86_toIR.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   145172 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_amd64_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    30093 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_amd64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   191170 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_amd64_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   218996 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_arm64_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    37441 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_arm64_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   163347 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_arm64_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   183248 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_arm_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    35420 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_arm_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   257988 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_arm_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11045 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_maddf.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1870 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_maddf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    60281 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_reg_alloc2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    55387 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_reg_alloc3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11727 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_regs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17459 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_regs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13196 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_simd128.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3773 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_simd128.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2155 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_simd256.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2066 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_simd256.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43649 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_simd64.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7296 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_generic_simd64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   131651 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_mips_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    26553 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_mips_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   151524 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_mips_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   231014 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_ppc_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    43619 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_ppc_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   266473 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_ppc_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   329366 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_s390_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    34560 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_s390_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   174718 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_s390_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    76788 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_tilegx_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20244 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_tilegx_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    56164 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_tilegx_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   120030 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_x86_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    26278 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_x86_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   164986 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/host_x86_isel.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   190764 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/ir_defs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    10919 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/ir_inject.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3802 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/ir_match.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3145 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/ir_match.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   230984 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/ir_opt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2820 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/ir_opt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/main_globals.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2803 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/main_globals.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    82312 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/main_main.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18330 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/main_util.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5609 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/main_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3163 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/multiarch_main_main.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6083 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/s390_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14758 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/s390_disasm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3277 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/s390_disasm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   180250 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/tilegx_disasm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    28210 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/priv/tilegx_disasm.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.249102 pyvex-9.2.9/vex/pub/
+-rw-r--r--   0 vsts      (1001) docker     (121)    41629 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6453 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_basictypes.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4889 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_emnote.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8755 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_amd64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7926 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_arm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6526 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_arm64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6330 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_mips32.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6397 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_mips64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11695 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_ppc32.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13411 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_ppc64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7258 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_s390x.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4896 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_tilegx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12432 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_guest_x86.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   122233 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_ir.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5025 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_s390x_common.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4451 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/pub/libvex_trc_values.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.253102 pyvex-9.2.9/vex/switchback/
+-rw-r--r--   0 vsts      (1001) docker     (121)      257 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/Makefile
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     9974 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/binary_switchback.pl
+-rw-r--r--   0 vsts      (1001) docker     (121)    45293 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/linker.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      113 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/linker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24229 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/switchback.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   184904 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/test_bzip2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    53078 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/test_emfloat.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      286 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/test_hello.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   115291 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/test_ppc_jm1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      180 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/switchback/test_simple.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.253102 pyvex-9.2.9/vex/test/
+-rw-r--r--   0 vsts      (1001) docker     (121)      542 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fldenv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      224 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fp1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      792 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fp1.s
+-rw-r--r--   0 vsts      (1001) docker     (121)     1572 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fpconst.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1451 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fpgames.s
+-rw-r--r--   0 vsts      (1001) docker     (121)      555 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fpspeed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      660 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fpucw.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1906 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/frstor.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1557 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fsave.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      393 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fstenv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3462 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/fxsave.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20405 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/mmxtest.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      694 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/mxcsr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2169 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/rounderr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2157 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-amd64-muldiv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4715 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-amd64-shift.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    45441 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-amd64.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6381 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-amd64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1521 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-i386-muldiv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4022 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-i386-shift.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    44331 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-i386.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5372 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/test-i386.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      926 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/x87fxam.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      403 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/test/x87tst.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.257102 pyvex-9.2.9/vex/unused/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1593 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/unused/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2502 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/unused/dispatch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    43051 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/unused/linker.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:09.257102 pyvex-9.2.9/vex/useful/
+-rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/Makefile-vex
+-rw-r--r--   0 vsts      (1001) docker     (121)     1326 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/cpuid.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19175 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/fp_80_64.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/fpround.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      383 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/fspill.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      201 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/gradual_underflow.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    54111 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/hd_fpu.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4886 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/show_fp_state.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7171 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/smchash.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    89474 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/test_main.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/test_main.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/test_main.h.base
+-rw-r--r--   0 vsts      (1001) docker     (121)     8384 2022-07-05 17:01:16.000000 pyvex-9.2.9/vex/useful/x87_to_vex_and_back.c
```

### Comparing `pyvex-9.2.8/LICENSE` & `pyvex-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/PKG-INFO` & `pyvex-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvex
-Version: 9.2.8
+Version: 9.2.9
 Summary: A Python interface to libVEX and VEX IR
 Home-page: https://github.com/angr/pyvex
 License: Mixed
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `pyvex-9.2.8/README.md` & `pyvex-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/make_ffi.py` & `pyvex-9.2.9/make_ffi.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/__init__.py` & `pyvex-9.2.9/pyvex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 PyVEX provides an interface that translates binary code into the VEX intermediate representation (IR).
 For an introduction to VEX, take a look here: https://docs.angr.io/advanced-topics/ir
 """
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 if bytes is str:
     raise Exception("This module is designed for python 3 only. Please install an older version to use python 2.")
 
 import os
 import sys
 import hashlib
```

### Comparing `pyvex-9.2.8/pyvex/block.py` & `pyvex-9.2.9/pyvex/block.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/const.py` & `pyvex-9.2.9/pyvex/const.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/data_ref.py` & `pyvex-9.2.9/pyvex/data_ref.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/enums.py` & `pyvex-9.2.9/pyvex/enums.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/errors.py` & `pyvex-9.2.9/pyvex/errors.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/expr.py` & `pyvex-9.2.9/pyvex/expr.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/__init__.py` & `pyvex-9.2.9/pyvex/lifting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/gym/aarch64_spotter.py` & `pyvex-9.2.9/pyvex/lifting/gym/aarch64_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/gym/arm_spotter.py` & `pyvex-9.2.9/pyvex/lifting/gym/arm_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/gym/x86_spotter.py` & `pyvex-9.2.9/pyvex/lifting/gym/x86_spotter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/libvex.py` & `pyvex-9.2.9/pyvex/lifting/libvex.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/lifter.py` & `pyvex-9.2.9/pyvex/lifting/lifter.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/util/instr_helper.py` & `pyvex-9.2.9/pyvex/lifting/util/instr_helper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/util/irsb_postprocess.py` & `pyvex-9.2.9/pyvex/lifting/util/irsb_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/util/lifter_helper.py` & `pyvex-9.2.9/pyvex/lifting/util/lifter_helper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/util/syntax_wrapper.py` & `pyvex-9.2.9/pyvex/lifting/util/syntax_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/util/vex_helper.py` & `pyvex-9.2.9/pyvex/lifting/util/vex_helper.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/lifting/zerodivision.py` & `pyvex-9.2.9/pyvex/lifting/zerodivision.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/stmt.py` & `pyvex-9.2.9/pyvex/stmt.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex/utils.py` & `pyvex-9.2.9/pyvex/utils.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex.egg-info/PKG-INFO` & `pyvex-9.2.9/pyvex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvex
-Version: 9.2.8
+Version: 9.2.9
 Summary: A Python interface to libVEX and VEX IR
 Home-page: https://github.com/angr/pyvex
 License: Mixed
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `pyvex-9.2.8/pyvex.egg-info/SOURCES.txt` & `pyvex-9.2.9/pyvex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/LICENSE` & `pyvex-9.2.9/pyvex_c/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/Makefile` & `pyvex-9.2.9/pyvex_c/Makefile`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/analysis.c` & `pyvex-9.2.9/pyvex_c/analysis.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/e4c_lite.h` & `pyvex-9.2.9/pyvex_c/e4c_lite.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/logging.c` & `pyvex-9.2.9/pyvex_c/logging.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/postprocess.c` & `pyvex-9.2.9/pyvex_c/postprocess.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/pyvex.c` & `pyvex-9.2.9/pyvex_c/pyvex.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/pyvex.def` & `pyvex-9.2.9/pyvex_c/pyvex.def`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/pyvex.h` & `pyvex-9.2.9/pyvex_c/pyvex.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/pyvex_c/pyvex_internal.h` & `pyvex-9.2.9/pyvex_c/pyvex_internal.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/setup.cfg` & `pyvex-9.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 description = A Python interface to libVEX and VEX IR
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 python_requires = >= 3.8
 install_requires = 
-	archinfo == 9.2.8
+	archinfo == 9.2.9
 	bitstring
 	cffi >= 1.0.3; implementation_name == 'cpython'
 include_package_data = True
 packages = find:
 
 [options.package_data]
 pyvex =
```

### Comparing `pyvex-9.2.8/setup.py` & `pyvex-9.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/LICENSE.GPL` & `pyvex-9.2.9/vex/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/LICENSE.README` & `pyvex-9.2.9/vex/LICENSE.README`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/Makefile-gcc` & `pyvex-9.2.9/vex/Makefile-gcc`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/Makefile-msvc` & `pyvex-9.2.9/vex/Makefile-msvc`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/TODO.txt` & `pyvex-9.2.9/vex/TODO.txt`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/auxprogs/genoffsets.c` & `pyvex-9.2.9/vex/auxprogs/genoffsets.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/common.mk` & `pyvex-9.2.9/vex/common.mk`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_amd64/Compare.hs` & `pyvex-9.2.9/vex/orig_amd64/Compare.hs`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_amd64/SortedToOrig.hs` & `pyvex-9.2.9/vex/orig_amd64/SortedToOrig.hs`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_amd64/test1.orig` & `pyvex-9.2.9/vex/orig_amd64/test1.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_amd64/test1.sorted` & `pyvex-9.2.9/vex/orig_amd64/test1.sorted`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_amd64/test2.orig` & `pyvex-9.2.9/vex/orig_amd64/test2.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_amd64/test2.sorted` & `pyvex-9.2.9/vex/orig_amd64/test2.sorted`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_ppc32/date.orig` & `pyvex-9.2.9/vex/orig_ppc32/date.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_ppc32/loadsafp.orig` & `pyvex-9.2.9/vex/orig_ppc32/loadsafp.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_ppc32/morefp.orig` & `pyvex-9.2.9/vex/orig_ppc32/morefp.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_ppc32/return0.orig` & `pyvex-9.2.9/vex/orig_ppc32/return0.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_x86/exit42.orig` & `pyvex-9.2.9/vex/orig_x86/exit42.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_x86/fpu_mmx_sse.orig` & `pyvex-9.2.9/vex/orig_x86/fpu_mmx_sse.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/orig_x86/manyfp.orig` & `pyvex-9.2.9/vex/orig_x86/manyfp.orig`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_amd64_defs.h` & `pyvex-9.2.9/vex/priv/guest_amd64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_amd64_helpers.c` & `pyvex-9.2.9/vex/priv/guest_amd64_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_amd64_toIR.c` & `pyvex-9.2.9/vex/priv/guest_amd64_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_arm64_defs.h` & `pyvex-9.2.9/vex/priv/guest_arm64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_arm64_helpers.c` & `pyvex-9.2.9/vex/priv/guest_arm64_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_arm64_toIR.c` & `pyvex-9.2.9/vex/priv/guest_arm64_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_arm_defs.h` & `pyvex-9.2.9/vex/priv/guest_arm_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_arm_helpers.c` & `pyvex-9.2.9/vex/priv/guest_arm_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_arm_toIR.c` & `pyvex-9.2.9/vex/priv/guest_arm_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_generic_bb_to_IR.c` & `pyvex-9.2.9/vex/priv/guest_generic_bb_to_IR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_generic_bb_to_IR.h` & `pyvex-9.2.9/vex/priv/guest_generic_bb_to_IR.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_generic_x87.c` & `pyvex-9.2.9/vex/priv/guest_generic_x87.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_generic_x87.h` & `pyvex-9.2.9/vex/priv/guest_generic_x87.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_mips_defs.h` & `pyvex-9.2.9/vex/priv/guest_mips_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_mips_helpers.c` & `pyvex-9.2.9/vex/priv/guest_mips_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_mips_toIR.c` & `pyvex-9.2.9/vex/priv/guest_mips_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_ppc_defs.h` & `pyvex-9.2.9/vex/priv/guest_ppc_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_ppc_helpers.c` & `pyvex-9.2.9/vex/priv/guest_ppc_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_ppc_toIR.c` & `pyvex-9.2.9/vex/priv/guest_ppc_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_s390_defs.h` & `pyvex-9.2.9/vex/priv/guest_s390_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_s390_helpers.c` & `pyvex-9.2.9/vex/priv/guest_s390_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_s390_insn_formats.py` & `pyvex-9.2.9/vex/priv/guest_s390_insn_formats.py`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_s390_toIR.c` & `pyvex-9.2.9/vex/priv/guest_s390_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_tilegx_defs.h` & `pyvex-9.2.9/vex/priv/guest_tilegx_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_tilegx_helpers.c` & `pyvex-9.2.9/vex/priv/guest_tilegx_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_tilegx_toIR.c` & `pyvex-9.2.9/vex/priv/guest_tilegx_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_x86_defs.h` & `pyvex-9.2.9/vex/priv/guest_x86_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_x86_helpers.c` & `pyvex-9.2.9/vex/priv/guest_x86_helpers.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/guest_x86_toIR.c` & `pyvex-9.2.9/vex/priv/guest_x86_toIR.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_amd64_defs.c` & `pyvex-9.2.9/vex/priv/host_amd64_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_amd64_defs.h` & `pyvex-9.2.9/vex/priv/host_amd64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_amd64_isel.c` & `pyvex-9.2.9/vex/priv/host_amd64_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_arm64_defs.c` & `pyvex-9.2.9/vex/priv/host_arm64_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_arm64_defs.h` & `pyvex-9.2.9/vex/priv/host_arm64_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_arm64_isel.c` & `pyvex-9.2.9/vex/priv/host_arm64_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_arm_defs.c` & `pyvex-9.2.9/vex/priv/host_arm_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_arm_defs.h` & `pyvex-9.2.9/vex/priv/host_arm_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_arm_isel.c` & `pyvex-9.2.9/vex/priv/host_arm_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_maddf.c` & `pyvex-9.2.9/vex/priv/host_generic_maddf.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_maddf.h` & `pyvex-9.2.9/vex/priv/host_generic_maddf.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_reg_alloc2.c` & `pyvex-9.2.9/vex/priv/host_generic_reg_alloc2.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_reg_alloc3.c` & `pyvex-9.2.9/vex/priv/host_generic_reg_alloc3.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_regs.c` & `pyvex-9.2.9/vex/priv/host_generic_regs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_regs.h` & `pyvex-9.2.9/vex/priv/host_generic_regs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_simd128.c` & `pyvex-9.2.9/vex/priv/host_generic_simd128.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_simd128.h` & `pyvex-9.2.9/vex/priv/host_generic_simd128.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_simd256.c` & `pyvex-9.2.9/vex/priv/host_generic_simd256.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_simd256.h` & `pyvex-9.2.9/vex/priv/host_generic_simd256.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_simd64.c` & `pyvex-9.2.9/vex/priv/host_generic_simd64.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_generic_simd64.h` & `pyvex-9.2.9/vex/priv/host_generic_simd64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_mips_defs.c` & `pyvex-9.2.9/vex/priv/host_mips_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_mips_defs.h` & `pyvex-9.2.9/vex/priv/host_mips_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_mips_isel.c` & `pyvex-9.2.9/vex/priv/host_mips_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_ppc_defs.c` & `pyvex-9.2.9/vex/priv/host_ppc_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_ppc_defs.h` & `pyvex-9.2.9/vex/priv/host_ppc_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_ppc_isel.c` & `pyvex-9.2.9/vex/priv/host_ppc_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_s390_defs.c` & `pyvex-9.2.9/vex/priv/host_s390_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_s390_defs.h` & `pyvex-9.2.9/vex/priv/host_s390_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_s390_isel.c` & `pyvex-9.2.9/vex/priv/host_s390_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_tilegx_defs.c` & `pyvex-9.2.9/vex/priv/host_tilegx_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_tilegx_defs.h` & `pyvex-9.2.9/vex/priv/host_tilegx_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_tilegx_isel.c` & `pyvex-9.2.9/vex/priv/host_tilegx_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_x86_defs.c` & `pyvex-9.2.9/vex/priv/host_x86_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_x86_defs.h` & `pyvex-9.2.9/vex/priv/host_x86_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/host_x86_isel.c` & `pyvex-9.2.9/vex/priv/host_x86_isel.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/ir_defs.c` & `pyvex-9.2.9/vex/priv/ir_defs.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/ir_inject.c` & `pyvex-9.2.9/vex/priv/ir_inject.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/ir_match.c` & `pyvex-9.2.9/vex/priv/ir_match.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/ir_match.h` & `pyvex-9.2.9/vex/priv/ir_match.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/ir_opt.c` & `pyvex-9.2.9/vex/priv/ir_opt.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/ir_opt.h` & `pyvex-9.2.9/vex/priv/ir_opt.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/main_globals.c` & `pyvex-9.2.9/vex/priv/main_globals.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/main_globals.h` & `pyvex-9.2.9/vex/priv/main_globals.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/main_main.c` & `pyvex-9.2.9/vex/priv/main_main.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/main_util.c` & `pyvex-9.2.9/vex/priv/main_util.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/main_util.h` & `pyvex-9.2.9/vex/priv/main_util.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/multiarch_main_main.c` & `pyvex-9.2.9/vex/priv/multiarch_main_main.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/s390_defs.h` & `pyvex-9.2.9/vex/priv/s390_defs.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/s390_disasm.c` & `pyvex-9.2.9/vex/priv/s390_disasm.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/s390_disasm.h` & `pyvex-9.2.9/vex/priv/s390_disasm.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/tilegx_disasm.c` & `pyvex-9.2.9/vex/priv/tilegx_disasm.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/priv/tilegx_disasm.h` & `pyvex-9.2.9/vex/priv/tilegx_disasm.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex.h` & `pyvex-9.2.9/vex/pub/libvex.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_basictypes.h` & `pyvex-9.2.9/vex/pub/libvex_basictypes.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_emnote.h` & `pyvex-9.2.9/vex/pub/libvex_emnote.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_amd64.h` & `pyvex-9.2.9/vex/pub/libvex_guest_amd64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_arm.h` & `pyvex-9.2.9/vex/pub/libvex_guest_arm.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_arm64.h` & `pyvex-9.2.9/vex/pub/libvex_guest_arm64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_mips32.h` & `pyvex-9.2.9/vex/pub/libvex_guest_mips32.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_mips64.h` & `pyvex-9.2.9/vex/pub/libvex_guest_mips64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_ppc32.h` & `pyvex-9.2.9/vex/pub/libvex_guest_ppc32.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_ppc64.h` & `pyvex-9.2.9/vex/pub/libvex_guest_ppc64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_s390x.h` & `pyvex-9.2.9/vex/pub/libvex_guest_s390x.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_tilegx.h` & `pyvex-9.2.9/vex/pub/libvex_guest_tilegx.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_guest_x86.h` & `pyvex-9.2.9/vex/pub/libvex_guest_x86.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_ir.h` & `pyvex-9.2.9/vex/pub/libvex_ir.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_s390x_common.h` & `pyvex-9.2.9/vex/pub/libvex_s390x_common.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/pub/libvex_trc_values.h` & `pyvex-9.2.9/vex/pub/libvex_trc_values.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/switchback/binary_switchback.pl` & `pyvex-9.2.9/vex/switchback/binary_switchback.pl`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/switchback/linker.c` & `pyvex-9.2.9/vex/switchback/linker.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/switchback/switchback.c` & `pyvex-9.2.9/vex/switchback/switchback.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/switchback/test_bzip2.c` & `pyvex-9.2.9/vex/switchback/test_bzip2.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/switchback/test_emfloat.c` & `pyvex-9.2.9/vex/switchback/test_emfloat.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/switchback/test_ppc_jm1.c` & `pyvex-9.2.9/vex/switchback/test_ppc_jm1.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fldenv.c` & `pyvex-9.2.9/vex/test/fldenv.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fp1.s` & `pyvex-9.2.9/vex/test/fp1.s`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fpconst.c` & `pyvex-9.2.9/vex/test/fpconst.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fpgames.s` & `pyvex-9.2.9/vex/test/fpgames.s`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fpspeed.c` & `pyvex-9.2.9/vex/test/fpspeed.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fpucw.c` & `pyvex-9.2.9/vex/test/fpucw.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/frstor.c` & `pyvex-9.2.9/vex/test/frstor.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fsave.c` & `pyvex-9.2.9/vex/test/fsave.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/fxsave.c` & `pyvex-9.2.9/vex/test/fxsave.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/mmxtest.c` & `pyvex-9.2.9/vex/test/mmxtest.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/mxcsr.c` & `pyvex-9.2.9/vex/test/mxcsr.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/rounderr.c` & `pyvex-9.2.9/vex/test/rounderr.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-amd64-muldiv.h` & `pyvex-9.2.9/vex/test/test-amd64-muldiv.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-amd64-shift.h` & `pyvex-9.2.9/vex/test/test-amd64-shift.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-amd64.c` & `pyvex-9.2.9/vex/test/test-amd64.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-amd64.h` & `pyvex-9.2.9/vex/test/test-amd64.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-i386-muldiv.h` & `pyvex-9.2.9/vex/test/test-i386-muldiv.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-i386-shift.h` & `pyvex-9.2.9/vex/test/test-i386-shift.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-i386.c` & `pyvex-9.2.9/vex/test/test-i386.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/test-i386.h` & `pyvex-9.2.9/vex/test/test-i386.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/test/x87fxam.c` & `pyvex-9.2.9/vex/test/x87fxam.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/unused/arena.h` & `pyvex-9.2.9/vex/unused/arena.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/unused/dispatch.c` & `pyvex-9.2.9/vex/unused/dispatch.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/unused/linker.c` & `pyvex-9.2.9/vex/unused/linker.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/cpuid.c` & `pyvex-9.2.9/vex/useful/cpuid.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/fp_80_64.c` & `pyvex-9.2.9/vex/useful/fp_80_64.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/hd_fpu.c` & `pyvex-9.2.9/vex/useful/hd_fpu.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/show_fp_state.c` & `pyvex-9.2.9/vex/useful/show_fp_state.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/smchash.c` & `pyvex-9.2.9/vex/useful/smchash.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/test_main.c` & `pyvex-9.2.9/vex/useful/test_main.c`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/test_main.h` & `pyvex-9.2.9/vex/useful/test_main.h`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/test_main.h.base` & `pyvex-9.2.9/vex/useful/test_main.h.base`

 * *Files identical despite different names*

### Comparing `pyvex-9.2.8/vex/useful/x87_to_vex_and_back.c` & `pyvex-9.2.9/vex/useful/x87_to_vex_and_back.c`

 * *Files identical despite different names*

