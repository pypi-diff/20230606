# Comparing `tmp/archr-9.2.8.tar.gz` & `tmp/archr-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archr-9.2.8.tar", last modified: Tue Jun 28 17:04:30 2022, max compression
+gzip compressed data, was "archr-9.2.9.tar", last modified: Tue Jul  5 17:03:41 2022, max compression
```

## Comparing `archr-9.2.8.tar` & `archr-9.2.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-06-28 17:01:21.000000 archr-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-06-28 17:01:21.000000 archr-9.2.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     4970 2022-06-28 17:04:30.975762 archr-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     4465 2022-06-28 17:01:21.000000 archr-9.2.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/
--rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-06-28 17:01:35.000000 archr-9.2.8/archr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/analyzers/
--rw-r--r--   0 vsts      (1001) docker     (121)     4699 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8029 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/angr_project.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5311 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/angr_state.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2539 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/angr_ultimate_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6321 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/bintrace_qemu_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1787 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/core.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9222 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/datascout.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3126 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (121)      507 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/gdbserver.py
--rw-r--r--   0 vsts      (1001) docker     (121)      905 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/input_fd.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/ltrace.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13797 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/qemu_tracer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1230 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/qtrace.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9148 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/rr.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2273 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/strace.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2654 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/tcpdump.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1115 2022-06-28 17:01:21.000000 archr-9.2.8/archr/analyzers/udp_tcp_convert.py
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-06-28 17:01:21.000000 archr-9.2.8/archr/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/implants/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/implants/GENERIC/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      511 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/GENERIC/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      150 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/GENERIC/fire
--rw-r--r--   0 vsts      (1001) docker     (121)      865 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/implants/bintrace_qemu/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      671 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/bintrace_qemu/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      352 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/bintrace_qemu/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/implants/emurrate/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1148 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/emurrate/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      200 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/emurrate/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/implants/gdb/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1178 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/gdb/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      218 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/gdb/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr/implants/gdbserver/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      429 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/gdbserver/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      147 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/gdbserver/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/archr/implants/ltrace/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      402 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/ltrace/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      170 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/ltrace/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/archr/implants/qtrace/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      851 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/qtrace/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      211 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/qtrace/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/archr/implants/rr/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1685 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/rr/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      217 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/rr/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/archr/implants/shellphish_qemu/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      617 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/shellphish_qemu/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)       62 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/shellphish_qemu/fire
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/archr/implants/udp_tcp_convert/
--rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/udp_tcp_convert/CMakeLists.txt
--rwxr-xr-x   0 vsts      (1001) docker     (121)      527 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/udp_tcp_convert/bundle
--rwxr-xr-x   0 vsts      (1001) docker     (121)      188 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/udp_tcp_convert/fire
--rw-r--r--   0 vsts      (1001) docker     (121)     5728 2022-06-28 17:01:21.000000 archr-9.2.8/archr/implants/udp_tcp_convert/udp_to_tcp.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6845 2022-06-28 17:01:21.000000 archr-9.2.8/archr/strace_parser.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.975762 archr-9.2.8/archr/targets/
--rw-r--r--   0 vsts      (1001) docker     (121)    15356 2022-06-28 17:01:21.000000 archr-9.2.8/archr/targets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4371 2022-06-28 17:01:21.000000 archr-9.2.8/archr/targets/actions.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17338 2022-06-28 17:01:21.000000 archr-9.2.8/archr/targets/docker_target.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3473 2022-06-28 17:01:21.000000 archr-9.2.8/archr/targets/flight.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4697 2022-06-28 17:01:21.000000 archr-9.2.8/archr/targets/local_target.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8280 2022-06-28 17:01:21.000000 archr-9.2.8/archr/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:04:30.971762 archr-9.2.8/archr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4970 2022-06-28 17:04:30.000000 archr-9.2.8/archr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1636 2022-06-28 17:04:30.000000 archr-9.2.8/archr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:04:30.000000 archr-9.2.8/archr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      145 2022-06-28 17:04:30.000000 archr-9.2.8/archr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-06-28 17:04:30.000000 archr-9.2.8/archr.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      116 2022-06-28 17:01:35.000000 archr-9.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      813 2022-06-28 17:04:30.975762 archr-9.2.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-06-28 17:01:21.000000 archr-9.2.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-07-05 17:01:32.000000 archr-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-07-05 17:01:32.000000 archr-9.2.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     4970 2022-07-05 17:03:41.573770 archr-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     4465 2022-07-05 17:01:32.000000 archr-9.2.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.565770 archr-9.2.9/archr/
+-rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-07-05 17:01:34.000000 archr-9.2.9/archr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/analyzers/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4699 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8029 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/angr_project.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5311 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/angr_state.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2539 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/angr_ultimate_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6321 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/bintrace_qemu_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1787 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/core.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9222 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/datascout.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3126 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      507 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/gdbserver.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      905 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/input_fd.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/ltrace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13797 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/qemu_tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1230 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/qtrace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9148 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/rr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2273 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/strace.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2654 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/tcpdump.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1115 2022-07-05 17:01:32.000000 archr-9.2.9/archr/analyzers/udp_tcp_convert.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-07-05 17:01:32.000000 archr-9.2.9/archr/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/implants/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/implants/GENERIC/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      511 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/GENERIC/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      150 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/GENERIC/fire
+-rw-r--r--   0 vsts      (1001) docker     (121)      865 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/implants/bintrace_qemu/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      671 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/bintrace_qemu/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      352 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/bintrace_qemu/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/implants/emurrate/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1148 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/emurrate/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      200 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/emurrate/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/implants/gdb/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1178 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/gdb/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      218 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/gdb/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.569770 archr-9.2.9/archr/implants/gdbserver/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      429 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/gdbserver/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      147 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/gdbserver/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/archr/implants/ltrace/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      402 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/ltrace/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      170 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/ltrace/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/archr/implants/qtrace/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      851 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/qtrace/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      211 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/qtrace/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/archr/implants/rr/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1685 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/rr/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      217 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/rr/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/archr/implants/shellphish_qemu/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      617 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/shellphish_qemu/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)       62 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/shellphish_qemu/fire
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/archr/implants/udp_tcp_convert/
+-rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/udp_tcp_convert/CMakeLists.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      527 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/udp_tcp_convert/bundle
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      188 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/udp_tcp_convert/fire
+-rw-r--r--   0 vsts      (1001) docker     (121)     5728 2022-07-05 17:01:32.000000 archr-9.2.9/archr/implants/udp_tcp_convert/udp_to_tcp.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6845 2022-07-05 17:01:32.000000 archr-9.2.9/archr/strace_parser.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.573770 archr-9.2.9/archr/targets/
+-rw-r--r--   0 vsts      (1001) docker     (121)    15356 2022-07-05 17:01:32.000000 archr-9.2.9/archr/targets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4371 2022-07-05 17:01:32.000000 archr-9.2.9/archr/targets/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17338 2022-07-05 17:01:32.000000 archr-9.2.9/archr/targets/docker_target.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3473 2022-07-05 17:01:32.000000 archr-9.2.9/archr/targets/flight.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4697 2022-07-05 17:01:32.000000 archr-9.2.9/archr/targets/local_target.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8280 2022-07-05 17:01:32.000000 archr-9.2.9/archr/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:03:41.565770 archr-9.2.9/archr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4970 2022-07-05 17:03:41.000000 archr-9.2.9/archr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1636 2022-07-05 17:03:41.000000 archr-9.2.9/archr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:03:41.000000 archr-9.2.9/archr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      145 2022-07-05 17:03:41.000000 archr-9.2.9/archr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-07-05 17:03:41.000000 archr-9.2.9/archr.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      116 2022-07-05 17:01:34.000000 archr-9.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)      813 2022-07-05 17:03:41.573770 archr-9.2.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-07-05 17:01:32.000000 archr-9.2.9/setup.py
```

### Comparing `archr-9.2.8/LICENSE` & `archr-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/PKG-INFO` & `archr-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archr
-Version: 9.2.8
+Version: 9.2.9
 Summary: Target-centric program analysis.
 Home-page: https://github.com/angr/archr
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `archr-9.2.8/README.md` & `archr-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/__init__.py` & `archr-9.2.9/archr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 import logging
 
 _LOG = logging.getLogger("archr")
 
 try:
     import angr
```

### Comparing `archr-9.2.8/archr/analyzers/__init__.py` & `archr-9.2.9/archr/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/angr_project.py` & `archr-9.2.9/archr/analyzers/angr_project.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/angr_state.py` & `archr-9.2.9/archr/analyzers/angr_state.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/angr_ultimate_tracer.py` & `archr-9.2.9/archr/analyzers/angr_ultimate_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/bintrace_qemu_tracer.py` & `archr-9.2.9/archr/analyzers/bintrace_qemu_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/core.py` & `archr-9.2.9/archr/analyzers/core.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/datascout.py` & `archr-9.2.9/archr/analyzers/datascout.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/gdb.py` & `archr-9.2.9/archr/analyzers/gdb.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/input_fd.py` & `archr-9.2.9/archr/analyzers/input_fd.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/ltrace.py` & `archr-9.2.9/archr/analyzers/ltrace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/qemu_tracer.py` & `archr-9.2.9/archr/analyzers/qemu_tracer.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/qtrace.py` & `archr-9.2.9/archr/analyzers/qtrace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/rr.py` & `archr-9.2.9/archr/analyzers/rr.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/strace.py` & `archr-9.2.9/archr/analyzers/strace.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/tcpdump.py` & `archr-9.2.9/archr/analyzers/tcpdump.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/analyzers/udp_tcp_convert.py` & `archr-9.2.9/archr/analyzers/udp_tcp_convert.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/__init__.py` & `archr-9.2.9/archr/implants/__init__.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/bintrace_qemu/bundle` & `archr-9.2.9/archr/implants/bintrace_qemu/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/emurrate/bundle` & `archr-9.2.9/archr/implants/emurrate/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/gdb/bundle` & `archr-9.2.9/archr/implants/gdb/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/qtrace/bundle` & `archr-9.2.9/archr/implants/qtrace/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/rr/bundle` & `archr-9.2.9/archr/implants/rr/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/shellphish_qemu/bundle` & `archr-9.2.9/archr/implants/shellphish_qemu/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/udp_tcp_convert/bundle` & `archr-9.2.9/archr/implants/udp_tcp_convert/bundle`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/implants/udp_tcp_convert/udp_to_tcp.c` & `archr-9.2.9/archr/implants/udp_tcp_convert/udp_to_tcp.c`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/strace_parser.py` & `archr-9.2.9/archr/strace_parser.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/targets/__init__.py` & `archr-9.2.9/archr/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/targets/actions.py` & `archr-9.2.9/archr/targets/actions.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/targets/docker_target.py` & `archr-9.2.9/archr/targets/docker_target.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/targets/flight.py` & `archr-9.2.9/archr/targets/flight.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/targets/local_target.py` & `archr-9.2.9/archr/targets/local_target.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr/utils.py` & `archr-9.2.9/archr/utils.py`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/archr.egg-info/PKG-INFO` & `archr-9.2.9/archr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archr
-Version: 9.2.8
+Version: 9.2.9
 Summary: Target-centric program analysis.
 Home-page: https://github.com/angr/archr
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `archr-9.2.8/archr.egg-info/SOURCES.txt` & `archr-9.2.9/archr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archr-9.2.8/setup.cfg` & `archr-9.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 [options]
 install_requires = 
 	shellphish_qemu>=0.12.2
 	pygdbmi
 	docker
 	nclib>=1.0.0rc3
 	patchelf-wrapper
-	cle==9.2.8
+	cle==9.2.9
 	ply
 python_requires = >= 3.6
 include_package_data = True
 packages = find:
 
 [options.extras_require]
-angr = angr==9.2.8
+angr = angr==9.2.9
 bintrace = bintrace
 qtrace = qtrace
 
 [options.package_data]
 archr = 
 	implants/*.sh
 	implants/*/*
```

### Comparing `archr-9.2.8/setup.py` & `archr-9.2.9/setup.py`

 * *Files identical despite different names*

