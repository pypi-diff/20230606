# Comparing `tmp/riscemu-2.0.5.tar.gz` & `tmp/riscemu-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riscemu-2.0.5.tar", last modified: Fri Jan 27 16:17:53 2023, max compression
+gzip compressed data, was "riscemu-2.1.0.tar", last modified: Tue Jun  6 15:00:25 2023, max compression
```

## Comparing `riscemu-2.0.5.tar` & `riscemu-2.1.0.tar`

### file list

```diff
@@ -1,77 +1,90 @@
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.683755 riscemu-2.0.5/
--rw-r--r--   0 anton     (1000) users      (100)     1073 2022-03-31 20:48:16.000000 riscemu-2.0.5/LICENSE
--rw-r--r--   0 anton     (1000) users      (100)     5480 2023-01-27 16:17:53.683755 riscemu-2.0.5/PKG-INFO
--rw-r--r--   0 anton     (1000) users      (100)     4952 2023-01-24 18:37:15.000000 riscemu-2.0.5/README.md
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.666756 riscemu-2.0.5/riscemu/
--rw-r--r--   0 anton     (1000) users      (100)     4133 2022-04-17 10:13:15.000000 riscemu-2.0.5/riscemu/CPU.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.666756 riscemu-2.0.5/riscemu/IO/
--rw-r--r--   0 anton     (1000) users      (100)      909 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/IO/IOModule.py
--rw-r--r--   0 anton     (1000) users      (100)     1543 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/IO/TextIO.py
--rw-r--r--   0 anton     (1000) users      (100)        0 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/IO/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)    10655 2022-04-17 10:03:43.000000 riscemu-2.0.5/riscemu/MMU.py
--rw-r--r--   0 anton     (1000) users      (100)      907 2023-01-27 16:16:19.000000 riscemu-2.0.5/riscemu/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     5350 2023-01-27 15:35:04.000000 riscemu-2.0.5/riscemu/__main__.py
--rw-r--r--   0 anton     (1000) users      (100)     7934 2022-04-18 16:59:01.000000 riscemu-2.0.5/riscemu/assembler.py
--rw-r--r--   0 anton     (1000) users      (100)      558 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/colors.py
--rw-r--r--   0 anton     (1000) users      (100)      561 2023-01-27 15:35:04.000000 riscemu-2.0.5/riscemu/config.py
--rw-r--r--   0 anton     (1000) users      (100)     2309 2022-04-01 11:21:41.000000 riscemu-2.0.5/riscemu/debug.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.668756 riscemu-2.0.5/riscemu/decoder/
--rw-r--r--   0 anton     (1000) users      (100)       73 2021-11-13 17:08:18.000000 riscemu-2.0.5/riscemu/decoder/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)      575 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/decoder/__main__.py
--rw-r--r--   0 anton     (1000) users      (100)     2644 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/decoder/decoder.py
--rw-r--r--   0 anton     (1000) users      (100)     2232 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/decoder/formats.py
--rw-r--r--   0 anton     (1000) users      (100)     1310 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/decoder/formatter.py
--rw-r--r--   0 anton     (1000) users      (100)     1850 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/decoder/instruction_table.py
--rw-r--r--   0 anton     (1000) users      (100)      228 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/decoder/regs.py
--rw-r--r--   0 anton     (1000) users      (100)     3198 2022-04-17 09:52:27.000000 riscemu-2.0.5/riscemu/helpers.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.669756 riscemu-2.0.5/riscemu/instructions/
--rw-r--r--   0 anton     (1000) users      (100)     2908 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/instructions/RV32A.py
--rw-r--r--   0 anton     (1000) users      (100)     9913 2023-01-24 18:37:15.000000 riscemu-2.0.5/riscemu/instructions/RV32I.py
--rw-r--r--   0 anton     (1000) users      (100)     1528 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/instructions/RV32M.py
--rw-r--r--   0 anton     (1000) users      (100)      345 2023-01-27 15:35:04.000000 riscemu-2.0.5/riscemu/instructions/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     4755 2023-01-24 18:37:15.000000 riscemu-2.0.5/riscemu/instructions/instruction_set.py
--rw-r--r--   0 anton     (1000) users      (100)      909 2022-04-08 18:59:41.000000 riscemu-2.0.5/riscemu/interactive.py
--rw-r--r--   0 anton     (1000) users      (100)     4930 2023-01-27 15:35:04.000000 riscemu-2.0.5/riscemu/parser.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.674756 riscemu-2.0.5/riscemu/priv/
--rw-r--r--   0 anton     (1000) users      (100)     4593 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/CSR.py
--rw-r--r--   0 anton     (1000) users      (100)     1978 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/priv/CSRConsts.py
--rw-r--r--   0 anton     (1000) users      (100)     4046 2022-04-01 12:45:52.000000 riscemu-2.0.5/riscemu/priv/ElfLoader.py
--rw-r--r--   0 anton     (1000) users      (100)     3130 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/Exceptions.py
--rw-r--r--   0 anton     (1000) users      (100)     2636 2022-04-01 12:45:52.000000 riscemu-2.0.5/riscemu/priv/ImageLoader.py
--rw-r--r--   0 anton     (1000) users      (100)     8277 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/PrivCPU.py
--rw-r--r--   0 anton     (1000) users      (100)     1632 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/PrivMMU.py
--rw-r--r--   0 anton     (1000) users      (100)     5870 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/PrivRV32I.py
--rw-r--r--   0 anton     (1000) users      (100)      454 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/priv/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     1512 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/__main__.py
--rw-r--r--   0 anton     (1000) users      (100)       96 2021-10-26 20:05:33.000000 riscemu-2.0.5/riscemu/priv/privmodes.py
--rw-r--r--   0 anton     (1000) users      (100)     5094 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/priv/types.py
--rw-r--r--   0 anton     (1000) users      (100)     5631 2023-01-27 15:35:04.000000 riscemu-2.0.5/riscemu/registers.py
--rw-r--r--   0 anton     (1000) users      (100)     6051 2022-04-18 16:59:42.000000 riscemu-2.0.5/riscemu/syscall.py
--rw-r--r--   0 anton     (1000) users      (100)     3359 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/tokenizer.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.678756 riscemu-2.0.5/riscemu/types/
--rw-r--r--   0 anton     (1000) users      (100)     1097 2023-01-24 18:34:50.000000 riscemu-2.0.5/riscemu/types/__init__.py
--rw-r--r--   0 anton     (1000) users      (100)     1486 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/binary_data_memory_section.py
--rw-r--r--   0 anton     (1000) users      (100)     3212 2023-01-27 15:35:04.000000 riscemu-2.0.5/riscemu/types/cpu.py
--rw-r--r--   0 anton     (1000) users      (100)     4481 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/exceptions.py
--rw-r--r--   0 anton     (1000) users      (100)      274 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/flags.py
--rw-r--r--   0 anton     (1000) users      (100)      642 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/instruction.py
--rw-r--r--   0 anton     (1000) users      (100)     1982 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/instruction_context.py
--rw-r--r--   0 anton     (1000) users      (100)     1220 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/instruction_memory_section.py
--rw-r--r--   0 anton     (1000) users      (100)     8261 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/int32.py
--rw-r--r--   0 anton     (1000) users      (100)     4379 2023-01-24 18:37:15.000000 riscemu-2.0.5/riscemu/types/memory_section.py
--rw-r--r--   0 anton     (1000) users      (100)     3956 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/program.py
--rw-r--r--   0 anton     (1000) users      (100)     1865 2023-01-25 10:45:13.000000 riscemu-2.0.5/riscemu/types/program_loader.py
--rw-r--r--   0 anton     (1000) users      (100)      898 2022-03-31 20:48:16.000000 riscemu-2.0.5/riscemu/types/simple_instruction.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.680755 riscemu-2.0.5/riscemu.egg-info/
--rw-r--r--   0 anton     (1000) users      (100)     5480 2023-01-27 16:17:53.000000 riscemu-2.0.5/riscemu.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) users      (100)     1765 2023-01-27 16:17:53.000000 riscemu-2.0.5/riscemu.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) users      (100)        1 2023-01-27 16:17:53.000000 riscemu-2.0.5/riscemu.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) users      (100)       17 2023-01-27 16:17:53.000000 riscemu-2.0.5/riscemu.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) users      (100)        8 2023-01-27 16:17:53.000000 riscemu-2.0.5/riscemu.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) users      (100)       38 2023-01-27 16:17:53.683755 riscemu-2.0.5/setup.cfg
--rw-r--r--   0 anton     (1000) users      (100)      958 2022-03-31 20:48:16.000000 riscemu-2.0.5/setup.py
-drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-01-27 16:17:53.682756 riscemu-2.0.5/test/
--rw-r--r--   0 anton     (1000) users      (100)      100 2022-04-17 09:50:16.000000 riscemu-2.0.5/test/test_helpers.py
--rw-r--r--   0 anton     (1000) users      (100)      649 2022-03-31 20:48:16.000000 riscemu-2.0.5/test/test_integers.py
--rw-r--r--   0 anton     (1000) users      (100)     2268 2022-03-31 20:48:16.000000 riscemu-2.0.5/test/test_isa.py
--rw-r--r--   0 anton     (1000) users      (100)     4168 2022-03-31 20:48:16.000000 riscemu-2.0.5/test/test_tokenizer.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.655292 riscemu-2.1.0/
+-rw-r--r--   0 anton     (1000) users      (100)     1074 2023-05-01 15:55:17.000000 riscemu-2.1.0/LICENSE
+-rw-r--r--   0 anton     (1000) users      (100)     5579 2023-06-06 15:00:25.655292 riscemu-2.1.0/PKG-INFO
+-rw-r--r--   0 anton     (1000) users      (100)     5049 2023-05-02 15:45:37.000000 riscemu-2.1.0/README.md
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.653293 riscemu-2.1.0/libc/
+-rw-r--r--   0 anton     (1000) users      (100)      345 2023-06-05 20:16:21.000000 riscemu-2.1.0/libc/crt0.s
+-rw-r--r--   0 anton     (1000) users      (100)     4518 2023-06-05 20:16:21.000000 riscemu-2.1.0/libc/stdlib.s
+-rw-r--r--   0 anton     (1000) users      (100)     4749 2023-06-05 20:16:21.000000 riscemu-2.1.0/libc/string.s
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.649293 riscemu-2.1.0/riscemu/
+-rw-r--r--   0 anton     (1000) users      (100)     4403 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/CPU.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.649293 riscemu-2.1.0/riscemu/IO/
+-rw-r--r--   0 anton     (1000) users      (100)      830 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/IO/IOModule.py
+-rw-r--r--   0 anton     (1000) users      (100)     1567 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/IO/TextIO.py
+-rw-r--r--   0 anton     (1000) users      (100)        0 2021-10-26 20:05:33.000000 riscemu-2.1.0/riscemu/IO/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)    11795 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/MMU.py
+-rw-r--r--   0 anton     (1000) users      (100)      942 2023-06-06 14:20:37.000000 riscemu-2.1.0/riscemu/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)      493 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/__main__.py
+-rw-r--r--   0 anton     (1000) users      (100)     8330 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/assembler.py
+-rw-r--r--   0 anton     (1000) users      (100)      559 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/colors.py
+-rw-r--r--   0 anton     (1000) users      (100)      621 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/config.py
+-rw-r--r--   0 anton     (1000) users      (100)     2259 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/debug.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.650293 riscemu-2.1.0/riscemu/decoder/
+-rw-r--r--   0 anton     (1000) users      (100)       74 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)      589 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/__main__.py
+-rw-r--r--   0 anton     (1000) users      (100)     2648 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/decoder.py
+-rw-r--r--   0 anton     (1000) users      (100)     2283 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/formats.py
+-rw-r--r--   0 anton     (1000) users      (100)     1349 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/formatter.py
+-rw-r--r--   0 anton     (1000) users      (100)     1842 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/instruction_table.py
+-rw-r--r--   0 anton     (1000) users      (100)      341 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/decoder/regs.py
+-rw-r--r--   0 anton     (1000) users      (100)     3340 2023-06-05 21:45:49.000000 riscemu-2.1.0/riscemu/helpers.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.651293 riscemu-2.1.0/riscemu/instructions/
+-rw-r--r--   0 anton     (1000) users      (100)     2908 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/instructions/RV32A.py
+-rw-r--r--   0 anton     (1000) users      (100)    20423 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/instructions/RV32F.py
+-rw-r--r--   0 anton     (1000) users      (100)     9416 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/instructions/RV32I.py
+-rw-r--r--   0 anton     (1000) users      (100)     1325 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/instructions/RV32M.py
+-rw-r--r--   0 anton     (1000) users      (100)      888 2023-06-06 14:08:20.000000 riscemu-2.1.0/riscemu/instructions/RV_Debug.py
+-rw-r--r--   0 anton     (1000) users      (100)      412 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/instructions/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)     4901 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/instructions/instruction_set.py
+-rw-r--r--   0 anton     (1000) users      (100)     1027 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/interactive.py
+-rw-r--r--   0 anton     (1000) users      (100)     5042 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/parser.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.652293 riscemu-2.1.0/riscemu/priv/
+-rw-r--r--   0 anton     (1000) users      (100)     4604 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/CSR.py
+-rw-r--r--   0 anton     (1000) users      (100)     1981 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/CSRConsts.py
+-rw-r--r--   0 anton     (1000) users      (100)     4414 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/ElfLoader.py
+-rw-r--r--   0 anton     (1000) users      (100)     3159 2023-05-01 15:55:17.000000 riscemu-2.1.0/riscemu/priv/Exceptions.py
+-rw-r--r--   0 anton     (1000) users      (100)     2843 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/ImageLoader.py
+-rw-r--r--   0 anton     (1000) users      (100)     8747 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/PrivCPU.py
+-rw-r--r--   0 anton     (1000) users      (100)     1737 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/PrivMMU.py
+-rw-r--r--   0 anton     (1000) users      (100)     5946 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/PrivRV32I.py
+-rw-r--r--   0 anton     (1000) users      (100)      455 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)     1706 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/__main__.py
+-rw-r--r--   0 anton     (1000) users      (100)       96 2021-10-26 20:05:33.000000 riscemu-2.1.0/riscemu/priv/privmodes.py
+-rw-r--r--   0 anton     (1000) users      (100)     5271 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/priv/types.py
+-rw-r--r--   0 anton     (1000) users      (100)        0 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/py.typed
+-rw-r--r--   0 anton     (1000) users      (100)     6444 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/registers.py
+-rw-r--r--   0 anton     (1000) users      (100)     9491 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/riscemu_main.py
+-rw-r--r--   0 anton     (1000) users      (100)     8444 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/syscall.py
+-rw-r--r--   0 anton     (1000) users      (100)     3366 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/tokenizer.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.654292 riscemu-2.1.0/riscemu/tools/
+-rwxr-xr-x   0 anton     (1000) users      (100)       44 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/tools/riscemu
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.653293 riscemu-2.1.0/riscemu/types/
+-rw-r--r--   0 anton     (1000) users      (100)     1193 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/types/__init__.py
+-rw-r--r--   0 anton     (1000) users      (100)     1718 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/binary_data_memory_section.py
+-rw-r--r--   0 anton     (1000) users      (100)     3334 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/cpu.py
+-rw-r--r--   0 anton     (1000) users      (100)     4807 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/exceptions.py
+-rw-r--r--   0 anton     (1000) users      (100)      262 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/flags.py
+-rw-r--r--   0 anton     (1000) users      (100)     5836 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/types/float32.py
+-rw-r--r--   0 anton     (1000) users      (100)      642 2022-03-31 20:48:16.000000 riscemu-2.1.0/riscemu/types/instruction.py
+-rw-r--r--   0 anton     (1000) users      (100)     2195 2023-05-01 15:55:17.000000 riscemu-2.1.0/riscemu/types/instruction_context.py
+-rw-r--r--   0 anton     (1000) users      (100)     1496 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/instruction_memory_section.py
+-rw-r--r--   0 anton     (1000) users      (100)     8612 2023-06-06 14:08:29.000000 riscemu-2.1.0/riscemu/types/int32.py
+-rw-r--r--   0 anton     (1000) users      (100)     5271 2023-06-05 20:16:21.000000 riscemu-2.1.0/riscemu/types/memory_section.py
+-rw-r--r--   0 anton     (1000) users      (100)     4143 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/program.py
+-rw-r--r--   0 anton     (1000) users      (100)     1865 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/program_loader.py
+-rw-r--r--   0 anton     (1000) users      (100)      927 2023-05-01 15:37:55.000000 riscemu-2.1.0/riscemu/types/simple_instruction.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.654292 riscemu-2.1.0/riscemu.egg-info/
+-rw-r--r--   0 anton     (1000) users      (100)     5579 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) users      (100)     2005 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) users      (100)        1 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) users      (100)       17 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) users      (100)        8 2023-06-06 15:00:25.000000 riscemu-2.1.0/riscemu.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) users      (100)       38 2023-06-06 15:00:25.655292 riscemu-2.1.0/setup.cfg
+-rw-r--r--   0 anton     (1000) users      (100)     1195 2023-06-06 14:52:50.000000 riscemu-2.1.0/setup.py
+drwxr-xr-x   0 anton     (1000) users      (100)        0 2023-06-06 15:00:25.654292 riscemu-2.1.0/test/
+-rw-r--r--   0 anton     (1000) users      (100)      466 2023-06-06 14:08:29.000000 riscemu-2.1.0/test/test_float32.py
+-rw-r--r--   0 anton     (1000) users      (100)      395 2023-06-05 21:52:17.000000 riscemu-2.1.0/test/test_helpers.py
+-rw-r--r--   0 anton     (1000) users      (100)      468 2023-05-01 15:29:41.000000 riscemu-2.1.0/test/test_integers.py
+-rw-r--r--   0 anton     (1000) users      (100)     2326 2023-05-01 15:37:55.000000 riscemu-2.1.0/test/test_isa.py
+-rw-r--r--   0 anton     (1000) users      (100)      578 2023-06-06 14:08:29.000000 riscemu-2.1.0/test/test_regs.py
+-rw-r--r--   0 anton     (1000) users      (100)     4548 2023-05-01 15:37:55.000000 riscemu-2.1.0/test/test_tokenizer.py
```

### Comparing `riscemu-2.0.5/LICENSE` & `riscemu-2.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `riscemu-2.0.5/PKG-INFO` & `riscemu-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: riscemu
-Version: 2.0.5
-Summary: RISC-V userspace and privileged emulator
+Version: 2.1.0
+Summary: RISC-V userspace and machine mode emulator
 Home-page: https://github.com/antonlydike/riscemu
 Author: Anton Lydike <Anton@Lydike.com>
 Author-email: pip@antonlydike.de
 Project-URL: Bug Tracker, https://github.com/AntonLydike/riscemu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RiscEmu - RISC-V (userspace) emulator in python
 
 [![Documentation Status](https://readthedocs.org/projects/riscemu/badge/?version=latest)](https://riscemu.readthedocs.io/en/latest/?badge=latest)
 
@@ -21,15 +21,15 @@
 or [riscemu.datenvorr.at](https://riscemu.datenvorr.at/index.html).
 
 This emulator contains:
 * RISC-V Assembly parser
 * RISC-V Assembly loader
 * Emulation for most parts of the basic RISC-V instruction set and the M and A extensions
 * Naive memory emulator
-* Basic implementation of some syscalls 
+* Basic implementation of some syscalls
 * A debugging environment
 
 ## Installation:
 
 ```bash
 $ pip install riscemu
 ```
@@ -44,15 +44,15 @@
 Hello world
 
 Program exited with code 0
 ```
 
 If you want to run it from a python script, here is [an online demo](https://AntonLydike.github.io/riscemu/lab/index.html?path=PythonDemo.ipynb).
 
-The [`read` syscall](docs/syscalls.md) defaults to readline behaviour. Reading "true chunks" (ignoring newlines) is currently not supported.  
+The [`read` syscall](docs/syscalls.md) defaults to readline behaviour. Reading "true chunks" (ignoring newlines) is currently not supported.
 
 See the docs on [asembly](docs/assembly.md) for more detail on how to write assembly code for this emulator.
 See the [list of implemented syscalls](docs/syscalls.md) for more details on how to syscall.
 
 Currently, symbols (such as `main` or `loop`) are looked-up at runtime. This allows for better debugging, I believe.
 
 Basic IO should work, as open, read, write and close are supported for stdin/stdout/stderr and even aribtrary file paths (if enabled)
@@ -82,18 +82,18 @@
                         Options to control syscall behaviour
 fs_access               Allow access to the filesystem
 disable_io              Disallow reading/writing from stdin/stdout/stderr
 
 --instruction-sets INSTRUCTION_SETS: (-is)
                         A list of comma separated instruction sets you want to load:
                         Currently implemented: RV32I, RV32M
-``` 
+```
 
-If multiple files are specified, all are loaded into memeory, but only the last one is executed. This might be improved 
-later, maybe the `_init` section of each binary is executed before the main loop starts? 
+If multiple files are specified, all are loaded into memeory, but only the last one is executed. This might be improved
+later, maybe the `_init` section of each binary is executed before the main loop starts?
 
 If `stack_size` is greater than zero, a stack is allocated and initialized, with the `sp` register pointing to the end of the stack.
 
 
 ## Debugging
 Debugging is done using the `ebreak` (formerly `sbreak`) instruction, which will launch a debugging session if encountered.
 See [docs/debugging.md](docs/debugging.md) for more info.
@@ -101,21 +101,21 @@
 ![debuggin the fibs program](docs/debug-session.png)
 
 
 ## The source code:
 Check out the [documentation](https://riscemu.readthedocs.io/en/latest/riscemu.html).
 
 ## Accessing local documentation:
-To generate your local documentation, first install everything in `sphinx-docs/requirements.txt`. Then run `./generate-docs.sh`, which will 
+To generate your local documentation, first install everything in `sphinx-docs/requirements.txt`. Then run `./generate-docs.sh`, which will
 generate and make all doc files for you. Finally, you can open the docs locall by runnint `open sphinx-docs/build/html/index.html`.
 
 ## Resources:
+  * RISC-V Programmers Handbook: https://github.com/riscv-non-isa/riscv-asm-manual/blob/master/riscv-asm.md
   * Pseudo ops: https://www.codetd.com/article/8981522
   * detailed instruction definition: https://msyksphinz-self.github.io/riscv-isadoc/html/rvi.html#add
   * RISC-V reference card: https://www.cl.cam.ac.uk/teaching/1617/ECAD+Arch/files/docs/RISCVGreenCardv8-20151013.pdf
-  
+
 ## TODO:
  * Correctly handle 12 and 20 bit immediate (currently not limited to bits at all)
  * Add a cycle limit to the options and CPU to catch infinite loops
  * Move away from `print` and use `logging.logger` instead
  * Writer proper tests
-
```

### Comparing `riscemu-2.0.5/README.md` & `riscemu-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 or [riscemu.datenvorr.at](https://riscemu.datenvorr.at/index.html).
 
 This emulator contains:
 * RISC-V Assembly parser
 * RISC-V Assembly loader
 * Emulation for most parts of the basic RISC-V instruction set and the M and A extensions
 * Naive memory emulator
-* Basic implementation of some syscalls 
+* Basic implementation of some syscalls
 * A debugging environment
 
 ## Installation:
 
 ```bash
 $ pip install riscemu
 ```
@@ -29,15 +29,15 @@
 Hello world
 
 Program exited with code 0
 ```
 
 If you want to run it from a python script, here is [an online demo](https://AntonLydike.github.io/riscemu/lab/index.html?path=PythonDemo.ipynb).
 
-The [`read` syscall](docs/syscalls.md) defaults to readline behaviour. Reading "true chunks" (ignoring newlines) is currently not supported.  
+The [`read` syscall](docs/syscalls.md) defaults to readline behaviour. Reading "true chunks" (ignoring newlines) is currently not supported.
 
 See the docs on [asembly](docs/assembly.md) for more detail on how to write assembly code for this emulator.
 See the [list of implemented syscalls](docs/syscalls.md) for more details on how to syscall.
 
 Currently, symbols (such as `main` or `loop`) are looked-up at runtime. This allows for better debugging, I believe.
 
 Basic IO should work, as open, read, write and close are supported for stdin/stdout/stderr and even aribtrary file paths (if enabled)
@@ -67,18 +67,18 @@
                         Options to control syscall behaviour
 fs_access               Allow access to the filesystem
 disable_io              Disallow reading/writing from stdin/stdout/stderr
 
 --instruction-sets INSTRUCTION_SETS: (-is)
                         A list of comma separated instruction sets you want to load:
                         Currently implemented: RV32I, RV32M
-``` 
+```
 
-If multiple files are specified, all are loaded into memeory, but only the last one is executed. This might be improved 
-later, maybe the `_init` section of each binary is executed before the main loop starts? 
+If multiple files are specified, all are loaded into memeory, but only the last one is executed. This might be improved
+later, maybe the `_init` section of each binary is executed before the main loop starts?
 
 If `stack_size` is greater than zero, a stack is allocated and initialized, with the `sp` register pointing to the end of the stack.
 
 
 ## Debugging
 Debugging is done using the `ebreak` (formerly `sbreak`) instruction, which will launch a debugging session if encountered.
 See [docs/debugging.md](docs/debugging.md) for more info.
@@ -86,21 +86,21 @@
 ![debuggin the fibs program](docs/debug-session.png)
 
 
 ## The source code:
 Check out the [documentation](https://riscemu.readthedocs.io/en/latest/riscemu.html).
 
 ## Accessing local documentation:
-To generate your local documentation, first install everything in `sphinx-docs/requirements.txt`. Then run `./generate-docs.sh`, which will 
+To generate your local documentation, first install everything in `sphinx-docs/requirements.txt`. Then run `./generate-docs.sh`, which will
 generate and make all doc files for you. Finally, you can open the docs locall by runnint `open sphinx-docs/build/html/index.html`.
 
 ## Resources:
+  * RISC-V Programmers Handbook: https://github.com/riscv-non-isa/riscv-asm-manual/blob/master/riscv-asm.md
   * Pseudo ops: https://www.codetd.com/article/8981522
   * detailed instruction definition: https://msyksphinz-self.github.io/riscv-isadoc/html/rvi.html#add
   * RISC-V reference card: https://www.cl.cam.ac.uk/teaching/1617/ECAD+Arch/files/docs/RISCVGreenCardv8-20151013.pdf
-  
+
 ## TODO:
  * Correctly handle 12 and 20 bit immediate (currently not limited to bits at all)
  * Add a cycle limit to the options and CPU to catch infinite loops
  * Move away from `print` and use `logging.logger` instead
  * Writer proper tests
-
```

### Comparing `riscemu-2.0.5/riscemu/CPU.py` & `riscemu-2.1.0/riscemu/CPU.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 class UserModeCPU(CPU):
     """
     This class represents a single CPU. It holds references to it's mmu, registers and syscall interrupt handler.
 
     It is initialized with a configuration and a list of instruction sets.
     """
 
-    def __init__(self, instruction_sets: List[Type['riscemu.InstructionSet']], conf: RunConfig):
+    def __init__(
+        self, instruction_sets: List[Type["riscemu.InstructionSet"]], conf: RunConfig
+    ):
         """
         Creates a CPU instance.
 
         :param instruction_sets: A list of instruction set classes. These must inherit from the InstructionSet class
         """
         # setup CPU states
         super().__init__(MMU(), instruction_sets, conf)
@@ -45,78 +47,92 @@
         self.syscall_int = SyscallInterface()
 
         # add global syscall symbols, but don't overwrite any user-defined symbols
         syscall_symbols = get_syscall_symbols()
         syscall_symbols.update(self.mmu.global_symbols)
         self.mmu.global_symbols.update(syscall_symbols)
 
-    def step(self, verbose=False):
+    def step(self, verbose: bool = False):
         """
         Execute a single instruction, then return.
         """
         if self.halted:
-            print(FMT_CPU + "[CPU] Program exited with code {}".format(self.exit_code) + FMT_NONE)
+            print(
+                FMT_CPU
+                + "[CPU] Program exited with code {}".format(self.exit_code)
+                + FMT_NONE
+            )
             return
 
         launch_debugger = False
 
         try:
             self.cycle += 1
             ins = self.mmu.read_ins(self.pc)
             if verbose:
-                print(FMT_CPU + "   Running 0x{:08X}:{} {}".format(self.pc, FMT_NONE, ins))
+                print(
+                    FMT_CPU + "   Running 0x{:08X}:{} {}".format(self.pc, FMT_NONE, ins)
+                )
             self.pc += self.INS_XLEN
             self.run_instruction(ins)
         except RiscemuBaseException as ex:
             if isinstance(ex, LaunchDebuggerException):
                 # if the debugger is active, raise the exception to
                 if self.debugger_active:
                     raise ex
 
-                print(FMT_CPU + '[CPU] Debugger launch requested!' + FMT_NONE)
+                print(FMT_CPU + "[CPU] Debugger launch requested!" + FMT_NONE)
                 launch_debugger = True
             else:
                 print(ex.message())
                 ex.print_stacktrace()
-                print(FMT_CPU + '[CPU] Halting due to exception!' + FMT_NONE)
+                print(FMT_CPU + "[CPU] Halting due to exception!" + FMT_NONE)
                 self.halted = True
 
         if launch_debugger:
             launch_debug_session(self)
 
-    def run(self, verbose=False):
+    def run(self, verbose: bool = False):
         while not self.halted:
             self.step(verbose)
 
         if self.conf.verbosity > 0:
-            print(FMT_CPU + "[CPU] Program exited with code {}".format(self.exit_code) + FMT_NONE)
+            print(
+                FMT_CPU
+                + "[CPU] Program exited with code {}".format(self.exit_code)
+                + FMT_NONE
+            )
 
-    def setup_stack(self, stack_size=1024 * 4) -> bool:
+    def setup_stack(self, stack_size: int = 1024 * 4) -> bool:
         """
         Create program stack and populate stack pointer
         :param stack_size: the size of the required stack, defaults to 4Kib
         :return:
         """
         stack_sec = BinaryDataMemorySection(
             bytearray(stack_size),
-            '.stack',
+            ".stack",
             None,  # FIXME: why does a binary data memory section require a context?
-            '',
-            0
+            "",
+            0,
         )
 
         if not self.mmu.load_section(stack_sec, fixed_position=False):
             print(FMT_ERROR + "[CPU] Could not insert stack section!" + FMT_NONE)
             return False
 
-        self.regs.set('sp', Int32(stack_sec.base + stack_sec.size))
+        self.regs.set("sp", Int32(stack_sec.base + stack_sec.size))
 
         if self.conf.verbosity > 1:
-            print(FMT_CPU + "[CPU] Created stack of size {} at 0x{:x}".format(
-                stack_size, stack_sec.base
-            ) + FMT_NONE)
+            print(
+                FMT_CPU
+                + "[CPU] Created stack of size {} at 0x{:x}".format(
+                    stack_size, stack_sec.base
+                )
+                + FMT_NONE
+            )
 
         return True
 
     @classmethod
     def get_loaders(cls) -> typing.Iterable[Type[ProgramLoader]]:
         return [AssemblyFileLoader]
```

### Comparing `riscemu-2.0.5/riscemu/IO/TextIO.py` & `riscemu-2.1.0/riscemu/IO/TextIO.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,38 +4,40 @@
 
 
 class TextIO(IOModule):
     def read_ins(self, offset: T_RelativeAddress) -> Instruction:
         raise InstructionAccessFault(self.base + offset)
 
     def __init__(self, base: int, buflen: int = 128):
-        super(TextIO, self).__init__('TextIO', MemoryFlags(False, False), buflen + 4, base=base)
+        super(TextIO, self).__init__(
+            "TextIO", MemoryFlags(False, False), buflen + 4, base=base
+        )
         self.buff = bytearray(buflen)
         self.current_line = ""
 
     def read(self, addr: int, size: int) -> bytearray:
         raise InstructionAccessFault(self.base + addr)
 
     def write(self, addr: int, size: int, data: bytearray):
         if addr == 0:
             if size > 4:
                 raise InstructionAccessFault(addr)
             if Int32(data) != 0:
                 self._print()
                 return
         buff_start = addr - 4
-        self.buff[buff_start:buff_start + size] = data[0:size]
+        self.buff[buff_start : buff_start + size] = data[0:size]
 
     def _print(self):
         buff = self.buff
         self.buff = bytearray(self.size)
-        if b'\x00' in buff:
-            buff = buff.split(b'\x00')[0]
-        text = buff.decode('ascii')
-        if '\n' in text:
+        if b"\x00" in buff:
+            buff = buff.split(b"\x00")[0]
+        text = buff.decode("ascii")
+        if "\n" in text:
             lines = text.split("\n")
             lines[0] = self.current_line + lines[0]
             for line in lines[:-1]:
                 self._present(line)
             self.current_line = lines[-1]
         else:
             self.current_line += text
```

### Comparing `riscemu-2.0.5/riscemu/MMU.py` & `riscemu-2.1.0/riscemu/MMU.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,24 @@
 SPDX-License-Identifier: MIT
 """
 
 from typing import Dict, List, Optional, Union
 
 from .colors import *
 from .helpers import align_addr
-from .types import Instruction, MemorySection, MemoryFlags, T_AbsoluteAddress, \
-    Program, InstructionContext, Int32
+from .types import (
+    Instruction,
+    MemorySection,
+    MemoryFlags,
+    T_AbsoluteAddress,
+    Program,
+    InstructionContext,
+    Int32,
+    Float32,
+)
 from .types.exceptions import InvalidAllocationException, MemoryAccessException
 
 
 class MMU:
     """
     The MemoryManagementUnit. This provides a unified interface for reading/writing data from/to memory.
 
@@ -61,135 +69,182 @@
         :return: The LoadedMemorySection or None
         """
         for sec in self.sections:
             if sec.base <= addr < sec.base + sec.size:
                 return sec
         return None
 
-    def get_bin_containing(self, addr: T_AbsoluteAddress) -> Optional[Program]:
+    def get_program_at_addr(self, addr: T_AbsoluteAddress) -> Optional[Program]:
         for program in self.programs:
             if program.base <= addr < program.base + program.size:
                 return program
         return None
 
     def read_ins(self, addr: T_AbsoluteAddress) -> Instruction:
         """
         Read a single instruction located at addr
 
         :param addr: The location
         :return: The Instruction
         """
         sec = self.get_sec_containing(addr)
         if sec is None:
-            print(FMT_MEM + "[MMU] Trying to read instruction form invalid region! (read at {}) ".format(addr)
-                  + "Have you forgotten an exit syscall or ret statement?" + FMT_NONE)
+            print(
+                FMT_MEM
+                + "[MMU] Trying to read instruction form invalid region! (read at {}) ".format(
+                    addr
+                )
+                + "Have you forgotten an exit syscall or ret statement?"
+                + FMT_NONE
+            )
             raise RuntimeError("No next instruction available!")
         return sec.read_ins(addr - sec.base)
 
     def read(self, addr: Union[int, Int32], size: int) -> bytearray:
         """
         Read size bytes of memory at addr
 
         :param addr: The addres at which to start reading
         :param size: The number of bytes to read
         :return: The bytearray at addr
         """
         if isinstance(addr, Int32):
-            breakpoint()
             addr = addr.unsigned_value
         sec = self.get_sec_containing(addr)
         if sec is None:
-            print(FMT_MEM + "[MMU] Trying to read data form invalid region at 0x{:x}! ".format(addr) + FMT_NONE)
-            raise MemoryAccessException("region is non-initialized!", addr, size, 'read')
+            print(
+                FMT_MEM
+                + "[MMU] Trying to read data form invalid region at 0x{:x}! ".format(
+                    addr
+                )
+                + FMT_NONE
+            )
+            raise MemoryAccessException(
+                "region is non-initialized!", addr, size, "read"
+            )
         return sec.read(addr - sec.base, size)
 
     def write(self, addr: int, size: int, data: bytearray):
         """
         Write bytes into memory
 
         :param addr: The address at which to write
         :param size: The number of bytes to write
         :param data: The bytearray to write (only first size bytes are written)
         """
         sec = self.get_sec_containing(addr)
         if sec is None:
-            print(FMT_MEM + '[MMU] Invalid write into non-initialized region at 0x{:08X}'.format(addr) + FMT_NONE)
-            raise MemoryAccessException("region is non-initialized!", addr, size, 'write')
+            print(
+                FMT_MEM
+                + "[MMU] Invalid write into non-initialized region at 0x{:08X}".format(
+                    addr
+                )
+                + FMT_NONE
+            )
+            raise MemoryAccessException(
+                "region is non-initialized!", addr, size, "write"
+            )
 
         return sec.write(addr - sec.base, size, data)
 
     def dump(self, addr, *args, **kwargs):
         """
         Dumpy the memory contents
 
         :param addr: The address at which to dump
         :param args: args for the dump function of the loaded memory section
         :param kwargs: kwargs for the dump function of the loaded memory section
         """
         sec = self.get_sec_containing(addr)
         if sec is None:
-            print(FMT_MEM + "[MMU] No section containing addr 0x{:08X}".format(addr) + FMT_NONE)
+            print(
+                FMT_MEM
+                + "[MMU] No section containing addr 0x{:08X}".format(addr)
+                + FMT_NONE
+            )
             return
         sec.dump(addr - sec.base, *args, **kwargs)
 
     def label(self, symb: str):
         """
         Look up the symbol symb in all local symbol tables (and the global one)
 
         :param symb: The symbol name to look up
         """
         print(FMT_MEM + "[MMU] Lookup for symbol {}:".format(symb) + FMT_NONE)
         if symb in self.global_symbols:
-            print("   Found global symbol {}: 0x{:X}".format(symb, self.global_symbols[symb]))
+            print(
+                "   Found global symbol {}: 0x{:X}".format(
+                    symb, self.global_symbols[symb]
+                )
+            )
         for bin in self.programs:
             if symb in bin.context.labels:
-                print("   Found local labels {}: 0x{:X} in {}".format(symb, bin.context.labels[symb], bin.name))
+                print(
+                    "   Found local labels {}: 0x{:X} in {}".format(
+                        symb, bin.context.labels[symb], bin.name
+                    )
+                )
 
     def read_int(self, addr: int) -> Int32:
         return Int32(self.read(addr, 4))
 
+    def read_float(self, addr: int) -> Float32:
+        return Float32(self.read(addr, 4))
+
     def translate_address(self, address: T_AbsoluteAddress) -> str:
         sec = self.get_sec_containing(address)
         if not sec:
             return "unknown at 0x{:0x}".format(address)
 
-        bin = self.get_bin_containing(address)
+        bin = self.get_program_at_addr(address)
         secs = set(sec.name for sec in bin.sections) if bin else []
         elf_markers = {
-            '__global_pointer$', '_fdata', '_etext', '_gp',
-            '_bss_start', '_bss_end', '_ftext', '_edata', '_end', '_fbss'
+            "__global_pointer$",
+            "_fdata",
+            "_etext",
+            "_gp",
+            "_bss_start",
+            "_bss_end",
+            "_ftext",
+            "_edata",
+            "_end",
+            "_fbss",
         }
 
         def key(x):
             name, val = x
             return address - val
 
-        best_fit = sorted(filter(lambda x: x[1] <= address, sec.context.labels.items()), key=key)
+        best_fit = sorted(
+            filter(lambda x: x[1] <= address, sec.context.labels.items()), key=key
+        )
 
-        best = ('', float('inf'))
+        best = ("", float("inf"))
         for name, val in best_fit:
             if address - val < best[1]:
                 best = (name, val)
             if address - val == best[1]:
                 if best[0] in elf_markers:
                     best = (name, val)
                 elif best[0] in secs and name not in elf_markers:
                     best = (name, val)
 
         name, val = best
 
         if not name:
             return "{}:{} + 0x{:x} (0x{:x})".format(
-                sec.owner, sec.name,
-                address - sec.base, address
+                sec.owner, sec.name, address - sec.base, address
             )
 
-        return str('{}:{} at {} (0x{:0x}) + 0x{:0x}'.format(
-            sec.owner, sec.name, name, val, address - val
-        ))
+        return str(
+            "{}:{} at {} (0x{:0x}) + 0x{:0x}".format(
+                sec.owner, sec.name, name, val, address - val
+            )
+        )
 
     def has_continous_free_region(self, start: int, end: int) -> bool:
         # if we have no sections we are all good
         if len(self.sections) == 0:
             return True
         # if the last section is located before the start we are also good
         if start >= self.sections[-1].base + self.sections[-1].size:
@@ -207,21 +262,32 @@
             return False
         # if all sections end before the requested start we are good
         # technically we shouldn't ever reach this point, but better safe than sorry
         return True
 
     def load_program(self, program: Program, align_to: int = 4):
         if program.base is not None:
-            if not self.has_continous_free_region(program.base, program.base + program.size):
-                print(FMT_MEM + "Cannot load program {} into desired space (0x{:0x}-0x{:0x}), area occupied.".format(
-                    program.name, program.base, program.base + program.size
-                ) + FMT_NONE)
-                raise InvalidAllocationException("Area occupied".format(
-                    program.name, program.base, program.base + program.size
-                ), program.name, program.size, MemoryFlags(False, True))
+            if not self.has_continous_free_region(
+                program.base, program.base + program.size
+            ):
+                print(
+                    FMT_MEM
+                    + "Cannot load program {} into desired space (0x{:0x}-0x{:0x}), area occupied.".format(
+                        program.name, program.base, program.base + program.size
+                    )
+                    + FMT_NONE
+                )
+                raise InvalidAllocationException(
+                    "Area occupied".format(
+                        program.name, program.base, program.base + program.size
+                    ),
+                    program.name,
+                    program.size,
+                    MemoryFlags(False, True),
+                )
 
             at_addr = program.base
         else:
             at_addr = align_addr(self.get_guaranteed_free_address(), align_to)
 
         # trigger the load event to set all addresses in the binary
         program.loaded_trigger(at_addr)
@@ -241,22 +307,27 @@
 
     def load_section(self, sec: MemorySection, fixed_position: bool = False) -> bool:
         if fixed_position:
             if self.has_continous_free_region(sec.base, sec.base + sec.size):
                 self.sections.append(sec)
                 self._update_state()
             else:
-                print(FMT_MEM + '[MMU] Cannot place section {} at {}, space is occupied!'.format(sec, sec.base))
+                print(
+                    FMT_MEM
+                    + "[MMU] Cannot place section {} at {}, space is occupied!".format(
+                        sec, sec.base
+                    )
+                )
                 return False
         else:
             at_addr = align_addr(self.get_guaranteed_free_address(), 8)
             sec.base = at_addr
             self.sections.append(sec)
             self._update_state()
-            return True
+        return True
 
     def _update_state(self):
         """
         Called whenever a section or program is added to keep the list of programs and sections consistent
         :return:
         """
         self.programs.sort(key=lambda bin: bin.base)
@@ -266,29 +337,27 @@
         if len(self.sections) == 0:
             return 0x100
         else:
             return self.sections[-1].base + self.sections[-1].size
 
     def __repr__(self):
         return "{}(\n\t{}\n)".format(
-            self.__class__.__name__,
-            "\n\t".join(repr(x) for x in self.programs)
+            self.__class__.__name__, "\n\t".join(repr(x) for x in self.programs)
         )
 
     def context_for(self, addr: T_AbsoluteAddress) -> InstructionContext:
         sec = self.get_sec_containing(addr)
 
         if sec is not None:
             return sec.context
 
         return InstructionContext()
 
-    def report_addr(self, addr: T_AbsoluteAddress):
-        sec = self.get_sec_containing(addr)
-        if not sec:
-            print("addr is in no section!")
-            return
-        owner = [b for b in self.programs if b.name == sec.owner]
-        if owner:
-            print("owned by: {}".format(owner[0]))
-
-        print("{}: 0x{:0x} + 0x{:0x}".format(name, val, addr - val))
+    def find_entrypoint(self) -> Optional[int]:
+        # try to find the global entrypoint
+        if "_start" in self.global_symbols:
+            return self.global_symbols["_start"]
+        # otherwise find a main (that's not necessarily global)
+        for p in self.programs:
+            if "main" in p.context.labels:
+                return p.context.resolve_label("main")
+        return None
```

### Comparing `riscemu-2.0.5/riscemu/__init__.py` & `riscemu-2.1.0/riscemu/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,34 @@
 SPDX-License-Identifier: MIT
 
 This package aims at providing an all-round usable RISC-V emulator and debugger
 
 It contains everything needed to run assembly files, so you don't need any custom compilers or toolchains
 """
 
-from .types.exceptions import RiscemuBaseException, LaunchDebuggerException, InvalidSyscallException, LinkerException, \
-    ParseException, NumberFormatException, InvalidRegisterException, MemoryAccessException, OutOfMemoryException
+from .types.exceptions import (
+    RiscemuBaseException,
+    LaunchDebuggerException,
+    InvalidSyscallException,
+    LinkerException,
+    ParseException,
+    NumberFormatException,
+    InvalidRegisterException,
+    MemoryAccessException,
+    OutOfMemoryException,
+)
 
 from .instructions import *
 
 from .MMU import MMU
 from .registers import Registers
 from .syscall import SyscallInterface, Syscall
 from .CPU import CPU, UserModeCPU
 from .debug import launch_debug_session
 
 from .config import RunConfig
 
 from .parser import tokenize, parse_tokens, AssemblyFileLoader
 
 __author__ = "Anton Lydike <Anton@Lydike.com>"
-__copyright__ = "Copyright 2022 Anton Lydike"
-__version__ = '2.0.5'
+__copyright__ = "Copyright 2023 Anton Lydike"
+__version__ = "2.1.0"
```

### Comparing `riscemu-2.0.5/riscemu/assembler.py` & `riscemu-2.1.0/riscemu/assembler.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 from typing import List
 from typing import Optional, Tuple, Union
 
 from .colors import FMT_PARSE, FMT_NONE
 from riscemu.types.exceptions import ParseException, ASSERT_LEN
 from .helpers import parse_numeric_argument, align_addr, get_section_base_name
 from .tokenizer import Token
-from .types import Program, T_RelativeAddress, InstructionContext, Instruction, BinaryDataMemorySection, \
-    InstructionMemorySection, Int32
+from .types import (
+    Program,
+    T_RelativeAddress,
+    InstructionContext,
+    Instruction,
+    BinaryDataMemorySection,
+    InstructionMemorySection,
+    Int32,
+)
 
-INSTRUCTION_SECTION_NAMES = ('.text', '.init', '.fini')
+INSTRUCTION_SECTION_NAMES = (".text", ".init", ".fini")
 """
 A tuple containing all section names which contain executable code (instead of data)
 
 The first segment of each segment (first segment of ".text.main" is ".text") is checked
 against this list to determine the type of it.
 """
 
@@ -43,16 +50,15 @@
     def current_address(self) -> T_RelativeAddress:
         if self.type == MemorySectionType.Data:
             return len(self.data) + self.base
         return len(self.data) * 4 + self.base
 
     def __repr__(self):
         return "{}(name={},data={},type={})".format(
-            self.__class__.__name__, self.name,
-            self.data, self.type.name
+            self.__class__.__name__, self.name, self.data, self.type.name
         )
 
 
 class ParseContext:
     section: Optional[CurrentSection]
     context: InstructionContext
     program: Program
@@ -68,32 +74,42 @@
 
     def _finalize_section(self):
         if self.section is None:
             return
 
         if self.section.type == MemorySectionType.Data:
             section = BinaryDataMemorySection(
-                self.section.data, self.section.name, self.context, self.program.name, self.section.base
+                self.section.data,
+                self.section.name,
+                self.context,
+                self.program.name,
+                self.section.base,
             )
             self.program.add_section(section)
         elif self.section.type == MemorySectionType.Instructions:
             section = InstructionMemorySection(
-                self.section.data, self.section.name, self.context, self.program.name, self.section.base
+                self.section.data,
+                self.section.name,
+                self.context,
+                self.program.name,
+                self.section.base,
             )
             self.program.add_section(section)
 
         self.section = None
 
     def new_section(self, name: str, type: MemorySectionType, alignment: int = 4):
         base = align_addr(self.current_address(), alignment)
 
         self._finalize_section()
         self.section = CurrentSection(name, type, base)
 
-    def add_label(self, name: str, value: int, is_global: bool = False, is_relative: bool = False):
+    def add_label(
+        self, name: str, value: int, is_global: bool = False, is_relative: bool = False
+    ):
         self.context.labels[name] = value
         if is_global:
             self.program.global_labels.add(name)
         if is_relative:
             self.program.relative_labels.add(name)
 
     def current_address(self):
@@ -105,18 +121,24 @@
         return "{}(\n\tsetion={},\n\tprogram={}\n)".format(
             self.__class__.__name__, self.section, self.program
         )
 
 
 def ASSERT_IN_SECTION_TYPE(context: ParseContext, type: MemorySectionType):
     if context.section is None:
-        raise ParseException('Error, expected to be in {} section, but no section is present...'.format(type.name))
+        raise ParseException(
+            "Error, expected to be in {} section, but no section is present...".format(
+                type.name
+            )
+        )
     if context.section.type != type:
         raise ParseException(
-            'Error, expected to be in {} section, but currently in {}...'.format(type.name, context.section)
+            "Error, expected to be in {} section, but currently in {}...".format(
+                type.name, context.section
+            )
         )
 
 
 class AssemblerDirectives:
     """
     This class represents a collection of all assembler directives as documented by
     https://github.com/riscv-non-isa/riscv-asm-manual/blob/master/riscv-asm.md#pseudo-ops
@@ -170,51 +192,65 @@
     def op_zero(cls, token: Token, args: Tuple[str], context: ParseContext):
         ASSERT_LEN(args, 1)
         ASSERT_IN_SECTION_TYPE(context, MemorySectionType.Data)
         size = parse_numeric_argument(args[0])
         cls.add_bytes(size, bytearray(size), context)
 
     @classmethod
-    def add_bytes(cls, size: int, content: Union[None, int, bytearray], context: ParseContext):
+    def add_bytes(
+        cls, size: int, content: Union[None, int, bytearray], context: ParseContext
+    ):
         ASSERT_IN_SECTION_TYPE(context, MemorySectionType.Data)
 
         if content is None:
             content = bytearray(size)
         if isinstance(content, int):
             content = Int32(content).to_bytes(size)
 
         context.section.data += content
 
     @classmethod
     def add_text(cls, text: str, context: ParseContext, zero_terminate: bool = True):
         # replace '\t' and '\n' escape sequences
-        text = text.replace('\\n', '\n').replace('\\t', '\t')
+        text = text.replace("\\n", "\n").replace("\\t", "\t")
 
-        encoded_bytes = bytearray(text.encode('ascii'))
+        encoded_bytes = bytearray(text.encode("ascii"))
         if zero_terminate:
             encoded_bytes += bytearray(1)
         cls.add_bytes(len(encoded_bytes), encoded_bytes, context)
 
     @classmethod
     def handle_instruction(cls, token: Token, args: Tuple[str], context: ParseContext):
         op = token.value[1:]
-        if hasattr(cls, 'op_' + op):
-            getattr(cls, 'op_' + op)(token, args, context)
-        elif op in ('text', 'data', 'rodata', 'bss', 'sbss'):
+        if hasattr(cls, "op_" + op):
+            getattr(cls, "op_" + op)(token, args, context)
+        elif op in ("text", "data", "rodata", "bss", "sbss"):
             cls.op_section(token, (token.value,), context)
-        elif op in ('string', 'asciiz', 'asciz', 'ascii'):
+        elif op in ("string", "asciiz", "asciz", "ascii"):
             ASSERT_LEN(args, 1)
-            cls.add_text(args[0], context, op == 'ascii')
+            cls.add_text(args[0], context, zero_terminate=(op != "ascii"))
         elif op in DATA_OP_SIZES:
             size = DATA_OP_SIZES[op]
             for arg in args:
                 cls.add_bytes(size, parse_numeric_argument(arg), context)
         else:
-            print(FMT_PARSE + "Unknown assembler directive: {} {} in {}".format(token, args, context) + FMT_NONE)
+            print(
+                FMT_PARSE
+                + "Unknown assembler directive: {} {} in {}".format(
+                    token, args, context
+                )
+                + FMT_NONE
+            )
 
 
 DATA_OP_SIZES = {
-    'byte': 1,
-    '2byte': 2, 'half': 2, 'short': 2,
-    '4byte': 4, 'word': 4, 'long': 4,
-    '8byte': 8, 'dword': 8, 'quad': 8,
+    "byte": 1,
+    "2byte": 2,
+    "half": 2,
+    "short": 2,
+    "4byte": 4,
+    "word": 4,
+    "long": 4,
+    "8byte": 8,
+    "dword": 8,
+    "quad": 8,
 }
```

### Comparing `riscemu-2.0.5/riscemu/config.py` & `riscemu-2.1.0/riscemu/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     debug_on_exception: bool = True
     # allowed syscalls
     scall_input: bool = True
     scall_fs: bool = False
     verbosity: int = 0
     slowdown: float = 1
     unlimited_registers: bool = False
-
-
-CONFIG = RunConfig()
+    # runtime config
+    use_libc: bool = False
+    ignore_exit_code: bool = False
```

### Comparing `riscemu-2.0.5/riscemu/debug.py` & `riscemu-2.1.0/riscemu/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 from .types import SimpleInstruction
 from .helpers import *
 
 if typing.TYPE_CHECKING:
     from riscemu import CPU, Registers
 
-HIST_FILE = os.path.join(os.path.expanduser('~'), '.riscemu_history')
+HIST_FILE = os.path.join(os.path.expanduser("~"), ".riscemu_history")
 
 
-def launch_debug_session(cpu: 'CPU', prompt=""):
+def launch_debug_session(cpu: "CPU", prompt=""):
     if cpu.debugger_active:
         return
     import code
     import readline
     import rlcompleter
 
     # set the active debug flag
@@ -35,39 +35,35 @@
     def dump(what, *args, **kwargs):
         if what == regs:
             regs.dump(*args, **kwargs)
         else:
             mmu.dump(what, *args, **kwargs)
 
     def dump_stack(*args, **kwargs):
-        mmu.dump(regs.get('sp'), *args, **kwargs)
+        mmu.dump(regs.get("sp"), *args, **kwargs)
 
     def ins():
         print("Current instruction at 0x{:08X}:".format(cpu.pc))
         return mmu.read_ins(cpu.pc)
 
     def run_ins(name, *args: str):
         if len(args) > 3:
             print("Invalid arg count!")
             return
         context = mmu.context_for(cpu.pc)
 
-        ins = SimpleInstruction(
-            name,
-            tuple(args),
-            context,
-            cpu.pc)
+        ins = SimpleInstruction(name, tuple(args), context, cpu.pc)
         print(FMT_DEBUG + "Running instruction {}".format(ins) + FMT_NONE)
         cpu.run_instruction(ins)
 
     def cont(verbose=False):
         try:
             cpu.run(verbose)
         except LaunchDebuggerException:
-            print(FMT_DEBUG + 'Returning to debugger...')
+            print(FMT_DEBUG + "Returning to debugger...")
             return
 
     def step():
         try:
             cpu.step()
         except LaunchDebuggerException:
             return
@@ -88,8 +84,7 @@
         code.InteractiveConsole(sess_vars).interact(
             banner=FMT_DEBUG + prompt + FMT_NONE,
             exitmsg="Exiting debugger",
         )
     finally:
         cpu.debugger_active = False
         readline.write_history_file(HIST_FILE)
-
```

### Comparing `riscemu-2.0.5/riscemu/decoder/__main__.py` & `riscemu-2.1.0/riscemu/decoder/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-if __name__ == '__main__':
+if __name__ == "__main__":
     import code
     import readline
     import rlcompleter
 
     from .decoder import *
     from .formats import *
     from .instruction_table import *
@@ -10,8 +10,10 @@
 
     sess_vars = globals()
     sess_vars.update(locals())
 
     readline.set_completer(rlcompleter.Completer(sess_vars).complete)
     readline.set_completer(rlcompleter.Completer(sess_vars).complete)
     readline.parse_and_bind("tab: complete")
-    code.InteractiveConsole(sess_vars).interact(banner="Interaktive decoding session started...", exitmsg="Closing...")
+    code.InteractiveConsole(sess_vars).interact(
+        banner="Interaktive decoding session started...", exitmsg="Closing..."
+    )
```

### Comparing `riscemu-2.0.5/riscemu/decoder/decoder.py` & `riscemu-2.1.0/riscemu/decoder/decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from .instruction_table import *
 from typing import Tuple, List
 
 
 def print_ins(ins: int):
     print("  f7      rs2   rs1   f3  rd    op")
     print(
-        f"0b{ins >> 25 :07b}_{(ins >> 20) & 0b11111:05b}_{(ins >> 15) & 0b11111:05b}_{(ins >> 12) & 0b111:03b}_{(ins >> 7) & 0b11111:05b}_{ins & 0b1111111:07b}");
+        f"0b{ins >> 25 :07b}_{(ins >> 20) & 0b11111:05b}_{(ins >> 15) & 0b11111:05b}_{(ins >> 12) & 0b111:03b}_{(ins >> 7) & 0b11111:05b}_{ins & 0b1111111:07b}"
+    )
 
 
 STATIC_INSN: Dict[int, Tuple[str, List[int], int]] = {
     0x00000013: ("nop", [], 0x00000013),
     0x00008067: ("ret", [], 0x00008067),
-    0xfe010113: ("addi", [2, 2, -32], 0xfe010113),
+    0xFE010113: ("addi", [2, 2, -32], 0xFE010113),
     0x02010113: ("addi", [2, 2, 32], 0x02010113),
     0x00100073: ("ebreak", [], 0x00100073),
     0x00000073: ("ecall", [], 0x00000073),
     0x30200073: ("mret", [], 0x30200073),
     0x00200073: ("uret", [], 0x00200073),
     0x10200073: ("sret", [], 0x10200073),
     0x10500073: ("wfi", [], 0x10500073),
 }
 
 
 def int_from_ins(insn: bytearray):
-    return int.from_bytes(insn, 'little')
+    return int.from_bytes(insn, "little")
 
 
 def name_from_insn(ins: int):
     opcode = op(ins)
     if opcode not in RV32:
         print_ins(ins)
         raise RuntimeError(f"Invalid opcode: {opcode:0x} in insn {ins:x}")
@@ -41,15 +42,15 @@
         print_ins(ins)
         raise RuntimeError(f"Invalid funct3: {fun3:0x} in insn {ins:x}")
 
     dec = dec[fun3]
     if isinstance(dec, str):
         return dec
 
-    if opcode == 0x1c and fun3 == 0:
+    if opcode == 0x1C and fun3 == 0:
         # we have ecall/ebreak
         token = imm110(ins)
         if token in dec:
             return dec[token]
         print_ins(ins)
         raise RuntimeError(f"Invalid instruction in ebreak/ecall region: {ins:x}")
```

### Comparing `riscemu-2.0.5/riscemu/decoder/formats.py` & `riscemu-2.1.0/riscemu/decoder/formats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, Callable, List, Union
 from .regs import RISCV_REGS
 
+
 def op(ins: int):
     return (ins >> 2) & 31
 
 
 def rd(ins: int):
     return (ins >> 7) & 31
 
@@ -42,28 +43,34 @@
     return sign_extend(num, 12)
 
 
 def imm_b(ins: int):
     lower = rd(ins)
     higher = funct7(ins)
 
-    num = (lower & 0b11110) + ((higher & 0b0111111) << 5) + ((lower & 1) << 11) + ((higher >> 6) << 12)
+    num = (
+        (lower & 0b11110)
+        + ((higher & 0b0111111) << 5)
+        + ((lower & 1) << 11)
+        + ((higher >> 6) << 12)
+    )
     return sign_extend(num, 13)
 
 
 def imm_u(ins: int):
     return sign_extend(imm3112(ins), 20)
 
 
 def imm_j(ins: int):
     return sign_extend(
-        (((ins >> 21) & 0b1111111111) << 1) +
-        (((ins >> 20) & 1) << 11) +
-        (((ins >> 12) & 0b11111111) << 12) +
-        (((ins >> 31) & 1) << 20), 21
+        (((ins >> 21) & 0b1111111111) << 1)
+        + (((ins >> 20) & 1) << 11)
+        + (((ins >> 12) & 0b11111111) << 12)
+        + (((ins >> 31) & 1) << 20),
+        21,
     )
 
 
 def sign_extend(num, bits):
     sign_mask = 1 << (bits - 1)
     return (num & (sign_mask - 1)) - (num & sign_mask)
 
@@ -107,11 +114,11 @@
     0x04: decode_i_shamt,
     0x05: decode_u,
     0x08: decode_s,
     0x0C: decode_r,
     0x0D: decode_u,
     0x18: decode_b,
     0x19: decode_i,
-    0x1b: decode_j,
-    0x1c: decode_i_unsigned,
-    0b1011: decode_r
+    0x1B: decode_j,
+    0x1C: decode_i_unsigned,
+    0b1011: decode_r,
 }
```

### Comparing `riscemu-2.0.5/riscemu/decoder/formatter.py` & `riscemu-2.1.0/riscemu/decoder/formatter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,40 @@
-from .formats import INSTRUCTION_ARGS_DECODER, op, decode_i, decode_r, decode_u, decode_b, decode_j, decode_s, \
-    decode_i_shamt, decode_i_unsigned
+from .formats import (
+    INSTRUCTION_ARGS_DECODER,
+    op,
+    decode_i,
+    decode_r,
+    decode_u,
+    decode_b,
+    decode_j,
+    decode_s,
+    decode_i_shamt,
+    decode_i_unsigned,
+)
 from .regs import RISCV_REGS
 
 
 def int_to_hex(num: int):
     if num < 0:
         return f"-0x{-num:x}"
     return f"0x{num:x}"
 
 
-def format_ins(ins: int, name: str, fmt: str = 'int'):
+def format_ins(ins: int, name: str, fmt: str = "int"):
     opcode = op(ins)
-    if fmt == 'hex':
+    if fmt == "hex":
         fmt = int_to_hex
     else:
         fmt = str
 
     if opcode not in INSTRUCTION_ARGS_DECODER:
         return f"{name} <unknown op>"
 
     decoder = INSTRUCTION_ARGS_DECODER[opcode]
-    if name in ('ecall', 'ebreak', 'mret', 'sret', 'uret'):
+    if name in ("ecall", "ebreak", "mret", "sret", "uret"):
         return name
     if opcode in (0x8, 0x0):
         r1, r2, imm = decoder(ins)
         return f"{name:<7} {RISCV_REGS[r1]}, {imm}({RISCV_REGS[r2]})"
     elif decoder in (decode_i, decode_i_unsigned, decode_b, decode_i_shamt, decode_s):
         r1, r2, imm = decoder(ins)
         r1, r2 = RISCV_REGS[r1], RISCV_REGS[r2]
```

### Comparing `riscemu-2.0.5/riscemu/decoder/instruction_table.py` & `riscemu-2.1.0/riscemu/decoder/instruction_table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from .formats import *
 
 tbl = lambda: defaultdict(tbl)
 
 RV32 = tbl()
-RV32[0x1b] = "jal"
+RV32[0x1B] = "jal"
 RV32[0x0D] = "lui"
 RV32[0x05] = "auipc"
 RV32[0x19][0] = "jalr"
 
 RV32[0x04][0] = "addi"
 RV32[0x04][1] = "slli"
 RV32[0x04][2] = "slti"
@@ -32,34 +32,34 @@
 RV32[0x00][4] = "lbu"
 RV32[0x00][5] = "lhu"
 
 RV32[0x08][0] = "sb"
 RV32[0x08][1] = "sh"
 RV32[0x08][2] = "sw"
 
-RV32[0x1c][1] = "csrrw"
-RV32[0x1c][2] = "csrrs"
-RV32[0x1c][3] = "csrrc"
-RV32[0x1c][5] = "csrrwi"
-RV32[0x1c][6] = "csrrsi"
-RV32[0x1c][7] = "csrrci"
+RV32[0x1C][1] = "csrrw"
+RV32[0x1C][2] = "csrrs"
+RV32[0x1C][3] = "csrrc"
+RV32[0x1C][5] = "csrrwi"
+RV32[0x1C][6] = "csrrsi"
+RV32[0x1C][7] = "csrrci"
 
-RV32[0x1c][0][0] = "ecall"
-RV32[0x1c][0][1] = "ebreak"
+RV32[0x1C][0][0] = "ecall"
+RV32[0x1C][0][1] = "ebreak"
 
-RV32[0x0C][0][0]  = "add"
+RV32[0x0C][0][0] = "add"
 RV32[0x0C][0][32] = "sub"
-RV32[0x0C][1][0]  = "sll"
-RV32[0x0C][2][0]  = "slt"
-RV32[0x0C][3][0]  = "sltu"
-RV32[0x0C][4][0]  = "xor"
-RV32[0x0C][5][0]  = "srl"
+RV32[0x0C][1][0] = "sll"
+RV32[0x0C][2][0] = "slt"
+RV32[0x0C][3][0] = "sltu"
+RV32[0x0C][4][0] = "xor"
+RV32[0x0C][5][0] = "srl"
 RV32[0x0C][5][32] = "sra"
-RV32[0x0C][6][0]  = "or"
-RV32[0x0C][7][0]  = "and"
+RV32[0x0C][6][0] = "or"
+RV32[0x0C][7][0] = "and"
 
 # rv32m
 RV32[0x0C][0][1] = "mul"
 RV32[0x0C][1][1] = "mulh"
 RV32[0x0C][2][1] = "mulhsu"
 RV32[0x0C][3][1] = "mulhu"
 RV32[0x0C][4][1] = "div"
```

### Comparing `riscemu-2.0.5/riscemu/helpers.py` & `riscemu-2.1.0/riscemu/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,65 +10,75 @@
 from .types import Int32, UInt32
 from .types.exceptions import *
 
 
 def align_addr(addr: int, to_bytes: int = 8) -> int:
     """
     align an address to `to_bytes` (meaning addr & to_bytes = 0)
+
+    This will increase the address
     """
     return addr + (-addr % to_bytes)
 
 
 def parse_numeric_argument(arg: str) -> int:
     """
     parse hex or int strings
     """
     try:
-        if arg.lower().startswith('0x'):
+        if arg.lower().startswith("0x"):
             return int(arg, 16)
         return int(arg)
     except ValueError as ex:
-        raise ParseException('Invalid immediate argument \"{}\", maybe missing symbol?'.format(arg), (arg, ex))
+        raise ParseException(
+            'Invalid immediate argument "{}", maybe missing symbol?'.format(arg),
+            (arg, ex),
+        )
 
 
 def create_chunks(my_list, chunk_size):
     """Split a list like [a,b,c,d,e,f,g,h,i,j,k,l,m] into e.g. [[a,b,c,d],[e,f,g,h],[i,j,k,l],[m]]"""
-    return [my_list[i:i + chunk_size] for i in range(0, len(my_list), chunk_size)]
+    return [my_list[i : i + chunk_size] for i in range(0, len(my_list), chunk_size)]
 
 
 def apply_highlight(item, ind, hi_ind):
     """
     applies some hightlight such as underline to item if ind == hi_ind
     """
     if ind == hi_ind:
         return FMT_UNDERLINE + FMT_ORANGE + item + FMT_NONE
     return item
 
 
 def highlight_in_list(items, hi_ind, joiner=" "):
-    return joiner.join([apply_highlight(item, i, hi_ind) for i, item in enumerate(items)])
+    return joiner.join(
+        [apply_highlight(item, i, hi_ind) for i, item in enumerate(items)]
+    )
 
 
 def format_bytes(byte_arr: bytearray, fmt: str, group: int = 1, highlight: int = -1):
     """Format byte array as per fmt. Group into groups of size `group`, and highlight index `highlight`."""
     chunks = create_chunks(byte_arr, group)
-    if fmt == 'hex':
-        return highlight_in_list(['0x{}'.format(ch.hex()) for ch in chunks], highlight)
-    if fmt == 'int':
+    if fmt == "hex":
+        return highlight_in_list(["0x{}".format(ch.hex()) for ch in chunks], highlight)
+    if fmt == "int":
         spc = str(ceil(log10(2 ** (group * 8 - 1))) + 1)
-        return highlight_in_list([('{:0' + spc + 'd}').format(Int32(ch)) for ch in chunks], highlight)
-    if fmt == 'uint':
+        return highlight_in_list(
+            [("{:0" + spc + "d}").format(Int32(ch)) for ch in chunks], highlight
+        )
+    if fmt == "uint":
         spc = str(ceil(log10(2 ** (group * 8))))
-        return highlight_in_list([('{:0' + spc + 'd}').format(UInt32(ch)) for ch in chunks],
-                                 highlight)
-    if fmt == 'char':
+        return highlight_in_list(
+            [("{:0" + spc + "d}").format(UInt32(ch)) for ch in chunks], highlight
+        )
+    if fmt == "char":
         return highlight_in_list((repr(chr(b))[1:-1] for b in byte_arr), highlight, "")
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class Peekable(Generic[T], Iterator[T]):
     def __init__(self, iterable: Iterable[T]):
         self.iterable = iter(iterable)
         self.cache: List[T] = list()
 
@@ -94,10 +104,14 @@
         self.cache = [item] + self.cache
 
     def is_empty(self) -> bool:
         return self.peek() is None
 
 
 def get_section_base_name(section_name: str) -> str:
-    if '.' not in section_name:
-        print(FMT_PARSE + f"Invalid section {section_name}, not starting with a dot!" + FMT_NONE)
-    return '.' + section_name.split('.')[1]
+    if "." not in section_name:
+        print(
+            FMT_PARSE
+            + f"Invalid section {section_name}, not starting with a dot!"
+            + FMT_NONE
+        )
+    return "." + section_name.split(".")[1]
```

### Comparing `riscemu-2.0.5/riscemu/instructions/RV32A.py` & `riscemu-2.1.0/riscemu/instructions/RV32A.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,73 +6,73 @@
 class RV32A(InstructionSet):
     """
     The RV32A instruction set. Currently, load-reserved and store conditionally are not supported
     due to limitations in the way the MMU is implemented. Maybe a later implementation will add support
     for this?
     """
 
-    def instruction_lr_w(self, ins: 'Instruction'):
+    def instruction_lr_w(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_sc_w(self, ins: 'Instruction'):
+    def instruction_sc_w(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_amoswap_w(self, ins: 'Instruction'):
+    def instruction_amoswap_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
-        if dest == 'zero':
+        if dest == "zero":
             self.mmu.write(addr, val.to_bytes())
         else:
             old = Int32(self.mmu.read(addr, 4))
             self.mmu.write(addr, val.to_bytes())
             self.regs.set(dest, old)
 
-    def instruction_amoadd_w(self, ins: 'Instruction'):
+    def instruction_amoadd_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
         old = Int32(self.mmu.read(addr, 4))
         self.mmu.write(addr, (old + val).to_bytes(4))
         self.regs.set(dest, old)
 
-    def instruction_amoand_w(self, ins: 'Instruction'):
+    def instruction_amoand_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
         old = Int32(self.mmu.read(addr, 4))
         self.mmu.write(addr, (old & val).to_bytes(4))
         self.regs.set(dest, old)
 
-    def instruction_amoor_w(self, ins: 'Instruction'):
+    def instruction_amoor_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
         old = Int32(self.mmu.read(addr, 4))
         self.mmu.write(addr, (old | val).to_bytes(4))
         self.regs.set(dest, old)
 
-    def instruction_amoxor_w(self, ins: 'Instruction'):
+    def instruction_amoxor_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
         old = Int32(self.mmu.read(addr, 4))
         self.mmu.write(addr, (old ^ val).to_bytes(4))
         self.regs.set(dest, old)
 
-    def instruction_amomax_w(self, ins: 'Instruction'):
+    def instruction_amomax_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
         old = Int32(self.mmu.read(addr, 4))
         self.mmu.write(addr, max(old, val).to_bytes(4))
         self.regs.set(dest, old)
 
-    def instruction_amomaxu_w(self, ins: 'Instruction'):
+    def instruction_amomaxu_w(self, ins: "Instruction"):
         val: UInt32
         dest, addr, val = self.parse_rd_rs_rs(ins, signed=False)
         old = UInt32(self.mmu.read(addr, 4))
 
         self.mmu.write(addr, max(old, val).to_bytes())
         self.regs.set(dest, old)
 
-    def instruction_amomin_w(self, ins: 'Instruction'):
+    def instruction_amomin_w(self, ins: "Instruction"):
         dest, addr, val = self.parse_rd_rs_rs(ins)
         old = Int32(self.mmu.read(addr, 4))
         self.mmu.write(addr, min(old, val).to_bytes(4))
         self.regs.set(dest, old)
 
-    def instruction_amominu_w(self, ins: 'Instruction'):
+    def instruction_amominu_w(self, ins: "Instruction"):
         val: UInt32
         dest, addr, val = self.parse_rd_rs_rs(ins, signed=False)
         old = UInt32(self.mmu.read(addr, 4))
 
         self.mmu.write(addr, min(old, val).to_bytes(4))
         self.regs.set(dest, old)
```

### Comparing `riscemu-2.0.5/riscemu/instructions/RV32I.py` & `riscemu-2.1.0/riscemu/instructions/RV32I.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,306 +18,254 @@
     The RV32I instruction set. Some instructions are missing, such as
     fence, fence.i, rdcycle, rdcycleh, rdtime, rdtimeh, rdinstret, rdinstreth
     All atomic read/writes are also not implemented yet
 
     See https://maxvytech.com/images/RV32I-11-2018.pdf for a more detailed overview
     """
 
-    def instruction_lb(self, ins: 'Instruction'):
+    def instruction_lb(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.regs.set(rd, Int32.sign_extend(self.mmu.read(addr.unsigned_value, 1), 8))
 
-    def instruction_lh(self, ins: 'Instruction'):
+    def instruction_lh(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.regs.set(rd, Int32.sign_extend(self.mmu.read(addr.unsigned_value, 2), 16))
 
-    def instruction_lw(self, ins: 'Instruction'):
+    def instruction_lw(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.regs.set(rd, Int32(self.mmu.read(addr.unsigned_value, 4)))
 
-    def instruction_lbu(self, ins: 'Instruction'):
+    def instruction_lbu(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.regs.set(rd, Int32(self.mmu.read(addr.unsigned_value, 1)))
 
-    def instruction_lhu(self, ins: 'Instruction'):
+    def instruction_lhu(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.regs.set(rd, Int32(self.mmu.read(addr.unsigned_value, 2)))
 
-    def instruction_sb(self, ins: 'Instruction'):
+    def instruction_sb(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.mmu.write(addr.unsigned_value, 1, self.regs.get(rd).to_bytes(1))
 
-    def instruction_sh(self, ins: 'Instruction'):
+    def instruction_sh(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.mmu.write(addr.unsigned_value, 2, self.regs.get(rd).to_bytes(2))
 
-    def instruction_sw(self, ins: 'Instruction'):
+    def instruction_sw(self, ins: "Instruction"):
         rd, addr = self.parse_mem_ins(ins)
         self.mmu.write(addr.unsigned_value, 4, self.regs.get(rd).to_bytes(4))
 
-    def instruction_sll(self, ins: 'Instruction'):
+    def instruction_sll(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         dst = ins.get_reg(0)
         src1 = ins.get_reg(1)
         src2 = ins.get_reg(2)
-        self.regs.set(
-            dst,
-            self.regs.get(src1) << (self.regs.get(src2) & 0b11111)
-        )
+        self.regs.set(dst, self.regs.get(src1) << (self.regs.get(src2) & 0b11111))
 
-    def instruction_slli(self, ins: 'Instruction'):
+    def instruction_slli(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         dst = ins.get_reg(0)
         src1 = ins.get_reg(1)
         imm = ins.get_imm(2)
-        self.regs.set(
-            dst,
-            self.regs.get(src1) << (imm & 0b11111)
-        )
+        self.regs.set(dst, self.regs.get(src1) << (imm & 0b11111))
 
-    def instruction_srl(self, ins: 'Instruction'):
+    def instruction_srl(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         dst = ins.get_reg(0)
         src1 = ins.get_reg(1)
         src2 = ins.get_reg(2)
         self.regs.set(
-            dst,
-            self.regs.get(src1).shift_right_logical(self.regs.get(src2) & 0b11111)
+            dst, self.regs.get(src1).shift_right_logical(self.regs.get(src2) & 0b11111)
         )
 
-    def instruction_srli(self, ins: 'Instruction'):
+    def instruction_srli(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         dst = ins.get_reg(0)
         src1 = ins.get_reg(1)
         imm = ins.get_imm(2)
-        self.regs.set(
-            dst,
-            self.regs.get(src1).shift_right_logical(imm & 0b11111)
-        )
+        self.regs.set(dst, self.regs.get(src1).shift_right_logical(imm & 0b11111))
 
-    def instruction_sra(self, ins: 'Instruction'):
+    def instruction_sra(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         dst = ins.get_reg(0)
         src1 = ins.get_reg(1)
         src2 = ins.get_reg(2)
-        self.regs.set(
-            dst,
-            self.regs.get(src1) >> (self.regs.get(src2) & 0b11111)
-        )
+        self.regs.set(dst, self.regs.get(src1) >> (self.regs.get(src2) & 0b11111))
 
-    def instruction_srai(self, ins: 'Instruction'):
+    def instruction_srai(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         dst = ins.get_reg(0)
         src1 = ins.get_reg(1)
         imm = ins.get_imm(2)
-        self.regs.set(
-            dst,
-            self.regs.get(src1) >> (imm & 0b11111)
-        )
+        self.regs.set(dst, self.regs.get(src1) >> (imm & 0b11111))
 
-    def instruction_add(self, ins: 'Instruction'):
+    def instruction_add(self, ins: "Instruction"):
         # FIXME: once configuration is figured out, add flag to support immediate arg in add instruction
         dst, rs1, rs2 = self.parse_rd_rs_rs(ins)
 
-        self.regs.set(
-            dst,
-            rs1 + rs2
-        )
+        self.regs.set(dst, rs1 + rs2)
 
-    def instruction_addi(self, ins: 'Instruction'):
+    def instruction_addi(self, ins: "Instruction"):
         dst, rs1, imm = self.parse_rd_rs_imm(ins)
-        self.regs.set(
-            dst,
-            rs1 + imm
-        )
+        self.regs.set(dst, rs1 + imm)
 
-    def instruction_sub(self, ins: 'Instruction'):
+    def instruction_sub(self, ins: "Instruction"):
         dst, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            dst,
-            rs1 - rs2
-        )
+        self.regs.set(dst, rs1 - rs2)
 
-    def instruction_lui(self, ins: 'Instruction'):
+    def instruction_lui(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         reg = ins.get_reg(0)
         imm = UInt32(ins.get_imm(1) << 12)
         self.regs.set(reg, Int32(imm))
 
-    def instruction_auipc(self, ins: 'Instruction'):
+    def instruction_auipc(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         reg = ins.get_reg(0)
         imm = UInt32(ins.get_imm(1) << 12)
         self.regs.set(reg, imm.signed() + self.pc)
 
-    def instruction_xor(self, ins: 'Instruction'):
+    def instruction_xor(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            rs1 ^ rs2
-        )
+        self.regs.set(rd, rs1 ^ rs2)
 
-    def instruction_xori(self, ins: 'Instruction'):
+    def instruction_xori(self, ins: "Instruction"):
         rd, rs1, imm = self.parse_rd_rs_imm(ins)
-        self.regs.set(
-            rd,
-            rs1 ^ imm
-        )
+        self.regs.set(rd, rs1 ^ imm)
 
-    def instruction_or(self, ins: 'Instruction'):
+    def instruction_or(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            rs1 | rs2
-        )
+        self.regs.set(rd, rs1 | rs2)
 
-    def instruction_ori(self, ins: 'Instruction'):
+    def instruction_ori(self, ins: "Instruction"):
         rd, rs1, imm = self.parse_rd_rs_imm(ins)
-        self.regs.set(
-            rd,
-            rs1 | imm
-        )
+        self.regs.set(rd, rs1 | imm)
 
-    def instruction_and(self, ins: 'Instruction'):
+    def instruction_and(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            rs1 & rs2
-        )
+        self.regs.set(rd, rs1 & rs2)
 
-    def instruction_andi(self, ins: 'Instruction'):
+    def instruction_andi(self, ins: "Instruction"):
         rd, rs1, imm = self.parse_rd_rs_imm(ins)
-        self.regs.set(
-            rd,
-            rs1 & imm
-        )
+        self.regs.set(rd, rs1 & imm)
 
-    def instruction_slt(self, ins: 'Instruction'):
+    def instruction_slt(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            Int32(int(rs1 < rs2))
-        )
+        self.regs.set(rd, Int32(int(rs1 < rs2)))
 
-    def instruction_slti(self, ins: 'Instruction'):
+    def instruction_slti(self, ins: "Instruction"):
         rd, rs1, imm = self.parse_rd_rs_imm(ins)
-        self.regs.set(
-            rd,
-            Int32(int(rs1 < imm))
-        )
+        self.regs.set(rd, Int32(int(rs1 < imm)))
 
-    def instruction_sltu(self, ins: 'Instruction'):
+    def instruction_sltu(self, ins: "Instruction"):
         dst, rs1, rs2 = self.parse_rd_rs_rs(ins, signed=False)
-        self.regs.set(
-            dst,
-            Int32(int(rs1 < rs2))
-        )
+        self.regs.set(dst, Int32(int(rs1 < rs2)))
 
-    def instruction_sltiu(self, ins: 'Instruction'):
+    def instruction_sltiu(self, ins: "Instruction"):
         dst, rs1, imm = self.parse_rd_rs_imm(ins, signed=False)
-        self.regs.set(
-            dst,
-            Int32(int(rs1 < imm))
-        )
+        self.regs.set(dst, Int32(int(rs1 < imm)))
 
-    def instruction_beq(self, ins: 'Instruction'):
+    def instruction_beq(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 == rs2:
             self.pc = dst.unsigned_value
 
-    def instruction_bne(self, ins: 'Instruction'):
+    def instruction_bne(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 != rs2:
             self.pc = dst.unsigned_value
 
-    def instruction_blt(self, ins: 'Instruction'):
+    def instruction_blt(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 < rs2:
             self.pc = dst.unsigned_value
 
-    def instruction_bge(self, ins: 'Instruction'):
+    def instruction_bge(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 >= rs2:
             self.pc = dst.unsigned_value
 
-    def instruction_bltu(self, ins: 'Instruction'):
+    def instruction_bltu(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins, signed=False)
         if rs1 < rs2:
             self.pc = dst.unsigned_value
 
-    def instruction_bgeu(self, ins: 'Instruction'):
+    def instruction_bgeu(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins, signed=False)
         if rs1 >= rs2:
             self.pc = dst.unsigned_value
 
     # technically deprecated
-    def instruction_j(self, ins: 'Instruction'):
+    def instruction_j(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 1)
         addr = ins.get_imm(0)
         self.pc = addr
 
-    def instruction_jal(self, ins: 'Instruction'):
-        reg = 'ra'  # default register is ra
+    def instruction_jal(self, ins: "Instruction"):
+        reg = "ra"  # default register is ra
         if len(ins.args) == 1:
             addr = ins.get_imm(0)
         else:
             ASSERT_LEN(ins.args, 2)
             reg = ins.get_reg(0)
             addr = ins.get_imm(1)
         self.regs.set(reg, Int32(self.pc))
         self.pc = addr
 
-    def instruction_jalr(self, ins: 'Instruction'):
+    def instruction_jalr(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         reg = ins.get_reg(0)
-        addr = ins.get_imm(1)
+        base = ins.get_reg(1)
+        addr = ins.get_imm(2)
         self.regs.set(reg, Int32(self.pc))
-        self.pc = addr
+        self.pc = self.regs.get(base).unsigned_value + addr
 
-    def instruction_ret(self, ins: 'Instruction'):
+    def instruction_ret(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 0)
-        self.pc = self.regs.get('ra').value
+        self.pc = self.regs.get("ra").value
 
-    def instruction_ecall(self, ins: 'Instruction'):
+    def instruction_ecall(self, ins: "Instruction"):
         self.instruction_scall(ins)
 
-    def instruction_ebreak(self, ins: 'Instruction'):
+    def instruction_ebreak(self, ins: "Instruction"):
         self.instruction_sbreak(ins)
 
-    def instruction_scall(self, ins: 'Instruction'):
+    def instruction_scall(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 0)
 
         if not isinstance(self.cpu, UserModeCPU):
             # FIXME: add exception for syscall not supported or something
             raise
 
-        syscall = Syscall(self.regs.get('a7'), self.cpu)
+        syscall = Syscall(self.regs.get("a7"), self.cpu)
         self.cpu.syscall_int.handle_syscall(syscall)
 
-    def instruction_sbreak(self, ins: 'Instruction'):
+    def instruction_sbreak(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 0)
         if self.cpu.conf.debug_instruction:
-            print(FMT_DEBUG + "Debug instruction encountered at 0x{:08X}".format(self.pc - 1) + FMT_NONE)
+            print(
+                FMT_DEBUG
+                + "Debug instruction encountered at 0x{:08X}".format(self.pc - 1)
+                + FMT_NONE
+            )
             raise LaunchDebuggerException()
 
-    def instruction_nop(self, ins: 'Instruction'):
+    def instruction_nop(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 0)
         pass
 
-    def instruction_li(self, ins: 'Instruction'):
+    def instruction_li(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         reg = ins.get_reg(0)
         immediate = ins.get_imm(1)
         self.regs.set(reg, Int32(immediate))
 
-    def instruction_la(self, ins: 'Instruction'):
+    def instruction_la(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         reg = ins.get_reg(0)
         immediate = ins.get_imm(1)
         self.regs.set(reg, Int32(immediate))
 
-    def instruction_mv(self, ins: 'Instruction'):
+    def instruction_mv(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         rd, rs = ins.get_reg(0), ins.get_reg(1)
         self.regs.set(rd, self.regs.get(rs))
-
-
```

### Comparing `riscemu-2.0.5/riscemu/instructions/RV32M.py` & `riscemu-2.1.0/riscemu/instructions/RV32M.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,54 +8,37 @@
 from riscemu.types.exceptions import INS_NOT_IMPLEMENTED
 
 
 class RV32M(InstructionSet):
     """
     The RV32M Instruction set, containing multiplication and division instructions
     """
-    def instruction_mul(self, ins: 'Instruction'):
+
+    def instruction_mul(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            rs1 * rs2
-        )
+        self.regs.set(rd, rs1 * rs2)
 
-    def instruction_mulh(self, ins: 'Instruction'):
+    def instruction_mulh(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            (rs1 * rs2) >> 32
-        )
+        self.regs.set(rd, (rs1 * rs2) >> 32)
 
-    def instruction_mulhsu(self, ins: 'Instruction'):
+    def instruction_mulhsu(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_mulhu(self, ins: 'Instruction'):
+    def instruction_mulhu(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_div(self, ins: 'Instruction'):
+    def instruction_div(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            rs1 // rs2
-        )
+        self.regs.set(rd, rs1 // rs2)
 
-    def instruction_divu(self, ins: 'Instruction'):
+    def instruction_divu(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins, signed=False)
-        self.regs.set(
-            rd,
-            rs1 // rs2
-        )
+        self.regs.set(rd, rs1 // rs2)
 
-    def instruction_rem(self, ins: 'Instruction'):
+    def instruction_rem(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(
-            rd,
-            rs1 % rs2
-        )
+        self.regs.set(rd, rs1 % rs2)
 
-    def instruction_remu(self, ins: 'Instruction'):
+    def instruction_remu(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins, signed=False)
-        self.regs.set(
-            rd,
-            rs1 % rs2
-        )
+        self.regs.set(rd, rs1 % rs2)
```

### Comparing `riscemu-2.0.5/riscemu/instructions/instruction_set.py` & `riscemu-2.1.0/riscemu/instructions/instruction_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,43 +19,41 @@
     Each instruction set has to inherit from this class. Each instruction should be it's own method:
 
     instruction_<name>(self, ins: LoadedInstruction)
 
     instructions containing a dot '.' should replace it with an underscore.
     """
 
-    def __init__(self, cpu: 'CPU'):
+    def __init__(self, cpu: "CPU"):
         """Create a new instance of the Instruction set. This requires access to a CPU, and grabs vertain things
         from it such as access to the MMU and registers.
         """
         self.name = self.__class__.__name__
         self.cpu = cpu
 
-    def load(self) -> Dict[str, Callable[['Instruction'], None]]:
+    def load(self) -> Dict[str, Callable[["Instruction"], None]]:
         """
         This is called by the CPU once it instantiates this instruction set
 
         It returns a dictionary of all instructions in this instruction set,
         pointing to the correct handler for it
         """
-        return {
-            name: ins for name, ins in self.get_instructions()
-        }
+        return {name: ins for name, ins in self.get_instructions()}
 
     def get_instructions(self):
         """
         Returns a list of all valid instruction names included in this instruction set
 
         converts underscores in names to dots
         """
         for member in dir(self):
-            if member.startswith('instruction_'):
-                yield member[12:].replace('_', '.'), getattr(self, member)
+            if member.startswith("instruction_"):
+                yield member[12:].replace("_", "."), getattr(self, member)
 
-    def parse_mem_ins(self, ins: 'Instruction') -> Tuple[str, Int32]:
+    def parse_mem_ins(self, ins: "Instruction") -> Tuple[str, Int32]:
         """
         parses both rd, rs, imm and rd, imm(rs) argument format and returns (rd, imm+rs1)
         (so a register and address tuple for memory instructions)
         """
         if len(ins.args) == 3:
             # handle rd, rs1, imm
             rs = self.get_reg_content(ins, 1)
@@ -65,59 +63,77 @@
             ASSERT_LEN(ins.args, 2)
             ASSERT_IN("(", ins.args[1])
             imm, rs_name = ins.get_imm_reg(1)
             rs = self.regs.get(rs_name)
         rd = ins.get_reg(0)
         return rd, rs + imm
 
-    def parse_rd_rs_rs(self, ins: 'Instruction', signed=True) -> Tuple[str, Int32, Int32]:
+    def parse_rd_rs_rs(
+        self, ins: "Instruction", signed=True
+    ) -> Tuple[str, Int32, Int32]:
         """
         Assumes the command is in <name> rd, rs1, rs2 format
         Returns the name of rd, and the values in rs1 and rs2
         """
         ASSERT_LEN(ins.args, 3)
         if signed:
-            return ins.get_reg(0), \
-                   Int32(self.get_reg_content(ins, 1)), \
-                   Int32(self.get_reg_content(ins, 2))
+            return (
+                ins.get_reg(0),
+                Int32(self.get_reg_content(ins, 1)),
+                Int32(self.get_reg_content(ins, 2)),
+            )
         else:
-            return ins.get_reg(0), \
-                   UInt32(self.get_reg_content(ins, 1)), \
-                   UInt32(self.get_reg_content(ins, 2))
-
-    def parse_rd_rs_imm(self, ins: 'Instruction', signed=True) -> Tuple[str, Int32, Int32]:
+            return (
+                ins.get_reg(0),
+                UInt32(self.get_reg_content(ins, 1)),
+                UInt32(self.get_reg_content(ins, 2)),
+            )
+
+    def parse_rd_rs_imm(
+        self, ins: "Instruction", signed=True
+    ) -> Tuple[str, Int32, Int32]:
         """
         Assumes the command is in <name> rd, rs, imm format
         Returns the name of rd, the value in rs and the immediate imm
         """
         ASSERT_LEN(ins.args, 3)
         if signed:
-            return ins.get_reg(0), \
-                   Int32(self.get_reg_content(ins, 1)), \
-                   Int32(ins.get_imm(2))
+            return (
+                ins.get_reg(0),
+                Int32(self.get_reg_content(ins, 1)),
+                Int32(ins.get_imm(2)),
+            )
         else:
-            return ins.get_reg(0), \
-                   UInt32(self.get_reg_content(ins, 1)), \
-                   UInt32(ins.get_imm(2))
-
-    def parse_rs_rs_imm(self, ins: 'Instruction', signed=True) -> Tuple[Int32, Int32, Int32]:
+            return (
+                ins.get_reg(0),
+                UInt32(self.get_reg_content(ins, 1)),
+                UInt32(ins.get_imm(2)),
+            )
+
+    def parse_rs_rs_imm(
+        self, ins: "Instruction", signed=True
+    ) -> Tuple[Int32, Int32, Int32]:
         """
         Assumes the command is in <name> rs1, rs2, imm format
         Returns the values in rs1, rs2 and the immediate imm
         """
         if signed:
-            return Int32(self.get_reg_content(ins, 0)), \
-                   Int32(self.get_reg_content(ins, 1)), \
-                   Int32(ins.get_imm(2))
+            return (
+                Int32(self.get_reg_content(ins, 0)),
+                Int32(self.get_reg_content(ins, 1)),
+                Int32(ins.get_imm(2)),
+            )
         else:
-            return UInt32(self.get_reg_content(ins, 0)), \
-                   UInt32(self.get_reg_content(ins, 1)), \
-                   UInt32(ins.get_imm(2))
+            return (
+                UInt32(self.get_reg_content(ins, 0)),
+                UInt32(self.get_reg_content(ins, 1)),
+                UInt32(ins.get_imm(2)),
+            )
 
-    def get_reg_content(self, ins: 'Instruction', ind: int) -> Int32:
+    def get_reg_content(self, ins: "Instruction", ind: int) -> Int32:
         """
         get the register name from ins and then return the register contents
         """
         return self.regs.get(ins.get_reg(ind))
 
     @property
     def pc(self):
@@ -136,10 +152,9 @@
 
     @property
     def regs(self):
         return self.cpu.regs
 
     def __repr__(self):
         return "InstructionSet[{}] with {} instructions".format(
-            self.__class__.__name__,
-            len(list(self.get_instructions()))
+            self.__class__.__name__, len(list(self.get_instructions()))
         )
```

### Comparing `riscemu-2.0.5/riscemu/interactive.py` & `riscemu-2.1.0/riscemu/interactive.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import sys
 
 from riscemu import RunConfig
 from riscemu.types import InstructionMemorySection, SimpleInstruction, Program
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from .CPU import UserModeCPU
     from .instructions import InstructionSetDict
     from .debug import launch_debug_session
 
     cpu = UserModeCPU(list(InstructionSetDict.values()), RunConfig(verbosity=4))
 
-    program = Program('interactive session', base=0x100)
+    program = Program("interactive session", base=0x100)
     context = program.context
-    program.add_section(InstructionMemorySection([
-        SimpleInstruction('ebreak', (), context, 0x100),
-        SimpleInstruction('addi', ('a0', 'zero', '0'), context, 0x104),
-        SimpleInstruction('addi', ('a7', 'zero', '93'), context, 0x108),
-        SimpleInstruction('scall', (), context, 0x10C),
-    ], '.text', context, program.name, 0x100))
+    program.add_section(
+        InstructionMemorySection(
+            [
+                SimpleInstruction("ebreak", (), context, 0x100),
+                SimpleInstruction("addi", ("a0", "zero", "0"), context, 0x104),
+                SimpleInstruction("addi", ("a7", "zero", "93"), context, 0x108),
+                SimpleInstruction("scall", (), context, 0x10C),
+            ],
+            ".text",
+            context,
+            program.name,
+            0x100,
+        )
+    )
 
     cpu.load_program(program)
 
     cpu.setup_stack()
 
-    cpu.launch(program)
+    cpu.launch()
 
     sys.exit(cpu.exit_code)
```

### Comparing `riscemu-2.0.5/riscemu/parser.py` & `riscemu-2.1.0/riscemu/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 from .tokenizer import Token, TokenType, tokenize
 from .types import Program, T_ParserOpts, ProgramLoader, SimpleInstruction
 from .types.exceptions import ParseException
 
 
 def parse_instruction(token: Token, args: Tuple[str], context: ParseContext):
     if context.section is None:
-        context.new_section('.text', MemorySectionType.Instructions)
+        context.new_section(".text", MemorySectionType.Instructions)
     if context.section.type != MemorySectionType.Instructions:
-        raise ParseException("{} {} encountered in invalid context: {}".format(token, args, context))
-    ins = SimpleInstruction(token.value, args, context.context, context.current_address())
+        raise ParseException(
+            "{} {} encountered in invalid context: {}".format(token, args, context)
+        )
+    ins = SimpleInstruction(
+        token.value, args, context.context, context.current_address()
+    )
     context.section.data.append(ins)
 
 
 def parse_label(token: Token, args: Tuple[str], context: ParseContext):
     name = token.value[:-1]
-    if re.match(r'^\d+$', name):
+    if re.match(r"^\d+$", name):
         # relative label:
         context.context.numbered_labels[name].append(context.current_address())
     else:
         if name in context.context.labels:
-            print(FMT_PARSE + 'Warn: Symbol {} defined twice!'.format(name))
+            print(FMT_PARSE + "Warn: Symbol {} defined twice!".format(name))
         context.add_label(name, context.current_address(), is_relative=True)
 
 
 PARSERS: Dict[TokenType, Callable[[Token, Tuple[str], ParseContext], None]] = {
     TokenType.PSEUDO_OP: AssemblerDirectives.handle_instruction,
     TokenType.LABEL: parse_label,
-    TokenType.INSTRUCTION_NAME: parse_instruction
+    TokenType.INSTRUCTION_NAME: parse_instruction,
 }
 
 
 def parse_tokens(name: str, tokens_iter: Iterable[Token]) -> Program:
     """
     Convert a token stream into a parsed program
     :param name: the programs name
@@ -54,28 +58,34 @@
         if token.type not in PARSERS:
             raise ParseException("Unexpected token type: {}, {}".format(token, args))
         PARSERS[token.type](token, args, context)
 
     return context.finalize()
 
 
-def composite_tokenizer(tokens_iter: Iterable[Token]) -> Iterable[Tuple[Token, Tuple[str]]]:
+def composite_tokenizer(
+    tokens_iter: Iterable[Token],
+) -> Iterable[Tuple[Token, Tuple[str]]]:
     """
     Convert an iterator over tokens into an iterator over tuples: (token, list(token))
 
     The first token ist either a pseudo_op, label, or instruction name. The token list are all remaining tokens before
     a newline is encountered
     :param tokens_iter: An iterator over tokens
     :return: An iterator over a slightly more structured representation of the tokens
     """
     tokens: Peekable[Token] = Peekable[Token](tokens_iter)
 
     while not tokens.is_empty():
         token = next(tokens)
-        if token.type in (TokenType.PSEUDO_OP, TokenType.LABEL, TokenType.INSTRUCTION_NAME):
+        if token.type in (
+            TokenType.PSEUDO_OP,
+            TokenType.LABEL,
+            TokenType.INSTRUCTION_NAME,
+        ):
             yield token, tuple(take_arguments(tokens))
 
 
 def take_arguments(tokens: Peekable[Token]) -> Iterable[str]:
     """
     Consumes (argument comma)* and yields argument.value until newline is reached
     If an argument is not followed by either a newline or a comma, a parse exception is raised
@@ -102,31 +112,32 @@
     pseudo instructions. It does very little verification of source correctness.
 
     It also supports numbered jump targets and properly supports local and global scope (.globl assembly directive)
 
 
     The AssemblyFileLoader loads .asm, .S and .s files by default, and acts as a weak fallback to all other filetypes.
     """
+
     def parse(self) -> Program:
-        with open(self.source_path, 'r') as f:
+        with open(self.source_path, "r") as f:
             return parse_tokens(self.filename, tokenize(f))
 
-    def parse_io(self, io):
+    def parse_io(self, io: Iterable[str]):
         return parse_tokens(self.filename, tokenize(io))
 
     @classmethod
     def can_parse(cls, source_path: str) -> float:
         """
 
         It also acts as a weak fallback if no other loaders want to take the file.
 
         :param source_path: the path to the source file
         :return:
         """
         # gcc recognizes these line endings as assembly. So we will do too.
-        if source_path.split('.')[-1] in ('asm', 'S', 's'):
+        if source_path.split(".")[-1] in ("asm", "S", "s"):
             return 1
         return 0.01
 
     @classmethod
-    def get_options(cls, argv: List[str]) -> [List[str], T_ParserOpts]:
+    def get_options(cls, argv: List[str]) -> Tuple[List[str], T_ParserOpts]:
         return argv, {}
```

### Comparing `riscemu-2.0.5/riscemu/priv/CSR.py` & `riscemu-2.1.0/riscemu/priv/CSR.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..types import UInt32
 
 
 class CSR:
     """
     This holds all Control and Status Registers (CSR)
     """
+
     regs: Dict[int, UInt32]
     """
     All Control and Status Registers are stored here
     """
 
     virtual_regs: Dict[int, Callable[[], UInt32]]
     """
@@ -48,15 +49,17 @@
         addr = self._name_to_addr(addr)
         if addr is None:
             raise RuntimeError(f"Invalid CSR name: {addr}!")
         if addr in self.virtual_regs:
             return self.virtual_regs[addr]()
         return self.regs[addr]
 
-    def set_listener(self, addr: Union[str, int], listener: Callable[[UInt32, UInt32], None]):
+    def set_listener(
+        self, addr: Union[str, int], listener: Callable[[UInt32, UInt32], None]
+    ):
         addr = self._name_to_addr(addr)
         if addr is None:
             print("unknown csr address name: {}".format(addr))
             return
         self.listeners[addr] = listener
 
     # mstatus properties
@@ -69,28 +72,28 @@
 
         :param name:
         :param val:
         :return:
         """
         size = 2 if name in MSTATUS_LEN_2 else 1
         off = MSTATUS_OFFSETS[name]
-        mask = (2 ** size - 1) << off
-        old_val = self.get('mstatus')
+        mask = (2**size - 1) << off
+        old_val = self.get("mstatus")
         erased = old_val & (~mask)
         new_val = erased | (val << off)
-        self.set('mstatus', new_val)
+        self.set("mstatus", new_val)
 
     def get_mstatus(self, name) -> UInt32:
         if not self.mstatus_cache_dirty and name in self.mstatus_cache:
             return self.mstatus_cache[name]
 
         size = 2 if name in MSTATUS_LEN_2 else 1
         off = MSTATUS_OFFSETS[name]
-        mask = (2 ** size - 1) << off
-        val = (self.get('mstatus') & mask) >> off
+        mask = (2**size - 1) << off
+        val = (self.get("mstatus") & mask) >> off
         if self.mstatus_cache_dirty:
             self.mstatus_cache = dict(name=val)
         else:
             self.mstatus_cache[name] = val
         return val
 
     def callback(self, addr: Union[str, int]):
```

### Comparing `riscemu-2.0.5/riscemu/priv/ElfLoader.py` & `riscemu-2.1.0/riscemu/priv/ElfLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,99 +7,122 @@
 
 FMT_ELF = FMT_GREEN + FMT_BOLD
 
 if typing.TYPE_CHECKING:
     from elftools.elf.elffile import ELFFile
     from elftools.elf.sections import Section, SymbolTableSection
 
-INCLUDE_SEC = ('.text', '.stack', '.bss', '.sdata', '.sbss')
+INCLUDE_SEC = (".text", ".stack", ".bss", ".sdata", ".sbss")
 
 
 class ElfBinaryFileLoader(ProgramLoader):
     """
     Loads compiled elf binaries (checks for the magic sequence 7f45 4c46)
 
     This loader respects local and global symbols.
     """
+
     program: Program
 
     def __init__(self, source_path: str, options: T_ParserOpts):
         super().__init__(source_path, options)
         self.program = Program(self.filename)
 
     @classmethod
     def can_parse(cls, source_path: str) -> float:
-        with open(source_path, 'rb') as f:
-            if f.read(4) == b'\x7f\x45\x4c\x46':
+        with open(source_path, "rb") as f:
+            if f.read(4) == b"\x7f\x45\x4c\x46":
                 return 1
         return 0
 
     @classmethod
     def get_options(cls, argv: List[str]) -> [List[str], T_ParserOpts]:
         return argv, {}
 
     def parse(self) -> Program:
         try:
             from elftools.elf.elffile import ELFFile
             from elftools.elf.sections import Section, SymbolTableSection
 
-            with open(self.source_path, 'rb') as f:
-                print(FMT_ELF + "[ElfLoader] Loading elf executable from: {}".format(self.source_path) + FMT_NONE)
+            with open(self.source_path, "rb") as f:
+                print(
+                    FMT_ELF
+                    + "[ElfLoader] Loading elf executable from: {}".format(
+                        self.source_path
+                    )
+                    + FMT_NONE
+                )
                 self._read_elf(ELFFile(f))
         except ImportError as e:
-            print(FMT_PARSE + "[ElfLoader] Cannot load elf files without PyElfTools package! You can install them "
-                              "using pip install pyelftools!" + FMT_NONE)
+            print(
+                FMT_PARSE
+                + "[ElfLoader] Cannot load elf files without PyElfTools package! You can install them "
+                "using pip install pyelftools!" + FMT_NONE
+            )
             raise e
 
         return self.program
 
-    def _read_elf(self, elf: 'ELFFile'):
-        if not elf.header.e_machine == 'EM_RISCV':
+    def _read_elf(self, elf: "ELFFile"):
+        if not elf.header.e_machine == "EM_RISCV":
             raise InvalidElfException("Not a RISC-V elf file!")
-        if not elf.header.e_ident.EI_CLASS == 'ELFCLASS32':
+        if not elf.header.e_ident.EI_CLASS == "ELFCLASS32":
             raise InvalidElfException("Only 32bit executables are supported!")
 
         from elftools.elf.sections import SymbolTableSection
+
         for sec in elf.iter_sections():
             if isinstance(sec, SymbolTableSection):
                 self._parse_symtab(sec)
                 continue
 
             if sec.name not in INCLUDE_SEC:
                 continue
 
             self._add_sec(self._lms_from_elf_sec(sec, self.filename))
 
-    def _lms_from_elf_sec(self, sec: 'Section', owner: str):
-        is_code = sec.name in ('.text',)
+    def _lms_from_elf_sec(self, sec: "Section", owner: str):
+        is_code = sec.name in (".text",)
         data = bytearray(sec.data())
         if len(data) < sec.data_size:
             data += bytearray(len(data) - sec.data_size)
         flags = MemoryFlags(is_code, is_code)
-        print(FMT_ELF + "[ElfLoader] Section {} at: {:X}".format(sec.name, sec.header.sh_addr) + FMT_NONE)
+        print(
+            FMT_ELF
+            + "[ElfLoader] Section {} at: {:X}".format(sec.name, sec.header.sh_addr)
+            + FMT_NONE
+        )
         return ElfMemorySection(
             data, sec.name, self.program.context, owner, sec.header.sh_addr, flags
         )
 
-    def _parse_symtab(self, symtab: 'SymbolTableSection'):
+    def _parse_symtab(self, symtab: "SymbolTableSection"):
         from elftools.elf.enums import ENUM_ST_VISIBILITY
 
         for sym in symtab.iter_symbols():
             if not sym.name:
                 continue
             self.program.context.labels[sym.name] = sym.entry.st_value
             # check if it has st_visibility bit set
-            if sym.entry.st_info.bind == 'STB_GLOBAL':
+            if sym.entry.st_info.bind == "STB_GLOBAL":
                 self.program.global_labels.add(sym.name)
-                print(FMT_PARSE + "LOADED GLOBAL SYMBOL {}: {}".format(sym.name, sym.entry.st_value) + FMT_NONE)
+                print(
+                    FMT_PARSE
+                    + "LOADED GLOBAL SYMBOL {}: {}".format(sym.name, sym.entry.st_value)
+                    + FMT_NONE
+                )
 
-    def _add_sec(self, new_sec: 'ElfMemorySection'):
+    def _add_sec(self, new_sec: "ElfMemorySection"):
         for sec in self.program.sections:
             if sec.base < sec.end <= new_sec.base or sec.end > sec.base >= new_sec.end:
                 continue
             else:
-                print(FMT_ELF + "[ElfLoader] Invalid elf layout: Two sections overlap: \n\t{}\n\t{}".format(
-                    sec, new_sec
-                ) + FMT_NONE)
+                print(
+                    FMT_ELF
+                    + "[ElfLoader] Invalid elf layout: Two sections overlap: \n\t{}\n\t{}".format(
+                        sec, new_sec
+                    )
+                    + FMT_NONE
+                )
                 raise RuntimeError("Cannot load elf with overlapping sections!")
 
         self.program.add_section(new_sec)
```

### Comparing `riscemu-2.0.5/riscemu/priv/Exceptions.py` & `riscemu-2.1.0/riscemu/priv/Exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,18 +38,20 @@
     type: CpuTrapType
     """
     The type (timer, external, software) of the trap
     """
 
     priv: PrivModes
     """
-    The privilege level this trap targets 
+    The privilege level this trap targets
     """
 
-    def __init__(self, code: int, mtval, type: CpuTrapType, priv: PrivModes = PrivModes.MACHINE):
+    def __init__(
+        self, code: int, mtval, type: CpuTrapType, priv: PrivModes = PrivModes.MACHINE
+    ):
         self.interrupt = 0 if type == CpuTrapType.EXCEPTION else 1
         self.code = code
         self.mtval = UInt32(mtval)
         self.priv = priv
         self.type = type
 
     @property
@@ -59,26 +61,28 @@
     def message(self) -> str:
         return ""
 
     def __repr__(self):
         name = "Reserved interrupt({}, {})".format(self.interrupt, self.code)
 
         if (self.interrupt, self.code) in MCAUSE_TRANSLATION:
-            name = MCAUSE_TRANSLATION[(self.interrupt, self.code)] + "({}, {})".format(self.interrupt, self.code)
+            name = MCAUSE_TRANSLATION[(self.interrupt, self.code)] + "({}, {})".format(
+                self.interrupt, self.code
+            )
 
         return "{} {{priv={}, type={}, mtval={:x}}} {}".format(
             name, self.priv.name, self.type.name, self.mtval, self.message()
         )
 
     def __str__(self):
         return self.__repr__()
 
 
 class IllegalInstructionTrap(CpuTrap):
-    def __init__(self, ins: 'ElfInstruction'):
+    def __init__(self, ins: "ElfInstruction"):
         super().__init__(2, ins.encoded, CpuTrapType.EXCEPTION)
 
 
 class InstructionAddressMisalignedTrap(CpuTrap):
     def __init__(self, addr: int):
         super().__init__(0, addr, CpuTrapType.EXCEPTION)
 
@@ -100,25 +104,24 @@
 
 class InvalidElfException(RiscemuBaseException):
     def __init__(self, msg: str):
         super().__init__()
         self.msg = msg
 
     def message(self):
-        return FMT_PARSE + "{}(\"{}\")".format(self.__class__.__name__, self.msg) + FMT_NONE
+        return (
+            FMT_PARSE + '{}("{}")'.format(self.__class__.__name__, self.msg) + FMT_NONE
+        )
 
 
 class LoadAccessFault(CpuTrap):
     def __init__(self, msg, addr, size, op):
         super(LoadAccessFault, self).__init__(5, addr, CpuTrapType.EXCEPTION)
         self.msg = msg
         self.addr = addr
         self.size = size
         self.op = op
 
     def message(self):
         return "(During {} at 0x{:08x} of size {}: {})".format(
-            self.op,
-            self.addr,
-            self.size,
-            self.msg
+            self.op, self.addr, self.size, self.msg
         )
```

### Comparing `riscemu-2.0.5/riscemu/priv/ImageLoader.py` & `riscemu-2.1.0/riscemu/priv/ImageLoader.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,66 +10,77 @@
 from ..assembler import INSTRUCTION_SECTION_NAMES
 from ..colors import FMT_NONE, FMT_PARSE
 from ..helpers import get_section_base_name
 from ..types import MemoryFlags, ProgramLoader, Program, T_ParserOpts
 
 
 class MemoryImageLoader(ProgramLoader):
-
     @classmethod
     def can_parse(cls, source_path: str) -> float:
-        if source_path.split('.')[-1] == 'img':
+        if source_path.split(".")[-1] == "img":
             return 1
         return 0
 
     @classmethod
     def get_options(cls, argv: List[str]) -> [List[str], T_ParserOpts]:
         return argv, {}
 
     def parse(self) -> Iterable[Program]:
-        if 'debug' not in self.options:
+        if "debug" not in self.options:
             yield self.parse_no_debug()
             return
 
-        with open(self.options.get('debug'), 'r') as debug_file:
+        with open(self.options.get("debug"), "r") as debug_file:
             debug_info = MemoryImageDebugInfos.load(debug_file.read())
 
-        with open(self.source_path, 'rb') as source_file:
+        with open(self.source_path, "rb") as source_file:
             data: bytearray = bytearray(source_file.read())
 
         for name, sections in debug_info.sections.items():
             program = Program(name)
 
             for sec_name, (start, size) in sections.items():
                 if program.base is None:
                     program.base = start
 
-                #in_code_sec = get_section_base_name(sec_name) in INSTRUCTION_SECTION_NAMES
+                # in_code_sec = get_section_base_name(sec_name) in INSTRUCTION_SECTION_NAMES
                 program.add_section(
                     ElfMemorySection(
-                        data[start:start+size], sec_name, program.context,
-                        name, start, MemoryFlags(False, True)
+                        data[start : start + size],
+                        sec_name,
+                        program.context,
+                        name,
+                        start,
+                        MemoryFlags(False, True),
                     )
                 )
 
             program.context.labels.update(debug_info.symbols.get(name, dict()))
             program.global_labels.update(debug_info.globals.get(name, set()))
 
             yield program
 
     def parse_no_debug(self) -> Program:
-        print(FMT_PARSE + "[MemoryImageLoader] Warning: loading memory image without debug information!" + FMT_NONE)
+        print(
+            FMT_PARSE
+            + "[MemoryImageLoader] Warning: loading memory image without debug information!"
+            + FMT_NONE
+        )
 
-        with open(self.source_path, 'rb') as source_file:
+        with open(self.source_path, "rb") as source_file:
             data: bytes = source_file.read()
 
         p = Program(self.filename)
-        p.add_section(ElfMemorySection(
-            bytearray(data), '.text', p.context, p.name, 0, MemoryFlags(False, True)
-        ))
+        p.add_section(
+            ElfMemorySection(
+                bytearray(data), ".text", p.context, p.name, 0, MemoryFlags(False, True)
+            )
+        )
         return p
 
     @classmethod
-    def instantiate(cls, source_path: str, options: T_ParserOpts) -> 'ProgramLoader':
-        if os.path.isfile(source_path + '.dbg'):
-            return MemoryImageLoader(source_path, dict(**options, debug=source_path + '.dbg'))
+    def instantiate(cls, source_path: str, options: T_ParserOpts) -> "ProgramLoader":
+        if os.path.isfile(source_path + ".dbg"):
+            return MemoryImageLoader(
+                source_path, dict(**options, debug=source_path + ".dbg")
+            )
         return MemoryImageLoader(source_path, options)
```

### Comparing `riscemu-2.0.5/riscemu/priv/PrivCPU.py` & `riscemu-2.1.0/riscemu/priv/PrivCPU.py`

 * *Files 27% similar despite different names*

```diff
@@ -83,72 +83,89 @@
         except RiscemuBaseException as ex:
             if isinstance(ex, LaunchDebuggerException):
                 launch_debug = True
                 self.pc += self.INS_XLEN
 
         if self.halted:
             print()
-            print(FMT_CPU + "[CPU] System halted with code {}".format(self.exit_code) + FMT_NONE)
+            print(
+                FMT_CPU
+                + "[CPU] System halted with code {}".format(self.exit_code)
+                + FMT_NONE
+            )
             sys.exit(self.exit_code)
 
         elif launch_debug:
             launch_debug_session(self)
             if not self.debugger_active:
                 self.run(verbose)
         else:
             print()
-            print(FMT_CPU + "[CPU] System stopped without halting - perhaps you stopped the debugger?" + FMT_NONE)
+            print(
+                FMT_CPU
+                + "[CPU] System stopped without halting - perhaps you stopped the debugger?"
+                + FMT_NONE
+            )
 
     def launch(self, program: Optional[Program] = None, verbose: bool = False):
-        print(FMT_CPU + '[CPU] Started running from 0x{:08X} ({})'.format(self.pc, "kernel") + FMT_NONE)
+        print(
+            FMT_CPU
+            + "[CPU] Started running from 0x{:08X} ({})".format(self.pc, "kernel")
+            + FMT_NONE
+        )
         self._time_start = time.perf_counter_ns() // self.TIME_RESOLUTION_NS
 
         self.run(self.conf.verbosity > 1 or verbose)
 
     def load_program(self, program: Program):
-        if program.name == 'kernel':
+        if program.name == "kernel":
             self.pc = program.entrypoint
         super().load_program(program)
 
     def _init_csr(self):
         # set up CSR
         self.csr = CSR()
-        self.csr.set('mhartid', UInt32(0))  # core id
+        self.csr.set("mhartid", UInt32(0))  # core id
         # TODO: set correct value
-        self.csr.set('mimpid', UInt32(0))  # implementation id
+        self.csr.set("mimpid", UInt32(0))  # implementation id
         # set mxl to 1 (32 bit) and set bits for i and m isa
-        self.csr.set('misa', UInt32((1 << 30) + (1 << 8) + (1 << 12)))  # available ISA
+        self.csr.set("misa", UInt32((1 << 30) + (1 << 8) + (1 << 12)))  # available ISA
 
         # CSR write callbacks:
 
-        @self.csr.callback('halt')
+        @self.csr.callback("halt")
         def halt(old: UInt32, new: UInt32):
             if new != 0:
                 self.halted = True
                 self.exit_code = new.value
 
-        @self.csr.callback('mtimecmp')
+        @self.csr.callback("mtimecmp")
         def mtimecmp(old: UInt32, new: UInt32):
-            self._time_timecmp = (self.csr.get('mtimecmph') << 32) + new
+            self._time_timecmp = (self.csr.get("mtimecmph") << 32) + new
             self._time_interrupt_enabled = True
 
-        @self.csr.callback('mtimecmph')
+        @self.csr.callback("mtimecmph")
         def mtimecmph(old: UInt32, new: UInt32):
-            self._time_timecmp = (new << 32) + self.csr.get('mtimecmp')
+            self._time_timecmp = (new << 32) + self.csr.get("mtimecmp")
             self._time_interrupt_enabled = True
 
         # virtual CSR registers:
 
-        @self.csr.virtual_register('time')
+        @self.csr.virtual_register("time")
         def get_time():
-            return UInt32(time.perf_counter_ns() // self.TIME_RESOLUTION_NS - self._time_start)
+            return UInt32(
+                time.perf_counter_ns() // self.TIME_RESOLUTION_NS - self._time_start
+            )
 
-        @self.csr.virtual_register('timeh')
+        @self.csr.virtual_register("timeh")
         def get_timeh():
-            return UInt32((time.perf_counter_ns() // self.TIME_RESOLUTION_NS - self._time_start) >> 32)
+            return UInt32(
+                (time.perf_counter_ns() // self.TIME_RESOLUTION_NS - self._time_start)
+                >> 32
+            )
 
         # add minstret and mcycle counters
 
     def _handle_trap(self, trap: CpuTrap):
         # implement trap handling!
         self.pending_traps.append(trap)
 
@@ -156,66 +173,79 @@
         try:
             self.cycle += 1
             if self.cycle % 20 == 0:
                 self._timer_step()
             self._check_interrupt()
             ins = self.mmu.read_ins(self.pc)
             if verbose and (self.mode == PrivModes.USER or self.conf.verbosity > 4):
-                print(FMT_CPU + "   Running 0x{:08X}:{} {}".format(self.pc, FMT_NONE, ins))
+                print(
+                    FMT_CPU + "   Running 0x{:08X}:{} {}".format(self.pc, FMT_NONE, ins)
+                )
             self.run_instruction(ins)
             self.pc += self.INS_XLEN
         except CpuTrap as trap:
             self._handle_trap(trap)
             if trap.interrupt == 0 and not isinstance(trap, EcallTrap):
-                print(FMT_CPU + "[CPU] Trap {} encountered at {} (0x{:x})".format(
-                    trap,
-                    self.mmu.translate_address(self.pc),
-                    self.pc
-                ) + FMT_NONE)
+                print(
+                    FMT_CPU
+                    + "[CPU] Trap {} encountered at {} (0x{:x})".format(
+                        trap, self.mmu.translate_address(self.pc), self.pc
+                    )
+                    + FMT_NONE
+                )
                 breakpoint()
                 if self.conf.debug_on_exception:
                     raise LaunchDebuggerException()
             self.pc += self.INS_XLEN
 
     def _timer_step(self):
         if not self._time_interrupt_enabled:
             return
-        if self._time_timecmp <= (time.perf_counter_ns() // self.TIME_RESOLUTION_NS) - self._time_start:
+        if (
+            self._time_timecmp
+            <= (time.perf_counter_ns() // self.TIME_RESOLUTION_NS) - self._time_start
+        ):
             self.pending_traps.append(TimerInterrupt())
             self._time_interrupt_enabled = False
 
     def _check_interrupt(self):
-        if not (len(self.pending_traps) > 0 and self.csr.get_mstatus('mie')):
+        if not (len(self.pending_traps) > 0 and self.csr.get_mstatus("mie")):
             return
         # select best interrupt
         # FIXME: actually select based on the official ranking
         trap = self.pending_traps.pop()  # use the most recent trap
         if self.conf.verbosity > 0:
             print(FMT_CPU + "[CPU] taking trap {}!".format(trap) + FMT_NONE)
             self.regs.dump_reg_a()
 
         if trap.priv != PrivModes.MACHINE:
-            print(FMT_CPU + "[CPU] Trap not targeting machine mode encountered! - undefined behaviour!" + FMT_NONE)
+            print(
+                FMT_CPU
+                + "[CPU] Trap not targeting machine mode encountered! - undefined behaviour!"
+                + FMT_NONE
+            )
             raise Exception("Undefined behaviour!")
 
         if self.mode != PrivModes.USER:
             print(FMT_CPU + "[CPU] Trap triggered outside of user mode?!" + FMT_NONE)
 
-        self.csr.set_mstatus('mpie', self.csr.get_mstatus('mie'))
-        self.csr.set_mstatus('mpp', self.mode.value)
-        self.csr.set_mstatus('mie', UInt32(0))
-        self.csr.set('mcause', trap.mcause)
-        self.csr.set('mepc', self.pc - self.INS_XLEN)
-        self.csr.set('mtval', trap.mtval)
+        self.csr.set_mstatus("mpie", self.csr.get_mstatus("mie"))
+        self.csr.set_mstatus("mpp", self.mode.value)
+        self.csr.set_mstatus("mie", UInt32(0))
+        self.csr.set("mcause", trap.mcause)
+        self.csr.set("mepc", self.pc - self.INS_XLEN)
+        self.csr.set("mtval", trap.mtval)
         self.mode = trap.priv
-        mtvec = self.csr.get('mtvec')
+        mtvec = self.csr.get("mtvec")
         if mtvec & 0b11 == 0:
             self.pc = mtvec.value
         if mtvec & 0b11 == 1:
-            self.pc = ((mtvec & 0b11111111111111111111111111111100) + (trap.code * 4)).value
+            self.pc = (
+                (mtvec & 0b11111111111111111111111111111100) + (trap.code * 4)
+            ).value
         self.record_perf_profile()
         if len(self._perf_counters) > 100:
             self.show_perf()
 
     def show_perf(self):
         timed = 0
         cycled = 0
@@ -228,18 +258,19 @@
                 timed = time_ns
                 continue
             cps = (cycle - cycled) / (time_ns - timed) * 1000000000
 
             cycled = cycle
             timed = time_ns
             cps_list.append(cps)
-        print("    on average {:.0f} instructions/s".format(sum(cps_list) / len(cps_list)) + FMT_NONE)
+        print(
+            "    on average {:.0f} instructions/s".format(sum(cps_list) / len(cps_list))
+            + FMT_NONE
+        )
         self._perf_counters = list()
 
     def record_perf_profile(self):
         self._perf_counters.append((time.perf_counter_ns(), self.cycle))
 
     @classmethod
     def get_loaders(cls) -> typing.Iterable[Type[ProgramLoader]]:
-        return [
-            AssemblyFileLoader, MemoryImageLoader, ElfBinaryFileLoader
-        ]
+        return [AssemblyFileLoader, MemoryImageLoader, ElfBinaryFileLoader]
```

### Comparing `riscemu-2.0.5/riscemu/priv/PrivMMU.py` & `riscemu-2.1.0/riscemu/priv/PrivMMU.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,47 @@
 import typing
 
 if typing.TYPE_CHECKING:
     from .PrivCPU import PrivCPU
 
 
 class PrivMMU(MMU):
-
     def get_sec_containing(self, addr: T_AbsoluteAddress) -> MemorySection:
         # try to get an existing section
         existing_sec = super().get_sec_containing(addr)
 
         if existing_sec is not None:
             return existing_sec
 
         # get section preceding empty space at addr
-        sec_before = next((sec for sec in reversed(self.sections) if sec.end < addr), None)
+        sec_before = next(
+            (sec for sec in reversed(self.sections) if sec.end < addr), None
+        )
         # get sec succeeding empty space at addr
         sec_after = next((sec for sec in self.sections if sec.base > addr), None)
 
         # calc start end end of "free" space
         prev_sec_end = 0 if sec_before is None else sec_before.end
         next_sec_start = 0x7FFFFFFF if sec_after is None else sec_after.base
 
         # start at the end of the prev section, or current address - 0xFFFF (aligned to 16 byte boundary)
         start = max(prev_sec_end, align_addr(addr - 0xFFFF, 16))
         # end at the start of the next section, or address + 0xFFFF (aligned to 16 byte boundary)
         end = min(next_sec_start, align_addr(addr + 0xFFFF, 16))
 
-        sec = ElfMemorySection(bytearray(end - start), '.empty', self.global_instruction_context(), '', start, MemoryFlags(False, True))
+        sec = ElfMemorySection(
+            bytearray(end - start),
+            ".empty",
+            self.global_instruction_context(),
+            "",
+            start,
+            MemoryFlags(False, True),
+        )
         self.sections.append(sec)
         self._update_state()
 
         return sec
 
     def global_instruction_context(self) -> InstructionContext:
         context = InstructionContext()
         context.global_symbol_dict = self.global_symbols
-        return context
+        return context
```

### Comparing `riscemu-2.0.5/riscemu/priv/PrivRV32I.py` & `riscemu-2.1.0/riscemu/priv/PrivRV32I.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,160 +12,164 @@
 import typing
 
 if typing.TYPE_CHECKING:
     from riscemu.priv.PrivCPU import PrivCPU
 
 
 class PrivRV32I(RV32I):
-    cpu: 'PrivCPU'
+    cpu: "PrivCPU"
     """
     This is an extension of RV32I, written for the PrivCPU class
     """
 
-    def instruction_csrrw(self, ins: 'Instruction'):
+    def instruction_csrrw(self, ins: "Instruction"):
         rd, rs, csr_addr = self.parse_crs_ins(ins)
         old_val = None
-        if rd != 'zero':
+        if rd != "zero":
             self.cpu.csr.assert_can_read(self.cpu.mode, csr_addr)
             old_val = self.cpu.csr.get(csr_addr)
-        if rs != 'zero':
+        if rs != "zero":
             new_val = self.regs.get(rs)
             self.cpu.csr.assert_can_write(self.cpu.mode, csr_addr)
             self.cpu.csr.set(csr_addr, new_val)
         if old_val is not None:
             self.regs.set(rd, old_val)
 
-    def instruction_csrrs(self, ins: 'Instruction'):
+    def instruction_csrrs(self, ins: "Instruction"):
         rd, rs, csr_addr = self.parse_crs_ins(ins)
-        if rs != 'zero':
+        if rs != "zero":
             # oh no, this should not happen!
             INS_NOT_IMPLEMENTED(ins)
-        if rd != 'zero':
+        if rd != "zero":
             self.cpu.csr.assert_can_read(self.cpu.mode, csr_addr)
             old_val = self.cpu.csr.get(csr_addr)
             self.regs.set(rd, old_val)
 
-    def instruction_csrrc(self, ins: 'Instruction'):
+    def instruction_csrrc(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_csrrsi(self, ins: 'Instruction'):
+    def instruction_csrrsi(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_csrrwi(self, ins: 'Instruction'):
+    def instruction_csrrwi(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         rd, imm, addr = ins.get_reg(0), ins.get_imm(1), ins.get_imm(2)
-        if rd != 'zero':
+        if rd != "zero":
             self.cpu.csr.assert_can_read(self.cpu.mode, addr)
             old_val = self.cpu.csr.get(addr)
             self.regs.set(rd, old_val)
         self.cpu.csr.assert_can_write(self.cpu.mode, addr)
         self.cpu.csr.set(addr, imm)
 
-    def instruction_csrrci(self, ins: 'Instruction'):
+    def instruction_csrrci(self, ins: "Instruction"):
         INS_NOT_IMPLEMENTED(ins)
 
-    def instruction_mret(self, ins: 'Instruction'):
+    def instruction_mret(self, ins: "Instruction"):
         if self.cpu.mode != PrivModes.MACHINE:
             print("MRET not inside machine level code!")
             raise IllegalInstructionTrap(ins)
         # retore mie
-        mpie = self.cpu.csr.get_mstatus('mpie')
-        self.cpu.csr.set_mstatus('mie', mpie)
+        mpie = self.cpu.csr.get_mstatus("mpie")
+        self.cpu.csr.set_mstatus("mie", mpie)
         # restore priv
-        mpp = self.cpu.csr.get_mstatus('mpp')
+        mpp = self.cpu.csr.get_mstatus("mpp")
         self.cpu.mode = PrivModes(mpp)
         # restore pc
-        mepc = self.cpu.csr.get('mepc')
+        mepc = self.cpu.csr.get("mepc")
         self.cpu.pc = (mepc - self.cpu.INS_XLEN).value
 
         if self.cpu.conf.verbosity > 0:
             sec = self.mmu.get_sec_containing(mepc.value)
             if sec is not None:
-                print(FMT_CPU + "[CPU] returning to mode {} in {} (0x{:x})".format(
-                    PrivModes(mpp).name,
-                    self.mmu.translate_address(mepc),
-                    mepc
-                ) + FMT_NONE)
+                print(
+                    FMT_CPU
+                    + "[CPU] returning to mode {} in {} (0x{:x})".format(
+                        PrivModes(mpp).name, self.mmu.translate_address(mepc), mepc
+                    )
+                    + FMT_NONE
+                )
                 if self.cpu.conf.verbosity > 1:
                     self.regs.dump_reg_a()
 
-    def instruction_uret(self, ins: 'Instruction'):
+    def instruction_uret(self, ins: "Instruction"):
         raise IllegalInstructionTrap(ins)
 
-    def instruction_sret(self, ins: 'Instruction'):
+    def instruction_sret(self, ins: "Instruction"):
         raise IllegalInstructionTrap(ins)
 
-    def instruction_scall(self, ins: 'Instruction'):
+    def instruction_scall(self, ins: "Instruction"):
         """
         Overwrite the scall from userspace RV32I
         """
         raise EcallTrap(self.cpu.mode)
 
-    def instruction_beq(self, ins: 'Instruction'):
+    def instruction_beq(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 == rs2:
             self.pc += dst.value - 4
 
-    def instruction_bne(self, ins: 'Instruction'):
+    def instruction_bne(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 != rs2:
             self.pc += dst.value - 4
 
-    def instruction_blt(self, ins: 'Instruction'):
+    def instruction_blt(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 < rs2:
             self.pc += dst.value - 4
 
-    def instruction_bge(self, ins: 'Instruction'):
+    def instruction_bge(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins)
         if rs1 >= rs2:
             self.pc += dst.value - 4
 
-    def instruction_bltu(self, ins: 'Instruction'):
+    def instruction_bltu(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins, signed=False)
         if rs1 < rs2:
             self.pc += dst.value - 4
 
-    def instruction_bgeu(self, ins: 'Instruction'):
+    def instruction_bgeu(self, ins: "Instruction"):
         rs1, rs2, dst = self.parse_rs_rs_imm(ins, signed=False)
         if rs1 >= rs2:
             self.pc += dst.value - 4
 
     # technically deprecated
-    def instruction_j(self, ins: 'Instruction'):
+    def instruction_j(self, ins: "Instruction"):
         raise NotImplementedError("Should never be reached!")
 
-    def instruction_jal(self, ins: 'Instruction'):
+    def instruction_jal(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 2)
         reg = ins.get_reg(0)
         addr = ins.get_imm(1)
-        if reg == 'ra' and (
-                (self.cpu.mode == PrivModes.USER and self.cpu.conf.verbosity > 1) or
-                (self.cpu.conf.verbosity > 3)
+        if reg == "ra" and (
+            (self.cpu.mode == PrivModes.USER and self.cpu.conf.verbosity > 1)
+            or (self.cpu.conf.verbosity > 3)
         ):
-            print(FMT_CPU + 'Jumping from 0x{:x} to {} (0x{:x})'.format(
-                self.pc,
-                self.mmu.translate_address(self.pc + addr),
-                self.pc + addr
-            ) + FMT_NONE)
+            print(
+                FMT_CPU
+                + "Jumping from 0x{:x} to {} (0x{:x})".format(
+                    self.pc, self.mmu.translate_address(self.pc + addr), self.pc + addr
+                )
+                + FMT_NONE
+            )
             self.regs.dump_reg_a()
         self.regs.set(reg, Int32(self.pc))
         self.pc += addr - 4
 
-    def instruction_jalr(self, ins: 'Instruction'):
+    def instruction_jalr(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         rd, rs, imm = self.parse_rd_rs_imm(ins)
         self.regs.set(rd, Int32(self.pc))
         self.pc = rs.value + imm.value - 4
 
-    def instruction_sbreak(self, ins: 'Instruction'):
+    def instruction_sbreak(self, ins: "Instruction"):
         raise LaunchDebuggerException()
 
-    def parse_crs_ins(self, ins: 'Instruction'):
+    def parse_crs_ins(self, ins: "Instruction"):
         ASSERT_LEN(ins.args, 3)
         return ins.get_reg(0), ins.get_reg(1), ins.get_imm(2)
 
-    def parse_mem_ins(self, ins: 'Instruction') -> Tuple[str, int]:
+    def parse_mem_ins(self, ins: "Instruction") -> Tuple[str, int]:
         ASSERT_LEN(ins.args, 3)
         addr = self.get_reg_content(ins, 1) + ins.get_imm(2)
         reg = ins.get_reg(0)
         return reg, addr
```

### Comparing `riscemu-2.0.5/riscemu/priv/__main__.py` & `riscemu-2.1.0/riscemu/priv/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,62 @@
 from riscemu import RunConfig
 from riscemu.types import Program
 from .PrivCPU import PrivCPU
 
 import sys
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import argparse
 
-    parser = argparse.ArgumentParser(description='RISC-V privileged architecture emulator', prog='riscemu')
-
-    parser.add_argument('source', type=str,
-                        help='Compiled RISC-V ELF file or memory image containing compiled RISC-V ELF files', nargs='+')
-    parser.add_argument('--debug-exceptions', help='Launch the interactive debugger when an exception is generated',
-                        action='store_true')
-
-    parser.add_argument('-v', '--verbose', help="Verbosity level (can be used multiple times)", action='count',
-                        default=0)
-
-    parser.add_argument('--slowdown', help="Slow down the emulated CPU clock by a factor", type=float, default=1)
+    parser = argparse.ArgumentParser(
+        description="RISC-V privileged architecture emulator", prog="riscemu"
+    )
+
+    parser.add_argument(
+        "source",
+        type=str,
+        help="Compiled RISC-V ELF file or memory image containing compiled RISC-V ELF files",
+        nargs="+",
+    )
+    parser.add_argument(
+        "--debug-exceptions",
+        help="Launch the interactive debugger when an exception is generated",
+        action="store_true",
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        help="Verbosity level (can be used multiple times)",
+        action="count",
+        default=0,
+    )
+
+    parser.add_argument(
+        "--slowdown",
+        help="Slow down the emulated CPU clock by a factor",
+        type=float,
+        default=1,
+    )
 
     args = parser.parse_args()
 
-    cpu = PrivCPU(RunConfig(verbosity=args.verbose, debug_on_exception=args.debug_exceptions, slowdown=args.slowdown))
+    cpu = PrivCPU(
+        RunConfig(
+            verbosity=args.verbose,
+            debug_on_exception=args.debug_exceptions,
+            slowdown=args.slowdown,
+        )
+    )
 
     for source_path in args.source:
-        loader = max((loader for loader in cpu.get_loaders()), key=lambda l: l.can_parse(source_path))
+        loader = max(
+            (loader for loader in cpu.get_loaders()),
+            key=lambda l: l.can_parse(source_path),
+        )
         argv, opts = loader.get_options(sys.argv)
         program = loader.instantiate(source_path, opts).parse()
         if isinstance(program, Program):
             cpu.load_program(program)
         else:
             program_iter = program
             for program in program_iter:
```

### Comparing `riscemu-2.0.5/riscemu/priv/types.py` & `riscemu-2.1.0/riscemu/priv/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,27 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import Tuple, Dict, Set
 
 from riscemu.colors import FMT_NONE, FMT_PARSE
 from riscemu.decoder import format_ins, RISCV_REGS, decode
-from riscemu.priv.Exceptions import InstructionAccessFault, InstructionAddressMisalignedTrap, LoadAccessFault
-from riscemu.types import Instruction, InstructionContext, T_RelativeAddress, MemoryFlags, T_AbsoluteAddress, \
-    BinaryDataMemorySection
+from riscemu.priv.Exceptions import (
+    InstructionAccessFault,
+    InstructionAddressMisalignedTrap,
+    LoadAccessFault,
+)
+from riscemu.types import (
+    Instruction,
+    InstructionContext,
+    T_RelativeAddress,
+    MemoryFlags,
+    T_AbsoluteAddress,
+    BinaryDataMemorySection,
+)
 
 
 @dataclass(frozen=True)
 class ElfInstruction(Instruction):
     name: str
     args: Tuple[int]
     encoded: int
@@ -23,52 +33,63 @@
     def get_imm_reg(self, num: int) -> Tuple[int, int]:
         return self.args[-1], self.args[-2]
 
     def get_reg(self, num: int) -> str:
         return RISCV_REGS[self.args[num]]
 
     def __repr__(self) -> str:
-        if self.name == 'jal' and self.args[0] == 0:
+        if self.name == "jal" and self.args[0] == 0:
             return "j       {}".format(self.args[1])
-        if self.name == 'addi' and self.args[2] == 0:
+        if self.name == "addi" and self.args[2] == 0:
             return "mv      {}, {}".format(self.get_reg(0), self.get_reg(1))
-        if self.name == 'addi' and self.args[1] == 0:
+        if self.name == "addi" and self.args[1] == 0:
             return "li      {}, {}".format(self.get_reg(0), self.args[2])
-        if self.name == 'ret' and len(self.args) == 0:
+        if self.name == "ret" and len(self.args) == 0:
             return "ret"
         return format_ins(self.encoded, self.name)
 
 
 class ElfMemorySection(BinaryDataMemorySection):
-    def __init__(self, data: bytearray, name: str, context: InstructionContext, owner: str, base: int,
-                 flags: MemoryFlags):
+    def __init__(
+        self,
+        data: bytearray,
+        name: str,
+        context: InstructionContext,
+        owner: str,
+        base: int,
+        flags: MemoryFlags,
+    ):
         super().__init__(data, name, context, owner, base=base, flags=flags)
         self.read_ins = lru_cache(maxsize=self.size // 4)(self.read_ins)
 
     def read_ins(self, offset):
         if not self.flags.executable:
-            print(FMT_PARSE + "Reading instruction from non-executable memory!" + FMT_NONE)
+            print(
+                FMT_PARSE + "Reading instruction from non-executable memory!" + FMT_NONE
+            )
             raise InstructionAccessFault(offset + self.base)
         if offset % 4 != 0:
             raise InstructionAddressMisalignedTrap(offset + self.base)
-        return ElfInstruction(*decode(self.data[offset:offset + 4]))
+        return ElfInstruction(*decode(self.data[offset : offset + 4]))
 
     def write(self, offset: T_RelativeAddress, size: int, data: bytearray):
         if self.flags.read_only:
-            raise LoadAccessFault('read-only section', offset + self.base, size, 'write')
+            raise LoadAccessFault(
+                "read-only section", offset + self.base, size, "write"
+            )
         self.read_ins.cache_clear()
         return super(ElfMemorySection, self).write(offset, size, data)
 
     @property
     def end(self):
         return self.size + self.base
 
 
 class MemoryImageDebugInfos:
-    VERSION = '1.0.0'
+    VERSION = "1.0.0"
     """
     Schema version
     """
 
     base: T_AbsoluteAddress = 0
     """
     The base address where the image starts. Defaults to zero.
@@ -85,63 +106,69 @@
     """
 
     globals: Dict[str, Set[str]]
     """
     This dictionary contains the list of all global symbols of a given program
     """
 
-    def __init__(self,
-                 sections: Dict[str, Dict[str, Tuple[int, int]]],
-                 symbols: Dict[str, Dict[str, int]],
-                 globals: Dict[str, Set[str]],
-                 base: int = 0
-                 ):
+    def __init__(
+        self,
+        sections: Dict[str, Dict[str, Tuple[int, int]]],
+        symbols: Dict[str, Dict[str, int]],
+        globals: Dict[str, Set[str]],
+        base: int = 0,
+    ):
         self.sections = sections
         self.symbols = symbols
         self.globals = globals
         for name in globals:
             globals[name] = set(globals[name])
         self.base = base
 
     def serialize(self) -> str:
         def serialize(obj: any) -> str:
             if isinstance(obj, defaultdict):
                 return json.dumps(dict(obj), default=serialize)
             if isinstance(obj, (set, tuple)):
                 return json.dumps(list(obj), default=serialize)
-            return "<<unserializable {}>>".format(getattr(obj, '__qualname__', '{unknown}'))
+            return "<<unserializable {}>>".format(
+                getattr(obj, "__qualname__", "{unknown}")
+            )
 
         return json.dumps(
             dict(
                 sections=self.sections,
                 symbols=self.symbols,
                 globals=self.globals,
                 base=self.base,
-                VERSION=self.VERSION
+                VERSION=self.VERSION,
             ),
-            default=serialize
+            default=serialize,
         )
 
     @classmethod
-    def load(cls, serialized_str: str) -> 'MemoryImageDebugInfos':
+    def load(cls, serialized_str: str) -> "MemoryImageDebugInfos":
         json_obj: dict = json.loads(serialized_str)
 
-        if 'VERSION' not in json_obj:
+        if "VERSION" not in json_obj:
             raise RuntimeError("Unknown MemoryImageDebugInfo version!")
 
-        version: str = json_obj.pop('VERSION')
+        version: str = json_obj.pop("VERSION")
 
         # compare major version
-        if version != cls.VERSION and version.split('.')[0] != cls.VERSION.split('.')[0]:
+        if (
+            version != cls.VERSION
+            and version.split(".")[0] != cls.VERSION.split(".")[0]
+        ):
             raise RuntimeError(
                 "Unknown MemoryImageDebugInfo version! This emulator expects version {}, debug info version {}".format(
                     cls.VERSION, version
                 )
             )
 
         return MemoryImageDebugInfos(**json_obj)
 
     @classmethod
-    def builder(cls) -> 'MemoryImageDebugInfos':
+    def builder(cls) -> "MemoryImageDebugInfos":
         return MemoryImageDebugInfos(
             defaultdict(dict), defaultdict(dict), defaultdict(set)
         )
```

### Comparing `riscemu-2.0.5/riscemu/tokenizer.py` & `riscemu-2.1.0/riscemu/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import List, Iterable
 
 from riscemu.decoder import RISCV_REGS
 from riscemu.types.exceptions import ParseException
 
-LINE_COMMENT_STARTERS = ('#', ';', '//')
-WHITESPACE_PATTERN = re.compile(r'\s+')
-MEMORY_ADDRESS_PATTERN = re.compile(r'^(0[xX][A-f0-9]+|\d+|0b[0-1]+|[A-z0-9_-]+)\(([A-z]+[0-9]{0,2})\)$')
+LINE_COMMENT_STARTERS = ("#", ";", "//")
+WHITESPACE_PATTERN = re.compile(r"\s+")
+MEMORY_ADDRESS_PATTERN = re.compile(
+    r"^(0[xX][A-f0-9]+|\d+|0b[0-1]+|[A-z0-9_-]+)\(([A-z]+[0-9]{0,2})\)$"
+)
 REGISTER_NAMES = RISCV_REGS
 
 
 class TokenType(Enum):
     COMMA = auto()
     ARGUMENT = auto()
     PSEUDO_OP = auto()
@@ -30,62 +32,62 @@
 @dataclass(frozen=True)
 class Token:
     type: TokenType
     value: str
 
     def __str__(self):
         if self.type == TokenType.NEWLINE:
-            return '\\n'
+            return "\\n"
         if self.type == TokenType.COMMA:
-            return ', '
-        return '{}({})'.format(self.type.name[0:3], self.value)
+            return ", "
+        return "{}({})".format(self.type.name[0:3], self.value)
 
 
-NEWLINE = Token(TokenType.NEWLINE, '\n')
-COMMA = Token(TokenType.COMMA, ',')
+NEWLINE = Token(TokenType.NEWLINE, "\n")
+COMMA = Token(TokenType.COMMA, ",")
 
 
 def tokenize(input: Iterable[str]) -> Iterable[Token]:
     for line in input:
         for line_comment_start in LINE_COMMENT_STARTERS:
             if line_comment_start in line:
-                line = line[:line.index(line_comment_start)]
-        line.strip(' \t\n')
+                line = line[: line.index(line_comment_start)]
+        line.strip(" \t\n")
         if not line:
             continue
 
         parts = list(part for part in split_whitespace_respecting_quotes(line) if part)
 
         yield from parse_line(parts)
         yield NEWLINE
 
 
 def parse_line(parts: List[str]) -> Iterable[Token]:
     if len(parts) == 0:
         return ()
     first_token = parts[0]
 
-    if first_token[0] == '.':
+    if first_token[0] == ".":
         yield Token(TokenType.PSEUDO_OP, first_token)
-    elif first_token[-1] == ':':
+    elif first_token[-1] == ":":
         yield Token(TokenType.LABEL, first_token)
         yield from parse_line(parts[1:])
         return
     else:
         yield Token(TokenType.INSTRUCTION_NAME, first_token)
 
     for part in parts[1:]:
-        if part == ',':
+        if part == ",":
             yield COMMA
             continue
         yield from parse_arg(part)
 
 
 def parse_arg(arg: str) -> Iterable[Token]:
-    comma = arg[-1] == ','
+    comma = arg[-1] == ","
     arg = arg[:-1] if comma else arg
     mem_match_resul = re.match(MEMORY_ADDRESS_PATTERN, arg)
     if mem_match_resul:
         register = mem_match_resul.group(2).lower()
         if register not in RISCV_REGS:
             raise ParseException(f'"{register}" is not a valid register!')
         yield Token(TokenType.ARGUMENT, register)
@@ -94,15 +96,15 @@
         yield Token(TokenType.ARGUMENT, arg)
     if comma:
         yield COMMA
 
 
 def print_tokens(tokens: Iterable[Token]):
     for token in tokens:
-        print(token, end='\n' if token == NEWLINE else '')
+        print(token, end="\n" if token == NEWLINE else "")
     print("", flush=True, end="")
 
 
 def split_whitespace_respecting_quotes(line: str) -> Iterable[str]:
     quote = ""
     part = ""
     for c in line:
@@ -119,15 +121,15 @@
         if c in "\"'":
             if part:
                 yield part
             quote = c
             part = ""
             continue
 
-        if c in ' \t\n':
+        if c in " \t\n":
             if part:
                 yield part
             part = ""
             continue
 
         part += c
```

### Comparing `riscemu-2.0.5/riscemu/types/__init__.py` & `riscemu-2.1.0/riscemu/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,41 @@
-from typing import Dict
+from typing import Dict, Any
 import re
 
 # define some base type aliases so we can keep track of absolute and relative addresses
 T_RelativeAddress = int
 T_AbsoluteAddress = int
 
 # parser options are just dictionaries with arbitrary values
-T_ParserOpts = Dict[str, any]
+T_ParserOpts = Dict[str, Any]
 
-NUMBER_SYMBOL_PATTERN = re.compile(r'^\d+[fb]$')
+NUMBER_SYMBOL_PATTERN = re.compile(r"^\d+[fb]$")
 
 # base classes
 from .flags import MemoryFlags
 from .int32 import UInt32, Int32
+from .float32 import Float32
 from .instruction import Instruction
 from .instruction_context import InstructionContext
 from .memory_section import MemorySection
 from .program import Program
 from .program_loader import ProgramLoader
 from .cpu import CPU
 from .simple_instruction import SimpleInstruction
 from .instruction_memory_section import InstructionMemorySection
 from .binary_data_memory_section import BinaryDataMemorySection
 
 # exceptions
-from .exceptions import ParseException, NumberFormatException, MemoryAccessException, OutOfMemoryException, \
-    LinkerException, LaunchDebuggerException, RiscemuBaseException, InvalidRegisterException, \
-    InvalidAllocationException, InvalidSyscallException, UnimplementedInstruction
+from .exceptions import (
+    ParseException,
+    NumberFormatException,
+    MemoryAccessException,
+    OutOfMemoryException,
+    LinkerException,
+    LaunchDebuggerException,
+    RiscemuBaseException,
+    InvalidRegisterException,
+    InvalidAllocationException,
+    InvalidSyscallException,
+    UnimplementedInstruction,
+    INS_NOT_IMPLEMENTED,
+)
```

### Comparing `riscemu-2.0.5/riscemu/types/cpu.py` & `riscemu-2.1.0/riscemu/types/cpu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-import typing
 from abc import ABC, abstractmethod
-from typing import List, Type, Callable, Set, Dict
+from typing import List, Type, Callable, Set, Dict, TYPE_CHECKING, Iterable
 
 from ..registers import Registers
 from ..config import RunConfig
-from ..colors import FMT_RED, FMT_NONE, FMT_ERROR, FMT_CPU
+from ..colors import FMT_NONE, FMT_CPU
 from . import T_AbsoluteAddress, Instruction, Program, ProgramLoader
 
+if TYPE_CHECKING:
+    from ..MMU import MMU
+    from ..instructions import InstructionSet
+
 
 class CPU(ABC):
     # static cpu configuration
     INS_XLEN: int = 4
 
     # housekeeping variables
     regs: Registers
-    mmu: 'MMU'
+    mmu: "MMU"
     pc: T_AbsoluteAddress
     cycle: int
     halted: bool
 
     # debugging context
     debugger_active: bool
 
     # instruction information
     instructions: Dict[str, Callable[[Instruction], None]]
-    instruction_sets: Set['InstructionSet']
+    instruction_sets: Set["InstructionSet"]
 
     # configuration
     conf: RunConfig
 
-    def __init__(self, mmu: 'MMU', instruction_sets: List[Type['InstructionSet']], conf: RunConfig):
+    def __init__(
+        self,
+        mmu: "MMU",
+        instruction_sets: List[Type["InstructionSet"]],
+        conf: RunConfig,
+    ):
         self.mmu = mmu
         self.regs = Registers(conf.unlimited_registers)
         self.conf = conf
 
         self.instruction_sets = set()
         self.instructions = dict()
 
@@ -67,40 +75,45 @@
         Returns a representation of the CPU and some of its state.
         """
         return "{}(pc=0x{:08X}, cycle={}, halted={} instructions={})".format(
             self.__class__.__name__,
             self.pc,
             self.cycle,
             self.halted,
-            " ".join(s.name for s in self.instruction_sets)
+            " ".join(s.name for s in self.instruction_sets),
         )
 
     @abstractmethod
-    def step(self, verbose=False):
+    def step(self, verbose: bool = False):
         pass
 
     @abstractmethod
-    def run(self, verbose=False):
+    def run(self, verbose: bool = False):
         pass
 
-    def launch(self, program: Program, verbose: bool = False):
-        if program not in self.mmu.programs:
-            print(FMT_ERROR + '[CPU] Cannot launch program that\'s not loaded!' + FMT_NONE)
-            return
+    def launch(self, verbose: bool = False):
+        entrypoint = self.mmu.find_entrypoint()
+
+        if entrypoint is None:
+            entrypoint = self.mmu.programs[0].entrypoint
+
         if self.conf.verbosity > 0:
-            print(FMT_CPU + "[CPU] Started running from {}".format(
-                self.mmu.translate_address(program.entrypoint)
-            ) + FMT_NONE)
-            print(program)
-        self.pc = program.entrypoint
+            print(
+                FMT_CPU
+                + "[CPU] Started running from {}".format(
+                    self.mmu.translate_address(entrypoint)
+                )
+                + FMT_NONE
+            )
+        self.pc = entrypoint
         self.run(verbose)
 
     @classmethod
     @abstractmethod
-    def get_loaders(cls) -> typing.Iterable[Type[ProgramLoader]]:
+    def get_loaders(cls) -> Iterable[Type[ProgramLoader]]:
         pass
 
     def get_best_loader_for(self, file_name: str) -> Type[ProgramLoader]:
         return max(self.get_loaders(), key=lambda ld: ld.can_parse(file_name))
 
     @property
     def sections(self):
```

### Comparing `riscemu-2.0.5/riscemu/types/exceptions.py` & `riscemu-2.1.0/riscemu/types/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,165 +10,191 @@
 
 if typing.TYPE_CHECKING:
     from . import Instruction
 
 
 class RiscemuBaseException(BaseException):
     @abstractmethod
-    def message(self):
-        pass
+    def message(self) -> str:
+        raise NotImplemented
 
     def print_stacktrace(self):
         import traceback
+
         traceback.print_exception(type(self), self, self.__traceback__)
 
+
 # Parsing exceptions:
 
+
 class ParseException(RiscemuBaseException):
-    def __init__(self, msg, data=None):
+    def __init__(self, msg: str, data=None):
         super().__init__(msg, data)
         self.msg = msg
         self.data = data
 
     def message(self):
-        return FMT_PARSE + "{}(\"{}\", data={})".format(self.__class__.__name__, self.msg, self.data) + FMT_NONE
+        return (
+            FMT_PARSE
+            + '{}("{}", data={})'.format(self.__class__.__name__, self.msg, self.data)
+            + FMT_NONE
+        )
 
 
 def ASSERT_EQ(a1, a2):
     if a1 != a2:
-        raise ParseException("ASSERTION_FAILED: Expected elements to be equal!", (a1, a2))
+        raise ParseException(
+            "ASSERTION_FAILED: Expected elements to be equal!", (a1, a2)
+        )
 
 
 def ASSERT_LEN(a1, size):
     if len(a1) != size:
-        raise ParseException("ASSERTION_FAILED: Expected {} to be of length {}".format(a1, size), (a1, size))
+        raise ParseException(
+            "ASSERTION_FAILED: Expected {} to be of length {}".format(a1, size),
+            (a1, size),
+        )
 
 
 def ASSERT_NOT_NULL(a1):
     if a1 is None:
-        raise ParseException("ASSERTION_FAILED: Expected {} to be non null".format(a1), (a1,))
+        raise ParseException(
+            "ASSERTION_FAILED: Expected {} to be non null".format(a1), (a1,)
+        )
 
 
 def ASSERT_NOT_IN(a1, a2):
     if a1 in a2:
-        raise ParseException("ASSERTION_FAILED: Expected {} to not be in {}".format(a1, a2), (a1, a2))
+        raise ParseException(
+            "ASSERTION_FAILED: Expected {} to not be in {}".format(a1, a2), (a1, a2)
+        )
 
 
 def ASSERT_IN(a1, a2):
     if a1 not in a2:
-        raise ParseException("ASSERTION_FAILED: Expected {} to not be in {}".format(a1, a2), (a1, a2))
+        raise ParseException(
+            "ASSERTION_FAILED: Expected {} to not be in {}".format(a1, a2), (a1, a2)
+        )
 
 
 class LinkerException(RiscemuBaseException):
-    def __init__(self, msg, data):
+    def __init__(self, msg: str, data):
         self.msg = msg
         self.data = data
 
     def message(self):
-        return FMT_PARSE + "{}(\"{}\", data={})".format(self.__class__.__name__, self.msg, self.data) + FMT_NONE
+        return (
+            FMT_PARSE
+            + '{}("{}", data={})'.format(self.__class__.__name__, self.msg, self.data)
+            + FMT_NONE
+        )
 
 
 # MMU Exceptions
 
+
 class MemoryAccessException(RiscemuBaseException):
-    def __init__(self, msg, addr, size, op):
+    def __init__(self, msg: str, addr, size, op):
         super(MemoryAccessException, self).__init__()
         self.msg = msg
         self.addr = addr
         self.size = size
         self.op = op
 
     def message(self):
-        return FMT_MEM + "{}(During {} at 0x{:08x} of size {}: {})".format(
-            self.__class__.__name__,
-            self.op,
-            self.addr,
-            self.size,
-            self.msg
-        ) + FMT_NONE
+        return (
+            FMT_MEM
+            + "{}(During {} at 0x{:08x} of size {}: {})".format(
+                self.__class__.__name__, self.op, self.addr, self.size, self.msg
+            )
+            + FMT_NONE
+        )
 
 
 class OutOfMemoryException(RiscemuBaseException):
     def __init__(self, action):
         self.action = action
 
     def message(self):
-        return FMT_MEM + '{}(Ran out of memory during {})'.format(
-            self.__class__.__name__,
-            self.action
-        ) + FMT_NONE
+        return (
+            FMT_MEM
+            + "{}(Ran out of memory during {})".format(
+                self.__class__.__name__, self.action
+            )
+            + FMT_NONE
+        )
 
 
 class InvalidAllocationException(RiscemuBaseException):
     def __init__(self, msg, name, size, flags):
         self.msg = msg
         self.name = name
         self.size = size
         self.flags = flags
 
     def message(self):
-        return FMT_MEM + '{}[{}](name={}, size={}, flags={})'.format(
-            self.__class__.__name__,
-            self.msg,
-            self.name,
-            self.size,
-            self.flags
+        return FMT_MEM + "{}[{}](name={}, size={}, flags={})".format(
+            self.__class__.__name__, self.msg, self.name, self.size, self.flags
         )
 
+
 # CPU Exceptions
 
 
 class UnimplementedInstruction(RiscemuBaseException):
-    def __init__(self, ins: 'Instruction', context = None):
+    def __init__(self, ins: "Instruction", context=None):
         self.ins = ins
         self.context = context
 
     def message(self):
-        return FMT_CPU + "{}({}{})".format(
-            self.__class__.__name__,
-            repr(self.ins),
-            ', context={}'.format(self.context) if self.context is not None else ''
-        ) + FMT_NONE
+        return (
+            FMT_CPU
+            + "{}({}{})".format(
+                self.__class__.__name__,
+                repr(self.ins),
+                ", context={}".format(self.context) if self.context is not None else "",
+            )
+            + FMT_NONE
+        )
 
 
 class InvalidRegisterException(RiscemuBaseException):
     def __init__(self, reg):
         self.reg = reg
 
     def message(self):
-        return FMT_CPU + "{}(Invalid register {})".format(
-            self.__class__.__name__,
-            self.reg
-        ) + FMT_NONE
+        return (
+            FMT_CPU
+            + "{}(Invalid register {})".format(self.__class__.__name__, self.reg)
+            + FMT_NONE
+        )
 
 
 class InvalidSyscallException(RiscemuBaseException):
     def __init__(self, scall):
         self.scall = scall
 
     def message(self):
-        return FMT_SYSCALL + "{}(Invalid syscall: {})".format(
-            self.__class__.__name__,
-            self.scall
-        ) + FMT_NONE
+        return (
+            FMT_SYSCALL
+            + "{}(Invalid syscall: {})".format(self.__class__.__name__, self.scall)
+            + FMT_NONE
+        )
 
 
 def INS_NOT_IMPLEMENTED(ins):
     raise UnimplementedInstruction(ins)
 
 
 class NumberFormatException(RiscemuBaseException):
     def __init__(self, msg):
         super().__init__()
         self.msg = msg
 
     def message(self):
-        return "{}({})".format(
-            self.__class__.__name__,
-            self.msg
-        )
+        return "{}({})".format(self.__class__.__name__, self.msg)
 
 
 # this exception is not printed and simply signals that an interactive debugging session is
 class LaunchDebuggerException(RiscemuBaseException):
-    def message(self):
+    def message(self) -> str:
         return ""
```

### Comparing `riscemu-2.0.5/riscemu/types/instruction.py` & `riscemu-2.1.0/riscemu/types/instruction.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.0.5/riscemu/types/instruction_context.py` & `riscemu-2.1.0/riscemu/types/instruction_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,40 +14,51 @@
     labels: Dict[str, T_RelativeAddress]
     """
     This dictionary maps all labels to their relative position of the instruction block
     """
 
     numbered_labels: Dict[str, List[T_RelativeAddress]]
     """
-    This dictionary maps numbered labels (which can occur multiple times) to a list of (block-relative) addresses where 
-    the label was placed 
+    This dictionary maps numbered labels (which can occur multiple times) to a list of (block-relative) addresses where
+    the label was placed
     """
 
     global_symbol_dict: Dict[str, T_AbsoluteAddress]
     """
     A reference to the MMU's global symbol dictionary for access to global symbols
     """
 
     def __init__(self):
         self.labels = dict()
         self.numbered_labels = defaultdict(list)
         self.base_address = 0
         self.global_symbol_dict = dict()
 
-    def resolve_label(self, symbol: str, address_at: Optional[T_RelativeAddress] = None) -> Optional[T_AbsoluteAddress]:
+    def resolve_label(
+        self, symbol: str, address_at: Optional[T_RelativeAddress] = None
+    ) -> Optional[T_AbsoluteAddress]:
         if NUMBER_SYMBOL_PATTERN.match(symbol):
             if address_at is None:
-                raise ParseException("Cannot resolve relative symbol {} without an address!".format(symbol))
+                raise ParseException(
+                    "Cannot resolve relative symbol {} without an address!".format(
+                        symbol
+                    )
+                )
 
             direction = symbol[-1]
             values = self.numbered_labels.get(symbol[:-1], [])
-            if direction == 'b':
-                return max((addr + self.base_address for addr in values if addr < address_at), default=None)
+            if direction == "b":
+                return max(
+                    (addr + self.base_address for addr in values if addr < address_at),
+                    default=None,
+                )
             else:
-                return min((addr + self.base_address for addr in values if addr > address_at), default=None)
+                return min(
+                    (addr + self.base_address for addr in values if addr > address_at),
+                    default=None,
+                )
         else:
             # if it's not a local symbol, try the globals
             if symbol not in self.labels:
                 return self.global_symbol_dict.get(symbol, None)
             # otherwise return the local symbol
             return self.labels.get(symbol, None)
-
```

### Comparing `riscemu-2.0.5/riscemu/types/instruction_memory_section.py` & `riscemu-2.1.0/riscemu/types/instruction_memory_section.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,54 @@
 from typing import List
 
-from . import MemorySection, Instruction, InstructionContext, MemoryFlags, T_RelativeAddress
+from . import (
+    MemorySection,
+    Instruction,
+    InstructionContext,
+    MemoryFlags,
+    T_RelativeAddress,
+)
 from .exceptions import MemoryAccessException
 
 
 class InstructionMemorySection(MemorySection):
-    def __init__(self, instructions: List[Instruction], name: str, context: InstructionContext, owner: str, base: int = 0):
+    def __init__(
+        self,
+        instructions: List[Instruction],
+        name: str,
+        context: InstructionContext,
+        owner: str,
+        base: int = 0,
+    ):
         self.name = name
         self.base = base
         self.context = context
         self.size = len(instructions) * 4
         self.flags = MemoryFlags(True, True)
         self.instructions = instructions
         self.owner = owner
 
     def read(self, offset: T_RelativeAddress, size: int) -> bytearray:
-        raise MemoryAccessException("Cannot read raw bytes from instruction section", self.base + offset, size, 'read')
+        raise MemoryAccessException(
+            "Cannot read raw bytes from instruction section",
+            self.base + offset,
+            size,
+            "read",
+        )
 
     def write(self, offset: T_RelativeAddress, size: int, data: bytearray):
-        raise MemoryAccessException("Cannot write raw bytes to instruction section", self.base + offset, size, 'write')
+        raise MemoryAccessException(
+            "Cannot write raw bytes to instruction section",
+            self.base + offset,
+            size,
+            "write",
+        )
 
     def read_ins(self, offset: T_RelativeAddress) -> Instruction:
         if offset % 4 != 0:
-            raise MemoryAccessException("Unaligned instruction fetch!", self.base + offset, 4, 'instruction fetch')
+            raise MemoryAccessException(
+                "Unaligned instruction fetch!",
+                self.base + offset,
+                4,
+                "instruction fetch",
+            )
         return self.instructions[offset // 4]
-
```

### Comparing `riscemu-2.0.5/riscemu/types/int32.py` & `riscemu-2.1.0/riscemu/types/int32.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,209 @@
-from typing import Union
+from typing import Any, Union
 from ctypes import c_int32, c_uint32
 
 
 class Int32:
     """
     This class implements 32bit signed integers (see :class:`UInt32` for unsigned integers)
 
     It implements basically all mathematical dunder magic methods (__add__, __sub__, etc.)
 
     You can use it just like you would any other integer, just be careful when passing it
     to functions which actually expect an integer and not a Int32.
     """
+
     _type = c_int32
-    __slots__ = ('_val',)
+    __slots__ = ("_val",)
 
-    def __init__(self, val: Union[int, c_int32, c_uint32, 'Int32', bytes, bytearray] = 0):
+    def __init__(
+        self, val: Union[int, c_int32, c_uint32, "Int32", bytes, bytearray, bool] = 0
+    ):
         if isinstance(val, (bytes, bytearray)):
             signed = len(val) == 4 and self._type == c_int32
-            self._val = self.__class__._type(int.from_bytes(val, 'little', signed=signed))
+            self._val = self.__class__._type(
+                int.from_bytes(val, "little", signed=signed)
+            )
         elif isinstance(val, self.__class__._type):
             self._val = val
         elif isinstance(val, (c_uint32, c_int32, Int32)):
             self._val = self.__class__._type(val.value)
-        elif isinstance(val, int):
+        elif isinstance(val, (int, bool)):
             self._val = self.__class__._type(val)
         else:
             raise RuntimeError(
-                "Unknonw {} input type: {} ({})".format(self.__class__.__name__, type(val), val)
+                "Unknonw {} input type: {} ({})".format(
+                    self.__class__.__name__, type(val), val
+                )
             )
 
-    def __add__(self, other: Union['Int32', int]):
+    def __add__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
 
         return self.__class__(self._val.value + other)
 
-    def __sub__(self, other: Union['Int32', int]):
+    def __sub__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self._val.value - other)
 
-    def __mul__(self, other: Union['Int32', int]):
+    def __mul__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self._val.value * other)
 
-    def __truediv__(self, other):
+    def __truediv__(self, other: Any):
         return self // other
 
-    def __floordiv__(self, other):
+    def __floordiv__(self, other: Any):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self.value // other)
 
-    def __mod__(self, other: Union['Int32', int]):
+    def __mod__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self._val.value % other)
 
-    def __and__(self, other: Union['Int32', int]):
+    def __and__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self._val.value & other)
 
-    def __or__(self, other: Union['Int32', int]):
+    def __or__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self._val.value | other)
 
-    def __xor__(self, other: Union['Int32', int]):
+    def __xor__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self._val.value ^ other)
 
-    def __lshift__(self, other: Union['Int32', int]):
+    def __lshift__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self.value << other)
 
-    def __rshift__(self, other: Union['Int32', int]):
+    def __rshift__(self, other: Union["Int32", int]):
         if isinstance(other, Int32):
             other = other.value
         return self.__class__(self.value >> other)
 
-    def __eq__(self, other: Union['Int32', int]):
-        if isinstance(other, Int32):
-            other = other.value
-        return self.value == other
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, int):
+            return self.value == other
+        elif isinstance(other, Int32):
+            return self.value == other.value
+        return False
 
     def __neg__(self):
         return self.__class__(-self._val.value)
 
     def __abs__(self):
         return self.__class__(abs(self.value))
 
     def __bytes__(self):
         return self.to_bytes(4)
 
     def __repr__(self):
-        return '{}({})'.format(self.__class__.__name__, self.value)
+        return "{}({})".format(self.__class__.__name__, self.value)
 
     def __str__(self):
         return str(self.value)
 
-    def __format__(self, format_spec):
+    def __format__(self, format_spec: str):
         return self.value.__format__(format_spec)
 
     def __hash__(self):
         return hash(self.value)
 
-    def __gt__(self, other):
+    def __gt__(self, other: Any):
         if isinstance(other, Int32):
             other = other.value
         return self.value > other
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any):
         if isinstance(other, Int32):
             other = other.value
         return self.value < other
 
-    def __le__(self, other):
+    def __le__(self, other: Any):
         if isinstance(other, Int32):
             other = other.value
         return self.value <= other
 
-    def __ge__(self, other):
+    def __ge__(self, other: Any):
         if isinstance(other, Int32):
             other = other.value
         return self.value >= other
 
     def __bool__(self):
         return bool(self.value)
 
-    def __cmp__(self, other):
+    def __cmp__(self, other: Any):
         if isinstance(other, Int32):
             other = other.value
         return self.value.__cmp__(other)
 
     # right handed binary operators
 
-    def __radd__(self, other):
+    def __radd__(self, other: Any):
         return self + other
 
-    def __rsub__(self, other):
+    def __rsub__(self, other: Any):
         return self.__class__(other) - self
 
-    def __rmul__(self, other):
+    def __rmul__(self, other: Any):
         return self * other
 
-    def __rtruediv__(self, other):
+    def __rtruediv__(self, other: Any):
         return self.__class__(other) // self
 
-    def __rfloordiv__(self, other):
+    def __rfloordiv__(self, other: Any):
         return self.__class__(other) // self
 
-    def __rmod__(self, other):
+    def __rmod__(self, other: Any):
         return self.__class__(other) % self
 
-    def __rand__(self, other):
+    def __rand__(self, other: Any):
         return self.__class__(other) & self
 
-    def __ror__(self, other):
+    def __ror__(self, other: Any):
         return self.__class__(other) | self
 
-    def __rxor__(self, other):
+    def __rxor__(self, other: Any):
         return self.__class__(other) ^ self
 
     @property
     def value(self) -> int:
         """
         The value represented by this Integer
         :return:
         """
         return self._val.value
 
-    def unsigned(self) -> 'UInt32':
+    def unsigned(self) -> "UInt32":
         """
         Convert to an unsigned representation. See :class:Uint32
         :return:
         """
         return UInt32(self)
 
     def to_bytes(self, bytes: int = 4) -> bytearray:
         """
         Convert to a bytearray of length :param:bytes
 
         :param bytes: The length of the bytearray
         :return: A little-endian representation of the contained integer
         """
-        return bytearray(self.unsigned_value.to_bytes(4, 'little'))[0:bytes]
+        return bytearray(self.unsigned_value.to_bytes(4, "little"))[0:bytes]
 
-    def signed(self) -> 'Int32':
+    def signed(self) -> "Int32":
         """
         Convert to a signed representation. See :class:Int32
         :return:
         """
         if self.__class__ == Int32:
             return self
         return Int32(self)
@@ -203,15 +212,15 @@
     def unsigned_value(self):
         """
         Return the value interpreted as an unsigned integer
         :return:
         """
         return c_uint32(self.value).value
 
-    def shift_right_logical(self, ammount: Union['Int32', int]) -> 'Int32':
+    def shift_right_logical(self, ammount: Union["Int32", int]) -> "Int32":
         """
         This function implements logical right shifts, meaning that the sign bit is shifted as well.
 
         This is equivalent to (self.value % 0x100000000) >> ammount
 
         :param ammount: Number of positions to shift
         :return: A new Int32 object representing the shifted value (keeps the signed-ness of the source)
@@ -233,41 +242,44 @@
         to 32 bits
 
         :param data: The source data
         :param bits: The number of bits in the source data
         :return: An instance of Int32, holding the sign-extended value
         """
         if isinstance(data, (bytes, bytearray)):
-            data = int.from_bytes(data, 'little')
+            data = int.from_bytes(data, "little")
         sign = data >> (bits - 1)
         if sign > 1:
             print("overflow in Int32.sext!")
         if sign:
-            data = (data & (2 ** (bits - 1) - 1)) - 2**(bits-1)
+            data = (data & (2 ** (bits - 1) - 1)) - 2 ** (bits - 1)
         return cls(data)
 
 
 class UInt32(Int32):
     """
     An unsigned version of :class:Int32.
     """
+
     _type = c_uint32
 
-    def unsigned(self) -> 'UInt32':
+    def unsigned(self) -> "UInt32":
         """
         Return a new instance representing the same bytes, but signed
         :return:
         """
         return self
 
     @property
     def unsigned_value(self) -> int:
         return self._val.value
 
-    def shift_right_logical(self, ammount: Union['Int32', int]) -> 'UInt32':
+    def shift_right_logical(self, ammount: Union["Int32", int]) -> "UInt32":
         """
         see :meth:`Int32.shift_right_logical <Int32.shift_right_logical>`
 
         :param ammount: Number of positions to shift
         :return: A new Int32 object representing the shifted value (keeps the signed-ness of the source)
         """
-        return self >> ammount
+        if isinstance(ammount, Int32):
+            ammount = ammount.value
+        return UInt32(self.value >> ammount)
```

### Comparing `riscemu-2.0.5/riscemu/types/memory_section.py` & `riscemu-2.1.0/riscemu/types/memory_section.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional
 
 from ..colors import FMT_MEM, FMT_NONE, FMT_UNDERLINE, FMT_ORANGE, FMT_ERROR
 from ..helpers import format_bytes
-from . import MemoryFlags, T_AbsoluteAddress, InstructionContext, T_RelativeAddress, Instruction, Int32
+from . import (
+    MemoryFlags,
+    T_AbsoluteAddress,
+    InstructionContext,
+    T_RelativeAddress,
+    Instruction,
+    Int32,
+)
 
 
 @dataclass
 class MemorySection(ABC):
     name: str
     flags: MemoryFlags
     size: int
@@ -28,16 +35,24 @@
     def write(self, offset: T_RelativeAddress, size: int, data: bytearray):
         pass
 
     @abstractmethod
     def read_ins(self, offset: T_RelativeAddress) -> Instruction:
         pass
 
-    def dump(self, start: T_RelativeAddress, end: Optional[T_RelativeAddress] = None, fmt: str = None,
-             bytes_per_row: int = None, rows: int = 10, group: int = None, highlight: int = None):
+    def dump(
+        self,
+        start: T_RelativeAddress,
+        end: Optional[T_RelativeAddress] = None,
+        fmt: Optional[str] = None,
+        bytes_per_row: Optional[int] = None,
+        rows: int = 10,
+        group: Optional[int] = None,
+        highlight: Optional[int] = None,
+    ):
         """
         Dump the section. If no end is given, the rows around start are printed and start is highlighted.
 
         :param start: The address to start at
         :param end: The end of the printed space
         :param fmt: either hex, int, char or asm
         :param bytes_per_row: the number of bytes displayed per row
@@ -50,77 +65,109 @@
             start = start.value
         if isinstance(end, Int32):
             end = end.value
 
         if fmt is None:
             if self.flags.executable and self.flags.read_only:
                 bytes_per_row = 4
-                fmt = 'asm'
+                fmt = "asm"
             else:
-                fmt = 'hex'
+                fmt = "hex"
 
-        if fmt == 'char':
+        if fmt == "char":
             if bytes_per_row is None:
                 bytes_per_row = 4
             if group is None:
                 group = 1
 
         if group is None:
             group = 4
 
         if bytes_per_row is None:
             bytes_per_row = 4
 
-        if fmt not in ('asm', 'hex', 'int', 'char'):
-            print(FMT_ERROR + '[MemorySection] Unknown format {}, known formats are {}'.format(
-                fmt, ", ".join(('asm', 'hex', 'int', 'char'))
-            ) + FMT_NONE)
+        if fmt not in ("asm", "hex", "int", "char"):
+            print(
+                FMT_ERROR
+                + "[MemorySection] Unknown format {}, known formats are {}".format(
+                    fmt, ", ".join(("asm", "hex", "int", "char"))
+                )
+                + FMT_NONE
+            )
 
         if end is None:
             end = min(start + (bytes_per_row * (rows // 2)), self.size)
             highlight = start
             start = max(0, start - (bytes_per_row * (rows // 2)))
 
-        if fmt == 'asm':
-            print(FMT_MEM + "{}, viewing {} instructions:".format(
-                self, (end - start) // 4
-            ) + FMT_NONE)
+        if fmt == "asm":
+            print(
+                FMT_MEM
+                + "{}, viewing {} instructions:".format(self, (end - start) // 4)
+                + FMT_NONE
+            )
 
             for addr in range(start, end, 4):
                 if addr == highlight:
-                    print(FMT_UNDERLINE + FMT_ORANGE, end='')
-                print("0x{:04x}: {}{}".format(
-                    self.base + addr, self.read_ins(addr), FMT_NONE
-                ))
+                    print(FMT_UNDERLINE + FMT_ORANGE, end="")
+                print(
+                    "0x{:04x}: {}{}".format(
+                        self.base + addr, self.read_ins(addr), FMT_NONE
+                    )
+                )
         else:
-            print(FMT_MEM + "{}, viewing {} bytes:".format(
-                self, (end - start)
-            ) + FMT_NONE)
-
-            aligned_end = end - (end % bytes_per_row) if end % bytes_per_row != 0 else end
+            print(
+                FMT_MEM + "{}, viewing {} bytes:".format(self, (end - start)) + FMT_NONE
+            )
+
+            aligned_end = (
+                end - (end % bytes_per_row) if end % bytes_per_row != 0 else end
+            )
 
             for addr in range(start, aligned_end, bytes_per_row):
                 hi_ind = (highlight - addr) // group if highlight is not None else -1
-                print("0x{:04x}: {}{}".format(
-                    self.base + addr, format_bytes(self.read(addr, bytes_per_row), fmt, group, hi_ind), FMT_NONE
-                ))
+                print(
+                    "0x{:04x}: {}{}".format(
+                        self.base + addr,
+                        format_bytes(
+                            self.read(addr, bytes_per_row), fmt, group, hi_ind
+                        ),
+                        FMT_NONE,
+                    )
+                )
 
             if aligned_end != end:
-                hi_ind = (highlight - aligned_end) // group if highlight is not None else -1
-                print("0x{:04x}: {}{}".format(
-                    self.base + aligned_end, format_bytes(
-                        self.read(aligned_end, end % bytes_per_row), fmt, group, hi_ind
-                    ), FMT_NONE
-                ))
-
-    def dump_all(self, *args, **kwargs):
-        self.dump(0, self.size, *args, **kwargs)
+                hi_ind = (
+                    (highlight - aligned_end) // group if highlight is not None else -1
+                )
+                print(
+                    "0x{:04x}: {}{}".format(
+                        self.base + aligned_end,
+                        format_bytes(
+                            self.read(aligned_end, end % bytes_per_row),
+                            fmt,
+                            group,
+                            hi_ind,
+                        ),
+                        FMT_NONE,
+                    )
+                )
+
+    def dump_all(
+        self,
+        fmt: Optional[str] = None,
+        bytes_per_row: Optional[int] = None,
+        rows: int = 10,
+        group: Optional[int] = None,
+        highlight: Optional[int] = None,
+    ):
+        self.dump(0, self.size, fmt, bytes_per_row, rows, group, highlight)
 
     def __repr__(self):
         return "{}[{}] at 0x{:08X} (size={}bytes, flags={}, owner={})".format(
             self.__class__.__name__,
             self.name,
             self.base,
             self.size,
             self.flags,
-            self.owner
+            self.owner,
         )
```

### Comparing `riscemu-2.0.5/riscemu/types/program.py` & `riscemu-2.1.0/riscemu/types/program.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     This represents a collection of sections which together form an executable program
 
     When you want to create a program which can be located anywhere in memory, set base to None,
     this signals the other components, that this is relocatable. Set the base of each section to
     the offset in the program, and everything will be taken care of for you.
 
     """
+
     name: str
     context: InstructionContext
     global_labels: Set[str]
     relative_labels: Set[str]
     sections: List[MemorySection]
     base: Optional[T_AbsoluteAddress]
     is_loaded: bool
@@ -40,36 +41,43 @@
         self.is_loaded = False
 
     def add_section(self, sec: MemorySection):
         # print a warning when a section is located before the programs base
         if self.base is not None:
             if sec.base < self.base:
                 print(
-                    FMT_RED + FMT_BOLD + "WARNING: memory section {} in {} is placed before program base (0x{:x})".format(
+                    FMT_RED
+                    + FMT_BOLD
+                    + "WARNING: memory section {} in {} is placed before program base (0x{:x})".format(
                         sec, self.name, self.base
-                    ) + FMT_NONE)
+                    )
+                    + FMT_NONE
+                )
 
         self.sections.append(sec)
         # keep section list ordered
         self.sections.sort(key=lambda section: section.base)
 
     def __repr__(self):
         return "{}(name={},sections={},base={})".format(
-            self.__class__.__name__, self.name, self.global_labels,
-            [s.name for s in self.sections], self.base
+            self.__class__.__name__,
+            self.name,
+            self.global_labels,
+            [s.name for s in self.sections],
+            self.base,
         )
 
     @property
     def entrypoint(self):
-        if '_start' in self.context.labels:
-            return self.context.labels.get('_start')
-        if 'main' in self.context.labels:
-            return self.context.labels.get('main')
+        if "_start" in self.context.labels:
+            return self.context.labels.get("_start")
+        if "main" in self.context.labels:
+            return self.context.labels.get("main")
         for sec in self.sections:
-            if get_section_base_name(sec.name) == '.text' and sec.flags.executable:
+            if get_section_base_name(sec.name) == ".text" and sec.flags.executable:
                 return sec.base
 
     def loaded_trigger(self, at_addr: T_AbsoluteAddress):
         """
         This trigger is called when the binary is loaded and its final address in memory is determined
 
         This will do a small sanity check to prevent programs loading twice, or at addresses they don't
@@ -77,20 +85,25 @@
 
         Then it will finalize all relative symbols defined in it to point to the correct addresses.
 
         :param at_addr: the address where the program will be located
         """
         if self.is_loaded:
             if at_addr != self.base:
-                raise RuntimeError("Program loaded twice at different addresses! This will probably break things!")
+                raise RuntimeError(
+                    "Program loaded twice at different addresses! This will probably break things!"
+                )
             return
 
         if self.base is not None and self.base != at_addr:
-            print(FMT_MEM + 'WARNING: Program loaded at different address then expected! (loaded at {}, '
-                            'but expects to be loaded at {})'.format(at_addr, self.base) + FMT_NONE)
+            print(
+                FMT_MEM
+                + "WARNING: Program loaded at different address then expected! (loaded at {}, "
+                "but expects to be loaded at {})".format(at_addr, self.base) + FMT_NONE
+            )
 
         # check if we are relocating
         if self.base != at_addr:
             offset = at_addr if self.base is None else at_addr - self.base
 
             # move all sections by the offset
             for sec in self.sections:
```

### Comparing `riscemu-2.0.5/riscemu/types/program_loader.py` & `riscemu-2.1.0/riscemu/types/program_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         :param argv: the command line args list
         :return: all remaining command line args and the parser options object
         """
         pass
 
     @classmethod
-    def instantiate(cls, source_path: str, options: T_ParserOpts) -> 'ProgramLoader':
+    def instantiate(cls, source_path: str, options: T_ParserOpts) -> "ProgramLoader":
         """
         Instantiate a loader for the given source file with the required arguments
 
         :param source_path: the path to the source file
         :param options: the parsed options (guaranteed to come from this classes get_options method.
         :return: An instance of a ProgramLoader for the spcified source
         """
```

### Comparing `riscemu-2.0.5/riscemu/types/simple_instruction.py` & `riscemu-2.1.0/riscemu/types/simple_instruction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from typing import Union, Tuple
 
 from . import Instruction, T_RelativeAddress, InstructionContext
 from ..helpers import parse_numeric_argument
 
 
 class SimpleInstruction(Instruction):
-    def __init__(self, name: str, args: Union[Tuple[()], Tuple[str], Tuple[str, str], Tuple[str, str, str]],
-                 context: InstructionContext, addr: T_RelativeAddress):
+    def __init__(
+        self,
+        name: str,
+        args: Union[Tuple[()], Tuple[str], Tuple[str, str], Tuple[str, str, str]],
+        context: InstructionContext,
+        addr: T_RelativeAddress,
+    ):
         self.context = context
         self.name = name
         self.args = args
         self.addr = addr
 
     def get_imm(self, num: int) -> int:
         resolved_label = self.context.resolve_label(self.args[num], self.addr)
@@ -19,8 +24,7 @@
         return resolved_label
 
     def get_imm_reg(self, num: int) -> Tuple[int, str]:
         return self.get_imm(num + 1), self.get_reg(num)
 
     def get_reg(self, num: int) -> str:
         return self.args[num]
-
```

### Comparing `riscemu-2.0.5/riscemu.egg-info/PKG-INFO` & `riscemu-2.1.0/riscemu.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: riscemu
-Version: 2.0.5
-Summary: RISC-V userspace and privileged emulator
+Version: 2.1.0
+Summary: RISC-V userspace and machine mode emulator
 Home-page: https://github.com/antonlydike/riscemu
 Author: Anton Lydike <Anton@Lydike.com>
 Author-email: pip@antonlydike.de
 Project-URL: Bug Tracker, https://github.com/AntonLydike/riscemu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RiscEmu - RISC-V (userspace) emulator in python
 
 [![Documentation Status](https://readthedocs.org/projects/riscemu/badge/?version=latest)](https://riscemu.readthedocs.io/en/latest/?badge=latest)
 
@@ -21,15 +21,15 @@
 or [riscemu.datenvorr.at](https://riscemu.datenvorr.at/index.html).
 
 This emulator contains:
 * RISC-V Assembly parser
 * RISC-V Assembly loader
 * Emulation for most parts of the basic RISC-V instruction set and the M and A extensions
 * Naive memory emulator
-* Basic implementation of some syscalls 
+* Basic implementation of some syscalls
 * A debugging environment
 
 ## Installation:
 
 ```bash
 $ pip install riscemu
 ```
@@ -44,15 +44,15 @@
 Hello world
 
 Program exited with code 0
 ```
 
 If you want to run it from a python script, here is [an online demo](https://AntonLydike.github.io/riscemu/lab/index.html?path=PythonDemo.ipynb).
 
-The [`read` syscall](docs/syscalls.md) defaults to readline behaviour. Reading "true chunks" (ignoring newlines) is currently not supported.  
+The [`read` syscall](docs/syscalls.md) defaults to readline behaviour. Reading "true chunks" (ignoring newlines) is currently not supported.
 
 See the docs on [asembly](docs/assembly.md) for more detail on how to write assembly code for this emulator.
 See the [list of implemented syscalls](docs/syscalls.md) for more details on how to syscall.
 
 Currently, symbols (such as `main` or `loop`) are looked-up at runtime. This allows for better debugging, I believe.
 
 Basic IO should work, as open, read, write and close are supported for stdin/stdout/stderr and even aribtrary file paths (if enabled)
@@ -82,18 +82,18 @@
                         Options to control syscall behaviour
 fs_access               Allow access to the filesystem
 disable_io              Disallow reading/writing from stdin/stdout/stderr
 
 --instruction-sets INSTRUCTION_SETS: (-is)
                         A list of comma separated instruction sets you want to load:
                         Currently implemented: RV32I, RV32M
-``` 
+```
 
-If multiple files are specified, all are loaded into memeory, but only the last one is executed. This might be improved 
-later, maybe the `_init` section of each binary is executed before the main loop starts? 
+If multiple files are specified, all are loaded into memeory, but only the last one is executed. This might be improved
+later, maybe the `_init` section of each binary is executed before the main loop starts?
 
 If `stack_size` is greater than zero, a stack is allocated and initialized, with the `sp` register pointing to the end of the stack.
 
 
 ## Debugging
 Debugging is done using the `ebreak` (formerly `sbreak`) instruction, which will launch a debugging session if encountered.
 See [docs/debugging.md](docs/debugging.md) for more info.
@@ -101,21 +101,21 @@
 ![debuggin the fibs program](docs/debug-session.png)
 
 
 ## The source code:
 Check out the [documentation](https://riscemu.readthedocs.io/en/latest/riscemu.html).
 
 ## Accessing local documentation:
-To generate your local documentation, first install everything in `sphinx-docs/requirements.txt`. Then run `./generate-docs.sh`, which will 
+To generate your local documentation, first install everything in `sphinx-docs/requirements.txt`. Then run `./generate-docs.sh`, which will
 generate and make all doc files for you. Finally, you can open the docs locall by runnint `open sphinx-docs/build/html/index.html`.
 
 ## Resources:
+  * RISC-V Programmers Handbook: https://github.com/riscv-non-isa/riscv-asm-manual/blob/master/riscv-asm.md
   * Pseudo ops: https://www.codetd.com/article/8981522
   * detailed instruction definition: https://msyksphinz-self.github.io/riscv-isadoc/html/rvi.html#add
   * RISC-V reference card: https://www.cl.cam.ac.uk/teaching/1617/ECAD+Arch/files/docs/RISCVGreenCardv8-20151013.pdf
-  
+
 ## TODO:
  * Correctly handle 12 and 20 bit immediate (currently not limited to bits at all)
  * Add a cycle limit to the options and CPU to catch infinite loops
  * Move away from `print` and use `logging.logger` instead
  * Writer proper tests
-
```

### Comparing `riscemu-2.0.5/riscemu.egg-info/SOURCES.txt` & `riscemu-2.1.0/riscemu.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 ./riscemu/assembler.py
 ./riscemu/colors.py
 ./riscemu/config.py
 ./riscemu/debug.py
 ./riscemu/helpers.py
 ./riscemu/interactive.py
 ./riscemu/parser.py
+./riscemu/py.typed
 ./riscemu/registers.py
+./riscemu/riscemu_main.py
 ./riscemu/syscall.py
 ./riscemu/tokenizer.py
 ./riscemu/IO/IOModule.py
 ./riscemu/IO/TextIO.py
 ./riscemu/IO/__init__.py
 ./riscemu/decoder/__init__.py
 ./riscemu/decoder/__main__.py
 ./riscemu/decoder/decoder.py
 ./riscemu/decoder/formats.py
 ./riscemu/decoder/formatter.py
 ./riscemu/decoder/instruction_table.py
 ./riscemu/decoder/regs.py
 ./riscemu/instructions/RV32A.py
+./riscemu/instructions/RV32F.py
 ./riscemu/instructions/RV32I.py
 ./riscemu/instructions/RV32M.py
+./riscemu/instructions/RV_Debug.py
 ./riscemu/instructions/__init__.py
 ./riscemu/instructions/instruction_set.py
 ./riscemu/priv/CSR.py
 ./riscemu/priv/CSRConsts.py
 ./riscemu/priv/ElfLoader.py
 ./riscemu/priv/Exceptions.py
 ./riscemu/priv/ImageLoader.py
@@ -43,24 +47,31 @@
 ./riscemu/priv/privmodes.py
 ./riscemu/priv/types.py
 ./riscemu/types/__init__.py
 ./riscemu/types/binary_data_memory_section.py
 ./riscemu/types/cpu.py
 ./riscemu/types/exceptions.py
 ./riscemu/types/flags.py
+./riscemu/types/float32.py
 ./riscemu/types/instruction.py
 ./riscemu/types/instruction_context.py
 ./riscemu/types/instruction_memory_section.py
 ./riscemu/types/int32.py
 ./riscemu/types/memory_section.py
 ./riscemu/types/program.py
 ./riscemu/types/program_loader.py
 ./riscemu/types/simple_instruction.py
+libc/crt0.s
+libc/stdlib.s
+libc/string.s
 riscemu.egg-info/PKG-INFO
 riscemu.egg-info/SOURCES.txt
 riscemu.egg-info/dependency_links.txt
 riscemu.egg-info/requires.txt
 riscemu.egg-info/top_level.txt
+riscemu/tools/riscemu
+test/test_float32.py
 test/test_helpers.py
 test/test_integers.py
 test/test_isa.py
+test/test_regs.py
 test/test_tokenizer.py
```

### Comparing `riscemu-2.0.5/setup.py` & `riscemu-2.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 import setuptools
+from glob import glob
 
 import riscemu
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="riscemu",
     version=riscemu.__version__,
     author=riscemu.__author__,
     author_email="pip@antonlydike.de",
-    description="RISC-V userspace and privileged emulator",
+    description="RISC-V userspace and machine mode emulator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/antonlydike/riscemu",
     project_urls={
         "Bug Tracker": "https://github.com/AntonLydike/riscemu/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "."},
-    packages=["riscemu", "riscemu.decoder", "riscemu.instructions", "riscemu.IO", "riscemu.priv", "riscemu.types"],
-    python_requires=">=3.6",
-    install_requires=[
-        "pyelftools~=0.27"
-    ]
-)
+    packages=[
+        "riscemu",
+        "riscemu.decoder",
+        "riscemu.instructions",
+        "riscemu.IO",
+        "riscemu.priv",
+        "riscemu.types",
+    ],
+    package_data={
+        "riscemu": ["libc/*.s", "py.typed"],
+    },
+    data_files=[
+        ('libc', glob('libc/*.s')),
+    ],
+    scripts=["riscemu/tools/riscemu"],
+    python_requires=">=3.8",
+    install_requires=["pyelftools~=0.27"],
+)
```

### Comparing `riscemu-2.0.5/test/test_isa.py` & `riscemu-2.1.0/test/test_isa.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,42 +34,48 @@
     a = ins.args[num]
     if a in RISCV_REGS:
         return cpu.regs.get(a)
     return ins.get_imm(num)
 
 
 assert_ops = {
-    '==': assert_equals,
-    '!=': _not(assert_equals),
-    'in': assert_in,
-    'not_in': _not(assert_in),
+    "==": assert_equals,
+    "!=": _not(assert_equals),
+    "in": assert_in,
+    "not_in": _not(assert_in),
 }
 
 
-class TestIS(InstructionSet):
-    def __init__(self, cpu: 'CPU'):
-        print('[Test] loading testing ISA, this is only meant for running testcases and is not part of the RISC-V ISA!')
+class Z_test(InstructionSet):
+    def __init__(self, cpu: "CPU"):
+        print(
+            "[Test] loading testing ISA, this is only meant for running testcases and is not part of the RISC-V ISA!"
+        )
         self.failed = False
         super().__init__(cpu)
 
     def instruction_assert(self, ins: Instruction):
         if len(ins.args) < 3:
-            print(FMT_ERROR + '[Test] Unknown assert statement: {}'.format(ins) + FMT_NONE)
+            print(
+                FMT_ERROR + "[Test] Unknown assert statement: {}".format(ins) + FMT_NONE
+            )
             return
         op = ins.args[1]
         if op not in assert_ops:
-            print(FMT_ERROR + '[Test] Unknown operation statement: {} in {}'.format(op, ins) + FMT_NONE)
+            print(
+                FMT_ERROR
+                + "[Test] Unknown operation statement: {} in {}".format(op, ins)
+                + FMT_NONE
+            )
             return
 
         if assert_ops[op](ins, self.cpu):
-            print(FMT_SUCCESS + '[TestCase] 🟢 passed assertion {}'.format(ins))
+            print(FMT_SUCCESS + "[TestCase] 🟢 passed assertion {}".format(ins))
         else:
-            print(FMT_ERROR + '[TestCase] 🔴 failed assertion {}'.format(ins))
+            print(FMT_ERROR + "[TestCase] 🔴 failed assertion {}".format(ins))
             self.cpu.halted = True
             self.failed = True
 
     def instruction_fail(self, ins: Instruction):
-            print(FMT_ERROR + '[TestCase] 🔴 reached fail instruction! {}'.format(ins))
-            self.cpu.halted = True
-            self.failed = True
-
-    def assert_mem(self, ins: Instruction):
+        print(FMT_ERROR + "[TestCase] 🔴 reached fail instruction! {}".format(ins))
+        self.cpu.halted = True
+        self.failed = True
```

